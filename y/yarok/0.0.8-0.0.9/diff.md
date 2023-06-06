# Comparing `tmp/yarok-0.0.8.tar.gz` & `tmp/yarok-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yarok-0.0.8.tar", last modified: Wed Feb 16 15:44:56 2022, max compression
+gzip compressed data, was "yarok-0.0.9.tar", last modified: Wed Feb 16 15:53:47 2022, max compression
```

## Comparing `yarok-0.0.8.tar` & `yarok-0.0.9.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.728627 yarok-0.0.8/
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.680627 yarok-0.0.8/.idea/
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.680627 yarok-0.0.8/.idea/inspectionProfiles/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      410 2022-02-15 22:20:03.000000 yarok-0.0.8/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      174 2022-02-15 22:20:03.000000 yarok-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      262 2022-02-15 22:20:03.000000 yarok-0.0.8/.idea/modules.xml
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      180 2022-02-15 22:20:03.000000 yarok-0.0.8/.idea/vcs.xml
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     4070 2022-02-16 14:14:32.000000 yarok-0.0.8/.idea/workspace.xml
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)       72 2022-02-15 23:12:45.000000 yarok-0.0.8/MANIFEST.in
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     7126 2022-02-16 15:44:56.728627 yarok-0.0.8/PKG-INFO
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     6820 2022-02-15 22:19:06.000000 yarok-0.0.8/README.md
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.680627 yarok-0.0.8/examples/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      547 2022-02-15 22:19:06.000000 yarok-0.0.8/examples/__init__.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.680627 yarok-0.0.8/examples/empty_world/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      547 2022-02-15 22:19:06.000000 yarok-0.0.8/examples/empty_world/__init__.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     1130 2022-02-15 23:27:32.000000 yarok-0.0.8/examples/empty_world/empty_world.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     4654 2022-02-15 23:23:05.000000 yarok-0.0.8/examples/empty_world/empty_world.xml
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.680627 yarok-0.0.8/examples/empty_world/meshes/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    31584 2022-02-15 22:19:06.000000 yarok-0.0.8/examples/empty_world/meshes/cone.stl
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.680627 yarok-0.0.8/examples/empty_world/textures/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   703432 2022-02-15 22:19:06.000000 yarok-0.0.8/examples/empty_world/textures/floor_tile.png
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   318067 2022-02-15 22:19:06.000000 yarok-0.0.8/examples/empty_world/textures/marble.png
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)       38 2022-02-16 15:44:56.732627 yarok-0.0.8/setup.cfg
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      948 2022-02-16 15:44:29.000000 yarok-0.0.8/setup.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.680627 yarok-0.0.8/yarok/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      547 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/__init__.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     3319 2022-02-16 15:38:41.000000 yarok-0.0.8/yarok/__main__.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.684627 yarok-0.0.8/yarok/components/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:49:37.000000 yarok-0.0.8/yarok/components/__init__.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.684627 yarok-0.0.8/yarok/components/anet_a30/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:48.000000 yarok-0.0.8/yarok/components/anet_a30/__init__.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     4887 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/anet_a30/anet_a30.xml
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      935 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/anet_a30/anet_at30.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.692627 yarok-0.0.8/yarok/components/anet_a30/meshes/
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)  1142284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/anet_a30/meshes/CR-10_platform2.stl
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)   875684 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/anet_a30/meshes/bed.stl
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)   875684 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/anet_a30/meshes/bed2.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   271584 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/anet_a30/meshes/bottom_frame.stl
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)   266684 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/anet_a30/meshes/external_frame.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    70034 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/anet_a30/meshes/side1_frame.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    70484 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/anet_a30/meshes/side2_frame.stl
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)    47934 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/anet_a30/meshes/x_axis.stl
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.692627 yarok-0.0.8/yarok/components/cam/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:37.000000 yarok-0.0.8/yarok/components/cam/__init__.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      380 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/cam/cam.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      115 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/cam/cam.xml
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.692627 yarok-0.0.8/yarok/components/empty_world/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:47:23.000000 yarok-0.0.8/yarok/components/empty_world/__init__.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     1127 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/empty_world/empty_world.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     4559 2022-02-15 22:25:34.000000 yarok-0.0.8/yarok/components/empty_world/empty_world.xml
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.692627 yarok-0.0.8/yarok/components/empty_world/meshes/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    31584 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/empty_world/meshes/cone.stl
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.692627 yarok-0.0.8/yarok/components/empty_world/textures/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   703432 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/empty_world/textures/floor_tile.png
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   318067 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/empty_world/textures/marble.png
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.692627 yarok-0.0.8/yarok/components/gelsight2014/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:32.000000 yarok-0.0.8/yarok/components/gelsight2014/__init__.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   207563 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/gelsight2014/background.png
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      120 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/gelsight2014/gelsight2014.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     2792 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/gelsight2014/gelsight2014.xml
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.696627 yarok-0.0.8/yarok/components/gelsight2014/meshes/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    23084 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/gelsight2014/meshes/back_cover.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    23084 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/gelsight2014/meshes/gelsight2014_back.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    61684 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/gelsight2014/meshes/gelsight2014_front.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    61684 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/gelsight2014/meshes/gelsight2014_smartlab.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      684 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/gelsight2014/meshes/glass.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    79484 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/gelsight2014/meshes/mountable_gelsight.stl
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.696627 yarok-0.0.8/yarok/components/gelsight2017/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:15.000000 yarok-0.0.8/yarok/components/gelsight2017/__init__.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.696627 yarok-0.0.8/yarok/components/geltip/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:06.000000 yarok-0.0.8/yarok/components/geltip/__init__.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      114 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/geltip.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     1612 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/geltip.xml
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.708627 yarok-0.0.8/yarok/components/geltip/meshes/
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)    64284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/elastomer.stl
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)    64284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/elastomer_inv.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    64284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/elastomer_long.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    64284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/elastomer_long_inv.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    64284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/elastomer_very_long.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)  1169884 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/elastomer_very_long_quad_1.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)  1412284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/elastomer_very_long_voxel_e-6.stl
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)    57284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/glass.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    57284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/glass_long.stl
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)   152284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/mount.stl
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)    29884 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/shell.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    44484 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/shell_open.stl
--rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)   178584 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/sleeve.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   181084 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/geltip/meshes/sleeve_open.stl
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.708627 yarok-0.0.8/yarok/components/robotiq_2f85/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:49:37.000000 yarok-0.0.8/yarok/components/robotiq_2f85/__init__.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.720627 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    80184 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_end_0 v0.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    80184 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_end_1 v1.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   155584 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger1_0 v1.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   155584 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger1_1 v1.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   213484 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger2_0 v1.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   234884 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger4_0 v1.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)  4008984 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/base0.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   155584 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger01.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   367184 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger02.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   213484 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger03.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   234884 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger04.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    80184 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger0tip.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   155584 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger11.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   367184 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger12.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   213484 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger13.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   234884 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger14.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    80184 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger1tip.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      412 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/robotiq_2f85.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     6944 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/robotiq_2f85/robotiq_2f85.xml
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.720627 yarok-0.0.8/yarok/components/ur5/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:49:37.000000 yarok-0.0.8/yarok/components/ur5/__init__.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.728627 yarok-0.0.8/yarok/components/ur5/meshes/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   117984 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link0.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   177734 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link1.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   442734 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link1_cap.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link1_connector.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   355384 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link2.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   888084 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link2_cap.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link2_connector.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   211484 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link2_tube.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   365934 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link3_cap.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     5084 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link3_tube.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   148384 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link3a.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link3a_connector.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    93334 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link3b.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    15684 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link3b_connector.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    23884 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link3b_connector2.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    93334 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link4.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   365934 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link4_cap.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link4_connector.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    93334 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link5.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   366134 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link5_cap.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link5_connector.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   222184 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link6.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/meshes/link6_connector.stl
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     1133 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/ur5.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    10353 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components/ur5/ur5.xml
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    11193 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/components_manager.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.728627 yarok-0.0.8/yarok/hw/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:39:44.000000 yarok-0.0.8/yarok/hw/__init__.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      156 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/hw/viewer.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.728627 yarok-0.0.8/yarok/mjc/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:39:25.000000 yarok-0.0.8/yarok/mjc/__init__.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      990 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/mjc/interface.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     2077 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/mjc/platform.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     2007 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/mjc/viewer.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.728627 yarok-0.0.8/yarok/utils/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     4714 2022-02-15 22:19:06.000000 yarok-0.0.8/yarok/utils/PID.py
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:23.000000 yarok-0.0.8/yarok/utils/__init__.py
-drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:44:56.680627 yarok-0.0.8/yarok.egg-info/
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     7126 2022-02-16 15:44:56.000000 yarok-0.0.8/yarok.egg-info/PKG-INFO
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     5286 2022-02-16 15:44:56.000000 yarok-0.0.8/yarok.egg-info/SOURCES.txt
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        1 2022-02-16 15:44:56.000000 yarok-0.0.8/yarok.egg-info/dependency_links.txt
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)       47 2022-02-16 15:44:56.000000 yarok-0.0.8/yarok.egg-info/entry_points.txt
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)       10 2022-02-16 15:44:56.000000 yarok-0.0.8/yarok.egg-info/requires.txt
--rw-rw-r--   0 danfergo  (1000) danfergo  (1000)       15 2022-02-16 15:44:56.000000 yarok-0.0.8/yarok.egg-info/top_level.txt
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.151045 yarok-0.0.9/
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.115045 yarok-0.0.9/.idea/
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.115045 yarok-0.0.9/.idea/inspectionProfiles/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      410 2022-02-15 22:20:03.000000 yarok-0.0.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      174 2022-02-15 22:20:03.000000 yarok-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      262 2022-02-15 22:20:03.000000 yarok-0.0.9/.idea/modules.xml
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      180 2022-02-15 22:20:03.000000 yarok-0.0.9/.idea/vcs.xml
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     3351 2022-02-16 15:48:55.000000 yarok-0.0.9/.idea/workspace.xml
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)       72 2022-02-15 23:12:45.000000 yarok-0.0.9/MANIFEST.in
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     7126 2022-02-16 15:53:47.151045 yarok-0.0.9/PKG-INFO
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     6820 2022-02-15 22:19:06.000000 yarok-0.0.9/README.md
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.115045 yarok-0.0.9/examples/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      547 2022-02-15 22:19:06.000000 yarok-0.0.9/examples/__init__.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.115045 yarok-0.0.9/examples/empty_world/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:52:34.000000 yarok-0.0.9/examples/empty_world/__init__.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     1130 2022-02-15 23:27:32.000000 yarok-0.0.9/examples/empty_world/empty_world.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     4559 2022-02-16 15:47:45.000000 yarok-0.0.9/examples/empty_world/empty_world.xml
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.115045 yarok-0.0.9/examples/empty_world/meshes/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    31584 2022-02-15 22:19:06.000000 yarok-0.0.9/examples/empty_world/meshes/cone.stl
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.119045 yarok-0.0.9/examples/empty_world/textures/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   703432 2022-02-15 22:19:06.000000 yarok-0.0.9/examples/empty_world/textures/floor_tile.png
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   318067 2022-02-15 22:19:06.000000 yarok-0.0.9/examples/empty_world/textures/marble.png
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)       38 2022-02-16 15:53:47.151045 yarok-0.0.9/setup.cfg
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      948 2022-02-16 15:53:31.000000 yarok-0.0.9/setup.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.119045 yarok-0.0.9/yarok/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      547 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/__init__.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     3259 2022-02-16 15:46:59.000000 yarok-0.0.9/yarok/__main__.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.119045 yarok-0.0.9/yarok/components/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:49:37.000000 yarok-0.0.9/yarok/components/__init__.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.119045 yarok-0.0.9/yarok/components/anet_a30/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:48.000000 yarok-0.0.9/yarok/components/anet_a30/__init__.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     4887 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/anet_a30/anet_a30.xml
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      935 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/anet_a30/anet_at30.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.123045 yarok-0.0.9/yarok/components/anet_a30/meshes/
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)  1142284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/anet_a30/meshes/CR-10_platform2.stl
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)   875684 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/anet_a30/meshes/bed.stl
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)   875684 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/anet_a30/meshes/bed2.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   271584 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/anet_a30/meshes/bottom_frame.stl
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)   266684 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/anet_a30/meshes/external_frame.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    70034 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/anet_a30/meshes/side1_frame.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    70484 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/anet_a30/meshes/side2_frame.stl
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)    47934 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/anet_a30/meshes/x_axis.stl
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.123045 yarok-0.0.9/yarok/components/cam/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:37.000000 yarok-0.0.9/yarok/components/cam/__init__.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      380 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/cam/cam.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      115 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/cam/cam.xml
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.123045 yarok-0.0.9/yarok/components/empty_world/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:47:23.000000 yarok-0.0.9/yarok/components/empty_world/__init__.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     1127 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/empty_world/empty_world.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     4559 2022-02-15 22:25:34.000000 yarok-0.0.9/yarok/components/empty_world/empty_world.xml
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.123045 yarok-0.0.9/yarok/components/empty_world/meshes/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    31584 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/empty_world/meshes/cone.stl
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.127045 yarok-0.0.9/yarok/components/empty_world/textures/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   703432 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/empty_world/textures/floor_tile.png
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   318067 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/empty_world/textures/marble.png
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.127045 yarok-0.0.9/yarok/components/gelsight2014/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:32.000000 yarok-0.0.9/yarok/components/gelsight2014/__init__.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   207563 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/gelsight2014/background.png
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      120 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/gelsight2014/gelsight2014.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     2792 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/gelsight2014/gelsight2014.xml
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.127045 yarok-0.0.9/yarok/components/gelsight2014/meshes/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    23084 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/gelsight2014/meshes/back_cover.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    23084 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/gelsight2014/meshes/gelsight2014_back.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    61684 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/gelsight2014/meshes/gelsight2014_front.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    61684 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/gelsight2014/meshes/gelsight2014_smartlab.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      684 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/gelsight2014/meshes/glass.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    79484 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/gelsight2014/meshes/mountable_gelsight.stl
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.127045 yarok-0.0.9/yarok/components/gelsight2017/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:15.000000 yarok-0.0.9/yarok/components/gelsight2017/__init__.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.127045 yarok-0.0.9/yarok/components/geltip/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:06.000000 yarok-0.0.9/yarok/components/geltip/__init__.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      114 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/geltip.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     1612 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/geltip.xml
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.131045 yarok-0.0.9/yarok/components/geltip/meshes/
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)    64284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/elastomer.stl
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)    64284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/elastomer_inv.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    64284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/elastomer_long.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    64284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/elastomer_long_inv.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    64284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/elastomer_very_long.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)  1169884 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/elastomer_very_long_quad_1.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)  1412284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/elastomer_very_long_voxel_e-6.stl
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)    57284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/glass.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    57284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/glass_long.stl
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)   152284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/mount.stl
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)    29884 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/shell.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    44484 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/shell_open.stl
+-rwxrwxr-x   0 danfergo  (1000) danfergo  (1000)   178584 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/sleeve.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   181084 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/geltip/meshes/sleeve_open.stl
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.131045 yarok-0.0.9/yarok/components/robotiq_2f85/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:49:37.000000 yarok-0.0.9/yarok/components/robotiq_2f85/__init__.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.143045 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    80184 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_end_0 v0.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    80184 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_end_1 v1.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   155584 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger1_0 v1.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   155584 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger1_1 v1.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   213484 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger2_0 v1.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   234884 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger4_0 v1.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)  4008984 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/base0.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   155584 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger01.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   367184 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger02.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   213484 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger03.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   234884 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger04.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    80184 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger0tip.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   155584 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger11.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   367184 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger12.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   213484 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger13.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   234884 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger14.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    80184 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger1tip.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      412 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/robotiq_2f85.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     6944 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/robotiq_2f85/robotiq_2f85.xml
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.143045 yarok-0.0.9/yarok/components/ur5/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:49:37.000000 yarok-0.0.9/yarok/components/ur5/__init__.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.147045 yarok-0.0.9/yarok/components/ur5/meshes/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   117984 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link0.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   177734 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link1.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   442734 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link1_cap.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link1_connector.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   355384 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link2.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   888084 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link2_cap.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link2_connector.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   211484 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link2_tube.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   365934 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link3_cap.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     5084 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link3_tube.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   148384 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link3a.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link3a_connector.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    93334 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link3b.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    15684 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link3b_connector.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    23884 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link3b_connector2.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    93334 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link4.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   365934 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link4_cap.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link4_connector.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    93334 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link5.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   366134 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link5_cap.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link5_connector.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)   222184 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link6.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     8284 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/meshes/link6_connector.stl
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     1133 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/ur5.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    10353 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components/ur5/ur5.xml
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)    11193 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/components_manager.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.147045 yarok-0.0.9/yarok/hw/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:39:44.000000 yarok-0.0.9/yarok/hw/__init__.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      156 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/hw/viewer.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.147045 yarok-0.0.9/yarok/mjc/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:39:25.000000 yarok-0.0.9/yarok/mjc/__init__.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)      990 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/mjc/interface.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     2077 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/mjc/platform.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     2007 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/mjc/viewer.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.147045 yarok-0.0.9/yarok/utils/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     4714 2022-02-15 22:19:06.000000 yarok-0.0.9/yarok/utils/PID.py
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        0 2022-02-15 22:50:23.000000 yarok-0.0.9/yarok/utils/__init__.py
+drwxrwxr-x   0 danfergo  (1000) danfergo  (1000)        0 2022-02-16 15:53:47.119045 yarok-0.0.9/yarok.egg-info/
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     7126 2022-02-16 15:53:46.000000 yarok-0.0.9/yarok.egg-info/PKG-INFO
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)     5286 2022-02-16 15:53:47.000000 yarok-0.0.9/yarok.egg-info/SOURCES.txt
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)        1 2022-02-16 15:53:46.000000 yarok-0.0.9/yarok.egg-info/dependency_links.txt
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)       47 2022-02-16 15:53:46.000000 yarok-0.0.9/yarok.egg-info/entry_points.txt
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)       10 2022-02-16 15:53:46.000000 yarok-0.0.9/yarok.egg-info/requires.txt
+-rw-rw-r--   0 danfergo  (1000) danfergo  (1000)       15 2022-02-16 15:53:46.000000 yarok-0.0.9/yarok.egg-info/top_level.txt
```

### Comparing `yarok-0.0.8/PKG-INFO` & `yarok-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarok
-Version: 0.0.8
+Version: 0.0.9
 Summary: YAROK - Yet another robot framework
 Home-page: https://github.com/danfergo/yarok
 Author: danfergo
 Author-email: danfergo@gmail.com
 License: UNKNOWN
 Keywords: yarok,robot,framework,mujoco
 Platform: UNKNOWN
