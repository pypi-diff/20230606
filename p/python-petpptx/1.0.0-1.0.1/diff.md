# Comparing `tmp/python-petpptx-1.0.0.tar.gz` & `tmp/python-petpptx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-petpptx-1.0.0.tar", last modified: Tue Jun  6 11:07:07 2023, max compression
+gzip compressed data, was "python-petpptx-1.0.1.tar", last modified: Tue Jun  6 12:01:48 2023, max compression
```

## Comparing `python-petpptx-1.0.0.tar` & `python-petpptx-1.0.1.tar`

### file list

```diff
@@ -1,563 +1,563 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.340761 python-petpptx-1.0.0/
--rw-rw-rw-   0        0        0    16106 2023-06-06 11:06:14.000000 python-petpptx-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1124 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      182 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    19461 2023-06-06 11:07:07.340761 python-petpptx-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1155 2023-06-06 11:06:14.000000 python-petpptx-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.359864 python-petpptx-1.0.0/features/
--rw-rw-rw-   0        0        0     3303 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/act-action.feature
--rw-rw-rw-   0        0        0     2098 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/act-hyperlink.feature
--rw-rw-rw-   0        0        0     6576 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-axis-props.feature
--rw-rw-rw-   0        0        0     1404 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-axistitle-props.feature
--rw-rw-rw-   0        0        0     2131 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-category-access.feature
--rw-rw-rw-   0        0        0      593 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-category-props.feature
--rw-rw-rw-   0        0        0     4335 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-chart.feature
--rw-rw-rw-   0        0        0     1418 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-charttitle-props.feature
--rw-rw-rw-   0        0        0     4748 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-data-props.feature
--rw-rw-rw-   0        0        0     7143 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-datalabels.feature
--rw-rw-rw-   0        0        0      417 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-gridlines-props.feature
--rw-rw-rw-   0        0        0     1065 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-legend-access.feature
--rw-rw-rw-   0        0        0     3267 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-legend-props.feature
--rw-rw-rw-   0        0        0     1824 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-marker-props.feature
--rw-rw-rw-   0        0        0     4444 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-plot-props.feature
--rw-rw-rw-   0        0        0      982 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-point-access.feature
--rw-rw-rw-   0        0        0      587 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-point-props.feature
--rw-rw-rw-   0        0        0     1511 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-replace-data.feature
--rw-rw-rw-   0        0        0     4792 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-series.feature
--rw-rw-rw-   0        0        0      998 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/cht-ticklabels-props.feature
--rw-rw-rw-   0        0        0      709 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/dml-color.feature
--rw-rw-rw-   0        0        0     1047 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/dml-effect.feature
--rw-rw-rw-   0        0        0     3204 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/dml-fill.feature
--rw-rw-rw-   0        0        0     2225 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/dml-line.feature
--rw-rw-rw-   0        0        0      542 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/environment.py
--rw-rw-rw-   0        0        0     1635 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/ph-inherit-props.feature
--rw-rw-rw-   0        0        0     1424 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/ph-insert-shape.feature
--rw-rw-rw-   0        0        0      840 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/ph-phfmt-props.feature
--rw-rw-rw-   0        0        0     1480 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/ph-placeholder-props.feature
--rw-rw-rw-   0        0        0     1012 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/prs-coreprops.feature
--rw-rw-rw-   0        0        0      475 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/prs-default-template.feature
--rw-rw-rw-   0        0        0     1452 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/prs-open-save.feature
--rw-rw-rw-   0        0        0     1172 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/prs-presentation-props.feature
--rw-rw-rw-   0        0        0      787 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/shp-autoshape.feature
--rw-rw-rw-   0        0        0     2803 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/shp-connector.feature
--rw-rw-rw-   0        0        0     2290 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/shp-freeform.feature
--rw-rw-rw-   0        0        0     1672 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/shp-graphicframe.feature
--rw-rw-rw-   0        0        0     1399 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/shp-groupshape.feature
--rw-rw-rw-   0        0        0      592 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/shp-movie-props.feature
--rw-rw-rw-   0        0        0     2548 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/shp-picture.feature
--rw-rw-rw-   0        0        0      628 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/shp-placeholder.feature
--rw-rw-rw-   0        0        0    14465 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/shp-shapes.feature
--rw-rw-rw-   0        0        0     6450 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/shp-shared.feature
--rw-rw-rw-   0        0        0      503 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/sld-background.feature
--rw-rw-rw-   0        0        0     4223 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/sld-slide.feature
--rw-rw-rw-   0        0        0     2417 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/sld-slides.feature
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.427987 python-petpptx-1.0.0/features/steps/
--rw-rw-rw-   0        0        0     3424 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/action.py
--rw-rw-rw-   0        0        0    11709 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/axis.py
--rw-rw-rw-   0        0        0     1049 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/background.py
--rw-rw-rw-   0        0        0     6174 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/category.py
--rw-rw-rw-   0        0        0    14266 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/chart.py
--rw-rw-rw-   0        0        0     7556 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/chartdata.py
--rw-rw-rw-   0        0        0     2188 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/color.py
--rw-rw-rw-   0        0        0     2835 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/coreprops.py
--rw-rw-rw-   0        0        0     8296 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/datalabel.py
--rw-rw-rw-   0        0        0     1212 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/effect.py
--rw-rw-rw-   0        0        0     5311 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/fill.py
--rw-rw-rw-   0        0        0     5136 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/font.py
--rw-rw-rw-   0        0        0     3473 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/font_color.py
--rw-rw-rw-   0        0        0     1590 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/helpers.py
--rw-rw-rw-   0        0        0     3240 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/legend.py
--rw-rw-rw-   0        0        0     3348 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/line.py
--rw-rw-rw-   0        0        0     2883 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/picture.py
--rw-rw-rw-   0        0        0    11499 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/placeholder.py
--rw-rw-rw-   0        0        0     4950 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/plot.py
--rw-rw-rw-   0        0        0     6237 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/presentation.py
--rw-rw-rw-   0        0        0    12689 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/series.py
--rw-rw-rw-   0        0        0    23072 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/shape.py
--rw-rw-rw-   0        0        0    12457 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/shapes.py
--rw-rw-rw-   0        0        0     7786 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/slide.py
--rw-rw-rw-   0        0        0     4790 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/slides.py
--rw-rw-rw-   0        0        0    10603 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/table.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.610766 python-petpptx-1.0.0/features/steps/test_files/
--rw-rw-rw-   0        0        0     9454 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/72-dpi.tiff
--rw-rw-rw-   0        0        0     1526 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/CVS_LOGO.WMF
--rw-rw-rw-   0        0        0   982098 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/act-props.pptm
--rw-rw-rw-   0        0        0   867288 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/calibriz.ttf
--rw-rw-rw-   0        0        0   366536 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-axis-props.pptx
--rw-rw-rw-   0        0        0   222711 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-category-access.pptx
--rw-rw-rw-   0        0        0   218303 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-chart-props.pptx
--rw-rw-rw-   0        0        0  1393564 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-chart-type.pptx
--rw-rw-rw-   0        0        0    77751 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-charts.pptx
--rw-rw-rw-   0        0        0   243765 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-datalabels.pptx
--rw-rw-rw-   0        0        0    62864 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-gridlines-props.pptx
--rw-rw-rw-   0        0        0   145467 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-legend-props.pptx
--rw-rw-rw-   0        0        0   125134 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-legend.pptx
--rw-rw-rw-   0        0        0    78544 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-marker-props.pptx
--rw-rw-rw-   0        0        0   214116 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-plot-props.pptx
--rw-rw-rw-   0        0        0   145108 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-point-access.pptx
--rw-rw-rw-   0        0        0   144812 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-point-props.pptx
--rw-rw-rw-   0        0        0   323685 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-replace-data.pptx
--rw-rw-rw-   0        0        0   518464 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-series.pptx
--rw-rw-rw-   0        0        0   127056 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/cht-ticklabels-props.pptx
--rw-rw-rw-   0        0        0    21620 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/dml-effect.pptx
--rw-rw-rw-   0        0        0   778084 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/dml-fill.pptx
--rw-rw-rw-   0        0        0    27246 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/dml-line.pptx
--rw-rw-rw-   0        0        0    21457 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/ext-rels.pptx
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.610766 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/
--rw-rw-rw-   0        0        0     3359 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/[Content_Types].xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.610766 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/_rels/
--rw-rw-rw-   0        0        0      758 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/_rels/.rels
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.626394 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/docProps/
--rw-rw-rw-   0        0        0     1398 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/docProps/app.xml
--rw-rw-rw-   0        0        0      778 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/docProps/core.xml
--rw-rw-rw-   0        0        0     8147 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.626394 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.640407 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/_rels/
--rw-rw-rw-   0        0        0     1170 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels
--rw-rw-rw-   0        0        0      703 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/presProps.xml
--rw-rw-rw-   0        0        0     4106 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/presentation.xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.642417 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/printerSettings/
--rw-rw-rw-   0        0        0     9395 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.658055 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.673679 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
--rw-rw-rw-   0        0        0     7413 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml
--rw-rw-rw-   0        0        0     4781 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml
--rw-rw-rw-   0        0        0     5129 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml
--rw-rw-rw-   0        0        0     4726 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml
--rw-rw-rw-   0        0        0     7553 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml
--rw-rw-rw-   0        0        0     8094 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml
--rw-rw-rw-   0        0        0    12441 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml
--rw-rw-rw-   0        0        0     3311 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml
--rw-rw-rw-   0        0        0     2697 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml
--rw-rw-rw-   0        0        0     8040 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml
--rw-rw-rw-   0        0        0     7573 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.673679 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideMasters/
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.673679 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/
--rw-rw-rw-   0        0        0     2043 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
--rw-rw-rw-   0        0        0    17841 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.673679 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slides/
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.689306 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slides/_rels/
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slides/_rels/slide1.xml.rels
--rw-rw-rw-   0        0        0     2202 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml
--rw-rw-rw-   0        0        0      184 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/tableStyles.xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.689306 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/theme/
--rw-rw-rw-   0        0        0    10294 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml
--rw-rw-rw-   0        0        0     1054 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/viewProps.xml
--rw-rw-rw-   0        0        0    25061 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/font-color.pptx
--rw-rw-rw-   0        0        0   470987 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/just-two-mice.mp4
--rw-rw-rw-   0        0        0   179346 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/just-two-mice.png
--rw-rw-rw-   0        0        0    23202 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/lyt-shapes.pptx
--rw-rw-rw-   0        0        0    15802 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/minimal.pptx
--rw-rw-rw-   0        0        0    64276 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/monty-truth.png
--rw-rw-rw-   0        0        0    25251 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/mst-placeholders.pptx
--rw-rw-rw-   0        0        0    25539 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/mst-shapes.pptx
--rw-rw-rw-   0        0        0    21166 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/mst-slide-layouts.pptx
--rw-rw-rw-   0        0        0    23566 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/ph-inherit-props.pptx
--rw-rw-rw-   0        0        0   172254 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/ph-populated-placeholders.pptx
--rw-rw-rw-   0        0        0    34405 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/ph-unpopulated-placeholders.pptx
--rw-rw-rw-   0        0        0    49704 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/pic.emf
--rw-rw-rw-   0        0        0    19655 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/prs-add-slide.pptx
--rw-rw-rw-   0        0        0    86792 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/prs-notes.pptx
--rw-rw-rw-   0        0        0    15806 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/prs-properties.pptx
--rw-rw-rw-   0        0        0    21528 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/prs-slide-masters.pptx
--rw-rw-rw-   0        0        0     3277 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/python-icon.jpeg
--rw-rw-rw-   0        0        0     6111 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/python-powered.png
--rw-rw-rw-   0        0        0    45210 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/python.bmp
--rw-rw-rw-   0        0        0    80038 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-access-chart.pptx
--rw-rw-rw-   0        0        0   119022 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-access-ole-object.pptx
--rw-rw-rw-   0        0        0    17626 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-autoshape-adjustments.pptx
--rw-rw-rw-   0        0        0    22929 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-autoshape-props.pptx
--rw-rw-rw-   0        0        0    81639 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-common-props.pptx
--rw-rw-rw-   0        0        0    22899 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-connector-props.pptx
--rw-rw-rw-   0        0        0    11680 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-embedded-docx.docx
--rw-rw-rw-   0        0        0    29214 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-embedded-pptx.pptx
--rw-rw-rw-   0        0        0     8250 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-embedded-xlsx.xlsx
--rw-rw-rw-   0        0        0    16704 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-freeform.pptx
--rw-rw-rw-   0        0        0    23786 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-groupshape.pptx
--rw-rw-rw-   0        0        0   684874 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-movie-props.pptx
--rw-rw-rw-   0        0        0    91730 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-picture.pptx
--rw-rw-rw-   0        0        0    94116 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-pos-and-size.pptx
--rw-rw-rw-   0        0        0   125205 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/shp-shapes.pptx
--rw-rw-rw-   0        0        0    17676 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/sld-background.pptx
--rw-rw-rw-   0        0        0    16703 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/sld-blank.pptx
--rw-rw-rw-   0        0        0    22964 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/sld-notes.pptx
--rw-rw-rw-   0        0        0    18894 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/sld-slide.pptx
--rw-rw-rw-   0        0        0    18478 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/sld-slides.pptx
--rw-rw-rw-   0        0        0    33273 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/sonic.gif
--rw-rw-rw-   0        0        0    28247 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/tbl-cell.pptx
--rw-rw-rw-   0        0        0    37859 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/test.pptx
--rw-rw-rw-   0        0        0    21337 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/txt-fit-text.pptx
--rw-rw-rw-   0        0        0    18874 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/txt-font-props.pptx
--rw-rw-rw-   0        0        0    25817 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/txt-font-typeface.pptx
--rw-rw-rw-   0        0        0    24620 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/txt-paragraph-spacing.pptx
--rw-rw-rw-   0        0        0    27659 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/txt-text-frame.pptx
--rw-rw-rw-   0        0        0    16051 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/test_files/txt-text.pptx
--rw-rw-rw-   0        0        0     8520 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/text.py
--rw-rw-rw-   0        0        0     4749 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/steps/text_frame.py
--rw-rw-rw-   0        0        0     3662 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/tbl-cell.feature
--rw-rw-rw-   0        0        0      353 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/tbl-column.feature
--rw-rw-rw-   0        0        0     1625 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/tbl-table.feature
--rw-rw-rw-   0        0        0      482 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/txt-fit-text.feature
--rw-rw-rw-   0        0        0     1788 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/txt-font-color.feature
--rw-rw-rw-   0        0        0     5094 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/txt-font-props.feature
--rw-rw-rw-   0        0        0     4064 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/txt-paragraph.feature
--rw-rw-rw-   0        0        0      757 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/txt-text.feature
--rw-rw-rw-   0        0        0     2446 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/features/txt-textframe.feature
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.704946 python-petpptx-1.0.0/pptx/
--rw-rw-rw-   0        0        0     2047 2023-06-06 11:06:14.000000 python-petpptx-1.0.0/pptx/__init__.py
--rw-rw-rw-   0        0        0     8922 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/action.py
--rw-rw-rw-   0        0        0     1644 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/api.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.721068 python-petpptx-1.0.0/pptx/chart/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/__init__.py
--rw-rw-rw-   0        0        0    17827 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/axis.py
--rw-rw-rw-   0        0        0     7452 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/category.py
--rw-rw-rw-   0        0        0    10283 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/chart.py
--rw-rw-rw-   0        0        0    30605 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/data.py
--rw-rw-rw-   0        0        0     9820 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/datalabel.py
--rw-rw-rw-   0        0        0     2649 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/legend.py
--rw-rw-rw-   0        0        0     2202 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/marker.py
--rw-rw-rw-   0        0        0    13629 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/plot.py
--rw-rw-rw-   0        0        0     2899 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/point.py
--rw-rw-rw-   0        0        0     7745 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/series.py
--rw-rw-rw-   0        0        0    11223 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/xlsx.py
--rw-rw-rw-   0        0        0    69538 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/chart/xmlwriter.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.740599 python-petpptx-1.0.0/pptx/compat/
--rw-rw-rw-   0        0        0      738 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/compat/__init__.py
--rw-rw-rw-   0        0        0     1343 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/compat/python2.py
--rw-rw-rw-   0        0        0      963 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/compat/python3.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.740599 python-petpptx-1.0.0/pptx/dml/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/dml/__init__.py
--rw-rw-rw-   0        0        0     1415 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/dml/chtfmt.py
--rw-rw-rw-   0        0        0     9429 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/dml/color.py
--rw-rw-rw-   0        0        0     1635 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/dml/effect.py
--rw-rw-rw-   0        0        0    13637 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/dml/fill.py
--rw-rw-rw-   0        0        0     3210 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/dml/line.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.752613 python-petpptx-1.0.0/pptx/enum/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/enum/__init__.py
--rw-rw-rw-   0        0        0     1594 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/enum/action.py
--rw-rw-rw-   0        0        0    11061 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/enum/base.py
--rw-rw-rw-   0        0        0    13589 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/enum/chart.py
--rw-rw-rw-   0        0        0    12259 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/enum/dml.py
--rw-rw-rw-   0        0        0    23308 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/enum/lang.py
--rw-rw-rw-   0        0        0    32343 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/enum/shapes.py
--rw-rw-rw-   0        0        0     8470 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/enum/text.py
--rw-rw-rw-   0        0        0      481 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/exc.py
--rw-rw-rw-   0        0        0    10731 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/media.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.768257 python-petpptx-1.0.0/pptx/opc/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/opc/__init__.py
--rw-rw-rw-   0        0        0    20491 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/opc/constants.py
--rw-rw-rw-   0        0        0     4667 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/opc/oxml.py
--rw-rw-rw-   0        0        0    27711 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/opc/package.py
--rw-rw-rw-   0        0        0     3996 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/opc/packuri.py
--rw-rw-rw-   0        0        0    10248 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/opc/serialized.py
--rw-rw-rw-   0        0        0      712 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/opc/shared.py
--rw-rw-rw-   0        0        0     1061 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/opc/spec.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.799509 python-petpptx-1.0.0/pptx/oxml/
--rw-rw-rw-   0        0        0    15938 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/__init__.py
--rw-rw-rw-   0        0        0     1663 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/action.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.818180 python-petpptx-1.0.0/pptx/oxml/chart/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/chart/__init__.py
--rw-rw-rw-   0        0        0     9727 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/chart/axis.py
--rw-rw-rw-   0        0        0     8478 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/chart/chart.py
--rw-rw-rw-   0        0        0     8019 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/chart/datalabel.py
--rw-rw-rw-   0        0        0     2205 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/chart/legend.py
--rw-rw-rw-   0        0        0     1903 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/chart/marker.py
--rw-rw-rw-   0        0        0     9573 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/chart/plot.py
--rw-rw-rw-   0        0        0     7883 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/chart/series.py
--rw-rw-rw-   0        0        0     6321 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/chart/shared.py
--rw-rw-rw-   0        0        0    10114 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/coreprops.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.818180 python-petpptx-1.0.0/pptx/oxml/dml/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/dml/__init__.py
--rw-rw-rw-   0        0        0     2592 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/dml/color.py
--rw-rw-rw-   0        0        0     6186 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/dml/fill.py
--rw-rw-rw-   0        0        0      460 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/dml/line.py
--rw-rw-rw-   0        0        0     4809 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/ns.py
--rw-rw-rw-   0        0        0     2890 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/presentation.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.840656 python-petpptx-1.0.0/pptx/oxml/shapes/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/shapes/__init__.py
--rw-rw-rw-   0        0        0    13857 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/shapes/autoshape.py
--rw-rw-rw-   0        0        0     3633 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/shapes/connector.py
--rw-rw-rw-   0        0        0    12391 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/shapes/graphfrm.py
--rw-rw-rw-   0        0        0     9492 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/shapes/groupshape.py
--rw-rw-rw-   0        0        0     8353 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/shapes/picture.py
--rw-rw-rw-   0        0        0    13199 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/shapes/shared.py
--rw-rw-rw-   0        0        0    20684 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/simpletypes.py
--rw-rw-rw-   0        0        0    10558 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/slide.py
--rw-rw-rw-   0        0        0    18865 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/table.py
--rw-rw-rw-   0        0        0    17016 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/text.py
--rw-rw-rw-   0        0        0      787 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/theme.py
--rw-rw-rw-   0        0        0    25824 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/oxml/xmlchemy.py
--rw-rw-rw-   0        0        0     7846 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/package.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.851171 python-petpptx-1.0.0/pptx/parts/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/parts/__init__.py
--rw-rw-rw-   0        0        0     3091 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/parts/chart.py
--rw-rw-rw-   0        0        0     4213 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/parts/coreprops.py
--rw-rw-rw-   0        0        0     2903 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/parts/embeddedpackage.py
--rw-rw-rw-   0        0        0     9327 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/parts/image.py
--rw-rw-rw-   0        0        0      938 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/parts/media.py
--rw-rw-rw-   0        0        0     4598 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/parts/presentation.py
--rw-rw-rw-   0        0        0    10732 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/parts/slide.py
--rw-rw-rw-   0        0        0     3450 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/presentation.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.866807 python-petpptx-1.0.0/pptx/shapes/
--rw-rw-rw-   0        0        0      614 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shapes/__init__.py
--rw-rw-rw-   0        0        0    14103 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shapes/autoshape.py
--rw-rw-rw-   0        0        0     7826 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shapes/base.py
--rw-rw-rw-   0        0        0    10362 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shapes/connector.py
--rw-rw-rw-   0        0        0    11244 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shapes/freeform.py
--rw-rw-rw-   0        0        0     5150 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shapes/graphfrm.py
--rw-rw-rw-   0        0        0     1920 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shapes/group.py
--rw-rw-rw-   0        0        0     6848 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shapes/picture.py
--rw-rw-rw-   0        0        0    14942 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shapes/placeholder.py
--rw-rw-rw-   0        0        0    42499 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shapes/shapetree.py
--rw-rw-rw-   0        0        0     2680 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/shared.py
--rw-rw-rw-   0        0        0    18411 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/slide.py
--rw-rw-rw-   0        0        0    24203 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/spec.py
--rw-rw-rw-   0        0        0    16796 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/table.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.898059 python-petpptx-1.0.0/pptx/templates/
--rw-rw-rw-   0        0        0    34030 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/templates/default.pptx
--rw-rw-rw-   0        0        0   127228 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/templates/docx-icon.emf
--rw-rw-rw-   0        0        0     5396 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/templates/generic-icon.emf
--rw-rw-rw-   0        0        0      745 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/templates/notes.xml
--rw-rw-rw-   0        0        0    11487 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/templates/notesMaster.xml
--rw-rw-rw-   0        0        0     5492 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/templates/pptx-icon.emf
--rw-rw-rw-   0        0        0    11285 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/templates/theme.xml
--rw-rw-rw-   0        0        0   130380 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/templates/xlsx-icon.emf
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.898059 python-petpptx-1.0.0/pptx/text/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/text/__init__.py
--rw-rw-rw-   0        0        0    13308 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/text/fonts.py
--rw-rw-rw-   0        0        0    10277 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/text/layout.py
--rw-rw-rw-   0        0        0    25979 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/text/text.py
--rw-rw-rw-   0        0        0     8064 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/pptx/util.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.945079 python-petpptx-1.0.0/python_petpptx.egg-info/
--rw-rw-rw-   0        0        0    19461 2023-06-06 11:07:05.000000 python-petpptx-1.0.0/python_petpptx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18674 2023-06-06 11:07:06.000000 python-petpptx-1.0.0/python_petpptx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 11:07:05.000000 python-petpptx-1.0.0/python_petpptx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 09:50:40.000000 python-petpptx-1.0.0/python_petpptx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       44 2023-06-06 11:07:05.000000 python-petpptx-1.0.0/python_petpptx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-06 11:07:05.000000 python-petpptx-1.0.0/python_petpptx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 11:07:07.340761 python-petpptx-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2712 2023-06-06 09:50:34.000000 python-petpptx-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.960715 python-petpptx-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:06.991988 python-petpptx-1.0.0/tests/chart/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/__init__.py
--rw-rw-rw-   0        0        0    49601 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_axis.py
--rw-rw-rw-   0        0        0     9600 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_category.py
--rw-rw-rw-   0        0        0    21804 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_chart.py
--rw-rw-rw-   0        0        0    35047 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_data.py
--rw-rw-rw-   0        0        0    26881 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_datalabel.py
--rw-rw-rw-   0        0        0     6982 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_legend.py
--rw-rw-rw-   0        0        0     4967 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_marker.py
--rw-rw-rw-   0        0        0    19254 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_plot.py
--rw-rw-rw-   0        0        0     7888 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_point.py
--rw-rw-rw-   0        0        0    19624 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_series.py
--rw-rw-rw-   0        0        0    16373 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_xlsx.py
--rw-rw-rw-   0        0        0    29186 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/chart/test_xmlwriter.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.007601 python-petpptx-1.0.0/tests/dml/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/dml/__init__.py
--rw-rw-rw-   0        0        0     3326 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/dml/test_chtfmt.py
--rw-rw-rw-   0        0        0    11930 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/dml/test_color.py
--rw-rw-rw-   0        0        0     1979 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/dml/test_effect.py
--rw-rw-rw-   0        0        0    26377 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/dml/test_fill.py
--rw-rw-rw-   0        0        0     6140 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/dml/test_line.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.007601 python-petpptx-1.0.0/tests/opc/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/opc/__init__.py
--rw-rw-rw-   0        0        0     6642 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/opc/test_oxml.py
--rw-rw-rw-   0        0        0    39420 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/opc/test_package.py
--rw-rw-rw-   0        0        0     3072 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/opc/test_packuri.py
--rw-rw-rw-   0        0        0    15207 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/opc/test_serialized.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.027419 python-petpptx-1.0.0/tests/opc/unitdata/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/opc/unitdata/__init__.py
--rw-rw-rw-   0        0        0     7741 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/opc/unitdata/rels.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.040468 python-petpptx-1.0.0/tests/oxml/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.054988 python-petpptx-1.0.0/tests/oxml/shapes/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/shapes/__init__.py
--rw-rw-rw-   0        0        0    10284 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/shapes/test_autoshape.py
--rw-rw-rw-   0        0        0     3466 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/shapes/test_graphfrm.py
--rw-rw-rw-   0        0        0    11125 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/shapes/test_groupshape.py
--rw-rw-rw-   0        0        0     3698 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/shapes/test_picture.py
--rw-rw-rw-   0        0        0     3314 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/test___init__.py
--rw-rw-rw-   0        0        0     5215 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/test_dml.py
--rw-rw-rw-   0        0        0     2771 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/test_ns.py
--rw-rw-rw-   0        0        0     1482 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/test_presentation.py
--rw-rw-rw-   0        0        0     9267 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/test_simpletypes.py
--rw-rw-rw-   0        0        0      742 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/test_slide.py
--rw-rw-rw-   0        0        0    10390 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/test_table.py
--rw-rw-rw-   0        0        0      720 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/test_theme.py
--rw-rw-rw-   0        0        0    21508 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/test_xmlchemy.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.054988 python-petpptx-1.0.0/tests/oxml/unitdata/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/unitdata/__init__.py
--rw-rw-rw-   0        0        0     2052 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/unitdata/dml.py
--rw-rw-rw-   0        0        0     4275 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/unitdata/shape.py
--rw-rw-rw-   0        0        0     1881 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/oxml/unitdata/text.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.070629 python-petpptx-1.0.0/tests/parts/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/parts/__init__.py
--rw-rw-rw-   0        0        0     6130 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/parts/test_chart.py
--rw-rw-rw-   0        0        0     9305 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/parts/test_coreprops.py
--rw-rw-rw-   0        0        0     3087 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/parts/test_embeddedpackage.py
--rw-rw-rw-   0        0        0     8047 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/parts/test_image.py
--rw-rw-rw-   0        0        0     1218 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/parts/test_media.py
--rw-rw-rw-   0        0        0     9395 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/parts/test_presentation.py
--rw-rw-rw-   0        0        0    23166 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/parts/test_slide.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.086273 python-petpptx-1.0.0/tests/shapes/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/shapes/__init__.py
--rw-rw-rw-   0        0        0    19158 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/shapes/test_autoshape.py
--rw-rw-rw-   0        0        0    20302 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/shapes/test_base.py
--rw-rw-rw-   0        0        0    16664 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/shapes/test_connector.py
--rw-rw-rw-   0        0        0    21195 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/shapes/test_freeform.py
--rw-rw-rw-   0        0        0     6826 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/shapes/test_graphfrm.py
--rw-rw-rw-   0        0        0     2435 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/shapes/test_group.py
--rw-rw-rw-   0        0        0    10931 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/shapes/test_picture.py
--rw-rw-rw-   0        0        0    23006 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/shapes/test_placeholder.py
--rw-rw-rw-   0        0        0    89451 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/shapes/test_shapetree.py
--rw-rw-rw-   0        0        0    14348 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_action.py
--rw-rw-rw-   0        0        0     1580 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_api.py
--rw-rw-rw-   0        0        0     3859 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_enum.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.133307 python-petpptx-1.0.0/tests/test_files/
--rw-rw-rw-   0        0        0   867288 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/calibriz.ttf
--rw-rw-rw-   0        0        0    22238 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/cdw-logo.eps
--rw-rw-rw-   0        0        0       43 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/dummy.mp4
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.133307 python-petpptx-1.0.0/tests/test_files/expanded_pptx/
--rw-rw-rw-   0        0        0     3359 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/[Content_Types].xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.133307 python-petpptx-1.0.0/tests/test_files/expanded_pptx/_rels/
--rw-rw-rw-   0        0        0      758 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/_rels/.rels
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.140323 python-petpptx-1.0.0/tests/test_files/expanded_pptx/docProps/
--rw-rw-rw-   0        0        0     1354 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/docProps/app.xml
--rw-rw-rw-   0        0        0      750 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/docProps/core.xml
--rw-rw-rw-   0        0        0     8147 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.149336 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.149336 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/_rels/
--rw-rw-rw-   0        0        0     1170 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels
--rw-rw-rw-   0        0        0      327 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/presProps.xml
--rw-rw-rw-   0        0        0     4157 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/presentation.xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.149336 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/printerSettings/
--rw-rw-rw-   0        0        0     9395 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.164980 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.196226 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
--rw-rw-rw-   0        0        0     7473 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml
--rw-rw-rw-   0        0        0     4783 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml
--rw-rw-rw-   0        0        0     5131 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml
--rw-rw-rw-   0        0        0     4786 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml
--rw-rw-rw-   0        0        0     7613 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml
--rw-rw-rw-   0        0        0     8154 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml
--rw-rw-rw-   0        0        0    12501 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml
--rw-rw-rw-   0        0        0     3371 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml
--rw-rw-rw-   0        0        0     2757 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml
--rw-rw-rw-   0        0        0     8100 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml
--rw-rw-rw-   0        0        0     7633 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.196226 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideMasters/
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.196226 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/
--rw-rw-rw-   0        0        0     2093 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
--rw-rw-rw-   0        0        0    17871 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.196226 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slides/
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.196226 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slides/_rels/
--rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slides/_rels/slide1.xml.rels
--rw-rw-rw-   0        0        0     2198 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slides/slide1.xml
--rw-rw-rw-   0        0        0      182 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/tableStyles.xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.196226 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/theme/
--rw-rw-rw-   0        0        0    10294 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/theme/theme1.xml
--rw-rw-rw-   0        0        0     1081 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/viewProps.xml
--rw-rw-rw-   0        0        0    15802 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/minimal.pptx
--rw-rw-rw-   0        0        0      492 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/minimal_slide.xml
--rw-rw-rw-   0        0        0    32944 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/missing_rels_item.pptx
--rw-rw-rw-   0        0        0    64276 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/monty-truth.png
--rw-rw-rw-   0        0        0    34436 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/no-core-props.pptx
--rw-rw-rw-   0        0        0    34036 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/no-slides.pptx
--rw-rw-rw-   0        0        0     4157 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/presentation.xml
--rw-rw-rw-   0        0        0     3277 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/python-icon.jpeg
--rw-rw-rw-   0        0        0     6111 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/python-powered.png
--rw-rw-rw-   0        0        0    45210 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/python.bmp
--rw-rw-rw-   0        0        0     8134 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/slideLayout1.xml
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.318975 python-petpptx-1.0.0/tests/test_files/snippets/
--rw-rw-rw-   0        0        0     5086 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-area-date.txt
--rw-rw-rw-   0        0        0     5083 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-area-float.txt
--rw-rw-rw-   0        0        0     4981 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-area-stacked-100.txt
--rw-rw-rw-   0        0        0     4974 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-area-stacked.txt
--rw-rw-rw-   0        0        0     4975 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-area.txt
--rw-rw-rw-   0        0        0     4453 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-bar-clustered-date.txt
--rw-rw-rw-   0        0        0     4391 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-bar-clustered-float.txt
--rw-rw-rw-   0        0        0     4283 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-bar-clustered.txt
--rw-rw-rw-   0        0        0     4320 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-bar-stacked-100.txt
--rw-rw-rw-   0        0        0     4313 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-bar-stacked.txt
--rw-rw-rw-   0        0        0     4283 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-column-clustered.txt
--rw-rw-rw-   0        0        0     4320 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-column-stacked-100.txt
--rw-rw-rw-   0        0        0     4313 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-column-stacked.txt
--rw-rw-rw-   0        0        0     4907 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-date.txt
--rw-rw-rw-   0        0        0     4845 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-float.txt
--rw-rw-rw-   0        0        0     4581 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-markers-stacked-100.txt
--rw-rw-rw-   0        0        0     4574 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-markers-stacked.txt
--rw-rw-rw-   0        0        0     4575 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-markers.txt
--rw-rw-rw-   0        0        0     4743 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-stacked-100.txt
--rw-rw-rw-   0        0        0     4736 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-stacked.txt
--rw-rw-rw-   0        0        0     4737 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x2-line.txt
--rw-rw-rw-   0        0        0     6655 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x3-bubble-3d.txt
--rw-rw-rw-   0        0        0     6655 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x3-bubble.txt
--rw-rw-rw-   0        0        0     5254 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x3-xy-lines-no-markers.txt
--rw-rw-rw-   0        0        0     5092 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x3-xy-lines.txt
--rw-rw-rw-   0        0        0     5256 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt
--rw-rw-rw-   0        0        0     5094 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x3-xy-smooth.txt
--rw-rw-rw-   0        0        0     5330 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x3-xy.txt
--rw-rw-rw-   0        0        0     6307 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/2x5-radar.txt
--rw-rw-rw-   0        0        0     2180 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/3x1-pie-exploded.txt
--rw-rw-rw-   0        0        0     2145 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/3x1-pie.txt
--rw-rw-rw-   0        0        0     4286 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/3x2-doughnut-exploded.txt
--rw-rw-rw-   0        0        0     4216 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/3x2-doughnut.txt
--rw-rw-rw-   0        0        0     5517 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/4x2-multi-cat-bar.txt
--rw-rw-rw-   0        0        0     3615 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/adjust-ser-count.txt
--rw-rw-rw-   0        0        0     3782 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/cat-labels.txt
--rw-rw-rw-   0        0        0      526 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/content-types-xml.txt
--rw-rw-rw-   0        0        0      688 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/default-notes.txt
--rw-rw-rw-   0        0        0    11409 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/default-notesMaster.txt
--rw-rw-rw-   0        0        0    11213 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/default-theme.txt
--rw-rw-rw-   0        0        0     1131 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/freeform.txt
--rw-rw-rw-   0        0        0      764 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/package-rels-xml.txt
--rw-rw-rw-   0        0        0     1817 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/placeholders.txt
--rw-rw-rw-   0        0        0      606 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/presentation-rels-xml.txt
--rw-rw-rw-   0        0        0      447 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/relationships.txt
--rw-rw-rw-   0        0        0      628 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/rels-load-from-xml.txt
--rw-rw-rw-   0        0        0    11033 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/rewrite-ser.txt
--rw-rw-rw-   0        0        0     2893 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/snippets/timing.txt
--rw-rw-rw-   0        0        0    37859 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/test.pptx
--rw-rw-rw-   0        0        0    38616 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_files/test_slides.pptx
--rw-rw-rw-   0        0        0     4740 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_media.py
--rw-rw-rw-   0        0        0    13882 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_package.py
--rw-rw-rw-   0        0        0     9170 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_presentation.py
--rw-rw-rw-   0        0        0     2538 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_shared.py
--rw-rw-rw-   0        0        0    40208 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_slide.py
--rw-rw-rw-   0        0        0    29977 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_table.py
--rw-rw-rw-   0        0        0     1941 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/test_util.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.322103 python-petpptx-1.0.0/tests/text/
--rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/text/__init__.py
--rw-rw-rw-   0        0        0    25932 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/text/test_fonts.py
--rw-rw-rw-   0        0        0     9269 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/text/test_layout.py
--rw-rw-rw-   0        0        0    46965 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/text/test_text.py
--rw-rw-rw-   0        0        0     3785 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/unitdata.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.337742 python-petpptx-1.0.0/tests/unitutil/
--rw-rw-rw-   0        0        0      262 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/unitutil/__init__.py
--rw-rw-rw-   0        0        0     8597 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/unitutil/cxml.py
--rw-rw-rw-   0        0        0     1919 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/unitutil/file.py
--rw-rw-rw-   0        0        0     4243 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tests/unitutil/mock.py
--rw-rw-rw-   0        0        0      689 2023-06-06 09:05:39.000000 python-petpptx-1.0.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.903262 python-petpptx-1.0.1/
+-rw-rw-rw-   0        0        0    16233 2023-06-06 12:01:11.000000 python-petpptx-1.0.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1124 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      182 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    19588 2023-06-06 12:01:48.903262 python-petpptx-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1155 2023-06-06 11:06:14.000000 python-petpptx-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:47.978806 python-petpptx-1.0.1/features/
+-rw-rw-rw-   0        0        0     3303 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/act-action.feature
+-rw-rw-rw-   0        0        0     2098 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/act-hyperlink.feature
+-rw-rw-rw-   0        0        0     6576 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-axis-props.feature
+-rw-rw-rw-   0        0        0     1404 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-axistitle-props.feature
+-rw-rw-rw-   0        0        0     2131 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-category-access.feature
+-rw-rw-rw-   0        0        0      593 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-category-props.feature
+-rw-rw-rw-   0        0        0     4335 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-chart.feature
+-rw-rw-rw-   0        0        0     1418 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-charttitle-props.feature
+-rw-rw-rw-   0        0        0     4748 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-data-props.feature
+-rw-rw-rw-   0        0        0     7143 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-datalabels.feature
+-rw-rw-rw-   0        0        0      417 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-gridlines-props.feature
+-rw-rw-rw-   0        0        0     1065 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-legend-access.feature
+-rw-rw-rw-   0        0        0     3267 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-legend-props.feature
+-rw-rw-rw-   0        0        0     1824 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-marker-props.feature
+-rw-rw-rw-   0        0        0     4444 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-plot-props.feature
+-rw-rw-rw-   0        0        0      982 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-point-access.feature
+-rw-rw-rw-   0        0        0      587 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-point-props.feature
+-rw-rw-rw-   0        0        0     1511 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-replace-data.feature
+-rw-rw-rw-   0        0        0     4792 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-series.feature
+-rw-rw-rw-   0        0        0      998 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/cht-ticklabels-props.feature
+-rw-rw-rw-   0        0        0      709 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/dml-color.feature
+-rw-rw-rw-   0        0        0     1047 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/dml-effect.feature
+-rw-rw-rw-   0        0        0     3204 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/dml-fill.feature
+-rw-rw-rw-   0        0        0     2225 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/dml-line.feature
+-rw-rw-rw-   0        0        0      542 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/environment.py
+-rw-rw-rw-   0        0        0     1635 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/ph-inherit-props.feature
+-rw-rw-rw-   0        0        0     1424 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/ph-insert-shape.feature
+-rw-rw-rw-   0        0        0      840 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/ph-phfmt-props.feature
+-rw-rw-rw-   0        0        0     1480 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/ph-placeholder-props.feature
+-rw-rw-rw-   0        0        0     1012 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/prs-coreprops.feature
+-rw-rw-rw-   0        0        0      475 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/prs-default-template.feature
+-rw-rw-rw-   0        0        0     1452 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/prs-open-save.feature
+-rw-rw-rw-   0        0        0     1172 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/prs-presentation-props.feature
+-rw-rw-rw-   0        0        0      787 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/shp-autoshape.feature
+-rw-rw-rw-   0        0        0     2803 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/shp-connector.feature
+-rw-rw-rw-   0        0        0     2290 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/shp-freeform.feature
+-rw-rw-rw-   0        0        0     1672 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/shp-graphicframe.feature
+-rw-rw-rw-   0        0        0     1399 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/shp-groupshape.feature
+-rw-rw-rw-   0        0        0      592 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/shp-movie-props.feature
+-rw-rw-rw-   0        0        0     2548 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/shp-picture.feature
+-rw-rw-rw-   0        0        0      628 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/shp-placeholder.feature
+-rw-rw-rw-   0        0        0    14465 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/shp-shapes.feature
+-rw-rw-rw-   0        0        0     6450 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/shp-shared.feature
+-rw-rw-rw-   0        0        0      503 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/sld-background.feature
+-rw-rw-rw-   0        0        0     4223 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/sld-slide.feature
+-rw-rw-rw-   0        0        0     2417 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/sld-slides.feature
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.040639 python-petpptx-1.0.1/features/steps/
+-rw-rw-rw-   0        0        0     3424 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/action.py
+-rw-rw-rw-   0        0        0    11709 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/axis.py
+-rw-rw-rw-   0        0        0     1049 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/background.py
+-rw-rw-rw-   0        0        0     6174 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/category.py
+-rw-rw-rw-   0        0        0    14266 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/chart.py
+-rw-rw-rw-   0        0        0     7556 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/chartdata.py
+-rw-rw-rw-   0        0        0     2188 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/color.py
+-rw-rw-rw-   0        0        0     2835 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/coreprops.py
+-rw-rw-rw-   0        0        0     8296 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/datalabel.py
+-rw-rw-rw-   0        0        0     1212 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/effect.py
+-rw-rw-rw-   0        0        0     5311 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/fill.py
+-rw-rw-rw-   0        0        0     5136 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/font.py
+-rw-rw-rw-   0        0        0     3473 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/font_color.py
+-rw-rw-rw-   0        0        0     1590 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/helpers.py
+-rw-rw-rw-   0        0        0     3240 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/legend.py
+-rw-rw-rw-   0        0        0     3348 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/line.py
+-rw-rw-rw-   0        0        0     2883 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/picture.py
+-rw-rw-rw-   0        0        0    11499 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/placeholder.py
+-rw-rw-rw-   0        0        0     4950 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/plot.py
+-rw-rw-rw-   0        0        0     6237 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/presentation.py
+-rw-rw-rw-   0        0        0    12689 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/series.py
+-rw-rw-rw-   0        0        0    23072 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/shape.py
+-rw-rw-rw-   0        0        0    12457 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/shapes.py
+-rw-rw-rw-   0        0        0     7786 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/slide.py
+-rw-rw-rw-   0        0        0     4790 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/slides.py
+-rw-rw-rw-   0        0        0    10603 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/table.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.213397 python-petpptx-1.0.1/features/steps/test_files/
+-rw-rw-rw-   0        0        0     9454 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/72-dpi.tiff
+-rw-rw-rw-   0        0        0     1526 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/CVS_LOGO.WMF
+-rw-rw-rw-   0        0        0   982098 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/act-props.pptm
+-rw-rw-rw-   0        0        0   867288 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/calibriz.ttf
+-rw-rw-rw-   0        0        0   366536 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-axis-props.pptx
+-rw-rw-rw-   0        0        0   222711 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-category-access.pptx
+-rw-rw-rw-   0        0        0   218303 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-chart-props.pptx
+-rw-rw-rw-   0        0        0  1393564 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-chart-type.pptx
+-rw-rw-rw-   0        0        0    77751 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-charts.pptx
+-rw-rw-rw-   0        0        0   243765 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-datalabels.pptx
+-rw-rw-rw-   0        0        0    62864 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-gridlines-props.pptx
+-rw-rw-rw-   0        0        0   145467 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-legend-props.pptx
+-rw-rw-rw-   0        0        0   125134 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-legend.pptx
+-rw-rw-rw-   0        0        0    78544 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-marker-props.pptx
+-rw-rw-rw-   0        0        0   214116 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-plot-props.pptx
+-rw-rw-rw-   0        0        0   145108 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-point-access.pptx
+-rw-rw-rw-   0        0        0   144812 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-point-props.pptx
+-rw-rw-rw-   0        0        0   323685 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-replace-data.pptx
+-rw-rw-rw-   0        0        0   518464 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-series.pptx
+-rw-rw-rw-   0        0        0   127056 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/cht-ticklabels-props.pptx
+-rw-rw-rw-   0        0        0    21620 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/dml-effect.pptx
+-rw-rw-rw-   0        0        0   778084 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/dml-fill.pptx
+-rw-rw-rw-   0        0        0    27246 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/dml-line.pptx
+-rw-rw-rw-   0        0        0    21457 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/ext-rels.pptx
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.229035 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/
+-rw-rw-rw-   0        0        0     3359 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/[Content_Types].xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.229035 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/_rels/
+-rw-rw-rw-   0        0        0      758 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/_rels/.rels
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.229035 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/docProps/
+-rw-rw-rw-   0        0        0     1398 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/docProps/app.xml
+-rw-rw-rw-   0        0        0      778 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/docProps/core.xml
+-rw-rw-rw-   0        0        0     8147 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.229035 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.244668 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/_rels/
+-rw-rw-rw-   0        0        0     1170 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels
+-rw-rw-rw-   0        0        0      703 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/presProps.xml
+-rw-rw-rw-   0        0        0     4106 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/presentation.xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.244668 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/printerSettings/
+-rw-rw-rw-   0        0        0     9395 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.260286 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.275919 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
+-rw-rw-rw-   0        0        0     7413 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml
+-rw-rw-rw-   0        0        0     4781 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml
+-rw-rw-rw-   0        0        0     5129 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml
+-rw-rw-rw-   0        0        0     4726 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml
+-rw-rw-rw-   0        0        0     7553 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml
+-rw-rw-rw-   0        0        0     8094 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml
+-rw-rw-rw-   0        0        0    12441 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml
+-rw-rw-rw-   0        0        0     3311 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml
+-rw-rw-rw-   0        0        0     2697 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml
+-rw-rw-rw-   0        0        0     8040 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml
+-rw-rw-rw-   0        0        0     7573 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.291552 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.291552 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/
+-rw-rw-rw-   0        0        0     2043 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
+-rw-rw-rw-   0        0        0    17841 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.291552 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slides/
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.291552 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slides/_rels/
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slides/_rels/slide1.xml.rels
+-rw-rw-rw-   0        0        0     2202 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml
+-rw-rw-rw-   0        0        0      184 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/tableStyles.xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.291552 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/theme/
+-rw-rw-rw-   0        0        0    10294 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml
+-rw-rw-rw-   0        0        0     1054 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/viewProps.xml
+-rw-rw-rw-   0        0        0    25061 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/font-color.pptx
+-rw-rw-rw-   0        0        0   470987 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/just-two-mice.mp4
+-rw-rw-rw-   0        0        0   179346 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/just-two-mice.png
+-rw-rw-rw-   0        0        0    23202 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/lyt-shapes.pptx
+-rw-rw-rw-   0        0        0    15802 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/minimal.pptx
+-rw-rw-rw-   0        0        0    64276 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/monty-truth.png
+-rw-rw-rw-   0        0        0    25251 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/mst-placeholders.pptx
+-rw-rw-rw-   0        0        0    25539 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/mst-shapes.pptx
+-rw-rw-rw-   0        0        0    21166 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/mst-slide-layouts.pptx
+-rw-rw-rw-   0        0        0    23566 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/ph-inherit-props.pptx
+-rw-rw-rw-   0        0        0   172254 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/ph-populated-placeholders.pptx
+-rw-rw-rw-   0        0        0    34405 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/ph-unpopulated-placeholders.pptx
+-rw-rw-rw-   0        0        0    49704 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/pic.emf
+-rw-rw-rw-   0        0        0    19655 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/prs-add-slide.pptx
+-rw-rw-rw-   0        0        0    86792 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/prs-notes.pptx
+-rw-rw-rw-   0        0        0    15806 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/prs-properties.pptx
+-rw-rw-rw-   0        0        0    21528 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/prs-slide-masters.pptx
+-rw-rw-rw-   0        0        0     3277 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/python-icon.jpeg
+-rw-rw-rw-   0        0        0     6111 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/python-powered.png
+-rw-rw-rw-   0        0        0    45210 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/python.bmp
+-rw-rw-rw-   0        0        0    80038 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-access-chart.pptx
+-rw-rw-rw-   0        0        0   119022 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-access-ole-object.pptx
+-rw-rw-rw-   0        0        0    17626 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-autoshape-adjustments.pptx
+-rw-rw-rw-   0        0        0    22929 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-autoshape-props.pptx
+-rw-rw-rw-   0        0        0    81639 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-common-props.pptx
+-rw-rw-rw-   0        0        0    22899 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-connector-props.pptx
+-rw-rw-rw-   0        0        0    11680 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-embedded-docx.docx
+-rw-rw-rw-   0        0        0    29214 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-embedded-pptx.pptx
+-rw-rw-rw-   0        0        0     8250 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-embedded-xlsx.xlsx
+-rw-rw-rw-   0        0        0    16704 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-freeform.pptx
+-rw-rw-rw-   0        0        0    23786 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-groupshape.pptx
+-rw-rw-rw-   0        0        0   684874 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-movie-props.pptx
+-rw-rw-rw-   0        0        0    91730 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-picture.pptx
+-rw-rw-rw-   0        0        0    94116 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-pos-and-size.pptx
+-rw-rw-rw-   0        0        0   125205 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/shp-shapes.pptx
+-rw-rw-rw-   0        0        0    17676 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/sld-background.pptx
+-rw-rw-rw-   0        0        0    16703 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/sld-blank.pptx
+-rw-rw-rw-   0        0        0    22964 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/sld-notes.pptx
+-rw-rw-rw-   0        0        0    18894 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/sld-slide.pptx
+-rw-rw-rw-   0        0        0    18478 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/sld-slides.pptx
+-rw-rw-rw-   0        0        0    33273 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/sonic.gif
+-rw-rw-rw-   0        0        0    28247 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/tbl-cell.pptx
+-rw-rw-rw-   0        0        0    37859 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/test.pptx
+-rw-rw-rw-   0        0        0    21337 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/txt-fit-text.pptx
+-rw-rw-rw-   0        0        0    18874 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/txt-font-props.pptx
+-rw-rw-rw-   0        0        0    25817 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/txt-font-typeface.pptx
+-rw-rw-rw-   0        0        0    24620 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/txt-paragraph-spacing.pptx
+-rw-rw-rw-   0        0        0    27659 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/txt-text-frame.pptx
+-rw-rw-rw-   0        0        0    16051 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/test_files/txt-text.pptx
+-rw-rw-rw-   0        0        0     8520 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/text.py
+-rw-rw-rw-   0        0        0     4749 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/steps/text_frame.py
+-rw-rw-rw-   0        0        0     3662 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/tbl-cell.feature
+-rw-rw-rw-   0        0        0      353 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/tbl-column.feature
+-rw-rw-rw-   0        0        0     1625 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/tbl-table.feature
+-rw-rw-rw-   0        0        0      482 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/txt-fit-text.feature
+-rw-rw-rw-   0        0        0     1788 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/txt-font-color.feature
+-rw-rw-rw-   0        0        0     5094 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/txt-font-props.feature
+-rw-rw-rw-   0        0        0     4064 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/txt-paragraph.feature
+-rw-rw-rw-   0        0        0      757 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/txt-text.feature
+-rw-rw-rw-   0        0        0     2446 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/features/txt-textframe.feature
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.307065 python-petpptx-1.0.1/pptx/
+-rw-rw-rw-   0        0        0     2049 2023-06-06 12:01:11.000000 python-petpptx-1.0.1/pptx/__init__.py
+-rw-rw-rw-   0        0        0     8922 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/action.py
+-rw-rw-rw-   0        0        0     1644 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/api.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.339281 python-petpptx-1.0.1/pptx/chart/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/__init__.py
+-rw-rw-rw-   0        0        0    17827 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/axis.py
+-rw-rw-rw-   0        0        0     7452 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/category.py
+-rw-rw-rw-   0        0        0    10283 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/chart.py
+-rw-rw-rw-   0        0        0    30605 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/data.py
+-rw-rw-rw-   0        0        0     9820 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/datalabel.py
+-rw-rw-rw-   0        0        0     2649 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/legend.py
+-rw-rw-rw-   0        0        0     2202 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/marker.py
+-rw-rw-rw-   0        0        0    13629 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/plot.py
+-rw-rw-rw-   0        0        0     2899 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/point.py
+-rw-rw-rw-   0        0        0     7745 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/series.py
+-rw-rw-rw-   0        0        0    11223 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/xlsx.py
+-rw-rw-rw-   0        0        0    69538 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/chart/xmlwriter.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.339281 python-petpptx-1.0.1/pptx/compat/
+-rw-rw-rw-   0        0        0      768 2023-06-06 11:59:28.000000 python-petpptx-1.0.1/pptx/compat/__init__.py
+-rw-rw-rw-   0        0        0     1343 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/compat/python2.py
+-rw-rw-rw-   0        0        0      963 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/compat/python3.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.353911 python-petpptx-1.0.1/pptx/dml/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/dml/__init__.py
+-rw-rw-rw-   0        0        0     1415 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/dml/chtfmt.py
+-rw-rw-rw-   0        0        0     9429 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/dml/color.py
+-rw-rw-rw-   0        0        0     1635 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/dml/effect.py
+-rw-rw-rw-   0        0        0    13637 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/dml/fill.py
+-rw-rw-rw-   0        0        0     3210 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/dml/line.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.371967 python-petpptx-1.0.1/pptx/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/enum/__init__.py
+-rw-rw-rw-   0        0        0     1594 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/enum/action.py
+-rw-rw-rw-   0        0        0    11061 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/enum/base.py
+-rw-rw-rw-   0        0        0    13589 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/enum/chart.py
+-rw-rw-rw-   0        0        0    12259 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/enum/dml.py
+-rw-rw-rw-   0        0        0    23308 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/enum/lang.py
+-rw-rw-rw-   0        0        0    32343 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/enum/shapes.py
+-rw-rw-rw-   0        0        0     8470 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/enum/text.py
+-rw-rw-rw-   0        0        0      481 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/exc.py
+-rw-rw-rw-   0        0        0    10731 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/media.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.371967 python-petpptx-1.0.1/pptx/opc/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/opc/__init__.py
+-rw-rw-rw-   0        0        0    20491 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/opc/constants.py
+-rw-rw-rw-   0        0        0     4667 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/opc/oxml.py
+-rw-rw-rw-   0        0        0    27711 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/opc/package.py
+-rw-rw-rw-   0        0        0     3996 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/opc/packuri.py
+-rw-rw-rw-   0        0        0    10248 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/opc/serialized.py
+-rw-rw-rw-   0        0        0      712 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/opc/shared.py
+-rw-rw-rw-   0        0        0     1061 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/opc/spec.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.407088 python-petpptx-1.0.1/pptx/oxml/
+-rw-rw-rw-   0        0        0    15938 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/__init__.py
+-rw-rw-rw-   0        0        0     1663 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/action.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.412223 python-petpptx-1.0.1/pptx/oxml/chart/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/chart/__init__.py
+-rw-rw-rw-   0        0        0     9727 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/chart/axis.py
+-rw-rw-rw-   0        0        0     8478 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/chart/chart.py
+-rw-rw-rw-   0        0        0     8019 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/chart/datalabel.py
+-rw-rw-rw-   0        0        0     2205 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/chart/legend.py
+-rw-rw-rw-   0        0        0     1903 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/chart/marker.py
+-rw-rw-rw-   0        0        0     9573 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/chart/plot.py
+-rw-rw-rw-   0        0        0     7883 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/chart/series.py
+-rw-rw-rw-   0        0        0     6321 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/chart/shared.py
+-rw-rw-rw-   0        0        0    10114 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/coreprops.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.427853 python-petpptx-1.0.1/pptx/oxml/dml/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/dml/__init__.py
+-rw-rw-rw-   0        0        0     2592 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/dml/color.py
+-rw-rw-rw-   0        0        0     6186 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/dml/fill.py
+-rw-rw-rw-   0        0        0      460 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/dml/line.py
+-rw-rw-rw-   0        0        0     4809 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/ns.py
+-rw-rw-rw-   0        0        0     2890 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/presentation.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.443492 python-petpptx-1.0.1/pptx/oxml/shapes/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/shapes/__init__.py
+-rw-rw-rw-   0        0        0    13857 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/shapes/autoshape.py
+-rw-rw-rw-   0        0        0     3633 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/shapes/connector.py
+-rw-rw-rw-   0        0        0    12391 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/shapes/graphfrm.py
+-rw-rw-rw-   0        0        0     9492 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/shapes/groupshape.py
+-rw-rw-rw-   0        0        0     8353 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/shapes/picture.py
+-rw-rw-rw-   0        0        0    13199 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/shapes/shared.py
+-rw-rw-rw-   0        0        0    20684 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/simpletypes.py
+-rw-rw-rw-   0        0        0    10558 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/slide.py
+-rw-rw-rw-   0        0        0    18865 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/table.py
+-rw-rw-rw-   0        0        0    17016 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/text.py
+-rw-rw-rw-   0        0        0      787 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/theme.py
+-rw-rw-rw-   0        0        0    25824 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/oxml/xmlchemy.py
+-rw-rw-rw-   0        0        0     7846 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/package.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.459100 python-petpptx-1.0.1/pptx/parts/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/parts/__init__.py
+-rw-rw-rw-   0        0        0     3091 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/parts/chart.py
+-rw-rw-rw-   0        0        0     4213 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/parts/coreprops.py
+-rw-rw-rw-   0        0        0     2903 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/parts/embeddedpackage.py
+-rw-rw-rw-   0        0        0     9327 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/parts/image.py
+-rw-rw-rw-   0        0        0      938 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/parts/media.py
+-rw-rw-rw-   0        0        0     4598 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/parts/presentation.py
+-rw-rw-rw-   0        0        0    10732 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/parts/slide.py
+-rw-rw-rw-   0        0        0     3450 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/presentation.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.474726 python-petpptx-1.0.1/pptx/shapes/
+-rw-rw-rw-   0        0        0      614 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shapes/__init__.py
+-rw-rw-rw-   0        0        0    14103 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shapes/autoshape.py
+-rw-rw-rw-   0        0        0     7826 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shapes/base.py
+-rw-rw-rw-   0        0        0    10362 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shapes/connector.py
+-rw-rw-rw-   0        0        0    11244 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shapes/freeform.py
+-rw-rw-rw-   0        0        0     5150 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shapes/graphfrm.py
+-rw-rw-rw-   0        0        0     1920 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shapes/group.py
+-rw-rw-rw-   0        0        0     6848 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shapes/picture.py
+-rw-rw-rw-   0        0        0    14942 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shapes/placeholder.py
+-rw-rw-rw-   0        0        0    42499 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shapes/shapetree.py
+-rw-rw-rw-   0        0        0     2680 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/shared.py
+-rw-rw-rw-   0        0        0    18411 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/slide.py
+-rw-rw-rw-   0        0        0    24203 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/spec.py
+-rw-rw-rw-   0        0        0    16796 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/table.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.490368 python-petpptx-1.0.1/pptx/templates/
+-rw-rw-rw-   0        0        0    34030 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/templates/default.pptx
+-rw-rw-rw-   0        0        0   127228 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/templates/docx-icon.emf
+-rw-rw-rw-   0        0        0     5396 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/templates/generic-icon.emf
+-rw-rw-rw-   0        0        0      745 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/templates/notes.xml
+-rw-rw-rw-   0        0        0    11487 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/templates/notesMaster.xml
+-rw-rw-rw-   0        0        0     5492 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/templates/pptx-icon.emf
+-rw-rw-rw-   0        0        0    11285 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/templates/theme.xml
+-rw-rw-rw-   0        0        0   130380 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/templates/xlsx-icon.emf
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.490368 python-petpptx-1.0.1/pptx/text/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/text/__init__.py
+-rw-rw-rw-   0        0        0    13308 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/text/fonts.py
+-rw-rw-rw-   0        0        0    10277 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/text/layout.py
+-rw-rw-rw-   0        0        0    25979 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/text/text.py
+-rw-rw-rw-   0        0        0     8064 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/pptx/util.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.522027 python-petpptx-1.0.1/python_petpptx.egg-info/
+-rw-rw-rw-   0        0        0    19588 2023-06-06 12:01:47.000000 python-petpptx-1.0.1/python_petpptx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18674 2023-06-06 12:01:47.000000 python-petpptx-1.0.1/python_petpptx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 12:01:47.000000 python-petpptx-1.0.1/python_petpptx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 09:50:40.000000 python-petpptx-1.0.1/python_petpptx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2023-06-06 12:01:47.000000 python-petpptx-1.0.1/python_petpptx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-06 12:01:47.000000 python-petpptx-1.0.1/python_petpptx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 12:01:48.903262 python-petpptx-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2712 2023-06-06 09:50:34.000000 python-petpptx-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.553293 python-petpptx-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.568924 python-petpptx-1.0.1/tests/chart/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/__init__.py
+-rw-rw-rw-   0        0        0    49601 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_axis.py
+-rw-rw-rw-   0        0        0     9600 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_category.py
+-rw-rw-rw-   0        0        0    21804 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_chart.py
+-rw-rw-rw-   0        0        0    35047 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_data.py
+-rw-rw-rw-   0        0        0    26881 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_datalabel.py
+-rw-rw-rw-   0        0        0     6982 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_legend.py
+-rw-rw-rw-   0        0        0     4967 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_marker.py
+-rw-rw-rw-   0        0        0    19254 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_plot.py
+-rw-rw-rw-   0        0        0     7888 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_point.py
+-rw-rw-rw-   0        0        0    19624 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_series.py
+-rw-rw-rw-   0        0        0    16373 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_xlsx.py
+-rw-rw-rw-   0        0        0    29186 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/chart/test_xmlwriter.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.584546 python-petpptx-1.0.1/tests/dml/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/dml/__init__.py
+-rw-rw-rw-   0        0        0     3326 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/dml/test_chtfmt.py
+-rw-rw-rw-   0        0        0    11930 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/dml/test_color.py
+-rw-rw-rw-   0        0        0     1979 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/dml/test_effect.py
+-rw-rw-rw-   0        0        0    26377 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/dml/test_fill.py
+-rw-rw-rw-   0        0        0     6140 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/dml/test_line.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.599280 python-petpptx-1.0.1/tests/opc/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/opc/__init__.py
+-rw-rw-rw-   0        0        0     6642 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/opc/test_oxml.py
+-rw-rw-rw-   0        0        0    39420 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/opc/test_package.py
+-rw-rw-rw-   0        0        0     3072 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/opc/test_packuri.py
+-rw-rw-rw-   0        0        0    15207 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/opc/test_serialized.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.600415 python-petpptx-1.0.1/tests/opc/unitdata/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/opc/unitdata/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/opc/unitdata/rels.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.615938 python-petpptx-1.0.1/tests/oxml/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.629161 python-petpptx-1.0.1/tests/oxml/shapes/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/shapes/__init__.py
+-rw-rw-rw-   0        0        0    10284 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/shapes/test_autoshape.py
+-rw-rw-rw-   0        0        0     3466 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/shapes/test_graphfrm.py
+-rw-rw-rw-   0        0        0    11125 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/shapes/test_groupshape.py
+-rw-rw-rw-   0        0        0     3698 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/shapes/test_picture.py
+-rw-rw-rw-   0        0        0     3314 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/test___init__.py
+-rw-rw-rw-   0        0        0     5215 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/test_dml.py
+-rw-rw-rw-   0        0        0     2771 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/test_ns.py
+-rw-rw-rw-   0        0        0     1482 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/test_presentation.py
+-rw-rw-rw-   0        0        0     9267 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/test_simpletypes.py
+-rw-rw-rw-   0        0        0      742 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/test_slide.py
+-rw-rw-rw-   0        0        0    10390 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/test_table.py
+-rw-rw-rw-   0        0        0      720 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/test_theme.py
+-rw-rw-rw-   0        0        0    21508 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/test_xmlchemy.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.631300 python-petpptx-1.0.1/tests/oxml/unitdata/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/unitdata/__init__.py
+-rw-rw-rw-   0        0        0     2052 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/unitdata/dml.py
+-rw-rw-rw-   0        0        0     4275 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/unitdata/shape.py
+-rw-rw-rw-   0        0        0     1881 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/oxml/unitdata/text.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.646927 python-petpptx-1.0.1/tests/parts/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/parts/__init__.py
+-rw-rw-rw-   0        0        0     6130 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/parts/test_chart.py
+-rw-rw-rw-   0        0        0     9305 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/parts/test_coreprops.py
+-rw-rw-rw-   0        0        0     3087 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/parts/test_embeddedpackage.py
+-rw-rw-rw-   0        0        0     8047 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/parts/test_image.py
+-rw-rw-rw-   0        0        0     1218 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/parts/test_media.py
+-rw-rw-rw-   0        0        0     9395 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/parts/test_presentation.py
+-rw-rw-rw-   0        0        0    23166 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/parts/test_slide.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.662219 python-petpptx-1.0.1/tests/shapes/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/shapes/__init__.py
+-rw-rw-rw-   0        0        0    19158 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/shapes/test_autoshape.py
+-rw-rw-rw-   0        0        0    20302 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/shapes/test_base.py
+-rw-rw-rw-   0        0        0    16664 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/shapes/test_connector.py
+-rw-rw-rw-   0        0        0    21195 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/shapes/test_freeform.py
+-rw-rw-rw-   0        0        0     6826 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/shapes/test_graphfrm.py
+-rw-rw-rw-   0        0        0     2435 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/shapes/test_group.py
+-rw-rw-rw-   0        0        0    10931 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/shapes/test_picture.py
+-rw-rw-rw-   0        0        0    23006 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/shapes/test_placeholder.py
+-rw-rw-rw-   0        0        0    89451 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/shapes/test_shapetree.py
+-rw-rw-rw-   0        0        0    14348 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_action.py
+-rw-rw-rw-   0        0        0     1580 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_api.py
+-rw-rw-rw-   0        0        0     3859 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_enum.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.693601 python-petpptx-1.0.1/tests/test_files/
+-rw-rw-rw-   0        0        0   867288 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/calibriz.ttf
+-rw-rw-rw-   0        0        0    22238 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/cdw-logo.eps
+-rw-rw-rw-   0        0        0       43 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/dummy.mp4
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.693601 python-petpptx-1.0.1/tests/test_files/expanded_pptx/
+-rw-rw-rw-   0        0        0     3359 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/[Content_Types].xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.693601 python-petpptx-1.0.1/tests/test_files/expanded_pptx/_rels/
+-rw-rw-rw-   0        0        0      758 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/_rels/.rels
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.707114 python-petpptx-1.0.1/tests/test_files/expanded_pptx/docProps/
+-rw-rw-rw-   0        0        0     1354 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/docProps/app.xml
+-rw-rw-rw-   0        0        0      750 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/docProps/core.xml
+-rw-rw-rw-   0        0        0     8147 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.709129 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.709129 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/_rels/
+-rw-rw-rw-   0        0        0     1170 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels
+-rw-rw-rw-   0        0        0      327 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/presProps.xml
+-rw-rw-rw-   0        0        0     4157 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/presentation.xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.718340 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/printerSettings/
+-rw-rw-rw-   0        0        0     9395 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.724604 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.755808 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout1.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout10.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout11.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout2.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout3.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout4.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout5.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout6.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout7.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout8.xml.rels
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/_rels/slideLayout9.xml.rels
+-rw-rw-rw-   0        0        0     7473 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml
+-rw-rw-rw-   0        0        0     4783 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml
+-rw-rw-rw-   0        0        0     5131 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml
+-rw-rw-rw-   0        0        0     4786 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml
+-rw-rw-rw-   0        0        0     7613 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml
+-rw-rw-rw-   0        0        0     8154 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml
+-rw-rw-rw-   0        0        0    12501 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml
+-rw-rw-rw-   0        0        0     3371 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml
+-rw-rw-rw-   0        0        0     2757 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml
+-rw-rw-rw-   0        0        0     8100 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml
+-rw-rw-rw-   0        0        0     7633 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.755808 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideMasters/
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.755808 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/
+-rw-rw-rw-   0        0        0     2093 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels
+-rw-rw-rw-   0        0        0    17871 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.755808 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slides/
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.755808 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slides/_rels/
+-rw-rw-rw-   0        0        0      319 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slides/_rels/slide1.xml.rels
+-rw-rw-rw-   0        0        0     2198 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slides/slide1.xml
+-rw-rw-rw-   0        0        0      182 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/tableStyles.xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.755808 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/theme/
+-rw-rw-rw-   0        0        0    10294 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/theme/theme1.xml
+-rw-rw-rw-   0        0        0     1081 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/viewProps.xml
+-rw-rw-rw-   0        0        0    15802 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/minimal.pptx
+-rw-rw-rw-   0        0        0      492 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/minimal_slide.xml
+-rw-rw-rw-   0        0        0    32944 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/missing_rels_item.pptx
+-rw-rw-rw-   0        0        0    64276 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/monty-truth.png
+-rw-rw-rw-   0        0        0    34436 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/no-core-props.pptx
+-rw-rw-rw-   0        0        0    34036 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/no-slides.pptx
+-rw-rw-rw-   0        0        0     4157 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/presentation.xml
+-rw-rw-rw-   0        0        0     3277 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/python-icon.jpeg
+-rw-rw-rw-   0        0        0     6111 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/python-powered.png
+-rw-rw-rw-   0        0        0    45210 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/python.bmp
+-rw-rw-rw-   0        0        0     8134 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/slideLayout1.xml
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.865494 python-petpptx-1.0.1/tests/test_files/snippets/
+-rw-rw-rw-   0        0        0     5086 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-area-date.txt
+-rw-rw-rw-   0        0        0     5083 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-area-float.txt
+-rw-rw-rw-   0        0        0     4981 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-area-stacked-100.txt
+-rw-rw-rw-   0        0        0     4974 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-area-stacked.txt
+-rw-rw-rw-   0        0        0     4975 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-area.txt
+-rw-rw-rw-   0        0        0     4453 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-bar-clustered-date.txt
+-rw-rw-rw-   0        0        0     4391 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-bar-clustered-float.txt
+-rw-rw-rw-   0        0        0     4283 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-bar-clustered.txt
+-rw-rw-rw-   0        0        0     4320 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-bar-stacked-100.txt
+-rw-rw-rw-   0        0        0     4313 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-bar-stacked.txt
+-rw-rw-rw-   0        0        0     4283 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-column-clustered.txt
+-rw-rw-rw-   0        0        0     4320 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-column-stacked-100.txt
+-rw-rw-rw-   0        0        0     4313 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-column-stacked.txt
+-rw-rw-rw-   0        0        0     4907 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-date.txt
+-rw-rw-rw-   0        0        0     4845 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-float.txt
+-rw-rw-rw-   0        0        0     4581 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-markers-stacked-100.txt
+-rw-rw-rw-   0        0        0     4574 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-markers-stacked.txt
+-rw-rw-rw-   0        0        0     4575 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-markers.txt
+-rw-rw-rw-   0        0        0     4743 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-stacked-100.txt
+-rw-rw-rw-   0        0        0     4736 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-stacked.txt
+-rw-rw-rw-   0        0        0     4737 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x2-line.txt
+-rw-rw-rw-   0        0        0     6655 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x3-bubble-3d.txt
+-rw-rw-rw-   0        0        0     6655 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x3-bubble.txt
+-rw-rw-rw-   0        0        0     5254 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x3-xy-lines-no-markers.txt
+-rw-rw-rw-   0        0        0     5092 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x3-xy-lines.txt
+-rw-rw-rw-   0        0        0     5256 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt
+-rw-rw-rw-   0        0        0     5094 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x3-xy-smooth.txt
+-rw-rw-rw-   0        0        0     5330 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x3-xy.txt
+-rw-rw-rw-   0        0        0     6307 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/2x5-radar.txt
+-rw-rw-rw-   0        0        0     2180 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/3x1-pie-exploded.txt
+-rw-rw-rw-   0        0        0     2145 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/3x1-pie.txt
+-rw-rw-rw-   0        0        0     4286 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/3x2-doughnut-exploded.txt
+-rw-rw-rw-   0        0        0     4216 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/3x2-doughnut.txt
+-rw-rw-rw-   0        0        0     5517 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/4x2-multi-cat-bar.txt
+-rw-rw-rw-   0        0        0     3615 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/adjust-ser-count.txt
+-rw-rw-rw-   0        0        0     3782 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/cat-labels.txt
+-rw-rw-rw-   0        0        0      526 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/content-types-xml.txt
+-rw-rw-rw-   0        0        0      688 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/default-notes.txt
+-rw-rw-rw-   0        0        0    11409 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/default-notesMaster.txt
+-rw-rw-rw-   0        0        0    11213 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/default-theme.txt
+-rw-rw-rw-   0        0        0     1131 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/freeform.txt
+-rw-rw-rw-   0        0        0      764 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/package-rels-xml.txt
+-rw-rw-rw-   0        0        0     1817 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/placeholders.txt
+-rw-rw-rw-   0        0        0      606 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/presentation-rels-xml.txt
+-rw-rw-rw-   0        0        0      447 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/relationships.txt
+-rw-rw-rw-   0        0        0      628 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/rels-load-from-xml.txt
+-rw-rw-rw-   0        0        0    11033 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/rewrite-ser.txt
+-rw-rw-rw-   0        0        0     2893 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/snippets/timing.txt
+-rw-rw-rw-   0        0        0    37859 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/test.pptx
+-rw-rw-rw-   0        0        0    38616 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_files/test_slides.pptx
+-rw-rw-rw-   0        0        0     4740 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_media.py
+-rw-rw-rw-   0        0        0    13882 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_package.py
+-rw-rw-rw-   0        0        0     9170 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_presentation.py
+-rw-rw-rw-   0        0        0     2538 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_shared.py
+-rw-rw-rw-   0        0        0    40208 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_slide.py
+-rw-rw-rw-   0        0        0    29977 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_table.py
+-rw-rw-rw-   0        0        0     1941 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.887637 python-petpptx-1.0.1/tests/text/
+-rw-rw-rw-   0        0        0        0 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/text/__init__.py
+-rw-rw-rw-   0        0        0    25932 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/text/test_fonts.py
+-rw-rw-rw-   0        0        0     9269 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/text/test_layout.py
+-rw-rw-rw-   0        0        0    46965 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/text/test_text.py
+-rw-rw-rw-   0        0        0     3785 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/unitdata.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:01:48.887637 python-petpptx-1.0.1/tests/unitutil/
+-rw-rw-rw-   0        0        0      262 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/unitutil/__init__.py
+-rw-rw-rw-   0        0        0     8597 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/unitutil/cxml.py
+-rw-rw-rw-   0        0        0     1919 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/unitutil/file.py
+-rw-rw-rw-   0        0        0     4243 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tests/unitutil/mock.py
+-rw-rw-rw-   0        0        0      689 2023-06-06 09:05:39.000000 python-petpptx-1.0.1/tox.ini
```

### Comparing `python-petpptx-1.0.0/HISTORY.rst` & `python-petpptx-1.0.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 Release History
 ---------------
 
