# Comparing `tmp/crillab-metrics-1.2.6.tar.gz` & `tmp/crillab_metrics-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crillab-metrics-1.2.6.tar", last modified: Fri Sep  2 16:53:53 2022, max compression
+gzip compressed data, was "crillab_metrics-1.3.0.tar", last modified: Tue Jun  6 12:21:25 2023, max compression
```

## Comparing `crillab-metrics-1.2.6.tar` & `crillab_metrics-1.3.0.tar`

### file list

```diff
@@ -1,63 +1,94 @@
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.602532 crillab-metrics-1.2.6/
--rw-rw-r--   0 falque    (1000) falque    (1000)     7598 2022-03-31 08:16:09.000000 crillab-metrics-1.2.6/LICENSE.md
--rw-rw-r--   0 falque    (1000) falque    (1000)     4277 2022-09-02 16:53:53.602532 crillab-metrics-1.2.6/PKG-INFO
--rw-rw-r--   0 falque    (1000) falque    (1000)     3623 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/README.md
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/bin/
--rwxrwxr-x   0 falque    (1000) falque    (1000)    11144 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/bin/metrics
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/crillab_metrics.egg-info/
--rw-rw-r--   0 falque    (1000) falque    (1000)     4277 2022-09-02 16:53:53.000000 crillab-metrics-1.2.6/crillab_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 falque    (1000) falque    (1000)     1489 2022-09-02 16:53:53.000000 crillab-metrics-1.2.6/crillab_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 falque    (1000) falque    (1000)        1 2022-09-02 16:53:53.000000 crillab-metrics-1.2.6/crillab_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 falque    (1000) falque    (1000)        1 2022-09-02 16:53:53.000000 crillab-metrics-1.2.6/crillab_metrics.egg-info/not-zip-safe
--rw-rw-r--   0 falque    (1000) falque    (1000)      145 2022-09-02 16:53:53.000000 crillab-metrics-1.2.6/crillab_metrics.egg-info/requires.txt
--rw-rw-r--   0 falque    (1000) falque    (1000)        8 2022-09-02 16:53:53.000000 crillab-metrics-1.2.6/crillab_metrics.egg-info/top_level.txt
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/metrics/
--rw-rw-r--   0 falque    (1000) falque    (1000)     2253 2022-09-02 16:50:17.000000 crillab-metrics-1.2.6/metrics/__init__.py
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/metrics/core/
--rw-rw-r--   0 falque    (1000) falque    (1000)     1921 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/core/__init__.py
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/metrics/core/builder/
--rw-rw-r--   0 falque    (1000) falque    (1000)     1978 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/core/builder/__init__.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    11741 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/core/builder/attribute_manager.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    15009 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/core/builder/builder.py
--rw-rw-r--   0 falque    (1000) falque    (1000)     4632 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/core/builder/typing_strategy.py
--rw-rw-r--   0 falque    (1000) falque    (1000)     3690 2022-06-24 14:56:08.000000 crillab-metrics-1.2.6/metrics/core/constants.py
--rw-rw-r--   0 falque    (1000) falque    (1000)     6044 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/core/model.py
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/metrics/scalpel/
--rw-rw-r--   0 falque    (1000) falque    (1000)     5938 2022-06-24 11:49:10.000000 crillab-metrics-1.2.6/metrics/scalpel/__init__.py
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/metrics/scalpel/config/
--rw-rw-r--   0 falque    (1000) falque    (1000)     3818 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/scalpel/config/__init__.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    22870 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/scalpel/config/config.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    12315 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/scalpel/config/configsaver.py
--rw-rw-r--   0 falque    (1000) falque    (1000)     4470 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/scalpel/config/datafile.py
--rw-rw-r--   0 falque    (1000) falque    (1000)     6386 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/scalpel/config/format.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    11647 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/scalpel/config/inputset.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    38302 2022-06-24 11:49:10.000000 crillab-metrics-1.2.6/metrics/scalpel/config/wrapper.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    21401 2022-06-24 11:49:10.000000 crillab-metrics-1.2.6/metrics/scalpel/listener.py
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/metrics/scalpel/parser/
--rw-rw-r--   0 falque    (1000) falque    (1000)     4761 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/scalpel/parser/__init__.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    27033 2022-06-24 11:49:10.000000 crillab-metrics-1.2.6/metrics/scalpel/parser/campaign.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    12171 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/scalpel/parser/output.py
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/metrics/scalpel/utils/
--rw-rw-r--   0 falque    (1000) falque    (1000)     2501 2022-06-24 11:49:10.000000 crillab-metrics-1.2.6/metrics/scalpel/utils/__init__.py
--rw-rw-r--   0 falque    (1000) falque    (1000)     7345 2022-06-24 11:49:10.000000 crillab-metrics-1.2.6/metrics/scalpel/utils/csvutils.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    14650 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/scalpel/utils/filters.py
--rw-rw-r--   0 falque    (1000) falque    (1000)     3628 2022-06-24 11:49:10.000000 crillab-metrics-1.2.6/metrics/scalpel/utils/logging.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    16230 2022-06-24 11:49:10.000000 crillab-metrics-1.2.6/metrics/scalpel/utils/pattern.py
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/metrics/studio/
--rw-rw-r--   0 falque    (1000) falque    (1000)     2173 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/studio/__init__.py
--rw-rw-r--   0 falque    (1000) falque    (1000)     6805 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/studio/report.py
--rw-rw-r--   0 falque    (1000) falque    (1000)     8057 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/studio/scalpelcli.py
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.598532 crillab-metrics-1.2.6/metrics/templates/
--rw-rw-r--   0 falque    (1000) falque    (1000)     1043 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/templates/README.md
--rw-rw-r--   0 falque    (1000) falque    (1000)       92 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/templates/gitignore
--rw-rw-r--   0 falque    (1000) falque    (1000)    12791 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/templates/load_experiments.ipynb
--rw-rw-r--   0 falque    (1000) falque    (1000)     9899 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/templates/optim_analysis.ipynb
--rw-rw-r--   0 falque    (1000) falque    (1000)       24 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/templates/requirements.txt
--rw-rw-r--   0 falque    (1000) falque    (1000)    12548 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/templates/runtime_analysis.ipynb
--rw-rw-r--   0 falque    (1000) falque    (1000)      752 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/templates/scalpel_config.yml
-drwxrwxr-x   0 falque    (1000) falque    (1000)        0 2022-09-02 16:53:53.602532 crillab-metrics-1.2.6/metrics/wallet/
--rw-rw-r--   0 falque    (1000) falque    (1000)     2356 2022-03-31 08:16:10.000000 crillab-metrics-1.2.6/metrics/wallet/__init__.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    47675 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/wallet/analysis.py
--rw-rw-r--   0 falque    (1000) falque    (1000)    10319 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/metrics/wallet/plot.py
--rw-rw-r--   0 falque    (1000) falque    (1000)       38 2022-09-02 16:53:53.602532 crillab-metrics-1.2.6/setup.cfg
--rw-rw-r--   0 falque    (1000) falque    (1000)     3734 2022-09-02 16:35:54.000000 crillab-metrics-1.2.6/setup.py
+-rw-r--r--   0        0        0     7598 2022-03-31 08:16:09.966226 crillab_metrics-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     3623 2022-09-02 16:35:54.822506 crillab_metrics-1.3.0/README.md
+-rw-r--r--   0        0        0     2253 2022-09-02 16:50:17.098527 crillab_metrics-1.3.0/metrics/__init__.py
+-rw-r--r--   0        0        0     1921 2022-03-31 08:16:10.194226 crillab_metrics-1.3.0/metrics/core/__init__.py
+-rw-r--r--   0        0        0     1978 2022-03-31 08:16:10.194226 crillab_metrics-1.3.0/metrics/core/builder/__init__.py
+-rw-r--r--   0        0        0    11741 2022-03-31 08:16:10.194226 crillab_metrics-1.3.0/metrics/core/builder/attribute_manager.py
+-rw-r--r--   0        0        0    15009 2022-09-02 16:35:54.826506 crillab_metrics-1.3.0/metrics/core/builder/builder.py
+-rw-r--r--   0        0        0     4632 2022-03-31 08:16:10.194226 crillab_metrics-1.3.0/metrics/core/builder/typing_strategy.py
+-rw-r--r--   0        0        0     3690 2022-06-24 14:56:08.394292 crillab_metrics-1.3.0/metrics/core/constants.py
+-rw-r--r--   0        0        0     6044 2022-03-31 08:16:10.194226 crillab_metrics-1.3.0/metrics/core/model.py
+-rw-r--r--   0        0        0     5938 2022-06-24 11:49:10.742014 crillab_metrics-1.3.0/metrics/scalpel/__init__.py
+-rw-r--r--   0        0        0     3818 2022-03-31 08:16:10.194226 crillab_metrics-1.3.0/metrics/scalpel/config/__init__.py
+-rw-r--r--   0        0        0    22870 2022-09-02 16:35:54.826506 crillab_metrics-1.3.0/metrics/scalpel/config/config.py
+-rw-r--r--   0        0        0    12315 2022-09-02 16:35:54.826506 crillab_metrics-1.3.0/metrics/scalpel/config/configsaver.py
+-rw-r--r--   0        0        0     4470 2022-03-31 08:16:10.194226 crillab_metrics-1.3.0/metrics/scalpel/config/datafile.py
+-rw-r--r--   0        0        0     6386 2022-09-02 16:35:54.826506 crillab_metrics-1.3.0/metrics/scalpel/config/format.py
+-rw-r--r--   0        0        0    11647 2022-03-31 08:16:10.194226 crillab_metrics-1.3.0/metrics/scalpel/config/inputset.py
+-rw-r--r--   0        0        0    38302 2022-06-24 11:49:10.742014 crillab_metrics-1.3.0/metrics/scalpel/config/wrapper.py
+-rw-r--r--   0        0        0    21401 2022-06-24 11:49:10.742014 crillab_metrics-1.3.0/metrics/scalpel/listener.py
+-rw-r--r--   0        0        0     4761 2022-03-31 08:16:10.194226 crillab_metrics-1.3.0/metrics/scalpel/parser/__init__.py
+-rw-r--r--   0        0        0    27033 2022-06-24 11:49:10.742014 crillab_metrics-1.3.0/metrics/scalpel/parser/campaign.py
+-rw-r--r--   0        0        0    12457 2023-06-02 13:34:46.058896 crillab_metrics-1.3.0/metrics/scalpel/parser/output.py
+-rw-r--r--   0        0        0     2501 2022-06-24 11:49:10.742014 crillab_metrics-1.3.0/metrics/scalpel/utils/__init__.py
+-rw-r--r--   0        0        0     7345 2022-06-24 11:49:10.742014 crillab_metrics-1.3.0/metrics/scalpel/utils/csvutils.py
+-rw-r--r--   0        0        0    14650 2022-03-31 08:16:10.194226 crillab_metrics-1.3.0/metrics/scalpel/utils/filters.py
+-rw-r--r--   0        0        0     3628 2022-06-24 11:49:10.742014 crillab_metrics-1.3.0/metrics/scalpel/utils/logging.py
+-rw-r--r--   0        0        0    16230 2022-06-24 11:49:10.742014 crillab_metrics-1.3.0/metrics/scalpel/utils/pattern.py
+-rw-r--r--   0        0        0     2173 2022-09-02 16:35:54.826506 crillab_metrics-1.3.0/metrics/studio/__init__.py
+-rw-r--r--   0        0        0     7211 2023-06-05 08:04:28.907429 crillab_metrics-1.3.0/metrics/studio/report.py
+-rw-r--r--   0        0        0     8057 2022-09-02 16:35:54.826506 crillab_metrics-1.3.0/metrics/studio/scalpelcli.py
+-rw-r--r--   0        0        0     1043 2022-09-02 16:35:54.826506 crillab_metrics-1.3.0/metrics/templates/README.md
+-rw-r--r--   0        0        0       92 2022-09-02 16:35:54.826506 crillab_metrics-1.3.0/metrics/templates/gitignore
+-rw-r--r--   0        0        0     9243 2023-06-05 08:04:28.907429 crillab_metrics-1.3.0/metrics/templates/load_experiments.ipynb
+-rw-r--r--   0        0        0    14667 2023-06-05 08:04:28.911429 crillab_metrics-1.3.0/metrics/templates/load_experiments_optim.ipynb
+-rw-r--r--   0        0        0    13429 2023-06-05 08:04:28.911429 crillab_metrics-1.3.0/metrics/templates/load_experiments_sat.ipynb
+-rw-r--r--   0        0        0     9916 2023-06-05 08:04:28.911429 crillab_metrics-1.3.0/metrics/templates/optim_analysis.ipynb
+-rw-r--r--   0        0        0       24 2022-09-02 16:35:54.826506 crillab_metrics-1.3.0/metrics/templates/requirements.txt
+-rw-r--r--   0        0        0    15761 2023-06-05 08:04:28.911429 crillab_metrics-1.3.0/metrics/templates/runtime_analysis.ipynb
+-rw-r--r--   0        0        0      752 2022-09-02 16:35:54.826506 crillab_metrics-1.3.0/metrics/templates/scalpel_config.yml
+-rw-r--r--   0        0        0     2397 2023-06-05 09:05:58.259046 crillab_metrics-1.3.0/metrics/wallet/__init__.py
+-rw-r--r--   0        0        0    52683 2023-06-05 09:26:09.724554 crillab_metrics-1.3.0/metrics/wallet/analysis.py
+-rw-r--r--   0        0        0    10301 2023-06-02 14:47:48.204146 crillab_metrics-1.3.0/metrics/wallet/plot.py
+-rw-r--r--   0        0        0     1049 2023-06-06 12:21:25.358993 crillab_metrics-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      853 2022-09-02 16:35:54.830505 crillab_metrics-1.3.0/tests/data/issue38/campaign/config/metrics_scalpel.yml
+-rw-r--r--   0        0        0        0 2022-09-02 16:35:54.830505 crillab_metrics-1.3.0/tests/data/issue38/campaign/experiments/.gitkeep
+-rw-r--r--   0        0        0    66825 2022-09-02 16:35:54.830505 crillab_metrics-1.3.0/tests/data/issue38/campaign/experiments/WDegCAxCD/home_cril_wattez_XCSP18_Auction_Auction_cnt_Auction_cnt_decay100_c18.xml.lzma/execution.out
+-rw-r--r--   0        0        0        0 2022-09-02 16:35:54.830505 crillab_metrics-1.3.0/tests/data/issue38/campaign/experiments/WDegCAxCD/home_cril_wattez_XCSP18_Auction_Auction_cnt_Auction_cnt_decay100_c18.xml.lzma/output/stderr
+-rw-r--r--   0        0        0   321473 2022-09-02 16:35:54.830505 crillab_metrics-1.3.0/tests/data/issue38/campaign/experiments/WDegCAxCD/home_cril_wattez_XCSP18_Auction_Auction_cnt_Auction_cnt_decay100_c18.xml.lzma/output/stdout
+-rw-r--r--   0        0        0      503 2022-09-02 16:35:54.830505 crillab_metrics-1.3.0/tests/data/issue38/campaign/experiments/WDegCAxCD/home_cril_wattez_XCSP18_Auction_Auction_cnt_Auction_cnt_decay100_c18.xml.lzma/statistics.out
+-rw-r--r--   0        0        0      563 2022-09-02 16:35:54.830505 crillab_metrics-1.3.0/tests/data/multi-csv-with-custom-separator-and-no-header/input/config.yml
+-rw-r--r--   0        0        0    35662 2022-09-02 16:35:54.830505 crillab_metrics-1.3.0/tests/data/multi-csv-with-custom-separator-and-no-header/input/data/glu.txt
+-rw-r--r--   0        0        0    35114 2022-09-02 16:35:54.830505 crillab_metrics-1.3.0/tests/data/multi-csv-with-custom-separator-and-no-header/input/data/kissat.txt
+-rw-r--r--   0        0        0  2635617 2022-09-02 16:35:54.838505 crillab_metrics-1.3.0/tests/data/sat-competition/2019/input/sat2019.csv
+-rw-r--r--   0        0        0    15223 2022-09-02 16:35:54.838505 crillab_metrics-1.3.0/tests/data/sat-competition/2019/input/sat2019.input
+-rw-r--r--   0        0        0      291 2022-09-02 16:35:54.838505 crillab_metrics-1.3.0/tests/data/sat-competition/2019/input/sat2019.yml
+-rw-r--r--   0        0        0    36784 2022-09-02 16:35:54.838505 crillab_metrics-1.3.0/tests/data/sat-competition/2019/output/box.pdf
+-rw-r--r--   0        0        0   107211 2022-09-02 16:35:54.838505 crillab_metrics-1.3.0/tests/data/sat-competition/2019/output/cactus.pdf
+-rw-r--r--   0        0        0    35523 2022-09-02 16:35:54.838505 crillab_metrics-1.3.0/tests/data/sat-competition/2019/output/cactus_zoom.pdf
+-rw-r--r--   0        0        0    77655 2022-09-02 16:35:54.838505 crillab_metrics-1.3.0/tests/data/sat-competition/2019/output/cdf.pdf
+-rw-r--r--   0        0        0     6428 2022-09-02 16:35:54.838505 crillab_metrics-1.3.0/tests/data/sat-competition/2019/output/contribution_table.tex
+-rw-r--r--   0        0        0    73959 2022-09-02 16:35:54.842506 crillab_metrics-1.3.0/tests/data/sat-competition/2019/output/scatter.pdf
+-rw-r--r--   0        0        0    71872 2022-09-02 16:35:54.842506 crillab_metrics-1.3.0/tests/data/sat-competition/2019/output/scatter_zoom.pdf
+-rw-r--r--   0        0        0     7688 2022-09-02 16:35:54.842506 crillab_metrics-1.3.0/tests/data/sat-competition/2019/output/stats_table.tex
+-rw-r--r--   0        0        0  5935236 2022-09-02 16:35:54.854505 crillab_metrics-1.3.0/tests/data/sat-competition/2020/results.csv
+-rw-r--r--   0        0        0     2361 2022-09-02 16:35:54.854505 crillab_metrics-1.3.0/tests/data/sat-competition/input/config.yml
+-rw-r--r--   0        0        0  2635617 2022-09-02 16:35:54.862506 crillab_metrics-1.3.0/tests/data/sat-competition/input/data/sat2019.csv
+-rw-r--r--   0        0        0    15223 2022-09-02 16:35:54.862506 crillab_metrics-1.3.0/tests/data/sat-competition/input/data/sat2019.input
+-rw-r--r--   0        0        0  3517742 2022-09-02 16:35:54.866505 crillab_metrics-1.3.0/tests/data/xcsp17.json
+-rw-r--r--   0        0        0       29 2022-09-02 16:35:54.866505 crillab_metrics-1.3.0/tests/data/xcsp19/full_analysis/.gitignore
+-rw-r--r--   0        0        0  2794101 2022-09-02 16:35:54.874505 crillab_metrics-1.3.0/tests/data/xcsp19/full_analysis/analysis.csv
+-rw-r--r--   0        0        0      393 2022-09-02 16:35:54.874505 crillab_metrics-1.3.0/tests/data/xcsp19/full_analysis/config/metrics_scalpel.yml
+-rw-r--r--   0        0        0      425 2022-09-02 16:35:54.874505 crillab_metrics-1.3.0/tests/data/xcsp19/full_analysis/config/metrics_scalpel_full_paths.yml
+-rw-r--r--   0        0        0  3028046 2022-09-02 16:35:54.882506 crillab_metrics-1.3.0/tests/data/xcsp19/full_analysis/input/XCSP19.txt
+-rw-r--r--   0        0        0        0 2022-09-02 16:35:54.882506 crillab_metrics-1.3.0/tests/data/xcsp19/full_analysis/output/.gitkeep
+-rw-r--r--   0        0        0       29 2022-09-02 16:35:54.882506 crillab_metrics-1.3.0/tests/data/xcsp19/problematic_analysis/.gitignore
+-rw-r--r--   0        0        0  1300732 2022-09-02 16:35:54.886505 crillab_metrics-1.3.0/tests/data/xcsp19/problematic_analysis/analysis.bin
+-rw-r--r--   0        0        0  1446397 2022-09-02 16:35:54.886505 crillab_metrics-1.3.0/tests/data/xcsp19/problematic_analysis/analysis.csv
+-rw-r--r--   0        0        0      393 2022-09-02 16:35:54.886505 crillab_metrics-1.3.0/tests/data/xcsp19/problematic_analysis/config/metrics_scalpel.yml
+-rw-r--r--   0        0        0      432 2022-09-02 16:35:54.886505 crillab_metrics-1.3.0/tests/data/xcsp19/problematic_analysis/config/metrics_scalpel_full_paths.yml
+-rw-r--r--   0        0        0  1825439 2022-09-02 16:35:54.890505 crillab_metrics-1.3.0/tests/data/xcsp19/problematic_analysis/input/XCSP19.txt
+-rw-r--r--   0        0        0     2230 2022-03-31 08:16:10.198226 crillab_metrics-1.3.0/tests/test_core/json_reader.py
+-rw-r--r--   0        0        0     4199 2022-03-31 08:16:10.198226 crillab_metrics-1.3.0/tests/test_core/test_campaign.py
+-rw-r--r--   0        0        0     1824 2022-09-02 16:35:54.890505 crillab_metrics-1.3.0/tests/test_core/test_global.py
+-rw-r--r--   0        0        0     1961 2022-03-31 08:16:10.198226 crillab_metrics-1.3.0/tests/test_core/test_typing.py
+-rw-r--r--   0        0        0     1280 2022-09-02 16:35:54.890505 crillab_metrics-1.3.0/tests/test_scalpel/test_config.py
+-rw-r--r--   0        0        0    12412 2022-03-31 08:16:10.198226 crillab_metrics-1.3.0/tests/test_scalpel/test_filters.py
+-rw-r--r--   0        0        0     2308 2022-03-31 08:16:10.198226 crillab_metrics-1.3.0/tests/test_scalpel/test_listener.py
+-rw-r--r--   0        0        0      575 2022-09-02 16:35:54.890505 crillab_metrics-1.3.0/tests/test_scalpel/test_output.py
+-rw-r--r--   0        0        0    11060 2022-03-31 08:16:10.198226 crillab_metrics-1.3.0/tests/test_scalpel/test_pattern.py
+-rw-r--r--   0        0        0     4606 2022-09-02 16:35:54.890505 crillab_metrics-1.3.0/tests/test_wallet/test_normal_analysis_manipulations.py
+-rw-r--r--   0        0        0     9106 2022-09-02 16:35:54.890505 crillab_metrics-1.3.0/tests/test_wallet/test_normal_analysis_static_plots.py
+-rw-r--r--   0        0        0     2414 2022-09-02 16:35:54.890505 crillab_metrics-1.3.0/tests/test_wallet/test_normal_analysis_tables.py
+-rw-r--r--   0        0        0     1353 2022-09-02 16:35:54.890505 crillab_metrics-1.3.0/tests/test_wallet/test_problematic_analysis.py
+-rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 crillab_metrics-1.3.0/PKG-INFO
```

### Comparing `crillab-metrics-1.2.6/LICENSE.md` & `crillab_metrics-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/PKG-INFO` & `crillab_metrics-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.1
 Name: crillab-metrics
