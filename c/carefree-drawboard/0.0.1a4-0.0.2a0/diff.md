# Comparing `tmp/carefree-drawboard-0.0.1a4.tar.gz` & `tmp/carefree-drawboard-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-drawboard-0.0.1a4.tar", last modified: Mon May 22 14:54:00 2023, max compression
+gzip compressed data, was "carefree-drawboard-0.0.2a0.tar", last modified: Tue Jun  6 05:16:15 2023, max compression
```

## Comparing `carefree-drawboard-0.0.1a4.tar` & `carefree-drawboard-0.0.2a0.tar`

### file list

```diff
@@ -1,245 +1,256 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.838981 carefree-drawboard-0.0.1a4/
--rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.1a4/LICENSE
--rw-rw-rw-   0        0        0      121 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/MANIFEST.in
--rw-rw-rw-   0        0        0     9469 2023-05-22 14:54:00.839977 carefree-drawboard-0.0.1a4/PKG-INFO
--rw-rw-rw-   0        0        0     9186 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.736814 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/
--rw-rw-rw-   0        0        0     9469 2023-05-22 14:53:57.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7667 2023-05-22 14:54:00.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:53:57.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 14:53:57.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      179 2023-05-22 14:53:57.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-22 14:53:57.000000 carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.738808 carefree-drawboard-0.0.1a4/cfdraw/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.742795 carefree-drawboard-0.0.1a4/cfdraw/.web/
--rw-rw-rw-   0        0        0      137 2023-05-13 11:08:39.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/.env
--rw-rw-rw-   0        0        0      143 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/.prettierrc
--rw-rw-rw-   0        0        0      548 2023-05-15 11:41:37.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/index.html
--rw-rw-rw-   0        0        0     1967 2023-05-22 14:36:20.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/package.json
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.747778 carefree-drawboard-0.0.1a4/cfdraw/.web/src/
--rw-rw-rw-   0        0        0     1012 2023-05-14 06:28:56.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/App.tsx
--rw-rw-rw-   0        0        0     1470 2023-05-14 03:25:05.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/BoardPanel.tsx
--rw-rw-rw-   0        0        0     6602 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/_settings.ts
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.752761 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/
--rw-rw-rw-   0        0        0     2316 2023-05-13 11:08:39.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/addImage.ts
--rw-rw-rw-   0        0        0      919 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/addText.ts
--rw-rw-rw-   0        0        0     9398 2023-05-13 11:08:39.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/arrange.ts
--rw-rw-rw-   0        0        0     1806 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/download.ts
--rw-rw-rw-   0        0        0     1979 2023-05-13 11:08:39.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/export.ts
--rw-rw-rw-   0        0        0      236 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/i18n.ts
--rw-rw-rw-   0        0        0     8257 2023-05-22 09:35:32.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/importMeta.ts
--rw-rw-rw-   0        0        0     1838 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/managePlugins.ts
--rw-rw-rw-   0        0        0     5032 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/manageProjects.ts
--rw-rw-rw-   0        0        0      272 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/update.ts
--rw-rw-rw-   0        0        0     1118 2023-05-06 09:50:20.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/uploadImage.ts
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.753757 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.764721 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/
--rw-rw-rw-   0        0        0      504 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-blank.svg
--rw-rw-rw-   0        0        0      615 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-frame.svg
--rw-rw-rw-   0        0        0     1243 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-image.svg
--rw-rw-rw-   0        0        0      837 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-project.svg
--rw-rw-rw-   0        0        0      414 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-text.svg
--rw-rw-rw-   0        0        0      307 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add.svg
--rw-rw-rw-   0        0        0      557 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/arrange.svg
--rw-rw-rw-   0        0        0      257 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/arrow-down.svg
--rw-rw-rw-   0        0        0     1378 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/brush.svg
--rw-rw-rw-   0        0        0      927 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/delete.svg
--rw-rw-rw-   0        0        0      574 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/download.svg
--rw-rw-rw-   0        0        0      770 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/editor.svg
--rw-rw-rw-   0        0        0      711 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/email.svg
--rw-rw-rw-   0        0        0     1346 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/github.svg
--rw-rw-rw-   0        0        0     1270 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/group-editor.svg
--rw-rw-rw-   0        0        0      718 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/meta.svg
--rw-rw-rw-   0        0        0      930 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/multi-editor.svg
--rw-rw-rw-   0        0        0      914 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/project.svg
--rw-rw-rw-   0        0        0      465 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/redo.svg
--rw-rw-rw-   0        0        0     1420 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/settings.svg
--rw-rw-rw-   0        0        0     1104 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/shortcuts.svg
--rw-rw-rw-   0        0        0      466 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/undo.svg
--rw-rw-rw-   0        0        0      464 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/wiki.svg
--rw-rw-rw-   0        0        0     3284 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/image-placeholder.svg
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.765718 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/lottie/
--rw-rw-rw-   0        0        0     6591 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/lottie/icon-loading.json
--rw-rw-rw-   0        0        0     6681 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/lottie/loading-page.json
--rw-rw-rw-   0        0        0     5930 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/nsfw-placeholder.svg
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.772694 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/
--rw-rw-rw-   0        0        0     2796 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFButton.tsx
--rw-rw-rw-   0        0        0      640 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFCircularProgress.tsx
--rw-rw-rw-   0        0        0     2202 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFColorPicker.tsx
--rw-rw-rw-   0        0        0      359 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFDivider.tsx
--rw-rw-rw-   0        0        0      235 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFHeading.tsx
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.773694 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFIcon/
--rw-rw-rw-   0        0        0      546 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFIcon/index.scss
--rw-rw-rw-   0        0        0     1568 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFIcon/index.tsx
--rw-rw-rw-   0        0        0     1484 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFImageUploader.tsx
--rw-rw-rw-   0        0        0      794 2023-05-22 14:32:05.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFInput.tsx
--rw-rw-rw-   0        0        0     1330 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFLoadingPage.tsx
--rw-rw-rw-   0        0        0      984 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFLottie.tsx
--rw-rw-rw-   0        0        0     1441 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFMarkdown.tsx
--rw-rw-rw-   0        0        0     3386 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSelect.tsx
--rw-rw-rw-   0        0        0     5270 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSlider.tsx
--rw-rw-rw-   0        0        0     1600 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSwitch.tsx
--rw-rw-rw-   0        0        0      738 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFText.tsx
--rw-rw-rw-   0        0        0      491 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFTextarea.tsx
--rw-rw-rw-   0        0        0     1007 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFTooltip.tsx
--rw-rw-rw-   0        0        0      185 2023-05-15 08:54:13.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/env.d.ts
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.776683 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/
--rw-rw-rw-   0        0        0     1316 2023-05-14 13:38:46.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useAuth.ts
--rw-rw-rw-   0        0        0     3471 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useDocumentEvents.ts
--rw-rw-rw-   0        0        0     3077 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useFileDropper.ts
--rw-rw-rw-   0        0        0     4410 2023-05-12 10:15:34.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useGridLines.ts
--rw-rw-rw-   0        0        0     3943 2023-05-14 03:25:05.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useInitBoard.ts
--rw-rw-rw-   0        0        0      669 2023-05-12 12:36:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/usePreventDefaults.ts
--rw-rw-rw-   0        0        0     6043 2023-05-19 13:14:54.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/usePython.ts
--rw-rw-rw-   0        0        0    11019 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useSetup.ts
--rw-rw-rw-   0        0        0      163 2023-05-12 12:36:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/index.scss
--rw-rw-rw-   0        0        0      345 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/index.tsx
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.781668 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/
--rw-rw-rw-   0        0        0     1103 2023-05-22 01:50:13.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/add.ts
--rw-rw-rw-   0        0        0      849 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/brush.ts
--rw-rw-rw-   0        0        0     1148 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/download.ts
--rw-rw-rw-   0        0        0     1466 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/index.ts
--rw-rw-rw-   0        0        0      404 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/nodeEditor.ts
--rw-rw-rw-   0        0        0     2556 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/plugins.ts
--rw-rw-rw-   0        0        0     1746 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/projects.ts
--rw-rw-rw-   0        0        0      896 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/settings.ts
--rw-rw-rw-   0        0        0    10266 2023-05-22 01:50:13.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/toast.ts
--rw-rw-rw-   0        0        0     2501 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/tooltip.ts
--rw-rw-rw-   0        0        0     1488 2023-05-21 12:53:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/ui.ts
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.782663 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.785653 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/
--rw-rw-rw-   0        0        0     2195 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx
--rw-rw-rw-   0        0        0     2996 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
--rw-rw-rw-   0        0        0      701 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/MarkdownPlugin.tsx
--rw-rw-rw-   0        0        0     2920 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/PluginGroup.tsx
--rw-rw-rw-   0        0        0     3576 2023-05-19 13:14:54.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
--rw-rw-rw-   0        0        0     1908 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
--rw-rw-rw-   0        0        0      804 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
--rw-rw-rw-   0        0        0     4365 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.791141 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/
--rw-rw-rw-   0        0        0     5887 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/AddPlugin.tsx
--rw-rw-rw-   0        0        0      658 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
--rw-rw-rw-   0        0        0     4581 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
--rw-rw-rw-   0        0        0      800 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
--rw-rw-rw-   0        0        0     4152 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
--rw-rw-rw-   0        0        0     1008 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
--rw-rw-rw-   0        0        0     1259 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
--rw-rw-rw-   0        0        0     1375 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
--rw-rw-rw-   0        0        0     8878 2023-05-22 14:33:43.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
--rw-rw-rw-   0        0        0     5152 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
--rw-rw-rw-   0        0        0     1909 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/ShortcutsPlugin.tsx
--rw-rw-rw-   0        0        0     4271 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
--rw-rw-rw-   0        0        0     1176 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.793134 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.797121 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/
--rw-rw-rw-   0        0        0     1083 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx
--rw-rw-rw-   0        0        0     1262 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/ColorField.tsx
--rw-rw-rw-   0        0        0      881 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/Field.tsx
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.798117 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/ListField/
--rw-rw-rw-   0        0        0      367 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/ListField/index.scss
--rw-rw-rw-   0        0        0     5940 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/ListField/index.tsx
--rw-rw-rw-   0        0        0     2013 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
--rw-rw-rw-   0        0        0     2516 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
--rw-rw-rw-   0        0        0     2276 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
--rw-rw-rw-   0        0        0     1915 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/index.tsx
--rw-rw-rw-   0        0        0     1763 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/utils.ts
--rw-rw-rw-   0        0        0     7706 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Floating.tsx
--rw-rw-rw-   0        0        0      410 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Link.tsx
--rw-rw-rw-   0        0        0    10883 2023-05-22 03:10:27.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Render.tsx
--rw-rw-rw-   0        0        0      214 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/hooks.ts
--rw-rw-rw-   0        0        0     2381 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/index.tsx
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.801108 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/
--rw-rw-rw-   0        0        0     1960 2023-05-06 06:34:44.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/cleanup.ts
--rw-rw-rw-   0        0        0     1450 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/factory.ts
--rw-rw-rw-   0        0        0     4081 2023-05-19 13:14:54.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/renderFilters.ts
--rw-rw-rw-   0        0        0      841 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/react-app-env.d.ts
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.803101 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/
--rw-rw-rw-   0        0        0     1290 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/actions.ts
--rw-rw-rw-   0        0        0     2921 2023-05-14 03:25:05.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.804098 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/interceptors/
--rw-rw-rw-   0        0        0      880 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/interceptors/_python.ts
--rw-rw-rw-   0        0        0      752 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/interceptors/index.ts
--rw-rw-rw-   0        0        0       38 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/reset.d.ts
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.809081 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/
--rw-rw-rw-   0        0        0     5031 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/_python.ts
--rw-rw-rw-   0        0        0     1854 2023-05-21 04:22:06.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/fields.ts
--rw-rw-rw-   0        0        0     2076 2023-05-06 09:11:52.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/meta.ts
--rw-rw-rw-   0        0        0      313 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/misc.ts
--rw-rw-rw-   0        0        0     3910 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/plugins.ts
--rw-rw-rw-   0        0        0      850 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/requests.ts
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.818051 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/
--rw-rw-rw-   0        0        0      792 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/debug.ts
--rw-rw-rw-   0        0        0     1495 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/gridLines.ts
--rw-rw-rw-   0        0        0      578 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/hooks.ts
--rw-rw-rw-   0        0        0     2162 2023-05-17 16:39:19.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/meta.ts
--rw-rw-rw-   0        0        0     7774 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/pluginsInfo.ts
--rw-rw-rw-   0        0        0     1968 2023-05-14 06:28:56.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/projects.ts
--rw-rw-rw-   0        0        0     1888 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/settings.ts
--rw-rw-rw-   0        0        0     9316 2023-05-14 06:28:56.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/socket.ts
--rw-rw-rw-   0        0        0     5090 2023-05-22 14:28:24.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/theme.ts
--rw-rw-rw-   0        0        0     2054 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/ui.ts
--rw-rw-rw-   0        0        0      501 2023-05-04 12:54:31.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/user.ts
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.820044 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/
--rw-rw-rw-   0        0        0      467 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/bem.ts
--rw-rw-rw-   0        0        0     1921 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/constants.ts
--rw-rw-rw-   0        0        0     1266 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/event.ts
--rw-rw-rw-   0        0        0     1822 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/misc.ts
--rw-rw-rw-   0        0        0     2053 2023-05-14 06:28:56.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/toast.ts
--rw-rw-rw-   0        0        0       39 2023-04-27 15:22:09.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/src/vite-env.d.ts
--rw-rw-rw-   0        0        0      656 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/tsconfig.json
--rw-rw-rw-   0        0        0      193 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/tsconfig.node.json
--rw-rw-rw-   0        0        0      103 2023-05-14 02:56:39.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/tsconfig.paths.json
--rw-rw-rw-   0        0        0     2165 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/vite.config.ts
--rw-rw-rw-   0        0        0   272589 2023-05-22 14:39:55.000000 carefree-drawboard-0.0.1a4/cfdraw/.web/yarn.lock
--rw-rw-rw-   0        0        0      475 2023-05-08 06:29:38.000000 carefree-drawboard-0.0.1a4/cfdraw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.821041 carefree-drawboard-0.0.1a4/cfdraw/app/
--rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.1a4/cfdraw/app/__init__.py
--rw-rw-rw-   0        0        0     4826 2023-05-22 14:28:31.000000 carefree-drawboard-0.0.1a4/cfdraw/app/app.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.825027 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/
--rw-rw-rw-   0        0        0      139 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/__init__.py
--rw-rw-rw-   0        0        0     1273 2023-05-15 11:41:37.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/assets.py
--rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/base.py
--rw-rw-rw-   0        0        0     7161 2023-05-19 13:15:29.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/project.py
--rw-rw-rw-   0        0        0     6900 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/queue.py
--rw-rw-rw-   0        0        0     3617 2023-05-22 14:28:17.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/upload.py
--rw-rw-rw-   0        0        0     3985 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/websocket.py
--rw-rw-rw-   0        0        0     1277 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/app/schema.py
--rw-rw-rw-   0        0        0     3518 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/cli.py
--rw-rw-rw-   0        0        0     2550 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/config.py
--rw-rw-rw-   0        0        0     2930 2023-05-22 11:26:26.000000 carefree-drawboard-0.0.1a4/cfdraw/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.827020 carefree-drawboard-0.0.1a4/cfdraw/parsers/
--rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.1a4/cfdraw/parsers/__init__.py
--rw-rw-rw-   0        0        0      710 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/parsers/chakra.py
--rw-rw-rw-   0        0        0    13291 2023-05-06 05:18:28.000000 carefree-drawboard-0.0.1a4/cfdraw/parsers/noli.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.829014 carefree-drawboard-0.0.1a4/cfdraw/plugins/
--rw-rw-rw-   0        0        0       97 2023-05-08 06:29:38.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.831008 carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/
--rw-rw-rw-   0        0        0       52 2023-05-08 06:29:38.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/__init__.py
--rw-rw-rw-   0        0        0     1399 2023-05-08 06:29:38.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/node_validator.py
--rw-rw-rw-   0        0        0     1510 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/sync.py
--rw-rw-rw-   0        0        0     4250 2023-05-21 08:11:29.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/base.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.831008 carefree-drawboard-0.0.1a4/cfdraw/plugins/community/
--rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/community/__init__.py
--rw-rw-rw-   0        0        0     1887 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.833001 carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/
--rw-rw-rw-   0        0        0       76 2023-05-05 11:49:30.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1776 2023-05-19 13:15:22.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/response.py
--rw-rw-rw-   0        0        0      904 2023-05-05 11:49:30.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/send_message.py
--rw-rw-rw-   0        0        0      643 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/timer.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.834994 carefree-drawboard-0.0.1a4/cfdraw/schema/
--rw-rw-rw-   0        0        0       72 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/schema/__init__.py
--rw-rw-rw-   0        0        0     6566 2023-05-18 14:43:58.000000 carefree-drawboard-0.0.1a4/cfdraw/schema/fields.py
--rw-rw-rw-   0        0        0    22856 2023-05-22 09:37:53.000000 carefree-drawboard-0.0.1a4/cfdraw/schema/plugins.py
--rw-rw-rw-   0        0        0     2355 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/schema/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:54:00.838981 carefree-drawboard-0.0.1a4/cfdraw/utils/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/cache.py
--rw-rw-rw-   0        0        0      875 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/console.py
--rw-rw-rw-   0        0        0     2622 2023-05-14 02:59:27.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/exec.py
--rw-rw-rw-   0        0        0     2327 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/misc.py
--rw-rw-rw-   0        0        0      638 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/prerequisites.py
--rw-rw-rw-   0        0        0     1766 2023-04-27 15:22:10.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/processes.py
--rw-rw-rw-   0        0        0     2140 2023-05-17 13:34:09.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/server.py
--rw-rw-rw-   0        0        0     2732 2023-05-04 12:54:25.000000 carefree-drawboard-0.0.1a4/cfdraw/utils/template.py
--rw-rw-rw-   0        0        0      113 2023-05-22 14:54:00.840974 carefree-drawboard-0.0.1a4/setup.cfg
--rw-rw-rw-   0        0        0     1102 2023-05-22 14:51:54.000000 carefree-drawboard-0.0.1a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.052091 carefree-drawboard-0.0.2a0/
+-rw-rw-rw-   0        0        0    11557 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/LICENSE
+-rw-rw-rw-   0        0        0      121 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9436 2023-06-06 05:16:15.053091 carefree-drawboard-0.0.2a0/PKG-INFO
+-rw-rw-rw-   0        0        0     9153 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.932809 carefree-drawboard-0.0.2a0/carefree_drawboard.egg-info/
+-rw-rw-rw-   0        0        0     9436 2023-06-06 05:16:11.000000 carefree-drawboard-0.0.2a0/carefree_drawboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8098 2023-06-06 05:16:14.000000 carefree-drawboard-0.0.2a0/carefree_drawboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:16:11.000000 carefree-drawboard-0.0.2a0/carefree_drawboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 05:16:11.000000 carefree-drawboard-0.0.2a0/carefree_drawboard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      181 2023-06-06 05:16:11.000000 carefree-drawboard-0.0.2a0/carefree_drawboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 05:16:11.000000 carefree-drawboard-0.0.2a0/carefree_drawboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.935807 carefree-drawboard-0.0.2a0/cfdraw/
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.939807 carefree-drawboard-0.0.2a0/cfdraw/.web/
+-rw-rw-rw-   0        0        0      137 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/.env
+-rw-rw-rw-   0        0        0      143 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/.prettierrc
+-rw-rw-rw-   0        0        0      548 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/index.html
+-rw-rw-rw-   0        0        0     1967 2023-06-06 05:00:33.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/package.json
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.944807 carefree-drawboard-0.0.2a0/cfdraw/.web/src/
+-rw-rw-rw-   0        0        0     1012 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/App.tsx
+-rw-rw-rw-   0        0        0     1470 2023-05-29 13:17:22.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/BoardPanel.tsx
+-rw-rw-rw-   0        0        0     7104 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/_settings.ts
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.949808 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/
+-rw-rw-rw-   0        0        0     2316 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/addImage.ts
+-rw-rw-rw-   0        0        0      919 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/addText.ts
+-rw-rw-rw-   0        0        0     9398 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/arrange.ts
+-rw-rw-rw-   0        0        0     1806 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/download.ts
+-rw-rw-rw-   0        0        0     1979 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/export.ts
+-rw-rw-rw-   0        0        0      236 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/i18n.ts
+-rw-rw-rw-   0        0        0     8053 2023-05-29 09:24:41.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/importMeta.ts
+-rw-rw-rw-   0        0        0     1838 2023-05-24 12:14:57.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/managePlugins.ts
+-rw-rw-rw-   0        0        0     5032 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/manageProjects.ts
+-rw-rw-rw-   0        0        0      272 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/update.ts
+-rw-rw-rw-   0        0        0     1186 2023-05-28 03:42:15.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/uploadImage.ts
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.950806 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.962807 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/
+-rw-rw-rw-   0        0        0      504 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/add-blank.svg
+-rw-rw-rw-   0        0        0      615 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/add-frame.svg
+-rw-rw-rw-   0        0        0     1243 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/add-image.svg
+-rw-rw-rw-   0        0        0      837 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/add-project.svg
+-rw-rw-rw-   0        0        0      414 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/add-text.svg
+-rw-rw-rw-   0        0        0      307 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/add.svg
+-rw-rw-rw-   0        0        0      557 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/arrange.svg
+-rw-rw-rw-   0        0        0      257 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/arrow-down.svg
+-rw-rw-rw-   0        0        0     1378 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/brush.svg
+-rw-rw-rw-   0        0        0      233 2023-05-25 12:01:54.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/corner-radius.svg
+-rw-rw-rw-   0        0        0      927 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/delete.svg
+-rw-rw-rw-   0        0        0      574 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/download.svg
+-rw-rw-rw-   0        0        0      770 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/editor.svg
+-rw-rw-rw-   0        0        0      711 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/email.svg
+-rw-rw-rw-   0        0        0     1346 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/github.svg
+-rw-rw-rw-   0        0        0     1270 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/group-editor.svg
+-rw-rw-rw-   0        0        0      856 2023-05-24 02:38:14.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/image.svg
+-rw-rw-rw-   0        0        0      535 2023-05-24 08:30:25.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/import.svg
+-rw-rw-rw-   0        0        0      718 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/meta.svg
+-rw-rw-rw-   0        0        0      930 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/multi-editor.svg
+-rw-rw-rw-   0        0        0      914 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/project.svg
+-rw-rw-rw-   0        0        0      465 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/redo.svg
+-rw-rw-rw-   0        0        0      230 2023-05-25 12:01:54.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/rotate.svg
+-rw-rw-rw-   0        0        0     1420 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/settings.svg
+-rw-rw-rw-   0        0        0     1104 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/shortcuts.svg
+-rw-rw-rw-   0        0        0      466 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/undo.svg
+-rw-rw-rw-   0        0        0      464 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/wiki.svg
+-rw-rw-rw-   0        0        0     3284 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/image-placeholder.svg
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.963807 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/lottie/
+-rw-rw-rw-   0        0        0     6591 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/lottie/icon-loading.json
+-rw-rw-rw-   0        0        0     6681 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/lottie/loading-page.json
+-rw-rw-rw-   0        0        0     5930 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/nsfw-placeholder.svg
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.977813 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/
+-rw-rw-rw-   0        0        0     2794 2023-05-25 02:54:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFButton.tsx
+-rw-rw-rw-   0        0        0      640 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFCircularProgress.tsx
+-rw-rw-rw-   0        0        0     2202 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFColorPicker.tsx
+-rw-rw-rw-   0        0        0      359 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFDivider.tsx
+-rw-rw-rw-   0        0        0      235 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFHeading.tsx
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.979813 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFIcon/
+-rw-rw-rw-   0        0        0      546 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFIcon/index.scss
+-rw-rw-rw-   0        0        0     1568 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFIcon/index.tsx
+-rw-rw-rw-   0        0        0     1524 2023-05-24 08:30:25.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFImageUploader.tsx
+-rw-rw-rw-   0        0        0      794 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFInput.tsx
+-rw-rw-rw-   0        0        0     1328 2023-05-25 02:54:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFLoadingPage.tsx
+-rw-rw-rw-   0        0        0      984 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFLottie.tsx
+-rw-rw-rw-   0        0        0     1441 2023-05-29 13:31:57.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFMarkdown.tsx
+-rw-rw-rw-   0        0        0     3346 2023-05-25 12:01:54.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFSelect.tsx
+-rw-rw-rw-   0        0        0     5215 2023-06-01 05:13:02.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFSlider.tsx
+-rw-rw-rw-   0        0        0     1600 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFSwitch.tsx
+-rw-rw-rw-   0        0        0      606 2023-05-24 08:30:25.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFText.tsx
+-rw-rw-rw-   0        0        0      491 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFTextarea.tsx
+-rw-rw-rw-   0        0        0     1113 2023-05-24 02:38:14.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFTooltip.tsx
+-rw-rw-rw-   0        0        0      185 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/env.d.ts
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.984813 carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/
+-rw-rw-rw-   0        0        0     1307 2023-05-28 03:42:15.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useAuth.ts
+-rw-rw-rw-   0        0        0     3559 2023-05-29 09:46:29.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useDocumentEvents.ts
+-rw-rw-rw-   0        0        0     3077 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useFileDropper.ts
+-rw-rw-rw-   0        0        0     4410 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useGridLines.ts
+-rw-rw-rw-   0        0        0     3938 2023-05-25 12:01:54.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useInitBoard.ts
+-rw-rw-rw-   0        0        0      669 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/usePreventDefaults.ts
+-rw-rw-rw-   0        0        0     6074 2023-05-28 03:42:15.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/usePython.ts
+-rw-rw-rw-   0        0        0    11547 2023-05-28 03:42:15.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useSetup.ts
+-rw-rw-rw-   0        0        0      163 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/index.scss
+-rw-rw-rw-   0        0        0      345 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/index.tsx
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.991092 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/
+-rw-rw-rw-   0        0        0     1103 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/add.ts
+-rw-rw-rw-   0        0        0      849 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/brush.ts
+-rw-rw-rw-   0        0        0     1995 2023-05-25 12:01:54.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/download.ts
+-rw-rw-rw-   0        0        0     1466 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/index.ts
+-rw-rw-rw-   0        0        0      610 2023-05-25 12:01:54.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/nodeEditor.ts
+-rw-rw-rw-   0        0        0     2635 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/plugins.ts
+-rw-rw-rw-   0        0        0     1746 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/projects.ts
+-rw-rw-rw-   0        0        0      896 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/settings.ts
+-rw-rw-rw-   0        0        0    10266 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/toast.ts
+-rw-rw-rw-   0        0        0     2693 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/tooltip.ts
+-rw-rw-rw-   0        0        0     2973 2023-05-25 02:54:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/ui.ts
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.992091 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:14.995091 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/
+-rw-rw-rw-   0        0        0     2195 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx
+-rw-rw-rw-   0        0        0     3161 2023-06-01 05:26:19.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx
+-rw-rw-rw-   0        0        0      701 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/MarkdownPlugin.tsx
+-rw-rw-rw-   0        0        0     2920 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/PluginGroup.tsx
+-rw-rw-rw-   0        0        0     3504 2023-06-01 05:26:19.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
+-rw-rw-rw-   0        0        0     1908 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/QAPlugin.tsx
+-rw-rw-rw-   0        0        0      804 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
+-rw-rw-rw-   0        0        0     5689 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.003092 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/
+-rw-rw-rw-   0        0        0     5887 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/AddPlugin.tsx
+-rw-rw-rw-   0        0        0      658 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
+-rw-rw-rw-   0        0        0      970 2023-05-25 12:01:54.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/BasicEditorPlugin.tsx
+-rw-rw-rw-   0        0        0     4581 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
+-rw-rw-rw-   0        0        0      836 2023-05-25 02:54:13.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
+-rw-rw-rw-   0        0        0     4334 2023-05-25 12:01:54.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
+-rw-rw-rw-   0        0        0     1008 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
+-rw-rw-rw-   0        0        0     1259 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
+-rw-rw-rw-   0        0        0     2268 2023-06-01 05:26:19.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
+-rw-rw-rw-   0        0        0     8878 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
+-rw-rw-rw-   0        0        0     5152 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
+-rw-rw-rw-   0        0        0     1909 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/ShortcutsPlugin.tsx
+-rw-rw-rw-   0        0        0     4555 2023-05-26 09:54:01.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
+-rw-rw-rw-   0        0        0     1176 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.003092 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/components/
+-rw-rw-rw-   0        0        0     2934 2023-05-26 09:54:01.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/components/BasicEditor.tsx
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.006091 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.009091 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/
+-rw-rw-rw-   0        0        0     1083 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx
+-rw-rw-rw-   0        0        0     1262 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/ColorField.tsx
+-rw-rw-rw-   0        0        0      991 2023-05-24 02:38:14.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/Field.tsx
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.010091 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/ImageField/
+-rw-rw-rw-   0        0        0      368 2023-05-24 02:38:14.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/ImageField/index.scss
+-rw-rw-rw-   0        0        0    10124 2023-05-28 16:26:34.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/ImageField/index.tsx
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.011092 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/ListField/
+-rw-rw-rw-   0        0        0      367 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/ListField/index.scss
+-rw-rw-rw-   0        0        0     6480 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/ListField/index.tsx
+-rw-rw-rw-   0        0        0     2013 2023-05-23 11:06:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
+-rw-rw-rw-   0        0        0     2680 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
+-rw-rw-rw-   0        0        0     2279 2023-05-24 02:38:14.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
+-rw-rw-rw-   0        0        0     1915 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/index.tsx
+-rw-rw-rw-   0        0        0     1763 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/utils.ts
+-rw-rw-rw-   0        0        0     7831 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Floating.tsx
+-rw-rw-rw-   0        0        0      410 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Link.tsx
+-rw-rw-rw-   0        0        0    11039 2023-05-29 13:58:37.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Render.tsx
+-rw-rw-rw-   0        0        0      214 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/hooks.ts
+-rw-rw-rw-   0        0        0     2426 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/index.tsx
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.012091 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/utils/
+-rw-rw-rw-   0        0        0     1960 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/utils/cleanup.ts
+-rw-rw-rw-   0        0        0     1450 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/utils/factory.ts
+-rw-rw-rw-   0        0        0     4058 2023-06-01 05:26:19.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/utils/renderFilters.ts
+-rw-rw-rw-   0        0        0      841 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/react-app-env.d.ts
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.013091 carefree-drawboard-0.0.2a0/cfdraw/.web/src/requests/
+-rw-rw-rw-   0        0        0     1290 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/requests/actions.ts
+-rw-rw-rw-   0        0        0     2921 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/requests/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.014092 carefree-drawboard-0.0.2a0/cfdraw/.web/src/requests/interceptors/
+-rw-rw-rw-   0        0        0      880 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/requests/interceptors/_python.ts
+-rw-rw-rw-   0        0        0      752 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/requests/interceptors/index.ts
+-rw-rw-rw-   0        0        0       38 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/reset.d.ts
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.017092 carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/
+-rw-rw-rw-   0        0        0     5124 2023-06-01 05:26:19.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/_python.ts
+-rw-rw-rw-   0        0        0     1855 2023-05-24 02:38:14.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/fields.ts
+-rw-rw-rw-   0        0        0     2155 2023-05-28 16:26:34.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/meta.ts
+-rw-rw-rw-   0        0        0      313 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/misc.ts
+-rw-rw-rw-   0        0        0     3954 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/plugins.ts
+-rw-rw-rw-   0        0        0      850 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/requests.ts
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.029091 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/
+-rw-rw-rw-   0        0        0      792 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/debug.ts
+-rw-rw-rw-   0        0        0     1495 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/gridLines.ts
+-rw-rw-rw-   0        0        0      578 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/hooks.ts
+-rw-rw-rw-   0        0        0     3781 2023-05-28 16:26:34.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/meta.ts
+-rw-rw-rw-   0        0        0     8165 2023-05-29 14:20:20.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/pluginsInfo.ts
+-rw-rw-rw-   0        0        0     1968 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/projects.ts
+-rw-rw-rw-   0        0        0     2353 2023-05-25 02:54:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/settings.ts
+-rw-rw-rw-   0        0        0     9316 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/socket.ts
+-rw-rw-rw-   0        0        0     5550 2023-05-25 02:54:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/theme.ts
+-rw-rw-rw-   0        0        0     2054 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/ui.ts
+-rw-rw-rw-   0        0        0      563 2023-05-28 03:42:15.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/user.ts
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.032091 carefree-drawboard-0.0.2a0/cfdraw/.web/src/utils/
+-rw-rw-rw-   0        0        0      467 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/utils/bem.ts
+-rw-rw-rw-   0        0        0     1915 2023-05-25 02:54:17.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/utils/constants.ts
+-rw-rw-rw-   0        0        0     1266 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/utils/event.ts
+-rw-rw-rw-   0        0        0     1822 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/utils/misc.ts
+-rw-rw-rw-   0        0        0     2053 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/utils/toast.ts
+-rw-rw-rw-   0        0        0       39 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/src/vite-env.d.ts
+-rw-rw-rw-   0        0        0      656 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/tsconfig.json
+-rw-rw-rw-   0        0        0      193 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/tsconfig.node.json
+-rw-rw-rw-   0        0        0      103 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/tsconfig.paths.json
+-rw-rw-rw-   0        0        0     2165 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/vite.config.ts
+-rw-rw-rw-   0        0        0   272587 2023-06-06 05:00:33.000000 carefree-drawboard-0.0.2a0/cfdraw/.web/yarn.lock
+-rw-rw-rw-   0        0        0      475 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.034091 carefree-drawboard-0.0.2a0/cfdraw/app/
+-rw-rw-rw-   0        0        0       20 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/app/__init__.py
+-rw-rw-rw-   0        0        0     4035 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/app/app.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.039093 carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/
+-rw-rw-rw-   0        0        0      139 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     1273 2023-06-01 09:18:17.000000 carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/assets.py
+-rw-rw-rw-   0        0        0      493 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/base.py
+-rw-rw-rw-   0        0        0     6882 2023-06-01 05:26:19.000000 carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/project.py
+-rw-rw-rw-   0        0        0     7095 2023-06-01 05:26:19.000000 carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/queue.py
+-rw-rw-rw-   0        0        0     3808 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/upload.py
+-rw-rw-rw-   0        0        0     3985 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/websocket.py
+-rw-rw-rw-   0        0        0     1277 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/app/schema.py
+-rw-rw-rw-   0        0        0     4284 2023-06-01 05:26:19.000000 carefree-drawboard-0.0.2a0/cfdraw/cli.py
+-rw-rw-rw-   0        0        0     2592 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/config.py
+-rw-rw-rw-   0        0        0     3460 2023-06-01 05:26:19.000000 carefree-drawboard-0.0.2a0/cfdraw/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.041091 carefree-drawboard-0.0.2a0/cfdraw/parsers/
+-rw-rw-rw-   0        0        0       44 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/parsers/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/parsers/chakra.py
+-rw-rw-rw-   0        0        0     6508 2023-06-01 05:26:19.000000 carefree-drawboard-0.0.2a0/cfdraw/parsers/noli.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.042092 carefree-drawboard-0.0.2a0/cfdraw/plugins/
+-rw-rw-rw-   0        0        0      122 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.044090 carefree-drawboard-0.0.2a0/cfdraw/plugins/_internal/
+-rw-rw-rw-   0        0        0       52 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/_internal/__init__.py
+-rw-rw-rw-   0        0        0     1399 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/_internal/node_validator.py
+-rw-rw-rw-   0        0        0     1510 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/_internal/sync.py
+-rw-rw-rw-   0        0        0     3712 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/base.py
+-rw-rw-rw-   0        0        0     1141 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/bindings.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.044090 carefree-drawboard-0.0.2a0/cfdraw/plugins/community/
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/community/__init__.py
+-rw-rw-rw-   0        0        0     1887 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/factory.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.046091 carefree-drawboard-0.0.2a0/cfdraw/plugins/middlewares/
+-rw-rw-rw-   0        0        0       76 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1837 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/middlewares/response.py
+-rw-rw-rw-   0        0        0      967 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/middlewares/send_message.py
+-rw-rw-rw-   0        0        0      643 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/plugins/middlewares/timer.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.048090 carefree-drawboard-0.0.2a0/cfdraw/schema/
+-rw-rw-rw-   0        0        0       72 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/schema/__init__.py
+-rw-rw-rw-   0        0        0     7736 2023-05-25 02:54:17.000000 carefree-drawboard-0.0.2a0/cfdraw/schema/fields.py
+-rw-rw-rw-   0        0        0    23928 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/schema/plugins.py
+-rw-rw-rw-   0        0        0     2355 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/schema/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:16:15.052091 carefree-drawboard-0.0.2a0/cfdraw/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/utils/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/utils/cache.py
+-rw-rw-rw-   0        0        0      875 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/utils/console.py
+-rw-rw-rw-   0        0        0     2622 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/utils/exec.py
+-rw-rw-rw-   0        0        0     2327 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/utils/misc.py
+-rw-rw-rw-   0        0        0      638 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/utils/prerequisites.py
+-rw-rw-rw-   0        0        0     1766 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/utils/processes.py
+-rw-rw-rw-   0        0        0     2140 2023-05-23 11:06:18.000000 carefree-drawboard-0.0.2a0/cfdraw/utils/server.py
+-rw-rw-rw-   0        0        0     2732 2023-06-05 10:27:10.000000 carefree-drawboard-0.0.2a0/cfdraw/utils/template.py
+-rw-rw-rw-   0        0        0      113 2023-06-06 05:16:15.058090 carefree-drawboard-0.0.2a0/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2023-06-06 05:15:37.000000 carefree-drawboard-0.0.2a0/setup.py
```

### Comparing `carefree-drawboard-0.0.1a4/LICENSE` & `carefree-drawboard-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/PKG-INFO` & `carefree-drawboard-0.0.2a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.1a4
+Version: 0.0.2a0
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # carefree-drawboard 🎨
 
