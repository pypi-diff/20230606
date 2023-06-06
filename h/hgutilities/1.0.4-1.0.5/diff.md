# Comparing `tmp/hgutilities-1.0.4.tar.gz` & `tmp/hgutilities-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgutilities-1.0.4.tar", last modified: Mon Jun  5 21:39:12 2023, max compression
+gzip compressed data, was "hgutilities-1.0.5.tar", last modified: Tue Jun  6 10:31:56 2023, max compression
```

## Comparing `hgutilities-1.0.4.tar` & `hgutilities-1.0.5.tar`

### file list

```diff
@@ -1,227 +1,228 @@
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.836202 hgutilities-1.0.4/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.645320 hgutilities-1.0.4/.github/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.654662 hgutilities-1.0.4/.github/workflows/
--rw-r-----   0 henry     (1000) henry     (1000)     1084 2023-06-05 19:53:05.000000 hgutilities-1.0.4/.github/workflows/python-publish.yml
--rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-05 19:53:05.000000 hgutilities-1.0.4/LICENSE.md
--rw-r-----   0 henry     (1000) henry     (1000)     7613 2023-06-05 21:39:12.835854 hgutilities-1.0.4/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     7063 2023-06-05 20:01:22.000000 hgutilities-1.0.4/README.md
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.655418 hgutilities-1.0.4/hgutilities/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.659959 hgutilities-1.0.4/hgutilities/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.662277 hgutilities-1.0.4/hgutilities/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      541 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/__pycache__/TesterProgram2.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      730 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/__pycache__/TesterProgram2.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      352 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/__pycache__/__init__.cpython-310.pyc
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.666534 hgutilities-1.0.4/hgutilities/defaults/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.671049 hgutilities-1.0.4/hgutilities/defaults/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      594 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/defaults.txt
--rw-r-----   0 henry     (1000) henry     (1000)      678 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/docs.txt
--rw-r-----   0 henry     (1000) henry     (1000)      333 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/inherit.txt
--rw-r-----   0 henry     (1000) henry     (1000)      589 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/loaddefaults.txt
--rw-r-----   0 henry     (1000) henry     (1000)      504 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/Documentation/processkwargs.txt
--rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.685305 hgutilities-1.0.4/hgutilities/defaults/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)   154356 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/DefaultsHelpText.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1923 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/DoDocs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3774 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/Docs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      728 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/Inherit.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2262 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/LoadDefaults.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3782 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/LoadDefaults.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3165 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4611 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1019 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/SetDocs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      432 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1065 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/__init__.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3805 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      749 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2265 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3186 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2881 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/docs.py
--rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/inherit.py
--rw-r-----   0 henry     (1000) henry     (1000)     1518 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/loaddefaults.py
--rw-r-----   0 henry     (1000) henry     (1000)     2502 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/defaults/processkwargs.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.690242 hgutilities-1.0.4/hgutilities/plotting/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.693716 hgutilities-1.0.4/hgutilities/plotting/Default Settings/
--rw-r-----   0 henry     (1000) henry     (1000)      181 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Default Settings/Animate.txt
--rw-r-----   0 henry     (1000) henry     (1000)      580 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Default Settings/Figure.txt
--rw-r-----   0 henry     (1000) henry     (1000)      314 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Default Settings/Figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/Default Settings/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.699841 hgutilities-1.0.4/hgutilities/plotting/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      504 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/Animate.txt
--rw-r-----   0 henry     (1000) henry     (1000)      414 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/Figure.txt
--rw-r-----   0 henry     (1000) henry     (1000)      564 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/Figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      771 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/create_animations.txt
--rw-r-----   0 henry     (1000) henry     (1000)      592 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/create_figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1155 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/Documentation/plotting.txt
--rw-r-----   0 henry     (1000) henry     (1000)     9033 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/README.md
--rw-r-----   0 henry     (1000) henry     (1000)     1098 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.729856 hgutilities-1.0.4/hgutilities/plotting/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)     3616 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Animate.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5849 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Animate.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     7105 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figure.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    12637 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figure.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3492 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figures.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4308 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figures.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      584 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Line.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      795 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Line.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      970 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Line.cpython-38.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1245 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Lines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2083 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Lines.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2773 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Lines.cpython-38.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     6113 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    10132 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plot.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    11426 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plot.cpython-38.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    11376 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotAxes.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     7542 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotAxes.cpython-38.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      519 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotFunctions.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      822 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotFunctions.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5102 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotShape.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     8252 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotShape.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5135 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotShape.cpython-38.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4366 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotUtils.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4172 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotUtils.cpython-38.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2928 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plots.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4497 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plots.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3439 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plots.cpython-38.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1121 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1990 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/__init__.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3641 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     7154 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3548 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      558 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2595 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/animate.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.737945 hgutilities-1.0.4/hgutilities/plotting/datatypes/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.746841 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/
--rw-r-----   0 henry     (1000) henry     (1000)      267 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Bar.txt
--rw-r-----   0 henry     (1000) henry     (1000)      173 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Bars.txt
--rw-r-----   0 henry     (1000) henry     (1000)      699 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
--rw-r-----   0 henry     (1000) henry     (1000)      421 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Data.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1081 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Line.txt
--rw-r-----   0 henry     (1000) henry     (1000)      180 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Lines.txt
--rw-r-----   0 henry     (1000) henry     (1000)      334 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Pie.txt
--rw-r-----   0 henry     (1000) henry     (1000)      553 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Surface.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.755552 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      676 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Bar.txt
--rw-r-----   0 henry     (1000) henry     (1000)      850 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Bars.txt
--rw-r-----   0 henry     (1000) henry     (1000)      345 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Colormap.txt
--rw-r-----   0 henry     (1000) henry     (1000)      742 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Data.txt
--rw-r-----   0 henry     (1000) henry     (1000)      639 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Line.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1190 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Lines.txt
--rw-r-----   0 henry     (1000) henry     (1000)      637 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Pie.txt
--rw-r-----   0 henry     (1000) henry     (1000)      963 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Surface.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.780395 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      541 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      883 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1552 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      886 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      855 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      898 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1273 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Colorplot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      691 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Data.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      966 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Data.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      550 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Line.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      785 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Line.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2248 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2215 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      782 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      883 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1626 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2413 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      565 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1548 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1288 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      715 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      574 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2244 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      797 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1641 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      219 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/bar.py
--rw-r-----   0 henry     (1000) henry     (1000)      992 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/bars.py
--rw-r-----   0 henry     (1000) henry     (1000)      845 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/colorplot.py
--rw-r-----   0 henry     (1000) henry     (1000)      244 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/data.py
--rw-r-----   0 henry     (1000) henry     (1000)      222 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/line.py
--rw-r-----   0 henry     (1000) henry     (1000)     1630 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/lines.py
--rw-r-----   0 henry     (1000) henry     (1000)      370 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/pie.py
--rw-r-----   0 henry     (1000) henry     (1000)      979 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/datatypes/surface.py
--rw-r-----   0 henry     (1000) henry     (1000)     5255 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/figure.py
--rw-r-----   0 henry     (1000) henry     (1000)     2538 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/figures.py
--rw-r-----   0 henry     (1000) henry     (1000)      386 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotfunctions.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.786623 hgutilities-1.0.4/hgutilities/plotting/plottypes/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.788576 hgutilities-1.0.4/hgutilities/plotting/plottypes/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      477 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/Documentation/Plot.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.807730 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)     3690 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1879 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3777 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1327 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1135 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1350 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2003 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotColorplot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4552 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     7970 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1350 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1322 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3219 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3141 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3657 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3788 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2014 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4573 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1361 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3230 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3209 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plot.py
--rw-r-----   0 henry     (1000) henry     (1000)     3354 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plotbars.py
--rw-r-----   0 henry     (1000) henry     (1000)     2613 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plotcolorplot.py
--rw-r-----   0 henry     (1000) henry     (1000)     6683 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plotlines.py
--rw-r-----   0 henry     (1000) henry     (1000)     1249 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plotpie.py
--rw-r-----   0 henry     (1000) henry     (1000)     3691 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plottypes/plotsurface.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.812225 hgutilities-1.0.4/hgutilities/plotting/plotutils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 21:37:49.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.822048 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)     1138 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1838 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5357 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     8558 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5262 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/PlotShape.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1453 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2325 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1159 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5378 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1474 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      690 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/figuresize.py
--rw-r-----   0 henry     (1000) henry     (1000)     4445 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/griddimensions.py
--rw-r-----   0 henry     (1000) henry     (1000)     4425 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/plotshape.py
--rw-r-----   0 henry     (1000) henry     (1000)     1287 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/plotting/plotutils/savefigure.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.825977 hgutilities-1.0.4/hgutilities/utils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.834975 hgutilities-1.0.4/hgutilities/utils/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      474 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Dicts.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1546 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Groups.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2364 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Groups.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1385 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Paths.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2695 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Paths.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      311 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/Strings.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      168 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      495 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1567 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/groups.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1406 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/__pycache__/paths.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/dicts.py
--rw-r-----   0 henry     (1000) henry     (1000)     1419 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/groups.py
--rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/paths.py
--rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-05 19:36:08.000000 hgutilities-1.0.4/hgutilities/utils/plots.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-05 21:39:12.659180 hgutilities-1.0.4/hgutilities.egg-info/
--rw-r-----   0 henry     (1000) henry     (1000)     7613 2023-06-05 21:39:12.000000 hgutilities-1.0.4/hgutilities.egg-info/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)    10759 2023-06-05 21:39:12.000000 hgutilities-1.0.4/hgutilities.egg-info/SOURCES.txt
--rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-05 21:39:12.000000 hgutilities-1.0.4/hgutilities.egg-info/dependency_links.txt
--rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-05 21:39:12.000000 hgutilities-1.0.4/hgutilities.egg-info/requires.txt
--rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-05 21:39:12.000000 hgutilities-1.0.4/hgutilities.egg-info/top_level.txt
--rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-05 21:39:12.836318 hgutilities-1.0.4/setup.cfg
--rw-r-----   0 henry     (1000) henry     (1000)     1342 2023-06-05 21:35:51.000000 hgutilities-1.0.4/setup.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.725046 hgutilities-1.0.5/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.693046 hgutilities-1.0.5/.github/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.697046 hgutilities-1.0.5/.github/workflows/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1084 2023-06-06 07:09:05.000000 hgutilities-1.0.5/.github/workflows/python-publish.yml
+-rw-rw-r--   0 henry     (1000) henry     (1000)    35149 2023-06-06 07:09:05.000000 hgutilities-1.0.5/LICENSE.md
+-rw-rw-r--   0 henry     (1000) henry     (1000)     7866 2023-06-06 10:31:56.725046 hgutilities-1.0.5/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)     7148 2023-06-06 08:09:48.000000 hgutilities-1.0.5/README.md
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.697046 hgutilities-1.0.5/hgutilities/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.697046 hgutilities-1.0.5/hgutilities/Documentation/
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/Documentation/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2483 2023-06-06 10:29:51.000000 hgutilities-1.0.5/hgutilities/Documentation/hgutilities.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      154 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/__init__.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.701046 hgutilities-1.0.5/hgutilities/__pycache__/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      541 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/__pycache__/TesterProgram2.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      730 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/__pycache__/TesterProgram2.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      352 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/__pycache__/__init__.cpython-310.pyc
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.701046 hgutilities-1.0.5/hgutilities/defaults/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.701046 hgutilities-1.0.5/hgutilities/defaults/Documentation/
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      614 2023-06-06 08:19:26.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/defaults.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      701 2023-06-06 08:19:23.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/docs.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      353 2023-06-06 08:19:42.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/inherit.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      608 2023-06-06 08:19:38.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/loaddefaults.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      524 2023-06-06 08:19:31.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/processkwargs.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      229 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__init__.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.701046 hgutilities-1.0.5/hgutilities/defaults/__pycache__/
+-rw-rw-r--   0 henry     (1000) henry     (1000)   154356 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/DefaultsHelpText.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1923 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/DoDocs.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3774 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/Docs.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      728 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/Inherit.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2262 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/LoadDefaults.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3782 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/LoadDefaults.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3165 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4611 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1019 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/SetDocs.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      432 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1065 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3805 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      749 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2265 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3186 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2881 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/docs.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      656 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/inherit.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1518 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/loaddefaults.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2502 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/processkwargs.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.705046 hgutilities-1.0.5/hgutilities/plotting/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.705046 hgutilities-1.0.5/hgutilities/plotting/Default Settings/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      181 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Default Settings/Animate.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      580 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Default Settings/Figure.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      314 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Default Settings/Figures.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Default Settings/__init__.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.705046 hgutilities-1.0.5/hgutilities/plotting/Documentation/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      581 2023-06-06 08:18:45.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/Animate.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      414 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/Figure.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      564 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/Figures.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      791 2023-06-06 08:18:42.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/create_animations.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      612 2023-06-06 08:18:39.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/create_figures.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1155 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/plotting.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)    10839 2023-06-06 08:05:19.000000 hgutilities-1.0.5/hgutilities/plotting/README.md
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1098 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__init__.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.709046 hgutilities-1.0.5/hgutilities/plotting/__pycache__/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3616 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Animate.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     5849 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Animate.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     7105 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figure.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)    12637 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figure.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3492 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figures.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4308 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figures.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      584 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Line.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      795 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Line.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      970 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Line.cpython-38.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1245 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Lines.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2083 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Lines.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2773 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Lines.cpython-38.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     6113 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plot.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)    10132 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plot.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)    11426 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plot.cpython-38.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)    11376 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotAxes.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     7542 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotAxes.cpython-38.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      519 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotFunctions.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      822 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotFunctions.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     5102 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotShape.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     8252 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotShape.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     5135 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotShape.cpython-38.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4366 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotUtils.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4172 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotUtils.cpython-38.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2928 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plots.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4497 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plots.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3439 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plots.cpython-38.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1121 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1990 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3641 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     7154 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3548 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      558 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2595 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/animate.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.713046 hgutilities-1.0.5/hgutilities/plotting/datatypes/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.713046 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      267 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Bar.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      173 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Bars.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      699 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      421 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Data.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1081 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Line.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      180 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Lines.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      334 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Pie.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      553 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Surface.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/__init__.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.713046 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      664 2023-06-06 08:18:34.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Bar.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      869 2023-06-06 08:18:26.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Bars.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      365 2023-06-06 08:18:23.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Colormap.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      762 2023-06-06 08:18:19.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Data.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      659 2023-06-06 08:18:14.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Line.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1210 2023-06-06 08:18:11.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Lines.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      656 2023-06-06 08:18:07.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Pie.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      859 2023-06-06 08:18:04.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Surface.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__init__.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.717046 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      541 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      883 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1552 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      886 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      855 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      898 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1273 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Colorplot.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      691 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Data.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      966 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Data.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      550 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Line.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      785 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Line.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2248 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2215 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      782 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      883 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1626 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2413 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      565 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1548 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1288 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      715 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      574 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2244 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      797 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1641 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      219 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/bar.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      992 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/bars.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      845 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/colorplot.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      244 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/data.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      222 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/line.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1630 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/lines.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      370 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/pie.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      979 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/surface.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     5255 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/figure.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2538 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/figures.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      386 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotfunctions.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.721046 hgutilities-1.0.5/hgutilities/plotting/plottypes/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.721046 hgutilities-1.0.5/hgutilities/plotting/plottypes/Documentation/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      497 2023-06-06 08:18:00.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/Documentation/Plot.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/Documentation/__init__.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__init__.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.721046 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3690 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1879 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3777 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1327 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1135 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1350 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2003 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotColorplot.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4552 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     7970 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1350 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1322 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3219 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3141 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3657 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3788 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2014 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4573 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1361 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3230 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3209 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plot.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3354 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plotbars.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2613 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plotcolorplot.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     6683 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plotlines.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1249 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plotpie.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     3691 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plotsurface.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.721046 hgutilities-1.0.5/hgutilities/plotting/plotutils/
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__init__.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.725046 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1138 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1838 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     5357 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     8558 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     5262 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/PlotShape.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1453 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2325 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1159 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     5378 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1474 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      690 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/figuresize.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4445 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/griddimensions.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     4425 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/plotshape.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1287 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/savefigure.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.725046 hgutilities-1.0.5/hgutilities/utils/
+-rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__init__.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.725046 hgutilities-1.0.5/hgutilities/utils/__pycache__/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      474 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Dicts.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1546 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Groups.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2364 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Groups.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1385 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Paths.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     2695 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Paths.cpython-311.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      311 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Strings.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      168 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      495 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1567 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/groups.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1406 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/paths.cpython-310.pyc
+-rw-rw-r--   0 henry     (1000) henry     (1000)      191 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/dicts.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1419 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/groups.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      927 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/paths.py
+-rw-rw-r--   0 henry     (1000) henry     (1000)      668 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/plots.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.697046 hgutilities-1.0.5/hgutilities.egg-info/
+-rw-rw-r--   0 henry     (1000) henry     (1000)     7866 2023-06-06 10:31:56.000000 hgutilities-1.0.5/hgutilities.egg-info/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)    10801 2023-06-06 10:31:56.000000 hgutilities-1.0.5/hgutilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-06-06 10:31:56.000000 hgutilities-1.0.5/hgutilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       35 2023-06-06 10:31:56.000000 hgutilities-1.0.5/hgutilities.egg-info/requires.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-06-06 10:31:56.000000 hgutilities-1.0.5/hgutilities.egg-info/top_level.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-06-06 10:31:56.725046 hgutilities-1.0.5/setup.cfg
+-rw-rw-r--   0 henry     (1000) henry     (1000)     1453 2023-06-06 10:28:34.000000 hgutilities-1.0.5/setup.py
```

### Comparing `hgutilities-1.0.4/.github/workflows/python-publish.yml` & `hgutilities-1.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/LICENSE.md` & `hgutilities-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/PKG-INFO` & `hgutilities-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.4
+Version: 1.0.5
 Summary: A triple of tools used for plotting, handling key-words, and utilities
