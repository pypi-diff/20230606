# Comparing `tmp/cmaps-1.0.5.tar.gz` & `tmp/cmaps-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmaps-1.0.5.tar", last modified: Sun Oct 31 14:27:26 2021, max compression
+gzip compressed data, was "cmaps-2.0.0.tar", last modified: Tue Jun  6 11:56:47 2023, max compression
```

## Comparing `cmaps-1.0.5.tar` & `cmaps-2.0.0.tar`

### file list

```diff
@@ -1,304 +1,304 @@
-drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2021-10-31 14:27:26.355548 cmaps-1.0.5/
--rw-r--r--   0 huanghao   (501) staff       (20)    35142 2019-06-05 02:05:34.000000 cmaps-1.0.5/LICENSE
--rw-r--r--   0 huanghao   (501) staff       (20)      203 2021-10-31 14:27:26.355340 cmaps-1.0.5/PKG-INFO
--rw-r--r--   0 huanghao   (501) staff       (20)     2431 2021-10-31 14:20:22.000000 cmaps-1.0.5/README.rst
-drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2021-10-31 14:27:26.306337 cmaps-1.0.5/cmaps/
--rw-r--r--   0 huanghao   (501) staff       (20)       68 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/__init__.py
--rw-r--r--   0 huanghao   (501) staff       (20)       61 2021-10-31 14:27:26.000000 cmaps-1.0.5/cmaps/_version.py
--rw-r--r--   0 huanghao   (501) staff       (20)   254574 2021-10-31 14:27:26.000000 cmaps-1.0.5/cmaps/cmaps.py
--rw-r--r--   0 huanghao   (501) staff       (20)     1047 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormap.py
-drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2021-10-31 14:27:26.304486 cmaps-1.0.5/cmaps/colormaps/
-drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2021-10-31 14:27:26.353410 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/
--rw-r--r--   0 huanghao   (501) staff       (20)     2719 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/3gauss.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2756 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/3saw.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BkBlAqGrYeOrReViWh200.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      289 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlAqGrWh2YeOrReVi22.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1326 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlAqGrYeOrRe.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlAqGrYeOrReVi200.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlGrYeOrReVi200.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1273 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlRe.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlWhRe.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      550 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueDarkOrange18.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      570 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueDarkRed18.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      442 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueGreen14.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5005 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueRed.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5024 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueRedGray.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5155 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueWhiteOrangeRed.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5298 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueYellowRed.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      406 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BrownBlue12.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      178 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/CBR_coldhot.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      178 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/CBR_drywet.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      167 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/CBR_set3.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      178 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/CBR_wet.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      450 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/Cat12.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      258 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/Copyright
--rw-r--r--   0 huanghao   (501) staff       (20)     1579 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GHRSST_anomaly.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      290 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_cool.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1370 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_copper.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1640 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_drywet.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1910 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_gebco.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     6933 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_globe.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      290 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_gray.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      884 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_haxby.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2721 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_hot.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     6933 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_jet.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      560 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_nighttime.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      452 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_no_green.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2180 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_ocean.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      344 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_paired.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      452 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_panoply.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      560 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_polar.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      560 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_red2green.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     6933 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_relief.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     4341 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_relief_oceanonly.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     6933 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_seis.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1100 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_split.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     6933 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_topo.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      560 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_wysiwyg.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5421 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_wysiwygcont.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      175 2019-02-27 23:51:14.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GSFC_landsat_udf_density.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5124 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GrayWhiteGray.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      502 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GreenMagenta16.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     4990 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GreenYellow.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Accent.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Blues.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_BrBG.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_BuGn.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_BuPu.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Dark2.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_GnBu.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Greens.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Greys.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_OrRd.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Oranges.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PRGn.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Paired.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Pastel1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Pastel2.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PiYG.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PuBu.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PuBuGn.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PuOr.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PuRd.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Purples.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_RdBu.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_RdGy.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_RdPu.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_RdYlBu.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_RdYlGn.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Reds.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Set1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Set2.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Set3.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Spectral.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_StepSeq.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_YlGn.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_YlGnBu.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_YlOrBr.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_YlOrRd.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_afmhot.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_autumn.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_bone.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_brg.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_bwr.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_cool.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_coolwarm.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_copper.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_cubehelix.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_flag.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_earth.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_gray.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_heat.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_ncar.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_rainbow.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_stern.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_yarg.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gnuplot.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gnuplot2.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_hot.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_hsv.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_jet.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_ocean.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_pink.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_prism.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_rainbow.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_s3pcpn.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_s3pcpn_l.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_seismic.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_spring.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_sstanom.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_summer.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_terrain.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     8723 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_viridis.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_winter.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3663 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_banded.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3728 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_blu_red.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3628 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_blue_red.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3667 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_bright.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      377 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_gebco.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3691 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_jaisnd.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3492 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_jet.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3738 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_manga.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3358 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_rainbow2.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3694 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_roullet.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3092 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_a.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3287 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_b.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3186 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_c.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2930 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NEO_modis_ndvi.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      325 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NMCRef.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      343 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NMCVel.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3311 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NOC_ndvi.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5239 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/OceanLakeLandSnow.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_Gallet13.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_Lindaa06.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_Lindaa07.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_bhw3_22.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_es_landscape_79.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_feb_sunrise.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_foggy_sunrise.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_fs2006.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      666 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/StepSeq25.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      214 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/UKM_hadcrut.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/ViBlGrWhYeOrRe.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1326 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhBlGrYeRe.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1327 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhBlReWh.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhViBlGrYeOrRe.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhViBlGrYeOrReWh.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5129 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhiteBlue.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5152 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhiteBlueGreenYellowRed.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5125 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhiteGreen.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5131 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhiteYellowOrangeRed.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      207 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/amwg.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     4090 2019-06-05 02:05:34.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/amwg256.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      219 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/amwg_blueyellowred.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      920 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cb_9step.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2832 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cb_rainbow.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2806 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cb_rainbow_inv.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      313 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/circular_0.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      412 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/circular_1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      423 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/circular_2.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     5397 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cividis.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_algae.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_amp.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_balance.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_curl.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_deep.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_delta.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_dense.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_gray.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_haline.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_ice.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_matter.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_oxy.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_phase.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_solar.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_speed.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_tempo.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_thermal.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_turbid.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      734 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmp_b2r.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      257 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmp_flux.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      752 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmp_haxby.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      155 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cosam.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      181 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cosam12.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      129 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cyclic.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      618 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/default.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2719 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/detail.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      518 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/draw_cmap.ncl
--rw-r--r--   0 huanghao   (501) staff       (20)      111 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/drought_severity.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3645 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/example.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2821 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/extrema.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      309 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/grads_default.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      294 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/grads_rainbow.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      153 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/gscyclic.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      927 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/gsdtol.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      927 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/gsltod.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      334 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/gui_default.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2320 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/helix.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2231 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/helix1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      611 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/hlu_default.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      343 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/hotcold_18lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      356 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/hotcolr_19lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2363 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/hotres.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2577 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/lithology.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      793 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/matlab_hot.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      793 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/matlab_hsv.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      793 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/matlab_jet.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      793 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/matlab_lines.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      291 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/mch_default.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     8703 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/ncl_default.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2551 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/ncview_default.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     6096 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/nice_gfdl.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      266 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/nrl_sirkes.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      242 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/nrl_sirkes_nowhite.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      226 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/perc2_9lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      252 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/percent_11lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      232 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/posneg_1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      253 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/posneg_2.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      245 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/prcp_1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      180 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/prcp_2.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      308 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/prcp_3.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      304 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/precip2_15lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      330 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/precip2_17lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      317 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/precip3_16lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      252 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/precip4_11lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      356 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/precip4_diff_19lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      252 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/precip_11lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      265 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/precip_diff_12lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      121 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/precip_diff_1lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     4789 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/psgcap.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      451 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/radar.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      336 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/radar_1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3108 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/rainbow+gray.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3121 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/rainbow+white+gray.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3108 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/rainbow+white.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2471 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/rainbow.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      356 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/rh_19lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      241 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/seaice_1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      192 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/seaice_2.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      299 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/so4_21.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      325 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/so4_23.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      304 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/spread_15lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      246 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/srip_reanalysis.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      226 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/sunshine_9lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      265 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/sunshine_diff_12lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      486 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/t2m_29lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1326 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbrAvg1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbrStd1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbrVar1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbr_240-300.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbr_stdev_0-30.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbr_var_0-500.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1431 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/temp1.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      356 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/temp_19lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      343 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/temp_diff_18lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      121 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/temp_diff_1lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2049 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/testcmap.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2867 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/thelix.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      304 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/topo_15lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     4527 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/uniform.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     3350 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/vegetation_ClarkU.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      294 2019-02-27 23:51:15.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/vegetation_modis.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      193 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/wgne15.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     2614 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/wh-bl-gr-ye-re.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      330 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/wind_17lev.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)     1326 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/ncar_ncl/wxpEnIR.rgb
-drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2021-10-31 14:27:26.355098 cmaps-1.0.5/cmaps/colormaps/self_defined/
--rw-r--r--   0 huanghao   (501) staff       (20)     2248 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/self_defined/Carbone42.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      324 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/self_defined/NMCRef.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      290 2020-03-14 01:35:50.000000 cmaps-1.0.5/cmaps/colormaps/self_defined/NMCVel2.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      424 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/self_defined/NWSRef.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      264 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/self_defined/NWSSPW.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)      467 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/self_defined/NWSVel.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)       57 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/self_defined/TopoGray.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)       40 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/self_defined/TwoClass.rgb
--rw-r--r--   0 huanghao   (501) staff       (20)       44 2019-06-05 02:05:35.000000 cmaps-1.0.5/cmaps/colormaps/self_defined/mask.rgb
-drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2021-10-31 14:27:26.307124 cmaps-1.0.5/cmaps.egg-info/
--rw-r--r--   0 huanghao   (501) staff       (20)      203 2021-10-31 14:27:26.000000 cmaps-1.0.5/cmaps.egg-info/PKG-INFO
--rw-r--r--   0 huanghao   (501) staff       (20)    11767 2021-10-31 14:27:26.000000 cmaps-1.0.5/cmaps.egg-info/SOURCES.txt
--rw-r--r--   0 huanghao   (501) staff       (20)        1 2021-10-31 14:27:26.000000 cmaps-1.0.5/cmaps.egg-info/dependency_links.txt
--rw-r--r--   0 huanghao   (501) staff       (20)       17 2021-10-31 14:27:26.000000 cmaps-1.0.5/cmaps.egg-info/requires.txt
--rw-r--r--   0 huanghao   (501) staff       (20)        6 2021-10-31 14:27:26.000000 cmaps-1.0.5/cmaps.egg-info/top_level.txt
--rw-r--r--   0 huanghao   (501) staff       (20)     2308 2021-10-31 13:57:23.000000 cmaps-1.0.5/cmaps.template
--rw-r--r--   0 huanghao   (501) staff       (20)       38 2021-10-31 14:27:26.355614 cmaps-1.0.5/setup.cfg
--rw-r--r--   0 huanghao   (501) staff       (20)     3382 2021-10-31 14:19:20.000000 cmaps-1.0.5/setup.py
+drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2023-06-06 11:56:47.089432 cmaps-2.0.0/
+-rw-r--r--   0 huanghao   (501) staff       (20)    35142 2019-06-05 02:05:34.000000 cmaps-2.0.0/LICENSE
+-rw-r--r--   0 huanghao   (501) staff       (20)      151 2023-06-06 11:56:47.089179 cmaps-2.0.0/PKG-INFO
+-rw-r--r--   0 huanghao   (501) staff       (20)     2925 2023-06-06 09:42:52.000000 cmaps-2.0.0/README.rst
+drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2023-06-06 11:56:46.992636 cmaps-2.0.0/cmaps/
+-rw-r--r--   0 huanghao   (501) staff       (20)       68 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/__init__.py
+-rw-r--r--   0 huanghao   (501) staff       (20)       61 2023-06-06 11:56:46.000000 cmaps-2.0.0/cmaps/_version.py
+-rw-r--r--   0 huanghao   (501) staff       (20)   204342 2023-06-06 11:56:46.000000 cmaps-2.0.0/cmaps/cmaps.py
+-rw-r--r--   0 huanghao   (501) staff       (20)     1929 2023-06-06 09:10:04.000000 cmaps-2.0.0/cmaps/colormap.py
+drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2023-06-06 11:56:46.989903 cmaps-2.0.0/cmaps/colormaps/
+drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2023-06-06 11:56:47.085588 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/
+-rw-r--r--   0 huanghao   (501) staff       (20)     2719 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/3gauss.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2756 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/3saw.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BkBlAqGrYeOrReViWh200.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      289 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlAqGrWh2YeOrReVi22.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1326 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlAqGrYeOrRe.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlAqGrYeOrReVi200.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlGrYeOrReVi200.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1273 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlRe.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlWhRe.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      550 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueDarkOrange18.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      570 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueDarkRed18.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      442 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueGreen14.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5005 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueRed.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5024 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueRedGray.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5155 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueWhiteOrangeRed.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5298 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueYellowRed.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      406 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BrownBlue12.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      178 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/CBR_coldhot.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      178 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/CBR_drywet.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      167 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/CBR_set3.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      178 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/CBR_wet.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      450 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/Cat12.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      258 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/Copyright
+-rw-r--r--   0 huanghao   (501) staff       (20)     1579 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GHRSST_anomaly.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      290 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_cool.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1370 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_copper.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1640 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_drywet.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1910 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_gebco.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     6933 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_globe.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      290 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_gray.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      884 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_haxby.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2721 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_hot.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     6933 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_jet.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      560 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_nighttime.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      452 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_no_green.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2180 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_ocean.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      344 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_paired.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      452 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_panoply.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      560 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_polar.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      560 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_red2green.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     6933 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_relief.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     4341 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_relief_oceanonly.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     6933 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_seis.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1100 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_split.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     6933 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_topo.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      560 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_wysiwyg.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5421 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_wysiwygcont.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      175 2019-02-27 23:51:14.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GSFC_landsat_udf_density.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5124 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GrayWhiteGray.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      502 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GreenMagenta16.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     4990 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GreenYellow.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Accent.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Blues.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_BrBG.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_BuGn.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_BuPu.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Dark2.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_GnBu.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Greens.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Greys.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_OrRd.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Oranges.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PRGn.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Paired.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Pastel1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Pastel2.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PiYG.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PuBu.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PuBuGn.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PuOr.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PuRd.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Purples.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_RdBu.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_RdGy.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_RdPu.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_RdYlBu.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_RdYlGn.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Reds.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Set1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Set2.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Set3.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Spectral.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_StepSeq.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_YlGn.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_YlGnBu.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_YlOrBr.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_YlOrRd.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_afmhot.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_autumn.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_bone.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_brg.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_bwr.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_cool.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_coolwarm.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_copper.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_cubehelix.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_flag.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_earth.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_gray.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_heat.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_ncar.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_rainbow.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_stern.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_yarg.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gnuplot.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gnuplot2.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_hot.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_hsv.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_jet.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_ocean.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_pink.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_prism.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_rainbow.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_s3pcpn.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_s3pcpn_l.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_seismic.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_spring.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_sstanom.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_summer.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_terrain.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     8723 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_viridis.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3477 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_winter.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3663 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_banded.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3728 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_blu_red.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3628 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_blue_red.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3667 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_bright.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      377 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_gebco.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3691 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_jaisnd.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3492 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_jet.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3738 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_manga.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3358 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_rainbow2.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3694 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_roullet.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3092 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_a.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3287 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_b.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3186 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_c.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2930 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NEO_modis_ndvi.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      325 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NMCRef.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      343 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NMCVel.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3311 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NOC_ndvi.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5239 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/OceanLakeLandSnow.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_Gallet13.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_Lindaa06.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_Lindaa07.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_bhw3_22.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_es_landscape_79.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_feb_sunrise.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_foggy_sunrise.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2662 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_fs2006.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      666 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/StepSeq25.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      214 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/UKM_hadcrut.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/ViBlGrWhYeOrRe.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1326 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhBlGrYeRe.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1327 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhBlReWh.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhViBlGrYeOrRe.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhViBlGrYeOrReWh.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5129 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhiteBlue.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5152 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhiteBlueGreenYellowRed.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5125 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhiteGreen.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5131 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhiteYellowOrangeRed.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      207 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/amwg.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     4090 2019-06-05 02:05:34.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/amwg256.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      219 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/amwg_blueyellowred.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      920 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cb_9step.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2832 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cb_rainbow.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2806 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cb_rainbow_inv.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      313 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/circular_0.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      412 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/circular_1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      423 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/circular_2.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     5397 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cividis.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_algae.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_amp.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_balance.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_curl.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_deep.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_delta.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_dense.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_gray.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_haline.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_ice.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_matter.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_oxy.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_phase.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_solar.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_speed.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_tempo.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_thermal.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3098 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_turbid.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      734 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmp_b2r.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      257 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmp_flux.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      752 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmp_haxby.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      155 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cosam.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      181 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cosam12.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      129 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cyclic.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      618 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/default.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2719 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/detail.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      518 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/draw_cmap.ncl
+-rw-r--r--   0 huanghao   (501) staff       (20)      111 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/drought_severity.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3645 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/example.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2821 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/extrema.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      309 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/grads_default.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      294 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/grads_rainbow.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      153 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/gscyclic.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      927 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/gsdtol.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      927 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/gsltod.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      334 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/gui_default.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2320 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/helix.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2231 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/helix1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      611 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/hlu_default.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      343 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/hotcold_18lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      356 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/hotcolr_19lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2363 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/hotres.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2577 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/lithology.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      793 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/matlab_hot.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      793 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/matlab_hsv.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      793 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/matlab_jet.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      793 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/matlab_lines.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      291 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/mch_default.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     8703 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/ncl_default.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2551 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/ncview_default.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     6096 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/nice_gfdl.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      266 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/nrl_sirkes.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      242 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/nrl_sirkes_nowhite.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      226 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/perc2_9lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      252 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/percent_11lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      232 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/posneg_1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      253 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/posneg_2.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      245 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/prcp_1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      180 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/prcp_2.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      308 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/prcp_3.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      304 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/precip2_15lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      330 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/precip2_17lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      317 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/precip3_16lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      252 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/precip4_11lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      356 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/precip4_diff_19lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      252 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/precip_11lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      265 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/precip_diff_12lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      121 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/precip_diff_1lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     4789 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/psgcap.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      451 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/radar.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      336 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/radar_1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3108 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/rainbow+gray.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3121 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/rainbow+white+gray.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3108 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/rainbow+white.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2471 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/rainbow.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      356 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/rh_19lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      241 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/seaice_1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      192 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/seaice_2.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      299 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/so4_21.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      325 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/so4_23.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      304 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/spread_15lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      246 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/srip_reanalysis.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      226 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/sunshine_9lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      265 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/sunshine_diff_12lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      486 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/t2m_29lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1326 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbrAvg1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbrStd1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1339 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbrVar1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbr_240-300.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbr_stdev_0-30.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2626 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbr_var_0-500.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1431 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/temp1.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      356 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/temp_19lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      343 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/temp_diff_18lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      121 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/temp_diff_1lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2049 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/testcmap.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2867 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/thelix.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      304 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/topo_15lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     4527 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/uniform.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     3350 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/vegetation_ClarkU.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      294 2019-02-27 23:51:15.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/vegetation_modis.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      193 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/wgne15.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     2614 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/wh-bl-gr-ye-re.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      330 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/wind_17lev.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)     1326 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/ncar_ncl/wxpEnIR.rgb
+drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2023-06-06 11:56:47.088808 cmaps-2.0.0/cmaps/colormaps/self_defined/
+-rw-r--r--   0 huanghao   (501) staff       (20)     2248 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/self_defined/Carbone42.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      324 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/self_defined/NMCRef.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      290 2020-03-14 01:35:50.000000 cmaps-2.0.0/cmaps/colormaps/self_defined/NMCVel2.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      424 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/self_defined/NWSRef.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      264 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/self_defined/NWSSPW.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)      467 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/self_defined/NWSVel.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)       57 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/self_defined/TopoGray.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)       40 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/self_defined/TwoClass.rgb
+-rw-r--r--   0 huanghao   (501) staff       (20)       44 2019-06-05 02:05:35.000000 cmaps-2.0.0/cmaps/colormaps/self_defined/mask.rgb
+drwxr-xr-x   0 huanghao   (501) staff       (20)        0 2023-06-06 11:56:46.993623 cmaps-2.0.0/cmaps.egg-info/
+-rw-r--r--   0 huanghao   (501) staff       (20)      151 2023-06-06 11:56:46.000000 cmaps-2.0.0/cmaps.egg-info/PKG-INFO
+-rw-r--r--   0 huanghao   (501) staff       (20)    11767 2023-06-06 11:56:46.000000 cmaps-2.0.0/cmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 huanghao   (501) staff       (20)        1 2023-06-06 11:56:46.000000 cmaps-2.0.0/cmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 huanghao   (501) staff       (20)       27 2023-06-06 11:56:46.000000 cmaps-2.0.0/cmaps.egg-info/requires.txt
+-rw-r--r--   0 huanghao   (501) staff       (20)        6 2023-06-06 11:56:46.000000 cmaps-2.0.0/cmaps.egg-info/top_level.txt
+-rw-r--r--   0 huanghao   (501) staff       (20)     2375 2023-06-06 00:04:13.000000 cmaps-2.0.0/cmaps.template
+-rw-r--r--   0 huanghao   (501) staff       (20)       38 2023-06-06 11:56:47.089486 cmaps-2.0.0/setup.cfg
+-rw-r--r--   0 huanghao   (501) staff       (20)     3174 2023-06-06 05:09:59.000000 cmaps-2.0.0/setup.py
```

### Comparing `cmaps-1.0.5/LICENSE` & `cmaps-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/README.rst` & `cmaps-2.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -82,13 +82,31 @@
         for i, k in enumerate(color):
             plt.subplot(nrows, ncmaps // nrows + 1, i + 1)
             plt.axis('off')
             plt.imshow(a, aspect='auto', cmap=getattr(cmaps, k), origin='lower')
             plt.title(k, rotation=90, fontsize=10)
             plt.title(k, fontsize=10)
         plt.savefig('colormaps.png', dpi=300)
+        plt.close()
 
-Note that "Slicing" function like list or numpy array is supported for cmaps::
+New features:
+
+#. "Slicing" function like list or numpy array is supported for cmaps::
 
     cmaps.amwg256[20:-20:2]
     cmaps.amwg256[-20:20:-2]
 
+#. "add" function for the cmaps are supported now::
+
+    cmaps.amwg256+WhiteBlueGreenYellowRed
+
+#. a cmap can now be interpolated (different from the "resampled" function in the new version of matplotlib which only take the nearest one)::
+
+    cmaps.amwg256.interp(50)
+    cmaps.amwg256.interp(1000)
+
+#. a cmap can now be convert to LinearSegmentedColormap with different number of colors, with part of effect similar to interp::
+
+    cmaps.amwg256.to_seg(N=100)
+
+
+
```

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/3gauss.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/3gauss.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/3saw.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/3saw.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BkBlAqGrYeOrReViWh200.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BkBlAqGrYeOrReViWh200.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlAqGrYeOrRe.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlAqGrYeOrRe.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlAqGrYeOrReVi200.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlAqGrYeOrReVi200.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlGrYeOrReVi200.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlGrYeOrReVi200.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlRe.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlRe.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlWhRe.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlWhRe.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueDarkOrange18.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueDarkOrange18.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueDarkRed18.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueDarkRed18.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueRed.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueRed.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueRedGray.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueRedGray.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueWhiteOrangeRed.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueWhiteOrangeRed.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/BlueYellowRed.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/BlueYellowRed.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GHRSST_anomaly.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GHRSST_anomaly.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_copper.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_copper.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_drywet.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_drywet.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_gebco.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_gebco.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_globe.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_globe.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_haxby.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_haxby.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_hot.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_hot.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_jet.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_jet.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_nighttime.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_nighttime.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_ocean.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_ocean.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_polar.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_polar.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_red2green.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_red2green.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_relief.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_relief.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_relief_oceanonly.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_relief_oceanonly.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_seis.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_seis.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_split.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_split.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_topo.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_topo.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_wysiwyg.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_wysiwyg.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GMT_wysiwygcont.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GMT_wysiwygcont.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GrayWhiteGray.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GrayWhiteGray.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/GreenYellow.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/GreenYellow.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Accent.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Accent.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Blues.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Blues.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_BrBG.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_BrBG.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_BuGn.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_BuGn.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_BuPu.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_BuPu.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Dark2.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Dark2.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_GnBu.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_GnBu.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Greens.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Greens.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Greys.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Greys.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_OrRd.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_OrRd.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Oranges.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Oranges.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PRGn.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PRGn.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Paired.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Paired.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Pastel1.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Pastel1.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Pastel2.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Pastel2.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PiYG.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PiYG.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PuBu.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PuBu.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PuBuGn.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PuBuGn.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PuOr.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PuOr.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_PuRd.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_PuRd.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Purples.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Purples.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_RdBu.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_RdBu.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_RdGy.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_RdGy.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_RdPu.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_RdPu.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_RdYlBu.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_RdYlBu.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_RdYlGn.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_RdYlGn.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Reds.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Reds.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Set1.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Set1.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Set2.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Set2.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Set3.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Set3.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_Spectral.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_Spectral.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_StepSeq.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_StepSeq.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_YlGn.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_YlGn.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_YlGnBu.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_YlGnBu.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_YlOrBr.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_YlOrBr.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_YlOrRd.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_YlOrRd.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_afmhot.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_afmhot.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_autumn.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_autumn.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_bone.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_bone.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_brg.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_brg.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_bwr.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_bwr.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_cool.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_cool.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_coolwarm.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_coolwarm.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_copper.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_copper.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_cubehelix.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_cubehelix.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_flag.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_flag.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_earth.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_earth.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_gray.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_gray.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_heat.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_heat.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_ncar.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_ncar.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_rainbow.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_rainbow.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_stern.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_stern.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gist_yarg.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gist_yarg.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gnuplot.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gnuplot.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_gnuplot2.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_gnuplot2.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_hot.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_hot.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_hsv.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_hsv.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_jet.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_jet.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_ocean.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_ocean.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_pink.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_pink.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_prism.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_prism.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_rainbow.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_rainbow.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_s3pcpn.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_s3pcpn.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_s3pcpn_l.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_s3pcpn_l.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_seismic.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_seismic.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_spring.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_spring.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_sstanom.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_sstanom.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_summer.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_summer.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_terrain.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_terrain.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_viridis.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_viridis.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/MPL_winter.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/MPL_winter.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_banded.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_banded.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_blu_red.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_blu_red.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_blue_red.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_blue_red.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_bright.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_bright.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_jaisnd.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_jaisnd.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_jet.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_jet.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_manga.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_manga.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_rainbow2.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_rainbow2.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NCV_roullet.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NCV_roullet.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_a.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_a.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_b.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_b.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_c.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NEO_div_vegetation_c.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NEO_modis_ndvi.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NEO_modis_ndvi.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/NOC_ndvi.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/NOC_ndvi.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/OceanLakeLandSnow.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/OceanLakeLandSnow.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_Gallet13.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_Gallet13.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_Lindaa06.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_Lindaa06.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_Lindaa07.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_Lindaa07.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_bhw3_22.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_bhw3_22.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_es_landscape_79.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_es_landscape_79.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_feb_sunrise.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_feb_sunrise.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_foggy_sunrise.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_foggy_sunrise.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/SVG_fs2006.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/SVG_fs2006.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/StepSeq25.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/StepSeq25.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/ViBlGrWhYeOrRe.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/ViBlGrWhYeOrRe.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhBlGrYeRe.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhBlGrYeRe.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhBlReWh.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhBlReWh.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhViBlGrYeOrRe.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhViBlGrYeOrRe.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhViBlGrYeOrReWh.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhViBlGrYeOrReWh.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhiteBlue.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhiteBlue.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhiteBlueGreenYellowRed.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhiteBlueGreenYellowRed.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhiteGreen.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhiteGreen.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/WhiteYellowOrangeRed.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/WhiteYellowOrangeRed.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/amwg256.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/amwg256.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cb_9step.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cb_9step.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cb_rainbow.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cb_rainbow.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cb_rainbow_inv.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cb_rainbow_inv.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cividis.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cividis.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_algae.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_algae.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_amp.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_amp.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_balance.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_balance.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_curl.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_curl.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_deep.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_deep.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_delta.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_delta.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_dense.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_dense.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_gray.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_gray.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_haline.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_haline.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_ice.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_ice.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_matter.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_matter.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_oxy.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_oxy.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_phase.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_phase.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_solar.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_solar.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_speed.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_speed.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_tempo.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_tempo.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_thermal.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_thermal.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmocean_turbid.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmocean_turbid.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmp_b2r.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmp_b2r.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/cmp_haxby.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/cmp_haxby.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/default.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/default.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/detail.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/detail.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/draw_cmap.ncl` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/draw_cmap.ncl`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/example.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/example.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/extrema.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/extrema.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/gsdtol.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/gsdtol.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/gsltod.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/gsltod.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/helix.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/helix.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/helix1.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/helix1.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/hlu_default.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/hlu_default.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/hotres.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/hotres.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/lithology.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/lithology.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/matlab_hot.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/matlab_hot.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/matlab_hsv.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/matlab_hsv.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/matlab_jet.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/matlab_jet.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/matlab_lines.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/matlab_lines.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/ncl_default.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/ncl_default.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/ncview_default.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/ncview_default.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/nice_gfdl.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/nice_gfdl.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/psgcap.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/psgcap.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/rainbow+gray.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/rainbow+gray.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/rainbow+white+gray.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/rainbow+white+gray.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/rainbow+white.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/rainbow+white.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/rainbow.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/rainbow.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbrAvg1.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbrAvg1.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbrStd1.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbrStd1.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbrVar1.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbrVar1.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbr_240-300.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbr_240-300.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbr_stdev_0-30.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbr_stdev_0-30.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/tbr_var_0-500.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/tbr_var_0-500.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/temp1.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/temp1.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/testcmap.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/testcmap.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/thelix.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/thelix.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/uniform.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/uniform.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/vegetation_ClarkU.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/vegetation_ClarkU.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/wh-bl-gr-ye-re.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/wh-bl-gr-ye-re.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/ncar_ncl/wxpEnIR.rgb` & `cmaps-2.0.0/cmaps/colormaps/ncar_ncl/wxpEnIR.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps/colormaps/self_defined/Carbone42.rgb` & `cmaps-2.0.0/cmaps/colormaps/self_defined/Carbone42.rgb`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps.egg-info/SOURCES.txt` & `cmaps-2.0.0/cmaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmaps-1.0.5/cmaps.template` & `cmaps-2.0.0/cmaps.template`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os
 import re
 from glob import glob
+from packaging import version
 
+import matplotlib
 import matplotlib.cm
 import numpy as np
 
 from ._version import __version__
 from .colormap import Colormap
 
 CMAPSFILE_DIR = os.path.join(
     os.path.dirname(os.path.abspath(__file__)), 'colormaps')
 USER_CMAPFILE_DIR = os.environ.get('CMAP_DIR')
 
+
+if version.parse(matplotlib.__version__) < version.parse('3.2.0'):
+    raise Exception('cmaps of version {} only supports matplotlib greater than 3.2'.format(__version__))
+
+if version.parse(matplotlib.__version__) >= version.parse('3.7'):
+    get_cmap = matplotlib.colormaps.get_cmap
+    register_cmap = matplotlib.colormaps.register
+else:
+    get_cmap = matplotlib.cm.get_cmap
+    register_cmap = matplotlib.cm.register_cmap
+    
+
 class Cmaps(object):
     """colormaps"""
 
     def __init__(self, ):
         self._parse_cmaps()
         self.__version__ = __version__
 
@@ -41,25 +55,15 @@
                 if cname[0].isdigit() or cname.startswith('_'):
                     cname = 'C' + cname
                 if '-' in cname:
                     cname = cname.replace('-', '_')
                 if '+' in cname:
                     cname = cname.replace('+', '_')
 
-                try:
-                    if cname in matplotlib.cm._cmap_registry:
-                        return matplotlib.cm.get_cmap(cname)
-                except:
-                    pass
                 cmap = Colormap(self._coltbl(cmap_file), name=cname)
-                matplotlib.cm.register_cmap(name=cname, cmap=cmap)
+                register_cmap(name=cname, cmap=cmap)
                 setattr(self, cname, cmap)
 
-                try:
-                    if cname in matplotlib.cm._cmap_registry:
-                        return matplotlib.cm.get_cmap(cname)
-                except:
-                    pass
                 cname = cname + '_r'
                 cmap = Colormap(self._coltbl(cmap_file)[::-1], name=cname)
-                matplotlib.cm.register_cmap(name=cname, cmap=cmap)
+                register_cmap(name=cname, cmap=cmap)
                 setattr(self, cname, cmap)
```

### Comparing `cmaps-1.0.5/setup.py` & `cmaps-2.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from glob import glob
 
 from setuptools import setup
 import os
 
-VERSION = '1.0.5'
+VERSION = '2.0.0'
 CMAPSFILE_DIR = os.path.join('./cmaps/colormaps')
 
 
 def write_version_py(version=VERSION, filename='cmaps/_version.py'):
     cnt = '# THIS FILE IS GENERATED FROM SETUP.PY\n' + \
           '__version__ = "%(version)s"\n'
     a = open(filename, 'w')
@@ -44,36 +44,34 @@
                 cname = cname.replace('-', '_')
             if '+' in cname:
                 cname = cname.replace('+', '_')
             c += '    @property\n'
             c += '    def {}(self):\n'.format(cname)
             c += '        cname = "{}"\n'.format(cname)
             c += '        try:\n'
-            c += '            if cname in matplotlib.cm._cmap_registry:\n'
-            c += '                return matplotlib.cm.get_cmap(cname)\n'
+            c += '            return get_cmap(cname)\n'
             c += '        except:\n'
             c += '            pass\n'
             c += '        cmap_file = {} "{}")\n'.format(
                 l[t]['p'], os.path.basename(cmap_file))
             c += '        cmap = Colormap(self._coltbl(cmap_file), name=cname)\n'
-            c += '        matplotlib.cm.register_cmap(name=cname, cmap=cmap)\n'
+            c += '        register_cmap(name=cname, cmap=cmap)\n'
             c += '        return cmap\n\n'
 
             c += '    @property\n'
             c += '    def {}(self):\n'.format(cname + '_r')
             c += '        cname = "{}"\n'.format(cname + '_r')
             c += '        try:\n'
-            c += '            if cname in matplotlib.cm._cmap_registry:\n'
-            c += '                return matplotlib.cm.get_cmap(cname)\n'
+            c += '            get_cmap(cname)\n'
             c += '        except:\n'
             c += '            pass\n'
             c += '        cmap_file = {} "{}")\n'.format(
                 l[t]['p'], os.path.basename(cmap_file))
             c += '        cmap = Colormap(self._coltbl(cmap_file)[::-1], name=cname)\n'
-            c += '        matplotlib.cm.register_cmap(name=cname, cmap=cmap)\n'
+            c += '        register_cmap(name=cname, cmap=cmap)\n'
             c += '        return cmap\n\n'
 
     cmapspy = './cmaps/cmaps.py'
     with open(cmapspy, 'wt') as fw:
         fw.write(c)
 
 
@@ -88,9 +86,9 @@
     package_data={'cmaps': ['colormaps/ncar_ncl/*',
                             'colormaps/self_defined/*'], },
     data_files=[('', ['cmaps.template', 'LICENSE']),],
     url='',
     license='LICENSE',
     description='',
     long_description='',
-    install_requires=['matplotlib', 'numpy'],
+    install_requires=['matplotlib', 'numpy', 'packaging'],
 )
```

