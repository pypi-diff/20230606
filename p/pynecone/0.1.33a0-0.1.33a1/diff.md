# Comparing `tmp/pynecone-0.1.33a0.tar.gz` & `tmp/pynecone-0.1.33a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.33a0.tar", max compression
+gzip compressed data, was "pynecone-0.1.33a1.tar", max compression
```

## Comparing `pynecone-0.1.33a0.tar` & `pynecone-0.1.33a1.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.33a0/LICENSE
--rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.33a0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.33a0/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-06-03 03:13:15.297910 pynecone-0.1.33a0/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.33a0/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.33a0/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.33a0/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.33a0/pynecone/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     2558 2023-06-05 21:02:06.179237 pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.33a0/pynecone/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.33a0/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.33a0/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.33a0/pynecone/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.33a0/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0      995 2023-06-01 03:15:26.563786 pynecone-0.1.33a0/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.33a0/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.33a0/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.33a0/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     8262 2023-06-05 21:02:06.181267 pynecone-0.1.33a0/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1448 2023-06-01 03:12:11.084175 pynecone-0.1.33a0/pynecone/__init__.py
--rw-r--r--   0        0        0    20197 2023-06-05 21:02:06.182089 pynecone-0.1.33a0/pynecone/app.py
--rw-r--r--   0        0        0     2524 2023-05-18 00:14:14.759391 pynecone-0.1.33a0/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.33a0/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     6688 2023-06-05 21:02:06.185518 pynecone-0.1.33a0/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.33a0/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     7761 2023-06-01 00:32:59.071818 pynecone-0.1.33a0/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     7062 2023-06-05 21:02:06.186808 pynecone-0.1.33a0/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.33a0/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.33a0/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.33a0/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.33a0/pynecone/components/base/document.py
--rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.33a0/pynecone/components/base/head.py
--rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.33a0/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.33a0/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    24243 2023-06-01 00:32:59.072142 pynecone-0.1.33a0/pynecone/components/component.py
--rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.33a0/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.33a0/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.33a0/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.33a0/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.33a0/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.33a0/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.33a0/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.33a0/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.33a0/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.33a0/pynecone/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.33a0/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.33a0/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.33a0/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.33a0/pynecone/components/disclosure/transition.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.33a0/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.33a0/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.33a0/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.33a0/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.33a0/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.33a0/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.33a0/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1308 2023-06-05 03:00:53.230974 pynecone-0.1.33a0/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.33a0/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.33a0/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.33a0/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      243 2023-06-05 03:00:53.231067 pynecone-0.1.33a0/pynecone/components/forms/date_picker.py
--rw-r--r--   0        0        0      277 2023-06-05 03:00:53.231162 pynecone-0.1.33a0/pynecone/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.33a0/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0      243 2023-06-01 00:48:48.431001 pynecone-0.1.33a0/pynecone/components/forms/email.py
--rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.33a0/pynecone/components/forms/form.py
--rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.33a0/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2880 2023-05-18 00:14:14.761287 pynecone-0.1.33a0/pynecone/components/forms/input.py
--rw-r--r--   0        0        0    12667 2023-06-03 03:13:18.319215 pynecone-0.1.33a0/pynecone/components/forms/multiselect.py
--rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.33a0/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.33a0/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.33a0/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.33a0/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.33a0/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3522 2023-06-03 03:13:18.320175 pynecone-0.1.33a0/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.33a0/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1552 2023-05-18 00:14:14.762398 pynecone-0.1.33a0/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1531 2023-05-18 00:14:14.762541 pynecone-0.1.33a0/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.33a0/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.33a0/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.33a0/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.33a0/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.33a0/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.33a0/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.33a0/pynecone/components/layout/box.py
--rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.33a0/pynecone/components/layout/card.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.33a0/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.33a0/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.33a0/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.33a0/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.33a0/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.33a0/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.33a0/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-05-30 04:03:19.236282 pynecone-0.1.33a0/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.33a0/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.33a0/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.33a0/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.33a0/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.33a0/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.33a0/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0     1391 2023-06-01 03:15:26.564372 pynecone-0.1.33a0/pynecone/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-06-01 03:15:26.564561 pynecone-0.1.33a0/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564687 pynecone-0.1.33a0/pynecone/components/media/audio.py
--rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.33a0/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.33a0/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1774 2023-06-01 03:15:26.564867 pynecone-0.1.33a0/pynecone/components/media/image.py
--rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564984 pynecone-0.1.33a0/pynecone/components/media/video.py
--rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.33a0/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.33a0/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1082 2023-05-26 18:45:47.408434 pynecone-0.1.33a0/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.33a0/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.33a0/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0      887 2023-06-05 21:02:06.187867 pynecone-0.1.33a0/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.33a0/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1016 2023-06-05 21:02:06.187998 pynecone-0.1.33a0/pynecone/components/overlay/banner.py
--rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.33a0/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.33a0/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.33a0/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5688 2023-05-18 00:14:14.764341 pynecone-0.1.33a0/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.33a0/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.33a0/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.33a0/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.33a0/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5018 2023-05-18 00:14:14.764773 pynecone-0.1.33a0/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.33a0/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      304 2023-06-01 00:32:59.073257 pynecone-0.1.33a0/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.33a0/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      682 2023-06-01 00:32:59.073664 pynecone-0.1.33a0/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     3460 2023-06-03 03:13:18.321195 pynecone-0.1.33a0/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.33a0/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.33a0/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     6858 2023-06-05 03:00:53.231552 pynecone-0.1.33a0/pynecone/config.py
--rw-r--r--   0        0        0    10169 2023-06-05 03:00:53.231706 pynecone-0.1.33a0/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.33a0/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.33a0/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.33a0/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.33a0/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.33a0/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1283 2023-05-15 02:04:07.619213 pynecone-0.1.33a0/pynecone/el/element.py
--rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.33a0/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.33a0/pynecone/el/precompile.py
--rw-r--r--   0        0        0    10977 2023-06-03 03:13:18.321601 pynecone-0.1.33a0/pynecone/event.py
--rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.33a0/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.33a0/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.33a0/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2085 2023-06-01 03:12:11.086155 pynecone-0.1.33a0/pynecone/model.py
--rw-r--r--   0        0        0     8431 2023-06-01 03:12:42.958684 pynecone-0.1.33a0/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.33a0/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.33a0/pynecone/route.py
--rw-r--r--   0        0        0    30953 2023-06-05 18:43:43.583090 pynecone-0.1.33a0/pynecone/state.py
--rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.33a0/pynecone/style.py
--rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.33a0/pynecone/utils/__init__.py
--rw-r--r--   0        0        0     7451 2023-06-01 03:12:42.959046 pynecone-0.1.33a0/pynecone/utils/build.py
--rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.33a0/pynecone/utils/console.py
--rw-r--r--   0        0        0     5229 2023-06-01 03:12:42.959181 pynecone-0.1.33a0/pynecone/utils/exec.py
--rw-r--r--   0        0        0    11859 2023-06-01 03:15:26.565621 pynecone-0.1.33a0/pynecone/utils/format.py
--rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.33a0/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.33a0/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0    10033 2023-05-17 03:31:04.698132 pynecone-0.1.33a0/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.33a0/pynecone/utils/processes.py
--rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.33a0/pynecone/utils/telemetry.py
--rw-r--r--   0        0        0     4806 2023-06-01 03:15:26.565774 pynecone-0.1.33a0/pynecone/utils/types.py
--rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.33a0/pynecone/utils/watch.py
--rw-r--r--   0        0        0    30928 2023-05-18 00:14:14.766310 pynecone-0.1.33a0/pynecone/vars.py
--rw-r--r--   0        0        0     1825 2023-06-05 21:02:13.244762 pynecone-0.1.33a0/pyproject.toml
--rw-r--r--   0        0        0     9462 1970-01-01 00:00:00.000000 pynecone-0.1.33a0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.33a1/LICENSE
+-rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.33a1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.33a1/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-06-03 03:13:15.297910 pynecone-0.1.33a1/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.33a1/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.33a1/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.33a1/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.33a1/pynecone/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     2558 2023-06-06 03:55:08.648087 pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.33a1/pynecone/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.33a1/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.33a1/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.33a1/pynecone/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.33a1/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0      995 2023-06-01 03:15:26.563786 pynecone-0.1.33a1/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.33a1/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.33a1/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.33a1/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     8262 2023-06-06 03:55:08.648388 pynecone-0.1.33a1/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1448 2023-06-01 03:12:11.084175 pynecone-0.1.33a1/pynecone/__init__.py
+-rw-r--r--   0        0        0    20112 2023-06-06 03:56:12.966996 pynecone-0.1.33a1/pynecone/app.py
+-rw-r--r--   0        0        0     2524 2023-05-18 00:14:14.759391 pynecone-0.1.33a1/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.33a1/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     6688 2023-06-06 03:55:08.649189 pynecone-0.1.33a1/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.33a1/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     7761 2023-06-01 00:32:59.071818 pynecone-0.1.33a1/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     7062 2023-06-06 03:55:08.649644 pynecone-0.1.33a1/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.33a1/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.33a1/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.33a1/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.33a1/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.33a1/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.33a1/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.33a1/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    24243 2023-06-01 00:32:59.072142 pynecone-0.1.33a1/pynecone/components/component.py
+-rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.33a1/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.33a1/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.33a1/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.33a1/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.33a1/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.33a1/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.33a1/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.33a1/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.33a1/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.33a1/pynecone/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.33a1/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.33a1/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.33a1/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.33a1/pynecone/components/disclosure/transition.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.33a1/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.33a1/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.33a1/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.33a1/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.33a1/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.33a1/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.33a1/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1308 2023-06-06 03:55:08.649928 pynecone-0.1.33a1/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.33a1/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.33a1/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.33a1/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      243 2023-06-06 03:55:08.650277 pynecone-0.1.33a1/pynecone/components/forms/date_picker.py
+-rw-r--r--   0        0        0      277 2023-06-06 03:55:08.650792 pynecone-0.1.33a1/pynecone/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.33a1/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0      243 2023-06-01 00:48:48.431001 pynecone-0.1.33a1/pynecone/components/forms/email.py
+-rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.33a1/pynecone/components/forms/form.py
+-rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.33a1/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2880 2023-05-18 00:14:14.761287 pynecone-0.1.33a1/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0    12667 2023-06-03 03:13:18.319215 pynecone-0.1.33a1/pynecone/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.33a1/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.33a1/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.33a1/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.33a1/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.33a1/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3522 2023-06-03 03:13:18.320175 pynecone-0.1.33a1/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.33a1/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1552 2023-05-18 00:14:14.762398 pynecone-0.1.33a1/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1531 2023-05-18 00:14:14.762541 pynecone-0.1.33a1/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.33a1/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.33a1/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.33a1/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.33a1/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.33a1/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.33a1/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.33a1/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.33a1/pynecone/components/layout/card.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.33a1/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.33a1/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.33a1/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.33a1/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.33a1/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.33a1/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.33a1/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-05-30 04:03:19.236282 pynecone-0.1.33a1/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.33a1/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.33a1/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.33a1/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.33a1/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.33a1/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.33a1/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0     1391 2023-06-01 03:15:26.564372 pynecone-0.1.33a1/pynecone/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-06-01 03:15:26.564561 pynecone-0.1.33a1/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564687 pynecone-0.1.33a1/pynecone/components/media/audio.py
+-rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.33a1/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.33a1/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1774 2023-06-01 03:15:26.564867 pynecone-0.1.33a1/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564984 pynecone-0.1.33a1/pynecone/components/media/video.py
+-rw-r--r--   0        0        0      282 2023-06-06 03:55:08.651124 pynecone-0.1.33a1/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.33a1/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0      753 2023-06-06 03:56:12.967444 pynecone-0.1.33a1/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.33a1/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.33a1/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0      887 2023-06-06 03:55:08.651436 pynecone-0.1.33a1/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.33a1/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1016 2023-06-06 03:55:08.651780 pynecone-0.1.33a1/pynecone/components/overlay/banner.py
+-rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.33a1/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.33a1/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.33a1/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5688 2023-05-18 00:14:14.764341 pynecone-0.1.33a1/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.33a1/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.33a1/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.33a1/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.33a1/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5018 2023-05-18 00:14:14.764773 pynecone-0.1.33a1/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.33a1/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      304 2023-06-01 00:32:59.073257 pynecone-0.1.33a1/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.33a1/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      682 2023-06-01 00:32:59.073664 pynecone-0.1.33a1/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3460 2023-06-03 03:13:18.321195 pynecone-0.1.33a1/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.33a1/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.33a1/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     6858 2023-06-06 03:55:08.652315 pynecone-0.1.33a1/pynecone/config.py
+-rw-r--r--   0        0        0    10169 2023-06-06 03:55:08.652752 pynecone-0.1.33a1/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.33a1/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.33a1/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.33a1/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.33a1/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.33a1/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1320 2023-06-06 03:56:12.968362 pynecone-0.1.33a1/pynecone/el/element.py
+-rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.33a1/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.33a1/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    10977 2023-06-03 03:13:18.321601 pynecone-0.1.33a1/pynecone/event.py
+-rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.33a1/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.33a1/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.33a1/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2085 2023-06-01 03:12:11.086155 pynecone-0.1.33a1/pynecone/model.py
+-rw-r--r--   0        0        0     8431 2023-06-01 03:12:42.958684 pynecone-0.1.33a1/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.33a1/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.33a1/pynecone/route.py
+-rw-r--r--   0        0        0    30953 2023-06-06 03:55:08.653419 pynecone-0.1.33a1/pynecone/state.py
+-rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.33a1/pynecone/style.py
+-rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.33a1/pynecone/utils/__init__.py
+-rw-r--r--   0        0        0     7451 2023-06-01 03:12:42.959046 pynecone-0.1.33a1/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.33a1/pynecone/utils/console.py
+-rw-r--r--   0        0        0     5229 2023-06-01 03:12:42.959181 pynecone-0.1.33a1/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    11859 2023-06-01 03:15:26.565621 pynecone-0.1.33a1/pynecone/utils/format.py
+-rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.33a1/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.33a1/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0    10033 2023-05-17 03:31:04.698132 pynecone-0.1.33a1/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.33a1/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.33a1/pynecone/utils/telemetry.py
+-rw-r--r--   0        0        0     4806 2023-06-01 03:15:26.565774 pynecone-0.1.33a1/pynecone/utils/types.py
+-rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.33a1/pynecone/utils/watch.py
+-rw-r--r--   0        0        0    30928 2023-05-18 00:14:14.766310 pynecone-0.1.33a1/pynecone/vars.py
+-rw-r--r--   0        0        0     1825 2023-06-06 03:56:37.113710 pynecone-0.1.33a1/pyproject.toml
+-rw-r--r--   0        0        0     9462 1970-01-01 00:00:00.000000 pynecone-0.1.33a1/PKG-INFO
```

### Comparing `pynecone-0.1.33a0/LICENSE` & `pynecone-0.1.33a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/README.md` & `pynecone-0.1.33a1/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.33a1/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.33a1/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.33a1/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/index.js.jinja2` & `pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2` & `pynecone-0.1.33a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.33a1/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/.templates/web/package.json` & `pynecone-0.1.33a1/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.33a1/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.33a1/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.33a1/pynecone/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/__init__.py` & `pynecone-0.1.33a1/pynecone/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/app.py` & `pynecone-0.1.33a1/pynecone/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from socketio import ASGIApp, AsyncNamespace, AsyncServer
 
 from pynecone import constants
 from pynecone.base import Base
 from pynecone.compiler import compiler
 from pynecone.compiler import utils as compiler_utils
 from pynecone.components.component import Component, ComponentStyle
