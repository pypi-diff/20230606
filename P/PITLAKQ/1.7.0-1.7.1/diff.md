# Comparing `tmp/pitlakq-1.7.0.tar.gz` & `tmp/pitlakq-1.7.1.tar.gz`

## Comparing `pitlakq-1.7.0.tar` & `pitlakq-1.7.1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/__init__.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/__init__.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/datastructures/__init__.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/datastructures/dicts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/dbftools/__init__.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/dbftools/flatdbf/__init__.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/dbftools/flatdbf/flatdbf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/dbftools/pcg/__init__.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/dbftools/pcg/pcgdatabase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/dirs/__init__.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/dirs/splitall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/filereader/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/filereader/fobj.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/filereader/read_columns_txt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/input/__init__.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/input/bathhelper.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/input/recursiveupdate.py
--rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/input/resources.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/input/xlsx_reader.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/input/yamlinput.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/output/__init__.py
--rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/output/ncoutput.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/timing/__init__.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/commontools/timing/timetools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/balance/__init__.py
--rw-r--r--   0        0        0    10412 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/balance/balance.py
--rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/balance/specie_balance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/configuration/__init__.py
--rw-r--r--   0        0        0    14001 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/configuration/configuration.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/configuration/getconfig.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/configuration/initialize.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/configuration/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/running/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/running/db.py
--rw-r--r--   0        0        0    25038 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/running/gw_lake_exchange.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/running/importhelper.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/running/introspection.py
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/running/pitlakq_scripter.py
--rw-r--r--   0        0        0    22889 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/running/run_pitlakq.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/metamodel/running/runlab.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/modflow/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/modmst/__init__.py
--rw-r--r--   0        0        0    15927 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/modmst/modmst.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/pcg/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/__init__.py
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/kb_calculation.py
--rw-r--r--   0        0        0    26621 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc.py
--rw-r--r--   0        0        0    19299 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_io.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_pyro_server.py
--rw-r--r--   0        0        0    11086 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_runner.py
--rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_thread.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/run_pyro_servers.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/tempenv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/__init__.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/balance.py
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/geometryupdater.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/jday_converter.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/pointers.py
--rw-r--r--   0        0        0    37755 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/w2.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/w2_proxy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/numericalmodels/newmodels/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/__init__.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/bath_viz.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/date_at_level.py
--rw-r--r--   0        0        0    24732 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/depth_time_contour.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/error_statistics.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/ice_table.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/kb_balance.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/level_volume_relation.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/relative_time.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/show_bath.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/show_volume_area_curve.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/postprocessing/waterlevel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/__init__.py
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/charge_loading.py
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/charge_tributaries.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/check_kb_balance.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/create_bathgrid.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/create_project.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/create_xlsx_input.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/inflow_step_graph.py
--rw-r--r--   0        0        0    11937 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/input_converter.py
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/make_pathnames.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/obswells.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/preprocess.py
--rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/preprocessor.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/surfer_volume.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/preprocessing/vol_area_check.py
--rw-r--r--   0        0        0  8440860 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/co2sat.nc
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/const_names.txt
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/converter.ini
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/kinetics.txt
--rw-r--r--   0        0        0   790862 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/llnl_w2.dat
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/mineral_names.txt
--rwxr-xr-x   0        0        0   971720 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/phreeqc2linux
--rwxr-xr-x   0        0        0   894572 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/phreeqc2mac
--rw-r--r--   0        0        0   483413 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/phreeqc2win.exe
--rw-r--r--   0        0        0    49285 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/phreeqc_w2.dat
--rw-r--r--   0        0        0   791012 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/phreeqc_w2_Dec27.dat
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/resources/rates.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/erosion/__init__.py
--rw-r--r--   0        0        0    21212 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/erosion/erosion.py
--rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/erosion/polygon_gridding.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/erosion/surfergrid.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/gw/__init__.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/gw/activecells.py
--rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/gw/gwh.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/gw/precalc_gw.py
--rw-r--r--   0        0        0    21624 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/gw/precalc_gw_in_out.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/lake/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/lake/co2sat.py
--rw-r--r--   0        0        0    33076 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/lake/lake.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/loading/__init__.py
--rw-r--r--   0        0        0    14779 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/loading/loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/sediment/__init__.py
--rw-r--r--   0        0        0    14207 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/sediment/leaching.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/treatment/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/treatment/substance_addition/__init__.py
--rw-r--r--   0        0        0    11154 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/submodels/treatment/substance_addition/addition.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/.pitlakq_sample
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/activeconst.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/branch_inflow.txt
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/branch_inflow_concentration.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/branch_inflow_temperature.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/branch_outflow.txt
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/leaching.yaml
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/meteorology.txt
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/pitlakq.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/precipitation.txt
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/precipitation_concentration.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/precipitation_temperature.txt
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/preprocessing.yaml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/tributary_concentration.txt
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/tributary_inflow.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/tributary_temperature.txt
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/w2.yaml
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pitlakq/templates/w2const.yaml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pitlakq-1.7.0/.gitignore
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pitlakq-1.7.0/.hgignore
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 pitlakq-1.7.0/README.md
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 pitlakq-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 pitlakq-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/__init__.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/__init__.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/datastructures/__init__.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/datastructures/dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/dbftools/__init__.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/dbftools/flatdbf/__init__.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/dbftools/flatdbf/flatdbf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/dbftools/pcg/__init__.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/dbftools/pcg/pcgdatabase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/dirs/__init__.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/dirs/splitall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/filereader/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/filereader/fobj.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/filereader/read_columns_txt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/input/__init__.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/input/bathhelper.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/input/recursiveupdate.py
+-rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/input/resources.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/input/xlsx_reader.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/input/yamlinput.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/output/__init__.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/output/ncoutput.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/timing/__init__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/commontools/timing/timetools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/balance/__init__.py
+-rw-r--r--   0        0        0    10412 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/balance/balance.py
+-rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/balance/specie_balance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/configuration/__init__.py
+-rw-r--r--   0        0        0    14001 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/configuration/configuration.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/configuration/getconfig.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/configuration/initialize.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/configuration/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/running/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/running/db.py
+-rw-r--r--   0        0        0    25038 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/running/gw_lake_exchange.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/running/importhelper.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/running/introspection.py
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/running/pitlakq_scripter.py
+-rw-r--r--   0        0        0    22889 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/running/run_pitlakq.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/metamodel/running/runlab.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/modflow/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/modmst/__init__.py
+-rw-r--r--   0        0        0    15927 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/modmst/modmst.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/pcg/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/__init__.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/kb_calculation.py
+-rw-r--r--   0        0        0    26621 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc.py
+-rw-r--r--   0        0        0    19299 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_io.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_pyro_server.py
+-rw-r--r--   0        0        0    11086 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_runner.py
+-rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_thread.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/run_pyro_servers.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/tempenv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/__init__.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/balance.py
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/geometryupdater.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/jday_converter.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/pointers.py
+-rw-r--r--   0        0        0    37755 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/w2.py
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/w2_proxy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/numericalmodels/newmodels/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/__init__.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/bath_viz.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/date_at_level.py
+-rw-r--r--   0        0        0    24732 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/depth_time_contour.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/error_statistics.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/ice_table.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/kb_balance.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/level_volume_relation.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/relative_time.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/show_bath.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/show_volume_area_curve.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/postprocessing/waterlevel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/__init__.py
+-rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/charge_loading.py
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/charge_tributaries.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/check_kb_balance.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/create_bathgrid.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/create_project.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/create_xlsx_input.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/inflow_step_graph.py
+-rw-r--r--   0        0        0    11937 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/input_converter.py
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/make_pathnames.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/obswells.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/preprocess.py
+-rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/preprocessor.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/surfer_volume.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/preprocessing/vol_area_check.py
+-rw-r--r--   0        0        0  8440860 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/co2sat.nc
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/const_names.txt
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/converter.ini
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/kinetics.txt
+-rw-r--r--   0        0        0   790862 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/llnl_w2.dat
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/mineral_names.txt
+-rwxr-xr-x   0        0        0   971720 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/phreeqc2linux
+-rwxr-xr-x   0        0        0   894572 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/phreeqc2mac
+-rw-r--r--   0        0        0   483413 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/phreeqc2win.exe
+-rw-r--r--   0        0        0    49285 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/phreeqc_w2.dat
+-rw-r--r--   0        0        0   791012 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/phreeqc_w2_Dec27.dat
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/resources/rates.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/erosion/__init__.py
+-rw-r--r--   0        0        0    21212 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/erosion/erosion.py
+-rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/erosion/polygon_gridding.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/erosion/surfergrid.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/gw/__init__.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/gw/activecells.py
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/gw/gwh.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/gw/precalc_gw.py
+-rw-r--r--   0        0        0    21624 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/gw/precalc_gw_in_out.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/lake/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/lake/co2sat.py
+-rw-r--r--   0        0        0    33076 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/lake/lake.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/loading/__init__.py
+-rw-r--r--   0        0        0    14779 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/loading/loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/sediment/__init__.py
+-rw-r--r--   0        0        0    14207 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/sediment/leaching.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/treatment/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/treatment/substance_addition/__init__.py
+-rw-r--r--   0        0        0    11154 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/submodels/treatment/substance_addition/addition.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/.pitlakq_sample
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/activeconst.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/branch_inflow.txt
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/branch_inflow_concentration.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/branch_inflow_temperature.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/branch_outflow.txt
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/leaching.yaml
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/meteorology.txt
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/pitlakq.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/precipitation.txt
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/precipitation_concentration.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/precipitation_temperature.txt
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/preprocessing.yaml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/tributary_concentration.txt
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/tributary_inflow.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/tributary_temperature.txt
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/w2.yaml
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pitlakq/templates/w2const.yaml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pitlakq-1.7.1/.gitignore
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pitlakq-1.7.1/.hgignore
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 pitlakq-1.7.1/README.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pitlakq-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pitlakq-1.7.1/PKG-INFO
```

### Comparing `pitlakq-1.7.0/pitlakq/commontools/tools.py` & `pitlakq-1.7.1/pitlakq/commontools/tools.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/datastructures/dicts.py` & `pitlakq-1.7.1/pitlakq/commontools/datastructures/dicts.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/dbftools/flatdbf/flatdbf.py` & `pitlakq-1.7.1/pitlakq/commontools/dbftools/flatdbf/flatdbf.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/dbftools/pcg/pcgdatabase.py` & `pitlakq-1.7.1/pitlakq/commontools/dbftools/pcg/pcgdatabase.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/dirs/splitall.py` & `pitlakq-1.7.1/pitlakq/commontools/dirs/splitall.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/filereader/fobj.py` & `pitlakq-1.7.1/pitlakq/commontools/filereader/fobj.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/filereader/read_columns_txt.py` & `pitlakq-1.7.1/pitlakq/commontools/filereader/read_columns_txt.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/input/bathhelper.py` & `pitlakq-1.7.1/pitlakq/commontools/input/bathhelper.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/input/recursiveupdate.py` & `pitlakq-1.7.1/pitlakq/commontools/input/recursiveupdate.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/input/resources.py` & `pitlakq-1.7.1/pitlakq/commontools/input/resources.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/input/xlsx_reader.py` & `pitlakq-1.7.1/pitlakq/commontools/input/xlsx_reader.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/input/yamlinput.py` & `pitlakq-1.7.1/pitlakq/commontools/input/yamlinput.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/commontools/output/ncoutput.py` & `pitlakq-1.7.1/pitlakq/commontools/output/ncoutput.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/balance/balance.py` & `pitlakq-1.7.1/pitlakq/metamodel/balance/balance.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/balance/specie_balance.py` & `pitlakq-1.7.1/pitlakq/metamodel/balance/specie_balance.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/configuration/configuration.py` & `pitlakq-1.7.1/pitlakq/metamodel/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/configuration/getconfig.py` & `pitlakq-1.7.1/pitlakq/metamodel/configuration/getconfig.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/configuration/initialize.py` & `pitlakq-1.7.1/pitlakq/metamodel/configuration/initialize.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/configuration/version.py` & `pitlakq-1.7.1/pitlakq/metamodel/configuration/version.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/running/db.py` & `pitlakq-1.7.1/pitlakq/metamodel/running/db.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/running/gw_lake_exchange.py` & `pitlakq-1.7.1/pitlakq/metamodel/running/gw_lake_exchange.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/running/introspection.py` & `pitlakq-1.7.1/pitlakq/metamodel/running/introspection.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/running/pitlakq_scripter.py` & `pitlakq-1.7.1/pitlakq/metamodel/running/pitlakq_scripter.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/running/run_pitlakq.py` & `pitlakq-1.7.1/pitlakq/metamodel/running/run_pitlakq.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/metamodel/running/runlab.py` & `pitlakq-1.7.1/pitlakq/metamodel/running/runlab.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/modmst/modmst.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/modmst/modmst.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/kb_calculation.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/kb_calculation.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_io.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_io.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_pyro_server.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_pyro_server.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_runner.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_runner.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_thread.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/phreeqc_thread.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/phreeqc/tempenv.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/phreeqc/tempenv.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/balance.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/balance.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/geometryupdater.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/geometryupdater.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/jday_converter.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/jday_converter.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/pointers.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/pointers.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/w2.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/w2.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/numericalmodels/existingmodels/w2/w2_proxy.py` & `pitlakq-1.7.1/pitlakq/numericalmodels/existingmodels/w2/w2_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 Wrapper class for W2 extension module.
 
 This a proxy and can be either started as a seperated
 process communicating with pyro with the main program
 or be imported as a normal module.
 """
-from __future__ import print_function
-
 import os
 
 # NumPy, dynamic members.
 # pylint: disable-msg=E1101
 
 import numpy
 from Pyro4 import core
 
+from libpitlakq import w2_fortran
+
 from . import pointers
-from . import w2_fortran
 
 
 DUMMY_W2_CODE_NAME = 'dummy'
 
 
 class W2Proxy(object):
     """Proxy for W2.