+Home-page: UNKNOWN
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
+License: UNKNOWN
 Keywords: python,matplotlib,plotting,default,keywords,utils
-Classifier: Development Status :: 1 - Planning
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
 # HGUtilities
@@ -36,40 +41,40 @@
 
 - To view all the defaults you need to go into the script itself
 - It is awkward to change the value of those variables from an interface
 - It is impossible to change the default values without digging into the code itself.
 - Passing in many arguments to functions is messy
 - Mutable default values need to be implemented more carefully
 
-Normally there are two ways of handling key word arguments with default values.The simpler way is to have the key word in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several key word arguemnts, this becomes messy however, and it would be preferred to pack the key words together with **kwargs. With this second method, there will need to be code that detects if a key word is in the **kwargs dict, and if so change it. This means we have a method for every key word argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the key word arguments a function takes in.
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
 
-In the second case, we cannot see what key word arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
 
 ### The Solution
 
 For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
 
-Whenever a method takes in key word arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any key word arguments that were not in the list of defaults, the file will be opened and overwritten with the new key word arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
 
     from hgutilities import defaults
 
     class MyClass():
 
         def __init__(self, **kwargs):
             defaults.kwargs(self, **kwargs)
 
     defaults.load(MyClass)
 
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such key word arguments should be set to `null` in the json file of defaults.
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
 
 The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
 
 ## Plotting
 
