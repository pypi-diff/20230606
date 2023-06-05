# Comparing `tmp/parsl-2023.5.8.tar.gz` & `tmp/parsl-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2023.5.8.tar", last modified: Mon May  8 22:42:47 2023, max compression
+gzip compressed data, was "parsl-2023.6.5.tar", last modified: Mon Jun  5 22:43:11 2023, max compression
```

## Comparing `parsl-2023.5.8.tar` & `parsl-2023.6.5.tar`

### file list

```diff
@@ -1,475 +1,472 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 22:42:42.000000 parsl-2023.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-08 22:42:42.000000 parsl-2023.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-08 22:42:47.564188 parsl-2023.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-08 22:42:42.000000 parsl-2023.5.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/cooley.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/cori.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/exex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/configs/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/data_provider/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62334 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/executor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/flow_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/job_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/executors/extreme_scale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/extreme_scale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/extreme_scale/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18710 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/extreme_scale/mpi_worker_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.540188 parsl-2023.5.8/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    33199 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33007 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/status_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/swift_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.544188 parsl-2023.5.8/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29073 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/serialize/facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.548188 parsl-2023.5.8/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/cori.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/exex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/workqueue_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.552188 parsl-2023.5.8/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_start_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_file_bug_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_checkpointing/test_task_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_data/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_data/test_file_staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.556188 parsl-2023.5.8/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_workflow3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_htex_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_htex_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_htex_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_flowcontrol/test_one_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_flowcontrol/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_manual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_manual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_manual/test_regression_220.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_monitoring/test_memoization_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_providers/test_local_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.560188 parsl-2023.5.8/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_at_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_type5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_python_apps/test_worker_fail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_69b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_97.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_scaling/test_scale_down.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_staging/test_staging_https_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/test_threads/test_lazy_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/tests/workqueue_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3835 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/tests/workqueue_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.564188 parsl-2023.5.8/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-05-08 22:42:42.000000 parsl-2023.5.8/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-08 22:42:46.000000 parsl-2023.5.8/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:42:47.536188 parsl-2023.5.8/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 22:42:47.000000 parsl-2023.5.8/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 22:42:42.000000 parsl-2023.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 22:42:47.564188 parsl-2023.5.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-05-08 22:42:42.000000 parsl-2023.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.190580 parsl-2023.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 22:43:01.000000 parsl-2023.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 22:43:01.000000 parsl-2023.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 22:43:11.190580 parsl-2023.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-05 22:43:01.000000 parsl-2023.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.122580 parsl-2023.6.5/parsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.130580 parsl-2023.6.5/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/cooley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/cori.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/exex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.130580 parsl-2023.6.5/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62269 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/job_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/executors/extreme_scale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/extreme_scale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/extreme_scale/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18710 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/extreme_scale/mpi_worker_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.138580 parsl-2023.6.5/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33191 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33011 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/status_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/swift_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.138580 parsl-2023.6.5/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48137 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.138580 parsl-2023.6.5/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29073 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.154580 parsl-2023.6.5/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.158580 parsl-2023.6.5/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/cori.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/exex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/workqueue_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.158580 parsl-2023.6.5/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.158580 parsl-2023.6.5/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_regression_220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_start_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_task_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_file_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_output_chain_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_memoization_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_viz_colouring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.174580 parsl-2023.6.5/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_providers/test_local_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.178580 parsl-2023.6.5/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_at_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_type5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_worker_fail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.182580 parsl-2023.6.5/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_69b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_97_parallelism_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.182580 parsl-2023.6.5/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_scaling/test_regression_1621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_scaling/test_scale_down.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.186580 parsl-2023.6.5/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_https_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.186580 parsl-2023.6.5/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_threads/test_lazy_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.190580 parsl-2023.6.5/parsl/tests/workqueue_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3835 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.190580 parsl-2023.6.5/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-05 22:43:09.000000 parsl-2023.6.5/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.122580 parsl-2023.6.5/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-05 22:43:01.000000 parsl-2023.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 22:43:11.190580 parsl-2023.6.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-06-05 22:43:01.000000 parsl-2023.6.5/setup.py
```

### Comparing `parsl-2023.5.8/LICENSE` & `parsl-2023.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/PKG-INFO` & `parsl-2023.6.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.5.8
+Version: 2023.6.5
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.05.08.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.06.05.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.5.8/README.rst` & `parsl-2023.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/__init__.py` & `parsl-2023.6.5/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/addresses.py` & `parsl-2023.6.5/parsl/addresses.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/app/app.py` & `parsl-2023.6.5/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/app/bash.py` & `parsl-2023.6.5/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/app/futures.py` & `parsl-2023.6.5/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/app/python.py` & `parsl-2023.6.5/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/benchmark/perf.py` & `parsl-2023.6.5/parsl/benchmark/perf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse
 import importlib
 import time
 import concurrent.futures
 import parsl
 
+min_iterations = 2
+
 
 # TODO: factor with conftest.py where this is copy/pasted from?
 def load_dfk_from_config(filename):
     spec = importlib.util.spec_from_file_location('', filename)
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
 
@@ -30,39 +32,39 @@
     delta_t: float
     delta_t = 0
 
     threshold_t = int(0.75 * target_t)
 
     iteration = 1
 
-    while delta_t < threshold_t:
+    while delta_t < threshold_t or iteration <= min_iterations:
         print(f"==== Iteration {iteration} ====")
         print(f"Will run {n} tasks to target {target_t} seconds runtime")
         start_t = time.time()
 
         fs = []
         print("Submitting tasks / invoking apps")
         for _ in range(n):
             fs.append(app(parsl_resource_specification=resources))
 
         submitted_t = time.time()
         print(f"All {n} tasks submitted ... waiting for completion")
-        print(f"Submission took {submitted_t - start_t} seconds = {n/(submitted_t - start_t)} tasks/second")
+        print(f"Submission took {submitted_t - start_t:.3f} seconds = {n/(submitted_t - start_t):.3f} tasks/second")
 
         for f in concurrent.futures.as_completed(fs):
             assert f.result() == 7
 
         end_t = time.time()
 
         delta_t = end_t - start_t
 
         rate = n / delta_t
 
-        print(f"Runtime: {delta_t}s vs target {target_t}")
-        print(f"Tasks per second: {rate}")
+        print(f"Runtime: actual {delta_t:.3f}s vs target {target_t}s")
+        print(f"Tasks per second: {rate:.3f}")
 
         n = int(target_t * rate)
 
         iteration += 1
 
 
 def cli_run() -> None:
```

### Comparing `parsl-2023.5.8/parsl/channels/base.py` & `parsl-2023.6.5/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/channels/errors.py` & `parsl-2023.6.5/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/channels/local/local.py` & `parsl-2023.6.5/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2023.6.5/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/channels/ssh/ssh.py` & `parsl-2023.6.5/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/channels/ssh_il/ssh_il.py` & `parsl-2023.6.5/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/concurrent/__init__.py` & `parsl-2023.6.5/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/config.py` & `parsl-2023.6.5/parsl/config.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/ASPIRE1.py` & `parsl-2023.6.5/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/Azure.py` & `parsl-2023.6.5/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/ad_hoc.py` & `parsl-2023.6.5/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/bluewaters.py` & `parsl-2023.6.5/parsl/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/bridges.py` & `parsl-2023.6.5/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/cc_in2p3.py` & `parsl-2023.6.5/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/comet.py` & `parsl-2023.6.5/parsl/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/cooley.py` & `parsl-2023.6.5/parsl/configs/cooley.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/cori.py` & `parsl-2023.6.5/parsl/configs/cori.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/ec2.py` & `parsl-2023.6.5/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/exex_local.py` & `parsl-2023.6.5/parsl/configs/exex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/frontera.py` & `parsl-2023.6.5/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/illinoiscluster.py` & `parsl-2023.6.5/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/kubernetes.py` & `parsl-2023.6.5/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/midway.py` & `parsl-2023.6.5/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/osg.py` & `parsl-2023.6.5/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/polaris.py` & `parsl-2023.6.5/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/stampede2.py` & `parsl-2023.6.5/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/summit.py` & `parsl-2023.6.5/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/theta.py` & `parsl-2023.6.5/parsl/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/toss3_llnl.py` & `parsl-2023.6.5/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/configs/wqex_local.py` & `parsl-2023.6.5/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/data_provider/data_manager.py` & `parsl-2023.6.5/parsl/data_provider/data_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/data_provider/files.py` & `parsl-2023.6.5/parsl/data_provider/files.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/data_provider/ftp.py` & `parsl-2023.6.5/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/data_provider/globus.py` & `parsl-2023.6.5/parsl/data_provider/globus.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         last_event_time = None
         """
         A Globus transfer job (task) can be in one of the three states: ACTIVE, SUCCEEDED, FAILED.
         Parsl every 15 seconds polls a status of the transfer job (task) from the Globus Transfer service,
         with 60 second timeout limit. If the task is ACTIVE after time runs out 'task_wait' returns False,
         and True otherwise.
         """
-        while not tc.task_wait(task['task_id'], 60, 15):
+        while not tc.task_wait(task['task_id'], timeout=60):
             task = tc.get_task(task['task_id'])
             # Get the last error Globus event
             events = tc.task_event_list(task['task_id'], num_results=1, filter='is_error:1')
             try:
                 event = next(events)
             # No error reported,  the transfer is still running
             except StopIteration:
```

### Comparing `parsl-2023.5.8/parsl/data_provider/http.py` & `parsl-2023.6.5/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/data_provider/rsync.py` & `parsl-2023.6.5/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/data_provider/staging.py` & `parsl-2023.6.5/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/dataflow/dflow.py` & `parsl-2023.6.5/parsl/dataflow/dflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from parsl.app.errors import RemoteExceptionWrapper
 from parsl.app.futures import DataFuture
 from parsl.channels import Channel
 from parsl.config import Config
 from parsl.data_provider.data_manager import DataManager
 from parsl.data_provider.files import File
 from parsl.dataflow.errors import BadCheckpoint, DependencyError, JoinError
-from parsl.dataflow.flow_control import FlowControl
 from parsl.dataflow.futures import AppFuture
+from parsl.dataflow.job_status_poller import JobStatusPoller
 from parsl.dataflow.memoization import Memoizer
 from parsl.dataflow.rundirs import make_rundir
 from parsl.dataflow.states import States, FINAL_STATES, FINAL_FAILURE_STATES
 from parsl.dataflow.taskrecord import TaskRecord
 from parsl.errors import ConfigurationError
 from parsl.usage_tracking.usage import UsageTracker
 from parsl.executors.base import ParslExecutor
@@ -170,18 +170,17 @@
 
         self.memoizer = Memoizer(self, memoize=config.app_cache, checkpoint=checkpoints)
         self.checkpointed_tasks = 0
         self._checkpoint_timer = None
         self.checkpoint_mode = config.checkpoint_mode
         self.checkpointable_tasks: List[TaskRecord] = []
 
