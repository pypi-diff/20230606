# Comparing `tmp/pyschism-0.1.6.tar.gz` & `tmp/pyschism-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyschism-0.1.6.tar", last modified: Thu Mar 30 18:15:30 2023, max compression
+gzip compressed data, was "pyschism-0.1.7.tar", last modified: Fri Apr 14 18:26:50 2023, max compression
```

## Comparing `pyschism-0.1.6.tar` & `pyschism-0.1.7.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.150735 pyschism-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-30 18:15:17.000000 pyschism-0.1.6/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.126735 pyschism-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.134735 pyschism-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-30 18:15:17.000000 pyschism-0.1.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-30 18:15:17.000000 pyschism-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-30 18:15:17.000000 pyschism-0.1.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-30 18:15:17.000000 pyschism-0.1.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-03-30 18:15:17.000000 pyschism-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-30 18:15:30.150735 pyschism-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-30 18:15:17.000000 pyschism-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.134735 pyschism-0.1.6/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-30 18:15:17.000000 pyschism-0.1.6/docker/arch-linux-base.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-30 18:15:17.000000 pyschism-0.1.6/docker/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-30 18:15:17.000000 pyschism-0.1.6/docker/pyschism-arch-unittest.Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.134735 pyschism-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.134735 pyschism-0.1.6/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.138735 pyschism-0.1.6/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/driver.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/mesh.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/param.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/pyschism.cmd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/pyschism.cmd.server.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/pyschism.forcing.atmosphere.rst
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/pyschism.forcing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/pyschism.forcing.tides.rst
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/pyschism.mesh.friction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/pyschism.mesh.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/pyschism.param.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/pyschism.rst
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/api/stations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-30 18:15:17.000000 pyschism-0.1.6/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.126735 pyschism-0.1.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.138735 pyschism-0.1.6/examples/example_1/
--rw-r--r--   0 runner    (1001) docker     (123)    30816 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/example_1/example_1.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)     2770 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/example_1/example_1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3652 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/example_1/example_1_tide-gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)   236679 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/example_1/hgrid.png
--rw-r--r--   0 runner    (1001) docker     (123)    18446 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/example_1/station.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.138735 pyschism-0.1.6/examples/example_2/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/example_2/example_2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.138735 pyschism-0.1.6/examples/example_3/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/example_3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    38167 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/example_3/example_3.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.138735 pyschism-0.1.6/examples/example_4/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/example_4/test_hycom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.138735 pyschism-0.1.6/examples/examples_gridgr3/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/examples_gridgr3/01_gen_drag.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/examples_gridgr3/02_gen_shapiro.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/examples_gridgr3/03_gen_shapiro2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.138735 pyschism-0.1.6/examples/examples_hindcast/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/examples_hindcast/01_nwm.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/examples_hindcast/02_era5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.138735 pyschism-0.1.6/examples/examples_sflux/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/examples_sflux/gen_sflux_era5.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/examples_sflux/gen_sflux_gfs2.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/examples_sflux/gen_sflux_hrrr3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-30 18:15:17.000000 pyschism-0.1.6/examples/examples_sflux/link_sflux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.138735 pyschism-0.1.6/pyschism/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.142735 pyschism-0.1.6/pyschism/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.142735 pyschism-0.1.6/pyschism/cmd/_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/_forecast/_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/_forecast/_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/_nudge.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/basedaemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/bctides.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.142735 pyschism-0.1.6/pyschism/cmd/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/bootstrap/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    62907 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.142735 pyschism-0.1.6/pyschism/cmd/fgrid/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/fgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/fgrid/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/fgrid/manning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/fluxflag.py
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/grd2sms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/hgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/sflux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/sms2grd.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/tvdflag.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/cmd/vgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)    33643 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.142735 pyschism-0.1.6/pyschism/forcing/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.142735 pyschism-0.1.6/pyschism/forcing/bctides/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/bctides.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/bctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/elev2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/hamtide.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/iettype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/ifltype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/isatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/itetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/itrtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/mod3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/nudge.py
--rw-r--r--   0 runner    (1001) docker     (123)    23270 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/tpxo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/bctides/uv3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.142735 pyschism-0.1.6/pyschism/forcing/hycom/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/hycom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/hycom/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34502 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/hycom/gofs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30460 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/hycom/hycom2schism.py
--rw-r--r--   0 runner    (1001) docker     (123)    25180 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/hycom/rtofs2schism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.142735 pyschism-0.1.6/pyschism/forcing/nws/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/best_track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.146735 pyschism-0.1.6/pyschism/forcing/nws/nws2/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/nws2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/nws2/era5.py
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/nws2/gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/nws2/gfs2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/nws2/hrrr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/nws2/hrrr2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/nws2/hrrr3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/nws2/nws2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/nws2/sflux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/nws2/sflux_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19900 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/nws/tcprof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.146735 pyschism-0.1.6/pyschism/forcing/source_sink/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/source_sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20108 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/source_sink/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    35640 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/forcing/source_sink/nwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/hotstart.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/makefile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.146735 pyschism-0.1.6/pyschism/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/fgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/gridgr3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/hgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.146735 pyschism-0.1.6/pyschism/mesh/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/parsers/grd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/parsers/sms2dm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/mesh/vgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.146735 pyschism-0.1.6/pyschism/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/outputs/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/outputs/hydro.py
--rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/outputs/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/outputs/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/outputs/stations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.146735 pyschism-0.1.6/pyschism/param/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/param/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/param/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/param/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/param/schism_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/param/schout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.146735 pyschism-0.1.6/pyschism/server/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/server/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/server/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/stations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.146735 pyschism-0.1.6/pyschism/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/utils/coops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-30 18:15:17.000000 pyschism-0.1.6/pyschism/utils/timedeltatype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.138735 pyschism-0.1.6/pyschism.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-30 18:15:30.000000 pyschism-0.1.6/pyschism.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-03-30 18:15:30.000000 pyschism-0.1.6/pyschism.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 18:15:30.000000 pyschism-0.1.6/pyschism.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 18:15:30.000000 pyschism-0.1.6/pyschism.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-30 18:15:30.000000 pyschism-0.1.6/pyschism.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 18:15:30.000000 pyschism-0.1.6/pyschism.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-30 18:15:30.150735 pyschism-0.1.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4497 2023-03-30 18:15:17.000000 pyschism-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.150735 pyschism-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.150735 pyschism-0.1.6/tests/_mesh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/_mesh/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12347 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/_mesh/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/_mesh/test_fgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/_mesh/test_grd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7599 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/_mesh/test_hgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/_mesh/test_manning.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4794 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/_mesh/test_mesh.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2815 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/_mesh/test_sms2dm.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/_mesh/test_vgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.130735 pyschism-0.1.6/tests/sciclone/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.130735 pyschism-0.1.6/tests/sciclone/Gulf_Stream_develop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.150735 pyschism-0.1.6/tests/sciclone/Gulf_Stream_develop/forecast-cli-2D/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/sciclone/Gulf_Stream_develop/forecast-cli-2D/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.130735 pyschism-0.1.6/tests/sciclone/ICOGS2D/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.130735 pyschism-0.1.6/tests/sciclone/ICOGS2D/Florence2018/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.130735 pyschism-0.1.6/tests/sciclone/ICOGS2D/Florence2018/bctides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.150735 pyschism-0.1.6/tests/sciclone/ICOGS2D/Florence2018/bctides/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/sciclone/ICOGS2D/Florence2018/bctides/cli/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/sciclone/ICOGS2D/Florence2018/bctides/cli/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.130735 pyschism-0.1.6/tests/sciclone/ICOGS3D/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.130735 pyschism-0.1.6/tests/sciclone/ICOGS3D/Florence2018/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:15:30.150735 pyschism-0.1.6/tests/sciclone/ICOGS3D/Florence2018/NWM/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/sciclone/ICOGS3D/Florence2018/NWM/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/sciclone/ICOGS3D/Florence2018/NWM/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2462 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/test_barotropic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3551 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/test_bctides.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/test_icogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/test_nwm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/test_outputs_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/test_outputs_api_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/test_paramwind.py
--rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-03-30 18:15:17.000000 pyschism-0.1.6/tests/tropycal.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 18:26:38.000000 pyschism-0.1.7/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.710524 pyschism-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-14 18:26:38.000000 pyschism-0.1.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-14 18:26:38.000000 pyschism-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-14 18:26:38.000000 pyschism-0.1.7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-14 18:26:38.000000 pyschism-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-04-14 18:26:38.000000 pyschism-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-14 18:26:50.726524 pyschism-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-14 18:26:38.000000 pyschism-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 18:26:38.000000 pyschism-0.1.7/docker/arch-linux-base.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-14 18:26:38.000000 pyschism-0.1.7/docker/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-14 18:26:38.000000 pyschism-0.1.7/docker/pyschism-arch-unittest.Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/driver.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/mesh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/param.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/pyschism.cmd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/pyschism.cmd.server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/pyschism.forcing.atmosphere.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/pyschism.forcing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/pyschism.forcing.tides.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/pyschism.mesh.friction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/pyschism.mesh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/pyschism.param.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/pyschism.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/api/stations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-14 18:26:38.000000 pyschism-0.1.7/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.710524 pyschism-0.1.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/examples/example_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30816 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/example_1/example_1.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2770 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/example_1/example_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3652 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/example_1/example_1_tide-gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   236679 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/example_1/hgrid.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18446 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/example_1/station.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/examples/example_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/example_2/example_2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/examples/example_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/example_3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    38167 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/example_3/example_3.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/examples/example_4/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/example_4/test_hycom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/examples/examples_gridgr3/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/examples_gridgr3/01_gen_drag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/examples_gridgr3/02_gen_shapiro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/examples_gridgr3/03_gen_shapiro2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/examples/examples_hindcast/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/examples_hindcast/01_nwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/examples_hindcast/02_era5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/examples/examples_sflux/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/examples_sflux/gen_sflux_era5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/examples_sflux/gen_sflux_gfs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/examples_sflux/gen_sflux_hrrr3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-14 18:26:38.000000 pyschism-0.1.7/examples/examples_sflux/link_sflux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/pyschism/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/pyschism/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/pyschism/cmd/_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/_forecast/_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/_forecast/_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/_nudge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/basedaemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/bctides.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/pyschism/cmd/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/bootstrap/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62907 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.722524 pyschism-0.1.7/pyschism/cmd/fgrid/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/fgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/fgrid/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/fgrid/manning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/fluxflag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/grd2sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/hgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/sflux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/sms2grd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/tvdflag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/cmd/vgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33649 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.722524 pyschism-0.1.7/pyschism/forcing/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.722524 pyschism-0.1.7/pyschism/forcing/bctides/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/bctides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/bctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/elev2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/hamtide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/iettype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/ifltype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/isatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/itetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/itrtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/mod3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/nudge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23270 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/tpxo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/bctides/uv3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.722524 pyschism-0.1.7/pyschism/forcing/hycom/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/hycom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/hycom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34502 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/hycom/gofs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30460 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/hycom/hycom2schism.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25180 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/hycom/rtofs2schism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.722524 pyschism-0.1.7/pyschism/forcing/nws/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/best_track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.722524 pyschism-0.1.7/pyschism/forcing/nws/nws2/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/nws2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/nws2/era5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/nws2/gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/nws2/gfs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/nws2/hrrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/nws2/hrrr2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/nws2/hrrr3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/nws2/nws2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/nws2/sflux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/nws2/sflux_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19900 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/nws/tcprof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.722524 pyschism-0.1.7/pyschism/forcing/source_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/source_sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20108 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/source_sink/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35640 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/forcing/source_sink/nwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/hotstart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/makefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/pyschism/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/fgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/gridgr3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/hgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/pyschism/mesh/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/parsers/grd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/parsers/sms2dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/mesh/vgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/pyschism/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/outputs/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/outputs/hydro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/outputs/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/outputs/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/outputs/stations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/pyschism/param/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/param/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/param/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/param/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/param/schism_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/param/schout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/pyschism/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/server/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/server/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/stations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/pyschism/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/utils/coops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-14 18:26:38.000000 pyschism-0.1.7/pyschism/utils/timedeltatype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.718524 pyschism-0.1.7/pyschism.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-14 18:26:50.000000 pyschism-0.1.7/pyschism.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-14 18:26:50.000000 pyschism-0.1.7/pyschism.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:26:50.000000 pyschism-0.1.7/pyschism.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 18:26:50.000000 pyschism-0.1.7/pyschism.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-14 18:26:50.000000 pyschism-0.1.7/pyschism.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 18:26:50.000000 pyschism-0.1.7/pyschism.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-14 18:26:50.730524 pyschism-0.1.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4433 2023-04-14 18:26:38.000000 pyschism-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/tests/_mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/_mesh/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12347 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/_mesh/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/_mesh/test_fgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/_mesh/test_grd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7599 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/_mesh/test_hgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/_mesh/test_manning.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4794 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/_mesh/test_mesh.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2815 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/_mesh/test_sms2dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/_mesh/test_vgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/tests/sciclone/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/tests/sciclone/Gulf_Stream_develop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/tests/sciclone/Gulf_Stream_develop/forecast-cli-2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/sciclone/Gulf_Stream_develop/forecast-cli-2D/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/tests/sciclone/ICOGS2D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/tests/sciclone/ICOGS2D/Florence2018/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/tests/sciclone/ICOGS2D/Florence2018/bctides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/tests/sciclone/ICOGS2D/Florence2018/bctides/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/sciclone/ICOGS2D/Florence2018/bctides/cli/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/sciclone/ICOGS2D/Florence2018/bctides/cli/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/tests/sciclone/ICOGS3D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.714524 pyschism-0.1.7/tests/sciclone/ICOGS3D/Florence2018/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:26:50.726524 pyschism-0.1.7/tests/sciclone/ICOGS3D/Florence2018/NWM/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/sciclone/ICOGS3D/Florence2018/NWM/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/sciclone/ICOGS3D/Florence2018/NWM/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2462 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/test_barotropic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3551 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/test_bctides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/test_icogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/test_nwm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/test_outputs_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/test_outputs_api_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/test_paramwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-04-14 18:26:38.000000 pyschism-0.1.7/tests/tropycal.ipynb
```

### Comparing `pyschism-0.1.6/.github/workflows/release.yml` & `pyschism-0.1.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/CONTRIBUTING.md` & `pyschism-0.1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/LICENSE.txt` & `pyschism-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/PKG-INFO` & `pyschism-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschism
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for working with SCHISM input and output files.
 Home-page: https://github.com/schism-dev/pyschism.git
 Author: "SCHISM development group"
 Author-email: jreniel@gmail.com, lcui@vims.edu
 License: "Apache 2.0"
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
```

### Comparing `pyschism-0.1.6/README.md` & `pyschism-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docker/pyschism-arch-unittest.Dockerfile` & `pyschism-0.1.7/docker/pyschism-arch-unittest.Dockerfile`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/Makefile` & `pyschism-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/make.bat` & `pyschism-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/source/api/pyschism.cmd.rst` & `pyschism-0.1.7/docs/source/api/pyschism.cmd.rst`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/source/api/pyschism.cmd.server.rst` & `pyschism-0.1.7/docs/source/api/pyschism.cmd.server.rst`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/source/api/pyschism.forcing.atmosphere.rst` & `pyschism-0.1.7/docs/source/api/pyschism.forcing.atmosphere.rst`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/source/api/pyschism.forcing.tides.rst` & `pyschism-0.1.7/docs/source/api/pyschism.forcing.tides.rst`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/source/api/pyschism.mesh.friction.rst` & `pyschism-0.1.7/docs/source/api/pyschism.mesh.friction.rst`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/source/api/pyschism.mesh.rst` & `pyschism-0.1.7/docs/source/api/pyschism.mesh.rst`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/source/api/pyschism.param.rst` & `pyschism-0.1.7/docs/source/api/pyschism.param.rst`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/source/conf.py` & `pyschism-0.1.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/source/index.rst` & `pyschism-0.1.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/docs/source/quickstart.rst` & `pyschism-0.1.7/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/example_1/example_1.ipynb` & `pyschism-0.1.7/examples/example_1/example_1.ipynb`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/example_1/example_1.py` & `pyschism-0.1.7/examples/example_1/example_1.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/example_1/example_1_tide-gfs.py` & `pyschism-0.1.7/examples/example_1/example_1_tide-gfs.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/example_1/hgrid.png` & `pyschism-0.1.7/examples/example_1/hgrid.png`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/example_1/station.in` & `pyschism-0.1.7/examples/example_1/station.in`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/example_2/example_2.json` & `pyschism-0.1.7/examples/example_2/example_2.json`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/example_3/example_3.ipynb` & `pyschism-0.1.7/examples/example_3/example_3.ipynb`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/example_4/test_hycom.py` & `pyschism-0.1.7/examples/example_4/test_hycom.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/examples_gridgr3/01_gen_drag.py` & `pyschism-0.1.7/examples/examples_gridgr3/01_gen_drag.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/examples_gridgr3/02_gen_shapiro.py` & `pyschism-0.1.7/examples/examples_gridgr3/02_gen_shapiro.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/examples_gridgr3/03_gen_shapiro2.py` & `pyschism-0.1.7/examples/examples_gridgr3/03_gen_shapiro2.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/examples_hindcast/01_nwm.py` & `pyschism-0.1.7/examples/examples_hindcast/01_nwm.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/examples_hindcast/02_era5.py` & `pyschism-0.1.7/examples/examples_hindcast/02_era5.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/examples_sflux/gen_sflux_era5.py` & `pyschism-0.1.7/examples/examples_sflux/gen_sflux_era5.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/examples_sflux/gen_sflux_gfs2.py` & `pyschism-0.1.7/examples/examples_sflux/gen_sflux_gfs2.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/examples_sflux/gen_sflux_hrrr3.py` & `pyschism-0.1.7/examples/examples_sflux/gen_sflux_hrrr3.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/examples/examples_sflux/link_sflux.py` & `pyschism-0.1.7/examples/examples_sflux/link_sflux.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/__main__.py` & `pyschism-0.1.7/pyschism/__main__.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/__init__.py` & `pyschism-0.1.7/pyschism/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/_forecast/_init.py` & `pyschism-0.1.7/pyschism/cmd/_forecast/_init.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/_forecast/_update.py` & `pyschism-0.1.7/pyschism/cmd/_forecast/_update.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/_nudge.py` & `pyschism-0.1.7/pyschism/cmd/_nudge.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/basedaemon.py` & `pyschism-0.1.7/pyschism/cmd/basedaemon.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/bctides.py` & `pyschism-0.1.7/pyschism/cmd/bctides.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/bootstrap/bootstrap.py` & `pyschism-0.1.7/pyschism/cmd/bootstrap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/common.py` & `pyschism-0.1.7/pyschism/cmd/common.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/fgrid/entry.py` & `pyschism-0.1.7/pyschism/cmd/fgrid/entry.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/fgrid/manning.py` & `pyschism-0.1.7/pyschism/cmd/fgrid/manning.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/fluxflag.py` & `pyschism-0.1.7/pyschism/cmd/fluxflag.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/forecast.py` & `pyschism-0.1.7/pyschism/cmd/forecast.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/grd2sms.py` & `pyschism-0.1.7/pyschism/cmd/grd2sms.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/hgrid.py` & `pyschism-0.1.7/pyschism/cmd/hgrid.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/outputs.py` & `pyschism-0.1.7/pyschism/cmd/outputs.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/sflux.py` & `pyschism-0.1.7/pyschism/cmd/sflux.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/sms2grd.py` & `pyschism-0.1.7/pyschism/cmd/sms2grd.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/stations.py` & `pyschism-0.1.7/pyschism/cmd/stations.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/tvdflag.py` & `pyschism-0.1.7/pyschism/cmd/tvdflag.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/cmd/vgrid.py` & `pyschism-0.1.7/pyschism/cmd/vgrid.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/dates.py` & `pyschism-0.1.7/pyschism/dates.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/driver.py` & `pyschism-0.1.7/pyschism/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
                     )
             elif isinstance(self.config.forcings.nws, BestTrackForcing):
                 # Writing the rotation file is still needed, but it's
                 # not meaningful for BestTrackForcing
                 self.config.forcings.nws.windrot = gridgr3.Windrot.default(
                     self.config.hgrid
                 )
-                self.param.opt.model_type_pahm = self.config.forcings.nws.model
+                self.param.opt.model_type_pahm = self.config.forcings.nws.model.value
 
             self.param.opt.wtiminc = self.param.core.dt
             self.param.opt.nws = self.config.forcings.nws.dtype.value
 
         if self.config.forcings.source_sink is not None:
             if self.elev_ic is None:
                 if self.hotstart is None:
```