-For full documentation, see the specific README inside the "Plotting" module folder.
+For full documentation, see the specific README inside the "plotting" module folder.
 
 When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
 
 The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
 
 It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
 
@@ -85,7 +90,10 @@
 - more control over subplot placement
 - automatic paragraph organisation for documentation
 - better distribution of subplots over multiple figures
 - control over tick labels
 - horizontal bar charts
 - better file extension handling for Defaults package
 - inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
+- add README to defaults subpackage
+
```

### Comparing `hgutilities-1.0.4/README.md` & `hgutilities-1.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -20,40 +20,40 @@
 
 - To view all the defaults you need to go into the script itself
 - It is awkward to change the value of those variables from an interface
 - It is impossible to change the default values without digging into the code itself.
 - Passing in many arguments to functions is messy
 - Mutable default values need to be implemented more carefully
 
-Normally there are two ways of handling key word arguments with default values.The simpler way is to have the key word in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several key word arguemnts, this becomes messy however, and it would be preferred to pack the key words together with **kwargs. With this second method, there will need to be code that detects if a key word is in the **kwargs dict, and if so change it. This means we have a method for every key word argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the key word arguments a function takes in.
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
 
-In the second case, we cannot see what key word arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
 
 ### The Solution
 
 For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
 
-Whenever a method takes in key word arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any key word arguments that were not in the list of defaults, the file will be opened and overwritten with the new key word arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
 
     from hgutilities import defaults
 
     class MyClass():
 
         def __init__(self, **kwargs):
             defaults.kwargs(self, **kwargs)
 
     defaults.load(MyClass)
 
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such key word arguments should be set to `null` in the json file of defaults.
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
 
 The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
 
 ## Plotting
 