-        # the flow control keeps track of executors and provider task states;
-        # must be set before executors are added since add_executors calls
-        # flowcontrol.add_executors.
-        self.flowcontrol = FlowControl(self)
+        # this must be set before executors are added since add_executors calls
+        # job_status_poller.add_executors.
+        self.job_status_poller = JobStatusPoller(self)
 
         self.executors: Dict[str, ParslExecutor] = {}
 
         self.data_manager = DataManager(self)
         parsl_internal_executor = ThreadPoolExecutor(max_threads=config.internal_tasks_max_threads, label='_parsl_internal')
         self.add_executors(config.executors)
         self.add_executors([parsl_internal_executor])
@@ -1118,15 +1117,15 @@
             if self.monitoring and block_ids:
                 new_status = {}
                 for bid in block_ids:
                     new_status[bid] = JobStatus(JobState.PENDING)
                 msg = executor.create_monitoring_info(new_status)
                 logger.debug("Sending monitoring message {} to hub from DFK".format(msg))
                 self.monitoring.send(MessageType.BLOCK_INFO, msg)
-        self.flowcontrol.add_executors(executors)
+        self.job_status_poller.add_executors(executors)
 
     def atexit_cleanup(self) -> None:
         if not self.cleanup_called:
             logger.info("DFK cleanup because python process is exiting")
             self.cleanup()
         else:
             logger.info("python process is exiting, but DFK has already been cleaned up")
@@ -1180,17 +1179,17 @@
                 logger.info("Stopping checkpoint timer")
                 self._checkpoint_timer.close()
 
         # Send final stats
         self.usage_tracker.send_message()
         self.usage_tracker.close()
 
-        logger.info("Closing flowcontrol")
-        self.flowcontrol.close()
-        logger.info("Terminated flow control")
+        logger.info("Closing job status poller")
+        self.job_status_poller.close()
+        logger.info("Terminated job status poller")
 
         logger.info("Scaling in and shutting down executors")
 
         for executor in self.executors.values():
             if not executor.bad_state_is_set:
                 if isinstance(executor, BlockProviderExecutor):
                     logger.info(f"Scaling in executor {executor.label}")
@@ -1351,36 +1350,34 @@
                 logger.error(reason)
                 raise BadCheckpoint(reason)
 
             logger.info("Completed loading checkpoint: {0} with {1} tasks".format(checkpoint_file,
                                                                                   len(memo_lookup_table.keys())))
         return memo_lookup_table
 
-    def load_checkpoints(self, checkpointDirs):
+    @typeguard.typechecked
+    def load_checkpoints(self, checkpointDirs: Optional[Sequence[str]]) -> Dict[str, Future]:
         """Load checkpoints from the checkpoint files into a dictionary.
 
         The results are used to pre-populate the memoizer's lookup_table
 
         Kwargs:
              - checkpointDirs (list) : List of run folder to use as checkpoints
                Eg. ['runinfo/001', 'runinfo/002']
 
         Returns:
              - dict containing, hashed -> future mappings
         """
         self.memo_lookup_table = None
 
-        if not checkpointDirs:
+        if checkpointDirs:
+            return self._load_checkpoints(checkpointDirs)
+        else:
             return {}
 
-        if type(checkpointDirs) is not list:
-            raise BadCheckpoint("checkpointDirs expects a list of checkpoints")
-
-        return self._load_checkpoints(checkpointDirs)
-
     @staticmethod
     def _log_std_streams(task_record: TaskRecord) -> None:
         if task_record['app_fu'].stdout is not None:
             logger.info("Standard output for task {} available at {}".format(task_record['id'], task_record['app_fu'].stdout))
         if task_record['app_fu'].stderr is not None:
             logger.info("Standard error for task {} available at {}".format(task_record['id'], task_record['app_fu'].stderr))
```

### Comparing `parsl-2023.5.8/parsl/dataflow/errors.py` & `parsl-2023.6.5/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/dataflow/futures.py` & `parsl-2023.6.5/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/dataflow/job_error_handler.py` & `parsl-2023.6.5/parsl/dataflow/job_error_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/dataflow/job_status_poller.py` & `parsl-2023.6.5/parsl/dataflow/job_status_poller.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from parsl.dataflow.job_error_handler import JobErrorHandler
 from parsl.dataflow.strategy import Strategy
 from parsl.executors.base import ParslExecutor
 from parsl.monitoring.message_type import MessageType
 
 from parsl.providers.base import JobStatus, JobState
 
+from parsl.utils import Timer
+
 logger = logging.getLogger(__name__)
 
 
 class PollItem(ExecutorStatus):
     def __init__(self, executor: ParslExecutor, dfk: "parsl.dataflow.dflow.DataFlowKernel"):
         self._executor = executor
         self._dfk = dfk
@@ -95,20 +97,22 @@
             self._status.update(new_status)
         return block_ids
 
     def __repr__(self) -> str:
         return self._status.__repr__()
 
 
-class JobStatusPoller:
+class JobStatusPoller(Timer):
     def __init__(self, dfk: "parsl.dataflow.dflow.DataFlowKernel"):
         self._poll_items = []  # type: List[PollItem]
         self.dfk = dfk
-        self._strategy = Strategy(dfk)
+        self._strategy = Strategy(strategy=dfk.config.strategy,
+                                  max_idletime=dfk.config.max_idletime)
         self._error_handler = JobErrorHandler()
+        super().__init__(self.poll, interval=5, name="JobStatusPoller")
 
     def poll(self):
         self._update_state()
         self._error_handler.run(self._poll_items)
         self._strategy.strategize(self._poll_items)
 
     def _update_state(self) -> None:
```

### Comparing `parsl-2023.5.8/parsl/dataflow/memoization.py` & `parsl-2023.6.5/parsl/dataflow/memoization.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,14 @@
 
         Args:
             - task (dict) : Task dictionary from dfk.tasks
 
         Returns:
             - hash (str) : A unique hash string
         """
-        # Function name TODO: Add fn body later
 
         t = []  # type: List[bytes]
 
         # if kwargs contains an outputs parameter, that parameter is removed
         # and normalised differently - with output_ref set to True.
         # kwargs listed in ignore_for_cache will also be removed
```

### Comparing `parsl-2023.5.8/parsl/dataflow/rundirs.py` & `parsl-2023.6.5/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/dataflow/states.py` & `parsl-2023.6.5/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/dataflow/strategy.py` & `parsl-2023.6.5/parsl/dataflow/strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import time
 import math
 import warnings
-from typing import List
+from typing import Dict, List, Optional
 
 from parsl.dataflow.executor_status import ExecutorStatus
 from parsl.executors import HighThroughputExecutor
+from parsl.executors.base import ParslExecutor
 from parsl.executors.status_handling import BlockProviderExecutor
 from parsl.providers.base import JobState
 from parsl.process_loggers import wrap_with_logs
 
 
 logger = logging.getLogger(__name__)
 
@@ -106,36 +107,32 @@
         | X      X  | ----> |           |
         | X      X  |       | X         |
         |slot   slot|       |slot   slot|
         +-----------+       +-----------+
 
     """
 
-    def __init__(self, dfk):
+    def __init__(self, *, strategy: Optional[str], max_idletime: float):
         """Initialize strategy."""
-        self.dfk = dfk
-        self.config = dfk.config
+        self.executors: Dict[str, ParslExecutor]
         self.executors = {}
-        self.max_idletime = self.dfk.config.max_idletime
-
-        for e in self.dfk.config.executors:
-            self.executors[e.label] = {'idle_since': None}
+        self.max_idletime = max_idletime
 
         self.strategies = {None: self._strategy_noop,
                            'none': self._strategy_noop,
                            'simple': self._strategy_simple,
                            'htex_auto_scale': self._strategy_htex_auto_scale}
 
-        if self.config.strategy is None:
+        if strategy is None:
             warnings.warn("literal None for strategy choice is deprecated. Use string 'none' instead.",
                           DeprecationWarning)
 
-        self.strategize = self.strategies[self.config.strategy]
+        self.strategize = self.strategies[strategy]
 
-        logger.debug("Scaling strategy: {0}".format(self.config.strategy))
+        logger.debug("Scaling strategy: {0}".format(strategy))
 
     def add_executors(self, executors):
         for executor in executors:
             self.executors[executor.label] = {'idle_since': None}
 
     def _strategy_noop(self, status: List[ExecutorStatus]) -> None:
         """Do nothing.
```

### Comparing `parsl-2023.5.8/parsl/dataflow/taskrecord.py` & `parsl-2023.6.5/parsl/dataflow/taskrecord.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/errors.py` & `parsl-2023.6.5/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/base.py` & `parsl-2023.6.5/parsl/executors/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from abc import ABCMeta, abstractmethod
 from concurrent.futures import Future
 from typing import Any, Callable, Dict, Optional, List
+from typing_extensions import Literal, Self
 
 from parsl.providers.base import JobStatus
 
 import parsl  # noqa F401
 
 
 class ParslExecutor(metaclass=ABCMeta):
     """Executors are abstractions that represent available compute resources
     to which you could submit arbitrary App tasks.
 
-    This is a metaclass that only enforces concrete implementations of
-    functionality by the child classes.
+    This is an abstract base class that only enforces concrete implementations
+    of functionality by the child classes.
 
     Can be used as a context manager. On exit, calls ``self.shutdown()`` with
     no arguments and re-raises any thrown exception.
 
     In addition to the listed methods, a ParslExecutor instance must always
     have a member field:
 
@@ -42,18 +43,18 @@
               persuaded otherwise. So if you're implementing an executor and want to
               @typeguard the constructor, you'll have to use List[Any] here.
     """
 
     label: str = "undefined"
     radio_mode: str = "udp"
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Literal[False]:
         self.shutdown()
         return False
 
     @abstractmethod
     def start(self) -> Optional[List[str]]:
         """Start the executor.
 
@@ -72,18 +73,14 @@
         """
         pass
 
     @abstractmethod
     def scale_out(self, blocks: int) -> List[str]:
         """Scale out method.
 
-        We should have the scale out method simply take resource object
-        which will have the scaling methods, scale_out itself should be a coroutine, since
-        scaling tasks can be slow.
-
         :return: A list of block ids corresponding to the blocks that were added.
         """
         pass
 
     @abstractmethod
     def scale_in(self, blocks: int) -> List[str]:
         """Scale in method.