### Comparing `pyschism-0.1.6/pyschism/enums.py` & `pyschism-0.1.7/pyschism/enums.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/figures.py` & `pyschism-0.1.7/pyschism/figures.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/elev2d.py` & `pyschism-0.1.7/pyschism/forcing/bctides/elev2d.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/hamtide.py` & `pyschism-0.1.7/pyschism/forcing/bctides/hamtide.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/iettype.py` & `pyschism-0.1.7/pyschism/forcing/bctides/iettype.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/ifltype.py` & `pyschism-0.1.7/pyschism/forcing/bctides/ifltype.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/isatype.py` & `pyschism-0.1.7/pyschism/forcing/bctides/isatype.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/itetype.py` & `pyschism-0.1.7/pyschism/forcing/bctides/itetype.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/itrtype.py` & `pyschism-0.1.7/pyschism/forcing/bctides/itrtype.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/mod3d.py` & `pyschism-0.1.7/pyschism/forcing/bctides/mod3d.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/nudge.py` & `pyschism-0.1.7/pyschism/forcing/bctides/nudge.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/tides.py` & `pyschism-0.1.7/pyschism/forcing/bctides/tides.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/tpxo.py` & `pyschism-0.1.7/pyschism/forcing/bctides/tpxo.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/bctides/uv3d.py` & `pyschism-0.1.7/pyschism/forcing/bctides/uv3d.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/hycom/base.py` & `pyschism-0.1.7/pyschism/forcing/hycom/base.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/hycom/gofs.py` & `pyschism-0.1.7/pyschism/forcing/hycom/gofs.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/hycom/hycom2schism.py` & `pyschism-0.1.7/pyschism/forcing/hycom/hycom2schism.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/hycom/rtofs2schism.py` & `pyschism-0.1.7/pyschism/forcing/hycom/rtofs2schism.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/base.py` & `pyschism-0.1.7/pyschism/forcing/nws/base.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/best_track.py` & `pyschism-0.1.7/pyschism/forcing/nws/best_track.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,66 +3,61 @@
 import logging
 import os
 import pathlib
 from enum import IntEnum
 from os import PathLike
 from typing import Union
 