-For full documentation, see the specific README inside the "Plotting" module folder.
+For full documentation, see the specific README inside the "plotting" module folder.
 
 When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
 
 The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
 
 It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
 
@@ -68,8 +68,10 @@
 - automatic prefixing to axes
 - more control over subplot placement
 - automatic paragraph organisation for documentation
 - better distribution of subplots over multiple figures
 - control over tick labels
 - horizontal bar charts
 - better file extension handling for Defaults package
-- inherit function should be able to take in a single attribute as a non-iterable
+- inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
+- add README to defaults subpackage
```

### Comparing `hgutilities-1.0.4/hgutilities/__pycache__/TesterProgram2.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/__pycache__/TesterProgram2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/__pycache__/TesterProgram2.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/__pycache__/TesterProgram2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/Documentation/defaults.txt` & `hgutilities-1.0.5/hgutilities/defaults/Documentation/defaults.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     load
     kwargs
     docs
     inherit
 
 For further documentation see the following:
 load, kwargs, docs, inherit
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Defaults
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.4/hgutilities/defaults/Documentation/docs.txt` & `hgutilities-1.0.5/hgutilities/defaults/Documentation/docs.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 The purpose of this function is to prevent bloated doc strings
 at the start of modules, classes, and functions by storing the
 doc strings in text files.
 
-By placing "Defaults.docs()" in a package __init__ file, all the
+By placing "defaults.docs()" in a package __init__.py file, all the
 modules, classes, and functions that were imported within that file
 that are part of the package will have their doc strings set. The
 doc strings are set from text files stored in folders called
 "Documentation", and these folders are in the same directory as
 the script for the corresponding module, class, or function.
 
 For further documentation see the following:
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Defaults
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.4/hgutilities/defaults/Documentation/loaddefaults.txt` & `hgutilities-1.0.5/hgutilities/defaults/Documentation/loaddefaults.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 class attributes. The file will have the same name as the class
 and should be located in a folder called "Default Settings" in
 the same folder as the script where the class is defined.
 
 After a class, (e.g. "MyClass") has been defined, calling
 "Defaults.load(MyClass)" will load from the file if it exists.
 