@@ -179,15 +176,15 @@
         scheme will be used.
         :param error_handler: a reference to the generic error handler calling this method
         :param status: status of all jobs launched by this executor
         """
         pass
 
     @abstractmethod
-    def set_bad_state_and_fail_all(self, exception: Exception):
+    def set_bad_state_and_fail_all(self, exception: Exception) -> None:
         """Allows external error handlers to mark this executor as irrecoverably bad and cause
         all tasks submitted to it now and in the future to fail. The executor is responsible
         for checking  :method:bad_state_is_set() in the :method:submit() method and raising the
         appropriate exception, which is available through :method:executor_exception().
         """
         pass
```

### Comparing `parsl-2023.5.8/parsl/executors/errors.py` & `parsl-2023.6.5/parsl/executors/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/extreme_scale/executor.py` & `parsl-2023.6.5/parsl/executors/extreme_scale/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/extreme_scale/mpi_worker_pool.py` & `parsl-2023.6.5/parsl/executors/extreme_scale/mpi_worker_pool.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/flux/execute_parsl_task.py` & `parsl-2023.6.5/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/flux/executor.py` & `parsl-2023.6.5/parsl/executors/flux/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/flux/flux_instance_manager.py` & `parsl-2023.6.5/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/high_throughput/executor.py` & `parsl-2023.6.5/parsl/executors/high_throughput/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,29 +501,28 @@
             self._queue_management_thread.daemon = True
             self._queue_management_thread.start()
             logger.debug("Started queue management thread")
 
         else:
             logger.error("Management thread already exists, returning")
 
-    def hold_worker(self, worker_id):
+    def hold_worker(self, worker_id: str) -> None:
         """Puts a worker on hold, preventing scheduling of additional tasks to it.
 
         This is called "hold" mostly because this only stops scheduling of tasks,
         and does not actually kill the worker.
 
         Parameters
         ----------
 
         worker_id : str
             Worker id to be put on hold
         """
-        c = self.command_client.run("HOLD_WORKER;{}".format(worker_id))
+        self.command_client.run("HOLD_WORKER;{}".format(worker_id))
         logger.debug("Sent hold request to manager: {}".format(worker_id))
-        return c
 
     @property
     def outstanding(self):
         outstanding_c = self.command_client.run("OUTSTANDING_C")
         return outstanding_c
 
     @property
```

### Comparing `parsl-2023.5.8/parsl/executors/high_throughput/interchange.py` & `parsl-2023.6.5/parsl/executors/high_throughput/interchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,18 +308,19 @@
                 elif command_req.startswith("HOLD_WORKER"):
                     cmd, s_manager = command_req.split(';')
                     manager_id = s_manager.encode('utf-8')
                     logger.info("Received HOLD_WORKER for {}".format(manager_id))
                     if manager_id in self._ready_managers:
                         m = self._ready_managers[manager_id]
                         m['active'] = False
-                        reply = True
                         self._send_monitoring_info(hub_channel, m)
                     else:
-                        reply = False
+                        logger.warning("Worker to hold was not in ready managers list")
+
+                    reply = None
 
                 else:
                     reply = None
 
                 logger.debug("Reply: {}".format(reply))
                 self.command_channel.send_pyobj(reply)
```

### Comparing `parsl-2023.5.8/parsl/executors/high_throughput/probe.py` & `parsl-2023.6.5/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2023.6.5/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,15 +590,15 @@
             worker_queue.get()
         except queue.Empty:
             logger.warning("Worker ID: {} failed to remove itself from ready_worker_queue".format(worker_id))
             pass
 
         try:
             result = execute_task(req['buffer'])
-            serialized_result = serialize(result, buffer_threshold=1e6)
+            serialized_result = serialize(result, buffer_threshold=1000000)
         except Exception as e:
             logger.info('Caught an exception: {}'.format(e))
             result_package = {'type': 'result', 'task_id': tid, 'exception': serialize(RemoteExceptionWrapper(*sys.exc_info()))}
         else:
             result_package = {'type': 'result', 'task_id': tid, 'result': serialized_result}
             # logger.debug("Result: {}".format(result))
```

### Comparing `parsl-2023.5.8/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2023.6.5/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/status_handling.py` & `parsl-2023.6.5/parsl/executors/status_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,17 @@
             except Exception as ex:
                 self._fail_job_async(block_id,
                                      "Failed to start block {}: {}".format(block_id, ex))
         return block_ids
 
     def _launch_block(self, block_id: str) -> Any:
         launch_cmd = self._get_launch_command(block_id)
-        job_id = self.provider.submit(launch_cmd, 1)
+        job_name = f"parsl.{self.label}.block-{block_id}"
+        logger.debug("Submitting to provider with job_name %s", job_name)
+        job_id = self.provider.submit(launch_cmd, 1, job_name)
         if job_id:
             logger.debug(f"Launched block {block_id} on executor {self.label} with job ID {job_id}")
         else:
             raise ScalingFailed(self,
                                 "Attempt to provision nodes did not return a job ID")
         return job_id
```

### Comparing `parsl-2023.5.8/parsl/executors/swift_t.py` & `parsl-2023.6.5/parsl/executors/swift_t.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/threads.py` & `parsl-2023.6.5/parsl/executors/threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2023.6.5/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/workqueue/executor.py` & `parsl-2023.6.5/parsl/executors/workqueue/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,14 @@
         logger.debug("Getting tasks_lock to set WQ-level task entry")
         with self.tasks_lock:
             logger.debug("Got tasks_lock to set WQ-level task entry")
             self.tasks[str(executor_task_id)] = fu
 
         logger.debug("Creating executor task {} for function {} with args {}".format(executor_task_id, func, args))
 
-        # Pickle the result into object to pass into message buffer
         function_file = self._path_in_task(executor_task_id, "function")
         result_file = self._path_in_task(executor_task_id, "result")
         map_file = self._path_in_task(executor_task_id, "map")
 
         logger.debug("Creating executor task {} with function at: {}".format(executor_task_id, function_file))
         logger.debug("Creating executor task {} with result to be found at: {}".format(executor_task_id, result_file))
 
@@ -856,15 +855,19 @@
                                                     result=os.path.basename(task.result_file))
                     logger.debug(command_str)
 
                     # Create WorkQueue task for the command
                     logger.debug("Sending executor task {} with command: {}".format(task.id, command_str))
                     t = wq.Task(command_str)
                 else:
-                    t = wq.RemoteTask("run_parsl_task", "parsl_coprocess", task.map_file, task.function_file, task.result_file)
+                    t = wq.RemoteTask("run_parsl_task",
+                                      "parsl_coprocess",
+                                      os.path.basename(task.map_file),
+                                      os.path.basename(task.function_file),
+                                      os.path.basename(task.result_file))
                     t.specify_exec_method("direct")
                     logger.debug("Sending executor task {} to coprocess".format(task.id))
 
             except Exception as e:
                 logger.error("Unable to create task: {}".format(e))
                 collector_queue.put_nowait(WqTaskToParsl(id=task.id,
                                                          result_received=False,
```

### Comparing `parsl-2023.5.8/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/launchers/__init__.py` & `parsl-2023.6.5/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/launchers/launchers.py` & `parsl-2023.6.5/parsl/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/log_utils.py` & `parsl-2023.6.5/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/db_manager.py` & `parsl-2023.6.5/parsl/monitoring/db_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/monitoring.py` & `parsl-2023.6.5/parsl/monitoring/monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/queries/pandas.py` & `parsl-2023.6.5/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/radios.py` & `parsl-2023.6.5/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/remote.py` & `parsl-2023.6.5/parsl/monitoring/remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/types.py` & `parsl-2023.6.5/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/app.py` & `parsl-2023.6.5/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/models.py` & `parsl-2023.6.5/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2023.6.5/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,30 @@
 import plotly.figure_factory as ff
 from plotly.offline import plot
 import networkx as nx
 
 from parsl.monitoring.visualization.utils import timestamp_to_int, num_to_timestamp, DB_DATE_FORMAT
 
 
+# gantt_colors must assign a color value for every state name defined
+# in parsl/dataflow/states.py
+gantt_colors = {'unsched': 'rgb(240, 240, 240)',
+                'pending': 'rgb(168, 168, 168)',
+                'launched': 'rgb(100, 255, 255)',
+                'running': 'rgb(0, 0, 255)',
+                'running_ended': 'rgb(64, 64, 255)',
+                'joining': 'rgb(128, 128, 255)',
+                'dep_fail': 'rgb(255, 128, 255)',
+                'failed': 'rgb(200, 0, 0)',
+                'exec_done': 'rgb(0, 200, 0)',
+                'memo_done': 'rgb(64, 200, 64)',
+                'fail_retryable': 'rgb(200, 128,128)'
+               }
+
+
 def task_gantt_plot(df_task, df_status, time_completed=None):
 
     # if the workflow is not recorded as completed, then assume
     # that tasks should continue in their last state until now,
     # rather than the workflow end time.
     if not time_completed:
         time_completed = df_status['timestamp'].max()
@@ -43,33 +59,17 @@
             last_status_bar = {'Task': description,
                                'Start': last_status['timestamp'],
                                'Finish': time_completed,
                                'Resource': last_status['task_status_name']
                               }
             parsl_tasks.extend([last_status_bar])
 
-    # colours must assign a colour value for every state name defined
-    # in parsl/dataflow/states.py
-
-    colors = {'unsched': 'rgb(240, 240, 240)',
-              'pending': 'rgb(168, 168, 168)',
-              'launched': 'rgb(100, 255, 255)',
-              'running': 'rgb(0, 0, 255)',
-              'running_ended': 'rgb(64, 64, 255)',
-              'joining': 'rgb(128, 128, 255)',
-              'dep_fail': 'rgb(255, 128, 255)',
-              'failed': 'rgb(200, 0, 0)',
-              'exec_done': 'rgb(0, 200, 0)',
-              'memo_done': 'rgb(64, 200, 64)',
-              'fail_retryable': 'rgb(200, 128,128)'
-             }
-
     fig = ff.create_gantt(parsl_tasks,
                           title="",
-                          colors=colors,
+                          colors=gantt_colors,
                           group_tasks=True,
                           show_colorbar=True,
                           index_col='Resource',
                           )
     fig['layout']['yaxis']['title'] = 'Task'
     fig['layout']['yaxis']['showticklabels'] = False
     fig['layout']['xaxis']['title'] = 'Time'
@@ -190,14 +190,28 @@
                     ],
         barmode='stack',
         title="Total tasks"))
 
     return plot(fig, show_link=False, output_type="div", include_plotlyjs=False)
 
 
+dag_state_colors = {"unsched": (0, 'rgb(240, 240, 240)'),
+                    "pending": (1, 'rgb(168, 168, 168)'),
+                    "launched": (2, 'rgb(100, 255, 255)'),
+                    "running": (3, 'rgb(0, 0, 255)'),
+                    "dep_fail": (4, 'rgb(255, 128, 255)'),
+                    "failed": (5, 'rgb(200, 0, 0)'),
+                    "exec_done": (6, 'rgb(0, 200, 0)'),
+                    "memo_done": (7, 'rgb(64, 200, 64)'),
+                    "fail_retryable": (8, 'rgb(200, 128,128)'),
+                    "joining": (9, 'rgb(128, 128, 255)'),
+                    "running_ended": (10, 'rgb(64, 64, 255)')
+                   }
+
+
 def workflow_dag_plot(df_tasks, group_by_apps=True):
     G = nx.DiGraph(directed=True)
     nodes = df_tasks['task_id'].unique()
     dic = df_tasks.set_index('task_id').to_dict()
     G.add_nodes_from(nodes)
 
     # Add edges or links between the nodes:
@@ -211,25 +225,15 @@
 
     node_positions = nx.nx_pydot.pydot_layout(G, prog='dot')
 
     if group_by_apps:
         groups_list = {app: (i, None) for i, app in enumerate(
             df_tasks['task_func_name'].unique())}
     else:
-        groups_list = {"unsched": (0, 'rgb(240, 240, 240)'),
-                       "pending": (1, 'rgb(168, 168, 168)'),
-                       "launched": (2, 'rgb(100, 255, 255)'),
-                       "running": (3, 'rgb(0, 0, 255)'),
-                       "dep_fail": (4, 'rgb(255, 128, 255)'),
-                       "failed": (5, 'rgb(200, 0, 0)'),
-                       "exec_done": (6, 'rgb(0, 200, 0)'),
-                       "memo_done": (7, 'rgb(64, 200, 64)'),
-                       "fail_retryable": (8, 'rgb(200, 128,128)'),
-                       "joining": (9, 'rgb(128, 128, 255)')
-                      }
+        groups_list = dag_state_colors
 
     node_traces = [...] * len(groups_list)
 
     for k, (index, color) in groups_list.items():
         node_trace = go.Scatter(
             x=[],
             y=[],
```

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2023.6.5/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/templates/app.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/templates/dag.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/templates/layout.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/templates/task.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/monitoring/visualization/views.py` & `parsl-2023.6.5/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/multiprocessing.py` & `parsl-2023.6.5/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/process_loggers.py` & `parsl-2023.6.5/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/__init__.py` & `parsl-2023.6.5/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2023.6.5/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/aws/aws.py` & `parsl-2023.6.5/parsl/providers/aws/aws.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/azure/azure.py` & `parsl-2023.6.5/parsl/providers/azure/azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/base.py` & `parsl-2023.6.5/parsl/providers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/cluster_provider.py` & `parsl-2023.6.5/parsl/providers/cluster_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/cobalt/cobalt.py` & `parsl-2023.6.5/parsl/providers/cobalt/cobalt.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/condor/condor.py` & `parsl-2023.6.5/parsl/providers/condor/condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/condor/template.py` & `parsl-2023.6.5/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/errors.py` & `parsl-2023.6.5/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/googlecloud/googlecloud.py` & `parsl-2023.6.5/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/grid_engine/grid_engine.py` & `parsl-2023.6.5/parsl/providers/grid_engine/grid_engine.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/kubernetes/kube.py` & `parsl-2023.6.5/parsl/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/local/local.py` & `parsl-2023.6.5/parsl/providers/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/lsf/lsf.py` & `parsl-2023.6.5/parsl/providers/lsf/lsf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/pbspro/pbspro.py` & `parsl-2023.6.5/parsl/providers/pbspro/pbspro.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/slurm/slurm.py` & `parsl-2023.6.5/parsl/providers/slurm/slurm.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/providers/torque/torque.py` & `parsl-2023.6.5/parsl/providers/torque/torque.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/serialize/concretes.py` & `parsl-2023.6.5/parsl/serialize/concretes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import dill
 import pickle
 import logging
 
 logger = logging.getLogger(__name__)
 from parsl.serialize.base import SerializerBase
 
+from typing import Any
+
 
 class PickleSerializer(SerializerBase):
     """ Pickle serialization covers most python objects, with some notable exceptions:
 
     * functions defined in a interpreter/notebook
     * classes defined in local context and not importable using a fully qualified name
     * closures, generators and coroutines
     * [sometimes] issues with wrapped/decorated functions
     """
 
     _identifier = b'01\n'
     _for_code = True
     _for_data = True
 
-    def serialize(self, data):
+    def serialize(self, data: Any) -> bytes:
         x = pickle.dumps(data)
         return self.identifier + x
 
-    def deserialize(self, payload):
+    def deserialize(self, payload: bytes) -> Any:
         chomped = self.chomp(payload)
         data = pickle.loads(chomped)
         return data
 
 
 class DillSerializer(SerializerBase):
     """ Dill serialization works on a superset of object including the ones covered by pickle.