-![Stable Diffusion](examples/assets/stable-diffusion.png)
+![Carefree Drawboard][socialify-image]
 
 <div align="center">
 
 <br>
 
 **✨ Build performant, business ready web apps in pure Python.**
 
 <br>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 
-### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Carefree Creator](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/carefree_creator) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
+### [Documentation](https://carefree0910.me/carefree-drawboard-doc/docs/getting-started) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples)
 
 <div align="left">
 
 <br>
 
 ## Installation
 
@@ -156,12 +156,15 @@
 
 My final goal is to make `carefree-drawboard` 🎨 a platform which can be used to build all kinds of AI applications. I know it will be a long journey but it is definitely worth trying.
 
 > And the middle-term goal is to make 🤗 & 🎨 appear together more often. We may think 🤗🎨 as HuggingFace models using a powerful palette to create the world (with AI)!
 
 ## Credits
 
+- [llunalabs](https://www.llunalabs.com/), for the kindeness & community support.
 - [pynecone](https://github.com/pynecone-io/pynecone), which inspires me a lot.
 - [Stable Diffusion](https://github.com/CompVis/stable-diffusion), the foundation of various image generation methods.
 - [Diffusers](https://github.com/huggingface/diffusers), the adopted library for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example.
 - [@liujs1](https://github.com/liujs1), who provides me the nice looking icons.
 - And You! Thank you for watching!
+
+[socialify-image]: https://socialify.git.ci/carefree0910/carefree-drawboard/image?description=1&descriptionEditable=Infinite%20Drawboard%20in%20Python%20🐍&forks=1&issues=1&logo=https%3A%2F%2Fem-content.zobj.net%2Fthumbs%2F240%2Fmicrosoft%2F319%2Fartist-palette_1f3a8.png&name=1&pattern=Floating%20Cogs&stargazers=1&theme=Auto
```

### Comparing `carefree-drawboard-0.0.1a4/README.md` & `carefree-drawboard-0.0.2a0/carefree_drawboard.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,35 @@
+Metadata-Version: 2.1
+Name: carefree-drawboard
+Version: 0.0.2a0
+Summary: 🎨 Infinite Drawboard in Python
+Author: carefree0910
+Author-email: syameimaru.saki@gmail.com
+Keywords: python carefree-learn drawboard
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # carefree-drawboard 🎨
 
-![Stable Diffusion](examples/assets/stable-diffusion.png)
+![Carefree Drawboard][socialify-image]
 
 <div align="center">
 
 <br>
 
 **✨ Build performant, business ready web apps in pure Python.**
 
 <br>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 
-### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Carefree Creator](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/carefree_creator) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
+### [Documentation](https://carefree0910.me/carefree-drawboard-doc/docs/getting-started) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples)
 
 <div align="left">
 
 <br>
 
 ## Installation
 
@@ -146,12 +156,15 @@
 
 My final goal is to make `carefree-drawboard` 🎨 a platform which can be used to build all kinds of AI applications. I know it will be a long journey but it is definitely worth trying.
 
 > And the middle-term goal is to make 🤗 & 🎨 appear together more often. We may think 🤗🎨 as HuggingFace models using a powerful palette to create the world (with AI)!
 
 ## Credits
 
+- [llunalabs](https://www.llunalabs.com/), for the kindeness & community support.
 - [pynecone](https://github.com/pynecone-io/pynecone), which inspires me a lot.
 - [Stable Diffusion](https://github.com/CompVis/stable-diffusion), the foundation of various image generation methods.
 - [Diffusers](https://github.com/huggingface/diffusers), the adopted library for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example.
 - [@liujs1](https://github.com/liujs1), who provides me the nice looking icons.
 - And You! Thank you for watching!
+
+[socialify-image]: https://socialify.git.ci/carefree0910/carefree-drawboard/image?description=1&descriptionEditable=Infinite%20Drawboard%20in%20Python%20🐍&forks=1&issues=1&logo=https%3A%2F%2Fem-content.zobj.net%2Fthumbs%2F240%2Fmicrosoft%2F319%2Fartist-palette_1f3a8.png&name=1&pattern=Floating%20Cogs&stargazers=1&theme=Auto
```

### Comparing `carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/PKG-INFO` & `carefree-drawboard-0.0.2a0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,25 @@
-Metadata-Version: 2.1
-Name: carefree-drawboard
-Version: 0.0.1a4
-Summary: 🎨 Infinite Drawboard in Python
-Author: carefree0910
-Author-email: syameimaru.saki@gmail.com
-Keywords: python carefree-learn drawboard
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # carefree-drawboard 🎨
 
-![Stable Diffusion](examples/assets/stable-diffusion.png)
+![Carefree Drawboard][socialify-image]
 
 <div align="center">
 
 <br>
 
 **✨ Build performant, business ready web apps in pure Python.**
 
 <br>
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 
-### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Carefree Creator](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/carefree_creator) | [Caption & Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/caption_and_diffusion) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet)
+### [Documentation](https://carefree0910.me/carefree-drawboard-doc/docs/getting-started) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples)
 
 <div align="left">
 
 <br>
 
 ## Installation
 
@@ -156,12 +146,15 @@
 
 My final goal is to make `carefree-drawboard` 🎨 a platform which can be used to build all kinds of AI applications. I know it will be a long journey but it is definitely worth trying.
 
 > And the middle-term goal is to make 🤗 & 🎨 appear together more often. We may think 🤗🎨 as HuggingFace models using a powerful palette to create the world (with AI)!
 
 ## Credits
 
+- [llunalabs](https://www.llunalabs.com/), for the kindeness & community support.
 - [pynecone](https://github.com/pynecone-io/pynecone), which inspires me a lot.
 - [Stable Diffusion](https://github.com/CompVis/stable-diffusion), the foundation of various image generation methods.
 - [Diffusers](https://github.com/huggingface/diffusers), the adopted library for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example.
 - [@liujs1](https://github.com/liujs1), who provides me the nice looking icons.
 - And You! Thank you for watching!
+
+[socialify-image]: https://socialify.git.ci/carefree0910/carefree-drawboard/image?description=1&descriptionEditable=Infinite%20Drawboard%20in%20Python%20🐍&forks=1&issues=1&logo=https%3A%2F%2Fem-content.zobj.net%2Fthumbs%2F240%2Fmicrosoft%2F319%2Fartist-palette_1f3a8.png&name=1&pattern=Floating%20Cogs&stargazers=1&theme=Auto
```

### Comparing `carefree-drawboard-0.0.1a4/carefree_drawboard.egg-info/SOURCES.txt` & `carefree-drawboard-0.0.2a0/carefree_drawboard.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,24 +49,28 @@
 cfdraw/.web/src/assets/icons/add-image.svg
 cfdraw/.web/src/assets/icons/add-project.svg
 cfdraw/.web/src/assets/icons/add-text.svg
 cfdraw/.web/src/assets/icons/add.svg
 cfdraw/.web/src/assets/icons/arrange.svg
 cfdraw/.web/src/assets/icons/arrow-down.svg
 cfdraw/.web/src/assets/icons/brush.svg
+cfdraw/.web/src/assets/icons/corner-radius.svg
 cfdraw/.web/src/assets/icons/delete.svg
 cfdraw/.web/src/assets/icons/download.svg
 cfdraw/.web/src/assets/icons/editor.svg
 cfdraw/.web/src/assets/icons/email.svg
 cfdraw/.web/src/assets/icons/github.svg
 cfdraw/.web/src/assets/icons/group-editor.svg
+cfdraw/.web/src/assets/icons/image.svg
+cfdraw/.web/src/assets/icons/import.svg
 cfdraw/.web/src/assets/icons/meta.svg
 cfdraw/.web/src/assets/icons/multi-editor.svg
 cfdraw/.web/src/assets/icons/project.svg
 cfdraw/.web/src/assets/icons/redo.svg
+cfdraw/.web/src/assets/icons/rotate.svg
 cfdraw/.web/src/assets/icons/settings.svg
 cfdraw/.web/src/assets/icons/shortcuts.svg
 cfdraw/.web/src/assets/icons/undo.svg
 cfdraw/.web/src/assets/icons/wiki.svg
 cfdraw/.web/src/assets/lottie/icon-loading.json
 cfdraw/.web/src/assets/lottie/loading-page.json
 cfdraw/.web/src/components/CFButton.tsx
@@ -113,37 +117,41 @@
 cfdraw/.web/src/plugins/_python/PluginGroup.tsx
 cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx
 cfdraw/.web/src/plugins/_python/QAPlugin.tsx
 cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx
 cfdraw/.web/src/plugins/_python/hooks.ts
 cfdraw/.web/src/plugins/_react/AddPlugin.tsx
 cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx
+cfdraw/.web/src/plugins/_react/BasicEditorPlugin.tsx
 cfdraw/.web/src/plugins/_react/BrushPlugin.tsx
 cfdraw/.web/src/plugins/_react/DeletePlugin.tsx
 cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx
 cfdraw/.web/src/plugins/_react/GroupPlugin.tsx
 cfdraw/.web/src/plugins/_react/LinksPlugin.tsx
 cfdraw/.web/src/plugins/_react/MetaPlugin.tsx
 cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx
 cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx
 cfdraw/.web/src/plugins/_react/ShortcutsPlugin.tsx
 cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx
 cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx
+cfdraw/.web/src/plugins/_react/components/BasicEditor.tsx
 cfdraw/.web/src/plugins/components/Floating.tsx
 cfdraw/.web/src/plugins/components/Link.tsx
 cfdraw/.web/src/plugins/components/Render.tsx
 cfdraw/.web/src/plugins/components/hooks.ts
 cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx
 cfdraw/.web/src/plugins/components/Fields/ColorField.tsx
 cfdraw/.web/src/plugins/components/Fields/Field.tsx
 cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
 cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
 cfdraw/.web/src/plugins/components/Fields/TextField.tsx
 cfdraw/.web/src/plugins/components/Fields/index.tsx
 cfdraw/.web/src/plugins/components/Fields/utils.ts
+cfdraw/.web/src/plugins/components/Fields/ImageField/index.scss
+cfdraw/.web/src/plugins/components/Fields/ImageField/index.tsx
 cfdraw/.web/src/plugins/components/Fields/ListField/index.scss
 cfdraw/.web/src/plugins/components/Fields/ListField/index.tsx
 cfdraw/.web/src/plugins/utils/cleanup.ts
 cfdraw/.web/src/plugins/utils/factory.ts
 cfdraw/.web/src/plugins/utils/renderFilters.ts
 cfdraw/.web/src/requests/actions.ts
 cfdraw/.web/src/requests/hooks.ts
@@ -182,14 +190,15 @@
 cfdraw/app/endpoints/upload.py
 cfdraw/app/endpoints/websocket.py
 cfdraw/parsers/__init__.py
 cfdraw/parsers/chakra.py
 cfdraw/parsers/noli.py
 cfdraw/plugins/__init__.py
 cfdraw/plugins/base.py
+cfdraw/plugins/bindings.py
 cfdraw/plugins/factory.py
 cfdraw/plugins/_internal/__init__.py
 cfdraw/plugins/_internal/node_validator.py
 cfdraw/plugins/_internal/sync.py
 cfdraw/plugins/community/__init__.py
 cfdraw/plugins/middlewares/__init__.py
 cfdraw/plugins/middlewares/response.py
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/index.html` & `carefree-drawboard-0.0.2a0/cfdraw/.web/index.html`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/package.json` & `carefree-drawboard-0.0.2a0/cfdraw/.web/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933673469387756%*

 * *Differences: {"'dependencies'": "{'@carefree0910/business': '~0.5.1-alpha.18', '@carefree0910/core': "*

 * *                   "'~0.5.1-alpha.18', '@carefree0910/native': '~0.5.1-alpha.18', "*

 * *                   "'@carefree0910/svg': '~0.5.1-alpha.18'}",*

 * * "'devDependencies'": "{'vite': '^4.3.9'}"}*

```diff
@@ -1,13 +1,13 @@
 {
     "dependencies": {
-        "@carefree0910/business": "~0.5.1-alpha.12",
-        "@carefree0910/core": "~0.5.1-alpha.12",
-        "@carefree0910/native": "~0.5.1-alpha.12",
-        "@carefree0910/svg": "~0.5.1-alpha.12",
+        "@carefree0910/business": "~0.5.1-alpha.18",
+        "@carefree0910/core": "~0.5.1-alpha.18",
+        "@carefree0910/native": "~0.5.1-alpha.18",
+        "@carefree0910/svg": "~0.5.1-alpha.18",
         "@chakra-ui/icons": "^2.0.4",
         "@chakra-ui/react": "^2.2.4",
         "@emotion/react": "^11.9.3",
         "@emotion/styled": "^11.9.3",
         "@svgdotjs/svg.filter.js": "^3.0.8",
         "@svgdotjs/svg.js": "^3.1.1",
         "@svgdotjs/svg.topath.js": "^2.0.3",
@@ -44,15 +44,15 @@
         "@types/react-dom": "18.0.11",
         "@types/react-syntax-highlighter": "^15.5.6",
         "@types/uuid": "^9.0.1",
         "@vitejs/plugin-react": "^3.1.0",
         "rollup-plugin-visualizer": "^5.9.0",
         "sass": "^1.60.0",
         "typescript": "^5.0.3",
-        "vite": "^4.2.0",
+        "vite": "^4.3.9",
         "vite-plugin-svgr": "^2.4.0",
         "vite-tsconfig-paths": "^4.0.8"
     },
     "name": "cfdraw",
     "private": true,
     "scripts": {
         "build": "tsc && vite build",
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/App.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/App.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/BoardPanel.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/BoardPanel.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/_settings.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/_settings.ts`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
   },
   {
     type: "add",
     props: {
       nodeConstraint: "none",
       renderInfo: {
         w: 256,
-        h: 220,
+        h: 190,
         offsetY: 120,
         src: AddIcon,
         tooltip: "add-new-stuff-tooltip",
         pivot: "rt",
         follow: false,
       },
       pluginInfo: {},
@@ -124,14 +124,18 @@
         w: 400,
         h: 400,
         offsetY: 48,
         src: MetaIcon,
         pivot: "rt",
         follow: true,
         keepOpen: true,
+        tooltip: {
+          zh: "显示 Meta 数据",
+          en: "Show Meta Data",
+        },
       },
       pluginInfo: {},
     },
   },
   {
     type: "download",
     props: {
@@ -161,20 +165,38 @@
         follow: true,
       },
       pluginInfo: {},
       noExpand: true,
     },
   },
   {
+    type: "basicEditor",
+    props: {
+      nodeConstraintRules: {
+        some: ["svg", "image", "path", "rectangle", "group", "frame"],
+      },
+      renderInfo: {
+        w: 280,
+        h: 210,
+        src: EditorIcon,
+        tooltip: "basic-editor-tooltip",
+        pivot: "right",
+        follow: true,
+        keepOpen: true,
+      },
+      pluginInfo: {},
+    },
+  },
+  {
     type: "textEditor",
     props: {
       nodeConstraint: "text",
       renderInfo: {
-        w: 300,
-        h: 400,
+        w: 400,
+        h: 420,
         src: EditorIcon,
         tooltip: "text-editor-tooltip",
         pivot: "right",
         follow: true,
       },
       pluginInfo: {},
     },
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/addImage.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/addImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/addText.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/addText.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/arrange.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/arrange.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/download.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/export.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/export.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/importMeta.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/importMeta.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import {
   RectangleShapeNode,
+  getAutoWH,
   getRandomHash,
   isGroupNode,
   isUndefined,
   shallowCopy,
 } from "@carefree0910/core";
 import {
   BoardStore,
@@ -28,22 +29,14 @@
 function updateElapsedTimes(alias: string): void {
   const node = BoardStore.graph.getNode(alias);
   if (!node || isGroupNode(node) || !node.params.meta?.data) return;
   node.params.meta.data.elapsedTimes = { endTime: Date.now() };
   updateMeta(alias, node.params.meta);
 }
 
-function getWHFromContent(content: string, fontSize: number): { w: number; h: number } {
-  const numChars = content.length;
-  const ratio = Math.sqrt(0.75 * numChars);
-  const h = Math.ceil(fontSize * ratio);
-  const w = h * 2;
-  return { w, h };
-}
-
 // consumers
 
 const consumers: Record<MetaType, (input: IImportMeta<any>) => void> = {
   upload: consumeUpload,
   "add.text": consumeAddText,
   "add.blank": consumeAddBlank,
   "add.sketch.path": consumeAddSketchPath,
@@ -92,15 +85,15 @@
   const failed = async () => {
     toastWord("error", Toast_Words["add-text-error-message"]);
   };
   const { addText } = useAddNode({ success, failed });
   metaData.alias = newAlias;
   const content = useDefaultTextContent(lang);
   const fontSize = DEFAULT_FONT_SIZE;
-  const { w, h } = getWHFromContent(content, fontSize);
+  const { w, h } = getAutoWH({ content, fontSize });
   addText({ trace: true })({
     alias: newAlias,
     initColor: textColor,
     lang,
     autoFit: true,
     meta: { type, data: metaData },
     content,
@@ -150,14 +143,15 @@
     results: T,
     getRectangleInfo: (res: T["value"][number]) => INewRectangle,
   ): IPack<T["value"][number]>[] {
     const packs: IPack<T["value"][number]>[] = [];
     results.value.forEach((res, i) => {
       const newAlias = getNewAlias();
       let iMetaData = shallowCopy(metaData);
+      iMetaData.response.index = i;
       iMetaData.response.value = metaData.response.value[i] as any;
       iMetaData.alias = newAlias;
       if (!res.safe) {
         if (results.type === "text") {
           results.value[i].text = `NSFW 🙈 (${results.value[i].reason})`;
         } else {
           results.value[i].url = NSFW_IMAGE_PLACEHOLDER;
@@ -208,15 +202,15 @@
         },
       );
     });
   } else if (metaData.response.type === "text") {
     const fontSize = DEFAULT_FONT_SIZE;
     const packs = gatherPacks(metaData.response, ({ text }) => ({
       autoFit: true,
-      wh: getWHFromContent(text, fontSize),
+      wh: getAutoWH({ content: text, fontSize }),
     }));
     const targets = getArrangements(packs.map(({ rectangle }) => rectangle)).targets;
     packs.forEach(({ res: { text }, alias, metaData }, i) => {
       const isLast = i === packs.length - 1;
       addNewText(alias, text, fontSize, {
         bbox: targets[i].bbox,
         meta: { type, data: metaData },
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/managePlugins.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/managePlugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/manageProjects.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/manageProjects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/actions/uploadImage.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/actions/uploadImage.ts`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import { Requests } from "@/requests/actions";
 import { userStore } from "@/stores/user";
 
 type UploadImageOptions = {
   failed: (e: any) => Promise<void>;
 };
 
-interface IUploadImageResponseData {
+export interface IUploadImageResponseData {
   w: number;
   h: number;
   url: string;
   safe: boolean;
   reason: string;
 }
 
@@ -23,15 +23,19 @@
 ): Promise<IUploadImageResponseData | void> {
   return safeCall(
     async () => {
       const res = await Requests.postForm<{
         success: boolean;
         message: string;
         data: IUploadImageResponseData;
-      }>("_python", "/upload_image", { image: blob, userId: userStore.userId });
+      }>("_python", "/upload_image", {
+        image: blob,
+        userId: userStore.userId,
+        userJson: userStore.json,
+      });
       if (!res.success) {
         toastWord("warning", Toast_Words["upload-image-error-message"], {
           appendix: ` - ${res.message}`,
         });
         throw Error;
       }
       return res.data;
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-frame.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/add-frame.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-image.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/add-image.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/add-project.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/add-project.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/arrange.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/arrange.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/brush.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/brush.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/delete.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/download.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/download.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/editor.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/editor.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/email.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/email.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/github.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/group-editor.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/group-editor.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/meta.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/meta.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/multi-editor.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/multi-editor.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/project.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/project.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/settings.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/icons/shortcuts.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/icons/shortcuts.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/image-placeholder.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/image-placeholder.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/lottie/icon-loading.json` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/lottie/icon-loading.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/lottie/loading-page.json` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/lottie/loading-page.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/assets/nsfw-placeholder.svg` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/assets/nsfw-placeholder.svg`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFButton.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFButton.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import { observer } from "mobx-react-lite";
 import { useState, useCallback } from "react";
 import { Box, Button, ButtonProps, Image, ImageProps } from "@chakra-ui/react";
 
 import iconLoading from "@/assets/lottie/icon-loading.json";
 
 import { Event } from "@/utils/event";
-import { makeVisibilityTransitionProps } from "@/utils/constants";
+import { useVisibilityTransitionProps } from "@/utils/constants";
 import { themeStore } from "@/stores/theme";
 import { settingsStore } from "@/stores/settings";
 import CFLottie from "./CFLottie";
 import CFTooltip from "./CFTooltip";
 
 function CFButton(props: ButtonProps) {
   const { textColor } = themeStore.styles;
@@ -62,15 +62,15 @@
           <Image
             src={src}
             w="100%"
             h="100%"
             draggable={false}
             onLoad={onIconLoaded}
             {...imageProps}
-            {...makeVisibilityTransitionProps({
+            {...useVisibilityTransitionProps({
               visible: iconLoaded,
               opacity: imageProps?.opacity,
             })}
           />
           {children}
           <CFLottie
             w="100%"
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFCircularProgress.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFCircularProgress.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFColorPicker.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFColorPicker.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFIcon/index.scss` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFIcon/index.scss`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFIcon/index.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFIcon/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFImageUploader.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFImageUploader.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import { observer } from "mobx-react-lite";
 
 import { langStore } from "@carefree0910/business";
 
 import { toastWord } from "@/utils/toast";
 import { Toast_Words } from "@/lang/toast";
 import { importMeta } from "@/actions/importMeta";
-import { uploadImage } from "@/actions/uploadImage";
+import { IUploadImageResponseData, uploadImage } from "@/actions/uploadImage";
 
 export interface CFImageUploaderProps {
   className?: string;
   children: ReactNode;
-  onUpload?: (url: string) => void;
+  onUpload?: (res: IUploadImageResponseData) => void;
   addToBoard?: boolean;
 }
 
 const CFImageUploader: React.FC<CFImageUploaderProps> = ({
   className,
   children,
   onUpload,
@@ -30,15 +30,15 @@
         async function failed(e: any): Promise<void> {
           toastWord("error", Toast_Words["upload-image-error-message"], { appendix: ` - ${e}` });
         }
         toastWord("info", Toast_Words["uploading-image-message"]);
         const blob = file as Blob;
         const uploadRes = await uploadImage(blob, { failed });
         if (!uploadRes) return;
-        onUpload?.(uploadRes.url);
+        onUpload?.(uploadRes);
         if (!addToBoard) return;
         importMeta({
           lang: langStore.tgt,
           type: "upload",
           metaData: { ...uploadRes, isDrag: false },
         });
       }}>
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFInput.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFInput.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFLoadingPage.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFLoadingPage.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import { observer } from "mobx-react-lite";
 import { Center, Flex, Spacer } from "@chakra-ui/react";
 
 import { useIsReady } from "@carefree0910/business";
 
 import loadingPage from "@/assets/lottie/loading-page.json";
 
-import { makeVisibilityTransitionProps } from "@/utils/constants";
+import { useVisibilityTransitionProps } from "@/utils/constants";
 import { useSettingsSynced } from "@/stores/settings";
 import { themeStore } from "@/stores/theme";
 import { useIsAllReady } from "@/hooks/useSetup";
 import CFLottie from "./CFLottie";
 
 const CFLoadingPage: React.FC<PropsWithChildren> = ({ children }) => {
   const isReady = useIsReady() && useIsAllReady();
@@ -25,15 +25,15 @@
           w="100%"
           h="100%"
           bg={boardBg}
           zIndex="1000"
           position="absolute"
           direction="column"
           alignContent="center"
-          {...makeVisibilityTransitionProps({ visible: !isReady, second: 0.5 })}>
+          {...useVisibilityTransitionProps({ visible: !isReady, second: 0.5 })}>
           <Spacer />
           <Center>
             <CFLottie hide={!isSynced} animationData={loadingPage} />
           </Center>
           <Spacer />
         </Flex>
       )}
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFLottie.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFLottie.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFMarkdown.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFMarkdown.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSelect.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFSelect.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import { observer } from "mobx-react-lite";
-import { Box, BoxProps, Flex, FlexProps, TextProps } from "@chakra-ui/react";
+import { Box, BoxProps, Flex, FlexProps, FormLabelProps, TooltipProps } from "@chakra-ui/react";
 import { GroupBase, OptionBase, Select } from "chakra-react-select";
 
 import { isUndefined } from "@carefree0910/core";
 
-import { themeStore, useScrollBarSx } from "@/stores/theme";
-import { CFLabel } from "./CFText";
-import CFTooltip from "./CFTooltip";
+import { themeStore, useActiveBorderProps, useScrollBarSx } from "@/stores/theme";
+import CFTooltip, { CFFormLabel } from "./CFTooltip";
 
 interface SelectItem<T> extends OptionBase {
   value: T;
   label: string;
 }
 export type ICFSelect<T, isMulti extends boolean> = Parameters<
   typeof Select<SelectItem<T>, isMulti, GroupBase<SelectItem<T>>>
->[0] & { tooltip?: string; height?: string; fontSize?: string; boxProps?: BoxProps };
+>[0] & {
+  tooltip?: string;
+  height?: string;
+  fontSize?: string;
+  boxProps?: BoxProps;
+  tooltipProps?: Omit<TooltipProps, "children">;
+};
 
 function CFSelect<T, isMulti extends boolean>({
   tooltip,
   height,
   fontSize,
   boxProps,
+  tooltipProps,
   chakraStyles,
   ...others
 }: ICFSelect<T, isMulti>) {
   height ??= "42px";
   fontSize ??= "16px";
   const {
     textColor,
@@ -50,18 +56,15 @@
           control: (provided) => ({
             ...provided,
             color: textColor,
             minHeight: height,
             borderRadius: "0px",
             borderColor: "transparent",
             fontSize,
-            _focus: {
-              borderColor: activeBorderColor,
-              boxShadow: `0 0 0 1px ${activeBorderColor}`,
-            },
+            _focus: useActiveBorderProps(activeBorderColor),
           }),
           menu: (provided) => ({
             ...provided,
             color: textColor,
           }),
           menuList: (provided) => ({
             ...provided,
@@ -70,53 +73,50 @@
           ...chakraStyles,
         }}
         {...others}
       />
     </Box>
   );
   if (isUndefined(tooltip)) return _Select;
-  return <CFTooltip label={tooltip}>{_Select}</CFTooltip>;
+  return (
+    <CFTooltip label={tooltip} {...tooltipProps}>
+      {_Select}
+    </CFTooltip>
+  );
 }
 
 interface ICFScrollableSelect<T, isMulti extends boolean> extends ICFSelect<T, isMulti> {
   label?: string;
   flexProps?: FlexProps;
-  labelProps?: TextProps;
+  labelProps?: FormLabelProps;
 }
 export const CFSrollableSelect = observer(
   <T, isMulti extends boolean>({
     label,
     tooltip,
     flexProps,
     labelProps,
     chakraStyles,
     ...others
   }: ICFScrollableSelect<T, isMulti>) => {
-    const Select = ({ tooltip }: { tooltip?: string }) => (
-      <CFSelect
-        tooltip={tooltip}
-        chakraStyles={{
-          menuList: (provided) => ({
-            ...provided,
-            p: "0px",
-            maxH: "116px",
-            ...useScrollBarSx(),
-          }),
-          ...chakraStyles,
-        }}
-        {...others}
-      />
-    );
-    if (isUndefined(label)) return <Select tooltip={tooltip} />;
+    const menuList = (provided: any) => ({
+      ...provided,
+      p: "0px",
+      maxH: "116px",
+      ...useScrollBarSx(),
+    });
+    if (isUndefined(label)) {
+      return (
+        <CFSelect tooltip={tooltip} chakraStyles={{ menuList, ...chakraStyles }} {...others} />
+      );
+    }
     return (
       <Flex w="100%" h="100%" align="center" {...flexProps}>
-        <CFTooltip label={tooltip}>
-          <CFLabel label={label} {...labelProps} />
-        </CFTooltip>
+        <CFFormLabel label={label} tooltip={{ label: tooltip }} {...labelProps} />
         <Box w="8px" />
-        <Select />
+        <CFSelect chakraStyles={{ menuList, ...chakraStyles }} {...others} />
       </Flex>
     );
   },
 );
 
 export default observer(CFSelect);
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSlider.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFSlider.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 import { observer } from "mobx-react-lite";
 import { useUnmount } from "ahooks";
 import React, { useCallback, useEffect, useState } from "react";
 
 import { BoardStore, useGlobalTransform, useIsReady } from "@carefree0910/business";
 
 import { themeStore } from "@/stores/theme";
-import { CFLabel } from "./CFText";
+import { CFFormLabel } from "./CFTooltip";
 import CFInput from "./CFInput";
-import CFTooltip from "./CFTooltip";
 
 export interface ICFSlider extends FlexProps {
   className?: string;
   min: number;
   max: number;
   value: number;
   step?: number;
@@ -131,17 +130,15 @@
   const {
     textColor,
     sliderColors: { sliderTrackColor, sliderThumbBorderColor, inputBgColor },
   } = themeStore.styles;
 
   return (
     <Flex className={className} align="center" color={textColor} {...props}>
-      <CFTooltip label={tooltip}>
-        <CFLabel label={label} />
-      </CFTooltip>
+      <CFFormLabel label={label} tooltip={{ label: tooltip }} />
       <Slider
         focusThumbOnChange={!iptFocused}
         flex={1}
         h="32px"
         mx="1em"
         value={scale === "linear" ? val : Math.log(val + offset)}
         min={scale === "linear" ? min : Math.log(min + offset)}
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFSwitch.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFSwitch.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/components/CFTooltip.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/components/CFTooltip.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import { observer } from "mobx-react-lite";
 import { FormLabel, FormLabelProps, Tooltip, TooltipProps } from "@chakra-ui/react";
 
+import { isUndefined } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
-import { themeStore } from "@/stores/theme";
+import { themeStore, useLabelProps } from "@/stores/theme";
 
 function CFTooltip({ label, ...others }: TooltipProps) {
   if (typeof label === "string") {
     label = translate(label, langStore.tgt);
   }
   return <Tooltip hasArrow label={label} {...others} />;
 }
 
 interface ICFFormLabel extends FormLabelProps {
-  label: string;
+  label?: string;
   tooltip?: Omit<TooltipProps, "children">;
 }
 export const CFFormLabel = observer(({ label, tooltip, ...others }: ICFFormLabel) => {
   const { textColor } = themeStore.styles;
 
+  if (isUndefined(label)) return null;
   return (
     <CFTooltip {...tooltip}>
       <FormLabel
         mb="0"
         color={textColor}
-        fontSize={others.fontSize ?? "14px"}
         userSelect="none"
+        {...useLabelProps(others.fontSize)}
         {...others}>
         {label}
       </FormLabel>
     </CFTooltip>
   );
 });
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useAuth.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useAuth.ts`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 import { useEffect } from "react";
 
+import type { IUserStore } from "@/stores/user";
 import { Event } from "@/utils/event";
 import { cleanURL, getEnv } from "@/utils/misc";
 
-type Message = {
-  userId: string;
-};
-
 const allowedOrigins = ["http://127.0.0.1:5123", "http://localhost:5123"];
 const allowedOriginRegexList = [/^http:\/\/localhost(:\d+)?$/];
 let envAllowedOrigins = getEnv("CFDRAW_ALLOWED_ORIGINS");
 if (!envAllowedOrigins) {
   // THIS IS DANGEROUS, but will be convenient for quick deployment
   envAllowedOrigins = window.location.origin;
 }
 allowedOrigins.push(...envAllowedOrigins.split(",").map(cleanURL));
 
 function isAllowedOrigin(origin: string): boolean {
   if (allowedOrigins.includes(origin)) return true;
   return allowedOriginRegexList.some((regex) => regex.test(origin));
 }
 
-export const authEvent = new Event<Message>();
+export const authEvent = new Event<IUserStore>();
 export const useAuth = () => {
   useEffect(() => {
-    const onMessage = (e: MessageEvent<Partial<Message>>) => {
+    const onMessage = (e: MessageEvent<IUserStore | any>) => {
       if (!isAllowedOrigin(e.origin)) {
         console.error(`unauthorized origin: ${e.origin}`);
         return;
       }
       if (e.data.userId) {
-        authEvent.emit({ userId: e.data.userId });
+        authEvent.emit(e.data);
       }
     };
 
     window.addEventListener("message", onMessage);
 
     return () => {
       window.removeEventListener("message", onMessage);
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useDocumentEvents.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useDocumentEvents.ts`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,41 @@
 import { makeObservable, observable } from "mobx";
 
 import { isUndefined } from "@carefree0910/core";
 import { ABCStore, BoardStore, useIsReady } from "@carefree0910/business";
 
 import type { ReactPlugins } from "@/schema/plugins";
 import { useReactPluginSettings } from "@/_settings";
-import { usePythonPluginSettings } from "@/stores/settings";
-import { setPluginExpanded, usePluginParent, usePluginsExpanded } from "@/stores/pluginsInfo";
+import { useFlattenedPythonPluginSettings } from "@/stores/settings";
+import {
+  setPluginExpanded,
+  usePluginIsExpanded,
+  usePluginParent,
+  usePluginsExpanded,
+} from "@/stores/pluginsInfo";
 import { collapseAllPlugins } from "@/actions/managePlugins";
 
 // helpers
 
 function smartCollapse(): void {
   const currentExpanded = usePluginsExpanded();
   const expanding = Object.keys(currentExpanded).find((key) => currentExpanded[key]);
   collapseAllPlugins({
     exceptReactPlugins: (["brush"] as ReactPlugins[]).concat(
       useReactPluginSettings()
         .filter((s) => s.props.renderInfo.keepOpen)
         .map((s) => s.type),
     ),
-    exceptIdentifiers: usePythonPluginSettings()
+    exceptIdentifiers: useFlattenedPythonPluginSettings()
       .filter((s) => s.props.renderInfo.keepOpen)
       .map((s) => s.props.pluginInfo.identifier),
   });
   if (!isUndefined(expanding)) {
     const parent = usePluginParent(expanding);
-    if (!isUndefined(parent)) {
+    if (!isUndefined(parent) && !usePluginIsExpanded(expanding)) {
       setPluginExpanded(parent, true);
     }
   }
 }
 
 // pointer
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useFileDropper.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useFileDropper.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useGridLines.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useGridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useInitBoard.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useInitBoard.ts`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     } else {
       const graph = Graph.fromJsonInfo(shallowCopy(initial.graphInfo));
       graph.allSingleNodes.forEach((node) => {
         if (node.type === "image") {
           node.renderParams.placeholder = IMAGE_PLACEHOLDER;
         }
       });
-      await unittest.renderGraph(graph, undefined, onEvents);
+      await unittest.renderGraph(graph, null, onEvents);
     }
 
     // setup options
     const storeOptions: BoardStoresOptions = {
       constantsOpt: {
         env: IS_PROD ? "production" : "development",
       },
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/usePreventDefaults.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/usePreventDefaults.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/usePython.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/usePython.ts`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,15 @@
   }
   const getNodeDataOpt: IGetNodeData = { exportBox, ...opt };
   const nodeData = needExportNodeData ? await getNodeData(node, getNodeDataOpt) : {};
   const nodeDataList =
     !needExportNodeData || nodes.length <= 1 ? [] : await getNodeDataList(nodes, getNodeDataOpt);
   return {
     userId: userStore.userId,
+    userJson: userStore.json,
     baseURL: getBaseURL(),
     identifier,
     nodeData,
     nodeDataList,
     extraData: getExtraRequestData ? getExtraRequestData() : {},
   };
 }
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/hooks/useSetup.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/hooks/useSetup.ts`

 * *Files 7% similar despite different names*

```diff
@@ -94,17 +94,17 @@
     userId = getRandomHash().toString();
     localStorage.setItem(USER_ID_KEY, userId);
   }
   window.postMessage({ userId }, window.location.origin);
 };
 const useUserInitialization = () => {
   useEffect(() => {
-    const { dispose } = authEvent.on(({ userId }) => {
-      Logger.debug(`user id: ${userId}`);
-      userStore.updateProperty("userId", userId);
+    const { dispose } = authEvent.on((data) => {
+      Logger.debug(`user data: ${JSON.stringify(data)}`);
+      userStore.updateProperty(data);
     });
     if (debugStore.postPseduoUserId) {
       postPseduoUserId();
     }
 
     return dispose;
   }, []);
@@ -189,27 +189,29 @@
   return true;
 };
 
 //// sync from python
 function useSyncPython() {
   const hash = "0";
   const userId = userStore.userId;
+  const userJson = userStore.json;
   const getMessage = useCallback(
     (): Promise<IPythonSocketRequest> =>
       Promise.resolve({
         hash,
-        userId: userStore.userId,
+        userId,
+        userJson,
         baseURL: getBaseURL(),
         identifier: "sync",
         nodeData: {},
         nodeDataList: [],
         extraData: {},
         isInternal: true,
       }),
-    [],
+    [userId, userJson],
   );
   const onMessage = useCallback<IPythonOnSocketMessage<ISettingsStore>>(
     async ({ status, total, pending, message, data: { final } }) => {
       collapseAllPlugins();
       if (status !== "finished") {
         if (status === "pending") {
           Logger.warn(`sync pending: ${pending} / ${total}`);
@@ -300,32 +302,47 @@
 
 //// check whether all icons of react plugins have loaded
 function useCheckIconLoaded() {
   const loaded = useRef<string[]>([]);
   const reactPlugins = useReactPluginSettings();
 
   useEffect(() => {
+    let timer: any;
+    const onLoad = (message: string) => {
+      Logger.debug(`${message} (loaded: ${loaded.current.join(", ")})`);
+      setupStore.updateProperty("iconLoaded", true);
+      bypassIconLoadedEvent = true;
+      clearTimeout(timer);
+    };
+    // check whether all icons have loaded
+    let bypassIconLoadedEvent = false;
     const { dispose } = iconLoadedEvent.on(({ id }) => {
+      if (bypassIconLoadedEvent) return;
       loaded.current.push(id);
       if (
         reactPlugins.every(
           ({
             type,
             props: {
               renderInfo: { follow },
             },
           }) => follow || loaded.current.some((id) => id.startsWith(type)),
         )
       ) {
-        Logger.debug(`all icons loaded: ${loaded.current.join(", ")}}`);
-        setupStore.updateProperty("iconLoaded", true);
-        dispose();
+        onLoad("all icons loaded");
       }
     });
-    return dispose;
+    // set timeout to load the page anyway
+    timer = setTimeout(() => {
+      onLoad("load the page anyway after 1 seconds");
+    }, 1000);
+    return () => {
+      dispose();
+      clearTimeout(timer);
+    };
   }, [reactPlugins]);
 }
 
 //// preload image placeholder
 function usePreloadImagePlaceholder() {
   useEffect(() => {
     const placeholder = new Image();
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/add.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/add.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/brush.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/brush.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/index.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/plugins.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/plugins.ts`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     download: "下载",
     delete: "删除",
     wiki: "文档",
     email: "邮件",
     github: "Github",
     shortcuts: "快捷键",
     logo: "Logo",
+    basicEditor: "编辑基础属性",
     textEditor: "编辑文本",
     groupEditor: "编辑组",
     multiEditor: "编辑多节点",
     brush: "画笔",
     "_python.pluginGroup": "Python 插件组",
     "_python.fields": "Python 插件",
     "_python.textArea": "Python 文本框",
@@ -40,14 +41,15 @@
     download: "Download",
     delete: "Delete",
     wiki: "Wiki",
     email: "Email",
     github: "Github",
     shortcuts: "Shortcuts",
     logo: "Logo",
+    basicEditor: "Edit Basic Fields",
     textEditor: "Edit Text",
     groupEditor: "Edit Group",
     multiEditor: "Edit Multi Nodes",
     brush: "Brush",
     "_python.pluginGroup": "Python Plugin Group",
     "_python.fields": "Python Plugin",
     "_python.textArea": "Python TextArea",
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/projects.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/settings.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/toast.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/lang/tooltip.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/lang/tooltip.ts`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 export enum Tooltip_Words {
   "settings-tooltip" = "settings-tooltip",
   "project-management-tooltip" = "project-management-tooltip",
   "add-new-stuff-tooltip" = "add-new-stuff-tooltip",
   "enter-sketch-mode-tooltip" = "enter-sketch-mode-tooltip",
   "undo-tooltip" = "undo-tooltip",
   "redo-tooltip" = "redo-tooltip",
+  "basic-editor-tooltip" = "basic-editor-tooltip",
   "text-editor-tooltip" = "text-editor-tooltip",
   "ungroup-the-nodes-tooltip" = "ungroup-the-nodes-tooltip",
   "group-the-nodes-tooltip" = "group-the-nodes-tooltip",
   "auto-arrange-tooltip" = "auto-arrange-tooltip",
   "wiki-tooltip" = "wiki-tooltip",
   "email-tooltip" = "email-tooltip",
   "github-tooltip" = "github-tooltip",
@@ -21,14 +22,15 @@
   zh: {
     [Tooltip_Words["settings-tooltip"]]: "设置",
     [Tooltip_Words["project-management-tooltip"]]: "项目管理",
     [Tooltip_Words["add-new-stuff-tooltip"]]: "添加新的元素",
     [Tooltip_Words["enter-sketch-mode-tooltip"]]: "进入涂鸦模式",
     [Tooltip_Words["undo-tooltip"]]: "撤销",
     [Tooltip_Words["redo-tooltip"]]: "重做",
+    [Tooltip_Words["basic-editor-tooltip"]]: "基础属性编辑器",
     [Tooltip_Words["text-editor-tooltip"]]: "文本编辑器",
     [Tooltip_Words["ungroup-the-nodes-tooltip"]]: "解组",
     [Tooltip_Words["group-the-nodes-tooltip"]]: "打组",
     [Tooltip_Words["auto-arrange-tooltip"]]: "自动排列",
     [Tooltip_Words["wiki-tooltip"]]: "Wiki",
     [Tooltip_Words["email-tooltip"]]: "Email",
     [Tooltip_Words["github-tooltip"]]: "Github",
@@ -37,14 +39,15 @@
   en: {
     [Tooltip_Words["settings-tooltip"]]: "Settings",
     [Tooltip_Words["project-management-tooltip"]]: "Project Management",
     [Tooltip_Words["add-new-stuff-tooltip"]]: "Add new stuff",
     [Tooltip_Words["enter-sketch-mode-tooltip"]]: "Enter Sketch Mode",
     [Tooltip_Words["undo-tooltip"]]: "Undo",
     [Tooltip_Words["redo-tooltip"]]: "Redo",
+    [Tooltip_Words["basic-editor-tooltip"]]: "Basic Fields Editor",
     [Tooltip_Words["text-editor-tooltip"]]: "Text Editor",
     [Tooltip_Words["ungroup-the-nodes-tooltip"]]: "Ungroup the Nodes",
     [Tooltip_Words["group-the-nodes-tooltip"]]: "Group the Nodes",
     [Tooltip_Words["auto-arrange-tooltip"]]: "Auto Arrange",
     [Tooltip_Words["wiki-tooltip"]]: "Wiki",
     [Tooltip_Words["email-tooltip"]]: "Email",
     [Tooltip_Words["github-tooltip"]]: "Github",
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/ChatPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/FieldsPlugin.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -13,39 +13,40 @@
 import { usePluginIds, usePluginTaskCache } from "@/stores/pluginsInfo";
 import { parseIStr } from "@/actions/i18n";
 import { importMeta } from "@/actions/importMeta";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "@/plugins/utils/factory";
 import { useClosePanel } from "../components/hooks";
 import { Definitions } from "../components/Fields";
-import { useDefinitionsRequestDataFn } from "./hooks";
+import { useDefinitionsGetInjectionsFn, useDefinitionsRequestDataFn } from "./hooks";
 import PythonPluginWithSubmit from "./PluginWithSubmit";
 
 const PythonFieldsPlugin = ({ pluginInfo, ...props }: IPythonFieldsPlugin) => {
   const { id, pureIdentifier } = usePluginIds(pluginInfo.identifier);
   const lang = langStore.tgt;
   const { definitions } = pluginInfo;
   const getExtraRequestData = useDefinitionsRequestDataFn(definitions);
+  const getInjections = useDefinitionsGetInjectionsFn(definitions);
   const emitClose = useClosePanel(id);
   const taskCache = usePluginTaskCache(id);
 
   const onFinished = useCallback<OnPythonPluginMessage>(
-    ({ data: { final, elapsedTimes } }) => {
+    ({ data: { final, injections, elapsedTimes } }) => {
       if (!final) {
         toastWord("success", Toast_Words["submit-task-finished-message"], {
           appendix: ` (${pureIdentifier})`,
         });
       } else {
         importMeta({
           lang,
           type: "python.fields",
           metaData: {
             identifier: pureIdentifier,
-            parameters: taskCache?.parameters ?? {},
             response: final,
+            injections: { ...taskCache?.injections, ...injections },
             elapsedTimes,
             from: taskCache?.currentMeta,
           },
         });
       }
     },
     [id, pureIdentifier, lang, taskCache],
@@ -57,19 +58,20 @@
     [lang],
   );
 
   const header = parseIStr(pluginInfo.header ?? titleCaseWord(pureIdentifier));
   return (
     <PythonPluginWithSubmit
       id={id}
+      pluginInfo={pluginInfo}
       buttonText={translate(UI_Words["submit-task"], lang)}
-      getExtraRequestData={getExtraRequestData}
       onFinished={onFinished}
       onSocketError={onSocketError}
-      pluginInfo={pluginInfo}
+      getExtraRequestData={getExtraRequestData}
+      getInjections={getInjections}
       {...props}>
       <Flex>
         <CFHeading>{header}</CFHeading>
         <Spacer />
         <CloseIcon w="12px" cursor="pointer" onClick={emitClose} />
       </Flex>
       <Definitions definitions={definitions} numColumns={pluginInfo.numColumns} />
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/MarkdownPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/MarkdownPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/PluginGroup.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/PluginGroup.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/PluginWithSubmit.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -23,20 +23,19 @@
 import { useCurrentMeta, useOnMessage } from "./hooks";
 
 export const socketFinishedEvent = new Event<{ id: string }>();
 function PythonPluginWithSubmit({
   id,
   pluginInfo,
   buttonText,
-  beforeSubmit,
-  afterSubmit,
   onIntermediate,
   onFinished,
   onSocketError,
   getExtraRequestData,
+  getInjections,
   children,
   ...props
 }: IPythonSocketPluginWithSubmit) {
   const {
     node,
     nodes,
     identifier,
@@ -50,19 +49,18 @@
   const [hash, setHash] = useState<string | undefined>(undefined);
   const [busy, setBusy] = useState(false);
   const taskCache = usePluginTaskCache(id);
   const hasConstraint = checkHasConstraint(props);
   const currentMeta = hasConstraint ? useCurrentMeta(node, nodes) : undefined;
   const onClick = useCallback(() => {
     if (busy) return;
-    beforeSubmit?.();
     setBusy(true);
     setHash(usePluginHash(id));
     if (!taskCache) {
-      setPluginTaskCache(id, { currentMeta, parameters: getExtraRequestData?.() ?? {} });
+      setPluginTaskCache(id, { currentMeta, injections: getInjections?.() ?? {} });
     }
     if (closeOnSubmit) {
       if (isUndefined(props.groupId)) {
         setPluginExpanded(id, false);
       } else {
         setPluginExpanded(props.groupId, true);
       }
@@ -71,24 +69,23 @@
       toast(
         "info",
         parseIStr(
           toastMessageOnSubmit ?? translate(Toast_Words["submit-task-success-message"], lang),
         ),
       );
     }
-    afterSubmit?.();
   }, [
     id,
     lang,
     closeOnSubmit,
     toastOnSubmit,
     toastMessageOnSubmit,
     busy,
     currentMeta,
-    getExtraRequestData,
+    getInjections,
   ]);
   const onMessage = useOnMessage({ id, pluginInfo, onIntermediate, onFinished });
 
   useSocketPython({
     hash,
     node,
     nodes,
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/QAPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/QAPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/TextAreaPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_python/hooks.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_python/hooks.ts`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,69 @@
 import { useCallback, useEffect, useMemo, useState } from "react";
 
 import { Dictionary, INode, getRandomHash, isSingleNode, shallowCopy } from "@carefree0910/core";
 import { langStore } from "@carefree0910/business";
 
 import type { IMeta } from "@/schema/meta";
-import type { IDefinitions } from "@/schema/fields";
+import type { IDefinitions, IFieldDefinition } from "@/schema/fields";
 import type {
   IPythonOnPluginMessage,
   IPythonPlugin,
   IUseOnPythonPluginMessage,
   OnPythonPluginMessage,
 } from "@/schema/_python";
-import { getMetaField } from "@/stores/meta";
+import { IMetaInjections, getMetaField, getMetaInjection } from "@/stores/meta";
 import { setPluginMessage, usePluginIds, usePluginNeedRender } from "@/stores/pluginsInfo";
 import { useSocketPython } from "@/hooks/usePython";
+import { ID_KEY } from "../components/Fields/ListField";
+import { checkHasConstraint } from "../utils/renderFilters";
 import { cleanupException, cleanupFinished, cleanupInterrupted } from "../utils/cleanup";
 import { socketFinishedEvent } from "./PluginWithSubmit";
-import { checkHasConstraint } from "../utils/renderFilters";
 
 export function useDefinitionsRequestDataFn(definitions: IDefinitions): () => Dictionary<any> {
   return useCallback(() => {
     const data: Dictionary<any> = {};
     Object.keys(definitions).forEach((field) => {
-      data[field] = getMetaField({ field });
+      const value = getMetaField({ field });
+      if (Array.isArray(value)) {
+        value.forEach((obj: any) => {
+          if (!!obj[ID_KEY]) {
+            delete obj[ID_KEY];
+          }
+        });
+      }
+      data[field] = value;
     });
     return data;
   }, [definitions]);
 }
+export function useDefinitionsGetInjectionsFn(definitions: IDefinitions): () => IMetaInjections {
+  return useCallback(() => {
+    const _inject = (prefix: string, field: string, definition: IFieldDefinition) => {
+      const key = !!prefix ? `${prefix}.${field}` : field;
+      if (definition.type !== "list") {
+        const injection = getMetaInjection(key);
+        if (!!injection) {
+          injections[key] = injection;
+        }
+      } else {
+        const definitionValues = getMetaField({ field });
+        if (!Array.isArray(definitionValues)) return;
+        definitionValues.forEach((_, i) => {
+          Object.entries(definition.item).forEach(([itemField, itemDefinition]) => {
+            _inject(`${key}.${i}`, itemField, itemDefinition);
+          });
+        });
+      }
+    };
+    const injections: IMetaInjections = {};
+    Object.entries(definitions).forEach(([field, definition]) => _inject("", field, definition));
+    return injections;
+  }, [definitions]);
+}
 export function useCurrentMeta(node: INode | null, nodes: INode[]): IMeta | undefined {
   return useMemo(() => {
     let currentMeta: IMeta | undefined;
     if (node && isSingleNode(node)) {
       currentMeta = node.params.meta as IMeta;
     } else if (nodes.length > 1) {
       // main + mask workaround
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/AddPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/AddPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/ArrangePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/BrushPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/DeletePlugin.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import { usePluginIds } from "@/stores/pluginsInfo";
 import { drawboardPluginFactory } from "../utils/factory";
 import Render from "../components/Render";
 
 const DeletePlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = usePluginIds("delete").id;
   const { type, nodes } = useSelecting("raw");
-  if (type === "none") return null;
+  if (type === "none") {
+    props.renderInfo.isInvisible = true;
+  }
   function onDelete(): void {
     useSafeExecute("remove", null, true)(nodes.map((node) => node.alias));
   }
   return <Render id={id} onFloatingButtonClick={async () => onDelete()} {...props} />;
 };
 
 drawboardPluginFactory.register("delete", true)(observer(DeletePlugin));
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/DownloadPlugin.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -3,47 +3,55 @@
 import { Flex, Spacer } from "@chakra-ui/react";
 
 import { langStore, translate, useSelecting } from "@carefree0910/business";
 
 import type { IPlugin } from "@/schema/plugins";
 import { DownloadFormat, allDownloadFormat } from "@/schema/misc";
 import { Download_Words } from "@/lang/download";
-import { themeStore } from "@/stores/theme";
 import { usePluginIds } from "@/stores/pluginsInfo";
 import { downloadNodes } from "@/actions/download";
 import CFSelect, { CFSrollableSelect } from "@/components/CFSelect";
-import CFText from "@/components/CFText";
+import CFText, { CFCaption } from "@/components/CFText";
 import CFButton from "@/components/CFButton";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import { drawboardPluginFactory } from "../utils/factory";
 import { useClosePanel } from "../components/hooks";
 import Render from "../components/Render";
 
 const DownloadPlugin = ({ pluginInfo, ...props }: IPlugin) => {
   const id = usePluginIds("download").id;
   const lang = langStore.tgt;
   const { type, nodes } = useSelecting("raw");
   const { w, h, imgWH } = useSelecting("basic")({ fixed: 0 }) ?? {};
-  const { captionColor } = themeStore.styles;
   const [format, setFormat] = useState<DownloadFormat>("PNG");
   const [keepOriginal, setKeepOriginal] = useState(true);
+  const tooltip = useMemo(
+    () =>
+      translate(
+        keepOriginal
+          ? Download_Words["download-original-image-tooltip"]
+          : Download_Words["download-drawboard-image-tooltip"],
+        lang,
+      ),
+    [lang, keepOriginal],
+  );
   const sizeString = useMemo(() => {
     if (!type || type === "none") return null;
     if (type === "multiple") return translate(Download_Words["download-multiple-caption"], lang);
     if (!keepOriginal || type !== "image") return `${w} x ${Math.abs(h!)}`;
     if (!imgWH) return "Loading...";
     return `${imgWH.w} x ${imgWH.h}`;
   }, [type, lang, w, h, imgWH, keepOriginal]);
   const getWord = useCallback(
     (keepOriginal: boolean) =>
       translate(
         keepOriginal
-          ? Download_Words["download-image-size-original"]
-          : Download_Words["download-image-size-drawboard"],
+          ? Download_Words["download-original-image"]
+          : Download_Words["download-drawboard-image"],
         lang,
       ),
     [lang],
   );
   const closePanel = useClosePanel(id);
   const onDownload = useCallback(() => {
     downloadNodes(nodes, format, keepOriginal);
@@ -58,16 +66,14 @@
 
   const selectedKeepOriginal = { value: keepOriginal, label: getWord(keepOriginal) };
   const keepOriginalOptions = [true, false].map((keepOriginal) => ({
     value: keepOriginal,
     label: getWord(keepOriginal),
   }));
 
-  if (!nodes) return null;
-
   return (
     <Render id={id} {...props}>
       <Flex w="100%" h="100%" direction="column">
         <Flex align="center">
           <CFHeading>{translate(Download_Words["download-plugin-header"], lang)}</CFHeading>
           <CFText ml="4px" fontSize="sm">
             ({nodes.length})
@@ -82,30 +88,30 @@
           onChange={(e) => {
             if (!!e) {
               setFormat(e.value);
             }
           }}
         />
         <CFSelect<boolean, false>
+          tooltip={tooltip}
+          tooltipProps={{ placement: "top" }}
           height="32px"
           fontSize="14px"
           boxProps={{ mt: "10px" }}
           value={selectedKeepOriginal}
           options={keepOriginalOptions}
           onChange={(e) => {
             if (!!e) {
               setKeepOriginal(e.value);
             }
           }}
         />
         <Flex mt="8px" pr="6px">
           <Spacer />
-          <CFText color={captionColor} fontSize="sm">
-            {sizeString}
-          </CFText>
+          <CFCaption fontSize="sm">{sizeString}</CFCaption>
         </Flex>
         <CFButton mt="12px" onClick={onDownload}>
           {translate(Download_Words["download-button"], lang)}
         </CFButton>
       </Flex>
     </Render>
   );
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/GroupPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/LinksPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/ProjectPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/SettingsPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/ShortcutsPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/ShortcutsPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/TextEditorPlugin.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import { CFSrollableSelect, ICFSelect } from "@/components/CFSelect";
 import CFSlider from "@/components/CFSlider";
 import CFDivider from "@/components/CFDivider";
 import CFHeading from "@/components/CFHeading";
 import CFTextarea from "@/components/CFTextarea";
 import CFColorPicker from "@/components/CFColorPicker";
 import { drawboardPluginFactory } from "../utils/factory";
+import BasicEditor from "./components/BasicEditor";
 import Render from "../components/Render";
 
 const textAlignDict: Record<TextAlign, Record<Lang, string>> = {
   left: { zh: "左对齐", en: "Left" },
   center: { zh: "居中", en: "Center" },
   right: { zh: "右对齐", en: "Right" },
   justify: { zh: "两端对齐", en: "Justify" },
@@ -50,23 +51,29 @@
   };
   const onChangeAlign: ICFSelect<TextAlign, false>["onChange"] = (e) => {
     if (!!e) {
       editAlign({ trace: true })(e.value);
     }
   };
 
-  if (node?.type !== "text" || !textParams) return null;
-
-  const textColor = textParams.color;
-  const textAlign = textParams.align ?? "left";
+  let textColor: string | undefined;
+  let textAlign: TextAlign = "left";
+  if (node?.type !== "text" || !textParams) {
+    props.renderInfo.isInvisible = true;
+  } else {
+    textColor = textParams.color;
+    textAlign = textParams.align ?? "left";
+  }
 
   return (
     <Render id={id} {...props}>
       <CFHeading>{translate(NodeEditor_Words["text-editor-plugin-header"], lang)}</CFHeading>
       <CFDivider />
+      <BasicEditor />
+      <CFDivider />
       <Flex direction="column" w="100%" h="100%">
         <Flex w="100%">
           <CFSlider
             flex={1}
             min={12}
             max={1024}
             precision={0}
@@ -91,18 +98,20 @@
           flexProps={{ h: "42px" }}
           labelProps={{ ml: "12px", mr: "4px", fontSize: "16px" }}
           boxProps={{ flex: 1 }}
           value={{
             value: textAlign,
             label: textAlignDict[textAlign][lang],
           }}
-          options={allTextAlign.map((align) => ({
-            value: align,
-            label: textAlignDict[align][lang],
-          }))}
+          options={allTextAlign
+            .filter((align) => align !== "justify")
+            .map((align) => ({
+              value: align,
+              label: textAlignDict[align][lang],
+            }))}
           onChange={onChangeAlign}
         />
         <CFDivider />
         <CFTextarea
           flex={1}
           value={content}
           onChange={(e) => {
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/_react/UndoRedoPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/BooleanField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/ColorField.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/ColorField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/Field.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/Field.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import TextField from "./TextField";
 import ColorField from "./ColorField";
+import ImageField from "./ImageField";
 import NumberField from "./NumberField";
 import SelectField from "./SelectField";
 import BooleanField from "./BooleanField";
 import { IFieldComponent, injectDefaultFieldProps } from "./utils";
 
 export function Field({ gap, definition, ...fieldKeys }: IFieldComponent) {
   let Field: any;
@@ -13,12 +14,14 @@
     Field = NumberField;
   } else if (definition.type === "select") {
     Field = SelectField;
   } else if (definition.type === "boolean") {
     Field = BooleanField;
   } else if (definition.type === "color") {
     Field = ColorField;
+  } else if (definition.type === "image") {
+    Field = ImageField;
   }
   if (!Field) return null;
   injectDefaultFieldProps({ gap, definition, ...fieldKeys });
   return <Field definition={definition} {...fieldKeys} />;
 }
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/ListField/index.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/ListField/index.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import { Fragment, useState } from "react";
 import { observer } from "mobx-react-lite";
+import { runInAction } from "mobx";
+import { Fragment, useState } from "react";
 import { Box, Center, Flex, Image, Spacer } from "@chakra-ui/react";
 
 import { Dictionary, getRandomHash } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
 import "./index.scss";
 import AddIcon from "@/assets/icons/add.svg";
@@ -12,43 +13,45 @@
 
 import type { IField, IListProperties } from "@/schema/plugins";
 import type { IDefinitions, IListField } from "@/schema/fields";
 import { genBlock } from "@/utils/bem";
 import { titleCaseWord } from "@/utils/misc";
 import { EXPAND_TRANSITION } from "@/utils/constants";
 import { UI_Words } from "@/lang/ui";
-import { themeStore, useScrollBarSx } from "@/stores/theme";
-import { getMetaField, setMetaField } from "@/stores/meta";
+import { useScrollBarSx } from "@/stores/theme";
+import { getMetaField, setMetaField, setMetaInjection } from "@/stores/meta";
 import { parseIStr } from "@/actions/i18n";
 import CFIcon from "@/components/CFIcon";
-import CFText from "@/components/CFText";
+import CFText, { CFCaption } from "@/components/CFText";
 import CFDivider from "@/components/CFDivider";
 import CFTooltip from "@/components/CFTooltip";
 import { getFieldH, useDefaultFieldValue } from "../utils";
 import { Field } from "../Field";
 
-const ID_KEY = "^_^__id__^_^";
+export const ID_KEY = "^_^__id__^_^";
 function getDefaults(item: IDefinitions): Dictionary<any> {
   const defaults: Dictionary<any> = { [ID_KEY]: getRandomHash() };
   for (const [key, value] of Object.entries(item)) {
     defaults[key] = value.default;
   }
   return defaults;
 }
 
 const block = genBlock("c-list-field");
 function ListField({ definition, gap, ...fieldKeys }: IField<IListField> & { gap: number }) {
+  if (!!fieldKeys.listProperties) {
+    throw Error("should not use `ListField` inside another `ListField`");
+  }
   useDefaultFieldValue({ definition, ...fieldKeys });
   const field = fieldKeys.field;
   const label = parseIStr(definition.label ?? titleCaseWord(field));
   const tooltip = parseIStr(definition.tooltip ?? "");
   const [expanded, setExpanded] = useState(false);
 
   const lang = langStore.tgt;
-  const { captionColor } = themeStore.styles;
   const values: any[] | undefined = getMetaField(fieldKeys);
 
   if (!values) return null;
 
   const itemRows = Object.keys(definition.item).length + 1;
   definition.numRows = Math.max(1, Math.min(values.length * itemRows, definition.maxNumRows ?? 4));
   const expandH = getFieldH({ gap, definition, field });
@@ -59,14 +62,22 @@
   const onAdd = () => {
     setMetaField(fieldKeys, [...values, getDefaults(definition.item)]);
   };
   const onDelete = (index: number) => {
     const newValues = [...values];
     newValues.splice(index, 1);
     setMetaField(fieldKeys, newValues);
+    runInAction(() => {
+      Object.keys(definition.item).forEach((key) => {
+        setMetaInjection(
+          { field: key, listProperties: { listKey: field, listIndex: index } },
+          undefined,
+        );
+      });
+    });
   };
 
   return (
     <Flex
       w="100%"
       h={`${expanded ? totalH : fieldH}px`}
       direction="column"
@@ -78,15 +89,17 @@
             <CFIcon
               svg={ArrowDownIcon}
               squared={false}
               className={block({ e: "icon", m: expanded ? "expanded" : "folded" })}
               fillbyCurrentColor
               transition={EXPAND_TRANSITION}
             />
-            <CFText ml="6px">{label}</CFText>
+            <CFText ml="6px" fontWeight={500}>
+              {label}
+            </CFText>
             <Spacer />
           </Flex>
         </CFTooltip>
         <CFTooltip label={translate(UI_Words["add-object-to-list-tooltip"], lang)}>
           <Image w="34px" h="34px" p="6px" src={AddIcon} cursor="pointer" onClick={onAdd} />
         </CFTooltip>
       </Flex>
@@ -95,32 +108,36 @@
         h={`${expanded ? expandH : 0}px`}
         mt={`${expanded ? 6 : 0}px`}
         overflow="hidden"
         direction="column"
         transition={EXPAND_TRANSITION}>
         {values.length === 0 ? (
           <Center>
-            <CFText color={captionColor}>
-              {translate(UI_Words["list-field-empty-caption"], lang)}
-            </CFText>
+            <CFCaption>{translate(UI_Words["list-field-empty-caption"], lang)}</CFCaption>
           </Center>
         ) : (
           <Flex
             flex={1}
             direction="column"
             overflowX="hidden"
             overflowY="auto"
             sx={useScrollBarSx()}>
             {values.map((pack, index) => {
               const keyId = `${field}-${pack[ID_KEY]}`;
               const isLast = index === values.length - 1;
               const listProperties: IListProperties = { listKey: field, listIndex: index };
               return (
                 <Fragment key={`${keyId}-${index}`}>
-                  <Flex mr="12px" flexShrink={0} direction="column">
+                  <Flex
+                    ml="8px"
+                    mr="12px"
+                    my="8px"
+                    flexShrink={0}
+                    direction="column"
+                    gap={`${gap}px`}>
                     {Object.entries(definition.item).map(([key, item]) => (
                       <Field
                         key={`${keyId}-${key}-${index}`}
                         gap={gap}
                         definition={item}
                         field={key}
                         listProperties={listProperties}
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 import { parseIStr } from "@/actions/i18n";
 import { CFSrollableSelect } from "@/components/CFSelect";
 import { useDefaultFieldValue } from "./utils";
 
 function SelectField({ definition, ...fieldKeys }: IField<ISelectField>) {
   useDefaultFieldValue({ definition, ...fieldKeys });
   const userId = userStore.userId;
+  const userJson = userStore.json;
   const label = parseIStr(definition.label ?? titleCaseWord(fieldKeys.field));
   const tooltip = parseIStr(definition.tooltip ?? "");
   const [value, setValue] = useState(getMetaField(fieldKeys) ?? definition.default);
-  const [options, setOptions] = useState(definition.values as IStr[]);
+  const [options, setOptions] = useState(definition.options as IStr[]);
   const onMenuOpen = useCallback(() => {
     if (definition.localProperties) {
       const extraData = definition.localProperties;
       const hash = getHash(JSON.stringify(extraData)).toString();
       runOneTimeSocketHook<{ options: string[] }>({
         key: "selectField",
         hook: {
           key: hash,
           getMessage: async () => ({
             hash,
             userId,
+            userJson,
             baseURL: getBaseURL(),
             identifier: "sync_local_select",
             nodeData: {},
             nodeDataList: [],
             extraData,
             isInternal: true,
           }),
@@ -44,31 +46,35 @@
         if (res) {
           setOptions(res.options);
         }
       });
     }
   }, [definition.localProperties]);
 
-  const selected = { value, label: parseIStr(value) };
-  const selectOptions = options.map((value) => ({ value, label: parseIStr(value) }));
+  const selected = { value: JSON.stringify(value), label: parseIStr(value) };
+  const selectOptions = options.map((value) => ({
+    value: JSON.stringify(value),
+    label: parseIStr(value),
+  }));
 
   return (
-    <CFSrollableSelect<IStr, false>
+    <CFSrollableSelect<string, false>
       fontSize="14px"
       label={label}
       tooltip={tooltip}
       flexProps={definition.props}
       boxProps={{ flex: 1 }}
       value={selected}
       options={selectOptions}
       onMenuOpen={onMenuOpen}
       onChange={(e) => {
         if (!!e) {
-          setValue(e.value);
-          setMetaField(fieldKeys, e.value);
+          const value = JSON.parse(e.value);
+          setValue(value);
+          setMetaField(fieldKeys, value);
         }
       }}
     />
   );
 }
 
 export default observer(SelectField);
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/TextField.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/TextField.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import CFInput from "@/components/CFInput";
 import CFTextarea from "@/components/CFTextarea";
 import { useDefaultFieldValue } from "./utils";
 
 function TextField({ definition, ...fieldKeys }: IField<ITextField>) {
   useDefaultFieldValue({ definition, ...fieldKeys });
   const label = parseIStr(definition.label ?? titleCaseWord(fieldKeys.field));
-  const tooltip = parseIStr(definition.tooltip ?? "");
+  const tooltip = parseIStr(definition.tooltip ?? label);
   const defaultText = parseIStr(definition.default ?? "");
   const [value, setValue] = useState(getMetaField(fieldKeys) ?? defaultText);
   const isNumber = useMemo(() => !!definition.numberOptions, [definition.numberOptions]);
   const Input = definition.numRows && definition.numRows > 1 ? CFTextarea : CFInput;
 
   const onChange = useCallback(
     (event: ChangeEvent<HTMLInputElement | HTMLTextAreaElement>) => {
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/index.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Fields/utils.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Fields/utils.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Floating.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Floating.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 import { isUndefined } from "@carefree0910/core";
 import { langStore, translate } from "@carefree0910/business";
 
 import type { IFloating } from "@/schema/plugins";
 import {
   BG_TRANSITION,
   DEFAULT_PLUGIN_SETTINGS,
-  makeVisibilityTransitionProps,
+  useVisibilityTransitionProps,
 } from "@/utils/constants";
 import { UI_Words } from "@/lang/ui";
 import { themeStore, useScrollBarSx } from "@/stores/theme";
 import {
   usePluginMessage,
   usePluginIsExpanded,
   setPluginExpanded,
   usePluginGroupIsExpanded,
+  usePluginChildren,
 } from "@/stores/pluginsInfo";
 import { isInteractingWithBoard } from "@/hooks/useDocumentEvents";
 import { parseIStr } from "@/actions/i18n";
 import CFText from "@/components/CFText";
 import { CFIconButton } from "@/components/CFButton";
 import { CFPendingProgress, CFWorkingProgress } from "@/components/CFCircularProgress";
 
@@ -50,16 +51,15 @@
       iconH,
       pivot,
       follow,
       src,
       tooltip,
       offsetY,
       bgOpacity,
-      useModal,
-      modalOpacity,
+      expandOpacity,
       expandProps,
       isInvisible,
     },
     noExpand,
     onFloatingButtonClick,
     children,
     ...props
@@ -167,17 +167,19 @@
   const parsedExpandProps: FlexProps = {};
   Object.entries(expandProps ?? {}).forEach(([key, value]) => {
     if (!isUndefined(value) && value !== null) {
       parsedExpandProps[key as keyof FlexProps] = value;
     }
   });
   // convert float to hex
-  modalOpacity ??= DEFAULT_PLUGIN_SETTINGS.expandOpacity;
-  const modalOpacityHex = Math.round(modalOpacity * 255).toString(16);
-  const expandBg = `${panelBg}${modalOpacityHex}`;
+  expandOpacity ??= DEFAULT_PLUGIN_SETTINGS.expandOpacity;
+  const expandOpacityHex = Math.round(expandOpacity * 255).toString(16);
+  const expandBg = `${panelBg}${expandOpacityHex}`;
+  // set expand render condition
+  const renderExpand = expand || usePluginChildren(id).length > 0;
 
   return (
     <>
       <CFIconButton
         src={parseIStr(src)}
         tooltip={iconActivated ? parseIStr(tooltip ?? "") : ""}
         id={id}
@@ -185,15 +187,15 @@
         h={`${iconH}px`}
         onClick={() => {
           if (!noExpand) {
             setPluginExpanded(id, !expand);
           }
           onFloatingButtonClick?.();
         }}
-        {...makeVisibilityTransitionProps({
+        {...useVisibilityTransitionProps({
           visible: !isInvisible,
           extraTransitions: BG_TRANSITION,
         })}
         _focus={{ outline: "none" }}
         {...getCommonProps(false)}
         {...props}
         imageProps={{ opacity: iconOpacity }}>
@@ -227,20 +229,20 @@
         <Portal containerRef={ref as any}>
           <Flex
             id={expandId}
             w={`${w}px`}
             h={`${h}px`}
             overflowX="hidden"
             direction="column"
-            {...makeVisibilityTransitionProps({ visible: expand })}
+            {...useVisibilityTransitionProps({ visible: expand })}
             {...getCommonProps(true)}
             bg={expandBg}
             sx={useScrollBarSx()}
             {...parsedExpandProps}>
-            {children}
+            {renderExpand && children}
           </Flex>
         </Portal>
       )}
     </>
   );
 });
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/components/Render.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/components/Render.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -17,24 +17,26 @@
   useBoardContainerLeftTop,
   useBoardContainerWH,
   useIsReady,
   useSelectHooks,
   useSelecting,
 } from "@carefree0910/business";
 
-import type { IExpandPositionInfo, IRender } from "@/schema/plugins";
+import type { IExpandPositionInfo, IRender, IRenderInfo } from "@/schema/plugins";
 import { DEFAULT_PLUGIN_SETTINGS } from "@/utils/constants";
 import {
   addPluginChild,
   usePluginGroupIsExpanded,
   usePluginIsExpanded,
   setPluginNeedRender,
   usePluginNeedRender,
   setPluginUpdater,
   usePluginUpdater,
+  setPluginIsFollow,
+  usePluginIsFollow,
 } from "@/stores/pluginsInfo";
 import { checkHasConstraint, hashInfo, useNodeFilter } from "../utils/renderFilters";
 import Floating, { getExpandId } from "./Floating";
 
 let DEBUG_PREFIX: string | undefined;
 
 function getExpandPosition(
@@ -51,14 +53,15 @@
     follow,
     expandOffsetX,
     expandOffsetY,
   }: { x: number; y: number; groupId?: string } & IExpandPositionInfo,
 ): Coordinate {
   // check group
   if (!isUndefined(groupId)) {
+    follow = usePluginIsFollow(groupId);
     const group = document.getElementById(groupId);
     if (group) {
       const rect = group.getBoundingClientRect();
       x = rect.left;
       y = rect.top;
       iconW = rect.width;
       iconH = rect.height;
@@ -165,14 +168,15 @@
   let { w, h, iconW, iconH, pivot, follow, offsetX, offsetY, expandOffsetX, expandOffsetY } =
     renderInfo;
   iconW ??= DEFAULT_PLUGIN_SETTINGS.iconW;
   iconH ??= DEFAULT_PLUGIN_SETTINGS.iconH;
   pivot ??= DEFAULT_PLUGIN_SETTINGS.pivot as PivotType;
   follow ??= DEFAULT_PLUGIN_SETTINGS.follow;
   follow = follow || inGroup;
+  setPluginIsFollow(_id, follow);
   expandOffsetX ??=
     renderInfo.useModal || ["top", "center", "bottom"].includes(pivot)
       ? 0
       : ["lt", "left", "lb"].includes(pivot) === follow
       ? -DEFAULT_PLUGIN_SETTINGS.expandOffsetX
       : DEFAULT_PLUGIN_SETTINGS.expandOffsetX;
   expandOffsetY ??=
@@ -180,43 +184,42 @@
       ? 0
       : pivot === "center"
       ? DEFAULT_PLUGIN_SETTINGS.expandOffsetY
       : (pivot === "top") === follow
       ? -DEFAULT_PLUGIN_SETTINGS.expandOffsetY
       : DEFAULT_PLUGIN_SETTINGS.expandOffsetY;
 
-  const updatedRenderInfo = {
+  const updatedRenderInfo: IRenderInfo = {
     ...renderInfo,
     w,
     h,
     iconW,
     iconH,
     pivot,
     follow,
     expandOffsetX,
     expandOffsetY,
+    isInvisible: !needRender ? true : renderInfo.isInvisible,
   };
 
-  const deps = [
+  const updateFloatingDeps = [
     _id,
-    needRender,
     ...infoDeps,
     groupId,
     iconW,
     iconH,
     pivot,
     follow,
     offsetX,
     offsetY,
     expandOffsetX,
     expandOffsetY,
     JSON.stringify(props),
   ];
   const updateFloating = useCallback(async (e: any) => {
-    if (!needRender) return;
     const _iconW = iconW!;
     const _iconH = iconH!;
     const _pivot = pivot!;
     const _follow = follow!;
     const _offsetX =
       offsetX ??
       (["top", "center", "bottom"].includes(_pivot)
@@ -309,15 +312,15 @@
       iconH: _iconH,
       pivot: _pivot,
       follow: _follow,
       expandOffsetX: expandOffsetX!,
       expandOffsetY: expandOffsetY!,
     });
     domFloatingExpand.style.transform = `matrix(1,0,0,1,${ex},${ey})`;
-  }, deps);
+  }, updateFloatingDeps);
 
   const updater = usePluginUpdater(_id);
   useEffect(() => {
     if (!isUndefined(groupId)) {
       addPluginChild(groupId, _id);
     }
   }, [_id, groupId]);
@@ -351,16 +354,14 @@
       if (hasConstraint) {
         useSelectHooks().remove(_id);
       }
       window.removeEventListener("resize", updater);
     };
   }, [updater, _id, inGroup, isReady, needRender, follow, hasConstraint]);
 
-  if (!needRender) return null;
-
   return (
     <Floating
       id={_id}
       groupId={groupId}
       ref={containerRef}
       renderInfo={updatedRenderInfo}
       {...props}>
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/index.tsx` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/index.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 export * from "./_react/SettingsPlugin";
 export * from "./_react/ProjectPlugin";
 export * from "./_react/AddPlugin";
 export * from "./_react/ArrangePlugin";
 export * from "./_react/UndoRedoPlugin";
 export * from "./_react/DownloadPlugin";
 export * from "./_react/DeletePlugin";
+export * from "./_react/BasicEditorPlugin";
 export * from "./_react/TextEditorPlugin";
 export * from "./_react/GroupPlugin";
 export * from "./_react/LinksPlugin";
 export * from "./_react/ShortcutsPlugin";
 export * from "./_react/BrushPlugin";
 export * from "./_python/PluginGroup";
 export * from "./_python/FieldsPlugin";
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/cleanup.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/utils/cleanup.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/factory.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/utils/factory.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/plugins/utils/renderFilters.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/plugins/utils/renderFilters.ts`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,27 @@
   if (!constraint || constraint === "none") return true;
   if (!info) return false;
   if (constraint === "anyNode") return info.type !== "none";
   if (constraint === "multiNode") return info.type === "multiple";
   if (constraint === "singleNode") return !["group", "multiple", "none"].includes(info.type);
   return info.type === constraint;
 }
-async function checkRules(
+function checkRules(
   rules: NodeConstraintSettings["nodeConstraintRules"],
   info?: IResponse,
-): Promise<boolean> {
+): boolean {
   if (rules?.some) {
     for (const nodeConstraint of rules.some) {
-      if (await useNodeFilter({ nodeConstraint })(info)) return true;
+      if (checkConstraint(nodeConstraint, info)) return true;
     }
     return false;
   }
   if (rules?.every) {
     for (const nodeConstraint of rules.every) {
-      if (!(await useNodeFilter({ nodeConstraint })(info))) return false;
+      if (!checkConstraint(nodeConstraint, info)) return false;
     }
     return true;
   }
   if (rules?.exactly) {
     if (!info) return false;
     if (info.nodes.length !== rules.exactly.length) return false;
     const selectedNodes = info.nodes.map((node) => node.type);
@@ -60,15 +60,15 @@
   if (!info) return "";
   const node = info.displayNode?.alias ?? "";
   const nodes = info.nodes.map((node) => node.alias).join(",");
   return getHash(`${node}-${nodes}`).toString();
 }
 function checkValidator(validator?: string, info?: IResponse): Promise<boolean> {
   if (isUndefined(validator)) return Promise.resolve(true);
-  const hash = hashInfo(info);
+  const hash = `${validator}-${hashInfo(info)}`;
   const getMessage = (): Promise<IPythonSocketRequest> => {
     return getPythonRequest({
       node: info?.displayNode ?? null,
       nodes: info?.nodes ?? [],
       identifier: "node_validator",
       opt: { noExport: true },
       needExportNodeData: true,
@@ -94,15 +94,15 @@
   return [settings.nodeConstraint, settings.nodeConstraintRules, settings.nodeConstraintValidator];
 }
 export function useNodeFilter(
   settings: NodeConstraintSettings,
 ): (info?: IResponse) => Promise<boolean> {
   return useCallback(async (info) => {
     if (!checkConstraint(settings.nodeConstraint, info)) return false;
-    if (!(await checkRules(settings.nodeConstraintRules, info))) return false;
+    if (!checkRules(settings.nodeConstraintRules, info)) return false;
     if (!(await checkValidator(settings.nodeConstraintValidator, info))) return false;
     return true;
   }, useConstraintDeps(settings));
 }
 
 export function checkHasConstraint({
   nodeConstraint,
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/react-app-env.d.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/react-app-env.d.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/actions.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/requests/actions.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/hooks.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/requests/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/interceptors/_python.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/requests/interceptors/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/requests/interceptors/index.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/requests/interceptors/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/_python.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/_python.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import type { TextareaProps } from "@chakra-ui/react";
 
 import type { Dictionary, INode, Matrix2DFields } from "@carefree0910/core";
 
+import type { IMetaInjections } from "@/stores/meta";
 import type { IElapsedTimes, IMeta, IPythonResults } from "./meta";
 import type { PythonPlugins, IMakePlugin, IPlugin, IPluginInfo } from "./plugins";
 import type { IDefinitions } from "./fields";
 import type { IStr } from "./misc";
 
 // general
 
@@ -61,16 +62,15 @@
 export type OnPythonPluginMessage = (message: IPythonPluginMessage) => void;
 export interface IPythonSocketPluginWithSubmit
   extends Omit<IPythonPlugin, "id" | "pluginInfo">,
     Omit<IPythonSocketCallbacks<IPythonResults>, "getMessage" | "onMessage">,
     IUseOnPythonPluginMessage {
   id: string;
   buttonText: string;
-  beforeSubmit?: () => void;
-  afterSubmit?: () => void;
+  getInjections?: () => IMetaInjections;
 }
 
 interface IPythonPluginWithSubmitPluginInfo {
   closeOnSubmit?: boolean;
   toastOnSubmit?: boolean;
   toastMessageOnSubmit?: IStr;
 }
@@ -100,14 +100,15 @@
 }
 
 // web
 
 export interface IPythonSocketRequest {
   hash: string;
   userId: string;
+  userJson?: string;
   baseURL: string;
   identifier: string;
   nodeData: INodeData;
   nodeDataList: INodeData[];
   extraData: Dictionary<any>;
   isInternal?: boolean;
 }
@@ -143,14 +144,15 @@
   imageList?: string[]; // intermediate images, if any
   textList?: string[]; // intermediate texts, if any
 }
 export interface IPythonSocketResponse<R> {
   progress?: number; // progress of current task, should be within [0, 1]
   intermediate?: IPythonSocketIntermediate;
   final?: R;
+  injections?: IMetaInjections;
   elapsedTimes?: IElapsedTimes;
 }
 export interface IPythonSocketMessage<R> {
   hash: string;
   status: PythonSocketStatus;
   total: number;
   pending: number;
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/fields.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/fields.ts`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   regex?: string;
   noExt: boolean;
   onlyFiles: boolean;
   defaultPlaceholder?: string;
 }
 export interface ISelectField extends IBaseFields {
   type: "select";
-  values: readonly IStr[];
+  options: readonly IStr[];
   default: IStr;
   isMulti?: boolean;
   localProperties?: ISelectLocalProperties;
 }
 export interface IBooleanField extends IBaseFields {
   type: "boolean";
   default: boolean;
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/meta.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/meta.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import type { Dictionary, Lang } from "@carefree0910/core";
 
+import type { IMetaInjections } from "@/stores/meta";
+
 export interface IElapsedTimes {
   createTime?: number;
   startTime?: number;
   endTime?: number;
   pending?: number;
   executing?: number;
   upload?: number;
@@ -44,16 +46,16 @@
 }
 export type IPythonResults = (
   | { type: "text"; value: { text: string; safe: boolean; reason: string }[] }
   | { type: "image"; value: { w: number; h: number; url: string; safe: boolean; reason: string }[] }
 ) & { extra?: Dictionary<any> };
 export type IPythonFieldsMetaData = ICommonMetaData & {
   identifier: string;
-  parameters: Dictionary<any>;
-  response: IPythonResults;
+  response: IPythonResults & { index?: number };
+  injections?: IMetaInjections;
 };
 
 export interface IMetaData {
   upload: IUploadMetaData;
   "add.text": ICommonMetaData;
   "add.blank": ICommonMetaData;
   "add.sketch.path": ICommonMetaData;
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/plugins.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/plugins.ts`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
   src: IStr;
   tooltip?: IStr;
   offsetX?: number;
   offsetY?: number;
   bgOpacity?: number;
   useModal?: boolean;
   keepOpen?: boolean;
-  modalOpacity?: number;
+  expandOpacity?: number;
   expandProps?: FlexProps;
   isInvisible?: boolean;
 }
 export interface IFloating extends ButtonProps {
   id: string;
   groupId?: string; // the id of the group this floating belongs to
   renderInfo: IRenderInfo;
@@ -97,14 +97,15 @@
   "download",
   "delete",
   "wiki",
   "email",
   "github",
   "shortcuts",
   "logo",
+  "basicEditor",
   "textEditor",
   "groupEditor",
   "multiEditor",
   "brush",
 ] as const;
 export const allPythonPlugins = [
   "_python.pluginGroup",
@@ -130,14 +131,15 @@
   download: IPlugin;
   delete: IPlugin;
   wiki: IPlugin;
   email: IPlugin;
   github: IPlugin;
   shortcuts: IPlugin;
   logo: ILogoPlugin;
+  basicEditor: IPlugin;
   textEditor: IPlugin;
   groupEditor: IPlugin;
   multiEditor: IPlugin;
   brush: IPlugin;
   // python plugins
   "_python.pluginGroup": IPythonPluginGroup;
   "_python.fields": IPythonFieldsPlugin;
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/schema/requests.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/schema/requests.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/debug.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/debug.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/gridLines.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/gridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/hooks.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/meta.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/meta.ts`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import { makeObservable, observable, runInAction } from "mobx";
 
-import { Logger } from "@carefree0910/core";
+import { ISingleNode, Logger, Matrix2DFields } from "@carefree0910/core";
 import { ABCStore } from "@carefree0910/business";
 
 import type { ICommonMetaData, IMeta } from "@/schema/meta";
 import type { IListProperties } from "@/schema/plugins";
 
 class MetaStore extends ABCStore<IMeta["data"]> {
   data: IMeta["data"] = {};
@@ -32,15 +32,15 @@
 export function getMetaField<T extends IGeneralKey>(fieldKeys: IGetMetaField<T>): any;
 export function getMetaField<T extends IMetaKey | IGeneralKey>({
   field,
   listProperties,
 }: IGetMetaField<T>): any {
   if (!listProperties) return metaStore.data[field];
   const list = metaStore.data[listProperties.listKey] as any[];
-  if (list.length <= listProperties.listIndex) return undefined;
+  if (list.length <= listProperties.listIndex) return;
   return list[listProperties.listIndex][field];
 }
 interface ISetMetaField<T extends IMetaKey | IGeneralKey> {
   field: T;
   listProperties?: IListProperties;
 }
 export function setMetaField<T extends IMetaKey>(
@@ -59,7 +59,54 @@
     if (list.length <= listProperties.listIndex) {
       Logger.warn(`list index ${listProperties.listIndex} out of range`);
     } else {
       runInAction(() => (list[listProperties.listIndex][field] = value));
     }
   }
 }
+
+export interface IMetaInjection {
+  meta: IMeta;
+  bboxFields?: Matrix2DFields;
+}
+export type IMetaInjections = Partial<Record<IMetaKey | IGeneralKey, IMetaInjection>>;
+class MetaInjectionsStore extends ABCStore<IMetaInjections> {
+  injections: IMetaInjections = {};
+
+  constructor() {
+    super();
+    makeObservable(this, {
+      injections: observable,
+    });
+  }
+
+  get info(): IMetaInjections {
+    return this.injections;
+  }
+}
+
+export const metaInjectionsStore = new MetaInjectionsStore();
+export function getListInjectionKey({ field, listProperties }: ISetMetaField<string>) {
+  if (!listProperties) return field;
+  return `${listProperties.listKey}.${listProperties.listIndex}.${field}`;
+}
+export function makeMetaInjectionFrom(node: ISingleNode): IMetaInjection | undefined {
+  return { meta: node.meta as IMeta, bboxFields: node.bboxFields };
+}
+export function getMetaInjection(key: string): IMetaInjection | undefined {
+  return metaInjectionsStore.injections[key];
+}
+// injection: undefined means remove the corresponding injection
+export function setMetaInjection<T extends IMetaKey>(
+  fieldKeys: ISetMetaField<T>,
+  injection: IMetaInjection | undefined,
+): void;
+export function setMetaInjection<T extends IGeneralKey>(
+  fieldKeys: ISetMetaField<T>,
+  injection: IMetaInjection | undefined,
+): void;
+export function setMetaInjection<T extends IMetaKey | IGeneralKey>(
+  fieldKeys: ISetMetaField<T>,
+  injection: IMetaInjection | undefined,
+): void {
+  metaInjectionsStore.updateProperty(getListInjectionKey(fieldKeys), injection);
+}
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/pluginsInfo.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/pluginsInfo.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import { useCallback, useEffect } from "react";
 import { action, makeObservable, observable, runInAction } from "mobx";
 
 import { Dictionary, getRandomHash, isUndefined } from "@carefree0910/core";
 import { ABCStore, useIsReady } from "@carefree0910/business";
 
 import type { IMeta } from "@/schema/meta";
-import { allReactPlugins, type ReactPlugins } from "@/schema/plugins";
+import type { ReactPlugins } from "@/schema/plugins";
 import type { IPythonPluginMessage } from "@/schema/_python";
+import type { IMetaInjections } from "./meta";
+import { allReactPlugins } from "@/schema/plugins";
 import { stripHashFromIdentifier } from "@/utils/misc";
 
 interface IDs {
   id: string;
   pureIdentifier: string;
 }
 interface ITaskCache {
   currentMeta?: IMeta;
-  parameters: Dictionary<any>;
+  injections?: IMetaInjections;
 }
 export interface IPluginsInfoStore {
   ids: Dictionary<IDs>;
   hashes: Dictionary<string>;
   messages: Dictionary<IPythonPluginMessage>;
   taskCaches: Dictionary<ITaskCache>;
   visible: Dictionary<boolean>;
   pythonVisible: Dictionary<boolean>;
   expanded: Dictionary<boolean>;
   needRender: Dictionary<boolean>;
   hierarchy: Dictionary<string[]>;
   updaters: Dictionary<(e: any) => Promise<void>>;
+  follows: Dictionary<boolean>;
 }
 type IPluginCollection = keyof IPluginsInfoStore;
 type IPluginCollectionValue<T extends IPluginCollection> = IPluginsInfoStore[T][string];
 interface ISetPluginDefault<T extends IPluginCollection> {
   key: string;
   hasEffect: boolean;
   getDefault: () => IPluginCollectionValue<T>;
@@ -43,28 +46,30 @@
   taskCaches: Dictionary<ITaskCache> = {};
   visible: Dictionary<boolean> = {};
   pythonVisible: Dictionary<boolean> = {};
   expanded: Dictionary<boolean> = {};
   needRender: Dictionary<boolean> = {};
   hierarchy: Dictionary<string[]> = {};
   updaters: Dictionary<(e: any) => Promise<void>> = {};
+  follows: Dictionary<boolean> = {};
 
   constructor() {
     super();
     makeObservable(this, {
       ids: observable,
       hashes: observable,
       messages: observable,
       taskCaches: observable,
       visible: observable,
       pythonVisible: observable,
       expanded: observable,
       needRender: observable,
       hierarchy: observable,
       updaters: observable,
+      follows: observable,
       set: action,
       setDefault: action,
       remove: action,
     });
   }
 
   get info(): IPluginsInfoStore {
@@ -209,7 +214,11 @@
     },
     [updater, children.sort().join(",")],
   );
 };
 export const setPluginUpdater = (id: string, updater: (e: any) => Promise<void>) => {
   pluginsInfoStore.set("updaters", id, updater);
 };
+// follows
+export const usePluginIsFollow = (id: string) => pluginsInfoStore.follows[id];
+export const setPluginIsFollow = (id: string, follow: boolean) =>
+  pluginsInfoStore.set("follows", id, follow);
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/projects.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/settings.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/settings.ts`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import { makeObservable, observable } from "mobx";
 
 import { IBoardOptions, Lang } from "@carefree0910/core";
 import { ABCStore } from "@carefree0910/business";
 
 import type { ReactPlugins, PythonPlugins, IMakePlugin } from "@/schema/plugins";
+import type { IPythonPluginGroup } from "@/schema/_python";
 import type { IProject } from "@/actions/manageProjects";
 import { ThemeType, ThemeStyles } from "./theme";
 
 interface IInternalSettings {
   timeout?: number;
   useStrictMode?: boolean;
   socketEndpoint?: string;
@@ -54,8 +55,16 @@
   get info(): ISettingsStore {
     return this;
   }
 }
 
 export const settingsStore = new SettingsStore();
 export const usePythonPluginSettings = () => settingsStore.pluginSettings;
+export const useFlattenedPythonPluginSettings = () => {
+  const flatten = (p: IMakePlugin<PythonPlugins>): IMakePlugin<PythonPlugins>[] => {
+    if (p.type !== "_python.pluginGroup") return [p];
+    const pluginInfo = p.props.pluginInfo as IPythonPluginGroup["pluginInfo"];
+    return pluginInfo.plugins.flatMap((p) => flatten(p));
+  };
+  return settingsStore.pluginSettings.flatMap(flatten);
+};
 export const useSettingsSynced = () => !!settingsStore.boardSettings;
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/socket.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/socket.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/theme.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/theme.ts`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
   panelBg: string;
   // color of the text
   textColor: string;
   // color of the caption
   captionColor: string;
   // color of the divider
   dividerColor: string;
+  // color of alert captions
+  alertCaptionColor: string;
   // colors of the `CFInput` component
   inputColors: {
     activeBorderColor: string;
   };
   // colors of the `CFSelect` component
   selectColors: {
     activeBorderColor: string;
@@ -59,14 +61,15 @@
 export const allThemes: Record<ThemeType, ThemeStyles> = {
   light: {
     boardBg: "#f7f7f7",
     panelBg: "#f9f9f9",
     textColor: "#333333",
     captionColor: "#888888",
     dividerColor: "#cccccc",
+    alertCaptionColor: "#e63333",
     inputColors: {
       activeBorderColor: "#3fc9a8",
     },
     selectColors: {
       activeBorderColor: "#3fc9a8",
     },
     sliderColors: {
@@ -100,14 +103,15 @@
   // currently dark mode is just a placeholder
   dark: {
     boardBg: "#242424",
     panelBg: "#f9f9f9",
     textColor: "#333333",
     captionColor: "#888888",
     dividerColor: "#cccccc",
+    alertCaptionColor: "#e63333",
     inputColors: {
       activeBorderColor: "#3fc9a8",
     },
     selectColors: {
       activeBorderColor: "#3fc9a8",
     },
     sliderColors: {
@@ -196,13 +200,24 @@
 
   return {
     color: textColor,
     borderWidth: "1px",
     borderRadius: "0px",
     flexShrink: 0,
     _placeholder: { color: captionColor },
-    _focusVisible: {
-      borderColor: activeBorderColor,
-      boxShadow: `0 0 0 1px ${activeBorderColor}`,
-    },
+    _focusVisible: useActiveBorderProps(activeBorderColor),
+  };
+}
+export function useLabelProps(fontSize?: ChakraProps["fontSize"]): ChakraProps {
+  return {
+    minW: "20%",
+    fontSize: fontSize ?? "14px",
+    textAlign: "center",
+    flexShrink: 0,
+  };
+}
+export function useActiveBorderProps(activeBorderColor: string): ChakraProps {
+  return {
+    borderColor: activeBorderColor,
+    boxShadow: `0 0 0 1px ${activeBorderColor}`,
   };
 }
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/stores/ui.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/stores/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/constants.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/utils/constants.ts`

 * *Files 7% similar despite different names*

```diff
@@ -3,45 +3,45 @@
 import ImagePlaceholder from "@/assets/image-placeholder.svg";
 import NSFWImagePlaceholder from "@/assets/nsfw-placeholder.svg";
 
 export const IS_PROD = import.meta.env.PROD;
 
 export const BOARD_CONTAINER_ID = "board.container";
 
-function makeCubicBezier(second: number) {
+function useCubicBezier(second: number) {
   return `${second}s cubic-bezier(.08,.52,.52,1)`;
 }
-function makeVisiblilityTransition(second: number) {
-  const cubic_bezier = makeCubicBezier(second);
+function useVisiblilityTransition(second: number) {
+  const cubic_bezier = useCubicBezier(second);
   return `opacity ${cubic_bezier}, visibility ${cubic_bezier}`;
 }
 interface IMakeVisibilityTransitionProps {
   visible: boolean;
   second?: number;
   opacity?: BoxProps["opacity"];
   extraTransitions?: string;
 }
-export function makeVisibilityTransitionProps({
+export function useVisibilityTransitionProps({
   visible,
   second,
   opacity,
   extraTransitions,
 }: IMakeVisibilityTransitionProps): {
   visibility: BoxProps["visibility"];
   transition: BoxProps["transition"];
   opacity: BoxProps["opacity"];
 } {
   second ??= 0.3;
   opacity ??= 1.0;
-  const baseTransition = makeVisiblilityTransition(second);
+  const baseTransition = useVisiblilityTransition(second);
   const transition = !!extraTransitions ? `${baseTransition}, ${extraTransitions}` : baseTransition;
   return { visibility: visible ? "visible" : "hidden", transition, opacity: visible ? opacity : 0 };
 }
-export const BG_TRANSITION = "background-color 0.3s ease-in-out";
-const expand_cubic_bezier = makeCubicBezier(0.3);
+export const BG_TRANSITION = `background ${useCubicBezier(0.3)}`;
+const expand_cubic_bezier = useCubicBezier(0.3);
 export const EXPAND_TRANSITION = `height ${expand_cubic_bezier}, transform ${expand_cubic_bezier}, margin-top ${expand_cubic_bezier}`;
 
 export const DEFAULT_PLUGIN_SETTINGS = {
   iconW: 48,
   iconH: 48,
   pivot: "bottom",
   follow: false,
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/event.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/utils/event.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/misc.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/utils/misc.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/src/utils/toast.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/src/utils/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/tsconfig.json` & `carefree-drawboard-0.0.2a0/cfdraw/.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/vite.config.ts` & `carefree-drawboard-0.0.2a0/cfdraw/.web/vite.config.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/.web/yarn.lock` & `carefree-drawboard-0.0.2a0/cfdraw/.web/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -213,41 +213,41 @@
   resolved "https://registry.npmmirror.com/@babel/types/-/types-7.21.5.tgz#18dfbd47c39d3904d5db3d3dc2cc80bedb60e5b6"
   integrity sha512-m4AfNvVF2mVC/F7fDEdH2El3HzUg9It/XsCxZiOTTA3m3qYfcSVSbTfM6Q9xG+hYDniZssYhlXKKUMD5m8tF4Q==
   dependencies:
     "@babel/helper-string-parser" "^7.21.5"
     "@babel/helper-validator-identifier" "^7.19.1"
     to-fast-properties "^2.0.0"
 
-"@carefree0910/business@~0.5.1-alpha.12":
-  version "0.5.1-alpha.12"
-  resolved "https://registry.npmmirror.com/@carefree0910/business/-/business-0.5.1-alpha.12.tgz#fe2c14e8a590ca110b7c43e7376a25ac3e9ed9a9"
-  integrity sha512-jNGSnyee48ReFQpQumPRO4ybD1WoZEsyUb6O6I6tjOhFY8VOYPOv7KlsTRybf5zMsyvufhQT/NnnPwmbubQW4Q==
-  dependencies:
-    "@carefree0910/core" "^0.5.1-alpha.12"
-    "@carefree0910/svg" "^0.5.1-alpha.12"
-
-"@carefree0910/core@^0.5.1-alpha.12", "@carefree0910/core@~0.5.1-alpha.12":
-  version "0.5.1-alpha.12"
-  resolved "https://registry.npmmirror.com/@carefree0910/core/-/core-0.5.1-alpha.12.tgz#9cbcd6387904fc6684ed9dd1e3977f21fa72337d"
-  integrity sha512-vcHr4avN6YAovMocPuhKUR9revZ0qWDGY0SoE9bI9MRHGEVN9XkjELk0USYcpUKRdWNAxejzeCJenPRXdWIvLQ==
-
-"@carefree0910/native@~0.5.1-alpha.12":
-  version "0.5.1-alpha.12"
-  resolved "https://registry.npmmirror.com/@carefree0910/native/-/native-0.5.1-alpha.12.tgz#560905a39f452ae0910115d3f772fbb306a098b6"
-  integrity sha512-Nnbg+5LIODPjYfDx3Oa5TuW4w5tw4VIyIGJJr0mC/JDys/xiSULKzPMJ2cAaaHfQES2TXyO+Ufru9yZRjWrBmA==
-  dependencies:
-    "@carefree0910/core" "^0.5.1-alpha.12"
-    "@carefree0910/svg" "^0.5.1-alpha.12"
-
-"@carefree0910/svg@^0.5.1-alpha.12", "@carefree0910/svg@~0.5.1-alpha.12":
-  version "0.5.1-alpha.12"
-  resolved "https://registry.npmmirror.com/@carefree0910/svg/-/svg-0.5.1-alpha.12.tgz#31d5fbb2b93b66c0995ea8df45bed69806008e18"
-  integrity sha512-7QNGWuu8r02HjwiHEAdGF5dh9lO8Mg+60X9AhvnTcWtftwPDRucXQBZEm02gutF8Anb3Rc4RYtjwxxqI8qwAHw==
+"@carefree0910/business@~0.5.1-alpha.18":
+  version "0.5.1-alpha.18"
+  resolved "https://registry.npmmirror.com/@carefree0910/business/-/business-0.5.1-alpha.18.tgz#ef53257d6975828d6435a442aea48ac54cd93340"
+  integrity sha512-5PAOF3xK79002LdQCWfA0iuikL+DLt+Ei5U6dTDKiiSg84xP+P+h5WPSpZO9iU2oKBAbme6ViVf61nXhNIEweA==
+  dependencies:
+    "@carefree0910/core" "^0.5.1-alpha.18"
+    "@carefree0910/svg" "^0.5.1-alpha.18"
+
+"@carefree0910/core@^0.5.1-alpha.18", "@carefree0910/core@~0.5.1-alpha.18":
+  version "0.5.1-alpha.18"
+  resolved "https://registry.npmmirror.com/@carefree0910/core/-/core-0.5.1-alpha.18.tgz#87afe57ddbd4b0da3a4d570bf4fa48f35c761502"
+  integrity sha512-FBGstQMiTkOsnagDYhQcCgQdpvCNgJH7RIkWuOY1LiEQl37tzAilOe23LSgTAtKhng0N783glqZOkw1s6EnlzQ==
+
+"@carefree0910/native@~0.5.1-alpha.18":
+  version "0.5.1-alpha.18"
+  resolved "https://registry.npmmirror.com/@carefree0910/native/-/native-0.5.1-alpha.18.tgz#5eab83e36ccd874f756cf72125f98e718ba405f9"
+  integrity sha512-KLWCwtFG7nR7ZoBcR+W2LsJwCTFZC5pbOf1npdTx0TcojLFaMYuLp+HBwz8DgEBqrGjmQGzPHiEyWJnxqMQv7w==
+  dependencies:
+    "@carefree0910/core" "^0.5.1-alpha.18"
+    "@carefree0910/svg" "^0.5.1-alpha.18"
+
+"@carefree0910/svg@^0.5.1-alpha.18", "@carefree0910/svg@~0.5.1-alpha.18":
+  version "0.5.1-alpha.18"
+  resolved "https://registry.npmmirror.com/@carefree0910/svg/-/svg-0.5.1-alpha.18.tgz#0c9d3c9ba586904deabad087c795ef081af91983"
+  integrity sha512-ekdFtLgO0ktPDRGXP2zGtdn7sukdJpd2doph4JKrQ9MM7UmZi+Be4Ch6P+i2MjvuWEnypKRidPO64BcaMA9uiQ==
   dependencies:
-    "@carefree0910/core" "^0.5.1-alpha.12"
+    "@carefree0910/core" "^0.5.1-alpha.18"
 
 "@chakra-ui/accordion@2.1.11":
   version "2.1.11"
   resolved "https://registry.npmmirror.com/@chakra-ui/accordion/-/accordion-2.1.11.tgz#c6df0100c543645d0631df3aefde2ea2b8ed6313"
   integrity sha512-mfVPmqETp9pyRDHJ33AdF19oHv/LyxVzQJtlxUByuvs8Cj9QQZ2LQLg5kejm+b3mj03A7A6yfbuo3RNaI4Bhsg==
   dependencies:
     "@chakra-ui/descendant" "3.0.14"
@@ -5502,18 +5502,18 @@
   resolved "https://registry.npmmirror.com/vite-tsconfig-paths/-/vite-tsconfig-paths-4.2.0.tgz#bd2647d3eadafb65a10fc98a2ca565211f2eaf63"
   integrity sha512-jGpus0eUy5qbbMVGiTxCL1iB9ZGN6Bd37VGLJU39kTDD6ZfULTTb1bcc5IeTWqWJKiWV5YihCaibeASPiGi8kw==
   dependencies:
     debug "^4.1.1"
     globrex "^0.1.2"
     tsconfck "^2.1.0"
 
-vite@^4.2.0:
-  version "4.3.5"
-  resolved "https://registry.npmmirror.com/vite/-/vite-4.3.5.tgz#3871fe0f4b582ea7f49a85386ac80e84826367d9"
-  integrity sha512-0gEnL9wiRFxgz40o/i/eTBwm+NEbpUeTWhzKrZDSdKm6nplj+z4lKz8ANDgildxHm47Vg8EUia0aicKbawUVVA==
+vite@^4.3.9:
+  version "4.3.9"
+  resolved "https://registry.yarnpkg.com/vite/-/vite-4.3.9.tgz#db896200c0b1aa13b37cdc35c9e99ee2fdd5f96d"
+  integrity sha512-qsTNZjO9NoJNW7KnOrgYwczm0WctJ8m/yqYAMAK9Lxt4SoySUfS5S8ia9K7JHpa3KEeMfyF8LoJ3c5NeBJy6pg==
   dependencies:
     esbuild "^0.17.5"
     postcss "^8.4.23"
     rollup "^3.21.0"
   optionalDependencies:
     fsevents "~2.3.2"
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/assets.py` & `carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/project.py` & `carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,14 @@
                 )
             except Exception as err:
                 move_to_buggy(path, userId, err)
         with open(upload_project_folder / constants.PROJECT_META_FILE, "w") as f:
             json.dump(project_meta, f)
 
 
-def maintain_all_meta(app: IApp) -> None:
-    for user_folder in app.config.upload_project_folder.iterdir():
-        if user_folder.is_dir():
-            maintain_meta(app, user_folder.name)
-
-
 def add_project_managements(app: IApp) -> None:
     @app.api.post("/save_project", responses=get_responses(SaveProjectResponse))
     def save_project(data: ProjectModel) -> SaveProjectResponse:
         with get_save_project_lock(data.userId):
             try:
                 upload_project_folder = get_project_folder(data.userId)
                 with open(upload_project_folder / f"{data.uid}{suffix}", "w") as f:
@@ -183,14 +177,11 @@
             maintain_meta(app, userId)
 
 
 class ProjectEndpoint(IEndpoint):
     def register(self) -> None:
         add_project_managements(self.app)
 
-    async def on_startup(self) -> None:
-        maintain_all_meta(self.app)
-
 
 __all__ = [
     "ProjectEndpoint",
 ]
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/queue.py` & `carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         uid = random_hash()
         self._queues.push(data.request.userId, Item(uid, data))
         self._senders[uid] = data.request.hash, send_message
         if DEBUG:
             print("~" * 50)
             print("> push.uid", uid)
             print("> push.userId", data.request.userId)
+            print("> push.userJson", data.request.userJson)
             print("> push.hash", data.request.hash)
         return uid
 
     async def run(self) -> None:
         if self._busy_uid is not None:
             return
         while True:
@@ -51,15 +52,18 @@
             request = request_item.data.request
             self._busy_uid = uid
             if DEBUG:
                 print(">>> run", uid)
             try:
                 plugin.elapsed_times.start()
                 if await self._broadcast_working(uid):
-                    await offload(plugin(request))
+                    future = plugin(request)
+                    if not plugin.settings.no_offload:
+                        future = offload(future)
+                    await future
             except Exception as err:
                 await self._broadcast_exception(uid, get_err_msg(err))
             # cleanup
             request_item.data.event.set()
             self._queues.remove(user_id, uid)
             self._senders.pop(uid, None)
             await self._broadcast_pending()
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/upload.py` & `carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 from io import BytesIO
 from PIL import Image
 from typing import Union
 from typing import Optional
 from fastapi import File
 from fastapi import Form
 from fastapi import Request
@@ -46,24 +48,26 @@
     * `upload_image`: save an image with given `contents`, will be better if `meta` can be stored.
     * `fetch_image`: fetch an image based on `url` and `jpeg` flag.
     """
 
     @staticmethod
     async def upload_image(
         contents: Union[bytes, Image.Image],
+        userJson: str,
         meta: PngInfo,
         base_url: str,
         audit: bool,
     ) -> ImageDataModel:
         """
         When this method is used in the:
         * `upload_image` endpoint, `contents` will be a `bytes` object.
-        * `FieldsMiddleWare`, `contents` will be an `Image.Image` object.
+        * `FieldsMiddleware`, `contents` will be an `Image.Image` object.
         """
 
+        meta.add_text("userJson", userJson)
         if isinstance(contents, Image.Image):
             image = contents
         else:
             image = Image.open(BytesIO(contents))
         return ImageDataModel(**save_image(image, meta, base_url))
 
     @staticmethod
@@ -73,24 +77,26 @@
 
 
 def add_upload_image(app: IApp) -> None:
     @app.api.post("/upload_image", responses=get_responses(UploadImageResponse))
     async def upload_image(
         image: UploadFile = File(),
         userId: str = Form(),
+        userJson: Optional[str] = Form(None),
         audit: bool = Form(True),
         *,
         request: Request,
     ) -> UploadImageResponse:
         try:
             base_url = str(request.base_url)
             contents = image.file.read()
-            meta = PngInfo()
-            meta.add_text("userId", userId)
-            data = await ImageUploader.upload_image(contents, meta, base_url, audit)
+            if userJson is None:
+                userJson = json.dumps(dict(userId=userId))
+            args = contents, userJson, PngInfo(), base_url, audit
+            data = await ImageUploader.upload_image(*args)
         except Exception as err:
             err_msg = get_err_msg(err)
             return UploadImageResponse(success=False, message=err_msg, data=None)
         finally:
             image.file.close()
         return UploadImageResponse(success=True, message="", data=data)
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/app/endpoints/websocket.py` & `carefree-drawboard-0.0.2a0/cfdraw/app/endpoints/websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                     identifier = data.identifier
                     target_plugin = app.internal_plugins.make(identifier)
                 else:
                     identifier = data.identifier.split(".", 1)[0]  # remove hash
                     target_plugin = app.plugins.make(identifier)
                 if target_plugin is not None:
                     # `send_message` should be handled by the plugin itself, or by
-                    # the `SendSocketMessageMiddleWare` which will provide a default handling
+                    # the `SendSocketMessageMiddleware` which will provide a default handling
                     target_plugin.task_hash = data.hash
                     target_plugin.send_message = send_message
                     target_plugin.elapsed_times = ElapsedTimes()
                     if data.isInternal:
                         target_plugin.elapsed_times.start()
                         await offload(target_plugin(data))
                     else:
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/app/schema.py` & `carefree-drawboard-0.0.2a0/cfdraw/app/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/config.py` & `carefree-drawboard-0.0.2a0/cfdraw/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     # api
     backend_port: str = constants.BACKEND_PORT
     ## if provided, will be set as `CFDRAW_API_URL`
     backend_hosting_url: Optional[str] = None
     # upload
     upload_root: str = field(default_factory=constants.get_upload_root)
     # board
-    board_settings: BoardSettings = BoardSettings()
+    board_settings: BoardSettings = field(default_factory=BoardSettings)
     # extra plugins
-    extra_plugins: ExtraPlugins = ExtraPlugins()
+    extra_plugins: ExtraPlugins = field(default_factory=ExtraPlugins)
     # misc
     use_react_strict_mode: bool = False
 
     @property
     def prod(self) -> bool:
         return constants.get_env() == constants.Env.PROD
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/constants.py` & `carefree-drawboard-0.0.2a0/cfdraw/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,18 +81,22 @@
 BUGGY_PROJECT_FOLDER = ".buggy"
 PROJECT_META_FILE = "_meta.json"
 
 # icons
 TEXT_TO_IMAGE_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/txt2img.svg"
 IMAGE_TO_IMAGE_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/img2img.svg"
 IMAGE_TO_TEXT_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/img2txt.svg"
-CONTROLNET_ICON = IMAGE_TO_IMAGE_ICON
+CONTROLNET_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/controlnet.svg"
+CONTROLNET_HINT_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/wrench.svg"
 SD_INPAINTING_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/sd-inpainting.svg"
 SD_OUTPAINTING_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/sd-outpainting.svg"
 SR_ICON = (
     "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/sr.svg"
 )
 SOD_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/sod.svg"
 INPAINTING_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/inpainting.svg"
 VARIATION_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/variation.svg"
+HARMONIZATION_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/sparkle.svg"
+WORKFLOW_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/workflow.svg"
+EXECUTE_WORKFLOW_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/execute-workflow.svg"
 DEFAULT_PLUGIN_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/default-plugin.svg"
 DEFAULT_PLUGIN_GROUP_ICON = "https://ailab-huawei-cdn.nolibox.com/upload/static/carefree-drawboard/icons/default-plugin-group.svg"
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/parsers/chakra.py` & `carefree-drawboard-0.0.2a0/cfdraw/parsers/chakra.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/node_validator.py` & `carefree-drawboard-0.0.2a0/cfdraw/plugins/_internal/node_validator.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/plugins/_internal/sync.py` & `carefree-drawboard-0.0.2a0/cfdraw/plugins/_internal/sync.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/plugins/base.py` & `carefree-drawboard-0.0.2a0/cfdraw/plugins/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import abstractmethod
 from abc import ABCMeta
 from PIL import Image
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from cftool.misc import shallow_copy_dict
 
 from cfdraw import constants
 from cfdraw.utils import server
 from cfdraw.utils.misc import offload_run
 from cfdraw.schema.plugins import *
 from cfdraw.plugins.middlewares import *
 from cfdraw.parsers.noli import SingleNodeType
@@ -20,22 +21,23 @@
     @abstractmethod
     async def process(self, data: ISocketRequest) -> Any:
         pass
 
     # internal APIs
 
     @property
-    def middlewares(self) -> List[IMiddleWare]:
+    def middlewares(self) -> List[IMiddleware]:
         return [
-            ResponseMiddleWare(self),
-            TimerMiddleWare(self),
-            SendSocketMessageMiddleWare(self),
+            ResponseMiddleware(self),
+            TimerMiddleware(self),
+            SendSocketMessageMiddleware(self),
         ]
 
     async def __call__(self, data: ISocketRequest) -> ISocketMessage:
+        self.injections = {}
         self.extra_responses = {}
         middlewares = self.middlewares
         for middleware in middlewares:
             await middleware.before(data)
         response = await self.process(data)
         for middleware in middlewares:
             response = await middleware(response)
@@ -76,70 +78,31 @@
         message = ISocketMessage.make_progress(self.task_hash, progress, intermediate)
         return offload_run(self.send_message(message))
 
     def send_exception(self, message: str) -> bool:
         message = ISocketMessage.make_exception(self.task_hash, message)
         return offload_run(self.send_message(message))
 
+    def set_extra_response(self, key: str, value: Any) -> None:
+        self.extra_responses[key] = value
+
+    def set_injection(self, key: str, node: INodeData) -> None:
+        self.injections[key] = dict(
+            meta=shallow_copy_dict(node.meta),
+            bboxFields=None if node.transform is None else node.transform.dict(),
+        )
+
 
 class IInternalSocketPlugin(ISocketPlugin, metaclass=ABCMeta):
     @property
     def type(self) -> PluginType:
         return PluginType._INTERNAL
 
     @property
     def settings(self) -> IPluginSettings:
         return IPluginSettings(w=1, h=1)
 
 
-# bindings
-
-
-class IPluginGroup(ISocketPlugin):
-    @property
-    def type(self) -> PluginType:
-        return PluginType.PLUGIN_GROUP
-
-    def process(self, data: ISocketRequest) -> Any:
-        return
-
-
-class IFieldsPlugin(ISocketPlugin):
-    @property
-    def type(self) -> PluginType:
-        return PluginType.FIELDS
-
-
-class ITextAreaPlugin(ISocketPlugin):
-    @property
-    def type(self) -> PluginType:
-        return PluginType.TEXT_AREA
-
-
-class IQAPlugin(ISocketPlugin):
-    @property
-    def type(self) -> PluginType:
-        return PluginType.QA
-
-
-class IChatPlugin(ISocketPlugin):
-    @property
-    def type(self) -> PluginType:
-        return PluginType.CHAT
-
-
-class IMarkdownPlugin(ISocketPlugin):
-    @property
-    def type(self) -> PluginType:
-        return PluginType.MARKDOWN
-
-
 __all__ = [
     "ISocketPlugin",
     "IInternalSocketPlugin",
-    "IPluginGroup",
-    "IFieldsPlugin",
-    "ITextAreaPlugin",
-    "IQAPlugin",
-    "IChatPlugin",
-    "IMarkdownPlugin",
 ]
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/plugins/factory.py` & `carefree-drawboard-0.0.2a0/cfdraw/plugins/factory.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/response.py` & `carefree-drawboard-0.0.2a0/cfdraw/plugins/middlewares/response.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 from typing import List
 from typing import Union
 from PIL.Image import Image
 from PIL.PngImagePlugin import PngInfo
 
 from cfdraw.schema.plugins import PluginType
-from cfdraw.schema.plugins import IMiddleWare
+from cfdraw.schema.plugins import IMiddleware
 from cfdraw.schema.plugins import Subscription
 from cfdraw.schema.plugins import ISocketMessage
 from cfdraw.schema.plugins import ISocketRequest
 from cfdraw.app.endpoints.upload import ImageUploader
 
 
-class ResponseMiddleWare(IMiddleWare):
+class ResponseMiddleware(IMiddleware):
     @property
     def subscriptions(self) -> Union[List[PluginType], Subscription]:
         return Subscription.ALL
 
     async def before(self, request: ISocketRequest) -> None:
         await super().before(request)
         self.request = request
@@ -38,16 +38,17 @@
             )
         meta = PngInfo()
         meta.add_text("request", self.request.json())
         t = time.time()
         audit = self.plugin.image_should_audit
         upload = ImageUploader.upload_image
         base_url = self.request.baseURL
-        futures = [upload(im, meta, base_url, audit) for im in response]
+        user_json = self.request.get_user_json()
+        futures = [upload(im, user_json, meta, base_url, audit) for im in response]
         urls = [data.dict() for data in await asyncio.gather(*futures)]
         self.plugin.elapsed_times.upload = time.time() - t
         return self.make_success(dict(type="image", value=urls))
 
 
 __all__ = [
-    "ResponseMiddleWare",
+    "ResponseMiddleware",
 ]
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/send_message.py` & `carefree-drawboard-0.0.2a0/cfdraw/plugins/middlewares/send_message.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from typing import List
 from typing import Union
 
 from cfdraw.schema.plugins import PluginType
-from cfdraw.schema.plugins import IMiddleWare
+from cfdraw.schema.plugins import IMiddleware
 from cfdraw.schema.plugins import Subscription
 from cfdraw.schema.plugins import ISocketMessage
 
 
-class SendSocketMessageMiddleWare(IMiddleWare):
+class SendSocketMessageMiddleware(IMiddleware):
     @property
     def subscriptions(self) -> Union[List[PluginType], Subscription]:
         return Subscription.ALL
 
     @property
     def can_handle_message(self) -> bool:
         return True
 
     async def process(self, response: ISocketMessage) -> ISocketMessage:
         if self.plugin.extra_responses:
             if response.data.final is None:
                 response.data.final = {}
             response.data.final["extra"] = self.plugin.extra_responses
+            response.data.injections = self.plugin.injections
         await self.plugin.send_message(response)
         return response
 
 
 __all__ = [
-    "SendSocketMessageMiddleWare",
+    "SendSocketMessageMiddleware",
 ]
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/plugins/middlewares/timer.py` & `carefree-drawboard-0.0.2a0/cfdraw/plugins/middlewares/timer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 
 from cfdraw.schema.plugins import PluginType
-from cfdraw.schema.plugins import IMiddleWare
+from cfdraw.schema.plugins import IMiddleware
 from cfdraw.schema.plugins import ISocketMessage
 
 
-class TimerMiddleWare(IMiddleWare):
+class TimerMiddleware(IMiddleware):
     @property
     def can_handle_message(self) -> bool:
         return True
 
     @property
     def subscriptions(self) -> List[PluginType]:
         return [PluginType.FIELDS]
@@ -17,9 +17,9 @@
     async def process(self, response: ISocketMessage) -> ISocketMessage:
         self.plugin.elapsed_times.end()
         response.data.elapsedTimes = self.plugin.elapsed_times
         return response
 
 
 __all__ = [
-    "TimerMiddleWare",
+    "TimerMiddleware",
 ]
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/schema/fields.py` & `carefree-drawboard-0.0.2a0/cfdraw/schema/fields.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 from typing import Optional
 from pathlib import Path
 from pydantic import Extra
 from pydantic import Field
 from pydantic import BaseModel
 
 from cfdraw.parsers.noli import IStr
+from cfdraw.parsers.noli import I18N
 from cfdraw.parsers.chakra import IChakra
 
 
 """ This file should be identical to `src/schema/fields.ts` """
 
 
 class FieldType(str, Enum):
     TEXT = "text"
     IMAGE = "image"
     NUMBER = "number"
     SELECT = "select"
+    I18N_SELECT = "i18n_select"
     SELECT_LOCAL = "select_local"
     BOOLEAN = "boolean"
     COLOR = "color"
     LIST = "list"
     OBJECT = "object"
 
 
@@ -67,20 +69,48 @@
     isInt: Optional[bool] = Field(None, description="Whether the field is an integer")
     scale: Optional[NumberScale] = Field(None, description="The scale of the field")
     precision: Optional[int] = Field(None, description="The precision of the field")
     type: FieldType = Field(FieldType.NUMBER, description="Type", const=True)
 
 
 class ISelectField(IBaseField):
-    values: List[IStr] = Field(..., description="The values of the field")
+    options: List[IStr] = Field(..., description="The options of the field")
     default: IStr = Field(..., description="The default value of the field")
     isMulti: Optional[bool] = Field(None, description="Whether use multi-select")
     type: FieldType = Field(FieldType.SELECT, description="Type", const=True)
 
 
+class I18NSelectField(IBaseField):
+    mapping: Dict[str, I18N] = Field(
+        ...,
+        description=(
+            "The mapping of the options. "
+            "The key is the 'actual' option, and the value is the i18n object to be displayed"
+        ),
+    )
+    default: str = Field(..., description="The default 'actual' option of the field")
+    isMulti: Optional[bool] = Field(None, description="Whether use multi-select")
+    type: FieldType = Field(FieldType.I18N_SELECT, description="Type", const=True)
+
+    def dict(self, **kwargs: Any) -> Dict[str, Any]:
+        d = super().dict(**kwargs)
+        d["type"] = FieldType.SELECT.value
+        mapping, default = map(d.pop, ["mapping", "default"])
+        d["options"] = list(mapping.values())
+        d["default"] = mapping[default]
+        return d
+
+    def parse(self, i18n_d: Dict[str, str]) -> Optional[str]:
+        i18n = I18N(**i18n_d)
+        for k, v in self.mapping.items():
+            if i18n == v:
+                return k
+        return None
+
+
 class ISelectLocalField(IBaseField):
     path: str = Field(..., description="The local path you want to read")
     default: Optional[str] = Field(None, description="The default value of the field")
     regex: Optional[str] = Field(None, description="The regex to filter the files")
     noExt: bool = Field(False, description="Whether to remove the extension")
     onlyFiles: bool = Field(True, description="Whether only consider files")
     defaultPlaceholder: Optional[str] = Field(
@@ -118,18 +148,18 @@
         kw = dict(
             path=d.pop("path"),
             regex=d.pop("regex"),
             noExt=d.pop("noExt"),
             onlyFiles=d.pop("onlyFiles"),
             defaultPlaceholder=d.pop("defaultPlaceholder"),
         )
-        values = self.get_options(**kw)
-        d["values"] = values
+        options = self.get_options(**kw)
+        d["options"] = options
         if d["default"] is None:
-            d["default"] = values[0]
+            d["default"] = options[0]
         d["isLocal"] = True
         d["localProperties"] = kw
         return d
 
 
 class IBooleanField(IBaseField):
     default: bool = Field(..., description="The default value of the field")
@@ -161,14 +191,15 @@
 
 
 IFieldDefinition = Union[
     ITextField,
     IImageField,
     INumberField,
     ISelectField,
+    I18NSelectField,
     ISelectLocalField,
     IBooleanField,
     IColorField,
     IListField,
     IObjectField,
 ]
 IListField.update_forward_refs()
@@ -178,14 +209,15 @@
 __all__ = [
     "FieldType",
     "ITextField",
     "IImageField",
     "NumberScale",
     "INumberField",
     "ISelectField",
+    "I18NSelectField",
     "ISelectLocalField",
     "IBooleanField",
     "IColorField",
     "IListField",
     "IObjectField",
     "IFieldDefinition",
 ]
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/schema/plugins.py` & `carefree-drawboard-0.0.2a0/cfdraw/schema/plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import time
 
 from abc import abstractmethod
 from abc import ABC
 from PIL import Image
 from enum import Enum
 from typing import Any
@@ -228,25 +229,35 @@
     offsetY: Optional[int] = Field(None, description="Y offset of the plugin button")
     bgOpacity: Optional[float] = Field(None, description="Opacity of the plugin button")
     useModal: bool = Field(False, description="Whether popup a modal for the plugin")
     keepOpen: bool = Field(
         False,
         description="Whether should we keep the expanded panel of the plugin open, even when users already clicked on the drawboard.",
     )
-    modalOpacity: Optional[float] = Field(None, description="Opacity of the modal")
+    expandOpacity: Optional[float] = Field(None, description="Opacity of the modal")
     expandProps: Optional[IChakra] = Field(
         None,
         description="Extra (chakra) props of the plugin's expanded panel",
     )
     # React fields
     pluginInfo: IPluginInfo = Field(IPluginInfo(), description="Plugin info")
     buttonProps: Optional[Dict[str, Any]] = Field(
         None,
         description="Extra (chakra) props of the plugin button",
     )
+    # internal fields
+    no_offload: bool = Field(
+        False,
+        description=(
+            "Whether not to offload the plugin to sub-thread when it is executed, "
+            "useful when you know the plugin is fast enough.\n"
+            "> This is introduced mainly because some libraries (e.g., `matplotlib`) "
+            "need to be executed in the main thread."
+        ),
+    )
 
     def to_react(self, type: str, hash: str, identifier: str) -> Dict[str, Any]:
         d = self.dict(exclude={"pluginInfo"})
         pI = self.pluginInfo
         kw = dict(exclude={"plugins"}) if isinstance(pI, IPluginGroupInfo) else {}
         plugin_info = self.pluginInfo.dict(**kw)
         plugin_info["identifier"] = identifier
@@ -352,20 +363,33 @@
         None,
         description=(
             "Will be a list of `INodeData` if and only if "
             "the node is a `Group` (i.e. `type` == 'group')"
         ),
     )
 
+    @property
+    def identifier(self) -> Optional[str]:
+        if self.meta is None:
+            return None
+        return self.meta.get("data", {}).get("identifier")
+
+    @property
+    def extra_responses(self) -> Optional[Dict[str, Any]]:
+        if self.meta is None:
+            return None
+        return self.meta.get("data", {}).get("response", {}).get("extra")
+
 
 class ISocketRequest(BaseModel):
     """This should align with `IPythonSocketRequest` at `src/schema/_python.ts`"""
 
     hash: str = Field(..., description="The hash of the request")
     userId: str = Field(..., description="The id of the user")
+    userJson: Optional[str] = Field(None, description="Full json of the user info")
     baseURL: str = Field(..., description="The base url of the request")
     identifier: str = Field(..., description="The identifier of the plugin")
     nodeData: INodeData = Field(
         ...,
         description="""
 Data extracted from `node`.
 > If multiple nodes are selected, this field will be empty and please use `nodeDataList` instead.
@@ -377,14 +401,19 @@
 List of data extracted from `nodes`.
 > If only one node is selected, this field will be empty and please use `nodeData` instead.
 """,
     )
     extraData: Dict[str, Any] = Field(..., description="Extra data of each plugin")
     isInternal: bool = Field(False, description="Whether the request is internal")
 
+    def get_user_json(self) -> str:
+        if self.userJson is not None:
+            return self.userJson
+        return json.dumps(dict(userId=self.userId))
+
 
 class SocketStatus(str, Enum):
     """This should align with `PythonSocketStatus` at `src/schema/_python.ts`"""
 
     PENDING = "pending"
     WORKING = "working"
     FINISHED = "finished"
@@ -415,14 +444,15 @@
         description="Progress of current task, if any",
     )
     intermediate: Optional[ISocketIntermediate] = Field(
         None,
         description="Intermediate responses, if any",
     )
     final: Optional[Dict[str, Any]] = Field(None, description="Final response, if any")
+    injections: Optional[Dict[str, Any]] = Field(None, description="Injections, if any")
     elapsedTimes: Optional[ElapsedTimes] = Field(None, description="Elapsed times.")
 
 
 class ISocketMessage(BaseModel):
     """This should align with `IPythonSocketMessage` at `src/schema/_python.ts`"""
 
     hash: str = Field(..., description="Hash of the current task")
@@ -478,14 +508,15 @@
     identifier: str
     http_session: ClientSession
     # task specific
     task_hash: str
     send_message: ISend
     elapsed_times: ElapsedTimes
     extra_responses: Dict[str, Any]
+    injections: Dict[str, Any]
     # internal
     _in_group: bool = False
 
     # abstract
 
     @property
     @abstractmethod
@@ -523,25 +554,23 @@
     ) -> bool:
         pass
 
     # optional
 
     ## Whether the images generated by this plugin should be audited
     image_should_audit: bool = True
-    ## List of python package requirements of the plugin
-    requirements: Optional[List[str]] = None
     ## The notification (introductions, hardware requirements, etc.) you want to print out
     notification: Optional[str] = None
 
 
 class Subscription(str, Enum):
     ALL = "__all__"
 
 
-class IMiddleWare(ABC):
+class IMiddleware(ABC):
     hash: str
     plugin: IPlugin
 
     # abstract
 
     @property
     @abstractmethod
@@ -658,15 +687,15 @@
     "ISocketRequest",
     "SocketStatus",
     "ISocketIntermediate",
     "ISocketResponse",
     "ISocketMessage",
     # plugin interface
     "IPlugin",
-    "IMiddleWare",
+    "IMiddleware",
     "IFieldsPluginInfo",
     # bindings
     "ILogoPluginInfo",
     "ILogoSettings",
     "IPluginGroupInfo",
     "ITextAreaPluginInfo",
     "IQAPluginInfo",
```

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/schema/settings.py` & `carefree-drawboard-0.0.2a0/cfdraw/schema/settings.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/utils/cache.py` & `carefree-drawboard-0.0.2a0/cfdraw/utils/cache.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/utils/console.py` & `carefree-drawboard-0.0.2a0/cfdraw/utils/console.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/utils/exec.py` & `carefree-drawboard-0.0.2a0/cfdraw/utils/exec.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/utils/misc.py` & `carefree-drawboard-0.0.2a0/cfdraw/utils/misc.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/utils/prerequisites.py` & `carefree-drawboard-0.0.2a0/cfdraw/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/utils/processes.py` & `carefree-drawboard-0.0.2a0/cfdraw/utils/processes.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/utils/server.py` & `carefree-drawboard-0.0.2a0/cfdraw/utils/server.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.1a4/cfdraw/utils/template.py` & `carefree-drawboard-0.0.2a0/cfdraw/utils/template.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     @property
     def settings(self) -> IPluginSettings:
         return IPluginSettings(
             w=300,
             h=180,
             tooltip="Apply Gaussian Blur to the image",
             nodeConstraint=NodeConstraints.IMAGE,
-            pivot=PivotType.RT,
             follow=True,
+            pivot=PivotType.RT,
             pluginInfo=IFieldsPluginInfo(
                 definitions=dict(
                     size=INumberField(
                         default=3,
                         min=1,
                         max=10,
                         step=1,
```

### Comparing `carefree-drawboard-0.0.1a4/setup.py` & `carefree-drawboard-0.0.2a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1-alpha.4"
+VERSION = "0.0.2-alpha.0"
 PACKAGE_NAME = "carefree-drawboard"
 
 DESCRIPTION = "🎨 Infinite Drawboard in Python"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
@@ -19,15 +19,15 @@
         "fastapi>=0.95.1",
         "gunicorn",
         "pydantic",
         "uvicorn",
         "websockets",
         "watchdog",
         "python-multipart",
-        "carefree-toolkit>=0.3.5",
+        "carefree-toolkit>=0.3.6.2",
         "pillow",
         "aiohttp",
         "charset-normalizer==2.1.0",
         "aiofiles",
         "regex",
         "filelock",
     ],
```

