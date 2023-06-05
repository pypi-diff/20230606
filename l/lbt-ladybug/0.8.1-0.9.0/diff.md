# Comparing `tmp/lbt-ladybug-0.8.1.tar.gz` & `tmp/lbt-ladybug-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbt-ladybug-0.8.1.tar", last modified: Wed Dec 11 21:54:11 2019, max compression
+gzip compressed data, was "dist/lbt-ladybug-0.9.0.tar", last modified: Thu Dec 19 21:05:30 2019, max compression
```

## Comparing `lbt-ladybug-0.8.1.tar` & `lbt-ladybug-0.9.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/Dockerfile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/.github/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1937 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/.github/FUNDING.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1734 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/.github/project-manager.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/docs/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/docs/_templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3668 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/docs/_templates/layout.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/docs/_build/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/docs/_build/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/docs/_build/docs/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/docs/_build/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/docs/_build/.nojekyll
--rw-rw-r--   0 travis    (2000) travis    (2000)      415 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/docs/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     6828 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      462 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/docs/modules.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/docs/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)      899 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/docs/_static/custom.css
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/ladybug/
--rw-rw-r--   0 travis    (2000) travis    (2000)    31377 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/stat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8825 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/graphic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4846 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/header.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20600 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/color.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31490 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/sunpath.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40050 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/wea.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/ladybug/datatype/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/energyintensity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2459 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/volumeflowrate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/fraction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3540 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/generic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2095 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/pressure.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3630 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/thermalcondition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1776 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/massflowrate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/power.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2238 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/temperature.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3002 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/volume.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1616 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/temperaturedelta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2113 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/temperaturetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2933 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/energy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2871 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/distance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2923 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/energyflux.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/angle.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/mass.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2849 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/area.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12876 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/uvalue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2267 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/specificenergy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      900 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1783 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/speed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1621 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/rvalue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1370 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/luminance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1498 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datatype/illuminance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55534 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/skymodel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17083 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/analysisperiod.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36578 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/legend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7282 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/location.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9688 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/futil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28930 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/_datacollectionbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69751 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/epw.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60309 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/designday.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      708 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15883 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/dt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3776 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datacollectionimmutable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63333 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/datacollection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17220 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/psychrometrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3817 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/ladybug/rootfind.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/.releaserc.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2483 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)    35142 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)      217 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/dev-requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1021 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/deploy.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6064 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/graphic_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10247 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/psychrometrics_test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/tests/fixtures/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/tests/fixtures/wea/
--rw-rw-r--   0 travis    (2000) travis    (2000)   899288 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/fixtures/wea/san_francisco_10min.wea
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/tests/fixtures/epw/
--rw-rw-r--   0 travis    (2000) travis    (2000)  1639985 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/fixtures/epw/chicago.epw
--rw-rw-r--   0 travis    (2000) travis    (2000)  2199246 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/fixtures/epw/tokyo.epw
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/tests/fixtures/stat/
--rw-rw-r--   0 travis    (2000) travis    (2000)    39499 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/fixtures/stat/tokyo.stat
--rw-rw-r--   0 travis    (2000) travis    (2000)    34989 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/fixtures/stat/santamonica.stat
--rw-rw-r--   0 travis    (2000) travis    (2000)    39961 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/fixtures/stat/chicago.stat
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/tests/fixtures/ddy/
--rw-rw-r--   0 travis    (2000) travis    (2000)    28793 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/fixtures/ddy/chicago.ddy
--rw-rw-r--   0 travis    (2000) travis    (2000)    28268 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/fixtures/ddy/tokyo.ddy
--rw-rw-r--   0 travis    (2000) travis    (2000)    44276 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/fixtures/ddy/chicago_edited.ddy
--rw-rw-r--   0 travis    (2000) travis    (2000)    29215 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/fixtures/ddy/chicago_monthly.ddy
--rw-rw-r--   0 travis    (2000) travis    (2000)     5120 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/analysisperiod_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5865 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/designday_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5442 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/color_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2085 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/sunpath_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16024 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/legend_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28305 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/datatype_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4266 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/location_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48935 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/datacollection_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1571 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/futil_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8922 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/datacollectionimmutable_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3107 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/skymodel_test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/tests/zip/
--rw-rw-r--   0 travis    (2000) travis    (2000)   239656 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/zip/test.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)    14849 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/epw_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5360 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/dt_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6075 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/stat_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11420 2019-12-11 21:53:26.000000 lbt-ladybug-0.8.1/tests/wea_test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/lbt_ladybug.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/lbt_ladybug.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/lbt_ladybug.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/lbt_ladybug.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2585 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/lbt_ladybug.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2019-12-11 21:54:11.000000 lbt-ladybug-0.8.1/lbt_ladybug.egg-info/requires.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      151 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/Dockerfile
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/.github/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1937 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/.github/FUNDING.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1734 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/.github/project-manager.yml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/docs/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/docs/_templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3668 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/docs/_templates/layout.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/docs/_build/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/docs/_build/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/docs/_build/docs/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/docs/_build/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/docs/_build/.nojekyll
+-rw-rw-r--   0 travis    (2000) travis    (2000)      415 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/docs/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6828 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      462 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       58 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/docs/modules.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/docs/_static/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      899 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/docs/_static/custom.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/ladybug/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31377 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/stat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8825 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/graphic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4846 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/header.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20600 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/color.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31490 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/sunpath.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40050 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/wea.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/ladybug/datatype/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/energyintensity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2459 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/volumeflowrate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/fraction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3540 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/generic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2095 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/pressure.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3630 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/thermalcondition.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1776 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/massflowrate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/power.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2238 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/temperature.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3002 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/volume.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1616 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/temperaturedelta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2113 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/temperaturetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2933 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/energy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2871 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/distance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2923 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/energyflux.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/angle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/mass.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2849 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/area.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12876 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/uvalue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2267 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/specificenergy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      900 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1783 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/speed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1621 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/rvalue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1370 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/luminance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1498 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datatype/illuminance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55534 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/skymodel.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17083 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/analysisperiod.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36578 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/legend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7282 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/location.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11377 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/futil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28930 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/_datacollectionbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69751 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/epw.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60309 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/designday.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      708 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15883 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/dt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3776 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datacollectionimmutable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63333 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/datacollection.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17220 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/psychrometrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3817 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/ladybug/rootfind.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/.releaserc.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2483 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      214 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tox.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/CONTRIBUTING.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35142 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/.coveragerc
+-rw-rw-r--   0 travis    (2000) travis    (2000)      217 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/dev-requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1021 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/deploy.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6064 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/graphic_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10247 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/psychrometrics_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/tests/fixtures/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/tests/fixtures/wea/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   899288 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/fixtures/wea/san_francisco_10min.wea
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/tests/fixtures/epw/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1639985 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/fixtures/epw/chicago.epw
+-rw-rw-r--   0 travis    (2000) travis    (2000)  2199246 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/fixtures/epw/tokyo.epw
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/tests/fixtures/stat/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39499 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/fixtures/stat/tokyo.stat
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34989 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/fixtures/stat/santamonica.stat
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39961 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/fixtures/stat/chicago.stat
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/tests/fixtures/ddy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28793 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/fixtures/ddy/chicago.ddy
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28268 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/fixtures/ddy/tokyo.ddy
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44276 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/fixtures/ddy/chicago_edited.ddy
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29215 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/fixtures/ddy/chicago_monthly.ddy
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5120 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/analysisperiod_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5865 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/designday_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5442 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/color_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2085 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/sunpath_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16024 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/legend_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28305 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/datatype_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4266 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/location_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48935 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/datacollection_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1571 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/futil_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8922 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/datacollectionimmutable_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3107 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/skymodel_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/tests/zip/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   239656 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/zip/test.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14849 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/epw_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5360 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/dt_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6075 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/stat_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11420 2019-12-19 21:04:53.000000 lbt-ladybug-0.9.0/tests/wea_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/lbt_ladybug.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3584 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/lbt_ladybug.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/lbt_ladybug.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/lbt_ladybug.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2585 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/lbt_ladybug.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2019-12-19 21:05:30.000000 lbt-ladybug-0.9.0/lbt_ladybug.egg-info/requires.txt
```

### Comparing `lbt-ladybug-0.8.1/.github/ISSUE_TEMPLATE.md` & `lbt-ladybug-0.9.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/.github/project-manager.yml` & `lbt-ladybug-0.9.0/.github/project-manager.yml`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/docs/_templates/layout.html` & `lbt-ladybug-0.9.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/docs/conf.py` & `lbt-ladybug-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/docs/_static/custom.css` & `lbt-ladybug-0.9.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/PKG-INFO` & `lbt-ladybug-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-ladybug
-Version: 0.8.1
+Version: 0.9.0
 Summary: Ladybug is a Python library to load, analyze and modify EneregyPlus Weather files (epw).
 Home-page: https://github.com/ladybug-tools/ladybug
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: 
         ![Ladybug](http://www.ladybug.tools/assets/img/ladybug.png)
```