+1.0.1 (2023-06-06)
++++++++++++++++++++
+
+- Fix module 'collections' has no attribute 'Container' for latest python 3.10
+
+
 1.0.0 (2023-06-06)
 +++++++++++++++++++
 
 - Release of a new version of the project
 - Add setter for font in Run
```

### Comparing `python-petpptx-1.0.0/LICENSE` & `python-petpptx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/PKG-INFO` & `python-petpptx-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-petpptx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate and manipulate Open XML PowerPoint (.pptx) files
 Home-page: https://github.com/sedrew/python-petpptx
 Author: Sergey Malygin
 Author-email: maligin.serega2010@yndex.ru
 License: The MIT License (MIT)
         Copyright (c) 2013 Steve Canny, https://github.com/scanny
         
@@ -67,14 +67,20 @@
 
 
 .. :changelog:
 
 Release History
 ---------------
 
+1.0.1 (2023-06-06)
++++++++++++++++++++
+
+- Fix module 'collections' has no attribute 'Container' for latest python 3.10
+
+
 1.0.0 (2023-06-06)
 +++++++++++++++++++
 
 - Release of a new version of the project
 - Add setter for font in Run
```

### Comparing `python-petpptx-1.0.0/README.rst` & `python-petpptx-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/act-action.feature` & `python-petpptx-1.0.1/features/act-action.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/act-hyperlink.feature` & `python-petpptx-1.0.1/features/act-hyperlink.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-axis-props.feature` & `python-petpptx-1.0.1/features/cht-axis-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-axistitle-props.feature` & `python-petpptx-1.0.1/features/cht-axistitle-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-category-access.feature` & `python-petpptx-1.0.1/features/cht-category-access.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-category-props.feature` & `python-petpptx-1.0.1/features/cht-category-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-chart.feature` & `python-petpptx-1.0.1/features/cht-chart.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-charttitle-props.feature` & `python-petpptx-1.0.1/features/cht-charttitle-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-data-props.feature` & `python-petpptx-1.0.1/features/cht-data-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-datalabels.feature` & `python-petpptx-1.0.1/features/cht-datalabels.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-legend-access.feature` & `python-petpptx-1.0.1/features/cht-legend-access.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-legend-props.feature` & `python-petpptx-1.0.1/features/cht-legend-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-marker-props.feature` & `python-petpptx-1.0.1/features/cht-marker-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-plot-props.feature` & `python-petpptx-1.0.1/features/cht-plot-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-point-access.feature` & `python-petpptx-1.0.1/features/cht-point-access.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-point-props.feature` & `python-petpptx-1.0.1/features/cht-point-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-replace-data.feature` & `python-petpptx-1.0.1/features/cht-replace-data.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-series.feature` & `python-petpptx-1.0.1/features/cht-series.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/cht-ticklabels-props.feature` & `python-petpptx-1.0.1/features/cht-ticklabels-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/dml-color.feature` & `python-petpptx-1.0.1/features/dml-color.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/dml-effect.feature` & `python-petpptx-1.0.1/features/dml-effect.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/dml-fill.feature` & `python-petpptx-1.0.1/features/dml-fill.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/dml-line.feature` & `python-petpptx-1.0.1/features/dml-line.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/environment.py` & `python-petpptx-1.0.1/features/environment.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/ph-inherit-props.feature` & `python-petpptx-1.0.1/features/ph-inherit-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/ph-insert-shape.feature` & `python-petpptx-1.0.1/features/ph-insert-shape.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/ph-phfmt-props.feature` & `python-petpptx-1.0.1/features/ph-phfmt-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/ph-placeholder-props.feature` & `python-petpptx-1.0.1/features/ph-placeholder-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/prs-coreprops.feature` & `python-petpptx-1.0.1/features/prs-coreprops.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/prs-open-save.feature` & `python-petpptx-1.0.1/features/prs-open-save.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/prs-presentation-props.feature` & `python-petpptx-1.0.1/features/prs-presentation-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/shp-autoshape.feature` & `python-petpptx-1.0.1/features/shp-autoshape.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/shp-connector.feature` & `python-petpptx-1.0.1/features/shp-connector.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/shp-freeform.feature` & `python-petpptx-1.0.1/features/shp-freeform.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/shp-graphicframe.feature` & `python-petpptx-1.0.1/features/shp-graphicframe.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/shp-groupshape.feature` & `python-petpptx-1.0.1/features/shp-groupshape.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/shp-movie-props.feature` & `python-petpptx-1.0.1/features/shp-movie-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/shp-picture.feature` & `python-petpptx-1.0.1/features/shp-picture.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/shp-placeholder.feature` & `python-petpptx-1.0.1/features/shp-placeholder.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/shp-shapes.feature` & `python-petpptx-1.0.1/features/shp-shapes.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/shp-shared.feature` & `python-petpptx-1.0.1/features/shp-shared.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/sld-slide.feature` & `python-petpptx-1.0.1/features/sld-slide.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/sld-slides.feature` & `python-petpptx-1.0.1/features/sld-slides.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/action.py` & `python-petpptx-1.0.1/features/steps/action.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/axis.py` & `python-petpptx-1.0.1/features/steps/axis.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/background.py` & `python-petpptx-1.0.1/features/steps/background.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/category.py` & `python-petpptx-1.0.1/features/steps/category.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/chart.py` & `python-petpptx-1.0.1/features/steps/chart.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/chartdata.py` & `python-petpptx-1.0.1/features/steps/chartdata.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/color.py` & `python-petpptx-1.0.1/features/steps/color.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/coreprops.py` & `python-petpptx-1.0.1/features/steps/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/datalabel.py` & `python-petpptx-1.0.1/features/steps/datalabel.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/effect.py` & `python-petpptx-1.0.1/features/steps/effect.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/fill.py` & `python-petpptx-1.0.1/features/steps/fill.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/font.py` & `python-petpptx-1.0.1/features/steps/font.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/font_color.py` & `python-petpptx-1.0.1/features/steps/font_color.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/helpers.py` & `python-petpptx-1.0.1/features/steps/helpers.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/legend.py` & `python-petpptx-1.0.1/features/steps/legend.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/line.py` & `python-petpptx-1.0.1/features/steps/line.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/picture.py` & `python-petpptx-1.0.1/features/steps/picture.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/placeholder.py` & `python-petpptx-1.0.1/features/steps/placeholder.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/plot.py` & `python-petpptx-1.0.1/features/steps/plot.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/presentation.py` & `python-petpptx-1.0.1/features/steps/presentation.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/series.py` & `python-petpptx-1.0.1/features/steps/series.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/shape.py` & `python-petpptx-1.0.1/features/steps/shape.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/shapes.py` & `python-petpptx-1.0.1/features/steps/shapes.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/slide.py` & `python-petpptx-1.0.1/features/steps/slide.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/slides.py` & `python-petpptx-1.0.1/features/steps/slides.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/table.py` & `python-petpptx-1.0.1/features/steps/table.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/72-dpi.tiff` & `python-petpptx-1.0.1/features/steps/test_files/72-dpi.tiff`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/CVS_LOGO.WMF` & `python-petpptx-1.0.1/features/steps/test_files/CVS_LOGO.WMF`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/act-props.pptm` & `python-petpptx-1.0.1/features/steps/test_files/act-props.pptm`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/calibriz.ttf` & `python-petpptx-1.0.1/features/steps/test_files/calibriz.ttf`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-axis-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-axis-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-category-access.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-category-access.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-chart-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-chart-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-chart-type.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-chart-type.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-charts.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-charts.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-datalabels.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-datalabels.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-gridlines-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-gridlines-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-legend-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-legend-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-legend.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-legend.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-marker-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-marker-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-plot-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-plot-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-point-access.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-point-access.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-point-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-point-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-replace-data.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-replace-data.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-series.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-series.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/cht-ticklabels-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/cht-ticklabels-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/dml-effect.pptx` & `python-petpptx-1.0.1/features/steps/test_files/dml-effect.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/dml-fill.pptx` & `python-petpptx-1.0.1/features/steps/test_files/dml-fill.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/dml-line.pptx` & `python-petpptx-1.0.1/features/steps/test_files/dml-line.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/ext-rels.pptx` & `python-petpptx-1.0.1/features/steps/test_files/ext-rels.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/[Content_Types].xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/_rels/.rels` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/docProps/app.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/docProps/core.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/_rels/presentation.xml.rels`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/presProps.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/presProps.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/presentation.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/presentation.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/printerSettings/printerSettings1.bin`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout1.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout10.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout11.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout2.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout3.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout4.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout5.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout6.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout7.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout8.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideLayouts/slideLayout9.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slideMasters/slideMaster1.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/slides/slide1.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/extracted-pptx/ppt/viewProps.xml` & `python-petpptx-1.0.1/features/steps/test_files/extracted-pptx/ppt/viewProps.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/font-color.pptx` & `python-petpptx-1.0.1/features/steps/test_files/font-color.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/just-two-mice.mp4` & `python-petpptx-1.0.1/features/steps/test_files/just-two-mice.mp4`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/just-two-mice.png` & `python-petpptx-1.0.1/features/steps/test_files/just-two-mice.png`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/lyt-shapes.pptx` & `python-petpptx-1.0.1/features/steps/test_files/lyt-shapes.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/minimal.pptx` & `python-petpptx-1.0.1/features/steps/test_files/minimal.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/monty-truth.png` & `python-petpptx-1.0.1/features/steps/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/mst-placeholders.pptx` & `python-petpptx-1.0.1/features/steps/test_files/mst-placeholders.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/mst-shapes.pptx` & `python-petpptx-1.0.1/features/steps/test_files/mst-shapes.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/mst-slide-layouts.pptx` & `python-petpptx-1.0.1/features/steps/test_files/mst-slide-layouts.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/ph-inherit-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/ph-inherit-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/ph-populated-placeholders.pptx` & `python-petpptx-1.0.1/features/steps/test_files/ph-populated-placeholders.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/ph-unpopulated-placeholders.pptx` & `python-petpptx-1.0.1/features/steps/test_files/ph-unpopulated-placeholders.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/pic.emf` & `python-petpptx-1.0.1/features/steps/test_files/pic.emf`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/prs-add-slide.pptx` & `python-petpptx-1.0.1/features/steps/test_files/prs-add-slide.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/prs-notes.pptx` & `python-petpptx-1.0.1/features/steps/test_files/prs-notes.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/prs-properties.pptx` & `python-petpptx-1.0.1/features/steps/test_files/prs-properties.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/prs-slide-masters.pptx` & `python-petpptx-1.0.1/features/steps/test_files/prs-slide-masters.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/python-icon.jpeg` & `python-petpptx-1.0.1/features/steps/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/python-powered.png` & `python-petpptx-1.0.1/features/steps/test_files/python-powered.png`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/python.bmp` & `python-petpptx-1.0.1/features/steps/test_files/python.bmp`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-access-chart.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-access-chart.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-access-ole-object.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-access-ole-object.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-autoshape-adjustments.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-autoshape-adjustments.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-autoshape-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-autoshape-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-common-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-common-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-connector-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-connector-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-embedded-docx.docx` & `python-petpptx-1.0.1/features/steps/test_files/shp-embedded-docx.docx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-embedded-pptx.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-embedded-pptx.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-embedded-xlsx.xlsx` & `python-petpptx-1.0.1/features/steps/test_files/shp-embedded-xlsx.xlsx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-freeform.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-freeform.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-groupshape.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-groupshape.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-movie-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-movie-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-picture.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-picture.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-pos-and-size.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-pos-and-size.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/shp-shapes.pptx` & `python-petpptx-1.0.1/features/steps/test_files/shp-shapes.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/sld-background.pptx` & `python-petpptx-1.0.1/features/steps/test_files/sld-background.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/sld-blank.pptx` & `python-petpptx-1.0.1/features/steps/test_files/sld-blank.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/sld-notes.pptx` & `python-petpptx-1.0.1/features/steps/test_files/sld-notes.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/sld-slide.pptx` & `python-petpptx-1.0.1/features/steps/test_files/sld-slide.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/sld-slides.pptx` & `python-petpptx-1.0.1/features/steps/test_files/sld-slides.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/sonic.gif` & `python-petpptx-1.0.1/features/steps/test_files/sonic.gif`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/tbl-cell.pptx` & `python-petpptx-1.0.1/features/steps/test_files/tbl-cell.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/test.pptx` & `python-petpptx-1.0.1/features/steps/test_files/test.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/txt-fit-text.pptx` & `python-petpptx-1.0.1/features/steps/test_files/txt-fit-text.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/txt-font-props.pptx` & `python-petpptx-1.0.1/features/steps/test_files/txt-font-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/txt-font-typeface.pptx` & `python-petpptx-1.0.1/features/steps/test_files/txt-font-typeface.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/txt-paragraph-spacing.pptx` & `python-petpptx-1.0.1/features/steps/test_files/txt-paragraph-spacing.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/txt-text-frame.pptx` & `python-petpptx-1.0.1/features/steps/test_files/txt-text-frame.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/test_files/txt-text.pptx` & `python-petpptx-1.0.1/features/steps/test_files/txt-text.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/text.py` & `python-petpptx-1.0.1/features/steps/text.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/steps/text_frame.py` & `python-petpptx-1.0.1/features/steps/text_frame.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/tbl-cell.feature` & `python-petpptx-1.0.1/features/tbl-cell.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/tbl-table.feature` & `python-petpptx-1.0.1/features/tbl-table.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/txt-font-color.feature` & `python-petpptx-1.0.1/features/txt-font-color.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/txt-font-props.feature` & `python-petpptx-1.0.1/features/txt-font-props.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/txt-paragraph.feature` & `python-petpptx-1.0.1/features/txt-paragraph.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/txt-text.feature` & `python-petpptx-1.0.1/features/txt-text.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/features/txt-textframe.feature` & `python-petpptx-1.0.1/features/txt-textframe.feature`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/__init__.py` & `python-petpptx-1.0.1/pptx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # encoding: utf-8
 
 """Initialization module for python-pptx package."""
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
-import pptx.exc as exceptions
 import sys
 
