# Comparing `tmp/angr-management-9.2.8.tar.gz` & `tmp/angr-management-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angr-management-9.2.8.tar", last modified: Tue Jun 28 17:04:18 2022, max compression
+gzip compressed data, was "angr-management-9.2.9.tar", last modified: Tue Jul  5 17:03:31 2022, max compression
```

## Comparing `angr-management-9.2.8.tar` & `angr-management-9.2.9.tar`

### file list

```diff
@@ -1,319 +1,319 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.398684 angr-management-9.2.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1326 2022-06-28 17:01:20.000000 angr-management-9.2.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)     2890 2022-06-28 17:04:18.398684 angr-management-9.2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     2452 2022-06-28 17:01:20.000000 angr-management-9.2.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.358680 angr-management-9.2.8/angr_management.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     2890 2022-06-28 17:04:17.000000 angr-management-9.2.8/angr_management.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)    11830 2022-06-28 17:04:18.000000 angr-management-9.2.8/angr_management.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-28 17:04:17.000000 angr-management-9.2.8/angr_management.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-06-28 17:04:17.000000 angr-management-9.2.8/angr_management.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      167 2022-06-28 17:04:18.000000 angr-management-9.2.8/angr_management.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       15 2022-06-28 17:04:18.000000 angr-management-9.2.8/angr_management.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.358680 angr-management-9.2.8/angrmanagement/
--rw-r--r--   0 vsts      (1001) docker     (121)      703 2022-06-28 17:01:35.000000 angr-management-9.2.8/angrmanagement/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9715 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.358680 angr-management-9.2.8/angrmanagement/config/
--rw-r--r--   0 vsts      (1001) docker     (121)      951 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10969 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/config/color_schemes.py
--rw-r--r--   0 vsts      (1001) docker     (121)      471 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/config/config_entry.py
--rw-r--r--   0 vsts      (1001) docker     (121)    20795 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/config/config_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.358680 angr-management-9.2.8/angrmanagement/daemon/
--rw-r--r--   0 vsts      (1001) docker     (121)      614 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/daemon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2437 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/daemon/client.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5011 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/daemon/server.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5077 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/daemon/url_handler.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.362681 angr-management-9.2.8/angrmanagement/data/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2054 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/breakpoint.py
--rw-r--r--   0 vsts      (1001) docker     (121)      881 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/function_graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)      222 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/highlight_region.py
--rw-r--r--   0 vsts      (1001) docker     (121)      259 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/indirect_jump.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13106 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/instance.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.366681 angr-management-9.2.8/angrmanagement/data/jobs/
--rw-r--r--   0 vsts      (1001) docker     (121)      536 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2844 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/cfg_generation.py
--rw-r--r--   0 vsts      (1001) docker     (121)      712 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/code_tagging.py
--rw-r--r--   0 vsts      (1001) docker     (121)      618 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/ddg_generation.py
--rw-r--r--   0 vsts      (1001) docker     (121)      862 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/decompile_function.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11053 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/dependency_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (121)      836 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/flirt_signature_recognition.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2836 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/job.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5652 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/loading.py
--rw-r--r--   0 vsts      (1001) docker     (121)      638 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/prototype_finding.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1435 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/simgr_explore.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1357 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/simgr_step.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3504 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/variable_recovery.py
--rw-r--r--   0 vsts      (1001) docker     (121)      494 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/jobs/vfg_generation.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1899 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/library_docs.py
--rw-r--r--   0 vsts      (1001) docker     (121)      784 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/log.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2700 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/object_container.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1143 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/data/trace.py
--rw-r--r--   0 vsts      (1001) docker     (121)      274 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.366681 angr-management-9.2.8/angrmanagement/logic/
--rw-r--r--   0 vsts      (1001) docker     (121)      476 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.366681 angr-management-9.2.8/angrmanagement/logic/debugger/
--rw-r--r--   0 vsts      (1001) docker     (121)       86 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/debugger/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10227 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/debugger/bintrace.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5703 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/debugger/debugger.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2855 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/debugger/simgr.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.366681 angr-management-9.2.8/angrmanagement/logic/disassembly/
--rw-r--r--   0 vsts      (1001) docker     (121)       92 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/disassembly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10684 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/disassembly/info_dock.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1624 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/disassembly/jump_history.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4969 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/singleton.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5971 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/threads.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5644 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/logic/url_scheme.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.370681 angr-management-9.2.8/angrmanagement/plugins/
--rw-r--r--   0 vsts      (1001) docker     (121)     2662 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.370681 angr-management-9.2.8/angrmanagement/plugins/ail2asm/
--rw-r--r--   0 vsts      (1001) docker     (121)       33 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/ail2asm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9827 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/ail2asm/ail2arm32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1330 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/ail2asm/asm_output.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.370681 angr-management-9.2.8/angrmanagement/plugins/angr_binsync/
--rw-r--r--   0 vsts      (1001) docker     (121)       77 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/angr_binsync/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6550 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/angr_binsync/binsync_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1111 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/angr_binsync/control_panel_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8809 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/angr_binsync/controller.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7128 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/base_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.370681 angr-management-9.2.8/angrmanagement/plugins/bughouse/
--rw-r--r--   0 vsts      (1001) docker     (121)       40 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/bughouse/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2312 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/bughouse/components.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.370681 angr-management-9.2.8/angrmanagement/plugins/bughouse/data/
--rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/bughouse/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1425 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/bughouse/data/component_tree.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.370681 angr-management-9.2.8/angrmanagement/plugins/bughouse/ui/
--rw-r--r--   0 vsts      (1001) docker     (121)      104 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/bughouse/ui/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3968 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/bughouse/ui/components_treeview.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7727 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/bughouse/ui/load_components_dialog.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.374682 angr-management-9.2.8/angrmanagement/plugins/chess_manager/
--rw-r--r--   0 vsts      (1001) docker     (121)      126 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7158 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/backend_selector_dialog.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10267 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/chess_connector.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8975 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/chess_url_handler.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5671 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/diagnose_handler.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7395 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/multi_poi.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7965 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/poi_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24203 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/qpoi_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11105 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/summary_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7972 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/target_selector.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4825 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/chess_manager/trace_statistics.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.374682 angr-management-9.2.8/angrmanagement/plugins/coverage/
--rw-r--r--   0 vsts      (1001) docker     (121)       37 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/coverage/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8376 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/coverage/coverage.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3825 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/coverage/parse_trace.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.374682 angr-management-9.2.8/angrmanagement/plugins/decompiler_poison/
--rw-r--r--   0 vsts      (1001) docker     (121)     6000 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/decompiler_poison/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.374682 angr-management-9.2.8/angrmanagement/plugins/dep_viewer/
--rw-r--r--   0 vsts      (1001) docker     (121)       41 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/dep_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1830 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/dep_viewer/dep_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2762 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/dep_viewer/sinks.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.374682 angr-management-9.2.8/angrmanagement/plugins/execution_statistics_viewer/
--rw-r--r--   0 vsts      (1001) docker     (121)       67 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/execution_statistics_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5234 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.374682 angr-management-9.2.8/angrmanagement/plugins/interaction_console/
--rw-r--r--   0 vsts      (1001) docker     (121)       52 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/interaction_console/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4522 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/interaction_console/interaction_console.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.374682 angr-management-9.2.8/angrmanagement/plugins/log_fatigue/
--rw-r--r--   0 vsts      (1001) docker     (121)       49 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/log_fatigue/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4341 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/log_fatigue/log_fatigue_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.374682 angr-management-9.2.8/angrmanagement/plugins/log_human_activities/
--rw-r--r--   0 vsts      (1001) docker     (121)       59 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/log_human_activities/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7136 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/log_human_activities/log_human_activities.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.374682 angr-management-9.2.8/angrmanagement/plugins/log_reverse_engineering/
--rw-r--r--   0 vsts      (1001) docker     (121)       72 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/log_reverse_engineering/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5421 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/log_reverse_engineering/log_reverse_engineering_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.378682 angr-management-9.2.8/angrmanagement/plugins/memory_checker/
--rw-r--r--   0 vsts      (1001) docker     (121)       42 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/memory_checker/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2632 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/memory_checker/memory_checker.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21617 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/plugin_manager.py
--rw-r--r--   0 vsts      (1001) docker     (121)      952 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/sample_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.378682 angr-management-9.2.8/angrmanagement/plugins/seed_table/
--rw-r--r--   0 vsts      (1001) docker     (121)       47 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/seed_table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4845 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/seed_table/seed_table.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12944 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/seed_table/seed_table_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.378682 angr-management-9.2.8/angrmanagement/plugins/source_importer/
--rw-r--r--   0 vsts      (1001) docker     (121)     1397 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/source_importer/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.378682 angr-management-9.2.8/angrmanagement/plugins/source_viewer/
--rw-r--r--   0 vsts      (1001) docker     (121)       53 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/source_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10698 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/source_viewer/source_viewer_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.378682 angr-management-9.2.8/angrmanagement/plugins/trace_viewer/
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/trace_viewer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8446 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8288 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/trace_viewer/chess_trace_list.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6034 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/trace_viewer/multi_trace.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19312 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/trace_viewer/qtrace_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17429 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/trace_viewer/trace_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9137 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/trace_viewer/trace_statistics.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.378682 angr-management-9.2.8/angrmanagement/plugins/varec/
--rw-r--r--   0 vsts      (1001) docker     (121)       25 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/varec/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6826 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/plugins/varec/varec.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.354680 angr-management-9.2.8/angrmanagement/resources/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.378682 angr-management-9.2.8/angrmanagement/resources/fonts/
--rw-r--r--   0 vsts      (1001) docker     (121)   340712 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/fonts/DejaVuSansMono.ttf
--rw-r--r--   0 vsts      (1001) docker     (121)   212880 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.382683 angr-management-9.2.8/angrmanagement/resources/images/
--rw-r--r--   0 vsts      (1001) docker     (121)   100896 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/angr-ds.png
--rw-r--r--   0 vsts      (1001) docker     (121)   143434 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/angr-splash.png
--rw-r--r--   0 vsts      (1001) docker     (121)   165662 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/angr.ico
--rw-r--r--   0 vsts      (1001) docker     (121)    79574 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/angr.png
--rw-r--r--   0 vsts      (1001) docker     (121)    11090 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/benchmark-icon.png
--rw-r--r--   0 vsts      (1001) docker     (121)     9627 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/error-icon.png
--rw-r--r--   0 vsts      (1001) docker     (121)     9671 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/toolbar-docker-open.png
--rw-r--r--   0 vsts      (1001) docker     (121)   176067 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/toolbar-file-open.ico
--rw-r--r--   0 vsts      (1001) docker     (121)   103065 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/toolbar-file-save.png
--rw-r--r--   0 vsts      (1001) docker     (121)     1219 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/toolbar-forward.png
--rw-r--r--   0 vsts      (1001) docker     (121)     1200 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/toolbar-previous.png
--rw-r--r--   0 vsts      (1001) docker     (121)     1891 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/toolbar-show-alignment.png
--rw-r--r--   0 vsts      (1001) docker     (121)    25190 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/resources/images/warning-icon.png
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.382683 angr-management-9.2.8/angrmanagement/ui/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.382683 angr-management-9.2.8/angrmanagement/ui/css/
--rw-r--r--   0 vsts      (1001) docker     (121)     4565 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/css/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.386683 angr-management-9.2.8/angrmanagement/ui/dialogs/
--rw-r--r--   0 vsts      (1001) docker     (121)      201 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1900 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/about.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4620 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/breakpoint.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5083 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/data_dep_graph_search.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6031 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/dependson.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2274 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/env_config.py
--rw-r--r--   0 vsts      (1001) docker     (121)      818 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/fs_mount.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1778 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/func_doc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4458 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/hook.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/input_prompt.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2560 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/jumpto.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11634 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/load_binary.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1529 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/load_docker_prompt.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4186 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/load_plugins.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14786 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/new_state.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6964 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/preferences.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3483 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/rename.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3341 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/rename_label.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9980 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/rename_node.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6381 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/retype_node.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2765 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/set_comment.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10891 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/socket_config.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5811 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/type_editor.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2095 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/dialogs/xref.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.386683 angr-management-9.2.8/angrmanagement/ui/documents/
--rw-r--r--   0 vsts      (1001) docker     (121)       42 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/documents/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6239 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/documents/qcodedocument.py
--rw-r--r--   0 vsts      (1001) docker     (121)    29514 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/main_window.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.386683 angr-management-9.2.8/angrmanagement/ui/menus/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      740 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/analyze_menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3796 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/disasm_insn_context_menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2418 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/disasm_label_context_menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2914 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/disasm_options_menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2204 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/file_menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)      585 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/function_context_menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)      487 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/help_menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)      823 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/log_menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4512 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)      292 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/plugin_menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4495 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/menus/view_menu.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1518 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/toolbar_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.386683 angr-management-9.2.8/angrmanagement/ui/toolbars/
--rw-r--r--   0 vsts      (1001) docker     (121)      171 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/toolbars/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8331 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/toolbars/debug_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1154 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/toolbars/file_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1104 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/toolbars/function_table_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3447 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/toolbars/nav_toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2923 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/toolbars/toolbar.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7634 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/view_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.390683 angr-management-9.2.8/angrmanagement/ui/views/
--rw-r--r--   0 vsts      (1001) docker     (121)      841 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5770 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/breakpoints_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6038 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/call_explorer_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18766 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/code_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2984 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/console_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9708 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/data_dep_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4441 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/dep_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)    31617 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/disassembly_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2927 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/functions_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)    71115 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/hex_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)    20630 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/interaction_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)      924 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/log_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1796 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/patches_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5822 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/proximity_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5050 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/registers_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4243 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/stack_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1204 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/states_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3736 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/strings_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4306 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/symexec_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1011 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/trace_map_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4567 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/traces_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5054 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/types_view.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6790 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/views/view.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.398684 angr-management-9.2.8/angrmanagement/ui/widgets/
--rw-r--r--   0 vsts      (1001) docker     (121)      552 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2288 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/filesystem_table.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1523 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qaddress_input.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5894 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qast_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13279 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qblock.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24658 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qblock_code.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2058 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qblock_label.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19367 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qccode_edit.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6186 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qccode_highlighter.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1343 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qcolor_option.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1907 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qconstraint_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10302 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qdatadep_graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7017 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qdatadepgraph_block.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8824 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qdecomp_options.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4398 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qdep_graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7823 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qdepgraph_block.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2942 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qdisasm_base_control.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11574 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qdisasm_graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4860 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qdisasm_statusbar.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17966 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qfeature_map.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2717 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qfiledesc_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1375 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qfunction_combobox.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5763 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qfunction_header.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16829 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qfunction_table.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10584 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qgraph.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11370 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qgraph_arrow.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1148 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qgraph_object.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8987 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qinst_annotation.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10812 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qinstruction.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1588 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qipython_widget.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19773 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qlinear_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8075 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qlog_widget.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9636 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qmemory_data_block.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5425 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qmemory_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9561 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qminimap.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18993 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qoperand.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4661 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qpatch_table.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4586 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qpathtree.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5164 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qphivariable.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5068 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qproximity_graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11938 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qproximitygraph_block.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3802 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qregister_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9458 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qsimulation_manager_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11780 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qsimulation_managers.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1053 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qsmart_dockwidget.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5389 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qstate_block.py
--rw-r--r--   0 vsts      (1001) docker     (121)      764 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qstate_combobox.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5862 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qstate_table.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6697 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qstring_table.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4644 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qsymexec_graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15284 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qtrace_map.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4536 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qtypedef.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2987 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qunknown_block.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3423 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qvariable.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2392 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qvextemps_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10273 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/qxref_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1642 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/widgets/state_inspector.py
--rw-r--r--   0 vsts      (1001) docker     (121)    34080 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/ui/workspace.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:18.398684 angr-management-9.2.8/angrmanagement/utils/
--rw-r--r--   0 vsts      (1001) docker     (121)     8081 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      650 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/block_objects.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3521 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/cfg.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1585 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/edge.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2380 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/env.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1285 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/func.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11547 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)    30880 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/graph_layouter.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2434 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/io.py
--rw-r--r--   0 vsts      (1001) docker     (121)    32985 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/namegen.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11733 2022-06-28 17:01:20.000000 angr-management-9.2.8/angrmanagement/utils/tree_graph_layouter.py
--rw-r--r--   0 vsts      (1001) docker     (121)       81 2022-06-28 17:01:35.000000 angr-management-9.2.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)      933 2022-06-28 17:04:18.402684 angr-management-9.2.8/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.109898 angr-management-9.2.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1326 2022-07-05 17:01:27.000000 angr-management-9.2.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)     2890 2022-07-05 17:03:31.109898 angr-management-9.2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     2452 2022-07-05 17:01:27.000000 angr-management-9.2.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.069897 angr-management-9.2.9/angr_management.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2890 2022-07-05 17:03:31.000000 angr-management-9.2.9/angr_management.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)    11830 2022-07-05 17:03:31.000000 angr-management-9.2.9/angr_management.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-05 17:03:31.000000 angr-management-9.2.9/angr_management.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-07-05 17:03:31.000000 angr-management-9.2.9/angr_management.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      170 2022-07-05 17:03:31.000000 angr-management-9.2.9/angr_management.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       15 2022-07-05 17:03:31.000000 angr-management-9.2.9/angr_management.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.069897 angr-management-9.2.9/angrmanagement/
+-rw-r--r--   0 vsts      (1001) docker     (121)      703 2022-07-05 17:01:34.000000 angr-management-9.2.9/angrmanagement/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9715 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.069897 angr-management-9.2.9/angrmanagement/config/
+-rw-r--r--   0 vsts      (1001) docker     (121)      951 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10969 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/config/color_schemes.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      471 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/config/config_entry.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    21509 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/config/config_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.069897 angr-management-9.2.9/angrmanagement/daemon/
+-rw-r--r--   0 vsts      (1001) docker     (121)      614 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/daemon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2437 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/daemon/client.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5011 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/daemon/server.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5077 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/daemon/url_handler.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.069897 angr-management-9.2.9/angrmanagement/data/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2054 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/breakpoint.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      881 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/function_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      222 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/highlight_region.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      259 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/indirect_jump.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13106 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/instance.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.073897 angr-management-9.2.9/angrmanagement/data/jobs/
+-rw-r--r--   0 vsts      (1001) docker     (121)      536 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2844 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/cfg_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      712 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/code_tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      618 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/ddg_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      862 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/decompile_function.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11053 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/dependency_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      836 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/flirt_signature_recognition.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2836 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/job.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5652 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/loading.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      638 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/prototype_finding.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1435 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/simgr_explore.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1357 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/simgr_step.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3504 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/variable_recovery.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      494 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/jobs/vfg_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1899 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/library_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      784 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/log.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2700 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/object_container.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1143 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/data/trace.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      274 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.073897 angr-management-9.2.9/angrmanagement/logic/
+-rw-r--r--   0 vsts      (1001) docker     (121)      476 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.073897 angr-management-9.2.9/angrmanagement/logic/debugger/
+-rw-r--r--   0 vsts      (1001) docker     (121)       86 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/debugger/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10227 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/debugger/bintrace.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5703 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/debugger/debugger.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2855 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/debugger/simgr.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.073897 angr-management-9.2.9/angrmanagement/logic/disassembly/
+-rw-r--r--   0 vsts      (1001) docker     (121)       92 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/disassembly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10684 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/disassembly/info_dock.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1624 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/disassembly/jump_history.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4969 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/singleton.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5971 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/threads.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5644 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/logic/url_scheme.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.077897 angr-management-9.2.9/angrmanagement/plugins/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2662 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.077897 angr-management-9.2.9/angrmanagement/plugins/ail2asm/
+-rw-r--r--   0 vsts      (1001) docker     (121)       33 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/ail2asm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9827 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/ail2asm/ail2arm32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1330 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/ail2asm/asm_output.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.077897 angr-management-9.2.9/angrmanagement/plugins/angr_binsync/
+-rw-r--r--   0 vsts      (1001) docker     (121)       77 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/angr_binsync/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6550 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/angr_binsync/binsync_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1111 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/angr_binsync/control_panel_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8809 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/angr_binsync/controller.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7128 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/base_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.077897 angr-management-9.2.9/angrmanagement/plugins/bughouse/
+-rw-r--r--   0 vsts      (1001) docker     (121)       40 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/bughouse/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2312 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/bughouse/components.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.077897 angr-management-9.2.9/angrmanagement/plugins/bughouse/data/
+-rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/bughouse/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1425 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/bughouse/data/component_tree.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.077897 angr-management-9.2.9/angrmanagement/plugins/bughouse/ui/
+-rw-r--r--   0 vsts      (1001) docker     (121)      104 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/bughouse/ui/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3968 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/bughouse/ui/components_treeview.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7727 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/bughouse/ui/load_components_dialog.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.077897 angr-management-9.2.9/angrmanagement/plugins/chess_manager/
+-rw-r--r--   0 vsts      (1001) docker     (121)      126 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7158 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/backend_selector_dialog.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10267 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/chess_connector.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9140 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/chess_url_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5671 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/diagnose_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7395 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/multi_poi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7965 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/poi_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    24203 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/qpoi_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11105 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/summary_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7972 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/target_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4825 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/chess_manager/trace_statistics.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/coverage/
+-rw-r--r--   0 vsts      (1001) docker     (121)       37 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/coverage/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8376 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/coverage/coverage.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3825 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/coverage/parse_trace.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/decompiler_poison/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6000 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/decompiler_poison/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/dep_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (121)       41 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/dep_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1830 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/dep_viewer/dep_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2762 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/dep_viewer/sinks.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/execution_statistics_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (121)       67 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/execution_statistics_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5234 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/interaction_console/
+-rw-r--r--   0 vsts      (1001) docker     (121)       52 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/interaction_console/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4522 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/interaction_console/interaction_console.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/log_fatigue/
+-rw-r--r--   0 vsts      (1001) docker     (121)       49 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/log_fatigue/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4341 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/log_fatigue/log_fatigue_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/log_human_activities/
+-rw-r--r--   0 vsts      (1001) docker     (121)       59 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/log_human_activities/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7136 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/log_human_activities/log_human_activities.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/log_reverse_engineering/
+-rw-r--r--   0 vsts      (1001) docker     (121)       72 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/log_reverse_engineering/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5421 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/log_reverse_engineering/log_reverse_engineering_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/memory_checker/
+-rw-r--r--   0 vsts      (1001) docker     (121)       42 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/memory_checker/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2632 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/memory_checker/memory_checker.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    21617 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/plugin_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      952 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/sample_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/seed_table/
+-rw-r--r--   0 vsts      (1001) docker     (121)       47 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/seed_table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4845 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/seed_table/seed_table.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12944 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/seed_table/seed_table_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/source_importer/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1397 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/source_importer/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.081898 angr-management-9.2.9/angrmanagement/plugins/source_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (121)       53 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/source_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10698 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/source_viewer/source_viewer_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.085898 angr-management-9.2.9/angrmanagement/plugins/trace_viewer/
+-rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/trace_viewer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8446 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8288 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/trace_viewer/chess_trace_list.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6034 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/trace_viewer/multi_trace.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19312 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/trace_viewer/qtrace_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17429 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/trace_viewer/trace_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9137 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/trace_viewer/trace_statistics.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.085898 angr-management-9.2.9/angrmanagement/plugins/varec/
+-rw-r--r--   0 vsts      (1001) docker     (121)       25 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/varec/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6849 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/plugins/varec/varec.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.065897 angr-management-9.2.9/angrmanagement/resources/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.085898 angr-management-9.2.9/angrmanagement/resources/fonts/
+-rw-r--r--   0 vsts      (1001) docker     (121)   340712 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/fonts/DejaVuSansMono.ttf
+-rw-r--r--   0 vsts      (1001) docker     (121)   212880 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.089898 angr-management-9.2.9/angrmanagement/resources/images/
+-rw-r--r--   0 vsts      (1001) docker     (121)   100896 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/angr-ds.png
+-rw-r--r--   0 vsts      (1001) docker     (121)   143434 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/angr-splash.png
+-rw-r--r--   0 vsts      (1001) docker     (121)   165662 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/angr.ico
+-rw-r--r--   0 vsts      (1001) docker     (121)    79574 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/angr.png
+-rw-r--r--   0 vsts      (1001) docker     (121)    11090 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/benchmark-icon.png
+-rw-r--r--   0 vsts      (1001) docker     (121)     9627 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/error-icon.png
+-rw-r--r--   0 vsts      (1001) docker     (121)     9671 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/toolbar-docker-open.png
+-rw-r--r--   0 vsts      (1001) docker     (121)   176067 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/toolbar-file-open.ico
+-rw-r--r--   0 vsts      (1001) docker     (121)   103065 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/toolbar-file-save.png
+-rw-r--r--   0 vsts      (1001) docker     (121)     1219 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/toolbar-forward.png
+-rw-r--r--   0 vsts      (1001) docker     (121)     1200 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/toolbar-previous.png
+-rw-r--r--   0 vsts      (1001) docker     (121)     1891 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/toolbar-show-alignment.png
+-rw-r--r--   0 vsts      (1001) docker     (121)    25190 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/resources/images/warning-icon.png
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.089898 angr-management-9.2.9/angrmanagement/ui/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.089898 angr-management-9.2.9/angrmanagement/ui/css/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4565 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/css/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.093898 angr-management-9.2.9/angrmanagement/ui/dialogs/
+-rw-r--r--   0 vsts      (1001) docker     (121)      201 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1900 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/about.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4620 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/breakpoint.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5083 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/data_dep_graph_search.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6031 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/dependson.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2274 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/env_config.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      818 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/fs_mount.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1778 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/func_doc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4458 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/hook.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/input_prompt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2560 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/jumpto.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11634 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/load_binary.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1529 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/load_docker_prompt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4186 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/load_plugins.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14786 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/new_state.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6964 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/preferences.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3483 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/rename.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3341 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/rename_label.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9980 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/rename_node.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6381 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/retype_node.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2765 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/set_comment.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10891 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/socket_config.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5811 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/type_editor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2095 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/dialogs/xref.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.093898 angr-management-9.2.9/angrmanagement/ui/documents/
+-rw-r--r--   0 vsts      (1001) docker     (121)       42 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/documents/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6239 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/documents/qcodedocument.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    27126 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/main_window.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.093898 angr-management-9.2.9/angrmanagement/ui/menus/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      740 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/analyze_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3796 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/disasm_insn_context_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2418 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/disasm_label_context_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2914 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/disasm_options_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2204 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/file_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      585 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/function_context_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      487 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/help_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      823 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/log_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4512 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      292 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/plugin_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4495 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/menus/view_menu.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1518 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/toolbar_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.097898 angr-management-9.2.9/angrmanagement/ui/toolbars/
+-rw-r--r--   0 vsts      (1001) docker     (121)      171 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/toolbars/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8331 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/toolbars/debug_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1154 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/toolbars/file_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1104 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/toolbars/function_table_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3447 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/toolbars/nav_toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2923 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/toolbars/toolbar.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7634 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/view_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.101898 angr-management-9.2.9/angrmanagement/ui/views/
+-rw-r--r--   0 vsts      (1001) docker     (121)      841 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5770 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/breakpoints_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6038 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/call_explorer_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18766 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/code_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2984 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/console_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9708 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/data_dep_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4441 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/dep_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    31617 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/disassembly_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2847 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/functions_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    71115 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/hex_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    20630 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/interaction_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      924 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/log_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1796 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/patches_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5822 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/proximity_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5050 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/registers_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4243 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/stack_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1204 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/states_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3736 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/strings_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4306 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/symexec_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1011 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/trace_map_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4567 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/traces_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5054 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/types_view.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6790 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/views/view.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.109898 angr-management-9.2.9/angrmanagement/ui/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (121)      552 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2288 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/filesystem_table.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1523 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qaddress_input.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5894 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qast_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13279 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qblock.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    24658 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qblock_code.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2058 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qblock_label.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19367 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qccode_edit.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6186 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qccode_highlighter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1343 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qcolor_option.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1907 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qconstraint_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10302 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qdatadep_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7017 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qdatadepgraph_block.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8824 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qdecomp_options.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4398 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qdep_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7823 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qdepgraph_block.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2942 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qdisasm_base_control.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11574 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qdisasm_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4860 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qdisasm_statusbar.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17966 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qfeature_map.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2717 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qfiledesc_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1375 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qfunction_combobox.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5763 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qfunction_header.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16829 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qfunction_table.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10584 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qgraph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11370 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qgraph_arrow.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1148 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qgraph_object.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8987 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qinst_annotation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10812 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qinstruction.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1588 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qipython_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19773 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qlinear_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8075 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qlog_widget.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9636 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qmemory_data_block.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5425 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qmemory_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9561 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qminimap.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18993 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qoperand.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4661 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qpatch_table.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4586 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qpathtree.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5164 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qphivariable.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5068 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qproximity_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11938 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qproximitygraph_block.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3802 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qregister_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9458 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qsimulation_manager_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11780 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qsimulation_managers.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1053 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qsmart_dockwidget.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5389 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qstate_block.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      764 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qstate_combobox.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5862 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qstate_table.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6697 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qstring_table.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4644 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qsymexec_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15284 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qtrace_map.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4536 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qtypedef.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2987 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qunknown_block.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3423 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qvariable.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2392 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qvextemps_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10273 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/qxref_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1642 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/widgets/state_inspector.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    34094 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/ui/workspace.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:31.109898 angr-management-9.2.9/angrmanagement/utils/
+-rw-r--r--   0 vsts      (1001) docker     (121)     8081 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      650 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/block_objects.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3521 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/cfg.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1585 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/edge.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2380 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/env.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1285 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/func.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11547 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    30880 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/graph_layouter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2434 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/io.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    32985 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/namegen.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11733 2022-07-05 17:01:27.000000 angr-management-9.2.9/angrmanagement/utils/tree_graph_layouter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       81 2022-07-05 17:01:34.000000 angr-management-9.2.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)      936 2022-07-05 17:03:31.109898 angr-management-9.2.9/setup.cfg
```

### Comparing `angr-management-9.2.8/LICENSE` & `angr-management-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/PKG-INFO` & `angr-management-9.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angr-management
-Version: 9.2.8
+Version: 9.2.9
 Summary: GUI for angr
 Home-page: https://github.com/angr/angr-management
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `angr-management-9.2.8/README.md` & `angr-management-9.2.9/README.md`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angr_management.egg-info/PKG-INFO` & `angr-management-9.2.9/angr_management.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angr-management
-Version: 9.2.8
+Version: 9.2.9
 Summary: GUI for angr
 Home-page: https://github.com/angr/angr-management
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `angr-management-9.2.8/angr_management.egg-info/SOURCES.txt` & `angr-management-9.2.9/angr_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/__init__.py` & `angr-management-9.2.9/angrmanagement/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "9.2.8"
+__version__ = "9.2.9"
 
 # Hack used to work around the slow-responsiveness issue with the GUI
 # PySide2 5.14.2 solves this problem but it introduces other bugs
 # See https://bugreports.qt.io/browse/PYSIDE-803
 try:
     import PySide2
     version = [int(k) for k in PySide2.__version__.split(".")[:4]]
```