```

### Comparing `yarok-0.0.8/README.md` & `yarok-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/examples/__init__.py` & `yarok-0.0.9/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/examples/empty_world/__init__.py` & `yarok-0.0.9/yarok/__init__.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/examples/empty_world/empty_world.py` & `yarok-0.0.9/examples/empty_world/empty_world.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/examples/empty_world/empty_world.xml` & `yarok-0.0.9/examples/empty_world/empty_world.xml`

 * *Files 4% similar despite different names*

#### Comparing `yarok-0.0.8/examples/empty_world/empty_world.xml` & `yarok-0.0.9/examples/empty_world/empty_world.xml`

```diff
@@ -26,23 +26,23 @@
     <body name="floor">
       <geom name="ground" type="plane" size="0 0 1" pos="0 0 0" quat="1 0 0 0" material="matplane" condim="1"/>
     </body>
     <body pos="3 2 0">
       <anet_a30 name="printer"/>
     </body>
     <!-- UR5 Arm & Gripper -->
-    <!--        <body pos="0 0 .615">-->
-    <!--            <ur5 name="mani">-->
-    <!--                <robotiq_2f85 name="gripper1" parent="ee_link">-->
-    <!--                    <geltip name="geltip1" parent="gelsight_0"/>-->
-    <!--&lt;!&ndash;                    <gelsight2014 name="gelsight1" parent="gelsight_0"/>&ndash;&gt;-->
-    <!--&lt;!&ndash;                    <gelsight2014 name="gelsight2" parent="gelsight_1"/>&ndash;&gt;-->
-    <!--                </robotiq_2f85>-->
-    <!--            </ur5>-->
-    <!--        </body>-->
+    <body pos="0 0 .615">
+      <ur5 name="mani">
+        <robotiq_2f85 name="gripper1" parent="ee_link">
+          <geltip name="geltip1" parent="gelsight_0"/>
+          <!--                    <gelsight2014 name="gelsight1" parent="gelsight_0"/>-->
+          <!--                    <gelsight2014 name="gelsight2" parent="gelsight_1"/>-->
+        </robotiq_2f85>
+      </ur5>
+    </body>
     <!--        <body pos="1 0 .615">-->
     <!--            <ur5 name="mani">-->
     <!--                <robotiq_2f85 name="gripper2" parent="ee_link">-->
     <!--                    <body zaxis="-1 0 0" parent="gelsight_0">-->
     <!--                        <geltip name="geltip1"/>-->
     <!--                    </body>-->
     <!--                    <body zaxis="-1 0 0" parent="gelsight_1">-->