@@ -41,15 +43,15 @@
     * closures
     """
 
     _identifier = b'02\n'
     _for_code = True
     _for_data = True
 
-    def serialize(self, data):
+    def serialize(self, data: Any) -> bytes:
         x = dill.dumps(data)
         return self.identifier + x
 
-    def deserialize(self, payload):
+    def deserialize(self, payload: bytes) -> Any:
         chomped = self.chomp(payload)
         data = dill.loads(chomped)
         return data
```

### Comparing `parsl-2023.5.8/parsl/serialize/facade.py` & `parsl-2023.6.5/parsl/serialize/facade.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from parsl.serialize.concretes import *  # noqa: F403,F401
-from parsl.serialize.base import METHODS_MAP_DATA, METHODS_MAP_CODE
+from parsl.serialize.base import METHODS_MAP_DATA, METHODS_MAP_CODE, SerializerBase
 import logging
 
+from typing import Any, Dict, List, Tuple, Union
+
 logger = logging.getLogger(__name__)
 
 
 """ Instantiate the appropriate classes
 """
 headers = list(METHODS_MAP_CODE.keys()) + list(METHODS_MAP_DATA.keys())
 header_size = len(headers[0])
@@ -13,148 +15,144 @@
 methods_for_code = {}
 methods_for_data = {}
 
 for key in METHODS_MAP_CODE:
     methods_for_code[key] = METHODS_MAP_CODE[key]()
     methods_for_code[key].enable_caching(maxsize=128)
 
-    for key in METHODS_MAP_DATA:
-        methods_for_data[key] = METHODS_MAP_DATA[key]()
+for key in METHODS_MAP_DATA:
+    methods_for_data[key] = METHODS_MAP_DATA[key]()
 
 
-def _list_methods():
+def _list_methods() -> Tuple[Dict[bytes, SerializerBase], Dict[bytes, SerializerBase]]:
     return methods_for_code, methods_for_data
 
 
-def pack_apply_message(func, args, kwargs, buffer_threshold=128 * 1e6):
+def pack_apply_message(func: Any, args: Any, kwargs: Any, buffer_threshold: int = int(128 * 1e6)) -> bytes:
     """Serialize and pack function and parameters
 
     Parameters
     ----------
 
     func: Function
         A function to ship
 
     args: Tuple/list of objects
         positional parameters as a list
 
     kwargs: Dict
         Dict containing named parameters
 
-    buffer_threshold: Ignored
+    buffer_threshold: int
         Limits buffer to specified size in bytes. Exceeding this limit would give you
         a warning in the log. Default is 128MB.
     """
     b_func = serialize(func, buffer_threshold=buffer_threshold)
     b_args = serialize(args, buffer_threshold=buffer_threshold)
     b_kwargs = serialize(kwargs, buffer_threshold=buffer_threshold)
     packed_buffer = pack_buffers([b_func, b_args, b_kwargs])
     return packed_buffer
 
 
-def unpack_apply_message(packed_buffer, user_ns=None, copy=False):
+def unpack_apply_message(packed_buffer: bytes, user_ns: Any = None, copy: Any = False) -> List[Any]:
     """ Unpack and deserialize function and parameters
 
     """
     return [deserialize(buf) for buf in unpack_buffers(packed_buffer)]
 
 
-def serialize(obj, buffer_threshold=1e6):
+def serialize(obj: Any, buffer_threshold: int = int(1e6)) -> bytes:
     """ Try available serialization methods one at a time
 
     Individual serialization methods might raise a TypeError (eg. if objects are non serializable)
     This method will raise the exception from the last method that was tried, if all methods fail.
     """
-    serialized = None
-    serialized_flag = False
-    last_exception = None
+    result: Union[bytes, Exception]
     if callable(obj):
         for method in methods_for_code.values():
             try:
-                serialized = method.serialize(obj)
+                result = method.serialize(obj)
             except Exception as e:
-                last_exception = e
+                result = e
                 continue
             else:
-                serialized_flag = True
                 break
     else:
         for method in methods_for_data.values():
             try:
-                serialized = method.serialize(obj)
+                result = method.serialize(obj)
             except Exception as e:
-                last_exception = e
+                result = e
                 continue
             else:
-                serialized_flag = True
                 break
 
-    if serialized_flag is False:
-        # TODO : Replace with a SerializationError
-        raise last_exception
-
-    if len(serialized) > buffer_threshold:
-        logger.warning(f"Serialized object exceeds buffer threshold of {buffer_threshold} bytes, this could cause overflows")
-    return serialized
+    if isinstance(result, BaseException):
+        raise result
+    else:
+        if len(result) > buffer_threshold:
+            logger.warning(f"Serialized object exceeds buffer threshold of {buffer_threshold} bytes, this could cause overflows")
+        return result
 
 
-def deserialize(payload):
+def deserialize(payload: bytes) -> Any:
     """
     Parameters
     ----------
     payload : str
        Payload object to be deserialized
 
     """
     header = payload[0:header_size]
     if header in methods_for_code:
         result = methods_for_code[header].deserialize(payload)
     elif header in methods_for_data:
         result = methods_for_data[header].deserialize(payload)
     else:
-        raise TypeError("Invalid header: {} in data payload. Buffer is either corrupt or not created by ParslSerializer".format(header))
+        raise TypeError("Invalid header: {!r} in data payload. Buffer is either corrupt or not created by ParslSerializer".format(header))
 
     return result
 
 
-def pack_buffers(buffers):
+def pack_buffers(buffers: List[bytes]) -> bytes:
     """
     Parameters
     ----------
-    buffers : list of \n terminated strings
+    buffers: list of byte strings
     """
     packed = b''
     for buf in buffers:
         s_length = bytes(str(len(buf)) + '\n', 'utf-8')
         packed += s_length + buf
 
     return packed
 
 
-def unpack_buffers(packed_buffer):
+def unpack_buffers(packed_buffer: bytes) -> List[bytes]:
     """
     Parameters
     ----------
-    packed_buffers : packed buffer as string
+    packed_buffers : packed buffer as byte sequence
     """
     unpacked = []
     while packed_buffer:
         s_length, buf = packed_buffer.split(b'\n', 1)
         i_length = int(s_length.decode('utf-8'))
         current, packed_buffer = buf[:i_length], buf[i_length:]
         unpacked.extend([current])
 
     return unpacked
 
 
-def unpack_and_deserialize(packed_buffer):
-    """ Unpacks a packed buffer and returns the deserialized contents
+def unpack_and_deserialize(packed_buffer: bytes) -> Any:
+    """ Unpacks a packed buffer of 3 byte sequences and returns the
+    deserialized contents for use in function application.
     Parameters
     ----------
-    packed_buffers : packed buffer as string
+    packed_buffers : packed buffer of 3 byte sequences
     """
     unpacked = []
     while packed_buffer:
         s_length, buf = packed_buffer.split(b'\n', 1)
         i_length = int(s_length.decode('utf-8'))
         current, packed_buffer = buf[:i_length], buf[i_length:]
         deserialized = deserialize(current)