### Comparing `lbt-ladybug-0.8.1/ladybug/stat.py` & `lbt-ladybug-0.9.0/ladybug/stat.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/graphic.py` & `lbt-ladybug-0.9.0/ladybug/graphic.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/header.py` & `lbt-ladybug-0.9.0/ladybug/header.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/color.py` & `lbt-ladybug-0.9.0/ladybug/color.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/sunpath.py` & `lbt-ladybug-0.9.0/ladybug/sunpath.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/wea.py` & `lbt-ladybug-0.9.0/ladybug/wea.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/energyintensity.py` & `lbt-ladybug-0.9.0/ladybug/datatype/energyintensity.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/volumeflowrate.py` & `lbt-ladybug-0.9.0/ladybug/datatype/volumeflowrate.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/fraction.py` & `lbt-ladybug-0.9.0/ladybug/datatype/fraction.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/generic.py` & `lbt-ladybug-0.9.0/ladybug/datatype/generic.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/pressure.py` & `lbt-ladybug-0.9.0/ladybug/datatype/pressure.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/thermalcondition.py` & `lbt-ladybug-0.9.0/ladybug/datatype/thermalcondition.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/massflowrate.py` & `lbt-ladybug-0.9.0/ladybug/datatype/massflowrate.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/power.py` & `lbt-ladybug-0.9.0/ladybug/datatype/power.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/temperature.py` & `lbt-ladybug-0.9.0/ladybug/datatype/temperature.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/volume.py` & `lbt-ladybug-0.9.0/ladybug/datatype/volume.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/temperaturedelta.py` & `lbt-ladybug-0.9.0/ladybug/datatype/temperaturedelta.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/temperaturetime.py` & `lbt-ladybug-0.9.0/ladybug/datatype/temperaturetime.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/energy.py` & `lbt-ladybug-0.9.0/ladybug/datatype/energy.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/distance.py` & `lbt-ladybug-0.9.0/ladybug/datatype/distance.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/energyflux.py` & `lbt-ladybug-0.9.0/ladybug/datatype/energyflux.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/angle.py` & `lbt-ladybug-0.9.0/ladybug/datatype/angle.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/mass.py` & `lbt-ladybug-0.9.0/ladybug/datatype/mass.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/area.py` & `lbt-ladybug-0.9.0/ladybug/datatype/area.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/base.py` & `lbt-ladybug-0.9.0/ladybug/datatype/base.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/uvalue.py` & `lbt-ladybug-0.9.0/ladybug/datatype/uvalue.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/specificenergy.py` & `lbt-ladybug-0.9.0/ladybug/datatype/specificenergy.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/__init__.py` & `lbt-ladybug-0.9.0/ladybug/datatype/__init__.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/speed.py` & `lbt-ladybug-0.9.0/ladybug/datatype/speed.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/rvalue.py` & `lbt-ladybug-0.9.0/ladybug/datatype/rvalue.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/luminance.py` & `lbt-ladybug-0.9.0/ladybug/datatype/luminance.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datatype/illuminance.py` & `lbt-ladybug-0.9.0/ladybug/datatype/illuminance.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/skymodel.py` & `lbt-ladybug-0.9.0/ladybug/skymodel.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/analysisperiod.py` & `lbt-ladybug-0.9.0/ladybug/analysisperiod.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/legend.py` & `lbt-ladybug-0.9.0/ladybug/legend.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/location.py` & `lbt-ladybug-0.9.0/ladybug/location.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/futil.py` & `lbt-ladybug-0.9.0/ladybug/futil.py`

 * *Files 14% similar despite different names*