### Comparing `angr-management-9.2.8/angrmanagement/__main__.py` & `angr-management-9.2.9/angrmanagement/__main__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/config/__init__.py` & `angr-management-9.2.9/angrmanagement/config/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/config/color_schemes.py` & `angr-management-9.2.9/angrmanagement/config/color_schemes.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/config/config_manager.py` & `angr-management-9.2.9/angrmanagement/config/config_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,60 @@
 import os
 import logging
 import re
-from typing import Union
+from typing import Union, Type, Any, Optional
 
-import toml
+import tomlkit
+import tomlkit.exceptions
+import tomlkit.items
 from PySide2.QtGui import QFont, QFontMetricsF, QColor
 from PySide2.QtWidgets import QApplication, QMessageBox
 
 from ..utils.env import app_root
 from .config_entry import ConfigurationEntry as CE
 
 
 _l = logging.getLogger(__name__)
 color_re = re.compile('[0-9a-fA-F]+')
 
+
+def tomltype2pytype(v, ty: Optional[Type]) -> Any:
+    if ty is str:
+        if not isinstance(v, tomlkit.items.String):
+            raise TypeError()
+        return v.value
+    elif ty is int:
+        if not isinstance(v, tomlkit.items.Integer):
+            raise TypeError()
+        return v.value
+    elif ty is list:
+        if not isinstance(v, tomlkit.items.Array):
+            raise TypeError()
+        return [ tomltype2pytype(v_, None) for v_ in v.value ]
+    return v.value
+
+
 def color_parser(config_option, value) -> Union[QColor, None]:
     if not isinstance(value, str) \
        or not color_re.match(value) \
        or len(value) not in (3, 6, 8, 12):
         _l.error('Failed to parse value %r as rgb color for option %s', value, config_option)
         return None
 
     return QColor('#' + value)
 