-Any key-word value pairs defined in parent classes will be
+Any keyword-value pairs defined in parent classes will be
 inherited.
 
 For further documentation see the following:
 kwargs
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Defaults
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/DefaultsHelpText.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/DefaultsHelpText.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/DoDocs.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/DoDocs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/Docs.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/Docs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/Inherit.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/Inherit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/LoadDefaults.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/LoadDefaults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/LoadDefaults.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/LoadDefaults.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/SetDocs.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/SetDocs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/__init__.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/docs.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/docs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/docs.py` & `hgutilities-1.0.5/hgutilities/defaults/docs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/inherit.py` & `hgutilities-1.0.5/hgutilities/defaults/inherit.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/loaddefaults.py` & `hgutilities-1.0.5/hgutilities/defaults/loaddefaults.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/defaults/processkwargs.py` & `hgutilities-1.0.5/hgutilities/defaults/processkwargs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/Default Settings/Figure.txt` & `hgutilities-1.0.5/hgutilities/plotting/Default Settings/Figure.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/Documentation/Figures.txt` & `hgutilities-1.0.5/hgutilities/plotting/Documentation/Figures.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/Documentation/create_animations.txt` & `hgutilities-1.0.5/hgutilities/plotting/Documentation/create_animations.txt`

 * *Files 23% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 This also returns the Figures object produced if
 the user wants to work with it directly, but this
 is not encouraged, and should only be necessary if
 a feature has not been implemented.
 
 For further documentation see the following:
 Animate, Figures, and Data classes
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.4/hgutilities/plotting/Documentation/plotting.txt` & `hgutilities-1.0.5/hgutilities/plotting/Documentation/plotting.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/README.md` & `hgutilities-1.0.5/hgutilities/plotting/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,45 +15,45 @@
 
 ## Overview and Structure
 
 This is a tool designed to make creating figures with multiple subplots easier. The data is prescribed, and the creation of the figures is handled by the package.
 
 ### Figures
 
-At the top level there is a Figures object. This contains all the information about the figures to be produced. This includes the data to be plotted, the title of the figures, if the figures are going to be shown or saved, the base path to be saved to if needed, the number of subplots per figure, and any appearance settings of the plots. It organises the creation of Figure objects, as if there is too much data for one figure, it will need to be splot over multiple.
+At the top level there is a Figures object. This contains all the information about the figures to be produced. This includes the data to be plotted, the title of the figures, if the figures are going to be shown or saved, the base path to be saved to if needed, the number of subplots per figure, and any appearance settings of the plots. It organises the creation of Figure objects, as if there is too much data for one figure, it will need to be spread over multiple.
 
 ### Animate
 
-This is a subclass of Figures, and allows you to make animations. Creating animations is done through exactly the same process as creating figures, with one difference. The independent variables can't be animated, but the dependent variables will need to be passed in as a list or array where each element gives the values of the variable for each frame.
+This is a subclass of Figures, and allows the user to make animations. Creating animations is done through exactly the same process as creating figures, with one difference. The independent variables can't be animated, but the dependent variables will need to be passed in as a list or array where each element of the list or array gives the values of the variable for each frame. See the [usage](#usage) section for more details.
 
 ### Figure
 
-The next level down is the Figure object. This arranges how the subplots will be arranged on the figure and organises the creation of the subplots which are handled by Plot objects. Adding the title and universal legend happens here. An aspect ratio can be specified, and it will try to arrange the plots to that ratio as closely as it can.
+The next level down is the Figure object. This arranges how the subplots will be arranged on the figure and organises the creation of the subplots, which are subsequently handled by Plot objects. Adding the title and universal legend happens here. An aspect ratio can be specified, and it will try to arrange the plots in that ratio as closely as it can.
 
 ### Plot
 
 A Plot object is responsible for each individual subplot. The subplot title, axis labels, plot legends, and the data to be put on the subplot are handled at this level. There are subclasses of Plot for different types of data object, and these classes follow the naming convention of appending "Plot" to the name of the data object they are associated with.
 
 ### Data
 
-This class handles the data to be plotted. The most basic is a Lines object which handles quantititive data on a 2D plot. There is also a Bars object which handles bar charts, and a Pie object that handles pie charts. Colormesh and Surface are also subclasses which work with 3 dimensional data. As a rule of thumb, if two matplotlib plotting functions are sufficiently different, their data will be handled by two distinct subclasses of Data. Here are the subclasses of Data.
+This class handles the data to be plotted. The most basic is a Lines object which handles quantititive data on a 2D plot. There is also a Bars object which handles bar charts, and a Pie object that handles pie charts. Colorplot and Surface are also subclasses which work with 3 dimensional data. As a rule of thumb, if two matplotlib plotting functions are sufficiently different, their data will be handled by two distinct subclasses of Data. Here are the subclasses of Data currently implemented.
 
 - Lines. This takes in a collection of Line objects. It also has an optional keyword argument called `plot_type` which controls whether the plot is made using `plot`, `semilogy`, `semilogx`, `loglog`, or `errorbar`. Each Line object corresponds to a single line on a subplot, and has a list of $x$ values and $y$ values. The Line object also has optional attributes that control the appearance of the line and the line label.
 - Bars. This is similar to Lines, but it handles Bar objects which are similar to Line objects. The key distinction here is that the $x$ axis has qualitative data, and that prescribing the appearance of the bars is very different from lines. We note that a Bar object handles an entire series of data, and a Bars object handles a bar chart plot, so a single plot with two data series on it will be handled by one Bars object and two Bar objects.
-- Pie. Pie charts cannot show multiple data series so this subclass does not have a correspondence to Line or Bar. This takes in all the arguments that the matplotlib pie function takes in, and also any of the arguments from the parent class, Plot.
-- Colormesh. This shows a single data series with two dimensional input and one dimensional output. It takes in all arguments that the matplotlib pcolormesh function takes in and uses pcolormesh instead of pcolor.
-- Surface. This shows a single data series with a two dimensional input and a one dimensional output. Different from Colormesh, this produces a plot in three spatial dimensions represented as a surface.
+- Pie. Pie charts cannot show multiple data series so this subclass does not have a correspondence to Line or Bar. This takes in all the arguments that the matplotlib `pie` function takes in, and also any of the arguments from the parent class, Plot.
+- Colormesh. This shows a single data series with two dimensional input and one dimensional output. It takes in almost all of the arguments that the matplotlib pcolormesh function takes in and uses pcolormesh instead of pcolor.
+- Surface. This shows a single data series with a two dimensional input and a one dimensional output. Different from Colormesh, this produces a plot in three spatial dimensions represented as a surface. Wireframe and 3D contour plotting is also supported by passing in "plot_wireframe" or "contour" as a value of the `plot_type` keyword
 
 ### Usage
 
 The first step in creating a figure is specifying the data. Here is an example with plotting a single line on a graph. `lines_obj` is the Data object in this case, and we pass it in to `create_figures`.
     
     # Importing
     import numpy as np
-    from hgutils import plotting
+    from hgutilities import plotting
 
     # Creation of Line object
     x_values = np.arange(0, 2*np.pi, 0.1)
     y_values = np.sin(x_values)
     line_obj = plotting.line(x_values, y_values)
 
     # Creation of Lines object
@@ -63,15 +63,15 @@
     plotting.create_figures(lines_obj)
 
 If we want to create multiple lines, we can pass in a list of line objects. We can also give our figure some labels.
 
 
     # Importing
     import numpy as np
-    from hgutils import plotting
+    from hgutilities import plotting
 
     # Creation of Line object
     def get_line_obj(n):
         y_values = np.sin(n*x_values)
         label = f"n = {n}"
         line_obj = plotting.line(x_values, y_values, label=label)
         return line_obj
@@ -81,32 +81,32 @@
     line_objects = [get_line_obj(n) for n in x_coefficients]
 
     # Creation of Lines object
     title = "Sin(nx)"
     x_label = "My x axis label"
     y_label = "My y axis label"
     lines_obj = plotting.lines(line_objects, title=title, legend=True,
-                               x_label=x_label, y_label=y_label)
+                                  x_label=x_label, y_label=y_label)
 
     # Creation of figures
     plotting.create_figures(lines_obj)
 
-We could have data split across multiple subplots. By default we have `subplots=None` and all subplots will be put on a figure. If subplots is specified and the subplots do not fit on one figure, they will be distributed across multiple. The number given by the subplots key-word is an upper bound on how many subplots there will be on a given figure, and the number of figures is as small as possible given that constraint.
+We could have data split across multiple subplots. By default we have `subplots=None` and all subplots will be put on a figure. If subplots is specified and the subplots do not fit on one figure, they will be distributed across multiple. The subplots will be evenly distributed over $\left \lfloor \frac{\text{total subplots}}{\text{subplots per figure}} \right \rfloor$ figures, so the number of subplots per figure is at least as big as the number specified. In future versions this behaviour will change, and the number given by the subplots keyword will be an upper bound on how many subplots there will be on a given figure, and the number of figures will be as small as possible given that constraint.
 
     # Importing
     import numpy as np
-    from hgutils import plotting
+    from hgutilities import plotting
 
     def get_lines_obj(n):
         line_obj = get_line_obj(n)
         title = f"Sin({n}x)"
         x_label = "My x axis label"
         y_label = "My y axis label"
         lines_obj = plotting.lines(line_obj, title=title,
-                                x_label=x_label, y_label=y_label)
+        x_label=x_label, y_label=y_label)
         return lines_obj
 
     def get_line_obj(n):
         y_values = np.sin(n*x_values)
         line_obj = plotting.line(x_values, y_values)
         return line_obj
 
@@ -118,15 +118,15 @@
     # Creation of figures
     plotting.create_figures(lines_objects, subplots=6)
 
 You can mix the types of plot within a figure. Here is an example that shows the other types of plot supported.
 
     # Importing
     import numpy as np
-    from hgutils import plotting
+    from hgutilities import plotting
 
     # Creating bars object
     x_values_1 = ["Red", "Green", "Blue"]
     y_values_1 = [4, 2, 7]
     bar_obj_1 = plotting.bar(x_values_1, y_values_1)
 
     x_values_2 = ["Green", "Red", "Blue"]
@@ -158,16 +158,44 @@
     colormap_obj = plotting.colorplot(x_mesh, y_mesh, z_mesh,
                                       title=title)
 
     # Creation of figures
     data_objects = [bars_obj, pie_obj, surface_obj, colormap_obj]
     plotting.create_figures(data_objects)
 
+Animations can also be made by adding a dimension to the dependent variable. Currently this is only implemented for Surface objects. We note that all matplotlib figure objects need to be kept open while making the animation, so this is only suitable for short animations.
+
+    # Importing
+    import numpy as np
+    from hgutilities import plotting
+
+    # Set independent variable values
+    x_values = np.arange(0, 10, 0.5)
+    y_values = np.arange(0, 10, 0.5)
+    x_mesh, y_mesh = np.meshgrid(x_values, y_values)
+
+    # Set dependent variable values
+    def get_z_mesh_layer(time_value):
+        time_mesh = np.ones(x_mesh.shape) * time_value
+        z_mesh_layer = (np.sin(x_mesh + time_mesh)
+                        + np.sin(y_mesh + time_mesh))
+        return z_mesh_layer
+
+    time_values = np.arange(0, 2*np.pi, 0.5)
+    z_meshes = [get_z_mesh_layer(time_value)
+                for time_value in time_values]
+    z_meshes = np.stack(z_meshes)
+
+    # Creating animation
+    surface_obj = plotting.surface(x_mesh, y_mesh, z_meshes)
+    surface_objects = [surface_obj]
+    plotting.create_animations(surface_objects)
+
 ## Features
 
 ### Universal Legend
 
-The universal legend is a tool that can be used if all subplots in a figure have the same legend. An extra blank subplot is created and the space is used to show a legend that corresponds to all plots. This can be activated by passing `universal_legend=True` as a keyword-value pair into the `create_figures` function, and any individual legends will be overruled.
+The universal legend is a tool that can be used if all subplots in a figure have the same legend. An extra blank subplot is created and the space is used to show a legend that corresponds to all plots. This can be activated by passing `universal_legend=True` as a keyword-value pair into the `create_figures` function, and any individual legends will be overruled. Exception handling not implemented, will crash or get unexpected results if not used properly.
 
 ### Subplot Adjustment
 
-If the optional key-word argument, `adjust_subplots=True` is passed in to `create_figures` (or `create_animation`), then the matplotlib subplot adjustment tool will appear when the figures are created. The subplots are usually plotted with using the constrained layout, but in this case that will be turned off and tight layout used instead.
+Note: this feature has not been implemented yet. If the optional keyword argument, `adjust_subplots=True` is passed in to `create_figures` (or `create_animation`), then the matplotlib subplot adjustment tool will appear when the figures are created. The subplots are usually plotted with using the constrained layout, but in this case that will be turned off and tight layout used instead.
```

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__init__.py` & `hgutilities-1.0.5/hgutilities/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Animate.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Animate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Animate.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Animate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figure.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figure.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figure.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figures.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Figures.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figures.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Line.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Line.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Line.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Line.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Line.cpython-38.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Line.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Lines.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Lines.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Lines.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Lines.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Lines.cpython-38.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Lines.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plot.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plot.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plot.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plot.cpython-38.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plot.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotAxes.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotAxes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotAxes.cpython-38.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotAxes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotFunctions.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotFunctions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotFunctions.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotFunctions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotShape.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotShape.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotShape.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotShape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotShape.cpython-38.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotShape.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotUtils.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotUtils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/PlotUtils.cpython-38.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotUtils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plots.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plots.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plots.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plots.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/Plots.cpython-38.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plots.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/__init__.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/animate.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/animate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/figure.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/figure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/figures.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/figures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/animate.py` & `hgutilities-1.0.5/hgutilities/plotting/animate.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Line.txt` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Line.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/Default Settings/Surface.txt` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Surface.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Bar.txt` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Bar.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,11 +4,10 @@
 supported, and the key-word arguments are the same. Care must be
 taken to enter the key-word arguments in relevant object (Bars
 properties not entered into Bar properties and vice versa).
 
 Bar.defaults shows a list of optional kwargs.
 
 For further documentation see the following:
-Bars, Data, and Figures classes
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
 https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
```

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Bars.txt` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Bars.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 This is a subclass of Data used to create bar charts.
 It takes in a bar object, or an iterable of bar objects,
-and key-word arguments thar are relevant only to the entire
+and keyword arguments thar are relevant only to the entire
 plot. If you wanted every data series to be the same color,
 you would need to specify that for each bar object, but if
 you wanted a log scale, you would specify that at this level.
 If it does not make sense for two distinct data series to
 have different values for a property, then it should be a
 property of this object. For more detail, look at the
 default values for Bars and Bar objects.
 
 Bars.defaults shows a list of optional kwargs.
 
 For further documentation see the following:
 Bar, Data, and Figures classes
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
 https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
```

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Data.txt` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Data.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 axis labels and settings, and anything else relevant
 to the entire plot should be specified at this level.
 
 Data.defaults shows a list of optional kwargs.
 
 For further documentation see the following:
 Subclasses (see above) and Figures classes
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Line.txt` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Line.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 should be specified here.If a line is given a label
 then this label will be used in the chart legend.
 
 Line.defaults shows a list of optional kwargs.
 
 For further documentation see the following:
 Lines, Data, and Figures classes
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
 https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
