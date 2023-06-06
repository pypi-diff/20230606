# Comparing `tmp/adafruit-circuitpython-midi-1.4.8.tar.gz` & `tmp/adafruit-circuitpython-midi-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-midi-1.4.8.tar", last modified: Sun Apr  3 19:13:21 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-midi-1.4.9.tar", last modified: Tue Jun  7 17:22:09 2022, max compression
```

## Comparing `adafruit-circuitpython-midi-1.4.8.tar` & `adafruit-circuitpython-midi-1.4.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.925581 adafruit-circuitpython-midi-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.909581 adafruit-circuitpython-midi-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.913581 adafruit-circuitpython-midi-1.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.913581 adafruit-circuitpython-midi-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16258 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.913581 adafruit-circuitpython-midi-1.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2022-04-03 19:13:21.925581 adafruit-circuitpython-midi-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.913581 adafruit-circuitpython-midi-1.4.8/adafruit_circuitpython_midi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2022-04-03 19:13:21.000000 adafruit-circuitpython-midi-1.4.8/adafruit_circuitpython_midi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-04-03 19:13:21.000000 adafruit-circuitpython-midi-1.4.8/adafruit_circuitpython_midi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-03 19:13:21.000000 adafruit-circuitpython-midi-1.4.8/adafruit_circuitpython_midi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-03 19:13:21.000000 adafruit-circuitpython-midi-1.4.8/adafruit_circuitpython_midi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-03 19:13:21.000000 adafruit-circuitpython-midi-1.4.8/adafruit_circuitpython_midi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.917581 adafruit-circuitpython-midi-1.4.8/adafruit_midi/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6008 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/channel_pressure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/control_change.py
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/control_change_values.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/midi_continue.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11250 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/midi_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/mtc_quarter_frame.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/note_off.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/note_on.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/pitch_bend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/polyphonic_key_pressure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/program_change.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/start.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/stop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/system_exclusive.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/adafruit_midi/timing_clock.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.921581 adafruit-circuitpython-midi-1.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.921581 adafruit-circuitpython-midi-1.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5409 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.921581 adafruit-circuitpython-midi-1.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/examples/midi_inoutdemo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/examples/midi_intest1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/examples/midi_memorycheck.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/examples/midi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-03 19:13:21.925581 adafruit-circuitpython-midi-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 19:13:21.925581 adafruit-circuitpython-midi-1.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    15526 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/tests/test_MIDIMessage_unittests.py
--rw-r--r--   0 runner    (1001) docker     (121)    17456 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/tests/test_MIDI_unittests.py
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-04-03 19:13:09.000000 adafruit-circuitpython-midi-1.4.8/tests/test_note_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.604071 adafruit-circuitpython-midi-1.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.596071 adafruit-circuitpython-midi-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.600071 adafruit-circuitpython-midi-1.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.600071 adafruit-circuitpython-midi-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16263 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.600071 adafruit-circuitpython-midi-1.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-06-07 17:22:09.604071 adafruit-circuitpython-midi-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.600071 adafruit-circuitpython-midi-1.4.9/adafruit_circuitpython_midi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-06-07 17:22:09.000000 adafruit-circuitpython-midi-1.4.9/adafruit_circuitpython_midi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-06-07 17:22:09.000000 adafruit-circuitpython-midi-1.4.9/adafruit_circuitpython_midi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:22:09.000000 adafruit-circuitpython-midi-1.4.9/adafruit_circuitpython_midi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 17:22:09.000000 adafruit-circuitpython-midi-1.4.9/adafruit_circuitpython_midi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-07 17:22:09.000000 adafruit-circuitpython-midi-1.4.9/adafruit_circuitpython_midi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.604071 adafruit-circuitpython-midi-1.4.9/adafruit_midi/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6008 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/channel_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/control_change.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/control_change_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/midi_continue.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11250 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/midi_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/mtc_quarter_frame.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/note_off.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/note_on.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/pitch_bend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/polyphonic_key_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/program_change.py
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/start.py
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/stop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/system_exclusive.py
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/adafruit_midi/timing_clock.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.604071 adafruit-circuitpython-midi-1.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.604071 adafruit-circuitpython-midi-1.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5409 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      891 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.604071 adafruit-circuitpython-midi-1.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/examples/midi_inoutdemo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/examples/midi_intest1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/examples/midi_memorycheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/examples/midi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:22:09.604071 adafruit-circuitpython-midi-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:22:09.604071 adafruit-circuitpython-midi-1.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    15526 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/tests/test_MIDIMessage_unittests.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17456 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/tests/test_MIDI_unittests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-06-07 17:21:56.000000 adafruit-circuitpython-midi-1.4.9/tests/test_note_parser.py
```

### Comparing `adafruit-circuitpython-midi-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-midi-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/.github/workflows/build.yml` & `adafruit-circuitpython-midi-1.4.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/.github/workflows/release.yml` & `adafruit-circuitpython-midi-1.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-midi-1.4.9/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
+  - repo: https://github.com/python/black
     rev: 22.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v0.14.0
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.2.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
     rev: v2.11.1
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
-    -   id: pylint
+      - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
-        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-    -   id: pylint
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
         name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
         types: [python]
         files: "^tests/"
         args:
-        - --disable=missing-docstring,consider-using-f-string,duplicate-code
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-midi-1.4.8/.pylintrc` & `adafruit-circuitpython-midi-1.4.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-midi-1.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-midi-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/LICENSE` & `adafruit-circuitpython-midi-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-midi-1.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-midi-1.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-midi-1.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/PKG-INFO` & `adafruit-circuitpython-midi-1.4.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-midi
-Version: 1.4.8
+Version: 1.4.9
 Summary: A CircuitPython helper for encoding/decoding MIDI packets over a MIDI or UART connection.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MIDI
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython midi uart encoding decoding
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-midi/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/midi/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MIDI/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_MIDI/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-midi-1.4.8/README.rst` & `adafruit-circuitpython-midi-1.4.9/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-midi/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/midi/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MIDI/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_MIDI/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_circuitpython_midi.egg-info/PKG-INFO` & `adafruit-circuitpython-midi-1.4.9/adafruit_circuitpython_midi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-midi
-Version: 1.4.8
+Version: 1.4.9
 Summary: A CircuitPython helper for encoding/decoding MIDI packets over a MIDI or UART connection.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MIDI
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython midi uart encoding decoding
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-midi/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/midi/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MIDI/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_MIDI/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_circuitpython_midi.egg-info/SOURCES.txt` & `adafruit-circuitpython-midi-1.4.9/adafruit_circuitpython_midi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/__init__.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/channel_pressure.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/channel_pressure.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/control_change.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/control_change.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/control_change_values.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/control_change_values.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/midi_continue.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/midi_continue.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/midi_message.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/midi_message.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/mtc_quarter_frame.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/mtc_quarter_frame.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/note_off.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/note_off.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/note_on.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/note_on.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/pitch_bend.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/pitch_bend.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/polyphonic_key_pressure.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/polyphonic_key_pressure.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/program_change.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/program_change.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/start.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/start.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/stop.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/stop.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/system_exclusive.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/system_exclusive.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/adafruit_midi/timing_clock.py` & `adafruit-circuitpython-midi-1.4.9/adafruit_midi/timing_clock.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-midi-1.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/docs/api.rst` & `adafruit-circuitpython-midi-1.4.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/docs/conf.py` & `adafruit-circuitpython-midi-1.4.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-midi-1.4.8/docs/index.rst` & `adafruit-circuitpython-midi-1.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/examples/midi_inoutdemo.py` & `adafruit-circuitpython-midi-1.4.9/examples/midi_inoutdemo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/examples/midi_intest1.py` & `adafruit-circuitpython-midi-1.4.9/examples/midi_intest1.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/examples/midi_memorycheck.py` & `adafruit-circuitpython-midi-1.4.9/examples/midi_memorycheck.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/examples/midi_simpletest.py` & `adafruit-circuitpython-midi-1.4.9/examples/midi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/setup.py` & `adafruit-circuitpython-midi-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/tests/test_MIDIMessage_unittests.py` & `adafruit-circuitpython-midi-1.4.9/tests/test_MIDIMessage_unittests.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/tests/test_MIDI_unittests.py` & `adafruit-circuitpython-midi-1.4.9/tests/test_MIDI_unittests.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-midi-1.4.8/tests/test_note_parser.py` & `adafruit-circuitpython-midi-1.4.9/tests/test_note_parser.py`

 * *Files identical despite different names*