+
 def color_serializer(config_option, value: QColor) -> str:
     if not isinstance(value, QColor):
         _l.error("Failed to serialize value %r as rgb color for option %s", value, config_option)
         return None
 
     return f'{value.alpha():02x}{value.red():02x}{value.green():02x}{value.blue():02x}'
 
+
 def font_parser(config_option, value) -> Union[QFont, None]:
     if not isinstance(value, str) or 'px ' not in value:
         _l.error('Failed to parse value %r as font for option %s', value, config_option)
         return None
 
     parts = value.split('px ', 1)
     try:
@@ -205,17 +226,17 @@
 
     # Recent
     CE("recent_files", list, []),
 ]
 
 
 class ConfigurationManager: # pylint: disable=assigning-non-slot
-    '''
+    """
     Globe Configuration Manager for UI configuration with save/load function
-    '''
+    """
     __slots__ = ('_entries',
                  '_disasm_font', '_disasm_font_metrics', '_disasm_font_height',
                  '_disasm_font_width', '_disasm_font_ascent',
                  '_symexec_font', '_symexec_font_metrics', '_symexec_font_height',
                  '_symexec_font_width', '_symexec_font_ascent',
                  '_code_font', '_code_font_metrics', '_code_font_height',
                  '_code_font_width', '_code_font_ascent', '_last_used_directory'
@@ -413,40 +434,43 @@
     @classmethod
     def parse(cls, f, ignore_unknown_entries: bool=True):
         entry_map = {}
         for entry in ENTRIES:
             entry_map[entry.name] = entry.copy()
 
         try:
-            loaded = toml.load(f)
+            loaded = tomlkit.load(f)
 
             for k, v in loaded.items():
                 if k not in entry_map:
                     if ignore_unknown_entries:
                         _l.warning('Unknown configuration option \'%s\'. Ignoring...', k)
                         continue
                     # default to a string
                     entry = CE(k, str, v)
                     entry_map[k] = entry
 
                 entry = entry_map[k]
 
                 if entry.type_ in data_serializers:
                     v = data_serializers[entry.type_][0](k, v)
-                if v is None:
-                    continue
-                if type(v) is not entry.type_:
-                    _l.warning('Value \'%s\' for configuration option \'%s\' has type \'%s\', '\
-                        ' expected type \'%s\'. Ignoring...',
-                        v, k, type(v), entry.type_
-                    )
-                    continue
+                    if v is None:
+                        continue
+                else:
+                    try:
+                        v = tomltype2pytype(v, entry.type_)
+                    except TypeError:
+                        _l.warning('Value \'%s\' for configuration option \'%s\' has type \'%s\', '
+                                   'expected type \'%s\'. Ignoring...',
+                                   v, k, type(v), entry.type_
+                        )
+                        continue
                 entry.value = v
-        except toml.TomlDecodeError as ex:
-            _l.error('Failed to parse configuration file: \'%s\'. Continuing with default options...', ex.msg)
+        except tomlkit.exceptions.ParseError:
+            _l.error('Failed to parse configuration file: \'%s\'. Continuing with default options...', exc_info=True)
 
         return cls(entry_map)
 
     @classmethod
     def parse_file(cls, path: str, ignore_unknown_entries: bool=True):
         with open(path, 'r', encoding="utf-8") as f:
             return cls.parse(f, ignore_unknown_entries=ignore_unknown_entries)
@@ -455,15 +479,15 @@
         out = {}
         for k, v in self._entries.items():
             v = v.value
             while type(v) in data_serializers:
                 v = data_serializers[type(v)][1](k, v)
             out[k] = v
 
-        toml.dump(out, f)
+        tomlkit.dump(out, f)
 
     def save_file(self, path:str):
         with open(path, 'w', encoding="utf-8") as f:
             self.save(f)
 
     def attempt_importing_initial_config(self) -> bool:
         """