```

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Lines.txt` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Lines.txt`

 * *Files 18% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 given for any line object, this will not be detected. The keyword
 plot_type="errorbar" needs to be passed in explicitily.
 
 lines.defaults shows a list of optional kwargs.
 
 For further documentation see the following:
 Line, Data, and Figures classes
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
 https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
```

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Pie.txt` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Pie.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 This is a Data subclass used to create pie charts. A pie chart can only
 display one data series, and so this takes in a list of values and
 labels directly unlike the Lines and Bars classes. Almost all
-matplotlib pie chart key-word arguments are accepted, and information
+matplotlib pie chart keyword arguments are accepted, and information
 about the plot legend should also be passed in, either upon creation
 or set directly.
 
 Pie.defaults shows a list of optional kwargs.
 
 For further documentation see the following:
 Data and Figures classes
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
 https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.pie.html
```

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/Documentation/Surface.txt` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Surface.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-This is a Data subclass used to create surfaces in 3D. It takes in x, y, and z values, all of which are 2D arrays of the same shape. Only one data series can be shown on each plot. All key-word arguments are the same as the matplotlib key-word arguments except for vmin and vmax which are defined in terms of a length 2 list called z_limits. This accepts the following arguments for the plot_type key-word, all of which are the names of the corresponding matplotlib plotting function. They are briefly described below:
+This is a Data subclass used to create surfaces in 3D. It takes in x, y, and z values, all of which are 2D arrays of the same shape. Only one data series can be shown on each plot. All keyword arguments are the same as the matplotlib keyword arguments. This accepts the following arguments for the plot_type keyword, all of which are the names of the corresponding matplotlib plotting function:
 
 plot_surface: standard surface plotter
 plot_wireframe: shows the surface as a wire frame
 contour: shows the level sets of a function
 
 Surface.defaults shows a list of optional kwargs.
 
 For further documentation see the following:
 Data and Figures classes
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
 https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.plot_surface.html
```

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Colorplot.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Colorplot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Data.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Data.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Line.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Line.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Line.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Line.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/bars.py` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/bars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/colorplot.py` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/colorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/lines.py` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/lines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/datatypes/surface.py` & `hgutilities-1.0.5/hgutilities/plotting/datatypes/surface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/figure.py` & `hgutilities-1.0.5/hgutilities/plotting/figure.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/figures.py` & `hgutilities-1.0.5/hgutilities/plotting/figures.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotColorplot.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotColorplot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/plot.py` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/plot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/plotbars.py` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/plotbars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/plotcolorplot.py` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/plotcolorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/plotlines.py` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/plotlines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/plotpie.py` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/plotpie.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plottypes/plotsurface.py` & `hgutilities-1.0.5/hgutilities/plotting/plottypes/plotsurface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/PlotShape.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/PlotShape.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/figuresize.py` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/figuresize.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/griddimensions.py` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/griddimensions.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/plotshape.py` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/plotshape.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/plotting/plotutils/savefigure.py` & `hgutilities-1.0.5/hgutilities/plotting/plotutils/savefigure.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/utils/__pycache__/Groups.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/utils/__pycache__/Groups.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/utils/__pycache__/Groups.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/utils/__pycache__/Groups.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/utils/__pycache__/Paths.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/utils/__pycache__/Paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/utils/__pycache__/Paths.cpython-311.pyc` & `hgutilities-1.0.5/hgutilities/utils/__pycache__/Paths.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/utils/__pycache__/groups.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/utils/__pycache__/groups.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/utils/__pycache__/paths.cpython-310.pyc` & `hgutilities-1.0.5/hgutilities/utils/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/utils/groups.py` & `hgutilities-1.0.5/hgutilities/utils/groups.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/utils/paths.py` & `hgutilities-1.0.5/hgutilities/utils/paths.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities/utils/plots.py` & `hgutilities-1.0.5/hgutilities/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.4/hgutilities.egg-info/PKG-INFO` & `hgutilities-1.0.5/hgutilities.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.4
+Version: 1.0.5
 Summary: A triple of tools used for plotting, handling key-words, and utilities
+Home-page: UNKNOWN
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
+License: UNKNOWN
 Keywords: python,matplotlib,plotting,default,keywords,utils
-Classifier: Development Status :: 1 - Planning
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
 # HGUtilities
@@ -36,40 +41,40 @@
 
 - To view all the defaults you need to go into the script itself
 - It is awkward to change the value of those variables from an interface
 - It is impossible to change the default values without digging into the code itself.
 - Passing in many arguments to functions is messy
 - Mutable default values need to be implemented more carefully
 
-Normally there are two ways of handling key word arguments with default values.The simpler way is to have the key word in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several key word arguemnts, this becomes messy however, and it would be preferred to pack the key words together with **kwargs. With this second method, there will need to be code that detects if a key word is in the **kwargs dict, and if so change it. This means we have a method for every key word argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the key word arguments a function takes in.
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
 
-In the second case, we cannot see what key word arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
 
 ### The Solution
 
 For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
 
-Whenever a method takes in key word arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any key word arguments that were not in the list of defaults, the file will be opened and overwritten with the new key word arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
 
     from hgutilities import defaults
 
     class MyClass():
 
         def __init__(self, **kwargs):
             defaults.kwargs(self, **kwargs)
 
     defaults.load(MyClass)
 
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such key word arguments should be set to `null` in the json file of defaults.
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
 
 The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
 
 ## Plotting
 
-For full documentation, see the specific README inside the "Plotting" module folder.
+For full documentation, see the specific README inside the "plotting" module folder.
 
 When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
 
 The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
 
 It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
 
@@ -85,7 +90,10 @@
 - more control over subplot placement
 - automatic paragraph organisation for documentation
 - better distribution of subplots over multiple figures
 - control over tick labels
 - horizontal bar charts
 - better file extension handling for Defaults package
 - inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
+- add README to defaults subpackage
+
```