```diff
@@ -163,14 +163,55 @@
             print('Copying %s to %s' % (os.path.split(f)[-1],
                                         os.path.normpath(target_folder)))
             shutil.copy(f, target)
 
     return [os.path.join(target_folder, os.path.split(f)[-1]) for f in files]
 
 
+def copy_file_tree(source_folder, dest_folder, overwrite=True):
+    """Copy an entire file tree from a source_folder to a dest_folder.
+
+    Args:
+        source_folder: The source folder containing the files and folders to
+            be copied.
+        dest_folder: The destination folder into which all the files and folders
+            of the source_folder will be copied.
+        overwrite: Boolean to note whether an existing folder with the same
+            name as the source_folder in the dest_folder directory should be
+            overwritten. Default: True.
+    """
+    # make the dest_folder if it does not exist
+    if not os.path.isdir(dest_folder):
+        os.mkdir(dest_folder)
+
+    # recursively copy each sub-folder and file
+    for f in os.listdir(source_folder):
+        # get the source and destination file paths
+        src_file_path = os.path.join(source_folder, f)
+        dst_file_path = os.path.join(dest_folder, f)
+
+        # if overwrite is True, delete any existing files
+        if overwrite:
+            if os.path.isfile(dst_file_path):
+                try:
+                    os.remove(dst_file_path)
+                except Exception:
+                    raise IOError("Failed to remove %s" % f)
+            elif os.path.isdir(dst_file_path):
+                nukedir(dst_file_path, True)
+
+        # copy the files and folders to their correct location
+        if os.path.isfile(src_file_path):
+            shutil.copyfile(src_file_path, dst_file_path)
+        elif os.path.isdir(src_file_path):
+            if not os.path.isdir(dst_file_path):
+                os.mkdir(dst_file_path)
+            copy_file_tree(src_file_path, dst_file_path, overwrite)
+
+
 def _download_py2(link, path, __hdr__):
     """Download a file from a link in Python 2."""
     try:
         req = urllib2.Request(link, headers=__hdr__)
         u = urllib2.urlopen(req)
     except Exception as e:
         raise Exception(' Download failed with the error:\n{}'.format(e))
```