```

### Comparing `parsl-2023.5.8/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2023.6.5/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/azure_single_node.py` & `parsl-2023.6.5/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/bluewaters.py` & `parsl-2023.6.5/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/bridges.py` & `parsl-2023.6.5/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/cc_in2p3.py` & `parsl-2023.6.5/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/comet.py` & `parsl-2023.6.5/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/cooley_htex.py` & `parsl-2023.6.5/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/cori.py` & `parsl-2023.6.5/parsl/tests/configs/cori.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/ec2_single_node.py` & `parsl-2023.6.5/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/ec2_spot.py` & `parsl-2023.6.5/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/exex_local.py` & `parsl-2023.6.5/parsl/tests/configs/exex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/frontera.py` & `parsl-2023.6.5/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2023.6.5/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/htex_local.py` & `parsl-2023.6.5/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/htex_local_alternate.py` & `parsl-2023.6.5/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2023.6.5/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2023.6.5/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/local_threads_globus.py` & `parsl-2023.6.5/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/midway.py` & `parsl-2023.6.5/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/nscc_singapore.py` & `parsl-2023.6.5/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/osg_htex.py` & `parsl-2023.6.5/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/petrelkube.py` & `parsl-2023.6.5/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/summit.py` & `parsl-2023.6.5/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/swan_htex.py` & `parsl-2023.6.5/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/theta.py` & `parsl-2023.6.5/parsl/tests/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/user_opts.py` & `parsl-2023.6.5/parsl/tests/configs/user_opts.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/configs/workqueue_blocks.py` & `parsl-2023.6.5/parsl/tests/configs/workqueue_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/conftest.py` & `parsl-2023.6.5/parsl/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,18 @@
         'markers',
         'issue363: Marks tests that require a shared filesystem for stdout/stderr - see issue #363'
     )
     config.addinivalue_line(
         'markers',
         'staging_required: Marks tests that require a staging provider, when there is no sharedFS)'
     )
+    config.addinivalue_line(
+        'markers',
+        'sshd_required: Marks tests that require a SSHD'
+    )
 
 
 @pytest.fixture(autouse=True, scope='session')
 def load_dfk_session(request, pytestconfig):
     """Load a dfk around entire test suite, except in local mode.
 
     The special path `local` indicates that configuration will not come
```

### Comparing `parsl-2023.5.8/parsl/tests/integration/latency.py` & `parsl-2023.6.5/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/manual_tests/htex_local.py` & `parsl-2023.6.5/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/manual_tests/test_basic.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/site_tests/site_config_selector.py` & `parsl-2023.6.5/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/site_tests/test_provider.py` & `parsl-2023.6.5/parsl/tests/site_tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/site_tests/test_site.py` & `parsl-2023.6.5/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/sites/test_affinity.py` & `parsl-2023.6.5/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/sites/test_concurrent.py` & `parsl-2023.6.5/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2023.6.5/parsl/tests/sites/test_dynamic_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,11 +71,7 @@
     results = [i.result() for i in tasks]
     print("Successfully added htex executor and ran with it. The results are", results)
 
     print("Done testing")
 
     dfk.cleanup()
     parsl.clear()
-
-
-if __name__ == "__main__":
-    test_dynamic_executor()
```

### Comparing `parsl-2023.5.8/parsl/tests/sites/test_ec2.py` & `parsl-2023.6.5/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/sites/test_local_adhoc.py` & `parsl-2023.6.5/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/sites/test_start_method.py` & `parsl-2023.6.5/parsl/tests/sites/test_start_method.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from parsl.channels import LocalChannel
 from parsl.config import Config
 from parsl.executors import HighThroughputExecutor
 from parsl import python_app
 
 
 @python_app()
-def test_function():
+def get_pid():
     return os.getpid()
 
 
 @contextmanager
 def config(start_method: str, **kwargs):
     my_config = Config(
         executors=[
@@ -43,15 +43,15 @@
 
 
 @mark.local
 @mark.parametrize("start_method", ["spawn", "fork", "thread"])
 def test_spawn_method(start_method: str):
     with config(start_method):
         # Get the PID for the child function as a way of making sure it launches
-        future = test_function()
+        future = get_pid()
         remote_pid = future.result()
         assert remote_pid != os.getpid()
 
 
 @mark.local
 def test_htex_config_failures():
     with raises(ValueError) as exc:
```

### Comparing `parsl-2023.5.8/parsl/tests/sites/test_worker_info.py` & `parsl-2023.6.5/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_aalst_patterns.py` & `parsl-2023.6.5/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,13 +19,7 @@
         x.result()
 
 
 def test_walltime_longer():
     """Test that an app that runs in less than walltime will succeed."""
     y = echo_to_file(walltime=2)
     y.result()
-
-
-if __name__ == "__main__":
-    parsl.clear()
-    parsl.load(config)
-    test_walltime()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_basic.py`

 * *Files 19% similar despite different names*

```diff
@@ -109,27 +109,7 @@
     print("Duration : {0}s".format(time.time() - start))
     stdout_file_count = len(
         [item for item in os.listdir(outdir) if item.endswith('.out')])
     assert stdout_file_count == n, "Only {0}/{1} files in '{2}' ".format(len(os.listdir('outputs/')),
                                                                          n, outdir)
     print("[TEST STATUS] test_parallel_for [SUCCESS]")
     return d
-
-
-if __name__ == '__main__':
-    parsl.clear()
-    dfk = parsl.load(config)
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default="10",
-                        help="Count of apps to launch")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    x = test_parallel_for(int(args.count))
-    y = test_command_format_1()
-    z = test_auto_log_filename_format()
-    # raise_error(0)
```

### Comparing `parsl-2023.5.8/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_bash_apps/test_kwarg_storage.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_kwarg_storage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,24 +66,7 @@
 
     d = {}
     for i in range(0, n):
         d[i] = fail_on_presence_kw(outputs=[temp_file], foo={"b": 2, "a": 1})
 
     for i in d:
         assert d[i].exception() is None
-
-
-if __name__ == '__main__':
-    parsl.clear()
-    parsl.load(config)
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default="10",
-                        help="Count of apps to launch")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    x = test_bash_memoization(n=4)
```

### Comparing `parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_bash_apps/test_multiline.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_multiline.py`

 * *Files 27% similar despite different names*

```diff
@@ -57,21 +57,7 @@
     with open('std.err', 'r') as o:
         err = o.read()
         assert err != "Testing STDERR", "Stderr is bad"
 
     os.remove('std.err')
     os.remove('std.out')
     return True
-
-
-if __name__ == '__main__':
-    parsl.clear()
-    dfk = parsl.load(config)
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    # if args.debug:
-    #    parsl.set_stream_logger()
-    test_multiline()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_bash_apps/test_pipeline.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -114,26 +114,7 @@
         if key > 0:
             fu = futs[key]
             data = open(fu.result().filepath, 'r').read().strip()
             assert data == str(
                 key), "[TEST] incr failed for key: {0} got: {1}".format(key, data)
 
     cleanup_work(depth)
-
-
-if __name__ == '__main__':
-    parsl.clear()
-    dfk = parsl.load(config)
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-w", "--width", default="5",
-                        help="width of the pipeline")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    # test_increment(depth=int(args.width))
-    # test_increment(depth=int(args.width))
-    test_increment_slow(depth=int(args.width))
```

### Comparing `parsl-2023.5.8/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files 20% similar despite different names*

```diff
@@ -109,29 +109,7 @@
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len2 = len(open(out).readlines())
 
     assert len1 == 1 and len2 == 2, "Line count of output files should be 1 and 2, but:  len1={} len2={}".format(len1, len2)
 
     os.system('rm -f ' + out + ' ' + err)
-
-
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default="10",
-                        help="Count of apps to launch")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Enable debug output to console")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    parsl.load(config)
-
-    # test_bad_stdout_specs is omitted because it is called in a
-    # more complicated parameterised fashion by pytest.
-
-    y = test_bad_stderr_file()
-    y = test_stdout_truncate()
-    y = test_stdout_append()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_callables.py` & `parsl-2023.6.5/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_channels/test_large_output.py` & `parsl-2023.6.5/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,22 +60,7 @@
         expected_msg2 = " No tasks checkpointed in this pass"
 
         lines = [line for line in log_lines if expected_msg in line or expected_msg2 in line]
         assert len(lines) >= 3, "Insufficient checkpoint lines in logfile"
         deltas = [tstamp_to_seconds(line) for line in lines]
         assert deltas[1] - deltas[0] < 5.5, "Delta between checkpoints exceeded period"
         assert deltas[2] - deltas[1] < 5.5, "Delta between checkpoints exceeded period"
-
-
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default="10",
-                        help="Count of apps to launch")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    x = test_periodic(n=4)
```

### Comparing `parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,45 @@
 import argparse
 import os
 import pytest
-
 import parsl
 from parsl import python_app
-from parsl.tests.configs.local_threads import fresh_config
+
+from parsl.tests.configs.local_threads import config
+from parsl.tests.configs.local_threads_checkpoint import fresh_config
 
 
 @python_app(cache=True)
 def random_app(i):
     import random
     return random.randint(i, 100000)
 
 
 def launch_n_random(n=2):
     """1. Launch a few apps and write the checkpoint once a few have completed
     """
-
     d = [random_app(i) for i in range(0, n)]
-    print("Done launching")
-
-    # Block till done
     return [i.result() for i in d]
 
 
 @pytest.mark.local
-def test_initial_checkpoint_write(n=2):
-    """1. Launch a few apps and write the checkpoint once a few have completed
+def test_loading_checkpoint(n=2):
+    """Load memoization table from previous checkpoint
     """
-    config = fresh_config()
-    config.checkpoint_mode = 'manual'
+    config.checkpoint_mode = 'task_exit'
     parsl.load(config)
     results = launch_n_random(n)
-
-    cpt_dir = parsl.dfk().checkpoint()
-
-    cptpath = cpt_dir + '/dfk.pkl'
-    print("Path exists : ", os.path.exists(cptpath))
-    assert os.path.exists(
-        cptpath), "DFK checkpoint missing: {0}".format(cptpath)
-
-    cptpath = cpt_dir + '/tasks.pkl'
-    print("Path exists : ", os.path.exists(cptpath))
-    assert os.path.exists(
-        cptpath), "Tasks checkpoint missing: {0}".format(cptpath)
-
-    run_dir = parsl.dfk().run_dir
-
+    rundir = parsl.dfk().run_dir
     parsl.dfk().cleanup()
     parsl.clear()
 
-    return run_dir, results
-
-
-if __name__ == '__main__':
+    local_config = fresh_config()
+    local_config.checkpoint_files = [os.path.join(rundir, 'checkpoint')]
+    parsl.load(local_config)
 
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default="10",
-                        help="Count of apps to launch")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
+    relaunched = launch_n_random(n)
+    assert len(relaunched) == len(results) == n, "Expected all results to have n items"
 