### Comparing `hgutilities-1.0.4/hgutilities.egg-info/SOURCES.txt` & `hgutilities-1.0.5/hgutilities.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 hgutilities/__init__.py
 hgutilities.egg-info/PKG-INFO
 hgutilities.egg-info/SOURCES.txt
 hgutilities.egg-info/dependency_links.txt
 hgutilities.egg-info/requires.txt
 hgutilities.egg-info/top_level.txt
 hgutilities/Documentation/__init__.py
+hgutilities/Documentation/hgutilities.txt
 hgutilities/__pycache__/TesterProgram2.cpython-310.pyc
 hgutilities/__pycache__/TesterProgram2.cpython-311.pyc
 hgutilities/__pycache__/__init__.cpython-310.pyc
 hgutilities/defaults/__init__.py
 hgutilities/defaults/docs.py
 hgutilities/defaults/inherit.py
 hgutilities/defaults/loaddefaults.py
```

### Comparing `hgutilities-1.0.4/setup.py` & `hgutilities-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.4"
+VERSION = "1.0.5"
 DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
 LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
                     "Plotting: a front end for matplotlib to easily create subplots.\n"
                     "Utils: a collection of generally useful functions")
 
 # Setting up
 setup(
@@ -23,14 +23,16 @@
     long_description_content_type="text/markdown",
     long_description=long_description,
     setup_requires=['setuptools_scm'],
     include_package_data=True,
     install_requires=["matplotlib", "numpy", "screeninfo", "pillow"],
     keywords=["python", "matplotlib", "plotting", "default", "keywords", "utils"],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Natural Language :: English",
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