-from matplotlib import pyplot
-from matplotlib.axis import Axis
 from matplotlib.transforms import Bbox
 import numpy as numpy
 from pandas import DataFrame
 from pyproj import CRS, Transformer
 from shapely import ops
 from shapely.geometry import Point, Polygon
 from stormevents.nhc import VortexTrack
-from stormevents.nhc.atcf import ATCF_Mode
 import utm
 
 from pyschism.enums import NWSType
 from pyschism.forcing.nws.base import NWS
-from pyschism.forcing.nws.nws2.sflux import SfluxDataset
-from pyschism.mesh import gridgr3
 
 
 class HurricaneModel(IntEnum):
     SYMMETRIC = 1
     GAHM = 10
 
+    @classmethod
+    def _missing_(cls, value):
+        raise ValueError(f"Invalid hurricane model specified: {value}, choose from: {cls.__members__}")
 
 
 class BestTrackForcing(VortexTrack, NWS):
 
     def __init__(
         self,
         storm: Union[str, PathLike, DataFrame, io.BytesIO],
         start_date: datetime = None,
         end_date: datetime = None,
-        mode: ATCF_Mode = None,
-        hurricane_model: HurricaneModel = HurricaneModel.GAHM
+        hurricane_model: Union[str, HurricaneModel] = 'gahm'
     ):
 