-    if args.debug:
-        parsl.set_stream_logger()
-
-    x = test_initial_checkpoint_write(n=4)
+    for i in range(n):
+        assert relaunched[i] == results[i], "Expected relaunched to contain cached results from first run"
+    parsl.dfk().cleanup()
+    parsl.clear()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,13 +80,7 @@
                 tasks.append(pickle.load(f))
                 print
         except EOFError:
             pass
         print("Tasks from cache : ", tasks)
         assert len(tasks) == count, "Expected {} checkpoint events, got {}".format(
             1, len(tasks))
-
-
-if __name__ == "__main__":
-
-    test_regress_232_task_exit()
-    test_regress_232_dfk_exit()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,7 @@
     print(last_checkpoint)
     cached, _ = run_checkpointed([last_checkpoint])
 
     print(cached)
     print(original)
 
     assert cached == original, "All tasks were not cached"
-
-
-if __name__ == "__main__":
-
-    test_checkpoint_availability()
-    # test_regress_234()
-    # test_slower_apps()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,12 +78,7 @@
             while f:
                 tasks.append(pickle.load(f))
                 print
         except EOFError:
             pass
         print("Tasks from cache : ", tasks)
         assert len(tasks) == 1, "Expected {} checkpoint events, got {}".format(1, len(tasks))
-
-
-if __name__ == "__main__":
-    test_regression_239()
-    test_checkpointing_at_dfk_exit()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,22 +60,7 @@
         try:
             while f:
                 tasks.append(pickle.load(f))
         except EOFError:
             pass
 
         assert len(tasks) == n, "Expected {} checkpoint events, got {}".format(n, len(tasks))
-
-
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default=10, type=int,
-                        help="Count of apps to launch")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    x = test_at_task_exit(args.count)
```

### Comparing `parsl-2023.5.8/parsl/tests/test_data/test_file.py` & `parsl-2023.6.5/parsl/tests/test_data/test_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,12 +26,7 @@
     with open('test-open.txt', 'w') as tfile:
         tfile.write('Hello')
 
     pfile = File('test-open.txt')
 
     with open(str(pfile), 'r') as opfile:
         assert (opfile.readlines()[0] == 'Hello')
-
-
-if __name__ == '__main__':
-
-    test_files()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_data/test_file_apps.py` & `parsl-2023.6.5/parsl/tests/test_data/test_file_apps.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,15 +68,7 @@
 
     for key in futs:
         if key > 0:
             fu = futs[key]
             data = open(fu.result().filepath, 'r').read().strip()
             assert data == str(
                 key), "[TEST] incr failed for key:{0} got:{1}".format(key, data)
-
-
-if __name__ == '__main__':
-    parsl.clear()
-    parsl.load(config)
-
-    test_files()
-    test_increment()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_data/test_file_staging.py` & `parsl-2023.6.5/parsl/tests/test_data/test_file_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_docs/test_from_slides.py` & `parsl-2023.6.5/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_docs/test_workflow1.py` & `parsl-2023.6.5/parsl/tests/test_docs/test_workflow1.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,7 @@
 
     saved = save(message, outputs=[File('output.txt')])
 
     with open(saved.outputs[0].result().filepath, 'r') as f:
         item = int(f.read().strip())
         assert item <= N, "Expected file to contain int <= N"
         assert item >= 1, "Expected file to contain int >= 1"
-
-
-if __name__ == "__main__":
-    parsl.clear()
-    parsl.load(config)
-
-    test_procedural()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_docs/test_workflow2.py` & `parsl-2023.6.5/parsl/tests/test_docs/test_workflow2.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,12 +37,7 @@
     print(doubled_z.result())
     time.time()
     delta = time.time() - start
 
     assert doubled_z.result() == N * \
         2, "Expected doubled_z = N*2 = {0}".format(N * 2)
     assert delta > 4 and delta < 5, "Time delta exceeded expected 4 < duration < 5"
-
-
-if __name__ == "__main__":
-
-    test_parallel()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_docs/test_workflow4.py` & `parsl-2023.6.5/parsl/tests/test_docs/test_workflow4.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,7 @@
     # concatenate the files into a single file
     cc = concat(inputs=[i.outputs[0]
                         for i in output_files], outputs=[File("all.txt")])
 
     # calculate the average of the random numbers
     totals = total(inputs=[cc.outputs[0]])
     print(totals.result())
-
-
-if __name__ == "__main__":
-    parsl.clear()
-    parsl.load(config)
-
-    test_parallel_dataflow()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_error_handling/test_htex_missing_worker.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_error_handling/test_htex_worker_failure.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_worker_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2023.6.5/parsl/tests/workqueue_tests/test_scale.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,190 +1,146 @@
-import argparse
+#!/usr/bin/env python3
 
-import pytest
+import argparse
+import time
 
 import parsl
-from parsl.app.app import python_app
-from parsl.tests.configs.local_threads import fresh_config
-
 
-def local_config():
-    c = fresh_config()
-    c.retries = 2
-    return c
+# from parsl.tests.configs.htex_local import config
+# from htex_local import config
+# from exex_local import config
+# from parsl.configs.local_threads import config
+# from parsl.configs.local_ipp import config
+# from parsl.tests.configs.exex_local import config
+
+# parsl.set_stream_logger()
+# config.executors[0].provider.tasks_per_node = 4
+# parsl.load(config)
+from parsl.app.app import python_app  # , bash_app
 
 
 @python_app
-def sleep_fail(sleep_dur, sleep_rand_max, fail_prob, inputs=[]):
-    import time
-    import random
+def double(x):
+    return x * 2
 
-    s = sleep_dur + random.randint(-sleep_rand_max, sleep_rand_max)
 
-    time.sleep(s)
-    x = float(random.randint(0, 100)) / 100
-    if x <= fail_prob:
-        # print("Fail")
-        raise Exception("App failure")
-    else:
-        pass
-        # print("Succeed")
+@python_app
+def echo(x, string, stdout=None):
+    print(string)
+    return x * 5
 
 
 @python_app
-def double(x):
-    return x * 2
+def import_echo(x, string, stdout=None):
+    # from time import sleep
+    # sleep(0)
+    print(string)
+    return x * 5
 
 
-@pytest.mark.local
-def test_simple(n=10):
+@python_app
+def platform(sleep=10, stdout=None):
+    import platform
     import time
+    time.sleep(sleep)
+    return platform.uname()
+
+
+def test_simple(n=2):
     start = time.time()
     x = double(n)
     print("Result : ", x.result())
     assert x.result() == n * \
         2, "Expected double to return:{0} instead got:{1}".format(
             n * 2, x.result())
     print("Duration : {0}s".format(time.time() - start))
     print("[TEST STATUS] test_parallel_for [SUCCESS]")
     return True
 
 
-@pytest.mark.skip('broken')
-def test_no_deps(numtasks=10):
-    """Test basic error handling, with no dependent failures
-    """
-
-    fus = []
-    for i in range(0, 10):
-
-        fu = sleep_fail(0.1, 0, .8)
-        fus.extend([fu])
-
-    count = 0
-    for fu in fus:
-        try:
-            fu.result()
-        except Exception as e:
-            print("Caught exception : ", "*" * 20)
-            print(e)
-            print("*" * 20)
-            count += 1
-
-    print("Caught failures of  {0}/{1}".format(count, len(fus)))
-
-
-@pytest.mark.skip('broken')
-def test_fail_sequence(numtasks=10):
-    """Test failure in a sequence of dependencies
-
-    App1 -> App2 ... -> AppN
-    """
-
-    sleep_dur = 0.1
-    fail_prob = 0.4
-
-    fus = {0: None}
-    for i in range(0, numtasks):
-        print("Chaining {0} to {1}".format(i + 1, fus[i]))
-        fus[i + 1] = sleep_fail(sleep_dur, 0, fail_prob, inputs=[fus[i]])
-
-    # time.sleep(numtasks*sleep_dur)
-    for k in sorted(fus.keys()):
-        try:
-            x = fus[i].result()
-            print("{0} : {1}".format(k, x))
-        except Exception as e:
-            print("{0} : {1}".format(k, e))
-
-    return
-
-
-@pytest.mark.skip('broken')
-def test_deps(numtasks=10):
-    """Random failures in branches of Map -> Map -> reduce
-
-    App1   App2  ... AppN
-    """
-
-    fus = []
-    for i in range(0, numtasks):
-        fu = sleep_fail(0.2, 0, .4)
-        fus.extend([fu])
-
-    # App1   App2  ... AppN
-    # |       |        |
-    # V       V        V
-    # App1   App2  ... AppN
-
-    fus_2 = []
-    for fu in fus:
-        fu = sleep_fail(0, 0, .8, inputs=[fu])
-        fus_2.extend([fu])
-
-    # App1   App2  ... AppN
-    #   |       |        |
-    #   V       V        V
-    # App1   App2  ... AppN
-    #    \      |       /
-    #     \     |      /
-    #       App_Final
-
-    fu_final = sleep_fail(1, 0, 0, inputs=fus_2)
-
-    try:
-        print("Final status : ", fu_final.result())
-    except parsl.dataflow.errors.DependencyError as e:
-        print("Caught the right exception")
-        print("Exception : ", e)
-    except Exception as e:
-        assert 5 == 1, "Expected DependencyError got : %s" % e
-    else:
-        print("Shoot! no errors ")
+def test_imports(n=2):
+    start = time.time()
+    x = import_echo(n, "hello world")
+    print("Result : ", x.result())
+    assert x.result() == n * \
+        5, "Expected double to return:{0} instead got:{1}".format(
+            n * 2, x.result())
+    print("Duration : {0}s".format(time.time() - start))
+    print("[TEST STATUS] test_parallel_for [SUCCESS]")
+    return True
 
 
-@python_app
-def sleep_then_fail(sleep_dur=0.1):
-    import time
-    import math
-    time.sleep(sleep_dur)
-    math.ceil("Trigger TypeError")
-    return 0
+def test_platform(n=2, sleep=1):
 
+    dfk = parsl.dfk()
+    # sync
+    x = platform(sleep=0)
+    print(x.result())
+
+    name = list(dfk.executors.keys())[0]
+    print("Trying to get executor : ", name)
+
+    print("Executor : ", dfk.executors[name])
+    print("Connected   : ", dfk.executors[name].connected_workers)
+    print("Outstanding : ", dfk.executors[name].outstanding)
+    d = []
+    for i in range(0, n):
+        x = platform(sleep=sleep)
+        d.append(x)
 