+import pptx.exc as exceptions
+
 sys.modules["pptx.exceptions"] = exceptions
 del sys
 
 from pptx.api import Presentation  # noqa
 
 from pptx.opc.constants import CONTENT_TYPE as CT  # noqa: E402
 from pptx.opc.package import PartFactory  # noqa: E402
```

### Comparing `python-petpptx-1.0.0/pptx/action.py` & `python-petpptx-1.0.1/pptx/action.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/api.py` & `python-petpptx-1.0.1/pptx/api.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/axis.py` & `python-petpptx-1.0.1/pptx/chart/axis.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/category.py` & `python-petpptx-1.0.1/pptx/chart/category.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/chart.py` & `python-petpptx-1.0.1/pptx/chart/chart.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/data.py` & `python-petpptx-1.0.1/pptx/chart/data.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/datalabel.py` & `python-petpptx-1.0.1/pptx/chart/datalabel.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/legend.py` & `python-petpptx-1.0.1/pptx/chart/legend.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/marker.py` & `python-petpptx-1.0.1/pptx/chart/marker.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/plot.py` & `python-petpptx-1.0.1/pptx/chart/plot.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/point.py` & `python-petpptx-1.0.1/pptx/chart/point.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/series.py` & `python-petpptx-1.0.1/pptx/chart/series.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/xlsx.py` & `python-petpptx-1.0.1/pptx/chart/xlsx.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/chart/xmlwriter.py` & `python-petpptx-1.0.1/pptx/chart/xmlwriter.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/compat/python2.py` & `python-petpptx-1.0.1/pptx/compat/python2.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/compat/python3.py` & `python-petpptx-1.0.1/pptx/compat/python3.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/dml/chtfmt.py` & `python-petpptx-1.0.1/pptx/dml/chtfmt.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/dml/color.py` & `python-petpptx-1.0.1/pptx/dml/color.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/dml/effect.py` & `python-petpptx-1.0.1/pptx/dml/effect.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/dml/fill.py` & `python-petpptx-1.0.1/pptx/dml/fill.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/dml/line.py` & `python-petpptx-1.0.1/pptx/dml/line.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/enum/action.py` & `python-petpptx-1.0.1/pptx/enum/action.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/enum/base.py` & `python-petpptx-1.0.1/pptx/enum/base.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/enum/chart.py` & `python-petpptx-1.0.1/pptx/enum/chart.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/enum/dml.py` & `python-petpptx-1.0.1/pptx/enum/dml.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/enum/lang.py` & `python-petpptx-1.0.1/pptx/enum/lang.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/enum/shapes.py` & `python-petpptx-1.0.1/pptx/enum/shapes.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/enum/text.py` & `python-petpptx-1.0.1/pptx/enum/text.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/media.py` & `python-petpptx-1.0.1/pptx/media.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/opc/constants.py` & `python-petpptx-1.0.1/pptx/opc/constants.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/opc/oxml.py` & `python-petpptx-1.0.1/pptx/opc/oxml.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/opc/package.py` & `python-petpptx-1.0.1/pptx/opc/package.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/opc/packuri.py` & `python-petpptx-1.0.1/pptx/opc/packuri.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/opc/serialized.py` & `python-petpptx-1.0.1/pptx/opc/serialized.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/opc/shared.py` & `python-petpptx-1.0.1/pptx/opc/shared.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/opc/spec.py` & `python-petpptx-1.0.1/pptx/opc/spec.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/__init__.py` & `python-petpptx-1.0.1/pptx/oxml/__init__.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/action.py` & `python-petpptx-1.0.1/pptx/oxml/action.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/chart/axis.py` & `python-petpptx-1.0.1/pptx/oxml/chart/axis.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/chart/chart.py` & `python-petpptx-1.0.1/pptx/oxml/chart/chart.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/chart/datalabel.py` & `python-petpptx-1.0.1/pptx/oxml/chart/datalabel.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/chart/legend.py` & `python-petpptx-1.0.1/pptx/oxml/chart/legend.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/chart/marker.py` & `python-petpptx-1.0.1/pptx/oxml/chart/marker.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/chart/plot.py` & `python-petpptx-1.0.1/pptx/oxml/chart/plot.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/chart/series.py` & `python-petpptx-1.0.1/pptx/oxml/chart/series.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/chart/shared.py` & `python-petpptx-1.0.1/pptx/oxml/chart/shared.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/coreprops.py` & `python-petpptx-1.0.1/pptx/oxml/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/dml/color.py` & `python-petpptx-1.0.1/pptx/oxml/dml/color.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/dml/fill.py` & `python-petpptx-1.0.1/pptx/oxml/dml/fill.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/ns.py` & `python-petpptx-1.0.1/pptx/oxml/ns.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/presentation.py` & `python-petpptx-1.0.1/pptx/oxml/presentation.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/shapes/autoshape.py` & `python-petpptx-1.0.1/pptx/oxml/shapes/autoshape.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/shapes/connector.py` & `python-petpptx-1.0.1/pptx/oxml/shapes/connector.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/shapes/graphfrm.py` & `python-petpptx-1.0.1/pptx/oxml/shapes/graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/shapes/groupshape.py` & `python-petpptx-1.0.1/pptx/oxml/shapes/groupshape.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/shapes/picture.py` & `python-petpptx-1.0.1/pptx/oxml/shapes/picture.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/shapes/shared.py` & `python-petpptx-1.0.1/pptx/oxml/shapes/shared.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/simpletypes.py` & `python-petpptx-1.0.1/pptx/oxml/simpletypes.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/slide.py` & `python-petpptx-1.0.1/pptx/oxml/slide.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/table.py` & `python-petpptx-1.0.1/pptx/oxml/table.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/text.py` & `python-petpptx-1.0.1/pptx/oxml/text.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/theme.py` & `python-petpptx-1.0.1/pptx/oxml/theme.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/oxml/xmlchemy.py` & `python-petpptx-1.0.1/pptx/oxml/xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/package.py` & `python-petpptx-1.0.1/pptx/package.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/parts/chart.py` & `python-petpptx-1.0.1/pptx/parts/chart.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/parts/coreprops.py` & `python-petpptx-1.0.1/pptx/parts/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/parts/embeddedpackage.py` & `python-petpptx-1.0.1/pptx/parts/embeddedpackage.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/parts/image.py` & `python-petpptx-1.0.1/pptx/parts/image.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/parts/media.py` & `python-petpptx-1.0.1/pptx/parts/media.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/parts/presentation.py` & `python-petpptx-1.0.1/pptx/parts/presentation.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/parts/slide.py` & `python-petpptx-1.0.1/pptx/parts/slide.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/presentation.py` & `python-petpptx-1.0.1/pptx/presentation.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shapes/__init__.py` & `python-petpptx-1.0.1/pptx/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shapes/autoshape.py` & `python-petpptx-1.0.1/pptx/shapes/autoshape.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shapes/base.py` & `python-petpptx-1.0.1/pptx/shapes/base.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shapes/connector.py` & `python-petpptx-1.0.1/pptx/shapes/connector.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shapes/freeform.py` & `python-petpptx-1.0.1/pptx/shapes/freeform.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shapes/graphfrm.py` & `python-petpptx-1.0.1/pptx/shapes/graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shapes/group.py` & `python-petpptx-1.0.1/pptx/shapes/group.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shapes/picture.py` & `python-petpptx-1.0.1/pptx/shapes/picture.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shapes/placeholder.py` & `python-petpptx-1.0.1/pptx/shapes/placeholder.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shapes/shapetree.py` & `python-petpptx-1.0.1/pptx/shapes/shapetree.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/shared.py` & `python-petpptx-1.0.1/pptx/shared.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/slide.py` & `python-petpptx-1.0.1/pptx/slide.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/spec.py` & `python-petpptx-1.0.1/pptx/spec.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/table.py` & `python-petpptx-1.0.1/pptx/table.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/templates/default.pptx` & `python-petpptx-1.0.1/pptx/templates/default.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/templates/docx-icon.emf` & `python-petpptx-1.0.1/pptx/templates/docx-icon.emf`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/templates/generic-icon.emf` & `python-petpptx-1.0.1/pptx/templates/generic-icon.emf`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/templates/notes.xml` & `python-petpptx-1.0.1/pptx/templates/notes.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/templates/notesMaster.xml` & `python-petpptx-1.0.1/pptx/templates/notesMaster.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/templates/pptx-icon.emf` & `python-petpptx-1.0.1/pptx/templates/pptx-icon.emf`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/templates/theme.xml` & `python-petpptx-1.0.1/pptx/templates/theme.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/templates/xlsx-icon.emf` & `python-petpptx-1.0.1/pptx/templates/xlsx-icon.emf`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/text/fonts.py` & `python-petpptx-1.0.1/pptx/text/fonts.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/text/layout.py` & `python-petpptx-1.0.1/pptx/text/layout.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/text/text.py` & `python-petpptx-1.0.1/pptx/text/text.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/pptx/util.py` & `python-petpptx-1.0.1/pptx/util.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/python_petpptx.egg-info/PKG-INFO` & `python-petpptx-1.0.1/python_petpptx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-petpptx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate and manipulate Open XML PowerPoint (.pptx) files
 Home-page: https://github.com/sedrew/python-petpptx
 Author: Sergey Malygin
 Author-email: maligin.serega2010@yndex.ru
 License: The MIT License (MIT)
         Copyright (c) 2013 Steve Canny, https://github.com/scanny
         