```

### Comparing `angr-management-9.2.8/angrmanagement/daemon/__init__.py` & `angr-management-9.2.9/angrmanagement/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/daemon/client.py` & `angr-management-9.2.9/angrmanagement/daemon/client.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/daemon/server.py` & `angr-management-9.2.9/angrmanagement/daemon/server.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/daemon/url_handler.py` & `angr-management-9.2.9/angrmanagement/daemon/url_handler.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/breakpoint.py` & `angr-management-9.2.9/angrmanagement/data/breakpoint.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/function_graph.py` & `angr-management-9.2.9/angrmanagement/data/function_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/instance.py` & `angr-management-9.2.9/angrmanagement/data/instance.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/__init__.py` & `angr-management-9.2.9/angrmanagement/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/cfg_generation.py` & `angr-management-9.2.9/angrmanagement/data/jobs/cfg_generation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/code_tagging.py` & `angr-management-9.2.9/angrmanagement/data/jobs/code_tagging.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/ddg_generation.py` & `angr-management-9.2.9/angrmanagement/data/jobs/ddg_generation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/decompile_function.py` & `angr-management-9.2.9/angrmanagement/data/jobs/decompile_function.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/dependency_analysis.py` & `angr-management-9.2.9/angrmanagement/data/jobs/dependency_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/flirt_signature_recognition.py` & `angr-management-9.2.9/angrmanagement/data/jobs/flirt_signature_recognition.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/job.py` & `angr-management-9.2.9/angrmanagement/data/jobs/job.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/loading.py` & `angr-management-9.2.9/angrmanagement/data/jobs/loading.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/prototype_finding.py` & `angr-management-9.2.9/angrmanagement/data/jobs/prototype_finding.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/simgr_explore.py` & `angr-management-9.2.9/angrmanagement/data/jobs/simgr_explore.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/simgr_step.py` & `angr-management-9.2.9/angrmanagement/data/jobs/simgr_step.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/jobs/variable_recovery.py` & `angr-management-9.2.9/angrmanagement/data/jobs/variable_recovery.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/library_docs.py` & `angr-management-9.2.9/angrmanagement/data/library_docs.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/log.py` & `angr-management-9.2.9/angrmanagement/data/log.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/object_container.py` & `angr-management-9.2.9/angrmanagement/data/object_container.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/data/trace.py` & `angr-management-9.2.9/angrmanagement/data/trace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/logic/debugger/bintrace.py` & `angr-management-9.2.9/angrmanagement/logic/debugger/bintrace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/logic/debugger/debugger.py` & `angr-management-9.2.9/angrmanagement/logic/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/logic/debugger/simgr.py` & `angr-management-9.2.9/angrmanagement/logic/debugger/simgr.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/logic/disassembly/info_dock.py` & `angr-management-9.2.9/angrmanagement/logic/disassembly/info_dock.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/logic/disassembly/jump_history.py` & `angr-management-9.2.9/angrmanagement/logic/disassembly/jump_history.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/logic/singleton.py` & `angr-management-9.2.9/angrmanagement/logic/singleton.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/logic/threads.py` & `angr-management-9.2.9/angrmanagement/logic/threads.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/logic/url_scheme.py` & `angr-management-9.2.9/angrmanagement/logic/url_scheme.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/__init__.py` & `angr-management-9.2.9/angrmanagement/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/ail2asm/ail2arm32.py` & `angr-management-9.2.9/angrmanagement/plugins/ail2asm/ail2arm32.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/ail2asm/asm_output.py` & `angr-management-9.2.9/angrmanagement/plugins/ail2asm/asm_output.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/angr_binsync/binsync_plugin.py` & `angr-management-9.2.9/angrmanagement/plugins/angr_binsync/binsync_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/angr_binsync/control_panel_view.py` & `angr-management-9.2.9/angrmanagement/plugins/angr_binsync/control_panel_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/angr_binsync/controller.py` & `angr-management-9.2.9/angrmanagement/plugins/angr_binsync/controller.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/base_plugin.py` & `angr-management-9.2.9/angrmanagement/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/bughouse/components.py` & `angr-management-9.2.9/angrmanagement/plugins/bughouse/components.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/bughouse/data/component_tree.py` & `angr-management-9.2.9/angrmanagement/plugins/bughouse/data/component_tree.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/bughouse/ui/components_treeview.py` & `angr-management-9.2.9/angrmanagement/plugins/bughouse/ui/components_treeview.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/bughouse/ui/load_components_dialog.py` & `angr-management-9.2.9/angrmanagement/plugins/bughouse/ui/load_components_dialog.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/chess_manager/backend_selector_dialog.py` & `angr-management-9.2.9/angrmanagement/plugins/chess_manager/backend_selector_dialog.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/chess_manager/chess_connector.py` & `angr-management-9.2.9/angrmanagement/plugins/chess_manager/chess_connector.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/chess_manager/chess_url_handler.py` & `angr-management-9.2.9/angrmanagement/plugins/chess_manager/chess_url_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+# pylint:disable=global-statement,missing-class-docstring,no-self-use,unspecified-encoding
 import os
 import sys
 import subprocess
 import logging
 from pathlib import Path
 from typing import Tuple, Optional
 