-@pytest.mark.skip('broken')
-def test_fail_nowait(numtasks=10):
-    """Test basic error handling, with no dependent failures
-    """
-    import time
-    fus = []
-    for i in range(0, numtasks):
-        fu = sleep_then_fail(sleep_dur=0.1)
-        fus.extend([fu])
-
-    try:
-        [x.result() for x in fus]
-    except Exception as e:
-        assert isinstance(e, TypeError), "Expected a TypeError, got {}".format(e)
-
-    # fus[0].result()
-    time.sleep(1)
-    print("Done")
+    print("Connected   : ", dfk.executors[name].connected_workers)
+    print("Outstanding : ", dfk.executors[name].outstanding)
+
+    print(set([i.result()for i in d]))
+
+    print("Connected   : ", dfk.executors[name].connected_workers)
+    print("Outstanding : ", dfk.executors[name].outstanding)
+
+    return True
+
+
+def test_parallel_for(n=2, sleep=1):
+    d = {}
+
+    start = time.time()
+    print("Priming ...")
+    double(10).result()
+    delta = time.time() - start
+    print("Priming done in {} seconds".format(delta))
+
+    start = time.time()
+    for i in range(0, n):
+        d[i] = platform(sleep=sleep)
+        # d[i] = double(i)
+        # time.sleep(0.01)
+    [d[i].result() for i in d]
+    delta = time.time() - start
+    print("Time to complete {} tasks: {:8.3f} s".format(n, delta))
+    print("Throughput : {:8.3f} Tasks/s".format(n / delta))
+    return d
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     parser = argparse.ArgumentParser()
+    parser.add_argument("-s", "--sleep", default="0")
     parser.add_argument("-c", "--count", default="10",
                         help="Count of apps to launch")
     parser.add_argument("-d", "--debug", action='store_true',
                         help="Count of apps to launch")
+    parser.add_argument("-f", "--fileconfig", required=True)
+
     args = parser.parse_args()
 
     if args.debug:
         parsl.set_stream_logger()
 
-    test_simple()
-    # test_fail_nowait(numtasks=int(args.count))
-    # test_no_deps(numtasks=int(args.count))
-    # test_fail_sequence(numtasks=int(args.count))
-    # test_deps(numtasks=int(args.count))
+    config = None
+    exec("from {} import config".format(args.fileconfig))
+    parsl.load(config)
+    # x = test_simple(int(args.count))
+    # x = test_imports()
+    x = test_parallel_for(int(args.count), float(args.sleep))
+    # x = test_platform(int(args.count), int(args.sleep))
+    # x = test_parallel_for(int(args.count))
+    # x = test_stdout()
+    # x = test_platform()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_error_handling/test_retries.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_retries.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,24 +105,7 @@
     try:
         os.remove(fname)
     except OSError:
         pass
     fu = succeed_on_retry(fname)
 
     fu.result()
-
-
-if __name__ == "__main__":
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default="10",
-                        help="Count of apps to launch")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    test_fail_nowait(numtasks=int(args.count))
-    # test_fail_delayed(numtasks=int(args.count))
-    # test_retry()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_flowcontrol/test_one_block.py` & `parsl-2023.6.5/parsl/tests/test_scaling/test_regression_1621.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_flowcontrol/test_python.py` & `parsl-2023.6.5/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,28 @@
+import parsl
 import pytest
+from parsl import python_app
+from parsl.tests.configs.local_threads import fresh_config
 
-from parsl.app.app import python_app
-from parsl.tests.configs.htex_local import fresh_config
 
+@pytest.mark.local
+def test_lazy_behavior():
+    """Testing that lazy errors work"""
 
-def local_config():
-    c = fresh_config()
-    c.executors[0].init_blocks = 0
-    return c
+    config = fresh_config()
+    parsl.load(config)
 
+    @python_app
+    def divide(a, b):
+        return a / b
 
-@python_app
-def py_app():
-    import platform
-    return "Hello from {0}".format(platform.uname())
+    futures = []
+    for i in range(0, 10):
+        futures.append(divide(10, 0))
 
+    for f in futures:
+        assert isinstance(f.exception(), ZeroDivisionError)
+        assert f.done()
 
-# @pytest.mark.local
-@pytest.mark.skip("Broke somewhere between PR #525 and PR #652")
-def test_python(N=2):
-    """Testing basic scaling|Python 0 -> 1 block """
-
-    results = {}
-    for i in range(0, N):
-        results[i] = py_app()
-
-    print("Waiting ....")
-    for i in range(0, N):
-        print(results[0].result())
-
-
-if __name__ == '__main__':
-
-    test_python()
+    parsl.dfk().cleanup()
+    parsl.clear()
+    return
```

### Comparing `parsl-2023.5.8/parsl/tests/test_flux.py` & `parsl-2023.6.5/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_manual/test_regression_220.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_monitoring/test_basic.py` & `parsl-2023.6.5/parsl/tests/test_monitoring/test_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,11 +79,7 @@
         assert c >= 2
 
         result = connection.execute(text("SELECT COUNT(*) FROM resource"))
         (c, ) = result.first()
         assert c >= 1
 
     logger.info("all done")