-        self._model = hurricane_model
+        self.model = hurricane_model
 
         VortexTrack.__init__(
             self,
             storm=storm,
             start_date=start_date,
             end_date=end_date,
             file_deck='b',
             advisories=['BEST'],
         )
 
-
     def __str__(self):
         """Returns string used in param.nml"""
         return f"{self.dtype.value}"
 
-
     @classmethod
     def from_nhc_bdeck(
         cls,
         nhc_bdeck: PathLike,
         start_date: datetime = None,
         end_date: datetime = None,
     ) -> 'NWS':
@@ -110,16 +105,25 @@
 
     @property
     def model(self) -> HurricaneModel:
         """Return hurricane model used for this best track forcing"""
         return self._model
 
     @model.setter
-    def model(self, value: HurricaneModel):
-        if value not in list(HurricaneModel):
+    def model(self, value: Union[str, HurricaneModel]):
+        """Set hurricane model used for this best track forcing"""
+        if isinstance(value, str):
+            if value.upper() not in HurricaneModel.__members__:
+                raise ValueError(f"Invalid hurricane model specified: {value}, choose from: {HurricaneModel.__members__}")
+            value = HurricaneModel[value.upper()]
+        elif isinstance(value, int):
+            value = HurricaneModel(value)
+        elif isinstance(value, HurricaneModel):
+            pass
+        else:
             raise ValueError(f"Invalid hurricane model specified: {value}")
         self._model = value
 
     def clip_to_bbox(self, bbox, bbox_crs):
         msg = f'bbox must be a {Bbox} instance.'
         assert isinstance(bbox, Bbox), msg
         bbox_pol = Polygon(
```

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/nws2/era5.py` & `pyschism-0.1.7/pyschism/forcing/nws/nws2/era5.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/nws2/gfs.py` & `pyschism-0.1.7/pyschism/forcing/nws/nws2/gfs.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/nws2/gfs2.py` & `pyschism-0.1.7/pyschism/forcing/nws/nws2/gfs2.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/nws2/hrrr.py` & `pyschism-0.1.7/pyschism/forcing/nws/nws2/hrrr.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/nws2/hrrr2.py` & `pyschism-0.1.7/pyschism/forcing/nws/nws2/hrrr2.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/nws2/hrrr3.py` & `pyschism-0.1.7/pyschism/forcing/nws/nws2/hrrr3.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/nws2/nws2.py` & `pyschism-0.1.7/pyschism/forcing/nws/nws2/nws2.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/nws2/sflux.py` & `pyschism-0.1.7/pyschism/forcing/nws/nws2/sflux.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/nws2/sflux_inputs.txt` & `pyschism-0.1.7/pyschism/forcing/nws/nws2/sflux_inputs.txt`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/nws/tcprof.py` & `pyschism-0.1.7/pyschism/forcing/nws/tcprof.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/source_sink/base.py` & `pyschism-0.1.7/pyschism/forcing/source_sink/base.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/forcing/source_sink/nwm.py` & `pyschism-0.1.7/pyschism/forcing/source_sink/nwm.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/hotstart.py` & `pyschism-0.1.7/pyschism/hotstart.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/makefile.py` & `pyschism-0.1.7/pyschism/makefile.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/mesh/base.py` & `pyschism-0.1.7/pyschism/mesh/base.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/mesh/boundaries.py` & `pyschism-0.1.7/pyschism/mesh/boundaries.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/mesh/fgrid.py` & `pyschism-0.1.7/pyschism/mesh/fgrid.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/mesh/gridgr3.py` & `pyschism-0.1.7/pyschism/mesh/gridgr3.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/mesh/hgrid.py` & `pyschism-0.1.7/pyschism/mesh/hgrid.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/mesh/parsers/grd.py` & `pyschism-0.1.7/pyschism/mesh/parsers/grd.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/mesh/parsers/sms2dm.py` & `pyschism-0.1.7/pyschism/mesh/parsers/sms2dm.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/mesh/prop.py` & `pyschism-0.1.7/pyschism/mesh/prop.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/mesh/vgrid.py` & `pyschism-0.1.7/pyschism/mesh/vgrid.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/outputs/combine.py` & `pyschism-0.1.7/pyschism/outputs/combine.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/outputs/outputs.py` & `pyschism-0.1.7/pyschism/outputs/outputs.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/outputs/plot.py` & `pyschism-0.1.7/pyschism/outputs/plot.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/outputs/stations.py` & `pyschism-0.1.7/pyschism/outputs/stations.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/param/core.py` & `pyschism-0.1.7/pyschism/param/core.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/param/opt.py` & `pyschism-0.1.7/pyschism/param/opt.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/param/param.py` & `pyschism-0.1.7/pyschism/param/param.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/param/schism_init.py` & `pyschism-0.1.7/pyschism/param/schism_init.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/param/schout.py` & `pyschism-0.1.7/pyschism/param/schout.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/server/base.py` & `pyschism-0.1.7/pyschism/server/base.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/server/slurm.py` & `pyschism-0.1.7/pyschism/server/slurm.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/stations.py` & `pyschism-0.1.7/pyschism/stations.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/utils/coops.py` & `pyschism-0.1.7/pyschism/utils/coops.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism/utils/timedeltatype.py` & `pyschism-0.1.7/pyschism/utils/timedeltatype.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/pyschism.egg-info/PKG-INFO` & `pyschism-0.1.7/pyschism.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschism
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for working with SCHISM input and output files.
 Home-page: https://github.com/schism-dev/pyschism.git
 Author: "SCHISM development group"
 Author-email: jreniel@gmail.com, lcui@vims.edu
 License: "Apache 2.0"
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
```

### Comparing `pyschism-0.1.6/pyschism.egg-info/SOURCES.txt` & `pyschism-0.1.7/pyschism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/setup.py` & `pyschism-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,39 +98,39 @@
                     'netcdf-flattener>=1.2.0'],
     include_package_data=True,
     extras_require={'dev': ['coverage', 'flake8', 'nose']},
     cmdclass={
         "build_schism": BuildSchism
     },
     install_requires=[
-        'pygeos',
+        'boto3',
+        'cdsapi',
+        'cf-python',
+        'cfgrib',
+        'f90nml',
+        'fsspec',
         'geopandas',
-        'netcdf-flattener>=1.2.0',
+        'metpy',
         'netCDF4',
-        'f90nml',
+        'netcdf-flattener>=1.2.0',
+        'numba',
+        'ordered-set',
         'psutil',
-        'scipy',
-        'wget',
-        'cf-python',
-        'metpy',
-        'sqlalchemy',
+        'pygeos',
         'pyugrid',
-        'boto3',
         'rtree',
-        'numba',
+        'scipy',
+        'seawater',
+        'sqlalchemy',
+        'stormevents',
         'tqdm',
         'tqdm-logging-wrapper',
-        'xmltodict',
-        'cdsapi',
-        'seawater',
+        'utm',
+        'wget',
         'xarray',
-        'cfgrib',
+        'xmltodict',
         'zarr',
-        'fsspec',
-        'stormevents',
-        'utm',
-        # 'dask_geopandas @ git+git://github.com/geopandas/dask-geopandas.git@master',
     ],
     entry_points={'console_scripts': ['pyschism = pyschism.__main__:main']},
     tests_require=['nose'],
     test_suite='nose.collector',
 )