-from pynecone.components.overlay.banner import ConnectionBanner
 from pynecone.config import get_config
 from pynecone.event import Event, EventHandler
 from pynecone.middleware import HydrateMiddleware, Middleware
 from pynecone.model import Model
 from pynecone.route import (
     DECORATED_ROUTES,
     catchall_in_route,
@@ -74,15 +73,15 @@
     # Middleware to add to the app.
     middleware: List[Middleware] = []
 
     # List of event handlers to trigger when a page loads.
     load_events: Dict[str, List[EventHandler]] = {}
 
     # The component to render if there is a connection error to the server.
-    connect_error_component: Optional[Component] = ConnectionBanner.create()
+    connect_error_component: Optional[Component] = None
 
     def __init__(self, *args, **kwargs):
         """Initialize the app.
 
         Args:
             *args: Args to initialize the app with.
             **kwargs: Kwargs to initialize the app with.
```

### Comparing `pynecone-0.1.33a0/pynecone/base.py` & `pynecone-0.1.33a1/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/compiler/compiler.py` & `pynecone-0.1.33a1/pynecone/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/compiler/templates.py` & `pynecone-0.1.33a1/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/compiler/utils.py` & `pynecone-0.1.33a1/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/__init__.py` & `pynecone-0.1.33a1/pynecone/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/base/bare.py` & `pynecone-0.1.33a1/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/base/document.py` & `pynecone-0.1.33a1/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/base/link.py` & `pynecone-0.1.33a1/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/base/meta.py` & `pynecone-0.1.33a1/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/component.py` & `pynecone-0.1.33a1/pynecone/components/component.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/datadisplay/code.py` & `pynecone-0.1.33a1/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.33a1/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.33a1/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/datadisplay/list.py` & `pynecone-0.1.33a1/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.33a1/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/datadisplay/table.py` & `pynecone-0.1.33a1/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/datadisplay/tag.py` & `pynecone-0.1.33a1/pynecone/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.33a1/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.33a1/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/disclosure/transition.py` & `pynecone-0.1.33a1/pynecone/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/feedback/alert.py` & `pynecone-0.1.33a1/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.33a1/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/feedback/progress.py` & `pynecone-0.1.33a1/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.33a1/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/feedback/spinner.py` & `pynecone-0.1.33a1/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/__init__.py` & `pynecone-0.1.33a1/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/button.py` & `pynecone-0.1.33a1/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/checkbox.py` & `pynecone-0.1.33a1/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.33a1/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/editable.py` & `pynecone-0.1.33a1/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/form.py` & `pynecone-0.1.33a1/pynecone/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.33a1/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/input.py` & `pynecone-0.1.33a1/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/multiselect.py` & `pynecone-0.1.33a1/pynecone/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/numberinput.py` & `pynecone-0.1.33a1/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/pininput.py` & `pynecone-0.1.33a1/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/radio.py` & `pynecone-0.1.33a1/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.33a1/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/select.py` & `pynecone-0.1.33a1/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/slider.py` & `pynecone-0.1.33a1/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/switch.py` & `pynecone-0.1.33a1/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/textarea.py` & `pynecone-0.1.33a1/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/forms/upload.py` & `pynecone-0.1.33a1/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/graphing/plotly.py` & `pynecone-0.1.33a1/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/graphing/victory.py` & `pynecone-0.1.33a1/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/__init__.py` & `pynecone-0.1.33a1/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/box.py` & `pynecone-0.1.33a1/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/card.py` & `pynecone-0.1.33a1/pynecone/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/cond.py` & `pynecone-0.1.33a1/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/flex.py` & `pynecone-0.1.33a1/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/foreach.py` & `pynecone-0.1.33a1/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/grid.py` & `pynecone-0.1.33a1/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/html.py` & `pynecone-0.1.33a1/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/responsive.py` & `pynecone-0.1.33a1/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/stack.py` & `pynecone-0.1.33a1/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/layout/wrap.py` & `pynecone-0.1.33a1/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/libs/react_player.py` & `pynecone-0.1.33a1/pynecone/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/media/avatar.py` & `pynecone-0.1.33a1/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/media/icon.py` & `pynecone-0.1.33a1/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/media/image.py` & `pynecone-0.1.33a1/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.33a1/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/navigation/link.py` & `pynecone-0.1.33a1/pynecone/components/navigation/link.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A link component."""
 
-from pynecone.components.component import Component
 from pynecone.components.libs.chakra import ChakraComponent
 from pynecone.components.navigation.nextlink import NextLink
-from pynecone.vars import Var
+from pynecone.utils import imports
+from pynecone.vars import BaseVar, Var
 
 
 class Link(ChakraComponent):
     """Link to another page."""
 
     tag = "Link"
 
@@ -17,25 +17,14 @@
     # The page to link to.
     href: Var[str]
 
     # The text to display.
     text: Var[str]
 
     # What the link renders to.
-    as_: Var[str] = "span"  # type: ignore
+    as_: Var[str] = BaseVar.create("{NextLink}", is_local=False)  # type: ignore
 
     # If true, the link will open in new tab.
     is_external: Var[bool]
 
-    @classmethod
-    def create(cls, *children, **props) -> Component:
-        """Create a NextJS link component, wrapping a Chakra link component.
-
-        Args:
-            *children: The children to pass to the component.
-            **props: The attributes to pass to the component.
-
-        Returns:
-            The component.
-        """
-        kwargs = {"href": props.pop("href") if "href" in props else "#"}
-        return NextLink.create(super().create(*children, **props), **kwargs)
+    def _get_imports(self) -> imports.ImportDict:
+        return {**super()._get_imports(), **NextLink(href=self.href)._get_imports()}
```

### Comparing `pynecone-0.1.33a0/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.33a1/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/overlay/__init__.py` & `pynecone-0.1.33a1/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.33a1/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/overlay/banner.py` & `pynecone-0.1.33a1/pynecone/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/overlay/drawer.py` & `pynecone-0.1.33a1/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/overlay/menu.py` & `pynecone-0.1.33a1/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/overlay/modal.py` & `pynecone-0.1.33a1/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/overlay/popover.py` & `pynecone-0.1.33a1/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.33a1/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.33a1/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/tags/tag.py` & `pynecone-0.1.33a1/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/tags/tagless.py` & `pynecone-0.1.33a1/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/typography/highlight.py` & `pynecone-0.1.33a1/pynecone/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/components/typography/markdown.py` & `pynecone-0.1.33a1/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/config.py` & `pynecone-0.1.33a1/pynecone/config.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/constants.py` & `pynecone-0.1.33a1/pynecone/constants.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/el/constants/html.py` & `pynecone-0.1.33a1/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/el/constants/pynecone.py` & `pynecone-0.1.33a1/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/el/constants/react.py` & `pynecone-0.1.33a1/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/el/element.py` & `pynecone-0.1.33a1/pynecone/el/element.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         return dict(
             tag.add_props(
                 **self.event_triggers,
                 key=self.key,
                 id=self.id,
                 style=self.style,
                 class_name=self.class_name,
+                **self.custom_attrs,
             ).set(
                 contents=str(tag.contents),
                 children=[child.render() for child in self.children],
                 props=tag.format_props(),
             )
         )
```

### Comparing `pynecone-0.1.33a0/pynecone/el/elements/__init__.py` & `pynecone-0.1.33a1/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/el/precompile.py` & `pynecone-0.1.33a1/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/event.py` & `pynecone-0.1.33a1/pynecone/event.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.33a1/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/middleware/middleware.py` & `pynecone-0.1.33a1/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/model.py` & `pynecone-0.1.33a1/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/pc.py` & `pynecone-0.1.33a1/pynecone/pc.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/route.py` & `pynecone-0.1.33a1/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/state.py` & `pynecone-0.1.33a1/pynecone/state.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/style.py` & `pynecone-0.1.33a1/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/build.py` & `pynecone-0.1.33a1/pynecone/utils/build.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/console.py` & `pynecone-0.1.33a1/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/exec.py` & `pynecone-0.1.33a1/pynecone/utils/exec.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/format.py` & `pynecone-0.1.33a1/pynecone/utils/format.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/imports.py` & `pynecone-0.1.33a1/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/path_ops.py` & `pynecone-0.1.33a1/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/prerequisites.py` & `pynecone-0.1.33a1/pynecone/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/processes.py` & `pynecone-0.1.33a1/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/telemetry.py` & `pynecone-0.1.33a1/pynecone/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/types.py` & `pynecone-0.1.33a1/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/utils/watch.py` & `pynecone-0.1.33a1/pynecone/utils/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pynecone/vars.py` & `pynecone-0.1.33a1/pynecone/vars.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a0/pyproject.toml` & `pynecone-0.1.33a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.33a0"
+version = "0.1.33a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `pynecone-0.1.33a0/PKG-INFO` & `pynecone-0.1.33a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.33a0
+Version: 0.1.33a1
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