-
-
-if __name__ == "__main__":
-    test_row_counts()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2023.6.5/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2023.6.5/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2023.6.5/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_providers/test_local_provider.py` & `parsl-2023.6.5/parsl/tests/test_providers/test_local_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 Subsystem sftp {sftp_path}
 """
 
 
 # It would probably be better, when more formalized site testing comes into existence, to
 # use a site-testing provided server/configuration instead of the current scheme
 @pytest.mark.local
+@pytest.mark.sshd_required
 def test_ssh_channel():
     with tempfile.TemporaryDirectory() as config_dir:
         sshd_thread, priv_key, server_port = _start_sshd(config_dir)
         try:
             with tempfile.TemporaryDirectory() as remote_script_dir:
                 # The SSH library fails to add the new host key to the file if the file does not
                 # already exist, so create it here.
```

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_at_scale.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_at_scale.py`

 * *Files 22% similar despite different names*

```diff
@@ -57,24 +57,7 @@
     for i in range(0, n):
         x.extend([double(i)])
 
     ttc = time.time() - start
     print("Total time : ", ttc)
 
     return ttc
-
-
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default="10",
-                        help="Count of apps to launch")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    x = test_plain(int(args.count))
-    x = test_parallel(int(args.count))
-    x = test_parallel2(int(args.count))
```

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_basic.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_fail.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_fail.py`

 * *Files 26% similar despite different names*

```diff
@@ -100,23 +100,7 @@
     except parsl.dataflow.errors.DependencyError as e:
         print("Caught the right exception")
         print("Exception : ", e)
     except Exception as e:
         assert False, "Expected DependencyError but got: %s" % e
     else:
         raise RuntimeError("Expected DependencyError, but got no exception")
-
-
-if __name__ == "__main__":
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default="10",
-                        help="Count of apps to launch")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    test_no_deps(numtasks=int(args.count))
-    test_fail_sequence(numtasks=int(args.count))
```

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_futures.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_futures.py`

 * *Files 14% similar despite different names*

```diff
@@ -125,28 +125,7 @@
     assert os.path.basename(result) == output_f2, \
         "DataFuture did not return the filename, got : {0}".format(result)
 
     contents = get_contents(result)
     assert contents == '3', 'Output does not match expected "3", got: "{0}"'.format(
         result)
     return True
-
-
-if __name__ == '__main__':
-    parsl.clear()
-    parsl.load(config)
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default="10",
-                        help="Count of apps to launch")
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    # x = test_parallel_for(int(args.count))
-    # y = test_fut_case_2()
-    # y = test_fut_case_3()
-    y = test_fut_case_4()
-    # raise_error(0)
```

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,7 @@
     if parsl.dfk().checkpoint_mode is not None:
         # We explicit call checkpoint if checkpoint_mode is enabled covering
         # cases like manual/periodic where checkpointing may be deferred.
         parsl.dfk().checkpoint()
 
     time.sleep(0.2)  # Give enough time for task wipes to work
     assert x.tid not in parsl.dfk().tasks, "Task record should be wiped after task completion"
-
-
-if __name__ == '__main__':
-
-    from parsl.tests.configs.htex_local_alternate import config
-    parsl.load(config)
-    # parsl.load()
-    test_garbage_collect()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_join.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_join.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_outputs.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_outputs.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,18 +35,7 @@
 
     wait(all_futs)
 
     stdout_file_count = len(
         [item for item in os.listdir(outdir) if item.endswith('.txt')])
     assert stdout_file_count == n, "Only {}/{} files in '{}' ".format(
             len(os.listdir('outputs/')), n, os.listdir(outdir))
-
-
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-c", "--count", default="10",
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    x = test_launch_apps(2, "outputs")
-    # raise_error(0)
```

### Comparing `parsl-2023.5.8/parsl/tests/test_python_apps/test_simple.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_regression/test_1480.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_1480.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,11 +13,7 @@
 @pytest.mark.local
 def test_1480(size=10**6):
     x = compute_descript(size=size)
 
     # Before PR#1841 this would have raised a TypeError
     # Now, with the threshold increased this should not trigger any error
     assert len(x.result()) == size, "Lengths do not match"
-
-
-if __name__ == "__main__":
-    test_1480()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_regression/test_221.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_221.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,12 +23,7 @@
         f = slow_double(i)
         round_1.append(f)
 
     round_2 = []
     for i in round_1:
         f = slow_double(i)
         round_2.append(f)
-
-
-if __name__ == "__main__":
-
-    test_cleanup_behavior_221()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_regression/test_2652.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_2652.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_regression/test_69a.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_69a.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,13 +63,7 @@
     print("State_2 : ", state_2, "Fu:", fu.parent)
     assert "running" in state_2, "DataFuture should now be running"
 
     d_fu.result()
     state_3 = d_fu.__str__()
     print("State_3 : ", state_3, "Fu:", fu.parent)
     assert "finished" in state_3, "DataFuture should now be finished"
-
-
-if __name__ == "__main__":
-
-    test_immediate_datafuture()
-    test_delayed_datafuture()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_regression/test_69b.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_69b.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,17 +119,7 @@
 
     # This step *cat*s hello1.txt to hello2.txt
     hello2 = cat(inputs=[hello.outputs[0]], outputs=[File('hello2.txt')])
 
     hello2.result()
     with open(hello2.outputs[0].result().filepath, 'r') as f:
         print(f.read())
-
-
-if __name__ == "__main__":
-    parsl.clear()
-    parsl.load(config)
-    test_1()
-    test_2()
-    test_3()
-    test_4()
-    test_5()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_regression/test_854.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_854.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,13 +54,7 @@
     p = multiprocessing.Process(target=consumer, args=(task_q, result_q,))
     p.start()
     task_q.put('STOP')
     p.join()
     assert result_q.empty() is False, "Result queue should not be empty"
     qlen = result_q.qsize()
     assert qlen == x + 1, "Result queue should be {}; instead got {}".format(x + 1, qlen)
-
-
-if __name__ == "__main__":
-
-    test_mac_safe_queue()
-    test_mac_safe_queue_size()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2023.6.5/parsl/tests/test_scaling/test_scale_down.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_staging/staging_provider.py` & `parsl-2023.6.5/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_staging/test_1316.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_staging/test_docs_1.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import pytest
 
 from parsl.app.app import python_app
 from parsl.data_provider.files import File
-from parsl.tests.configs.local_threads_ftp_in_task import config
-
-local_config = config
+from parsl.tests.configs.local_threads_ftp_in_task import fresh_config as local_config
 
 
 @python_app
 def sort_strings(inputs=[], outputs=[]):
     with open(inputs[0].filepath, 'r') as u:
         strs = u.readlines()
         strs.sort()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_staging_globus.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,22 +65,7 @@
     assert unsorted_file.local_path is None, "Input file on local side has overridden local_path, file: {}".format(repr(unsorted_file))
 
     # use 'is' rather than '==' because specifically want to check
     # object identity rather than value equality
     assert sorted_file is result_file, "Result file is not the specified input-output file"
 
     assert result_file.local_path is None, "Result file on local side has overridden local_path, file: {}".format(repr(result_file))
-
-
-if __name__ == "__main__":
-
-    import argparse
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-d", "--debug", action='store_true',
-                        help="Count of apps to launch")
-    args = parser.parse_args()
-
-    if args.debug:
-        parsl.set_stream_logger()
-
-    test_stage_in_out_globus()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_staging/test_staging_https.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_staging/test_staging_https_in_task.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_staging_https_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_summary.py` & `parsl-2023.6.5/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/test_swift.py` & `parsl-2023.6.5/parsl/tests/test_swift.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pytest
 
-import parsl
-
 from parsl.executors.swift_t import TurbineExecutor
 
 
 def foo(x, y):
     return x * y
 
 
@@ -50,17 +48,7 @@
 @pytest.mark.skip('fails intermittently')
 def test_except():
     with pytest.raises(NameError):
         tex = TurbineExecutor()
         tex.start()
         x = tex.submit(bad_foo, 5, 10)
         x.result()
-
-
-if __name__ == "__main__":
-    parsl.set_stream_logger()
-
-    # test_simple()
-    # test_slow()
-    test_except()
-
-    print("Done")
```

### Comparing `parsl-2023.5.8/parsl/tests/test_thread_parallelism.py` & `parsl-2023.6.5/parsl/tests/test_thread_parallelism.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,13 +59,7 @@
     for i in d:
         i.result()
     end = time.time()
     delta = end - start
     print("Sleep time : {0}, expected ~{1}+/- 0.3s".format(delta, sleep_dur))
     assert delta > sleep_dur - tolerance, "Slept too little"
     assert delta < sleep_dur + tolerance, "Slept too much"
-
-
-if __name__ == "__main__":
-
-    test_parallel_sleep_bash()
-    test_parallel_sleep_python()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_threads/test_configs.py` & `parsl-2023.6.5/parsl/tests/test_threads/test_configs.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,12 +28,7 @@
     thread_count = len(set([item.result()['tid'] for item in d]))
     process_count = len(set([item.result()['pid'] for item in d]))
     assert thread_count <= config.executors[0].max_threads, "More threads than allowed"
     assert process_count == 1, "More processes than allowed"
     dfk.cleanup()
     parsl.clear()
     return d
-
-
-if __name__ == "__main__":
-
-    test_parallel_for()
```

### Comparing `parsl-2023.5.8/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,38 @@
+import argparse
+
 import parsl
-import pytest
-from parsl import python_app
-from parsl.tests.configs.local_threads import fresh_config
+from parsl.app.app import python_app
+from parsl.tests.configs.local_threads import config
 
 
-@pytest.mark.local
-def test_lazy_behavior():
-    """Testing that lazy errors work"""
+@python_app
+def increment(x):
+    return x + 1
 
-    config = fresh_config()
-    parsl.load(config)
 
-    @python_app
-    def divide(a, b):
-        return a / b
+@python_app
+def slow_increment(x, dur):
+    import time
+    time.sleep(dur)
+    return x + 1
 
-    futures = []
-    for i in range(0, 10):
-        futures.append(divide(10, 0))
 
-    for f in futures:
-        assert isinstance(f.exception(), ZeroDivisionError)
-        assert f.done()
+def test_increment(depth=2):
+    """Test simple pipeline A->B...->N
+    """
+    futs = {0: 0}
+    for i in range(1, depth):
+        futs[i] = increment(futs[i - 1])
 
-    parsl.dfk().cleanup()
-    parsl.clear()
-    return
+    print([futs[i].result() for i in futs if not isinstance(futs[i], int)])
 
 
-if __name__ == "__main__":
+def test_increment_slow(depth=2):
+    """Test simple pipeline A->B...->N with delay
+    """
+    futs = {0: 0}
+    for i in range(1, depth):
+        futs[i] = slow_increment(futs[i - 1], 0.5)
 
-    test_lazy_behavior()
+    print(futs[i])
+    print([futs[i].result() for i in futs if not isinstance(futs[i], int)])
```

### Comparing `parsl-2023.5.8/parsl/tests/workqueue_tests/htex_local.py` & `parsl-2023.6.5/parsl/tests/workqueue_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/workqueue_tests/wqex_condor.py` & `parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/tests/workqueue_tests/wqex_local.py` & `parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/usage_tracking/usage.py` & `parsl-2023.6.5/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl/utils.py` & `parsl-2023.6.5/parsl/utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.5.8/parsl.egg-info/PKG-INFO` & `parsl-2023.6.5/parsl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.5.8
+Version: 2023.6.5
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.05.08.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.06.05.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.5.8/parsl.egg-info/SOURCES.txt` & `parsl-2023.6.5/parsl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 parsl/data_provider/http.py
 parsl/data_provider/rsync.py
 parsl/data_provider/staging.py
 parsl/dataflow/__init__.py
 parsl/dataflow/dflow.py
 parsl/dataflow/errors.py
 parsl/dataflow/executor_status.py
-parsl/dataflow/flow_control.py
 parsl/dataflow/futures.py
 parsl/dataflow/job_error_handler.py
 parsl/dataflow/job_status_poller.py
 parsl/dataflow/memoization.py
 parsl/dataflow/rundirs.py
 parsl/dataflow/states.py
 parsl/dataflow/strategy.py
@@ -259,14 +258,15 @@
 parsl/tests/manual_tests/htex_local.py
 parsl/tests/manual_tests/test_ad_hoc_htex.py
 parsl/tests/manual_tests/test_basic.py
 parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
 parsl/tests/manual_tests/test_log_filter.py
 parsl/tests/manual_tests/test_memory_limits.py
 parsl/tests/manual_tests/test_oauth_ssh.py
+parsl/tests/manual_tests/test_regression_220.py
 parsl/tests/manual_tests/test_udp_simple.py
 parsl/tests/manual_tests/test_worker_count.py
 parsl/tests/site_tests/__init__.py
 parsl/tests/site_tests/site_config_selector.py
 parsl/tests/site_tests/test_provider.py
 parsl/tests/site_tests/test_site.py
 parsl/tests/sites/__init__.py
@@ -279,15 +279,14 @@
 parsl/tests/sites/test_start_method.py
 parsl/tests/sites/test_worker_info.py
 parsl/tests/sites/test_mpi/__init__.py
 parsl/tests/test_bash_apps/__init__.py
 parsl/tests/test_bash_apps/test_apptimeout.py
 parsl/tests/test_bash_apps/test_basic.py
 parsl/tests/test_bash_apps/test_error_codes.py
-parsl/tests/test_bash_apps/test_file_bug_1.py
 parsl/tests/test_bash_apps/test_keyword_overlaps.py
 parsl/tests/test_bash_apps/test_kwarg_storage.py
 parsl/tests/test_bash_apps/test_memoize.py
 parsl/tests/test_bash_apps/test_memoize_ignore_args.py
 parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
 parsl/tests/test_bash_apps/test_multiline.py
 parsl/tests/test_bash_apps/test_pipeline.py
@@ -303,14 +302,15 @@
 parsl/tests/test_checkpointing/test_regression_233.py
 parsl/tests/test_checkpointing/test_regression_239.py
 parsl/tests/test_checkpointing/test_task_exit.py
 parsl/tests/test_data/__init__.py
 parsl/tests/test_data/test_file.py
 parsl/tests/test_data/test_file_apps.py
 parsl/tests/test_data/test_file_staging.py
+parsl/tests/test_data/test_output_chain_filenames.py
 parsl/tests/test_docs/__init__.py
 parsl/tests/test_docs/test_from_slides.py
 parsl/tests/test_docs/test_tutorial_1.py
 parsl/tests/test_docs/test_workflow1.py
 parsl/tests/test_docs/test_workflow2.py
 parsl/tests/test_docs/test_workflow3.py
 parsl/tests/test_docs/test_workflow4.py
@@ -324,23 +324,20 @@
 parsl/tests/test_error_handling/test_resource_spec.py
 parsl/tests/test_error_handling/test_retries.py
 parsl/tests/test_error_handling/test_retry_handler.py
 parsl/tests/test_error_handling/test_retry_handler_failure.py
 parsl/tests/test_error_handling/test_serialization_fail.py
 parsl/tests/test_error_handling/test_wrap_with_logs.py
 parsl/tests/test_flowcontrol/__init__.py
-parsl/tests/test_flowcontrol/test_one_block.py
-parsl/tests/test_flowcontrol/test_python.py
-parsl/tests/test_manual/__init__.py
-parsl/tests/test_manual/test_regression_220.py
 parsl/tests/test_monitoring/__init__.py
 parsl/tests/test_monitoring/test_basic.py
 parsl/tests/test_monitoring/test_db_locks.py
 parsl/tests/test_monitoring/test_fuzz_zmq.py
 parsl/tests/test_monitoring/test_memoization_representation.py
+parsl/tests/test_monitoring/test_viz_colouring.py
 parsl/tests/test_providers/__init__.py
 parsl/tests/test_providers/test_local_provider.py
 parsl/tests/test_python_apps/__init__.py
 parsl/tests/test_python_apps/test_arg_input_types.py
 parsl/tests/test_python_apps/test_at_scale.py
 parsl/tests/test_python_apps/test_basic.py
 parsl/tests/test_python_apps/test_dep_standard_futures.py
@@ -372,17 +369,18 @@
 parsl/tests/test_regression/test_1653.py
 parsl/tests/test_regression/test_221.py
 parsl/tests/test_regression/test_226.py
 parsl/tests/test_regression/test_2652.py
 parsl/tests/test_regression/test_69a.py
 parsl/tests/test_regression/test_69b.py
 parsl/tests/test_regression/test_854.py
-parsl/tests/test_regression/test_97.py
+parsl/tests/test_regression/test_97_parallelism_0.py
 parsl/tests/test_regression/test_98.py
 parsl/tests/test_scaling/__init__.py
+parsl/tests/test_scaling/test_regression_1621.py
 parsl/tests/test_scaling/test_scale_down.py
 parsl/tests/test_staging/__init__.py
 parsl/tests/test_staging/staging_provider.py
 parsl/tests/test_staging/test_1316.py
 parsl/tests/test_staging/test_docs_1.py
 parsl/tests/test_staging/test_docs_2.py
 parsl/tests/test_staging/test_elaborate_noop_file.py
```

### Comparing `parsl-2023.5.8/parsl.egg-info/requires.txt` & `parsl-2023.6.5/parsl.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pyzmq>=17.1.2
 typeguard<3,>=2.10
-typing-extensions
+typing-extensions<5,>=4.6
 types-paramiko
 types-requests
 types-six
 six
 globus-sdk
 dill
 tblib
```

### Comparing `parsl-2023.5.8/setup.py` & `parsl-2023.6.5/setup.py`

 * *Files identical despite different names*