```

### Comparing `pyschism-0.1.6/tests/_mesh/test_base.py` & `pyschism-0.1.7/tests/_mesh/test_base.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/_mesh/test_fgrid.py` & `pyschism-0.1.7/tests/_mesh/test_fgrid.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/_mesh/test_grd.py` & `pyschism-0.1.7/tests/_mesh/test_grd.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/_mesh/test_hgrid.py` & `pyschism-0.1.7/tests/_mesh/test_hgrid.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/_mesh/test_mesh.py` & `pyschism-0.1.7/tests/_mesh/test_mesh.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/_mesh/test_sms2dm.py` & `pyschism-0.1.7/tests/_mesh/test_sms2dm.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/_mesh/test_vgrid.py` & `pyschism-0.1.7/tests/_mesh/test_vgrid.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/sciclone/Gulf_Stream_develop/forecast-cli-2D/Makefile` & `pyschism-0.1.7/tests/sciclone/Gulf_Stream_develop/forecast-cli-2D/Makefile`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/sciclone/ICOGS3D/Florence2018/NWM/main.py` & `pyschism-0.1.7/tests/sciclone/ICOGS3D/Florence2018/NWM/main.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/test_barotropic.py` & `pyschism-0.1.7/tests/test_barotropic.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/test_bctides.py` & `pyschism-0.1.7/tests/test_bctides.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/test_icogs.py` & `pyschism-0.1.7/tests/test_icogs.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/test_nwm.py` & `pyschism-0.1.7/tests/test_nwm.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/test_outputs_api.py` & `pyschism-0.1.7/tests/test_outputs_api.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/test_outputs_api_2.py` & `pyschism-0.1.7/tests/test_outputs_api_2.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/test_paramwind.py` & `pyschism-0.1.7/tests/test_paramwind.py`

 * *Files identical despite different names*

### Comparing `pyschism-0.1.6/tests/tropycal.ipynb` & `pyschism-0.1.7/tests/tropycal.ipynb`

 * *Files identical despite different names*