-import toml
+import tomlkit
+import tomlkit.exceptions
 from xdg import BaseDirectory
 from PySide2.QtWidgets import QApplication
 from PySide2.QtWidgets import QMessageBox, QFileDialog
 
 from angrmanagement.plugins import BasePlugin
 from angrmanagement.daemon.url_handler import UrlActionBase, register_url_action
 from angrmanagement.daemon.server import register_server_exposed_method
 
 _l = logging.getLogger(name=__name__)
 
 # we probably want to put this feature into angr management
 _app = None
+
 def tmp_app():
     global _app
     if _app is None:
         _app = QApplication()
     return _app
 
 
@@ -83,46 +86,47 @@
     def _get_rootdir_config_path(self) -> str:
         am_root = BaseDirectory.save_config_path('angr-management')
         if am_root is not None:
             rootdirs_path = os.path.join(am_root, "challenge_rootdirs.toml")
             return rootdirs_path
         raise ValueError("Cannot get the configuration file root directory for angr-management.")
 
-    def _get_rootdir(self, target_uuid: str, challenge_name: str, source_file: str) -> Tuple[Optional[str],Optional[str]]:
+    def _get_rootdir(self, target_uuid: str, challenge_name: str,
+                     source_file: str) -> Tuple[Optional[str],Optional[str]]:
         rootdirs_path = self._get_rootdir_config_path()
         # load it if it exists
         entries = { }
         if os.path.isfile(rootdirs_path):
             with open(rootdirs_path, "r") as f:
                 try:
-                    entries = toml.load(f)
-                except toml.TomlDecodeError:
+                    entries = tomlkit.load(f)
+                except tomlkit.exceptions.ParseError:
                     _l.error("Cannot decode rootdirs file %s. Ignore existing content.",
                              rootdirs_path)
 
         dir_path = None
         if 'uuid_to_rootdir' in entries:
             if target_uuid in entries['uuid_to_rootdir']:
                 # yes there is already one
-                dir_path = entries['uuid_to_rootdir'][target_uuid]
+                dir_path = entries['uuid_to_rootdir'][target_uuid].value
             else:
                 dir_path = None
 
         while True:
             # test the existing dir_path for the existence of the file
             if dir_path:
                 if not source_file:
                     # source file is not specified. we take whatever is there!
                     return dir_path, None
 
                 file_found = False
                 full_path = None
 
                 source_file_name = os.path.basename(source_file)
-                for base, directories, files in os.walk(dir_path):
+                for base, _, files in os.walk(dir_path):
                     if source_file_name in files:
                         # check the full path
                         full_path = os.path.normpath(os.path.join(base, source_file_name))
                         if full_path.endswith(source_file):
                             # found it!
                             file_found = True
                             break
@@ -157,29 +161,29 @@
     def _save_rootdir(self, target_uuid: str, challenge_name: str, root_dir: str):
         rootdirs_path = self._get_rootdir_config_path()
         # load it
         entries = { }
         if os.path.isfile(rootdirs_path):
             with open(rootdirs_path, "r") as f:
                 try:
-                    entries = toml.load(f)
-                except toml.TomlDecodeError:
+                    entries = tomlkit.load(f)
+                except tomlkit.exceptions.ParseError:
                     _l.error("Cannot decode rootdirs file %s. Ignore existing content.",
                              rootdirs_path)
 
         if 'uuid_to_challenge' not in entries:
             entries['uuid_to_challenge'] = { }
         if 'uuid_to_rootdir' not in entries:
             entries['uuid_to_rootdir'] = { }
         entries['uuid_to_challenge'][target_uuid] = challenge_name
         entries['uuid_to_rootdir'][target_uuid] = root_dir
 
         # store it
         with open(rootdirs_path, "w") as f:
-            toml.dump(entries, f)
+            tomlkit.dump(entries, f)
 
     def _vscode_path(self) -> Optional[str]:
         if sys.platform == "win32":
             default_locations = [
                 os.path.join(os.getenv("LOCALAPPDATA"), "Programs", "Microsoft VS Code"),
             ]
             default_locations += os.getenv("PATH").split(";")
```

### Comparing `angr-management-9.2.8/angrmanagement/plugins/chess_manager/diagnose_handler.py` & `angr-management-9.2.9/angrmanagement/plugins/chess_manager/diagnose_handler.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/chess_manager/multi_poi.py` & `angr-management-9.2.9/angrmanagement/plugins/chess_manager/multi_poi.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/chess_manager/poi_plugin.py` & `angr-management-9.2.9/angrmanagement/plugins/chess_manager/poi_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/chess_manager/qpoi_viewer.py` & `angr-management-9.2.9/angrmanagement/plugins/chess_manager/qpoi_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/chess_manager/summary_view.py` & `angr-management-9.2.9/angrmanagement/plugins/chess_manager/summary_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/chess_manager/target_selector.py` & `angr-management-9.2.9/angrmanagement/plugins/chess_manager/target_selector.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/chess_manager/trace_statistics.py` & `angr-management-9.2.9/angrmanagement/plugins/chess_manager/trace_statistics.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/coverage/coverage.py` & `angr-management-9.2.9/angrmanagement/plugins/coverage/coverage.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/coverage/parse_trace.py` & `angr-management-9.2.9/angrmanagement/plugins/coverage/parse_trace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/decompiler_poison/__init__.py` & `angr-management-9.2.9/angrmanagement/plugins/decompiler_poison/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/dep_viewer/dep_plugin.py` & `angr-management-9.2.9/angrmanagement/plugins/dep_viewer/dep_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/dep_viewer/sinks.py` & `angr-management-9.2.9/angrmanagement/plugins/dep_viewer/sinks.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py` & `angr-management-9.2.9/angrmanagement/plugins/execution_statistics_viewer/execution_statistics_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/interaction_console/interaction_console.py` & `angr-management-9.2.9/angrmanagement/plugins/interaction_console/interaction_console.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/log_fatigue/log_fatigue_plugin.py` & `angr-management-9.2.9/angrmanagement/plugins/log_fatigue/log_fatigue_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/log_human_activities/log_human_activities.py` & `angr-management-9.2.9/angrmanagement/plugins/log_human_activities/log_human_activities.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/log_reverse_engineering/log_reverse_engineering_plugin.py` & `angr-management-9.2.9/angrmanagement/plugins/log_reverse_engineering/log_reverse_engineering_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/memory_checker/memory_checker.py` & `angr-management-9.2.9/angrmanagement/plugins/memory_checker/memory_checker.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/plugin_manager.py` & `angr-management-9.2.9/angrmanagement/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/sample_plugin.py` & `angr-management-9.2.9/angrmanagement/plugins/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/seed_table/seed_table.py` & `angr-management-9.2.9/angrmanagement/plugins/seed_table/seed_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/seed_table/seed_table_plugin.py` & `angr-management-9.2.9/angrmanagement/plugins/seed_table/seed_table_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/source_importer/__init__.py` & `angr-management-9.2.9/angrmanagement/plugins/source_importer/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/source_viewer/source_viewer_plugin.py` & `angr-management-9.2.9/angrmanagement/plugins/source_viewer/source_viewer_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py` & `angr-management-9.2.9/angrmanagement/plugins/trace_viewer/afl_qemu_bitmap.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/trace_viewer/chess_trace_list.py` & `angr-management-9.2.9/angrmanagement/plugins/trace_viewer/chess_trace_list.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/trace_viewer/multi_trace.py` & `angr-management-9.2.9/angrmanagement/plugins/trace_viewer/multi_trace.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/trace_viewer/qtrace_viewer.py` & `angr-management-9.2.9/angrmanagement/plugins/trace_viewer/qtrace_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/trace_viewer/trace_plugin.py` & `angr-management-9.2.9/angrmanagement/plugins/trace_viewer/trace_plugin.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/trace_viewer/trace_statistics.py` & `angr-management-9.2.9/angrmanagement/plugins/trace_viewer/trace_statistics.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/plugins/varec/varec.py` & `angr-management-9.2.9/angrmanagement/plugins/varec/varec.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                                  "Error in variable name prediction",
                                  "Failed to predict names for all variables involved.",
                                  QMessageBox.Ok
                                  )
 
             return
 