```

### Comparing `yarok-0.0.8/examples/empty_world/meshes/cone.stl` & `yarok-0.0.9/examples/empty_world/meshes/cone.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/examples/empty_world/textures/floor_tile.png` & `yarok-0.0.9/examples/empty_world/textures/floor_tile.png`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/examples/empty_world/textures/marble.png` & `yarok-0.0.9/examples/empty_world/textures/marble.png`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/setup.py` & `yarok-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 setup(
     name='yarok',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
-    version='0.0.8',
+    version='0.0.9',
     description='YAROK - Yet another robot framework',
     author='danfergo',
     entry_points={
         'console_scripts': [
             'yarok = yarok.__main__:main'
         ],
     },
```

### Comparing `yarok-0.0.8/yarok/__main__.py` & `yarok-0.0.9/yarok/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 
     try:
         spec = importlib.util.spec_from_file_location(module_name, os.getcwd() + '/' + p.replace('.', '/') + ".py")
         module = importlib.util.module_from_spec(spec)
         sys.modules[module_name] = module
         spec.loader.exec_module(module)
     except FileNotFoundError:
-        module = importlib.import_module(path, __package__)
-    # print('>> ', p.rfind('.'), p, module_name, to_camel_case(module_name))
+        module = importlib.import_module('.components.' + path, __package__)
     return getattr(module, to_camel_case(module_name))
 
 
 def main():
     """
         Converter command entry point.
     """
```

### Comparing `yarok-0.0.8/yarok/components/anet_a30/anet_a30.xml` & `yarok-0.0.9/yarok/components/anet_a30/anet_a30.xml`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/anet_a30/anet_at30.py` & `yarok-0.0.9/yarok/components/anet_a30/anet_at30.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/anet_a30/meshes/CR-10_platform2.stl` & `yarok-0.0.9/yarok/components/anet_a30/meshes/CR-10_platform2.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/anet_a30/meshes/bed.stl` & `yarok-0.0.9/yarok/components/anet_a30/meshes/bed.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/anet_a30/meshes/bed2.stl` & `yarok-0.0.9/yarok/components/anet_a30/meshes/bed2.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/anet_a30/meshes/bottom_frame.stl` & `yarok-0.0.9/yarok/components/anet_a30/meshes/bottom_frame.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/anet_a30/meshes/external_frame.stl` & `yarok-0.0.9/yarok/components/anet_a30/meshes/external_frame.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/anet_a30/meshes/side1_frame.stl` & `yarok-0.0.9/yarok/components/anet_a30/meshes/side1_frame.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/anet_a30/meshes/side2_frame.stl` & `yarok-0.0.9/yarok/components/anet_a30/meshes/side2_frame.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/anet_a30/meshes/x_axis.stl` & `yarok-0.0.9/yarok/components/anet_a30/meshes/x_axis.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/empty_world/empty_world.py` & `yarok-0.0.9/yarok/components/empty_world/empty_world.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/empty_world/empty_world.xml` & `yarok-0.0.9/yarok/components/empty_world/empty_world.xml`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/empty_world/meshes/cone.stl` & `yarok-0.0.9/yarok/components/empty_world/meshes/cone.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/empty_world/textures/floor_tile.png` & `yarok-0.0.9/yarok/components/empty_world/textures/floor_tile.png`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/empty_world/textures/marble.png` & `yarok-0.0.9/yarok/components/empty_world/textures/marble.png`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/gelsight2014/background.png` & `yarok-0.0.9/yarok/components/gelsight2014/background.png`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/gelsight2014/gelsight2014.xml` & `yarok-0.0.9/yarok/components/gelsight2014/gelsight2014.xml`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/gelsight2014/meshes/back_cover.stl` & `yarok-0.0.9/yarok/components/gelsight2014/meshes/back_cover.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/gelsight2014/meshes/gelsight2014_back.stl` & `yarok-0.0.9/yarok/components/gelsight2014/meshes/gelsight2014_back.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/gelsight2014/meshes/gelsight2014_front.stl` & `yarok-0.0.9/yarok/components/gelsight2014/meshes/gelsight2014_front.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/gelsight2014/meshes/gelsight2014_smartlab.stl` & `yarok-0.0.9/yarok/components/gelsight2014/meshes/gelsight2014_smartlab.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/gelsight2014/meshes/glass.stl` & `yarok-0.0.9/yarok/components/gelsight2014/meshes/glass.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/gelsight2014/meshes/mountable_gelsight.stl` & `yarok-0.0.9/yarok/components/gelsight2014/meshes/mountable_gelsight.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/geltip.xml` & `yarok-0.0.9/yarok/components/geltip/geltip.xml`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/elastomer.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/elastomer.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/elastomer_inv.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/elastomer_inv.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/elastomer_long.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/elastomer_long.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/elastomer_long_inv.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/elastomer_long_inv.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/elastomer_very_long.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/elastomer_very_long.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/elastomer_very_long_quad_1.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/elastomer_very_long_quad_1.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/elastomer_very_long_voxel_e-6.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/elastomer_very_long_voxel_e-6.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/glass.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/glass.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/glass_long.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/glass_long.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/mount.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/mount.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/shell.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/shell.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/shell_open.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/shell_open.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/sleeve.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/sleeve.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/geltip/meshes/sleeve_open.stl` & `yarok-0.0.9/yarok/components/geltip/meshes/sleeve_open.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_end_0 v0.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_end_0 v0.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_end_1 v1.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_end_1 v1.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger1_0 v1.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger1_0 v1.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger1_1 v1.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger1_1 v1.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger2_0 v1.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger2_0 v1.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger4_0 v1.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/2F85_Opened_20190924_finger4_0 v1.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/base0.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/base0.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger01.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger01.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger02.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger02.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger03.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger03.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger04.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger04.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger0tip.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger0tip.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger11.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger11.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger12.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger12.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger13.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger13.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger14.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger14.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/meshes/finger1tip.stl` & `yarok-0.0.9/yarok/components/robotiq_2f85/meshes/finger1tip.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/robotiq_2f85/robotiq_2f85.xml` & `yarok-0.0.9/yarok/components/robotiq_2f85/robotiq_2f85.xml`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link0.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link0.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link1.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link1.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link1_cap.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link1_cap.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link1_connector.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link1_connector.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link2.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link2.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link2_cap.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link2_cap.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link2_connector.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link2_connector.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link2_tube.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link2_tube.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link3_cap.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link3_cap.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link3_tube.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link3_tube.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link3a.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link3a.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link3a_connector.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link3a_connector.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link3b.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link3b.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link3b_connector.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link3b_connector.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link3b_connector2.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link3b_connector2.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link4.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link4.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link4_cap.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link4_cap.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link4_connector.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link4_connector.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link5.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link5.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link5_cap.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link5_cap.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link5_connector.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link5_connector.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link6.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link6.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/meshes/link6_connector.stl` & `yarok-0.0.9/yarok/components/ur5/meshes/link6_connector.stl`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/ur5.py` & `yarok-0.0.9/yarok/components/ur5/ur5.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components/ur5/ur5.xml` & `yarok-0.0.9/yarok/components/ur5/ur5.xml`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/components_manager.py` & `yarok-0.0.9/yarok/components_manager.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/mjc/interface.py` & `yarok-0.0.9/yarok/mjc/interface.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/mjc/platform.py` & `yarok-0.0.9/yarok/mjc/platform.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/mjc/viewer.py` & `yarok-0.0.9/yarok/mjc/viewer.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok/utils/PID.py` & `yarok-0.0.9/yarok/utils/PID.py`

 * *Files identical despite different names*

### Comparing `yarok-0.0.8/yarok.egg-info/PKG-INFO` & `yarok-0.0.9/yarok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarok
-Version: 0.0.8
+Version: 0.0.9
 Summary: YAROK - Yet another robot framework
 Home-page: https://github.com/danfergo/yarok
 Author: danfergo
 Author-email: danfergo@gmail.com
 License: UNKNOWN
 Keywords: yarok,robot,framework,mujoco
 Platform: UNKNOWN
```

### Comparing `yarok-0.0.8/yarok.egg-info/SOURCES.txt` & `yarok-0.0.9/yarok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