@@ -67,14 +67,20 @@
 
 
 .. :changelog:
 
 Release History
 ---------------
 
+1.0.1 (2023-06-06)
++++++++++++++++++++
+
+- Fix module 'collections' has no attribute 'Container' for latest python 3.10
+
+
 1.0.0 (2023-06-06)
 +++++++++++++++++++
 
 - Release of a new version of the project
 - Add setter for font in Run
```

### Comparing `python-petpptx-1.0.0/python_petpptx.egg-info/SOURCES.txt` & `python-petpptx-1.0.1/python_petpptx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/setup.py` & `python-petpptx-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_axis.py` & `python-petpptx-1.0.1/tests/chart/test_axis.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_category.py` & `python-petpptx-1.0.1/tests/chart/test_category.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_chart.py` & `python-petpptx-1.0.1/tests/chart/test_chart.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_data.py` & `python-petpptx-1.0.1/tests/chart/test_data.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_datalabel.py` & `python-petpptx-1.0.1/tests/chart/test_datalabel.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_legend.py` & `python-petpptx-1.0.1/tests/chart/test_legend.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_marker.py` & `python-petpptx-1.0.1/tests/chart/test_marker.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_plot.py` & `python-petpptx-1.0.1/tests/chart/test_plot.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_point.py` & `python-petpptx-1.0.1/tests/chart/test_point.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_series.py` & `python-petpptx-1.0.1/tests/chart/test_series.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_xlsx.py` & `python-petpptx-1.0.1/tests/chart/test_xlsx.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/chart/test_xmlwriter.py` & `python-petpptx-1.0.1/tests/chart/test_xmlwriter.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/dml/test_chtfmt.py` & `python-petpptx-1.0.1/tests/dml/test_chtfmt.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/dml/test_color.py` & `python-petpptx-1.0.1/tests/dml/test_color.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/dml/test_effect.py` & `python-petpptx-1.0.1/tests/dml/test_effect.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/dml/test_fill.py` & `python-petpptx-1.0.1/tests/dml/test_fill.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/dml/test_line.py` & `python-petpptx-1.0.1/tests/dml/test_line.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/opc/test_oxml.py` & `python-petpptx-1.0.1/tests/opc/test_oxml.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/opc/test_package.py` & `python-petpptx-1.0.1/tests/opc/test_package.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/opc/test_packuri.py` & `python-petpptx-1.0.1/tests/opc/test_packuri.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/opc/test_serialized.py` & `python-petpptx-1.0.1/tests/opc/test_serialized.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/opc/unitdata/rels.py` & `python-petpptx-1.0.1/tests/opc/unitdata/rels.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/shapes/test_autoshape.py` & `python-petpptx-1.0.1/tests/oxml/shapes/test_autoshape.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/shapes/test_graphfrm.py` & `python-petpptx-1.0.1/tests/oxml/shapes/test_graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/shapes/test_groupshape.py` & `python-petpptx-1.0.1/tests/oxml/shapes/test_groupshape.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/shapes/test_picture.py` & `python-petpptx-1.0.1/tests/oxml/shapes/test_picture.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/test___init__.py` & `python-petpptx-1.0.1/tests/oxml/test___init__.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/test_dml.py` & `python-petpptx-1.0.1/tests/oxml/test_dml.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/test_ns.py` & `python-petpptx-1.0.1/tests/oxml/test_ns.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/test_presentation.py` & `python-petpptx-1.0.1/tests/oxml/test_presentation.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/test_simpletypes.py` & `python-petpptx-1.0.1/tests/oxml/test_simpletypes.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/test_slide.py` & `python-petpptx-1.0.1/tests/oxml/test_slide.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/test_table.py` & `python-petpptx-1.0.1/tests/oxml/test_table.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/test_theme.py` & `python-petpptx-1.0.1/tests/oxml/test_theme.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/test_xmlchemy.py` & `python-petpptx-1.0.1/tests/oxml/test_xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/unitdata/dml.py` & `python-petpptx-1.0.1/tests/oxml/unitdata/dml.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/unitdata/shape.py` & `python-petpptx-1.0.1/tests/oxml/unitdata/shape.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/oxml/unitdata/text.py` & `python-petpptx-1.0.1/tests/oxml/unitdata/text.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/parts/test_chart.py` & `python-petpptx-1.0.1/tests/parts/test_chart.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/parts/test_coreprops.py` & `python-petpptx-1.0.1/tests/parts/test_coreprops.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/parts/test_embeddedpackage.py` & `python-petpptx-1.0.1/tests/parts/test_embeddedpackage.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/parts/test_image.py` & `python-petpptx-1.0.1/tests/parts/test_image.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/parts/test_media.py` & `python-petpptx-1.0.1/tests/parts/test_media.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/parts/test_presentation.py` & `python-petpptx-1.0.1/tests/parts/test_presentation.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/parts/test_slide.py` & `python-petpptx-1.0.1/tests/parts/test_slide.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/shapes/test_autoshape.py` & `python-petpptx-1.0.1/tests/shapes/test_autoshape.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/shapes/test_base.py` & `python-petpptx-1.0.1/tests/shapes/test_base.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/shapes/test_connector.py` & `python-petpptx-1.0.1/tests/shapes/test_connector.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/shapes/test_freeform.py` & `python-petpptx-1.0.1/tests/shapes/test_freeform.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/shapes/test_graphfrm.py` & `python-petpptx-1.0.1/tests/shapes/test_graphfrm.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/shapes/test_group.py` & `python-petpptx-1.0.1/tests/shapes/test_group.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/shapes/test_picture.py` & `python-petpptx-1.0.1/tests/shapes/test_picture.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/shapes/test_placeholder.py` & `python-petpptx-1.0.1/tests/shapes/test_placeholder.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/shapes/test_shapetree.py` & `python-petpptx-1.0.1/tests/shapes/test_shapetree.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_action.py` & `python-petpptx-1.0.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_api.py` & `python-petpptx-1.0.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_enum.py` & `python-petpptx-1.0.1/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/calibriz.ttf` & `python-petpptx-1.0.1/tests/test_files/calibriz.ttf`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/cdw-logo.eps` & `python-petpptx-1.0.1/tests/test_files/cdw-logo.eps`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/[Content_Types].xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/_rels/.rels` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/docProps/app.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/docProps/core.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/_rels/presentation.xml.rels`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/presentation.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/presentation.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/printerSettings/printerSettings1.bin`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout1.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout10.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout11.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout2.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout3.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout4.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout5.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout6.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout7.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout8.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideLayouts/slideLayout9.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideMasters/_rels/slideMaster1.xml.rels`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slideMasters/slideMaster1.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/slides/slide1.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/slides/slide1.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/theme/theme1.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/expanded_pptx/ppt/viewProps.xml` & `python-petpptx-1.0.1/tests/test_files/expanded_pptx/ppt/viewProps.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/minimal.pptx` & `python-petpptx-1.0.1/tests/test_files/minimal.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/missing_rels_item.pptx` & `python-petpptx-1.0.1/tests/test_files/missing_rels_item.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/monty-truth.png` & `python-petpptx-1.0.1/tests/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/no-core-props.pptx` & `python-petpptx-1.0.1/tests/test_files/no-core-props.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/no-slides.pptx` & `python-petpptx-1.0.1/tests/test_files/no-slides.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/presentation.xml` & `python-petpptx-1.0.1/tests/test_files/presentation.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/python-icon.jpeg` & `python-petpptx-1.0.1/tests/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/python-powered.png` & `python-petpptx-1.0.1/tests/test_files/python-powered.png`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/python.bmp` & `python-petpptx-1.0.1/tests/test_files/python.bmp`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/slideLayout1.xml` & `python-petpptx-1.0.1/tests/test_files/slideLayout1.xml`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-area-date.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-area-date.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-area-float.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-area-float.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-area-stacked-100.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-area-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-area-stacked.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-area-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-area.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-area.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-bar-clustered-date.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-bar-clustered-date.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-bar-clustered-float.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-bar-clustered-float.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-bar-clustered.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-bar-clustered.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-bar-stacked-100.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-bar-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-bar-stacked.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-bar-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-column-clustered.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-column-clustered.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-column-stacked-100.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-column-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-column-stacked.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-column-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-date.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-date.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-float.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-float.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-markers-stacked-100.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-markers-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-markers-stacked.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-markers-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-markers.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-markers.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-stacked-100.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-stacked-100.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-line-stacked.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-line-stacked.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x2-line.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x2-line.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x3-bubble-3d.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x3-bubble-3d.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x3-bubble.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x3-bubble.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x3-xy-lines-no-markers.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x3-xy-lines-no-markers.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x3-xy-lines.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x3-xy-lines.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x3-xy-smooth-no-markers.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x3-xy-smooth.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x3-xy-smooth.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x3-xy.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x3-xy.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/2x5-radar.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/2x5-radar.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/3x1-pie-exploded.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/3x1-pie-exploded.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/3x1-pie.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/3x1-pie.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/3x2-doughnut-exploded.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/3x2-doughnut-exploded.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/3x2-doughnut.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/3x2-doughnut.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/4x2-multi-cat-bar.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/4x2-multi-cat-bar.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/adjust-ser-count.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/adjust-ser-count.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/cat-labels.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/cat-labels.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/content-types-xml.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/content-types-xml.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/default-notes.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/default-notes.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/default-notesMaster.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/default-notesMaster.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/default-theme.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/default-theme.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/freeform.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/freeform.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/package-rels-xml.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/package-rels-xml.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/placeholders.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/placeholders.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/presentation-rels-xml.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/presentation-rels-xml.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/rels-load-from-xml.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/rels-load-from-xml.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/rewrite-ser.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/rewrite-ser.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/snippets/timing.txt` & `python-petpptx-1.0.1/tests/test_files/snippets/timing.txt`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/test.pptx` & `python-petpptx-1.0.1/tests/test_files/test.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_files/test_slides.pptx` & `python-petpptx-1.0.1/tests/test_files/test_slides.pptx`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_media.py` & `python-petpptx-1.0.1/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_package.py` & `python-petpptx-1.0.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_presentation.py` & `python-petpptx-1.0.1/tests/test_presentation.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_shared.py` & `python-petpptx-1.0.1/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_slide.py` & `python-petpptx-1.0.1/tests/test_slide.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_table.py` & `python-petpptx-1.0.1/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/test_util.py` & `python-petpptx-1.0.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/text/test_fonts.py` & `python-petpptx-1.0.1/tests/text/test_fonts.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/text/test_layout.py` & `python-petpptx-1.0.1/tests/text/test_layout.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/text/test_text.py` & `python-petpptx-1.0.1/tests/text/test_text.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/unitdata.py` & `python-petpptx-1.0.1/tests/unitdata.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/unitutil/cxml.py` & `python-petpptx-1.0.1/tests/unitutil/cxml.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/unitutil/file.py` & `python-petpptx-1.0.1/tests/unitutil/file.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tests/unitutil/mock.py` & `python-petpptx-1.0.1/tests/unitutil/mock.py`

 * *Files identical despite different names*

### Comparing `python-petpptx-1.0.0/tox.ini` & `python-petpptx-1.0.1/tox.ini`

 * *Files identical despite different names*