-        varname_blacklist = {'UNK', 'null', "true", "false", }
+        varname_blacklist = {'UNK', 'null', "true", "false", "return", "do", "while"}
         varname_to_predicted = defaultdict(list)
 
         # handle failure cases
         if 'code' not in result or not result['code']:
             self._restore_stage(view)
             QMessageBox.critical(self.workspace._main_window,
                                  "Error in variable name prediction",
```

### Comparing `angr-management-9.2.8/angrmanagement/resources/fonts/DejaVuSansMono.ttf` & `angr-management-9.2.9/angrmanagement/resources/fonts/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf` & `angr-management-9.2.9/angrmanagement/resources/fonts/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/angr-ds.png` & `angr-management-9.2.9/angrmanagement/resources/images/angr-ds.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/angr-splash.png` & `angr-management-9.2.9/angrmanagement/resources/images/angr-splash.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/angr.ico` & `angr-management-9.2.9/angrmanagement/resources/images/angr.ico`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/angr.png` & `angr-management-9.2.9/angrmanagement/resources/images/angr.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/benchmark-icon.png` & `angr-management-9.2.9/angrmanagement/resources/images/benchmark-icon.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/error-icon.png` & `angr-management-9.2.9/angrmanagement/resources/images/error-icon.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/toolbar-docker-open.png` & `angr-management-9.2.9/angrmanagement/resources/images/toolbar-docker-open.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/toolbar-file-open.ico` & `angr-management-9.2.9/angrmanagement/resources/images/toolbar-file-open.ico`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/toolbar-file-save.png` & `angr-management-9.2.9/angrmanagement/resources/images/toolbar-file-save.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/toolbar-forward.png` & `angr-management-9.2.9/angrmanagement/resources/images/toolbar-forward.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/toolbar-previous.png` & `angr-management-9.2.9/angrmanagement/resources/images/toolbar-previous.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/toolbar-show-alignment.png` & `angr-management-9.2.9/angrmanagement/resources/images/toolbar-show-alignment.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/resources/images/warning-icon.png` & `angr-management-9.2.9/angrmanagement/resources/images/warning-icon.png`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/css/__init__.py` & `angr-management-9.2.9/angrmanagement/ui/css/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/about.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/about.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/breakpoint.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/breakpoint.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/data_dep_graph_search.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/data_dep_graph_search.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/dependson.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/dependson.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/env_config.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/env_config.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/fs_mount.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/fs_mount.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/func_doc.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/func_doc.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/hook.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/hook.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/input_prompt.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/input_prompt.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/jumpto.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/jumpto.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/load_binary.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/load_binary.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/load_docker_prompt.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/load_docker_prompt.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/load_plugins.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/load_plugins.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/new_state.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/new_state.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/preferences.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/preferences.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/rename.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/rename.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/rename_label.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/rename_label.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/rename_node.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/rename_node.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/retype_node.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/retype_node.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/set_comment.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/set_comment.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/socket_config.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/socket_config.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/type_editor.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/type_editor.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/dialogs/xref.py` & `angr-management-9.2.9/angrmanagement/ui/dialogs/xref.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/documents/qcodedocument.py` & `angr-management-9.2.9/angrmanagement/ui/documents/qcodedocument.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/main_window.py` & `angr-management-9.2.9/angrmanagement/ui/main_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sys
 import time
 from functools import partial
 from typing import Optional, TYPE_CHECKING
 
 from PySide2.QtWidgets import QMainWindow, QTabWidget, QFileDialog, QProgressBar, QProgressDialog
 from PySide2.QtWidgets import QMessageBox, QShortcut, QTabBar
-from PySide2.QtGui import QResizeEvent, QIcon, QDesktopServices, QKeySequence
-from PySide2.QtCore import Qt, QSize, QEvent, QTimer, QUrl
+from PySide2.QtGui import QIcon, QDesktopServices, QKeySequence
+from PySide2.QtCore import Qt, QSize, QEvent, QUrl
 
 import angr
 import angr.flirt
 
 try:
     from angr.angrdb import AngrDB
 except ImportError:
@@ -398,23 +398,14 @@
                                         "The following exception occurred:\n"
                                         + str(ex))
 
     #
     # Event
     #
 
-    def resizeEvent(self, event: QResizeEvent):
-        """
-
-        :param event:
-        :return:
-        """
-
-        self._recalculate_view_sizes(event.oldSize())
-
     def closeEvent(self, event):
 
         # Ask if the user wants to save things
         if self.workspace.instance is not None and not self.workspace.instance.project.am_none:
             msgbox = QMessageBox()
             msgbox.setWindowTitle("Save database")
             msgbox.setText("angr management is about to exit. Do you want to save the database?")
@@ -759,64 +750,7 @@
             self.workspace.instance.pseudocode_variable_kb,
         ],
                     extra_info=extra_info,
                     )
 
         self.workspace.instance.database_path = file_path
         return True
-
-    def _recalculate_view_sizes(self, old_size):
-        adjustable_dockable_views = [dock for dock in self.workspace.view_manager.docks
-                                     if dock.widget().default_docking_position in ('left', 'bottom',)]
-
-        if not adjustable_dockable_views:
-            return
-
-        for dock in adjustable_dockable_views:
-            widget = dock.widget()
-
-            if old_size.width() < 0:
-                dock.old_size = widget.sizeHint()
-                continue
-
-            if old_size != self.size():
-                # calculate the width ratio
-
-                if widget.default_docking_position == 'left':
-                    # we want to adjust the width
-                    ratio = widget.old_width * 1.0 / old_size.width()
-                    new_width = int(self.width() * ratio)
-                    widget.width_hint = new_width
-                    widget.updateGeometry()
-                elif widget.default_docking_position == 'bottom':
-                    # we want to adjust the height
-                    ratio = widget.old_height * 1.0 / old_size.height()
-                    new_height = int(self.height() * ratio)
-                    widget.height_hint = new_height
-                    widget.updateGeometry()
-
-                dock.old_size = widget.size()
-
-    def _resize_dock_widget(self, dock_widget, new_width, new_height):
-
-        original_size = dock_widget.size()
-        original_min = dock_widget.minimumSize()
-        original_max = dock_widget.maximumSize()
-
-        dock_widget.resize(new_width, new_height)
-
-        if new_width != original_size.width():
-            if original_size.width() > new_width:
-                dock_widget.setMaximumWidth(new_width)
-            else:
-                dock_widget.setMinimumWidth(new_width)
-
-        if new_height != original_size.height():
-            if original_size.height() > new_height:
-                dock_widget.setMaximumHeight(new_height)
-            else:
-                dock_widget.setMinimumHeight(new_height)
-
-        dock_widget.original_min = original_min
-        dock_widget.original_max = original_max
-
-        QTimer.singleShot(1, dock_widget.restore_original_size)
```

### Comparing `angr-management-9.2.8/angrmanagement/ui/menus/analyze_menu.py` & `angr-management-9.2.9/angrmanagement/ui/menus/analyze_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/menus/disasm_insn_context_menu.py` & `angr-management-9.2.9/angrmanagement/ui/menus/disasm_insn_context_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/menus/disasm_label_context_menu.py` & `angr-management-9.2.9/angrmanagement/ui/menus/disasm_label_context_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/menus/disasm_options_menu.py` & `angr-management-9.2.9/angrmanagement/ui/menus/disasm_options_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/menus/file_menu.py` & `angr-management-9.2.9/angrmanagement/ui/menus/file_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/menus/function_context_menu.py` & `angr-management-9.2.9/angrmanagement/ui/menus/function_context_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/menus/log_menu.py` & `angr-management-9.2.9/angrmanagement/ui/menus/log_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/menus/menu.py` & `angr-management-9.2.9/angrmanagement/ui/menus/menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/menus/view_menu.py` & `angr-management-9.2.9/angrmanagement/ui/menus/view_menu.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/toolbar_manager.py` & `angr-management-9.2.9/angrmanagement/ui/toolbar_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/toolbars/debug_toolbar.py` & `angr-management-9.2.9/angrmanagement/ui/toolbars/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/toolbars/file_toolbar.py` & `angr-management-9.2.9/angrmanagement/ui/toolbars/file_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/toolbars/function_table_toolbar.py` & `angr-management-9.2.9/angrmanagement/ui/toolbars/function_table_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/toolbars/nav_toolbar.py` & `angr-management-9.2.9/angrmanagement/ui/toolbars/nav_toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/toolbars/toolbar.py` & `angr-management-9.2.9/angrmanagement/ui/toolbars/toolbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/view_manager.py` & `angr-management-9.2.9/angrmanagement/ui/view_manager.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/__init__.py` & `angr-management-9.2.9/angrmanagement/ui/views/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/breakpoints_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/breakpoints_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/call_explorer_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/call_explorer_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/code_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/code_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/console_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/console_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/data_dep_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/data_dep_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/dep_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/dep_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/disassembly_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/disassembly_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/functions_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/functions_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._function_table = None  # type: QFunctionTable
         self._status_label = None
 
         self.workspace.instance.cfg.am_subscribe(self.reload)
 
         self._init_widgets()
 
-        self.width_hint = 100
+        self.width_hint = 300
         self.height_hint = 0
         self.updateGeometry()
 
         self.function_count = None
         self._displayed_function_count = None
 
         self.reload()
@@ -41,17 +41,14 @@
         self._displayed_function_count = count
         self._refresh_status_label()
 
     def reload(self):
         if not self.workspace.instance.cfg.am_none:
             self._function_table.function_manager = self.workspace.instance.kb.functions
 
-    def minimumSizeHint(self, *args, **kwargs):
-        return QSize(100, 500)
-
     def subscribe_func_select(self, callback):
         """
         Appends the provided function to the list of callbacks to be called when a function is selected in the
         functions table. The callback's only parameter is the `angr.knowledge_plugins.functions.function.Function`
         :param callback: The callback function to call, which must accept **kwargs
         """
         self._function_table.subscribe_func_select(callback)
```

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/hex_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/hex_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/interaction_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/interaction_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/log_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/log_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/patches_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/patches_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/proximity_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/proximity_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/registers_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/registers_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/stack_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/stack_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/states_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/states_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/strings_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/strings_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/symexec_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/symexec_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/trace_map_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/trace_map_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/traces_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/traces_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/types_view.py` & `angr-management-9.2.9/angrmanagement/ui/views/types_view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/views/view.py` & `angr-management-9.2.9/angrmanagement/ui/views/view.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/__init__.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/filesystem_table.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/filesystem_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qaddress_input.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qaddress_input.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qast_viewer.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qast_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qblock.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qblock.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qblock_code.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qblock_code.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qblock_label.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qblock_label.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qccode_edit.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qccode_edit.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qccode_highlighter.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qccode_highlighter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qcolor_option.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qcolor_option.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qconstraint_viewer.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qconstraint_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qdatadep_graph.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qdatadep_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qdatadepgraph_block.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qdatadepgraph_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qdecomp_options.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qdecomp_options.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qdep_graph.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qdep_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qdepgraph_block.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qdepgraph_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qdisasm_base_control.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qdisasm_base_control.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qdisasm_graph.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qdisasm_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qdisasm_statusbar.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qdisasm_statusbar.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qfeature_map.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qfeature_map.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qfiledesc_viewer.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qfiledesc_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qfunction_combobox.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qfunction_combobox.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qfunction_header.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qfunction_header.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qfunction_table.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qfunction_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qgraph.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qgraph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qgraph_arrow.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qgraph_arrow.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qgraph_object.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qgraph_object.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qinst_annotation.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qinst_annotation.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qinstruction.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qinstruction.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qipython_widget.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qipython_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qlinear_viewer.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qlinear_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qlog_widget.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qlog_widget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qmemory_data_block.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qmemory_data_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qmemory_viewer.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qmemory_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qminimap.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qminimap.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qoperand.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qoperand.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qpatch_table.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qpatch_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qpathtree.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qpathtree.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qphivariable.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qphivariable.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qproximity_graph.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qproximity_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qproximitygraph_block.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qproximitygraph_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qregister_viewer.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qregister_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qsimulation_manager_viewer.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qsimulation_manager_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qsimulation_managers.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qsimulation_managers.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qsmart_dockwidget.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qsmart_dockwidget.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qstate_block.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qstate_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qstate_combobox.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qstate_combobox.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qstate_table.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qstate_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qstring_table.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qstring_table.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qsymexec_graph.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qsymexec_graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qtrace_map.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qtrace_map.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qtypedef.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qtypedef.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qunknown_block.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qunknown_block.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qvariable.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qvariable.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qvextemps_viewer.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qvextemps_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/qxref_viewer.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/qxref_viewer.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/widgets/state_inspector.py` & `angr-management-9.2.9/angrmanagement/ui/widgets/state_inspector.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/ui/workspace.py` & `angr-management-9.2.9/angrmanagement/ui/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,18 +380,18 @@
 
     def set_comment(self, addr, comment_text):
         kb = self.instance.project.kb
         exists = addr in kb.comments
 
         # callback
         if comment_text is None and exists:
-            self.plugins.handle_comment_changed(addr, "", False, False)
+            self.plugins.handle_comment_changed(addr, "", False, False, False)
             del kb.comments[addr]
         else:
-            self.plugins.handle_comment_changed(addr, comment_text, not exists, False)
+            self.plugins.handle_comment_changed(addr, comment_text, not exists, False, False)
             kb.comments[addr] = comment_text
 
         # callback first
         # TODO: can this be removed?
         if self.instance.set_comment_callback:
             self.instance.set_comment_callback(addr=addr, comment_text=comment_text)
```

### Comparing `angr-management-9.2.8/angrmanagement/utils/__init__.py` & `angr-management-9.2.9/angrmanagement/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/utils/block_objects.py` & `angr-management-9.2.9/angrmanagement/utils/block_objects.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/utils/cfg.py` & `angr-management-9.2.9/angrmanagement/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/utils/edge.py` & `angr-management-9.2.9/angrmanagement/utils/edge.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/utils/env.py` & `angr-management-9.2.9/angrmanagement/utils/env.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/utils/func.py` & `angr-management-9.2.9/angrmanagement/utils/func.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/utils/graph.py` & `angr-management-9.2.9/angrmanagement/utils/graph.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/utils/graph_layouter.py` & `angr-management-9.2.9/angrmanagement/utils/graph_layouter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/utils/io.py` & `angr-management-9.2.9/angrmanagement/utils/io.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/utils/namegen.py` & `angr-management-9.2.9/angrmanagement/utils/namegen.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/angrmanagement/utils/tree_graph_layouter.py` & `angr-management-9.2.9/angrmanagement/utils/tree_graph_layouter.py`

 * *Files identical despite different names*

### Comparing `angr-management-9.2.8/setup.cfg` & `angr-management-9.2.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 license_files = LICENSE
 description = GUI for angr
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 install_requires = 
-	angr[angrDB] == 9.2.8
+	angr[angrDB] == 9.2.9
 	qtconsole
 	ipython
 	PySide2 > 5.14.2.1
-	toml
+	tomlkit
 	pyxdg
 	requests[socks]
 	pyqodeng.core
 	qtterm
 	getmac
 	QtAwesome
 python_requires = >= 3.8
```