### Comparing `lbt-ladybug-0.8.1/ladybug/_datacollectionbase.py` & `lbt-ladybug-0.9.0/ladybug/_datacollectionbase.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/epw.py` & `lbt-ladybug-0.9.0/ladybug/epw.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/designday.py` & `lbt-ladybug-0.9.0/ladybug/designday.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/__init__.py` & `lbt-ladybug-0.9.0/ladybug/__init__.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/dt.py` & `lbt-ladybug-0.9.0/ladybug/dt.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datacollectionimmutable.py` & `lbt-ladybug-0.9.0/ladybug/datacollectionimmutable.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/datacollection.py` & `lbt-ladybug-0.9.0/ladybug/datacollection.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/psychrometrics.py` & `lbt-ladybug-0.9.0/ladybug/psychrometrics.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/ladybug/rootfind.py` & `lbt-ladybug-0.9.0/ladybug/rootfind.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/README.md` & `lbt-ladybug-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/.travis.yml` & `lbt-ladybug-0.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/LICENSE` & `lbt-ladybug-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/setup.py` & `lbt-ladybug-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/graphic_test.py` & `lbt-ladybug-0.9.0/tests/graphic_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/psychrometrics_test.py` & `lbt-ladybug-0.9.0/tests/psychrometrics_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/fixtures/wea/san_francisco_10min.wea` & `lbt-ladybug-0.9.0/tests/fixtures/wea/san_francisco_10min.wea`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/fixtures/epw/chicago.epw` & `lbt-ladybug-0.9.0/tests/fixtures/epw/chicago.epw`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/fixtures/epw/tokyo.epw` & `lbt-ladybug-0.9.0/tests/fixtures/epw/tokyo.epw`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/fixtures/stat/tokyo.stat` & `lbt-ladybug-0.9.0/tests/fixtures/stat/tokyo.stat`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/fixtures/stat/santamonica.stat` & `lbt-ladybug-0.9.0/tests/fixtures/stat/santamonica.stat`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/fixtures/stat/chicago.stat` & `lbt-ladybug-0.9.0/tests/fixtures/stat/chicago.stat`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/fixtures/ddy/chicago.ddy` & `lbt-ladybug-0.9.0/tests/fixtures/ddy/chicago.ddy`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/fixtures/ddy/tokyo.ddy` & `lbt-ladybug-0.9.0/tests/fixtures/ddy/tokyo.ddy`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/fixtures/ddy/chicago_edited.ddy` & `lbt-ladybug-0.9.0/tests/fixtures/ddy/chicago_edited.ddy`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/fixtures/ddy/chicago_monthly.ddy` & `lbt-ladybug-0.9.0/tests/fixtures/ddy/chicago_monthly.ddy`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/analysisperiod_test.py` & `lbt-ladybug-0.9.0/tests/analysisperiod_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/designday_test.py` & `lbt-ladybug-0.9.0/tests/designday_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/color_test.py` & `lbt-ladybug-0.9.0/tests/color_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/sunpath_test.py` & `lbt-ladybug-0.9.0/tests/sunpath_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/legend_test.py` & `lbt-ladybug-0.9.0/tests/legend_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/datatype_test.py` & `lbt-ladybug-0.9.0/tests/datatype_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/location_test.py` & `lbt-ladybug-0.9.0/tests/location_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/datacollection_test.py` & `lbt-ladybug-0.9.0/tests/datacollection_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/futil_test.py` & `lbt-ladybug-0.9.0/tests/futil_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/datacollectionimmutable_test.py` & `lbt-ladybug-0.9.0/tests/datacollectionimmutable_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/skymodel_test.py` & `lbt-ladybug-0.9.0/tests/skymodel_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/zip/test.zip` & `lbt-ladybug-0.9.0/tests/zip/test.zip`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/epw_test.py` & `lbt-ladybug-0.9.0/tests/epw_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/dt_test.py` & `lbt-ladybug-0.9.0/tests/dt_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/stat_test.py` & `lbt-ladybug-0.9.0/tests/stat_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/tests/wea_test.py` & `lbt-ladybug-0.9.0/tests/wea_test.py`

 * *Files identical despite different names*

### Comparing `lbt-ladybug-0.8.1/lbt_ladybug.egg-info/PKG-INFO` & `lbt-ladybug-0.9.0/lbt_ladybug.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-ladybug
-Version: 0.8.1
+Version: 0.9.0
 Summary: Ladybug is a Python library to load, analyze and modify EneregyPlus Weather files (epw).
 Home-page: https://github.com/ladybug-tools/ladybug
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: 
         ![Ladybug](http://www.ladybug.tools/assets/img/ladybug.png)
```

### Comparing `lbt-ladybug-0.8.1/lbt_ladybug.egg-info/SOURCES.txt` & `lbt-ladybug-0.9.0/lbt_ladybug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