-Version: 1.2.6
+Version: 1.3.0
 Summary: rEproducible sofTware peRformance analysIs in perfeCt Simplicity
-Home-page: https://github.com/crillab/metrics
+Keywords: reproducible software performance analysis
 Author: Thibault Falque, Romain Wallon, Hugues Wattez
-Author-email: metrics@cril.fr
+Author-Email: Unknown <metrics@cril.fr>
 License: LGPLv3+
-Keywords: reproducible software performance analysis
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Project-URL: Homepage, https://github.com/crillab/metrics
+Requires-Python: >=3.10
+Requires-Dist: InquirerPy
+Requires-Dist: crillab-autograph
+Requires-Dist: dash-bootstrap-components
+Requires-Dist: deprecated
+Requires-Dist: jinja2
+Requires-Dist: jsonpickle
+Requires-Dist: loguru
+Requires-Dist: myst-parser
+Requires-Dist: pandas
+Requires-Dist: pyfiglet
+Requires-Dist: pyparsing
+Requires-Dist: pyyaml
+Requires-Dist: tenacity
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
 
 # mETRICS - rEproducible sofTware peRformance analysIs in perfeCt Simplicity
 
 [![License](https://img.shields.io/pypi/l/crillab-metrics)](LICENSE.md)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/crillab-metrics)
 ![PyPI - Status](https://img.shields.io/pypi/status/crillab-metrics)
 ![Travis (.org)](https://img.shields.io/travis/crillab/metrics)
@@ -91,9 +103,7 @@
 
 + [*Metrics : Mission Expérimentations*.](https://hal.archives-ouvertes.fr/hal-03295285/document)
   Thibault Falque, Romain Wallon and Hugues Wattez.
   16es Journées Francophones de Programmation par Contraintes (JFPC'21), 2021.
 + *Metrics: Towards a Unified Library for Experimenting Solvers*.
   Thibault Falque, Romain Wallon and Hugues Wattez.
   11th International Workshop on Pragmatics of SAT (POS'20), 2020.
-
-
```

### Comparing `crillab-metrics-1.2.6/README.md` & `crillab_metrics-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/__init__.py` & `crillab_metrics-1.3.0/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/core/__init__.py` & `crillab_metrics-1.3.0/metrics/core/__init__.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/core/builder/__init__.py` & `crillab_metrics-1.3.0/metrics/core/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/core/builder/attribute_manager.py` & `crillab_metrics-1.3.0/metrics/core/builder/attribute_manager.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/core/builder/builder.py` & `crillab_metrics-1.3.0/metrics/core/builder/builder.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/core/builder/typing_strategy.py` & `crillab_metrics-1.3.0/metrics/core/builder/typing_strategy.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/core/constants.py` & `crillab_metrics-1.3.0/metrics/core/constants.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/core/model.py` & `crillab_metrics-1.3.0/metrics/core/model.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/__init__.py` & `crillab_metrics-1.3.0/metrics/scalpel/__init__.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/config/__init__.py` & `crillab_metrics-1.3.0/metrics/scalpel/config/__init__.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/config/config.py` & `crillab_metrics-1.3.0/metrics/scalpel/config/config.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/config/configsaver.py` & `crillab_metrics-1.3.0/metrics/scalpel/config/configsaver.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/config/datafile.py` & `crillab_metrics-1.3.0/metrics/scalpel/config/datafile.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/config/format.py` & `crillab_metrics-1.3.0/metrics/scalpel/config/format.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/config/inputset.py` & `crillab_metrics-1.3.0/metrics/scalpel/config/inputset.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/config/wrapper.py` & `crillab_metrics-1.3.0/metrics/scalpel/config/wrapper.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/listener.py` & `crillab_metrics-1.3.0/metrics/scalpel/listener.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/parser/__init__.py` & `crillab_metrics-1.3.0/metrics/scalpel/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/parser/campaign.py` & `crillab_metrics-1.3.0/metrics/scalpel/parser/campaign.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/parser/output.py` & `crillab_metrics-1.3.0/metrics/scalpel/parser/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,22 +26,22 @@
 
 """
 This module provides various classes for parsing different types of files
 containing the output of experiment-wares produced during a campaign, to
 extract the data they contain.
 """
 
-
 from json import load as load_json
 from typing import Any, Optional, TextIO
 from xml.etree.ElementTree import Element, parse as load_xml
 
 from metrics.scalpel import CampaignParserListener
 from metrics.scalpel.config import ScalpelConfiguration
 from metrics.scalpel.utils import CsvConfiguration, CsvReader
+from loguru import logger
 
 
 class CampaignOutputParser:
     """
     The CampaignOutputParser is the parent class for the parsers used to
     read the output files produced by an experiment-ware during an experiment.
     """
@@ -286,16 +286,24 @@
 
     def _internal_parse(self, stream: TextIO) -> None:
         """
         Parses the given stream to extract data about the campaign.
 
         :param stream: The stream to read.
         """
-        for line in stream:
-            self._parse_line(line.rstrip())
+        iter_lines = iter(stream)
+        while True:
+            try:
+                line = next(iter_lines)
+                self._parse_line(line.rstrip())
+            except StopIteration:
+                break
+            except Exception as e:
+                logger.warning(f'{self._file_path}: {e}')
+                continue
 
     def _parse_line(self, line: str) -> None:
         """
         Parses the given line to extract data about the campaign.
 
         :param line: The line to read.
         """
```

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/utils/__init__.py` & `crillab_metrics-1.3.0/metrics/scalpel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/utils/csvutils.py` & `crillab_metrics-1.3.0/metrics/scalpel/utils/csvutils.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/utils/filters.py` & `crillab_metrics-1.3.0/metrics/scalpel/utils/filters.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/utils/logging.py` & `crillab_metrics-1.3.0/metrics/scalpel/utils/logging.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/scalpel/utils/pattern.py` & `crillab_metrics-1.3.0/metrics/scalpel/utils/pattern.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/studio/__init__.py` & `crillab_metrics-1.3.0/metrics/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/studio/report.py` & `crillab_metrics-1.3.0/metrics/studio/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         Creates a new report builder.
 
         :param root_dir: The directory in which to build the report.
         """
         self._root_dir = root_dir
         self._template_vars = {}
         self._env = Environment(loader=PackageLoader('metrics'), autoescape=select_autoescape())
+        self._has_runtime_analysis = False
+        self._has_optim_analysis = False
 
     def create_directories(self) -> None:
         """
         Creates the directories needed for the report.
         """
         if not os.path.exists(self._root_dir):
             os.mkdir(self._root_dir)
@@ -102,32 +104,39 @@
 
     def add_load_experiments(self, notebook_name: str = 'load_experiments') -> None:
         """
         Adds the Jupyter Notebook allowing to load experiment data from the campaign.
 
         :param notebook_name: The name of the notebook to add.
         """
-        self._write_template('load_experiments.ipynb', f'{notebook_name}.ipynb')
+        notebook_source = 'load_experiments.ipynb'
+        if self._has_optim_analysis:
+            notebook_source = 'load_experiments_optim.ipynb'
+        elif self._has_runtime_analysis:
+            notebook_source = 'load_experiments_sat.ipynb'
+        self._write_template(notebook_source, f'{notebook_name}.ipynb')
 
     def add_runtime_analysis(self, notebook_name: str = 'runtime_analysis') -> None:
         """
         Adds the Jupyter Notebook allowing to perform a runtime analysis of the experiment-wares
         run during the campaign.
 
         :param notebook_name: The name of the notebook to add.
         """
+        self._has_runtime_analysis = True
         self._write_template('runtime_analysis.ipynb', f'{notebook_name}.ipynb')
 
     def add_optim_analysis(self, notebook_name: str = 'optim_analysis') -> None:
         """
         Adds the Jupyter Notebook allowing to perform an optimization analysis of the
         experiment-wares run during the campaign.
 
         :param notebook_name: The name of the notebook to add.
         """
+        self._has_optim_analysis = True
         self._write_template('optim_analysis.ipynb', f'{notebook_name}.ipynb')
 
     def _write_template(self, template_name: str, output_file: str) -> None:
         """
         Writes a report file following a template.
 
         :param template_name: The name of the file to use as template.
```

### Comparing `crillab-metrics-1.2.6/metrics/studio/scalpelcli.py` & `crillab_metrics-1.3.0/metrics/studio/scalpelcli.py`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/templates/README.md` & `crillab_metrics-1.3.0/metrics/templates/README.md`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/templates/load_experiments.ipynb` & `crillab_metrics-1.3.0/metrics/templates/load_experiments_sat.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984733566538002%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(0, 'import pandas as pd\\n')], delete: [0]}}, 7: {'source': "*

 * *            "{insert: [(0, '%%time\\n')]}}, 16: {'source': {insert: [(1, '    xp_ware: xp_ware for "*

 * *            "xp_ware in analysis.experiment_wares\\n')], delete: [1]}}, 17: {'source': ['Based on "*

 * *            'the map above, we can easily replace the name of the experiment-wares as '*

 * *            "follows.\\n', 'For convenience, note that we keep a copy of the previous "*

 * *            "experiment-ware names […]*

```diff
@@ -55,15 +55,15 @@
                 },
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "from itertools import product\n",
+                "import pandas as pd\n",
                 "from metrics.wallet import BasicAnalysis"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "pycharm": {
@@ -96,14 +96,15 @@
                 },
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
+                "%%time\n",
                 "analysis = BasicAnalysis(input_file='config/{{ config_file }}.yml', log_level='WARNING')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "pycharm": {
@@ -149,14 +150,34 @@
             "source": [
                 "**TODO: CHECK THAT EVERYTHING IS INDEED OK BEFORE PREPROCESSING THE DATA!**"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "Before making any change to the data, we keep a copy of the analysis in its current state to allow rolling back our changes if needed."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "analysis.export('.cache-original')"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "## More meaningful names for experiment-wares"
             ]
@@ -182,41 +203,45 @@
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
                 "name_map = {\n",
-                "    xp_ware: xp_ware for xp_ware in analysis.experiment_wares()\n",
+                "    xp_ware: xp_ware for xp_ware in analysis.experiment_wares\n",
                 "}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
-                "Based on the map above, we can easily replace the name of the experiment-wares as follows."
+                "Based on the map above, we can easily replace the name of the experiment-wares as follows.\n",
+                "For convenience, note that we keep a copy of the previous experiment-ware names, as they may be easier to handle programmatically."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
                 "analysis = analysis.add_variable(\n",
-                "    new_var='experiment_ware', \n",
+                "    new_var='raw_experiment_ware',\n",
+                "    function=lambda xp: xp['experiment_ware']\n",
+                ").add_variable(\n",
+                "    new_var='experiment_ware',\n",
                 "    function=lambda xp: name_map[xp['experiment_ware']]\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -283,45 +308,67 @@
             "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "During our analysis, we will need to know whether a given experiment was successful.\n",
-                "As an example, we provide below the code to check the success of an optimization solver."
+                "To this end, we will need to have a look to different columns of the analysis, that allow to identify the experiment-ware's answer.\n",
+                "You may need to edit them if you do not have given the same names in your analysis."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "# The decision given by the experiment-ware w.r.t. the satisfiability of the input.\n",
+                "decision = 'decision'"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "The function below will be used to check that the solver terminated with its final decision."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
                 "def is_success(xp):\n",
                 "    \"\"\"\n",
-                "    This function checks that a solver either proved the optimality of its best\n",
-                "    bound within the time limit, or proved the input to be unsatisfiable.\n",
+                "    This function checks that an experiment-ware either found a solution within\n",
+                "    the time limit, or proved the input to be unsatisfiable.\n",
                 "    \"\"\"\n",
-                "    return xp['decision'] == 'OPTIMUM FOUND' or xp['decision'] == 'UNSATISFIABLE'"
+                "    return xp[decision] == 'SATISFIABLE' or xp[decision] == 'UNSATISFIABLE'"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "To make sure that our experiments are consistent, we also need to compare the results obtained by the different experiment-wares.\n",
-                "As an example, we provide below the code to check that if different optimization solvers claim to have found an optimal value, this value must be the same for all solvers."
+                "The function below checks that all solvers agree on the (un)satisfiability of their inputs."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "pycharm": {
@@ -329,38 +376,28 @@
                 },
                 "scrolled": true
             },
             "outputs": [],
             "source": [
                 "def is_consistent_by_input(df_input):\n",
                 "    \"\"\"\n",
-                "    This function checks that the pairwise comparison between two different\n",
-                "    optimal bounds found on the same input is small enough to consider these bounds as consistent.\n",
+                "    This function checks that there is no contradictory answers between the solvers,\n",
+                "    both regarding the answer they give w.r.t. the satisfiability of their input.\n",
                 "    \"\"\"\n",
                 "    # Checking the decision of the solvers.\n",
-                "    decisions = df_input['decision'].unique()\n",
+                "    decisions = df_input[decision].unique()\n",
                 "    if 'OPTIMUM FOUND' in decisions and 'UNSATISFIABLE' in decisions:\n",
                 "        # A solver has found an optimal solution while another proved unsatisfiability.\n",
                 "        return False\n",
                 "    if 'SATISFIABLE' in decisions and 'UNSATISFIABLE' in decisions:\n",
                 "        # A solver has found a solution while another proved unsatisfiability.\n",
                 "        return False\n",
                 "\n",
-                "    # Checking that at most one optimal value exists.\n",
-                "    best_values_for_complete_search = df_input[df_input['success']]['best_bound'].unique()\n",
-                "\n",
-                "    # Checking that there is no better value than the optimal one.\n",
-                "    if df_input['objective'].unique()[0] == 'min':\n",
-                "        best_global_value = df_input['best_bound'].min()\n",
-                "    else:\n",
-                "        best_global_value = df_input['best_bound'].max()\n",
-                "\n",
-                "    return best_global_value is None or \\\n",
-                "           len(best_values_for_complete_search) <= 1 and \\\n",
-                "           best_values_for_complete_search[0] != best_global_value"
+                "    # Otherwise, all solvers agree on the (un)satisfiability of their inputs.\n",
+                "    return True"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false,
                 "pycharm": {
```

### Comparing `crillab-metrics-1.2.6/metrics/templates/optim_analysis.ipynb` & `crillab_metrics-1.3.0/metrics/templates/optim_analysis.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998070987654322%*

 * *Differences: {"'cells'": "{19: {'source': {insert: [(0, '%%time\\n')]}}}"}*

```diff
@@ -267,14 +267,15 @@
                 "pycharm": {
                     "name": "#%%\n"
                 },
                 "scrolled": false
             },
             "outputs": [],
             "source": [
+                "%%time\n",
                 "analysis.compute_scores(default_solver=default_xp_ware, score_map=score_methods)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "02815d19",
             "metadata": {
```

### Comparing `crillab-metrics-1.2.6/metrics/templates/runtime_analysis.ipynb` & `crillab_metrics-1.3.0/metrics/templates/runtime_analysis.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9719765568264342%*

 * *Differences: {"'cells'": '{20: {\'source\': {insert: [(8, "    color_map={ \'VBEW\': \'#000000\' },\\n"), (9, '*

 * *            '"    style_map={ \'VBEW\': LineType.DASH_DOT },\\n"), (11, \'    '*

 * *            'dynamic=False\\n\')], delete: [11, 9, 8]}}, 24: {\'source\': {insert: [(9, "    '*

 * *            'color_map={ \'VBEW\': \'#000000\' },\\n"), (10, "    style_map={ \'VBEW\': '*

 * *            'LineType.DASH_DOT },\\n"), (12, \'    dynamic=False\\n\')], delete: [12, 10, 9]}}, '*

 * *            "27: {'source': {insert: [(6, '    dyn […]*

```diff
@@ -210,14 +210,35 @@
                 "In the first column, we can see for each experiment-ware the number of inputs for which the runtime of the experiment-ware is equal to that of the VBEW.\n",
                 "In the second column (resp. third column), we can see for each experiment-ware the number of inputs for which the experiment-ware is at least 1 second faster (resp. 10 seconds faster) than any other experiment-ware.\n",
                 "Finally, in the fourth column, we can see the number of inputs for which this experiment-ware is the only one to run until completion (and thus, all other experiment-wares reached the time limit on this input)."
             ]
         },
         {
             "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "For a more visual representation of these contributions, we can represent the information provided in the table above with a bar plot.\n",
+                "This plot shows for each solver the number of times the runtime of this solver is equal to that of the VBEW."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "analysis.marginal_contribution()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "091ac4a5",
             "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
@@ -251,18 +272,18 @@
                 "    cactus_col='cpu_time',\n",
                 "    show_marker=False,\n",
                 "\n",
                 "    title='Cactus-plot',\n",
                 "    x_axis_name='Number of solved inputs',\n",
                 "    y_axis_name='Time (s)',\n",
                 "\n",
-                "    color_map={ 'VBS': '#000000' },\n",
-                "    style_map={ 'VBS': LineType.DASH_DOT },\n",
+                "    color_map={ 'VBEW': '#000000' },\n",
+                "    style_map={ 'VBEW': LineType.DASH_DOT },\n",
                 "\n",
-                "    latex_writing=True\n",
+                "    dynamic=False\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "131d6ce1",
             "metadata": {
@@ -316,18 +337,18 @@
                 "    show_marker=False,\n",
                 "    normalized=True,\n",
                 "\n",
                 "    title='CDF',\n",
                 "    x_axis_name='Time (s)',\n",
                 "    y_axis_name='Percentage of solved inputs',\n",
                 "\n",
-                "    color_map={ 'VBS': '#000000' },\n",
-                "    style_map={ 'VBS': LineType.DASH_DOT },\n",
+                "    color_map={ 'VBEW': '#000000' },\n",
+                "    style_map={ 'VBEW': LineType.DASH_DOT },\n",
                 "\n",
-                "    latex_writing=True\n",
+                "    dynamic=False\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "17a03d2e",
             "metadata": {
@@ -366,15 +387,15 @@
             "source": [
                 "analysis.box_plot(\n",
                 "    box_by='experiment_ware',\n",
                 "    box_col='cpu_time',\n",
                 "\n",
                 "    title='Box-plots of the runtime',\n",
                 "\n",
-                "    latex_writing=True\n",
+                "    dynamic=False\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a3ea916a",
             "metadata": {
@@ -384,14 +405,107 @@
             },
             "source": [
                 "**TODO: ADD HERE AN INTERPRETATION FOR THESE BOXPLOTS!**"
             ]
         },
         {
             "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "## Numerical results"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "To get more information about the statistics of our experiments, let us refer to the following table."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "analysis.stat_table(\n",
+                "    commas_for_number=True,\n",
+                "    dollars_for_number=True\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "Let us describe the content of this table, for each considered experiment-ware:\n",
+                "\n",
+                "- The column `count` is the number of inputs solved by the experiment-ware.\n",
+                "- The column `sum` is the time taken by the experiment-ware to run on all inputs (including timeouts).\n",
+                "- The columns `PARx` are equivalent to `sum` but add a penalty of `x` times the timeout to failed experiments (*PAR* stands for *Penalized Average Runtime*).\n",
+                "- The column `common count` is the number of inputs commonly solved by all experiment-wares.\n",
+                "- The column `common sum` is the time taken by the (current) experiment-ware to solve the commonly solved inputs.\n",
+                "- The column `uncommon count` is the number of inputs solved by the experiment-ware without considering common ones (which are considered as *easy*).\n",
+                "- The column `total` is the total number of experiments run with the experiment-ware."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "**TODO: ADD AN INTERPRETATION OF THE RESULTS IN THE TABLE ABOVE.**"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "Let us now consider another table, which provides for each input and for each experiment-ware the information relative to a particular variable in the analysis, for instance the `cpu_time` of the experiment-ware on an input."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "analysis.pivot_table(\n",
+                "    index='input',\n",
+                "    columns='experiment_ware',\n",
+                "    values='cpu_time',\n",
+                "    commas_for_number=True,\n",
+                "    dollars_for_number=True\n",
+                ")#.head()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "**TODO: ADD HERE AN INTERPRETATION OF THE TABLE ABOVE.**"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "1d51f8a1",
             "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
@@ -474,15 +588,15 @@
                 "    x_max={{ timeout }},\n",
                 "    y_min=1,\n",
                 "    y_max={{ timeout }},\n",
                 "\n",
                 "    logx=True,\n",
                 "    logy=True,\n",
                 "\n",
-                "    latex_writing=True\n",
+                "    dynamic=False\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false,
```

### Comparing `crillab-metrics-1.2.6/metrics/templates/scalpel_config.yml` & `crillab_metrics-1.3.0/metrics/templates/scalpel_config.yml`

 * *Files identical despite different names*

### Comparing `crillab-metrics-1.2.6/metrics/wallet/__init__.py` & `crillab_metrics-1.3.0/metrics/wallet/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 #                                                                              #
 #  You should have received a copy of the GNU Lesser General Public License    #
 #  along with this program.                                                    #
 #  If not, see <https://www.gnu.org/licenses/>.                                #
 # ##############################################################################
 import pickle
 
-from metrics.wallet.analysis import Analysis, BasicAnalysis, DecisionAnalysis, OptiAnalysis, \
-    find_best_cpu_time_input, export_data_frame
+from metrics.wallet.analysis import Analysis, BasicAnalysis, DecisionAnalysis, BoundOptiAnalysis, OptiAnalysis, \
+    OverviewOptiAnalysis, find_best_cpu_time_input, export_data_frame
 from autograph.core.enumstyle import *
 
 import pandas as pd
 import jsonpickle.ext.pandas as jsonpickle_pd
 
 jsonpickle_pd.register_handlers()
```

### Comparing `crillab-metrics-1.2.6/metrics/wallet/analysis.py` & `crillab_metrics-1.3.0/metrics/wallet/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -470,14 +470,25 @@
         """
         return self.filter_inputs(
             function=lambda x: x[SUCCESS_COL],
             how='all',
             inplace=inplace
         )
 
+    def delete_simple_inputs(self, limit=10, inplace=False):
+        """
+        Based on success column and cpu time, it removes all the inputs commonly solved within a certain time limit
+        @rtype: the filtered analysis
+        """
+        return self.filter_inputs(
+            function=lambda x: not x[SUCCESS_COL] or x[EXPERIMENT_CPU_TIME] > limit,
+            how='any',
+            inplace=inplace
+        )
+
     def groupby(self, column) -> List[BasicAnalysis]:
         """
         Makes a group by a given column.
         @param column: column where to applu the groupby.
         @return: a list of Analysis with each group.
         """
         return [
@@ -555,16 +566,17 @@
 
         return export_data_frame(
             data_frame=pd.Series({
                 'n_experiment_wares': len(self.experiment_wares),
                 'n_inputs': len(self.inputs),
                 'n_experiments': len(df),
                 'n_missing_xp': (df['missing']).sum(),
-                'n_inconsistent_xp': (~df['consistent_xp']).sum(),
-                'n_inconsistent_xp_due_to_input': (~df['consistent_input']).sum(),
+                'n_inconsistent_xp': (~df['consistent_xp']).sum() if 'consistent_xp' in df.columns else None,
+                'n_inconsistent_xp_due_to_input': (
+                    ~df['consistent_input']).sum() if 'consistent_input' in df.columns else None,
                 'more_info_about_variables': "<analysis>.data_frame.describe(include='all')"
             }, name='analysis').to_frame(),
             **kwargs
         )
 
     def pivot_table(self, index=EXPERIMENT_INPUT, columns=EXPERIMENT_XP_WARE,
                     values=EXPERIMENT_CPU_TIME, **kwargs):
@@ -581,14 +593,38 @@
                 index=index,
                 columns=columns,
                 values=values
             ),
             **kwargs
         )
 
+    def score_table(self, cell_function, best_function, score_function, default_solver=None, score_name=None,
+                    normalize_function=None):
+        def default_normalize_function(values, group):
+            pass
+
+        if normalize_function is None:
+            normalize_function = default_normalize_function
+        tab = []
+        for index, group in self.data_frame.groupby('input'):
+            row = {'input': index}
+            values = []
+            for ew in self.experiment_wares:
+                cell = cell_function(group, ew)
+                row[ew] = normalize_function([cell], group)[0]
+                values.append(cell)
+            row['best'] = best_function(normalize_function(values, group))
+            tab.append(row)
+        df = pd.DataFrame(tab)
+        score_df = score_function(df, default_solver)
+        total = score_df.sum(numeric_only=True)
+        total['input'] = f'Score ({score_name})' if score_name is not None else 'Score'
+        new_df = df.append(total.transpose(), ignore_index=True)
+        return new_df
+
     def line_plot(self, index, column, values, **kwargs: dict):
         """
         Makes a lineplot of the data
         @param index: the x axis (colname of the current dataframe) of the line plot
         @param column: the different plots (colname of the current dataframe)
         @param values: the y axis (colname of the current dataframe) of the line plot
         @param kwargs: kwargs are given to the @LinePlot object
@@ -636,14 +672,41 @@
                 df = pd.read_csv(file)
             else:
                 df = pickle.load(file)
             if eval_data:
                 df = df.applymap(lambda x: eval(str(x)))
             return cls(data_frame=df)
 
+    def scatter_plot(self, xp_ware_x, xp_ware_y, color_col=None, scatter_col=EXPERIMENT_CPU_TIME,
+                     **kwargs):
+        """
+        To draw a scatter-plot, we need to specify the experiment-wares on the x-axis and tge
+        y-axis: xp_ware_x and
+        xp_ware_y. By default, the scatter plot draw its graphic by using the cpu_time of results:
+        you are free to
+        change this behaviour by replacing the scatter_col parameter.
+        @param xp_ware_x: the first experiment-ware
+        @param xp_ware_y: the second experiment-ware
+        @param color_col: to give a specific color to points in function of a column
+        @param scatter_col: The data to plot (cpu_time by default)
+        @param kwargs: kwargs are given to the ScatterPlot(...) object.
+        @return: the drawn figure
+        """
+        if xp_ware_x not in self.experiment_wares:
+            raise ValueError(f'Experiment-ware xp_ware_x={xp_ware_x} does not exist.')
+        if xp_ware_y not in self.experiment_wares:
+            raise ValueError(f'Experiment-ware xp_ware_y={xp_ware_y} does not exist.')
+
+        df = _make_scatter_plot_df(self, xp_ware_x, xp_ware_y, scatter_col, color_col)
+
+        plot = ScatterPlot(df, color_col=color_col, **kwargs)
+        plot.save()
+
+        return plot.show()
+
 
 def _is_none_or_nan(x):
     return x is None or math.isnan(x)
 
 
 def _make_list(l):
     if isinstance(l, list):
@@ -801,15 +864,15 @@
         'experiment_ware': d['experiment_ware'],
         'timeout': d['timeout'],
         col: df[col].mean()
     }
     return pd.Series(d2)
 
 
-class OptiAnalysis(BasicAnalysis):
+class BoundOptiAnalysis(BasicAnalysis):
     """
     An Optimality Analysis is an analysis with the constraint of having the cartesian product of
     experiment-wares and inputs and additionnal informations:
 
     - the success status of the experiment
     - the cpu time for producing this success status
     - the list of each found bound during the resolution
@@ -888,14 +951,92 @@
         ).line_plot(
             index='timeout',
             column='experiment_ware',
             values=col,
             **kwargs
         )
 
+    # def score_number_times_best_bound(self):
+
+
+class OverviewOptiAnalysis(BasicAnalysis):
+    def __init__(self, input_file: str = None, data_frame: DataFrame = None,
+                 basic_analysis: BasicAnalysis = None, log_level: str = 'WARNING'):
+        """
+        Constructs a decision analysis by giving an 'input_file' to parse the campaign logs OR a
+        'data_frame' of already build analysis OR a 'basic_analysis' with the necessary data to
+        build a DecisionAnalysis.
+        @param input_file: the yaml file to extract data
+        @param data_frame: a valid dataframe containing the exploded experiments
+        @param basic_analysis: a BasicAnalysis with the needed columns
+        @param log_level: The minimum level for the events to log while parsing the campaign.
+        """
+        if input_file is not None:
+            super().__init__(input_file, data_frame, log_level)
+        elif data_frame is not None:
+            self._data_frame = data_frame
+        elif basic_analysis is not None:
+            self._data_frame = basic_analysis.data_frame
+        else:
+            raise AttributeError('input_file or data_frame or basic_analysis needs to be given.')
+
+        # test if the analysis is in conformity
+        columns = set(self._data_frame.columns)
+        expected_columns = {EXPERIMENT_CPU_TIME, EXPERIMENT_TIMESTAMP_LIST, EXPERIMENT_BOUND_LIST,
+                            EXPERIMENT_BEST_BOUND, EXPERIMENT_OBJECTIVE, EXPERIMENT_STATUS}
+        missing = expected_columns - columns
+        if missing:
+            raise ValueError(f'Some columns are missing: {missing}')
+
+    def bound_stat_table(self, agg_col=None):
+        if agg_col is None:
+            agg_col = []
+        agg_col = [EXPERIMENT_XP_WARE] + agg_col
+        new_df = []
+        for index, group in self._data_frame.groupby(EXPERIMENT_INPUT):
+            best = min if 'min' in group[EXPERIMENT_OBJECTIVE].values else max
+            best_bound = best([v for v in group[EXPERIMENT_BEST_BOUND]])
+            for ew in group[EXPERIMENT_XP_WARE]:
+                tmp = dict()
+                row = group[group[EXPERIMENT_XP_WARE] == ew].iloc[0]
+                for c in agg_col:
+                    tmp[c] = row[c]
+                bound = get_as_list(row[EXPERIMENT_BOUND_LIST], -1)
+                tmp['Number of best bounds'] = bound == best_bound
+                tmp['Number of solutions'] = bound is not None
+                tmp['Number of optimal solutions'] = row[EXPERIMENT_CPU_TIME] < row[TIMEOUT_COL]
+                new_df.append(tmp)
+        return pd.DataFrame(new_df).groupby(agg_col).agg('sum')
+
+    def bound_bar_plot(self):
+        df = self.bound_stat_table()
+        new_df = []
+        for index, row in df.iterrows():
+            for c in df.columns:
+                if c == 'experiment_ware':
+                    continue
+                tmp = {'experiment_ware': index, 'title': c, 'total': row[c]}
+                new_df.append(tmp)
+
+        df2 = pd.DataFrame(new_df)
+        plot = BarPlot(df2, colx="experiment_ware", coly="total", category="title")
+        plot.plot.hline(len(self.inputs))
+        plot.save()
+        return plot.show()
+
+
+
+def get_as_list(l, index):
+    if isinstance(l, list):
+        return l[index]
+    elif pd.isnull(l):
+        return None
+    else:
+        return l
+
 
 def _cpu_time_stat(x, i):
     return x[EXPERIMENT_CPU_TIME] if x[SUCCESS_COL] else x[TIMEOUT_COL] * i
 
 
 def _compute_cpu_time_stats(df, par):
     return pd.Series({**{
@@ -941,15 +1082,15 @@
 
 
 def _compute_performance_ratio(df, row, vbew_name):
     time_vbew = df[(df[EXPERIMENT_INPUT] == row[EXPERIMENT_INPUT]) & (df[EXPERIMENT_XP_WARE] == vbew_name)][
         EXPERIMENT_CPU_TIME]
     if len(time_vbew) > 0:
         return row[EXPERIMENT_CPU_TIME] / \
-               time_vbew.iloc[0]
+            time_vbew.iloc[0]
     return None
 
 
 def _make_scatter_plot_df(analysis, xp_ware_x, xp_ware_y, scatter_col, color_col=None):
     df = analysis.keep_experiment_wares({xp_ware_x, xp_ware_y}).data_frame
     df = df[df[SUCCESS_COL]]
 
@@ -1075,14 +1216,15 @@
             **kwargs
         )
 
     def marginal_contribution(self, **kwargs: dict):
         df = self.contribution_table(contribution=False)
         df['experiment_ware'] = df.index
         plot = BarPlot(df, 'experiment_ware', 'vbew simple', **kwargs)
+        plot.plot.hline(len(self.inputs))
         plot.save()
         return plot.show()
 
     def cactus_plot(self, cumulated=False, cactus_col=EXPERIMENT_CPU_TIME, **kwargs: dict):
         """
         By default, the cactus plot draws its graphic by using the cpu_time of the results: you are
         free to change this
@@ -1126,41 +1268,14 @@
 
     def performance_profile(self, vbew_name, **kwargs: dict):
         df_solved = self.data_frame[self.data_frame[SUCCESS_COL]]
         local_analysis = self.add_variable('performance_ratio',
                                            lambda row: _compute_performance_ratio(df_solved, row, vbew_name))
         return local_analysis.cdf_plot(cdf_col='performance_ratio', **kwargs)
 
-    def scatter_plot(self, xp_ware_x, xp_ware_y, color_col=None, scatter_col=EXPERIMENT_CPU_TIME,
-                     **kwargs):
-        """
-        To draw a scatter-plot, we need to specify the experiment-wares on the x-axis and tge
-        y-axis: xp_ware_x and
-        xp_ware_y. By default, the scatter plot draw its graphic by using the cpu_time of results:
-        you are free to
-        change this behaviour by replacing the scatter_col parameter.
-        @param xp_ware_x: the first experiment-ware
-        @param xp_ware_y: the second experiment-ware
-        @param color_col: to give a specific color to points in function of a column
-        @param scatter_col: The data to plot (cpu_time by default)
-        @param kwargs: kwargs are given to the ScatterPlot(...) object.
-        @return: the drawn figure
-        """
-        if xp_ware_x not in self.experiment_wares:
-            raise ValueError(f'Experiment-ware xp_ware_x={xp_ware_x} does not exist.')
-        if xp_ware_y not in self.experiment_wares:
-            raise ValueError(f'Experiment-ware xp_ware_y={xp_ware_y} does not exist.')
-
-        df = _make_scatter_plot_df(self, xp_ware_x, xp_ware_y, scatter_col, color_col)
-
-        plot = ScatterPlot(df, color_col=color_col, **kwargs)
-        plot.save()
-
-        return plot.show()
-
     def box_plot(self, box_col=EXPERIMENT_CPU_TIME, box_by=EXPERIMENT_XP_WARE, **kwargs: dict):
         """
         By default, the box plot draw its graphic by using the cpu_time of results: the user is
         free to change this
         behaviour by replacing the box_col parameter. Also, by default, the box_by parameter is
         set to experiment_ware
         meaning that each box represents an experiment_ware. The user may like to replace this by
@@ -1176,14 +1291,15 @@
         plot = BoxPlot(df, **kwargs)
         plot.save()
 
         return plot.show()
 
 
 Analysis = DecisionAnalysis
+OptiAnalysis = BoundOptiAnalysis
 
 
 class DataFrameBuilder:
     """
     This builder permits to make a dataframe composed of the Campaign information.
     """
```

### Comparing `crillab-metrics-1.2.6/metrics/wallet/plot.py` & `crillab_metrics-1.3.0/metrics/wallet/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
         self._plot.x_label = x_axis_name
         self._plot.y_label = y_axis_name
 
         color_map = dict() if color_map is None else color_map
         style_map = dict() if style_map is None else style_map
 
-        for name, series in df.iteritems():
+        for name, series in df.items():
             style = PlotStyle()
             if name in color_map:
                 style.color = color_map[name]
             if name in style_map:
                 style.line_type = style_map[name]
             if show_marker:
                 style.marker_shape = MarkerShape.CIRCLE
@@ -163,15 +163,15 @@
 
         self._plot.x_label = x_axis_name
         self._plot.y_label = y_axis_name
 
         color_map = dict() if color_map is None else color_map
         style_map = dict() if style_map is None else style_map
 
-        for name, series in df.iteritems():
+        for name, series in df.items():
             style = PlotStyle()
             if name in color_map:
                 style.color = color_map[name]
             if name in style_map:
                 style.line_type = style_map[name]
             if show_marker:
                 style.marker_shape = MarkerShape.CIRCLE
@@ -269,15 +269,15 @@
                  df,
                  colx,
                  coly,
                  category=None,
                  title=BAR_TITLE,
                  x_axis_name=None,
                  y_axis_name=None,
-                 legend_location=Position.RIGHT,
+                 legend_location=None,
                  legend_offset=(0, 0),
                  ncol_legend=1,
                  estimator=sum,
                  **kwargs
                  ):
         super().__init__(**kwargs)
```