```

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/bath_viz.py` & `pitlakq-1.7.1/pitlakq/postprocessing/bath_viz.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/date_at_level.py` & `pitlakq-1.7.1/pitlakq/postprocessing/date_at_level.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/depth_time_contour.py` & `pitlakq-1.7.1/pitlakq/postprocessing/depth_time_contour.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/error_statistics.py` & `pitlakq-1.7.1/pitlakq/postprocessing/error_statistics.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/ice_table.py` & `pitlakq-1.7.1/pitlakq/postprocessing/ice_table.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/kb_balance.py` & `pitlakq-1.7.1/pitlakq/postprocessing/kb_balance.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/level_volume_relation.py` & `pitlakq-1.7.1/pitlakq/postprocessing/level_volume_relation.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/relative_time.py` & `pitlakq-1.7.1/pitlakq/postprocessing/relative_time.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/show_bath.py` & `pitlakq-1.7.1/pitlakq/postprocessing/show_bath.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/show_volume_area_curve.py` & `pitlakq-1.7.1/pitlakq/postprocessing/show_volume_area_curve.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/postprocessing/waterlevel.py` & `pitlakq-1.7.1/pitlakq/postprocessing/waterlevel.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/charge_loading.py` & `pitlakq-1.7.1/pitlakq/preprocessing/charge_loading.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/charge_tributaries.py` & `pitlakq-1.7.1/pitlakq/preprocessing/charge_tributaries.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/check_kb_balance.py` & `pitlakq-1.7.1/pitlakq/preprocessing/check_kb_balance.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/create_bathgrid.py` & `pitlakq-1.7.1/pitlakq/preprocessing/create_bathgrid.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/create_project.py` & `pitlakq-1.7.1/pitlakq/preprocessing/create_project.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/create_xlsx_input.py` & `pitlakq-1.7.1/pitlakq/preprocessing/create_xlsx_input.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/inflow_step_graph.py` & `pitlakq-1.7.1/pitlakq/preprocessing/inflow_step_graph.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/input_converter.py` & `pitlakq-1.7.1/pitlakq/preprocessing/input_converter.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/make_pathnames.py` & `pitlakq-1.7.1/pitlakq/preprocessing/make_pathnames.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/obswells.py` & `pitlakq-1.7.1/pitlakq/preprocessing/obswells.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/preprocess.py` & `pitlakq-1.7.1/pitlakq/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/preprocessor.py` & `pitlakq-1.7.1/pitlakq/preprocessing/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/surfer_volume.py` & `pitlakq-1.7.1/pitlakq/preprocessing/surfer_volume.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/preprocessing/vol_area_check.py` & `pitlakq-1.7.1/pitlakq/preprocessing/vol_area_check.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/co2sat.nc` & `pitlakq-1.7.1/pitlakq/resources/co2sat.nc`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/const_names.txt` & `pitlakq-1.7.1/pitlakq/resources/const_names.txt`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/converter.ini` & `pitlakq-1.7.1/pitlakq/resources/converter.ini`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/kinetics.txt` & `pitlakq-1.7.1/pitlakq/resources/kinetics.txt`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/llnl_w2.dat` & `pitlakq-1.7.1/pitlakq/resources/llnl_w2.dat`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/phreeqc2linux` & `pitlakq-1.7.1/pitlakq/resources/phreeqc2linux`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/phreeqc2mac` & `pitlakq-1.7.1/pitlakq/resources/phreeqc2mac`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/phreeqc2win.exe` & `pitlakq-1.7.1/pitlakq/resources/phreeqc2win.exe`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/phreeqc_w2.dat` & `pitlakq-1.7.1/pitlakq/resources/phreeqc_w2.dat`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/phreeqc_w2_Dec27.dat` & `pitlakq-1.7.1/pitlakq/resources/phreeqc_w2_Dec27.dat`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/resources/rates.txt` & `pitlakq-1.7.1/pitlakq/resources/rates.txt`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/erosion/erosion.py` & `pitlakq-1.7.1/pitlakq/submodels/erosion/erosion.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/erosion/polygon_gridding.py` & `pitlakq-1.7.1/pitlakq/submodels/erosion/polygon_gridding.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/erosion/surfergrid.py` & `pitlakq-1.7.1/pitlakq/submodels/erosion/surfergrid.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/gw/activecells.py` & `pitlakq-1.7.1/pitlakq/submodels/gw/activecells.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/gw/gwh.py` & `pitlakq-1.7.1/pitlakq/submodels/gw/gwh.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/gw/precalc_gw.py` & `pitlakq-1.7.1/pitlakq/submodels/gw/precalc_gw.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/gw/precalc_gw_in_out.py` & `pitlakq-1.7.1/pitlakq/submodels/gw/precalc_gw_in_out.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/lake/co2sat.py` & `pitlakq-1.7.1/pitlakq/submodels/lake/co2sat.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/lake/lake.py` & `pitlakq-1.7.1/pitlakq/submodels/lake/lake.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/loading/loading.py` & `pitlakq-1.7.1/pitlakq/submodels/loading/loading.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/sediment/leaching.py` & `pitlakq-1.7.1/pitlakq/submodels/sediment/leaching.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/submodels/treatment/substance_addition/addition.py` & `pitlakq-1.7.1/pitlakq/submodels/treatment/substance_addition/addition.py`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/templates/activeconst.txt` & `pitlakq-1.7.1/pitlakq/templates/activeconst.txt`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/templates/leaching.yaml` & `pitlakq-1.7.1/pitlakq/templates/leaching.yaml`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/templates/pitlakq.yaml` & `pitlakq-1.7.1/pitlakq/templates/pitlakq.yaml`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/templates/precipitation_concentration.txt` & `pitlakq-1.7.1/pitlakq/templates/precipitation_concentration.txt`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/templates/w2.yaml` & `pitlakq-1.7.1/pitlakq/templates/w2.yaml`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pitlakq/templates/w2const.yaml` & `pitlakq-1.7.1/pitlakq/templates/w2const.yaml`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/.hgignore` & `pitlakq-1.7.1/.hgignore`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/README.md` & `pitlakq-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pitlakq-1.7.0/pyproject.toml` & `pitlakq-1.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "PITLAKQ"
-version = "1.7.0"
+version = "1.7.1"
 authors = [
   { name="Mike Müller", email="mmueller@hydrocomputing.com" },
 ]
 description = "The Pit Lake Hydrodynamic and Water Quality Model"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -32,15 +32,14 @@
     "jupyterlab",
     "numpy",
     "matplotlib",
     "netcdf4",
     "openpyxl",
     "pandas",
     "pyro4",
-    "python",
     "pywin32; sys_platform == 'win32'",
     "pyyaml",
     "scipy",
     "xlsxwriter",
     "zodb",
 ]
```

### Comparing `pitlakq-1.7.0/PKG-INFO` & `pitlakq-1.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PITLAKQ
-Version: 1.7.0
+Version: 1.7.1
 Summary: The Pit Lake Hydrodynamic and Water Quality Model
 Project-URL: Homepage, http://www.pitlakq.com
 Project-URL: Documentation, https://github.com/pypa/sampleproject/issues
 Author-email: Mike Müller <mmueller@hydrocomputing.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,14 @@
 Requires-Dist: libpitlakq
 Requires-Dist: matplotlib
 Requires-Dist: netcdf4
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: pyro4
-Requires-Dist: python
 Requires-Dist: pywin32; sys_platform == 'win32'
 Requires-Dist: pyyaml
 Requires-Dist: scipy
 Requires-Dist: xlsxwriter
 Requires-Dist: zodb
 Description-Content-Type: text/markdown
```

