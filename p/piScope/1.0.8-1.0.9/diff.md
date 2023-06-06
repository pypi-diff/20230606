# Comparing `tmp/piScope-1.0.8.tar.gz` & `tmp/piScope-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piScope-1.0.8.tar", last modified: Fri Apr  7 18:25:59 2023, max compression
+gzip compressed data, was "piScope-1.0.9.tar", last modified: Sun Apr  9 14:10:58 2023, max compression
```

## Comparing `piScope-1.0.8.tar` & `piScope-1.0.9.tar`

### file list

```diff
@@ -1,892 +1,892 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.442841 piScope-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-07 18:25:47.000000 piScope-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-07 18:25:59.442841 piScope-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-07 18:25:47.000000 piScope-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.318839 piScope-1.0.8/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.322839 piScope-1.0.8/python/ifigure/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.322839 piScope-1.0.8/python/ifigure/add_on/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.322839 piScope-1.0.8/python/ifigure/add_on/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.322839 piScope-1.0.8/python/ifigure/add_on/model/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/efit_afile.py
--rw-r--r--   0 runner    (1001) docker     (123)    25060 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/efit_gfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/efit_pfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/idl_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/matlab_mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/mdsplus_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/name_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/netcdf4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.322839 piScope-1.0.8/python/ifigure/add_on/model/module/subs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/subs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/subs/dwscope_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/subs/dwscope_subs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/subs/idl_save_subs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/subs/mdsplus_tree_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/subs/netcdf_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/module/tsc_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.322839 piScope-1.0.8/python/ifigure/add_on/model/script/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/model/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.326840 piScope-1.0.8/python/ifigure/add_on/setting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/setting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.326840 piScope-1.0.8/python/ifigure/add_on/setting/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/setting/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/setting/module/cmod_pyro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/setting/module/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/setting/module/mdsplus_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/setting/module/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.326840 piScope-1.0.8/python/ifigure/add_on/setting/script/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/setting/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.326840 piScope-1.0.8/python/ifigure/add_on/solver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.326840 piScope-1.0.8/python/ifigure/add_on/solver/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.326840 piScope-1.0.8/python/ifigure/add_on/solver/script/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/script/cost_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/script/def_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/script/genray_loki.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/script/merge_sol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/script/merge_sol_parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/script/merge_sol_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/script/run_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/script/run_parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/add_on/solver/script/run_stdsolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.326840 piScope-1.0.8/python/ifigure/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/example/cmod_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/example/gl_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/example/plot_demos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.326840 piScope-1.0.8/python/ifigure/extra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/extra/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    79953 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/ifigure_app.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/ifigure_app_macport_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/ifigure_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    43923 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.330839 piScope-1.0.8/python/ifigure/matplotlib_mod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40807 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/art3d_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)    58925 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/axes3d_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/axes_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/backend_wx_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/backend_wxagg_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/backend_wxagg_gl_12.py
--rw-r--r--   0 runner    (1001) docker     (123)    91905 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/backend_wxagg_gl_15.py
--rw-r--r--   0 runner    (1001) docker     (123)    18636 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/backend_wxagg_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/canvas_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/cz_linecollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/depthmap_12.frag
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/depthmap_12.vert
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/depthmap_15.frag
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/depthmap_15.vert
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/figure_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    84975 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/glcanvas_12.py
--rw-r--r--   0 runner    (1001) docker     (123)    98007 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/glcanvas_15.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/is_supported_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/lines_15.frag
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/lines_15.geom
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/lines_15.vert
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/mpl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/renderer_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/simple.frag
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/simple_12.vert
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/simple_15.geom
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/simple_15.vert
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/simple_oit.frag
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/simple_oit_12.frag
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/simple_oit_15.frag
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/simple_oit_final.frag
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/triangles_15.geom
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/matplotlib_mod/triplot_mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.338840 piScope-1.0.8/python/ifigure/mdsplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/direct_jobrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/direct_jobrunner_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    24134 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/dlg_mdssession.py
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/dlg_mdssession_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/dlg_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/dlg_setting2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/event_listener_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/event_listener_proc_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/event_listener_proc_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/fake_jobrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    49430 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/fig_mds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/fig_mdsbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/fig_mdsdata.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/filebacked_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/filed_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/import_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mds_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mds_mpth_directworker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mds_mpth_proxyworker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mds_mpth_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mds_sp_directworker.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mds_sp_echobackworker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mds_sp_proxyworker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mds_sp_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mdsplus_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mdsplus_gateway_th.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mdsplusr.py
--rw-r--r--   0 runner    (1001) docker     (123)   106154 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mdsscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mdsscope_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mdsscope_nw.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mp_global.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/mp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/proxy_jobrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/proxyworker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/shot_number_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mdsplus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.346840 piScope-1.0.8/python/ifigure/mto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/abs_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    25917 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/axis_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/axis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    92651 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_axline.py
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_axlinec.py
--rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_axspan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_axspanc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_book.py
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    33310 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    33524 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_eps.py
--rw-r--r--   0 runner    (1001) docker     (123)    19833 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_grp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_hist.py
--rw-r--r--   0 runner    (1001) docker     (123)    34413 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_legend.py
--rw-r--r--   0 runner    (1001) docker     (123)    58299 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    24743 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    40355 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_plotc.py
--rw-r--r--   0 runner    (1001) docker     (123)    28205 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_solid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)    26081 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_tricontour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_tripcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_triplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fig_trisurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/figobj_gpholder.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/figobj_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/fileholder.py
--rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/generic_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/gl_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)    47705 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/hg_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    22311 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/project_top.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/py_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    42110 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/py_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/py_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23838 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/py_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/py_extfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/py_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/py_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/py_moduled.py
--rw-r--r--   0 runner    (1001) docker     (123)    36206 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/py_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/py_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/threaded_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    75704 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/treedict.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/treedict_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/treelink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/mto/triangle_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/numerical_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/piscope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.346840 piScope-1.0.8/python/ifigure/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.346840 piScope-1.0.8/python/ifigure/resources/icon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.366840 piScope-1.0.8/python/ifigure/resources/icon/16x16/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/a.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/amode.png
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrow_firstpage.png
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrow_fwdplay.png
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrow_fwdstep.png
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrow_lastpage.png
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrow_revplay.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrow_revstep.png
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrowleft.png
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrowmove.png
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrowmove_all.png
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/arrowright.png
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/axes.png
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/book.png
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/box.png
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/circle.png
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/close.png
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/cog.png
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/colorbar.png
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/copy.png
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/ctrl.png
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/cursor.png
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/curve.png
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/data.png
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/eps.png
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/expand.png
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/external_overlay.png
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/file.png
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/fill.png
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/flip_cp_side.png
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/folder.png
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/folder_ext.png
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/folder_hg.png
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/form.png
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/grid.png
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/group.png
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/help.png
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/hg.png
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/image.png
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/legend.png
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/line.png
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/log.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/mail_pic.png
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/margin.png
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/mdsplus.png
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/minus_phi.png
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/minus_theta.png
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/model.png
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/model_hg.png
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/next.png
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/no_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/open_book.png
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/page.png
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/paste.png
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/pi.png
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/pifile.png
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/plot.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/plot1.png
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/plotc.png
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/plus_phi.png
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/plus_theta.png
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/pmode.png
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/previous.png
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/reset.png
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/resetrange_all.png
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/samex.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/samey.png
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/save_pic.png
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/script.png
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/script_ext.png
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/script_link.png
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/select.png
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/setting.png
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/shift_cp.png
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/shift_phi.png
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/shift_theta.png
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/smode.png
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/solver.png
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/stop_play.png
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/sun.png
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/suppress.png
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/surf.png
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/t.png
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/text.png
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/three_d.png
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/threed_rot.png
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/timetrace.png
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/trash.png
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/variable.png
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/world_link.png
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/xauto.png
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/xlog.png
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/xy_plane.png
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/xz_plane.png
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/yauto.png
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/ylog.png
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/yz_plane.png
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom2.png
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom2menu.png
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom2minus.png
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom2minusmenu.png
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom3minus.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.370840 piScope-1.0.8/python/ifigure/resources/icon/24x24/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/a.png
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/axes.png
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/book.png
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/cog.png
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/copy.png
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/cursor.png
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/expand.png
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/file.png
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/fill.png
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/folder.png
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/form.png
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/help.png
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/log.png
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/mail_pic.png
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/model.png
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/next.png
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/no_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/open_book.png
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/page.png
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/paste.png
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/pifile.png
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/plot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/plot1.png
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/previous.png
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/save_pic.png
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/setting.png
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/sun.png
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/surf.png
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/text.png
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/threed_rot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/trash.png
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/24x24/world_link.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.374840 piScope-1.0.8/python/ifigure/resources/icon/32x32/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/a.png
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/axes.png
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/book.png
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/cog.png
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/copy.png
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/cursor.png
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/data.png
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/expand.png
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/external_overlay.png
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/file.png
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/fill.png
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/folder.png
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/form.png
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/help.png
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/log.png
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/mail_pic.png
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/model.png
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/next.png
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/no_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/open_book.png
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/page.png
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/paste.png
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/pi.png
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/pifile.png
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/plot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/plot1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/previous.png
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/save_pic.png
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/script.png
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/script_ext.png
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/setting.png
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/solver.png
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/sun.png
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/surf.png
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/text.png
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/threed_rot.png
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/trash.png
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/32x32/world_link.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28583 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/app_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/app_logo_middle.png
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/app_logo_small.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.418841 piScope-1.0.8/python/ifigure/resources/icon/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_BarAB.png
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_BracketA.png
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_BracketAB.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_BracketB.png
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Curve.png
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_CurveA.png
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_CurveAB.png
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_CurveB.png
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_CurveFilledA.png
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_CurveFilledAB.png
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_CurveFilledB.png
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Fancy.png
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Q3VydmU=.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Q3VydmVB.png
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Q3VydmVBQg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Q3VydmVC.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Q3VydmVGaWxsZWRB.png
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Q3VydmVGaWxsZWRBQg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Q3VydmVGaWxsZWRC.png
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_QmFyQUI=.png
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_QnJhY2tldEE=.png
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_QnJhY2tldEFC.png
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_QnJhY2tldEI=.png
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_RmFuY3k=.png
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Simple.png
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_U2ltcGxl.png
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_V2VkZ2U=.png
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Wedge.png
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_Y3lhbg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_Yg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_Ymx1ZQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_YmxhY2s=.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_Yw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_Z3JlZW4=.png
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_Z3JleQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_ZGFya2dyZXk=.png
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_Zw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_aw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_b3RoZXI=.png
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_bGlnaHRncmV5.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_bQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_bWFnZW50YQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_black.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_bm9uZQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_cg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_cmVk.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_cyan.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_d2hpdGU=.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_darkgray.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_darkgrey.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_dw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_eQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_eWVsbG93.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_gray.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_green.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_grey.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_lightgrey.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_magenta.png
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_none.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_red.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_white.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/color_yellow.png
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Blues.png
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_BrBG.png
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_BuGn.png
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_BuPu.png
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Dark2.png
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_GnBu.png
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Greens.png
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Greys.png
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_OrRd.png
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Oranges.png
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_PRGn.png
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Paired.png
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Pastel1.png
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Pastel2.png
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_PiYG.png
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_PuBu.png
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_PuBuGn.png
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_PuOr.png
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_PuRd.png
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Purples.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Q01SbWFw.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_QWNjZW50.png
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Qmx1ZXM=.png
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_QnJCRw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_QnVHbg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_QnVQdQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_R25CdQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_R3JlZW5z.png
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_R3JleXM=.png
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_RGFyazI=.png
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_RdBu.png
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_RdGy.png
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_RdPu.png
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_RdYlBu.png
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_RdYlGn.png
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Reds.png
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Set1.png
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Set2.png
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Set3.png
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_T3JSZA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_T3Jhbmdlcw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_U2V0MQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_U2V0Mg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_U2V0Mw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_U3BlY3RyYWw=.png
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UFJHbg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UGFpcmVk.png
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UGFzdGVsMQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UGFzdGVsMg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UGlZRw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UHVCdQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UHVCdUdu.png
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UHVPcg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UHVSZA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UHVycGxlcw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UmRCdQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UmRHeQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UmRQdQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UmRZbEJ1.png
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UmRZbEdu.png
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UmVkcw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_V2lzdGlh.png
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_VmVnYTEw.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_VmVnYTIw.png
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_VmVnYTIwYg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_VmVnYTIwYw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_WWxHbg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_WWxHbkJ1.png
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_WWxPckJy.png
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_WWxPclJk.png
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Y29vbA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Y29vbHdhcm0=.png
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Y29wcGVy.png
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Y2l2aWRpcw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Y3ViZWhlbGl4.png
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_YWZtaG90.png
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_YXV0dW1u.png
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_YlGn.png
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_YlGnBu.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_YlOrBr.png
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_YlOrRd.png
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Ym9uZQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_YmluYXJ5.png
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_YnJn.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Yndy.png
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z251cGxvdA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z251cGxvdDI=.png
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z2lzdF95YXJn.png
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z2lzdF9lYXJ0aA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z2lzdF9ncmF5.png
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z2lzdF9oZWF0.png
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z2lzdF9uY2Fy.png
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z2lzdF9yYWluYm93.png
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z2lzdF9zdGVybg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z3JheQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_ZmxhZw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aG90.png
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aHN2.png
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aW5mZXJubw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTA=.png
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTE=.png
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTI=.png
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTM=.png
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTQ=.png
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTU=.png
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTY=.png
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTc=.png
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTg=.png
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTk=.png
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjA=.png
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjE=.png
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjI=.png
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjM=.png
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjQ=.png
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjU=.png
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjY=.png
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjc=.png
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjg=.png
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjk=.png
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzA=.png
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzE=.png
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzI=.png
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzM=.png
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzQ=.png
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzU=.png
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzY=.png
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzc=.png
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzg=.png
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzk=.png
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsNA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsNQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsNg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsNw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsOA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsOQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_afmhot.png
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_amV0.png
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_autumn.png
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_b2NlYW4=.png
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_bWFnbWE=.png
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_binary.png
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_bmlweV9zcGVjdHJhbA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_bone.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_brg.png
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_bwr.png
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_c2Vpc21pYw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_c3BlY3RyYWw=.png
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_c3ByaW5n.png
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_c3VtbWVy.png
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_cGluaw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_cGxhc21h.png
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_cHJpc20=.png
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_cmFpbmJvdw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_cool.png
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_coolwarm.png
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_copper.png
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_cubehelix.png
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_d2ludGVy.png
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dGFiMTA=.png
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dGFiMjA=.png
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dGFiMjBi.png
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dGFiMjBj.png
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dGVycmFpbg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dHdpbGlnaHQ=.png
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dHdpbGlnaHRfc2hpZnRlZA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dmlyaWRpcw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_flag.png
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_gist_earth.png
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_gist_gray.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_gist_heat.png
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_gist_ncar.png
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_gist_rainbow.png
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_gist_stern.png
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_gist_yarg.png
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_gnuplot.png
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_gnuplot2.png
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_gray.png
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_hot.png
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_hsv.png
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_jet.png
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_ocean.png
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_pink.png
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_prism.png
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_rainbow.png
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_seismic.png
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_spectral.png
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_spring.png
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_summer.png
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_terrain.png
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/colormap_winter.png
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linestyle_LQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linestyle_LS0=.png
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linestyle_LS4=.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linestyle_Tm9uZQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linestyle_Y29sb24=.png
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_1.5.png
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_2.5.png
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_MA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_MC4w.png
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_MQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_MS41.png
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_MS4w.png
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_Mg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_Mi41.png
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_Mi4w.png
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_Mw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/linewidth_My4w.png
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_Kg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_MQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_Mg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_Mw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_NA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_RA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_SA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_Tm9uZQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_ZA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_aA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_aGxpbmU=.png
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_bw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_cA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_cGl4ZWw=.png
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_cGludA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_cGx1cw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_cw==.png
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_dHJpYW5nbGVfZG93bg==.png
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_dHJpYW5nbGVfbGVmdA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_dHJpYW5nbGVfcmlnaHQ=.png
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_dHJpYW5nbGVfdXA=.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_dmxpbmU=.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/marker_eA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_LQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_LS0=.png
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_LS4=.png
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_Og==.png
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_Tm9uZQ==.png
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_ZG90dGVk.png
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_ZGFzaGRvdA==.png
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_ZGFzaGVk.png
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_c29saWQ=.png
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_dashdot.png
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_dashed.png
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_dotted.png
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/plinestyle_solid.png
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/image/slider.png
--rw-r--r--   0 runner    (1001) docker     (123)    47842 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/icon/launcher_app_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   133120 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/idl_colors.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.418841 piScope-1.0.8/python/ifigure/resources/mdsplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/mdsplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/mdsplus/connection_setting
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/mdsplus/default_mdsserver
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/mdsplus/mdsserver_config
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/mdsplus/scope_setting
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.418841 piScope-1.0.8/python/ifigure/resources/pref/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/advanced_config
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/appearance_config
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/cursor_config
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/file_helper
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/general_config
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/helperapp_config
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/helperapp_mac_config
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/hg_config
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/hg_default_config
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/postoffice_config
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/resources/pref/visual_config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.418841 piScope-1.0.8/python/ifigure/rpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/rpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/rpo/client_efit.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/rpo/client_nepolar.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/rpo/client_nete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/rpo/proxy_efit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/rpo/proxy_nepolar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/rpo/proxy_nete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/rpo/pyro_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/rpo/unused_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.422840 piScope-1.0.8/python/ifigure/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/new_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/new_module_nochild.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/new_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.422840 piScope-1.0.8/python/ifigure/template/script/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/script/_blank_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/script/bookgui_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/script/function_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/script/mdsscope_extramenu.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/script/plot_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/template/script/sample_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.422840 piScope-1.0.8/python/ifigure/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/test/gldemo.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/test/run_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.430841 piScope-1.0.8/python/ifigure/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/add_sys_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/arraykey_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/buildxobj.py
--rw-r--r--   0 runner    (1001) docker     (123)    32990 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/cbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/checkbox_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)   177164 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/edit_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/eval_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/event_driven_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/event_driven_thread2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/game.py
--rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/get_ifigure_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/get_memory_usage_win.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/get_username.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/gif_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/hdf_data_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/helper_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/image_transition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/images2gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/key_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/mailfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/make_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/marker_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/mdsplus_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/minifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/model_setup_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/mp_tarzip.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/ndarray_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/pickle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/pickled_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/pid_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/pix_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/png_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/postoffice.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/print_openfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/read_afile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/recarray.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/rollback_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/safename.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/sample_child.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/sample_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/setting_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/show_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/sync_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/triangulation_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/vctr_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/weak_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/utils/wx3to4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.442841 piScope-1.0.8/python/ifigure/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/advanced_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/appearance_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    59339 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/artist_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/at_wxthread.py
--rw-r--r--   0 runner    (1001) docker     (123)    21305 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/axes_range_subs.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/base_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    77433 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/book_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/book_viewer_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/button_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.442841 piScope-1.0.8/python/ifigure/widgets/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/canvas/custom_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/canvas/dnd_areasplitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/canvas/file_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)   180834 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/canvas/ifigure_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    49315 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/canvas/layout_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/command_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/consol.py
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/custom_double_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/cutplane_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/debugger_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/dlg_axspine_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/dlg_fileimportmode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/dlg_message_scroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/dlg_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/file_helper_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/find_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/growable_text_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/hdf_export_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/hgdiff_window.py
--rw-r--r--   0 runner    (1001) docker     (123)   508985 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/logwindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/margin_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/miniframe_with_windowlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    36061 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/navibar2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14346 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/panel_checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/passwd_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/primitive_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    53316 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/proj_tree_viewer_aui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20390 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/proj_tree_viewer_aui2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/property_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/radio_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/redirect_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    70550 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/script_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/section_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/shellvar_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/simple_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/slice_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/syntax_styles.py
--rw-r--r--   0 runner    (1001) docker     (123)    49564 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/taskbar.py
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/text_ctrl_copypaste.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/textctrl_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/tipwindow.py
--rw-r--r--   0 runner    (1001) docker     (123)    28166 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/undo_redo_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    30190 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/var_viewerg2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/video_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/videoplayer_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-04-07 18:25:47.000000 piScope-1.0.8/python/ifigure/widgets/wave_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:25:59.442841 piScope-1.0.8/python/piScope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-07 18:25:59.000000 piScope-1.0.8/python/piScope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40758 2023-04-07 18:25:59.000000 piScope-1.0.8/python/piScope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:25:59.000000 piScope-1.0.8/python/piScope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-07 18:25:59.000000 piScope-1.0.8/python/piScope.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-07 18:25:59.000000 piScope-1.0.8/python/piScope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 18:25:59.000000 piScope-1.0.8/python/piScope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 18:25:59.442841 piScope-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-07 18:25:47.000000 piScope-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.433597 piScope-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-09 14:10:46.000000 piScope-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-09 14:10:58.433597 piScope-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-09 14:10:46.000000 piScope-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.297598 piScope-1.0.9/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.297598 piScope-1.0.9/python/ifigure/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.297598 piScope-1.0.9/python/ifigure/add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.297598 piScope-1.0.9/python/ifigure/add_on/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.301598 piScope-1.0.9/python/ifigure/add_on/model/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/efit_afile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25060 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/efit_gfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/efit_pfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/idl_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/matlab_mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/mdsplus_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/name_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/netcdf4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.301598 piScope-1.0.9/python/ifigure/add_on/model/module/subs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/subs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/subs/dwscope_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/subs/dwscope_subs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/subs/idl_save_subs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/subs/mdsplus_tree_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/subs/netcdf_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/module/tsc_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.301598 piScope-1.0.9/python/ifigure/add_on/model/script/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/model/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.301598 piScope-1.0.9/python/ifigure/add_on/setting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/setting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.301598 piScope-1.0.9/python/ifigure/add_on/setting/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/setting/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/setting/module/cmod_pyro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/setting/module/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/setting/module/mdsplus_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/setting/module/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.305598 piScope-1.0.9/python/ifigure/add_on/setting/script/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/setting/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.305598 piScope-1.0.9/python/ifigure/add_on/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.305598 piScope-1.0.9/python/ifigure/add_on/solver/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.305598 piScope-1.0.9/python/ifigure/add_on/solver/script/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/script/cost_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/script/def_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/script/genray_loki.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/script/merge_sol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/script/merge_sol_parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/script/merge_sol_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/script/run_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/script/run_parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/add_on/solver/script/run_stdsolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.305598 piScope-1.0.9/python/ifigure/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/example/cmod_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/example/gl_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/example/plot_demos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.305598 piScope-1.0.9/python/ifigure/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/extra/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79953 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/ifigure_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/ifigure_app_macport_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/ifigure_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43923 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.313598 piScope-1.0.9/python/ifigure/matplotlib_mod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40807 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/art3d_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58925 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/axes3d_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/axes_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/backend_wx_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/backend_wxagg_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/backend_wxagg_gl_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91905 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/backend_wxagg_gl_15.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18636 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/backend_wxagg_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/canvas_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/cz_linecollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/depthmap_12.frag
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/depthmap_12.vert
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/depthmap_15.frag
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/depthmap_15.vert
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/figure_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84975 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/glcanvas_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98007 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/glcanvas_15.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/is_supported_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/lines_15.frag
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/lines_15.geom
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/lines_15.vert
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/mpl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/renderer_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/simple.frag
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/simple_12.vert
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/simple_15.geom
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/simple_15.vert
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/simple_oit.frag
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/simple_oit_12.frag
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/simple_oit_15.frag
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/simple_oit_final.frag
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/triangles_15.geom
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/matplotlib_mod/triplot_mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.317598 piScope-1.0.9/python/ifigure/mdsplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/direct_jobrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/direct_jobrunner_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24134 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/dlg_mdssession.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/dlg_mdssession_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/dlg_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/dlg_setting2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/event_listener_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/event_listener_proc_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/event_listener_proc_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/fake_jobrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49430 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/fig_mds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/fig_mdsbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/fig_mdsdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/filebacked_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/filed_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/import_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mds_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mds_mpth_directworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mds_mpth_proxyworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mds_mpth_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mds_sp_directworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mds_sp_echobackworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mds_sp_proxyworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mds_sp_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mdsplus_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mdsplus_gateway_th.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mdsplusr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106154 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mdsscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mdsscope_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mdsscope_nw.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mp_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/mp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/proxy_jobrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/proxyworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/shot_number_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mdsplus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.325598 piScope-1.0.9/python/ifigure/mto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/abs_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25917 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/axis_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/axis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92651 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_axline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_axlinec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_axspan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_axspanc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33310 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33524 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_eps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19833 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_grp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34413 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21519 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58299 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24743 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40355 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_plotc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28205 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_solid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26081 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_tricontour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_tripcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_triplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fig_trisurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/figobj_gpholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/figobj_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/fileholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/generic_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/gl_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47705 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/hg_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22311 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/project_top.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/py_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42110 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/py_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/py_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23838 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/py_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/py_extfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/py_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/py_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/py_moduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36206 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/py_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/py_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/threaded_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75704 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/treedict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/treedict_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/treelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/mto/triangle_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/numerical_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/piscope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.325598 piScope-1.0.9/python/ifigure/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.325598 piScope-1.0.9/python/ifigure/resources/icon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.337597 piScope-1.0.9/python/ifigure/resources/icon/16x16/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/a.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/amode.png
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrow_firstpage.png
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrow_fwdplay.png
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrow_fwdstep.png
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrow_lastpage.png
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrow_revplay.png
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrow_revstep.png
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrowleft.png
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrowmove.png
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrowmove_all.png
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/arrowright.png
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/axes.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/book.png
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/box.png
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/close.png
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/cog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/colorbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/ctrl.png
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/cursor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/curve.png
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/data.png
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/eps.png
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/expand.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/external_overlay.png
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/fill.png
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/flip_cp_side.png
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/folder_ext.png
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/folder_hg.png
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/form.png
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/grid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/group.png
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/hg.png
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/image.png
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/legend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/log.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/mail_pic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/margin.png
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/mdsplus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/minus_phi.png
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/minus_theta.png
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/model.png
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/model_hg.png
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/no_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/open_book.png
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/page.png
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/paste.png
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/pi.png
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/pifile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/plot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/plotc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/plus_phi.png
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/plus_theta.png
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/pmode.png
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/previous.png
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/reset.png
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/resetrange_all.png
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/samex.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/samey.png
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/save_pic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/script.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/script_ext.png
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/script_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/select.png
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/setting.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/shift_cp.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/shift_phi.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/shift_theta.png
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/smode.png
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/solver.png
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/stop_play.png
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/sun.png
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/suppress.png
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/surf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/t.png
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/text.png
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/three_d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/threed_rot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/timetrace.png
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/trash.png
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/variable.png
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/world_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/xauto.png
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/xlog.png
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/xy_plane.png
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/xz_plane.png
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/yauto.png
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/ylog.png
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/yz_plane.png
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom2menu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom2minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom2minusmenu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom3minus.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.341597 piScope-1.0.9/python/ifigure/resources/icon/24x24/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/a.png
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/axes.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/book.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/cog.png
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/cursor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/expand.png
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/fill.png
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/form.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/log.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/mail_pic.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/model.png
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/no_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/open_book.png
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/page.png
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/paste.png
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/pifile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/plot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/previous.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/save_pic.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/setting.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/sun.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/surf.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/text.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/threed_rot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/trash.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/24x24/world_link.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.345598 piScope-1.0.9/python/ifigure/resources/icon/32x32/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/a.png
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/axes.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/book.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/cog.png
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/cursor.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/data.png
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/expand.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/external_overlay.png
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/fill.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/form.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/log.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/mail_pic.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/no_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/open_book.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/page.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/paste.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/pi.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/pifile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/plot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/previous.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/save_pic.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/script.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/script_ext.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/setting.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/solver.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/sun.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/surf.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/text.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/threed_rot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/trash.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/32x32/world_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28583 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/app_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/app_logo_middle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/app_logo_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.393597 piScope-1.0.9/python/ifigure/resources/icon/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_BarAB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_BracketA.png
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_BracketAB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_BracketB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Curve.png
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_CurveA.png
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_CurveAB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_CurveB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_CurveFilledA.png
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_CurveFilledAB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_CurveFilledB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Fancy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Q3VydmU=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Q3VydmVB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Q3VydmVBQg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Q3VydmVC.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Q3VydmVGaWxsZWRB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Q3VydmVGaWxsZWRBQg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Q3VydmVGaWxsZWRC.png
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_QmFyQUI=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_QnJhY2tldEE=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_QnJhY2tldEFC.png
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_QnJhY2tldEI=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_RmFuY3k=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Simple.png
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_U2ltcGxl.png
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_V2VkZ2U=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Wedge.png
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_Y3lhbg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_Yg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_Ymx1ZQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_YmxhY2s=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_Yw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_Z3JlZW4=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_Z3JleQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_ZGFya2dyZXk=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_Zw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_aw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_b3RoZXI=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_bGlnaHRncmV5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_bQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_bWFnZW50YQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_bm9uZQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_cg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_cmVk.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_cyan.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_d2hpdGU=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_darkgray.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_darkgrey.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_dw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_eQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_eWVsbG93.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_gray.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_green.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_grey.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_lightgrey.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_magenta.png
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_none.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_red.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/color_yellow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Blues.png
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_BrBG.png
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_BuGn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_BuPu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Dark2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_GnBu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Greens.png
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Greys.png
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_OrRd.png
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Oranges.png
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_PRGn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Paired.png
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Pastel1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Pastel2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_PiYG.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_PuBu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_PuBuGn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_PuOr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_PuRd.png
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Purples.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Q01SbWFw.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_QWNjZW50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Qmx1ZXM=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_QnJCRw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_QnVHbg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_QnVQdQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_R25CdQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_R3JlZW5z.png
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_R3JleXM=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_RGFyazI=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_RdBu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_RdGy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_RdPu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_RdYlBu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_RdYlGn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Reds.png
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Set1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Set2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Set3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_T3JSZA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_T3Jhbmdlcw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_U2V0MQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_U2V0Mg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_U2V0Mw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_U3BlY3RyYWw=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UFJHbg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UGFpcmVk.png
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UGFzdGVsMQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UGFzdGVsMg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UGlZRw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UHVCdQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UHVCdUdu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UHVPcg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UHVSZA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UHVycGxlcw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UmRCdQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UmRHeQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UmRQdQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UmRZbEJ1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UmRZbEdu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UmVkcw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_V2lzdGlh.png
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_VmVnYTEw.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_VmVnYTIw.png
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_VmVnYTIwYg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_VmVnYTIwYw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_WWxHbg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_WWxHbkJ1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_WWxPckJy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_WWxPclJk.png
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Y29vbA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Y29vbHdhcm0=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Y29wcGVy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Y2l2aWRpcw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Y3ViZWhlbGl4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_YWZtaG90.png
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_YXV0dW1u.png
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_YlGn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_YlGnBu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_YlOrBr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_YlOrRd.png
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Ym9uZQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_YmluYXJ5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_YnJn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Yndy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z251cGxvdA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z251cGxvdDI=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z2lzdF95YXJn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z2lzdF9lYXJ0aA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z2lzdF9ncmF5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z2lzdF9oZWF0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z2lzdF9uY2Fy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z2lzdF9yYWluYm93.png
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z2lzdF9zdGVybg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z3JheQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_ZmxhZw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aG90.png
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aHN2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aW5mZXJubw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTA=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTE=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTI=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTM=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTQ=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTU=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTY=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTc=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTg=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTk=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjA=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjE=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjI=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjM=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjQ=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjU=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjY=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjc=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjg=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjk=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzA=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzE=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzI=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzM=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzQ=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzU=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzY=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzc=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzg=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzk=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsNA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsNQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsNg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsNw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsOA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsOQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_afmhot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_amV0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_autumn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_b2NlYW4=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_bWFnbWE=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_binary.png
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_bmlweV9zcGVjdHJhbA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_bone.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_brg.png
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_bwr.png
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_c2Vpc21pYw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_c3BlY3RyYWw=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_c3ByaW5n.png
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_c3VtbWVy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_cGluaw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_cGxhc21h.png
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_cHJpc20=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_cmFpbmJvdw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_cool.png
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_coolwarm.png
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_copper.png
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_cubehelix.png
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_d2ludGVy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dGFiMTA=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dGFiMjA=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dGFiMjBi.png
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dGFiMjBj.png
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dGVycmFpbg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dHdpbGlnaHQ=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dHdpbGlnaHRfc2hpZnRlZA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dmlyaWRpcw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_flag.png
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_gist_earth.png
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_gist_gray.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_gist_heat.png
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_gist_ncar.png
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_gist_rainbow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_gist_stern.png
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_gist_yarg.png
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_gnuplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_gnuplot2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_gray.png
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_hot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_hsv.png
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_jet.png
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_ocean.png
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_pink.png
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_prism.png
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_rainbow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_seismic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_spectral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_spring.png
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_summer.png
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_terrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/colormap_winter.png
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linestyle_LQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linestyle_LS0=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linestyle_LS4=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linestyle_Tm9uZQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linestyle_Y29sb24=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_1.5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_2.5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_MA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_MC4w.png
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_MQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_MS41.png
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_MS4w.png
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_Mg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_Mi41.png
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_Mi4w.png
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_Mw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/linewidth_My4w.png
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_Kg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_MQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_Mg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_Mw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_NA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_RA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_SA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_Tm9uZQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_ZA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_aA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_aGxpbmU=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_bw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_cA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_cGl4ZWw=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_cGludA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_cGx1cw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_cw==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_dHJpYW5nbGVfZG93bg==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_dHJpYW5nbGVfbGVmdA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_dHJpYW5nbGVfcmlnaHQ=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_dHJpYW5nbGVfdXA=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_dmxpbmU=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/marker_eA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_LQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_LS0=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_LS4=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_Og==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_Tm9uZQ==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_ZG90dGVk.png
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_ZGFzaGRvdA==.png
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_ZGFzaGVk.png
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_c29saWQ=.png
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_dashdot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_dashed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_dotted.png
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/plinestyle_solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/image/slider.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47842 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/icon/launcher_app_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   133120 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/idl_colors.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.397597 piScope-1.0.9/python/ifigure/resources/mdsplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/mdsplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/mdsplus/connection_setting
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/mdsplus/default_mdsserver
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/mdsplus/mdsserver_config
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/mdsplus/scope_setting
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.397597 piScope-1.0.9/python/ifigure/resources/pref/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/advanced_config
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/appearance_config
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/cursor_config
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/file_helper
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/general_config
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/helperapp_config
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/helperapp_mac_config
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/hg_config
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/hg_default_config
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/postoffice_config
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/resources/pref/visual_config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.401597 piScope-1.0.9/python/ifigure/rpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/rpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/rpo/client_efit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/rpo/client_nepolar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/rpo/client_nete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/rpo/proxy_efit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/rpo/proxy_nepolar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/rpo/proxy_nete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/rpo/pyro_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/rpo/unused_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.401597 piScope-1.0.9/python/ifigure/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/new_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/new_module_nochild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/new_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.401597 piScope-1.0.9/python/ifigure/template/script/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/script/_blank_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/script/bookgui_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/script/function_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/script/mdsscope_extramenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/script/plot_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/template/script/sample_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.405597 piScope-1.0.9/python/ifigure/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/test/gldemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/test/run_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.417597 piScope-1.0.9/python/ifigure/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/add_sys_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/arraykey_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/buildxobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32990 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/cbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/checkbox_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)   177164 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/edit_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/eval_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/event_driven_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/event_driven_thread2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/get_ifigure_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/get_memory_usage_win.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/get_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/gif_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/hdf_data_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/helper_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/image_transition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/images2gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/key_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/mailfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/make_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/marker_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/mdsplus_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/minifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/model_setup_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/mp_tarzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/ndarray_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/pickle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/pickled_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/pid_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/pix_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/png_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/postoffice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/print_openfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/read_afile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/recarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/rollback_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/safename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/sample_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/sample_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/setting_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/show_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/sync_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/triangulation_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/vctr_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/weak_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/utils/wx3to4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.429597 piScope-1.0.9/python/ifigure/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/advanced_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/appearance_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59339 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/artist_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/at_wxthread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21305 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/axes_range_subs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/base_widget.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77433 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/book_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/book_viewer_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/button_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.429597 piScope-1.0.9/python/ifigure/widgets/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/canvas/custom_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/canvas/dnd_areasplitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/canvas/file_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180834 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/canvas/ifigure_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49315 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/canvas/layout_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/command_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/consol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/custom_double_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/cutplane_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/debugger_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/dlg_axspine_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/dlg_fileimportmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/dlg_message_scroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/dlg_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/file_helper_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/find_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/growable_text_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/hdf_export_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/hgdiff_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)   508985 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/logwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/margin_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/miniframe_with_windowlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36061 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/navibar2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14346 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/panel_checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/passwd_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/primitive_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53316 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/proj_tree_viewer_aui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20390 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/proj_tree_viewer_aui2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/property_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/radio_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/redirect_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70550 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/script_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/section_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/shellvar_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/simple_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/slice_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/syntax_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49564 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/taskbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/text_ctrl_copypaste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/textctrl_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/tipwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28166 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/undo_redo_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30190 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/var_viewerg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/video_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/videoplayer_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-04-09 14:10:46.000000 piScope-1.0.9/python/ifigure/widgets/wave_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:10:58.433597 piScope-1.0.9/python/piScope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-09 14:10:58.000000 piScope-1.0.9/python/piScope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40758 2023-04-09 14:10:58.000000 piScope-1.0.9/python/piScope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:10:58.000000 piScope-1.0.9/python/piScope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-09 14:10:58.000000 piScope-1.0.9/python/piScope.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-09 14:10:58.000000 piScope-1.0.9/python/piScope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 14:10:58.000000 piScope-1.0.9/python/piScope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:10:58.433597 piScope-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-09 14:10:46.000000 piScope-1.0.9/setup.py
```

### Comparing `piScope-1.0.8/LICENSE` & `piScope-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/PKG-INFO` & `piScope-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piScope
-Version: 1.0.8
+Version: 1.0.9
 Summary: piScope data analysis workbench
 Download-URL: https://github.com/piScope/piScope
 Author: S. Shiraiwa
 Author-email: shiraiwa@princeton.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `piScope-1.0.8/README.md` & `piScope-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/csv.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/csv.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/efit_afile.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/efit_afile.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/efit_gfile.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/efit_gfile.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/efit_pfile.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/efit_pfile.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/idl_save.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/idl_save.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/matlab_mat.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/matlab_mat.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/mdsplus_tree.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/mdsplus_tree.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/name_list.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/name_list.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/netcdf4.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/netcdf4.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/subs/dwscope_sub.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/subs/dwscope_sub.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/subs/dwscope_subs.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/subs/dwscope_subs.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/subs/idl_save_subs.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/subs/idl_save_subs.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/subs/mdsplus_tree_node.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/subs/mdsplus_tree_node.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/subs/netcdf_node.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/subs/netcdf_node.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/model/module/tsc_input.py` & `piScope-1.0.9/python/ifigure/add_on/model/module/tsc_input.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/setting/module/cmod_pyro.py` & `piScope-1.0.9/python/ifigure/add_on/setting/module/cmod_pyro.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/setting/module/connection.py` & `piScope-1.0.9/python/ifigure/add_on/setting/module/connection.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/setting/module/mdsplus_worker.py` & `piScope-1.0.9/python/ifigure/add_on/setting/module/mdsplus_worker.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/setting/module/ssh.py` & `piScope-1.0.9/python/ifigure/add_on/setting/module/ssh.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/solver/script/genray_loki.py` & `piScope-1.0.9/python/ifigure/add_on/solver/script/genray_loki.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/solver/script/merge_sol.py` & `piScope-1.0.9/python/ifigure/add_on/solver/script/merge_sol.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/solver/script/merge_sol_parametric.py` & `piScope-1.0.9/python/ifigure/add_on/solver/script/merge_sol_parametric.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/solver/script/merge_sol_std.py` & `piScope-1.0.9/python/ifigure/add_on/solver/script/merge_sol_std.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/solver/script/run_optimizer.py` & `piScope-1.0.9/python/ifigure/add_on/solver/script/run_optimizer.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/solver/script/run_parametric.py` & `piScope-1.0.9/python/ifigure/add_on/solver/script/run_parametric.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/add_on/solver/script/run_stdsolver.py` & `piScope-1.0.9/python/ifigure/add_on/solver/script/run_stdsolver.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/client.py` & `piScope-1.0.9/python/ifigure/client.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/events.py` & `piScope-1.0.9/python/ifigure/events.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/example/cmod_tiles.py` & `piScope-1.0.9/python/ifigure/example/cmod_tiles.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/example/gl_demos.py` & `piScope-1.0.9/python/ifigure/example/gl_demos.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/example/plot_demos.py` & `piScope-1.0.9/python/ifigure/example/plot_demos.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/extra/connections.py` & `piScope-1.0.9/python/ifigure/extra/connections.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/ifigure_app.py` & `piScope-1.0.9/python/ifigure/ifigure_app.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/ifigure_config.py` & `piScope-1.0.9/python/ifigure/ifigure_config.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/interactive.py` & `piScope-1.0.9/python/ifigure/interactive.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/art3d_gl.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/art3d_gl.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/axes3d_mod.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/axes3d_mod.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/axes_mod.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/axes_mod.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/backend_wx_mod.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/backend_wx_mod.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/backend_wxagg_gl.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/backend_wxagg_gl.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/backend_wxagg_gl_12.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/backend_wxagg_gl_12.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/backend_wxagg_gl_15.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/backend_wxagg_gl_15.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/backend_wxagg_mod.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/backend_wxagg_mod.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/canvas_common.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/canvas_common.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/cz_linecollection.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/cz_linecollection.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/depthmap_12.frag` & `piScope-1.0.9/python/ifigure/matplotlib_mod/depthmap_12.frag`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/depthmap_12.vert` & `piScope-1.0.9/python/ifigure/matplotlib_mod/depthmap_12.vert`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/depthmap_15.frag` & `piScope-1.0.9/python/ifigure/matplotlib_mod/depthmap_15.frag`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/depthmap_15.vert` & `piScope-1.0.9/python/ifigure/matplotlib_mod/depthmap_15.vert`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/figure_mod.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/figure_mod.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/glcanvas_12.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/glcanvas_12.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/glcanvas_15.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/glcanvas_15.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/is_supported_renderer.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/is_supported_renderer.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/lines_15.frag` & `piScope-1.0.9/python/ifigure/matplotlib_mod/lines_15.frag`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/lines_15.geom` & `piScope-1.0.9/python/ifigure/matplotlib_mod/lines_15.geom`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/lines_15.vert` & `piScope-1.0.9/python/ifigure/matplotlib_mod/lines_15.vert`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/mpl_utils.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/mpl_utils.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/renderer_gl.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/renderer_gl.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/simple.frag` & `piScope-1.0.9/python/ifigure/matplotlib_mod/simple.frag`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/simple_12.vert` & `piScope-1.0.9/python/ifigure/matplotlib_mod/simple_12.vert`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/simple_15.geom` & `piScope-1.0.9/python/ifigure/matplotlib_mod/simple_15.geom`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/simple_15.vert` & `piScope-1.0.9/python/ifigure/matplotlib_mod/simple_15.vert`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/simple_oit.frag` & `piScope-1.0.9/python/ifigure/matplotlib_mod/simple_oit.frag`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/simple_oit_12.frag` & `piScope-1.0.9/python/ifigure/matplotlib_mod/simple_oit_12.frag`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/simple_oit_15.frag` & `piScope-1.0.9/python/ifigure/matplotlib_mod/simple_oit_15.frag`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/simple_oit_final.frag` & `piScope-1.0.9/python/ifigure/matplotlib_mod/simple_oit_final.frag`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/triangles_15.geom` & `piScope-1.0.9/python/ifigure/matplotlib_mod/triangles_15.geom`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/matplotlib_mod/triplot_mod.py` & `piScope-1.0.9/python/ifigure/matplotlib_mod/triplot_mod.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/direct_jobrunner.py` & `piScope-1.0.9/python/ifigure/mdsplus/direct_jobrunner.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/direct_jobrunner_ts.py` & `piScope-1.0.9/python/ifigure/mdsplus/direct_jobrunner_ts.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/dlg_mdssession.py` & `piScope-1.0.9/python/ifigure/mdsplus/dlg_mdssession.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/dlg_mdssession_data.py` & `piScope-1.0.9/python/ifigure/mdsplus/dlg_mdssession_data.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/dlg_setting.py` & `piScope-1.0.9/python/ifigure/mdsplus/dlg_setting.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/dlg_setting2.py` & `piScope-1.0.9/python/ifigure/mdsplus/dlg_setting2.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/event_listener.py` & `piScope-1.0.9/python/ifigure/mdsplus/event_listener.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/event_listener_proc.py` & `piScope-1.0.9/python/ifigure/mdsplus/event_listener_proc.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/event_listener_proc_debug.py` & `piScope-1.0.9/python/ifigure/mdsplus/event_listener_proc_debug.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/event_listener_proc_fake.py` & `piScope-1.0.9/python/ifigure/mdsplus/event_listener_proc_fake.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/fake_jobrunner.py` & `piScope-1.0.9/python/ifigure/mdsplus/fake_jobrunner.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/fig_mds.py` & `piScope-1.0.9/python/ifigure/mdsplus/fig_mds.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/fig_mdsbook.py` & `piScope-1.0.9/python/ifigure/mdsplus/fig_mdsbook.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/fig_mdsdata.py` & `piScope-1.0.9/python/ifigure/mdsplus/fig_mdsdata.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/filed_ndarray.py` & `piScope-1.0.9/python/ifigure/mdsplus/filed_ndarray.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/import_dw.py` & `piScope-1.0.9/python/ifigure/mdsplus/import_dw.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mds_mpth_directworker.py` & `piScope-1.0.9/python/ifigure/mdsplus/mds_mpth_directworker.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mds_mpth_proxyworker.py` & `piScope-1.0.9/python/ifigure/mdsplus/mds_mpth_proxyworker.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mds_mpth_worker_pool.py` & `piScope-1.0.9/python/ifigure/mdsplus/mds_mpth_worker_pool.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mds_sp_directworker.py` & `piScope-1.0.9/python/ifigure/mdsplus/mds_sp_directworker.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mds_sp_proxyworker.py` & `piScope-1.0.9/python/ifigure/mdsplus/mds_sp_proxyworker.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mds_sp_worker_pool.py` & `piScope-1.0.9/python/ifigure/mdsplus/mds_sp_worker_pool.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mdsplus_gateway.py` & `piScope-1.0.9/python/ifigure/mdsplus/mdsplus_gateway.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mdsplus_gateway_th.py` & `piScope-1.0.9/python/ifigure/mdsplus/mdsplus_gateway_th.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mdsscope.py` & `piScope-1.0.9/python/ifigure/mdsplus/mdsscope.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mdsscope_canvas.py` & `piScope-1.0.9/python/ifigure/mdsplus/mdsscope_canvas.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mdsscope_nw.py` & `piScope-1.0.9/python/ifigure/mdsplus/mdsscope_nw.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/mp_test.py` & `piScope-1.0.9/python/ifigure/mdsplus/mp_test.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/proxy_jobrunner.py` & `piScope-1.0.9/python/ifigure/mdsplus/proxy_jobrunner.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mdsplus/shot_number_ctrl.py` & `piScope-1.0.9/python/ifigure/mdsplus/shot_number_ctrl.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/abs_module.py` & `piScope-1.0.9/python/ifigure/mto/abs_module.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/axis_param.py` & `piScope-1.0.9/python/ifigure/mto/axis_param.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/axis_user.py` & `piScope-1.0.9/python/ifigure/mto/axis_user.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_annotate.py` & `piScope-1.0.9/python/ifigure/mto/fig_annotate.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_arrow.py` & `piScope-1.0.9/python/ifigure/mto/fig_arrow.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_axes.py` & `piScope-1.0.9/python/ifigure/mto/fig_axes.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_axline.py` & `piScope-1.0.9/python/ifigure/mto/fig_axline.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_axlinec.py` & `piScope-1.0.9/python/ifigure/mto/fig_axlinec.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_axspan.py` & `piScope-1.0.9/python/ifigure/mto/fig_axspan.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_axspanc.py` & `piScope-1.0.9/python/ifigure/mto/fig_axspanc.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_book.py` & `piScope-1.0.9/python/ifigure/mto/fig_book.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_box.py` & `piScope-1.0.9/python/ifigure/mto/fig_box.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_circle.py` & `piScope-1.0.9/python/ifigure/mto/fig_circle.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_contour.py` & `piScope-1.0.9/python/ifigure/mto/fig_contour.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_control.py` & `piScope-1.0.9/python/ifigure/mto/fig_control.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_curve.py` & `piScope-1.0.9/python/ifigure/mto/fig_curve.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_eps.py` & `piScope-1.0.9/python/ifigure/mto/fig_eps.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_fill.py` & `piScope-1.0.9/python/ifigure/mto/fig_fill.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_grp.py` & `piScope-1.0.9/python/ifigure/mto/fig_grp.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_hist.py` & `piScope-1.0.9/python/ifigure/mto/fig_hist.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_image.py` & `piScope-1.0.9/python/ifigure/mto/fig_image.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_legend.py` & `piScope-1.0.9/python/ifigure/mto/fig_legend.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
             self.highlight_artist(False, artistlist)
             for a in artistlist:
                 if self.get_figaxes() is None:
                     if a in c.legends:
                         c.legends.remove(a)
                 else:
                     if a in c.artists:
-                        c.artists.remove(a)
+                        a.remove()#c.artists.remove(a)
 
         super(FigLegend, self).del_artist(artistlist)
 
     def highlight_artist(self, val, artist=None):
         if artist is None:
             alist = self._artists
         else:
```

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_obj.py` & `piScope-1.0.9/python/ifigure/mto/fig_obj.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_page.py` & `piScope-1.0.9/python/ifigure/mto/fig_page.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_plot.py` & `piScope-1.0.9/python/ifigure/mto/fig_plot.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_plotc.py` & `piScope-1.0.9/python/ifigure/mto/fig_plotc.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_quiver.py` & `piScope-1.0.9/python/ifigure/mto/fig_quiver.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_scatter.py` & `piScope-1.0.9/python/ifigure/mto/fig_scatter.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_solid.py` & `piScope-1.0.9/python/ifigure/mto/fig_solid.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_spec.py` & `piScope-1.0.9/python/ifigure/mto/fig_spec.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_spline.py` & `piScope-1.0.9/python/ifigure/mto/fig_spline.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_surface.py` & `piScope-1.0.9/python/ifigure/mto/fig_surface.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_text.py` & `piScope-1.0.9/python/ifigure/mto/fig_text.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_tricontour.py` & `piScope-1.0.9/python/ifigure/mto/fig_tricontour.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_tripcolor.py` & `piScope-1.0.9/python/ifigure/mto/fig_tripcolor.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_triplot.py` & `piScope-1.0.9/python/ifigure/mto/fig_triplot.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fig_trisurface.py` & `piScope-1.0.9/python/ifigure/mto/fig_trisurface.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/figobj_gpholder.py` & `piScope-1.0.9/python/ifigure/mto/figobj_gpholder.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/fileholder.py` & `piScope-1.0.9/python/ifigure/mto/fileholder.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/generic_points.py` & `piScope-1.0.9/python/ifigure/mto/generic_points.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/gl_compound.py` & `piScope-1.0.9/python/ifigure/mto/gl_compound.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/hg_support.py` & `piScope-1.0.9/python/ifigure/mto/hg_support.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/metadata.py` & `piScope-1.0.9/python/ifigure/mto/metadata.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/project_top.py` & `piScope-1.0.9/python/ifigure/mto/project_top.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/py_class.py` & `piScope-1.0.9/python/ifigure/mto/py_class.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/py_code.py` & `piScope-1.0.9/python/ifigure/mto/py_code.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/py_connection.py` & `piScope-1.0.9/python/ifigure/mto/py_connection.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/py_contents.py` & `piScope-1.0.9/python/ifigure/mto/py_contents.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/py_extfile.py` & `piScope-1.0.9/python/ifigure/mto/py_extfile.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/py_file.py` & `piScope-1.0.9/python/ifigure/mto/py_file.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/py_module.py` & `piScope-1.0.9/python/ifigure/mto/py_module.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/py_moduled.py` & `piScope-1.0.9/python/ifigure/mto/py_moduled.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/py_script.py` & `piScope-1.0.9/python/ifigure/mto/py_script.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/py_solver.py` & `piScope-1.0.9/python/ifigure/mto/py_solver.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/threaded_worker.py` & `piScope-1.0.9/python/ifigure/mto/threaded_worker.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/treedict.py` & `piScope-1.0.9/python/ifigure/mto/treedict.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/treelink.py` & `piScope-1.0.9/python/ifigure/mto/treelink.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/mto/triangle_plots.py` & `piScope-1.0.9/python/ifigure/mto/triangle_plots.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/piscope.py` & `piScope-1.0.9/python/ifigure/piscope.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/arrowmove.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/arrowmove.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/arrowmove_all.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/arrowmove_all.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/book.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/book.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/cog.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/cog.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/colorbar.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/colorbar.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/data.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/data.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/eps.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/eps.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/external_overlay.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/external_overlay.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/flip_cp_side.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/flip_cp_side.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/folder.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/folder.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/folder_ext.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/folder_ext.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/folder_hg.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/folder_hg.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/form.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/form.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/group.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/group.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/help.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/help.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/image.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/image.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/log.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/log.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/mail_pic.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/mail_pic.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/minus_phi.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/minus_phi.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/minus_theta.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/minus_theta.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/model.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/model.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/model_hg.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/model_hg.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/next.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/next.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/open_book.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/open_book.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/page.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/page.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/pi.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/pi.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/pifile.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/pifile.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/plot.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/plot.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/plot1.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/plot1.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/plotc.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/plotc.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/plus_phi.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/plus_phi.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/plus_theta.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/plus_theta.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/previous.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/previous.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/reset.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/reset.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/save_pic.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/save_pic.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/script.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/script.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/script_ext.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/script_ext.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/script_link.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/script_link.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/setting.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/setting.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/shift_cp.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/shift_cp.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/shift_phi.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/shift_phi.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/shift_theta.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/shift_theta.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/solver.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/solver.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/sun.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/sun.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/surf.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/surf.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/text.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/text.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/threed_rot.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/threed_rot.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/timetrace.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/timetrace.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/trash.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/trash.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/world_link.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/world_link.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/xy_plane.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/xy_plane.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/xz_plane.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/xz_plane.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/yz_plane.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/yz_plane.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom2.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom2.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom2menu.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom2menu.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom2minus.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom2minus.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom2minusmenu.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom2minusmenu.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/16x16/zoom3minus.png` & `piScope-1.0.9/python/ifigure/resources/icon/16x16/zoom3minus.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/a.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/a.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/book.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/book.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/cog.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/cog.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/copy.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/copy.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/cursor.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/cursor.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/fill.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/fill.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/folder.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/folder.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/form.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/form.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/help.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/help.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/image.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/image.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/log.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/log.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/mail_pic.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/mail_pic.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/model.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/model.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/next.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/next.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/open_book.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/open_book.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/page.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/page.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/paste.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/paste.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/pifile.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/pifile.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/plot.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/plot.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/plot1.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/plot1.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/previous.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/previous.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/save_pic.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/save_pic.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/setting.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/setting.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/sun.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/sun.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/surf.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/surf.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/text.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/text.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/threed_rot.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/threed_rot.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/trash.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/trash.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/24x24/world_link.png` & `piScope-1.0.9/python/ifigure/resources/icon/24x24/world_link.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/a.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/a.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/book.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/book.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/cog.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/cog.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/copy.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/copy.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/cursor.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/cursor.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/data.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/data.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/expand.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/expand.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/external_overlay.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/external_overlay.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/fill.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/fill.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/folder.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/folder.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/form.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/form.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/help.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/help.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/image.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/image.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/log.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/log.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/mail_pic.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/mail_pic.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/model.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/model.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/next.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/next.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/open_book.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/open_book.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/page.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/page.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/paste.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/paste.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/pi.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/pi.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/pifile.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/pifile.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/plot.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/plot.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/plot1.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/plot1.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/previous.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/previous.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/save_pic.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/save_pic.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/script.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/script.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/script_ext.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/script_ext.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/setting.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/setting.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/solver.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/solver.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/sun.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/sun.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/surf.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/surf.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/text.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/text.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/threed_rot.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/threed_rot.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/trash.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/trash.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/32x32/world_link.png` & `piScope-1.0.9/python/ifigure/resources/icon/32x32/world_link.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/app_logo.png` & `piScope-1.0.9/python/ifigure/resources/icon/app_logo.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/app_logo_middle.png` & `piScope-1.0.9/python/ifigure/resources/icon/app_logo_middle.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/app_logo_small.png` & `piScope-1.0.9/python/ifigure/resources/icon/app_logo_small.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/arrow_Fancy.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/arrow_Fancy.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/arrow_RmFuY3k=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/arrow_RmFuY3k=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_QnJCRw==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_QnJCRw==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_U3BlY3RyYWw=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_U3BlY3RyYWw=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UFJHbg==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UFJHbg==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UGlZRw==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UGlZRw==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UHVPcg==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UHVPcg==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UmRCdQ==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UmRCdQ==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_UmRZbEJ1.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_UmRZbEJ1.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Y29vbHdhcm0=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Y29vbHdhcm0=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Y3ViZWhlbGl4.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Y3ViZWhlbGl4.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z251cGxvdA==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z251cGxvdA==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z2lzdF9lYXJ0aA==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z2lzdF9lYXJ0aA==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_Z2lzdF9uY2Fy.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_Z2lzdF9uY2Fy.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_ZmxhZw==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_ZmxhZw==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aW5mZXJubw==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aW5mZXJubw==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTc=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTc=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMTk=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMTk=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjA=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjA=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjM=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjM=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjY=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjY=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjc=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjc=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjg=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjg=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMjk=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMjk=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzA=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzA=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzI=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzI=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzU=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzU=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzY=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzY=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_aWRsMzc=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_aWRsMzc=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_bWFnbWE=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_bWFnbWE=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_bmlweV9zcGVjdHJhbA==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_bmlweV9zcGVjdHJhbA==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_cHJpc20=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_cHJpc20=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dHdpbGlnaHQ=.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dHdpbGlnaHQ=.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dHdpbGlnaHRfc2hpZnRlZA==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dHdpbGlnaHRfc2hpZnRlZA==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_dmlyaWRpcw==.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_dmlyaWRpcw==.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_flag.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_flag.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/colormap_prism.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/colormap_prism.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/image/slider.png` & `piScope-1.0.9/python/ifigure/resources/icon/image/slider.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/icon/launcher_app_logo.png` & `piScope-1.0.9/python/ifigure/resources/icon/launcher_app_logo.png`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/idl_colors.txt` & `piScope-1.0.9/python/ifigure/resources/idl_colors.txt`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/mdsplus/scope_setting` & `piScope-1.0.9/python/ifigure/resources/mdsplus/scope_setting`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/resources/pref/file_helper` & `piScope-1.0.9/python/ifigure/resources/pref/file_helper`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/rpo/proxy_efit.py` & `piScope-1.0.9/python/ifigure/rpo/proxy_efit.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/rpo/proxy_nepolar.py` & `piScope-1.0.9/python/ifigure/rpo/proxy_nepolar.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/rpo/proxy_nete.py` & `piScope-1.0.9/python/ifigure/rpo/proxy_nete.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/rpo/pyro_ssh.py` & `piScope-1.0.9/python/ifigure/rpo/pyro_ssh.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/rpo/unused_port.py` & `piScope-1.0.9/python/ifigure/rpo/unused_port.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/server.py` & `piScope-1.0.9/python/ifigure/server.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/startup.py` & `piScope-1.0.9/python/ifigure/startup.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/template/new_module.py` & `piScope-1.0.9/python/ifigure/template/new_module.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/template/new_module_nochild.py` & `piScope-1.0.9/python/ifigure/template/new_module_nochild.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/template/new_script.py` & `piScope-1.0.9/python/ifigure/template/new_script.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/template/script/bookgui_template.py` & `piScope-1.0.9/python/ifigure/template/script/bookgui_template.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/template/script/mdsscope_extramenu.py` & `piScope-1.0.9/python/ifigure/template/script/mdsscope_extramenu.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/template/script/plot_template.py` & `piScope-1.0.9/python/ifigure/template/script/plot_template.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/template/script/sample_script.py` & `piScope-1.0.9/python/ifigure/template/script/sample_script.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/test/gldemo.py` & `piScope-1.0.9/python/ifigure/test/gldemo.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/test/run_test.py` & `piScope-1.0.9/python/ifigure/test/run_test.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/add_sys_path.py` & `piScope-1.0.9/python/ifigure/utils/add_sys_path.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/addon_utils.py` & `piScope-1.0.9/python/ifigure/utils/addon_utils.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/args_parser.py` & `piScope-1.0.9/python/ifigure/utils/args_parser.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/arraykey_dict.py` & `piScope-1.0.9/python/ifigure/utils/arraykey_dict.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/buildxobj.py` & `piScope-1.0.9/python/ifigure/utils/buildxobj.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/cbook.py` & `piScope-1.0.9/python/ifigure/utils/cbook.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/checkbox_panel.py` & `piScope-1.0.9/python/ifigure/utils/checkbox_panel.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/daemon.py` & `piScope-1.0.9/python/ifigure/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/debug.py` & `piScope-1.0.9/python/ifigure/utils/debug.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/edit_list.py` & `piScope-1.0.9/python/ifigure/utils/edit_list.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/event_driven_thread.py` & `piScope-1.0.9/python/ifigure/utils/event_driven_thread.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/event_driven_thread2.py` & `piScope-1.0.9/python/ifigure/utils/event_driven_thread2.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/future.py` & `piScope-1.0.9/python/ifigure/utils/future.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/game.py` & `piScope-1.0.9/python/ifigure/utils/game.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/geom.py` & `piScope-1.0.9/python/ifigure/utils/geom.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/get_memory_usage_win.py` & `piScope-1.0.9/python/ifigure/utils/get_memory_usage_win.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/gif_animation.py` & `piScope-1.0.9/python/ifigure/utils/gif_animation.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/hdf_data_export.py` & `piScope-1.0.9/python/ifigure/utils/hdf_data_export.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/helper_app.py` & `piScope-1.0.9/python/ifigure/utils/helper_app.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/image_transition.py` & `piScope-1.0.9/python/ifigure/utils/image_transition.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/images2gif.py` & `piScope-1.0.9/python/ifigure/utils/images2gif.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/key_binding.py` & `piScope-1.0.9/python/ifigure/utils/key_binding.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/mailfile.py` & `piScope-1.0.9/python/ifigure/utils/mailfile.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/make_release.py` & `piScope-1.0.9/python/ifigure/utils/make_release.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/marker_image.py` & `piScope-1.0.9/python/ifigure/utils/marker_image.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/mdsplus_gateway.py` & `piScope-1.0.9/python/ifigure/utils/mdsplus_gateway.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/minifier.py` & `piScope-1.0.9/python/ifigure/utils/minifier.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/model_setup_tools.py` & `piScope-1.0.9/python/ifigure/utils/model_setup_tools.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/mp_tarzip.py` & `piScope-1.0.9/python/ifigure/utils/mp_tarzip.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/ndarray_cache.py` & `piScope-1.0.9/python/ifigure/utils/ndarray_cache.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/pickle_wrapper.py` & `piScope-1.0.9/python/ifigure/utils/pickle_wrapper.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/pickled_pipe.py` & `piScope-1.0.9/python/ifigure/utils/pickled_pipe.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/pid_exists.py` & `piScope-1.0.9/python/ifigure/utils/pid_exists.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/pix_gen.py` & `piScope-1.0.9/python/ifigure/utils/pix_gen.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/png_animation.py` & `piScope-1.0.9/python/ifigure/utils/png_animation.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/postoffice.py` & `piScope-1.0.9/python/ifigure/utils/postoffice.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/print_openfile.py` & `piScope-1.0.9/python/ifigure/utils/print_openfile.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/read_afile.py` & `piScope-1.0.9/python/ifigure/utils/read_afile.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/recarray.py` & `piScope-1.0.9/python/ifigure/utils/recarray.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/rollback_importer.py` & `piScope-1.0.9/python/ifigure/utils/rollback_importer.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/safename.py` & `piScope-1.0.9/python/ifigure/utils/safename.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/setting_parser.py` & `piScope-1.0.9/python/ifigure/utils/setting_parser.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/show_image.py` & `piScope-1.0.9/python/ifigure/utils/show_image.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/sync_hg.py` & `piScope-1.0.9/python/ifigure/utils/sync_hg.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/triangulation_wrapper.py` & `piScope-1.0.9/python/ifigure/utils/triangulation_wrapper.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/vctr_array.py` & `piScope-1.0.9/python/ifigure/utils/vctr_array.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/weak_callback.py` & `piScope-1.0.9/python/ifigure/utils/weak_callback.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/utils/wx3to4.py` & `piScope-1.0.9/python/ifigure/utils/wx3to4.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/advanced_config.py` & `piScope-1.0.9/python/ifigure/widgets/advanced_config.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/appearance_config.py` & `piScope-1.0.9/python/ifigure/widgets/appearance_config.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/artist_widgets.py` & `piScope-1.0.9/python/ifigure/widgets/artist_widgets.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/at_wxthread.py` & `piScope-1.0.9/python/ifigure/widgets/at_wxthread.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/axes_range_subs.py` & `piScope-1.0.9/python/ifigure/widgets/axes_range_subs.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/book_viewer.py` & `piScope-1.0.9/python/ifigure/widgets/book_viewer.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/book_viewer_interactive.py` & `piScope-1.0.9/python/ifigure/widgets/book_viewer_interactive.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/button_example.py` & `piScope-1.0.9/python/ifigure/widgets/button_example.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/canvas/custom_picker.py` & `piScope-1.0.9/python/ifigure/widgets/canvas/custom_picker.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/canvas/dnd_areasplitter.py` & `piScope-1.0.9/python/ifigure/widgets/canvas/dnd_areasplitter.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/canvas/file_structure.py` & `piScope-1.0.9/python/ifigure/widgets/canvas/file_structure.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/canvas/ifigure_canvas.py` & `piScope-1.0.9/python/ifigure/widgets/canvas/ifigure_canvas.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/canvas/layout_editor.py` & `piScope-1.0.9/python/ifigure/widgets/canvas/layout_editor.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/color.py` & `piScope-1.0.9/python/ifigure/widgets/color.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/command_history.py` & `piScope-1.0.9/python/ifigure/widgets/command_history.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/custom_double_slider.py` & `piScope-1.0.9/python/ifigure/widgets/custom_double_slider.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/cutplane_buttons.py` & `piScope-1.0.9/python/ifigure/widgets/cutplane_buttons.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/debugger.py` & `piScope-1.0.9/python/ifigure/widgets/debugger.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/debugger_core.py` & `piScope-1.0.9/python/ifigure/widgets/debugger_core.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/dialog.py` & `piScope-1.0.9/python/ifigure/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/dlg_axspine_setting.py` & `piScope-1.0.9/python/ifigure/widgets/dlg_axspine_setting.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/dlg_fileimportmode.py` & `piScope-1.0.9/python/ifigure/widgets/dlg_fileimportmode.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/dlg_message_scroll.py` & `piScope-1.0.9/python/ifigure/widgets/dlg_message_scroll.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/dlg_preference.py` & `piScope-1.0.9/python/ifigure/widgets/dlg_preference.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/file_helper_dialog.py` & `piScope-1.0.9/python/ifigure/widgets/file_helper_dialog.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/find_panel.py` & `piScope-1.0.9/python/ifigure/widgets/find_panel.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/growable_text_ctrl.py` & `piScope-1.0.9/python/ifigure/widgets/growable_text_ctrl.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/hdf_export_window.py` & `piScope-1.0.9/python/ifigure/widgets/hdf_export_window.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/hgdiff_window.py` & `piScope-1.0.9/python/ifigure/widgets/hgdiff_window.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/images.py` & `piScope-1.0.9/python/ifigure/widgets/images.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/logwindow.py` & `piScope-1.0.9/python/ifigure/widgets/logwindow.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/margin_widget.py` & `piScope-1.0.9/python/ifigure/widgets/margin_widget.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/miniframe_with_windowlist.py` & `piScope-1.0.9/python/ifigure/widgets/miniframe_with_windowlist.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/navibar2.py` & `piScope-1.0.9/python/ifigure/widgets/navibar2.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/panel_checkbox.py` & `piScope-1.0.9/python/ifigure/widgets/panel_checkbox.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/passwd_dialog.py` & `piScope-1.0.9/python/ifigure/widgets/passwd_dialog.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/primitive_widgets.py` & `piScope-1.0.9/python/ifigure/widgets/primitive_widgets.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/proj_tree_viewer_aui.py` & `piScope-1.0.9/python/ifigure/widgets/proj_tree_viewer_aui.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/proj_tree_viewer_aui2.py` & `piScope-1.0.9/python/ifigure/widgets/proj_tree_viewer_aui2.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/property_editor.py` & `piScope-1.0.9/python/ifigure/widgets/property_editor.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/radio_button.py` & `piScope-1.0.9/python/ifigure/widgets/radio_button.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/redirect_output.py` & `piScope-1.0.9/python/ifigure/widgets/redirect_output.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/script_editor.py` & `piScope-1.0.9/python/ifigure/widgets/script_editor.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/section_editor.py` & `piScope-1.0.9/python/ifigure/widgets/section_editor.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/shellvar_viewer.py` & `piScope-1.0.9/python/ifigure/widgets/shellvar_viewer.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/simple_shell.py` & `piScope-1.0.9/python/ifigure/widgets/simple_shell.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/slice_viewer.py` & `piScope-1.0.9/python/ifigure/widgets/slice_viewer.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/statusbar.py` & `piScope-1.0.9/python/ifigure/widgets/statusbar.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/syntax_styles.py` & `piScope-1.0.9/python/ifigure/widgets/syntax_styles.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/taskbar.py` & `piScope-1.0.9/python/ifigure/widgets/taskbar.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/textctrl_trunc.py` & `piScope-1.0.9/python/ifigure/widgets/textctrl_trunc.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/tipwindow.py` & `piScope-1.0.9/python/ifigure/widgets/tipwindow.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/undo_redo_history.py` & `piScope-1.0.9/python/ifigure/widgets/undo_redo_history.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/var_viewerg2.py` & `piScope-1.0.9/python/ifigure/widgets/var_viewerg2.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/video_viewer.py` & `piScope-1.0.9/python/ifigure/widgets/video_viewer.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/videoplayer_buttons.py` & `piScope-1.0.9/python/ifigure/widgets/videoplayer_buttons.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/ifigure/widgets/wave_viewer.py` & `piScope-1.0.9/python/ifigure/widgets/wave_viewer.py`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/python/piScope.egg-info/PKG-INFO` & `piScope-1.0.9/python/piScope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piScope
-Version: 1.0.8
+Version: 1.0.9
 Summary: piScope data analysis workbench
 Download-URL: https://github.com/piScope/piScope
 Author: S. Shiraiwa
 Author-email: shiraiwa@princeton.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `piScope-1.0.8/python/piScope.egg-info/SOURCES.txt` & `piScope-1.0.9/python/piScope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piScope-1.0.8/setup.py` & `piScope-1.0.9/setup.py`

 * *Files identical despite different names*

