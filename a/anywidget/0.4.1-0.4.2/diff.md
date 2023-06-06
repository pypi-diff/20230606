# Comparing `tmp/anywidget-0.4.1.tar.gz` & `tmp/anywidget-0.4.2.tar.gz`

## Comparing `anywidget-0.4.1.tar` & `anywidget-0.4.2.tar`

### file list

```diff
@@ -1,103 +1,102 @@
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget.json
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 anywidget-0.4.1/package.json
--rw-r--r--   0        0        0   251374 2020-02-02 00:00:00.000000 anywidget-0.4.1/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.4.1/pnpm-workspace.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.4.1/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/__init__.py
--rw-r--r--   0        0        0    25080 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/_version.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/experimental.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/widget.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/static/138.da9bcb3835f584489120.js
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/static/326.00a9c40e24b6392a7970.js
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/static/remoteEntry.68d0702ea589c32d2c52.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 anywidget-0.4.1/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/astro.config.mjs
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/scripts/render.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Counter.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     6344 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/en/experimental.md
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.4.1/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.4.1/examples/Counter.ipynb
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 anywidget-0.4.1/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/package.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 anywidget-0.4.1/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_descriptor.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_experimental.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_utils.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.4.1/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.4.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.4.1/LICENSE
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.4.1/README.md
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 anywidget-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 anywidget-0.4.2/package.json
+-rw-r--r--   0        0        0   259862 2020-02-02 00:00:00.000000 anywidget-0.4.2/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.4.2/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.4.2/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/__init__.py
+-rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/_version.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/experimental.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/static/138.60ddf4a50d830c18a721.js
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/static/326.53aec23a9e055d4c6252.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/static/remoteEntry.9229e22154b84f74e1ee.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/astro.config.js
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/scripts/render.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/en/experimental.md
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.4.2/examples/Counter.ipynb
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 anywidget-0.4.2/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_descriptor.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_experimental.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_utils.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.4.2/README.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 anywidget-0.4.2/PKG-INFO
```

### Comparing `anywidget-0.4.1/.pre-commit-config.yaml` & `anywidget-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/package.json` & `anywidget-0.4.2/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'packageManager'": "'pnpm@8.6.1'"}*

```diff
@@ -2,15 +2,15 @@
     "devDependencies": {
         "@changesets/cli": "^2.26.0",
         "@svitejs/changesets-changelog-github-compact": "^1.1.0",
         "esbuild": "^0.17.12",
         "typescript": "^5.0.2"
     },
     "name": "@anywidget/monorepo",
-    "packageManager": "pnpm@7.30.0",
+    "packageManager": "pnpm@8.6.1",
     "scripts": {
         "build": "pnpm build:nb && pnpm build:lab",
         "build:lab": "jupyter labextension build packages/anywidget",
         "build:nb": "pnpm --filter=!docs build && cp packages/anywidget/dist/index.js anywidget/nbextension/index.js",
         "clean": "rm -rf anywidget/nbextension/index.js anywidget/labextension && pnpm -r exec rm -rf dist",
         "release": "python -m build && changeset publish && twine upload dist/*",
         "version": "changeset version && pnpm install"
```

### Comparing `anywidget-0.4.1/pnpm-lock.yaml` & `anywidget-0.4.2/pnpm-lock.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-lockfileVersion: '6.0'
+lockfileVersion: '6.1'
+
+settings:
+  autoInstallPeers: true
+  excludeLinksFromLockfile: false
 
 importers:
 
   .:
     devDependencies:
       '@changesets/cli':
         specifier: ^2.26.0
@@ -19,62 +23,65 @@
 
   docs:
     dependencies:
       '@algolia/client-search':
         specifier: ^4.13.1
         version: 4.15.0
       '@astrojs/markdown-remark':
-        specifier: ^2.1.0
-        version: 2.1.0(astro@2.1.2)
+        specifier: ^2.2.1
+        version: 2.2.1(astro@2.5.7)
       '@astrojs/mdx':
-        specifier: ^0.15.1
-        version: 0.15.2(astro@2.1.2)(rollup@3.18.0)
+        specifier: ^0.19.6
+        version: 0.19.6(astro@2.5.7)
       '@astrojs/preact':
-        specifier: ^2.0.0
-        version: 2.1.0(preact@10.13.0)
+        specifier: ^2.2.1
+        version: 2.2.1(preact@10.13.0)
       '@astrojs/react':
-        specifier: ^2.0.1
-        version: 2.1.0(@types/react-dom@18.0.11)(@types/react@17.0.53)(react-dom@18.2.0)(react@18.2.0)
+        specifier: ^2.2.1
+        version: 2.2.1(@types/react-dom@18.2.4)(@types/react@18.2.8)(react-dom@18.2.0)(react@18.2.0)
       '@astrojs/tailwind':
-        specifier: ^3.0.0
-        version: 3.1.0(astro@2.1.2)(tailwindcss@3.2.7)
+        specifier: ^3.1.3
+        version: 3.1.3(astro@2.5.7)(tailwindcss@3.3.2)
       '@docsearch/css':
         specifier: ^3.1.0
         version: 3.3.3
       '@docsearch/react':
         specifier: ^3.1.0
-        version: 3.3.3(@algolia/client-search@4.15.0)(@types/react@17.0.53)(react-dom@18.2.0)(react@18.2.0)
+        version: 3.3.3(@algolia/client-search@4.15.0)(@types/react@18.2.8)(react-dom@18.2.0)(react@18.2.0)
+      '@types/html-escaper':
+        specifier: ^3.0.0
+        version: 3.0.0
       '@types/node':
         specifier: ^18.0.0
         version: 18.14.6
       '@types/react':
-        specifier: ^17.0.45
-        version: 17.0.53
+        specifier: ^18.2.8
+        version: 18.2.8
       '@types/react-dom':
-        specifier: ^18.0.0
-        version: 18.0.11
-      astro:
-        specifier: ^2.0.2
-        version: 2.1.2(@types/node@18.14.6)
+        specifier: ^18.2.4
+        version: 18.2.4
       gray-matter:
         specifier: ^4.0.3
         version: 4.0.3
       preact:
         specifier: ^10.7.3
         version: 10.13.0
       react:
-        specifier: ^18.1.0
+        specifier: ^18.2.0
         version: 18.2.0
       react-dom:
-        specifier: ^18.1.0
+        specifier: ^18.2.0
         version: 18.2.0(react@18.2.0)
       tailwindcss:
-        specifier: ^3.2.4
-        version: 3.2.7(postcss@8.4.21)
+        specifier: ^3.3.2
+        version: 3.3.2
     devDependencies:
+      astro:
+        specifier: ^2.5.7
+        version: 2.5.7(@types/node@18.14.6)
       html-escaper:
         specifier: ^3.0.3
         version: 3.0.3
       prettier:
         specifier: ^2.8.2
         version: 2.8.4
       prettier-plugin-astro:
@@ -224,329 +231,341 @@
     resolution: {integrity: sha512-JoWR+ixG3EmA0UPntQFN/FV5TasYcYu93d5+oKzHFeZ6Z7rtW5Im9iy/Oh/ggk1AAN5fTdqKewtbBpdaYDbKsQ==}
     dependencies:
       '@algolia/cache-common': 4.15.0
       '@algolia/logger-common': 4.15.0
       '@algolia/requester-common': 4.15.0
     dev: false
 
+  /@alloc/quick-lru@5.2.0:
+    resolution: {integrity: sha512-UrcABB+4bUrFABwbluTIBErXwvbsU/V7TZWfmbgJfbkwiBuziS9gxdODUyuiecfdGQ85jglMW6juS3+z5TsKLw==}
+    engines: {node: '>=10'}
+    dev: false
+
   /@ampproject/remapping@2.2.0:
     resolution: {integrity: sha512-qRmjj8nj9qmLTQXXmaR1cck3UXSRMPrbsLJAasZpF+t3riI71BXed5ebIOYwQntykeZuhjsdweEc9BxH5Jc26w==}
     engines: {node: '>=6.0.0'}
     dependencies:
       '@jridgewell/gen-mapping': 0.1.1
       '@jridgewell/trace-mapping': 0.3.17
-    dev: false
 
   /@astrojs/compiler@0.31.4:
     resolution: {integrity: sha512-6bBFeDTtPOn4jZaiD3p0f05MEGQL9pw2Zbfj546oFETNmjJFWO3nzHz6/m+P53calknCvyVzZ5YhoBLIvzn5iw==}
+    dev: true
 
-  /@astrojs/compiler@1.2.0:
-    resolution: {integrity: sha512-O8yPCyuq+PU9Fjht2tIW6WzSWiq8qDF1e8uAX2x+SOGFzKqOznp52UlDG2mSf+ekf0Z3R34sb64O7SgX+asTxg==}
-    dev: false
+  /@astrojs/compiler@1.5.0:
+    resolution: {integrity: sha512-k04X/7nlMklU0HQUScxbCTf5n8/Vr+0U0bawb9QWulWxd6qJf3FmBrNATgTYiltjB4pc5HBqmmttAfFi7m4lLg==}
 
-  /@astrojs/language-server@0.28.3:
-    resolution: {integrity: sha512-fPovAX/X46eE2w03jNRMpQ7W9m2mAvNt4Ay65lD9wl1Z5vIQYxlg7Enp9qP225muTr4jSVB5QiLumFJmZMAaVA==}
+  /@astrojs/language-server@1.0.8:
+    resolution: {integrity: sha512-gssRxLGb8XnvKpqSzrDW5jdzdFnXD7eBXVkPCkkt2hv7Qzb+SAzv6hVgMok3jDCxpR1aeB+XNd9Qszj2h29iog==}
     hasBin: true
     dependencies:
+      '@astrojs/compiler': 1.5.0
+      '@jridgewell/trace-mapping': 0.3.17
       '@vscode/emmet-helper': 2.8.6
       events: 3.3.0
-      prettier: 2.8.4
-      prettier-plugin-astro: 0.7.2
-      source-map: 0.7.4
+      prettier: 2.8.8
+      prettier-plugin-astro: 0.9.1
       vscode-css-languageservice: 6.2.4
       vscode-html-languageservice: 5.0.4
       vscode-languageserver: 8.1.0
       vscode-languageserver-protocol: 3.17.3
       vscode-languageserver-textdocument: 1.0.8
       vscode-languageserver-types: 3.17.3
       vscode-uri: 3.0.7
-    dev: false
 
-  /@astrojs/markdown-remark@2.1.0(astro@2.1.2):
-    resolution: {integrity: sha512-w9T5o3UWQIfMcCkM2nLWrlfVQazh/7mw+2N/85QGcSUkZy6oNJoyy8Xz/ZkDhHLx8HPO0RT9fABR0B/H+aDaEw==}
+  /@astrojs/markdown-remark@2.2.1(astro@2.5.7):
+    resolution: {integrity: sha512-VF0HRv4GpC1XEMLnsKf6jth7JSmlt9qpqP0josQgA2eSpCIAC/Et+y94mgdBIZVBYH/yFnMoIxgKVe93xfO2GA==}
     peerDependencies:
-      astro: ^2.1.0
+      astro: ^2.5.0
     dependencies:
-      '@astrojs/prism': 2.1.0
-      astro: 2.1.2(@types/node@18.14.6)
+      '@astrojs/prism': 2.1.2
+      astro: 2.5.7(@types/node@18.14.6)
       github-slugger: 1.5.0
-      image-size: 1.0.2
       import-meta-resolve: 2.2.1
       rehype-raw: 6.1.1
       rehype-stringify: 9.0.3
       remark-gfm: 3.0.1
       remark-parse: 10.0.1
       remark-rehype: 10.1.0
       remark-smartypants: 2.0.0
-      shiki: 0.11.1
+      shiki: 0.14.1
       unified: 10.1.2
       unist-util-visit: 4.1.2
       vfile: 5.3.7
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
-  /@astrojs/mdx@0.15.2(astro@2.1.2)(rollup@3.18.0):
-    resolution: {integrity: sha512-vrv1fw5kLZqaV0FHr6IKR46Rq5DENHhqUVZIXpAbvpRG/qXxHpg9QVN9ji+3bgLDKvG2Yz4wi8CYvSjmUtJHBQ==}
+  /@astrojs/mdx@0.19.6(astro@2.5.7):
+    resolution: {integrity: sha512-P9CU+l/GveJPG3OOOdlZtIK5NWcJuEnXPtxwfjJUaoIPHDByp6okT/yN/WwLAA4TfnluFnULNG4bDsEnwcpYvw==}
     engines: {node: '>=16.12.0'}
     dependencies:
-      '@astrojs/markdown-remark': 2.1.0(astro@2.1.2)
-      '@astrojs/prism': 2.1.0
+      '@astrojs/markdown-remark': 2.2.1(astro@2.5.7)
+      '@astrojs/prism': 2.1.2
       '@mdx-js/mdx': 2.3.0
-      '@mdx-js/rollup': 2.3.0(rollup@3.18.0)
       acorn: 8.8.2
-      es-module-lexer: 0.10.5
+      es-module-lexer: 1.2.0
       estree-util-visit: 1.2.1
       github-slugger: 1.5.0
       gray-matter: 4.0.3
+      hast-util-to-html: 8.0.4
       kleur: 4.1.5
       rehype-raw: 6.1.1
       remark-frontmatter: 4.0.1
       remark-gfm: 3.0.1
       remark-smartypants: 2.0.0
-      shiki: 0.11.1
+      shiki: 0.14.1
+      source-map: 0.7.4
       unist-util-visit: 4.1.2
       vfile: 5.3.7
     transitivePeerDependencies:
       - astro
-      - rollup
       - supports-color
     dev: false
 
-  /@astrojs/preact@2.1.0(preact@10.13.0):
-    resolution: {integrity: sha512-1AnXpnjC24/mWJyq+EN5DoWp+w9Hg/y3dwFX3728rlBhyuY573jx+4+VHuG/g0A1alzJuIAhSPtqCP0YQktUnw==}
+  /@astrojs/preact@2.2.1(preact@10.13.0):
+    resolution: {integrity: sha512-lObgrX/qfK2sEnGDWoyQ8KojFJ54FIKB4TeywWmgj4ZTg0yLnvvOz6ReyPQ8VfR/1MU+vWs22jE4cuZJ/vPnOA==}
     engines: {node: '>=16.12.0'}
     peerDependencies:
       preact: ^10.6.5
     dependencies:
-      '@babel/core': 7.21.0
-      '@babel/plugin-transform-react-jsx': 7.21.0(@babel/core@7.21.0)
+      '@babel/core': 7.22.1
+      '@babel/plugin-transform-react-jsx': 7.21.0(@babel/core@7.22.1)
       '@preact/signals': 1.1.3(preact@10.13.0)
       babel-plugin-module-resolver: 5.0.0
       preact: 10.13.0
       preact-render-to-string: 5.2.6(preact@10.13.0)
     transitivePeerDependencies:
       - supports-color
     dev: false
 
-  /@astrojs/prism@2.1.0:
-    resolution: {integrity: sha512-+II6nfIFGZ7iH0FunhRGcj/J1mCxjcHl85cZRuFePKLoIhFHJT3nC3myQnUw386hUaIn2W20McxxtAVf4leeRQ==}
+  /@astrojs/prism@2.1.2:
+    resolution: {integrity: sha512-3antim1gb34689GHRQFJ88JEo93HuZKQBnmxDT5W/nxiNz1p/iRxnCTEhIbJhqMOTRbbo5h2ldm5qSxx+TMFQA==}
     engines: {node: '>=16.12.0'}
     dependencies:
       prismjs: 1.29.0
-    dev: false
 
-  /@astrojs/react@2.1.0(@types/react-dom@18.0.11)(@types/react@17.0.53)(react-dom@18.2.0)(react@18.2.0):
-    resolution: {integrity: sha512-AzopsCVjsHlX1oVkgLusDRngnpJfoi03kj6c8p/K6+i/PQ3ZnVwRmJl7IgFBC2YJSbexyNxK2BmLvwkjGvQaCA==}
+  /@astrojs/react@2.2.1(@types/react-dom@18.2.4)(@types/react@18.2.8)(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-nq5Zr8iWdwjSp5fh1NReaCplwsnL4w5PXAY5XWu1jE/frxEfF/ycGHrrhwWW0uJHX9G+kUtmQLR0GBhlR4FmAw==}
     engines: {node: '>=16.12.0'}
     peerDependencies:
       '@types/react': ^17.0.50 || ^18.0.21
       '@types/react-dom': ^17.0.17 || ^18.0.6
       react: ^17.0.2 || ^18.0.0
       react-dom: ^17.0.2 || ^18.0.0
     dependencies:
-      '@babel/core': 7.21.0
-      '@babel/plugin-transform-react-jsx': 7.21.0(@babel/core@7.21.0)
-      '@types/react': 17.0.53
-      '@types/react-dom': 18.0.11
+      '@babel/core': 7.22.1
+      '@babel/plugin-transform-react-jsx': 7.21.0(@babel/core@7.22.1)
+      '@types/react': 18.2.8
+      '@types/react-dom': 18.2.4
       react: 18.2.0
       react-dom: 18.2.0(react@18.2.0)
     transitivePeerDependencies:
       - supports-color
     dev: false
 
-  /@astrojs/tailwind@3.1.0(astro@2.1.2)(tailwindcss@3.2.7):
-    resolution: {integrity: sha512-eNflzlCdCtLZjc8pK0xQb/hXYnN/mVGVJFRAMWStrFwg8Tsvj6WVCPyRy77D5NL2tQ1piS2wiouOzAgiy1Dsiw==}
+  /@astrojs/tailwind@3.1.3(astro@2.5.7)(tailwindcss@3.3.2):
+    resolution: {integrity: sha512-10S1omrv5K5HRVAZ0fBgN5vQykn2HRL332LAVFyBASMn1Ff6gDfSK+CPUeUu94eZUOEaPnECLK8EHAqZ8iY9CA==}
     peerDependencies:
-      astro: ^2.1.0
+      astro: ^2.5.0
       tailwindcss: ^3.0.24
     dependencies:
       '@proload/core': 0.3.3
-      astro: 2.1.2(@types/node@18.14.6)
-      autoprefixer: 10.4.13(postcss@8.4.21)
-      postcss: 8.4.21
-      postcss-load-config: 4.0.1(postcss@8.4.21)
-      tailwindcss: 3.2.7(postcss@8.4.21)
+      astro: 2.5.7(@types/node@18.14.6)
+      autoprefixer: 10.4.14(postcss@8.4.24)
+      postcss: 8.4.24
+      postcss-load-config: 4.0.1(postcss@8.4.24)
+      tailwindcss: 3.3.2
     transitivePeerDependencies:
       - ts-node
     dev: false
 
-  /@astrojs/telemetry@2.1.0:
-    resolution: {integrity: sha512-P3gXNNOkRJM8zpnasNoi5kXp3LnFt0smlOSUXhkynfJpTJMIDrcMbKpNORN0OYbqpKt9JPdgRN7nsnGWpbH1ww==}
+  /@astrojs/telemetry@2.1.1:
+    resolution: {integrity: sha512-4pRhyeQr0MLB5PKYgkdu+YE8sSpMbHL8dUuslBWBIdgcYjtD1SufPMBI8pgXJ+xlwrQJHKKfK2X1KonHYuOS9A==}
     engines: {node: '>=16.12.0'}
     dependencies:
       ci-info: 3.8.0
       debug: 4.3.4
       dlv: 1.1.3
       dset: 3.1.2
       is-docker: 3.0.0
       is-wsl: 2.2.0
-      undici: 5.20.0
+      undici: 5.22.1
       which-pm-runs: 1.1.0
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
-  /@astrojs/webapi@2.1.0:
-    resolution: {integrity: sha512-sbF44s/uU33jAdefzKzXZaENPeXR0sR3ptLs+1xp9xf5zIBhedH2AfaFB5qTEv9q5udUVoKxubZGT3G1nWs6rA==}
+  /@astrojs/webapi@2.2.0:
+    resolution: {integrity: sha512-mHAOApWyjqSe5AQMOUD9rsZJqbMQqe3Wosb1a40JV6Okvyxj1G6GTlthwYadWCymq/lbgwh0PLiY8Fr4eFxtuQ==}
     dependencies:
-      undici: 5.20.0
-    dev: false
+      undici: 5.22.1
 
   /@babel/code-frame@7.18.6:
     resolution: {integrity: sha512-TDCmlK5eOvH+eH7cdAFlNXeVJqWIQ7gW9tY1GJIpUtFb6CmjVyq2VM3u71bOyR8CRihcCgMUYoDNyLXao3+70Q==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/highlight': 7.18.6
 
-  /@babel/compat-data@7.21.0:
-    resolution: {integrity: sha512-gMuZsmsgxk/ENC3O/fRw5QY8A9/uxQbbCEypnLIiYYc/qVJtEV7ouxC3EllIIwNzMqAQee5tanFabWsUOutS7g==}
+  /@babel/code-frame@7.21.4:
+    resolution: {integrity: sha512-LYvhNKfwWSPpocw8GI7gpK2nq3HSDuEPC/uSYaALSJu9xjsalaaYFOq0Pwt5KmVqwEbZlDu81aLXwBOmD/Fv9g==}
     engines: {node: '>=6.9.0'}
-    dev: false
+    dependencies:
+      '@babel/highlight': 7.18.6
 
-  /@babel/core@7.21.0:
-    resolution: {integrity: sha512-PuxUbxcW6ZYe656yL3EAhpy7qXKq0DmYsrJLpbB8XrsCP9Nm+XCg9XFMb5vIDliPD7+U/+M+QJlH17XOcB7eXA==}
+  /@babel/compat-data@7.22.3:
+    resolution: {integrity: sha512-aNtko9OPOwVESUFp3MZfD8Uzxl7JzSeJpd7npIoxCasU37PFbAQRpKglkaKwlHOyeJdrREpo8TW8ldrkYWwvIQ==}
+    engines: {node: '>=6.9.0'}
+
+  /@babel/core@7.22.1:
+    resolution: {integrity: sha512-Hkqu7J4ynysSXxmAahpN1jjRwVJ+NdpraFLIWflgjpVob3KNyK3/tIUc7Q7szed8WMp0JNa7Qtd1E9Oo22F9gA==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@ampproject/remapping': 2.2.0
-      '@babel/code-frame': 7.18.6
-      '@babel/generator': 7.21.1
-      '@babel/helper-compilation-targets': 7.20.7(@babel/core@7.21.0)
-      '@babel/helper-module-transforms': 7.21.2
-      '@babel/helpers': 7.21.0
-      '@babel/parser': 7.21.2
-      '@babel/template': 7.20.7
-      '@babel/traverse': 7.21.2
-      '@babel/types': 7.21.2
+      '@babel/code-frame': 7.21.4
+      '@babel/generator': 7.22.3
+      '@babel/helper-compilation-targets': 7.22.1(@babel/core@7.22.1)
+      '@babel/helper-module-transforms': 7.22.1
+      '@babel/helpers': 7.22.3
+      '@babel/parser': 7.22.4
+      '@babel/template': 7.21.9
+      '@babel/traverse': 7.22.4
+      '@babel/types': 7.22.4
       convert-source-map: 1.9.0
       debug: 4.3.4
       gensync: 1.0.0-beta.2
       json5: 2.2.3
       semver: 6.3.0
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
   /@babel/generator@7.21.1:
     resolution: {integrity: sha512-1lT45bAYlQhFn/BHivJs43AiW2rg3/UbLyShGfF3C0KmHvO5fSghWd5kBJy30kpRRucGzXStvnnCFniCR2kXAA==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/types': 7.21.2
       '@jridgewell/gen-mapping': 0.3.2
       '@jridgewell/trace-mapping': 0.3.17
       jsesc: 2.5.2
-    dev: false
+
+  /@babel/generator@7.22.3:
+    resolution: {integrity: sha512-C17MW4wlk//ES/CJDL51kPNwl+qiBQyN7b9SKyVp11BLGFeSPoVaHrv+MNt8jwQFhQWowW88z1eeBx3pFz9v8A==}
+    engines: {node: '>=6.9.0'}
+    dependencies:
+      '@babel/types': 7.22.4
+      '@jridgewell/gen-mapping': 0.3.2
+      '@jridgewell/trace-mapping': 0.3.17
+      jsesc: 2.5.2
 
   /@babel/helper-annotate-as-pure@7.18.6:
     resolution: {integrity: sha512-duORpUiYrEpzKIop6iNbjnwKLAKnJ47csTyRACyEmWj0QdUrm5aqNJGHSSEQSUAvNW0ojX0dOmK9dZduvkfeXA==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/types': 7.21.2
-    dev: false
 
-  /@babel/helper-compilation-targets@7.20.7(@babel/core@7.21.0):
-    resolution: {integrity: sha512-4tGORmfQcrc+bvrjb5y3dG9Mx1IOZjsHqQVUz7XCNHO+iTmqxWnVg3KRygjGmpRLJGdQSKuvFinbIb0CnZwHAQ==}
+  /@babel/helper-compilation-targets@7.22.1(@babel/core@7.22.1):
+    resolution: {integrity: sha512-Rqx13UM3yVB5q0D/KwQ8+SPfX/+Rnsy1Lw1k/UwOC4KC6qrzIQoY3lYnBu5EHKBlEHHcj0M0W8ltPSkD8rqfsQ==}
     engines: {node: '>=6.9.0'}
     peerDependencies:
       '@babel/core': ^7.0.0
     dependencies:
-      '@babel/compat-data': 7.21.0
-      '@babel/core': 7.21.0
+      '@babel/compat-data': 7.22.3
+      '@babel/core': 7.22.1
       '@babel/helper-validator-option': 7.21.0
       browserslist: 4.21.5
       lru-cache: 5.1.1
       semver: 6.3.0
-    dev: false
 
   /@babel/helper-environment-visitor@7.18.9:
     resolution: {integrity: sha512-3r/aACDJ3fhQ/EVgFy0hpj8oHyHpQc+LPtJoY9SzTThAsStm4Ptegq92vqKoE3vD706ZVFWITnMnxucw+S9Ipg==}
     engines: {node: '>=6.9.0'}
-    dev: false
+
+  /@babel/helper-environment-visitor@7.22.1:
+    resolution: {integrity: sha512-Z2tgopurB/kTbidvzeBrc2To3PUP/9i5MUe+fU6QJCQDyPwSH2oRapkLw3KGECDYSjhQZCNxEvNvZlLw8JjGwA==}
+    engines: {node: '>=6.9.0'}
 
   /@babel/helper-function-name@7.21.0:
     resolution: {integrity: sha512-HfK1aMRanKHpxemaY2gqBmL04iAPOPRj7DxtNbiDOrJK+gdwkiNRVpCpUJYbUT+aZyemKN8brqTOxzCaG6ExRg==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/template': 7.20.7
       '@babel/types': 7.21.2
-    dev: false
 
   /@babel/helper-hoist-variables@7.18.6:
     resolution: {integrity: sha512-UlJQPkFqFULIcyW5sbzgbkxn2FKRgwWiRexcuaR8RNJRy8+LLveqPjwZV/bwrLZCN0eUHD/x8D0heK1ozuoo6Q==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/types': 7.21.2
-    dev: false
 
   /@babel/helper-module-imports@7.18.6:
     resolution: {integrity: sha512-0NFvs3VkuSYbFi1x2Vd6tKrywq+z/cLeYC/RJNFrIX/30Bf5aiGYbtvGXolEktzJH8o5E5KJ3tT+nkxuuZFVlA==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/types': 7.21.2
-    dev: false
 
-  /@babel/helper-module-transforms@7.21.2:
-    resolution: {integrity: sha512-79yj2AR4U/Oqq/WOV7Lx6hUjau1Zfo4cI+JLAVYeMV5XIlbOhmjEk5ulbTc9fMpmlojzZHkUUxAiK+UKn+hNQQ==}
+  /@babel/helper-module-imports@7.21.4:
+    resolution: {integrity: sha512-orajc5T2PsRYUN3ZryCEFeMDYwyw09c/pZeaQEZPH0MpKzSvn3e0uXsDBu3k03VI+9DBiRo+l22BfKTpKwa/Wg==}
     engines: {node: '>=6.9.0'}
     dependencies:
-      '@babel/helper-environment-visitor': 7.18.9
-      '@babel/helper-module-imports': 7.18.6
-      '@babel/helper-simple-access': 7.20.2
+      '@babel/types': 7.22.4
+
+  /@babel/helper-module-transforms@7.22.1:
+    resolution: {integrity: sha512-dxAe9E7ySDGbQdCVOY/4+UcD8M9ZFqZcZhSPsPacvCG4M+9lwtDDQfI2EoaSvmf7W/8yCBkGU0m7Pvt1ru3UZw==}
+    engines: {node: '>=6.9.0'}
+    dependencies:
+      '@babel/helper-environment-visitor': 7.22.1
+      '@babel/helper-module-imports': 7.21.4
+      '@babel/helper-simple-access': 7.21.5
       '@babel/helper-split-export-declaration': 7.18.6
       '@babel/helper-validator-identifier': 7.19.1
-      '@babel/template': 7.20.7
-      '@babel/traverse': 7.21.2
-      '@babel/types': 7.21.2
+      '@babel/template': 7.21.9
+      '@babel/traverse': 7.22.4
+      '@babel/types': 7.22.4
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
   /@babel/helper-plugin-utils@7.20.2:
     resolution: {integrity: sha512-8RvlJG2mj4huQ4pZ+rU9lqKi9ZKiRmuvGuM2HlWmkmgOhbs6zEAw6IEiJ5cQqGbDzGZOhwuOQNtZMi/ENLjZoQ==}
     engines: {node: '>=6.9.0'}
-    dev: false
 
-  /@babel/helper-simple-access@7.20.2:
-    resolution: {integrity: sha512-+0woI/WPq59IrqDYbVGfshjT5Dmk/nnbdpcF8SnMhhXObpTq2KNBdLFRFrkVdbDOyUmHBCxzm5FHV1rACIkIbA==}
+  /@babel/helper-simple-access@7.21.5:
+    resolution: {integrity: sha512-ENPDAMC1wAjR0uaCUwliBdiSl1KBJAVnMTzXqi64c2MG8MPR6ii4qf7bSXDqSFbr4W6W028/rf5ivoHop5/mkg==}
     engines: {node: '>=6.9.0'}
     dependencies:
-      '@babel/types': 7.21.2
-    dev: false
+      '@babel/types': 7.22.4
 
   /@babel/helper-split-export-declaration@7.18.6:
     resolution: {integrity: sha512-bde1etTx6ZyTmobl9LLMMQsaizFVZrquTEHOqKeQESMKo4PlObf+8+JA25ZsIpZhT/WEd39+vOdLXAFG/nELpA==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/types': 7.21.2
-    dev: false
 
   /@babel/helper-string-parser@7.19.4:
     resolution: {integrity: sha512-nHtDoQcuqFmwYNYPz3Rah5ph2p8PFeFCsZk9A/48dPc/rGocJ5J3hAAZ7pb76VWX3fZKu+uEr/FhH5jLx7umrw==}
     engines: {node: '>=6.9.0'}
-    dev: false
+
+  /@babel/helper-string-parser@7.21.5:
+    resolution: {integrity: sha512-5pTUx3hAJaZIdW99sJ6ZUUgWq/Y+Hja7TowEnLNMm1VivRgZQL3vpBY3qUACVsvw+yQU6+YgfBVmcbLaZtrA1w==}
+    engines: {node: '>=6.9.0'}
 
   /@babel/helper-validator-identifier@7.19.1:
     resolution: {integrity: sha512-awrNfaMtnHUr653GgGEs++LlAvW6w+DcPrOliSMXWCKo597CwL5Acf/wWdNkf/tfEQE3mjkeD1YOVZOUV/od1w==}
     engines: {node: '>=6.9.0'}
 
   /@babel/helper-validator-option@7.21.0:
     resolution: {integrity: sha512-rmL/B8/f0mKS2baE9ZpyTcTavvEuWhTTW8amjzXNvYG4AwBsqTLikfXsEofsJEfKHf+HQVQbFOHy6o+4cnC/fQ==}
     engines: {node: '>=6.9.0'}
-    dev: false
 
-  /@babel/helpers@7.21.0:
-    resolution: {integrity: sha512-XXve0CBtOW0pd7MRzzmoyuSj0e3SEzj8pgyFxnTT1NJZL38BD1MK7yYrm8yefRPIDvNNe14xR4FdbHwpInD4rA==}
+  /@babel/helpers@7.22.3:
+    resolution: {integrity: sha512-jBJ7jWblbgr7r6wYZHMdIqKc73ycaTcCaWRq4/2LpuPHcx7xMlZvpGQkOYc9HeSjn6rcx15CPlgVcBtZ4WZJ2w==}
     engines: {node: '>=6.9.0'}
     dependencies:
-      '@babel/template': 7.20.7
-      '@babel/traverse': 7.21.2
-      '@babel/types': 7.21.2
+      '@babel/template': 7.21.9
+      '@babel/traverse': 7.22.4
+      '@babel/types': 7.22.4
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
   /@babel/highlight@7.18.6:
     resolution: {integrity: sha512-u7stbOuYjaPezCuLj29hNW1v64M2Md2qupEKP1fHc7WdOA3DgLh37suiSrZYY7haUB7iBeQZ9P1uiRF359do3g==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/helper-validator-identifier': 7.19.1
       chalk: 2.4.2
@@ -554,39 +573,43 @@
 
   /@babel/parser@7.21.2:
     resolution: {integrity: sha512-URpaIJQwEkEC2T9Kn+Ai6Xe/02iNaVCuT/PtoRz3GPVJVDpPd7mLo+VddTbhCRU9TXqW5mSrQfXZyi8kDKOVpQ==}
     engines: {node: '>=6.0.0'}
     hasBin: true
     dependencies:
       '@babel/types': 7.21.2
-    dev: false
 
-  /@babel/plugin-syntax-jsx@7.18.6(@babel/core@7.21.0):
+  /@babel/parser@7.22.4:
+    resolution: {integrity: sha512-VLLsx06XkEYqBtE5YGPwfSGwfrjnyPP5oiGty3S8pQLFDFLaS8VwWSIxkTXpcvr5zeYLE6+MBNl2npl/YnfofA==}
+    engines: {node: '>=6.0.0'}
+    hasBin: true
+    dependencies:
+      '@babel/types': 7.22.4
+
+  /@babel/plugin-syntax-jsx@7.18.6(@babel/core@7.22.1):
     resolution: {integrity: sha512-6mmljtAedFGTWu2p/8WIORGwy+61PLgOMPOdazc7YoJ9ZCWUyFy3A6CpPkRKLKD1ToAesxX8KGEViAiLo9N+7Q==}
     engines: {node: '>=6.9.0'}
     peerDependencies:
       '@babel/core': ^7.0.0-0
     dependencies:
-      '@babel/core': 7.21.0
+      '@babel/core': 7.22.1
       '@babel/helper-plugin-utils': 7.20.2
-    dev: false
 
-  /@babel/plugin-transform-react-jsx@7.21.0(@babel/core@7.21.0):
+  /@babel/plugin-transform-react-jsx@7.21.0(@babel/core@7.22.1):
     resolution: {integrity: sha512-6OAWljMvQrZjR2DaNhVfRz6dkCAVV+ymcLUmaf8bccGOHn2v5rHJK3tTpij0BuhdYWP4LLaqj5lwcdlpAAPuvg==}
     engines: {node: '>=6.9.0'}
     peerDependencies:
       '@babel/core': ^7.0.0-0
     dependencies:
-      '@babel/core': 7.21.0
+      '@babel/core': 7.22.1
       '@babel/helper-annotate-as-pure': 7.18.6
       '@babel/helper-module-imports': 7.18.6
       '@babel/helper-plugin-utils': 7.20.2
-      '@babel/plugin-syntax-jsx': 7.18.6(@babel/core@7.21.0)
+      '@babel/plugin-syntax-jsx': 7.18.6(@babel/core@7.22.1)
       '@babel/types': 7.21.2
-    dev: false
 
   /@babel/runtime@7.21.0:
     resolution: {integrity: sha512-xwII0//EObnq89Ji5AKYQaRYiW/nZ3llSv29d49IuxPhKbtJoLP+9QUUZ4nVragQVtaVGeZrpB+ZtG/Pdy/POw==}
     engines: {node: '>=6.9.0'}
     dependencies:
       regenerator-runtime: 0.13.11
     dev: true
@@ -594,15 +617,22 @@
   /@babel/template@7.20.7:
     resolution: {integrity: sha512-8SegXApWe6VoNw0r9JHpSteLKTpTiLZ4rMlGIm9JQ18KiCtyQiAMEazujAHrUS5flrcqYZa75ukev3P6QmUwUw==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/code-frame': 7.18.6
       '@babel/parser': 7.21.2
       '@babel/types': 7.21.2
-    dev: false
+
+  /@babel/template@7.21.9:
+    resolution: {integrity: sha512-MK0X5k8NKOuWRamiEfc3KEJiHMTkGZNUjzMipqCGDDc6ijRl/B7RGSKVGncu4Ro/HdyzzY6cmoXuKI2Gffk7vQ==}
+    engines: {node: '>=6.9.0'}
+    dependencies:
+      '@babel/code-frame': 7.21.4
+      '@babel/parser': 7.22.4
+      '@babel/types': 7.22.4
 
   /@babel/traverse@7.21.2:
     resolution: {integrity: sha512-ts5FFU/dSUPS13tv8XiEObDu9K+iagEKME9kAbaP7r0Y9KtZJZ+NGndDvWoRAYNpeWafbpFeki3q9QoMD6gxyw==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/code-frame': 7.18.6
       '@babel/generator': 7.21.1
@@ -612,24 +642,47 @@
       '@babel/helper-split-export-declaration': 7.18.6
       '@babel/parser': 7.21.2
       '@babel/types': 7.21.2
       debug: 4.3.4
       globals: 11.12.0
     transitivePeerDependencies:
       - supports-color
-    dev: false
+
+  /@babel/traverse@7.22.4:
+    resolution: {integrity: sha512-Tn1pDsjIcI+JcLKq1AVlZEr4226gpuAQTsLMorsYg9tuS/kG7nuwwJ4AB8jfQuEgb/COBwR/DqJxmoiYFu5/rQ==}
+    engines: {node: '>=6.9.0'}
+    dependencies:
+      '@babel/code-frame': 7.21.4
+      '@babel/generator': 7.22.3
+      '@babel/helper-environment-visitor': 7.22.1
+      '@babel/helper-function-name': 7.21.0
+      '@babel/helper-hoist-variables': 7.18.6
+      '@babel/helper-split-export-declaration': 7.18.6
+      '@babel/parser': 7.22.4
+      '@babel/types': 7.22.4
+      debug: 4.3.4
+      globals: 11.12.0
+    transitivePeerDependencies:
+      - supports-color
 
   /@babel/types@7.21.2:
     resolution: {integrity: sha512-3wRZSs7jiFaB8AjxiiD+VqN5DTG2iRvJGQ+qYFrs/654lg6kGTQWIOFjlBo5RaXuAZjBmP3+OQH4dmhqiiyYxw==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/helper-string-parser': 7.19.4
       '@babel/helper-validator-identifier': 7.19.1
       to-fast-properties: 2.0.0
-    dev: false
+
+  /@babel/types@7.22.4:
+    resolution: {integrity: sha512-Tx9x3UBHTTsMSW85WB2kphxYQVvrZ/t1FxD88IpSgIjiUJlCm9z+xWIDwyo1vffTwSqteqyznB8ZE9vYYk16zA==}
+    engines: {node: '>=6.9.0'}
+    dependencies:
+      '@babel/helper-string-parser': 7.21.5
+      '@babel/helper-validator-identifier': 7.19.1
+      to-fast-properties: 2.0.0
 
   /@changesets/apply-release-plan@6.1.3:
     resolution: {integrity: sha512-ECDNeoc3nfeAe1jqJb5aFQX7CqzQhD2klXRez2JDb/aVpGUbX673HgKrnrgJRuQR/9f2TtLoYIzrGB9qwD77mg==}
     dependencies:
       '@babel/runtime': 7.21.0
       '@changesets/config': 2.3.0
       '@changesets/get-version-range-type': 0.3.2
@@ -825,15 +878,15 @@
     engines: {node: '>=10.0.0'}
     dev: true
 
   /@docsearch/css@3.3.3:
     resolution: {integrity: sha512-6SCwI7P8ao+se1TUsdZ7B4XzL+gqeQZnBc+2EONZlcVa0dVrk0NjETxozFKgMv0eEGH8QzP1fkN+A1rH61l4eg==}
     dev: false
 
-  /@docsearch/react@3.3.3(@algolia/client-search@4.15.0)(@types/react@17.0.53)(react-dom@18.2.0)(react@18.2.0):
+  /@docsearch/react@3.3.3(@algolia/client-search@4.15.0)(@types/react@18.2.8)(react-dom@18.2.0)(react@18.2.0):
     resolution: {integrity: sha512-pLa0cxnl+G0FuIDuYlW+EBK6Rw2jwLw9B1RHIeS4N4s2VhsfJ/wzeCi3CWcs5yVfxLd5ZK50t//TMA5e79YT7Q==}
     peerDependencies:
       '@types/react': '>= 16.8.0 < 19.0.0'
       react: '>= 16.8.0 < 19.0.0'
       react-dom: '>= 16.8.0 < 19.0.0'
     peerDependenciesMeta:
       '@types/react':
@@ -842,423 +895,617 @@
         optional: true
       react-dom:
         optional: true
     dependencies:
       '@algolia/autocomplete-core': 1.7.4
       '@algolia/autocomplete-preset-algolia': 1.7.4(@algolia/client-search@4.15.0)(algoliasearch@4.15.0)
       '@docsearch/css': 3.3.3
-      '@types/react': 17.0.53
+      '@types/react': 18.2.8
       algoliasearch: 4.15.0
       react: 18.2.0
       react-dom: 18.2.0(react@18.2.0)
     transitivePeerDependencies:
       - '@algolia/client-search'
     dev: false
 
   /@emmetio/abbreviation@2.2.3:
     resolution: {integrity: sha512-87pltuCPt99aL+y9xS6GPZ+Wmmyhll2WXH73gG/xpGcQ84DRnptBsI2r0BeIQ0EB/SQTOe2ANPqFqj3Rj5FOGA==}
     dependencies:
       '@emmetio/scanner': 1.0.0
-    dev: false
 
   /@emmetio/css-abbreviation@2.1.4:
     resolution: {integrity: sha512-qk9L60Y+uRtM5CPbB0y+QNl/1XKE09mSO+AhhSauIfr2YOx/ta3NJw2d8RtCFxgzHeRqFRr8jgyzThbu+MZ4Uw==}
     dependencies:
       '@emmetio/scanner': 1.0.0
-    dev: false
 
   /@emmetio/scanner@1.0.0:
     resolution: {integrity: sha512-8HqW8EVqjnCmWXVpqAOZf+EGESdkR27odcMMMGefgKXtar00SoYNSryGv//TELI4T3QFsECo78p+0lmalk/CFA==}
-    dev: false
 
   /@esbuild/android-arm64@0.16.17:
     resolution: {integrity: sha512-MIGl6p5sc3RDTLLkYL1MyL8BMRN4tLMRCn+yRJJmEDvYZ2M7tmAf80hx1kbNEUX2KJ50RRtxZ4JHLvCfuB6kBg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/android-arm64@0.17.12:
     resolution: {integrity: sha512-WQ9p5oiXXYJ33F2EkE3r0FRDFVpEdcDiwNX3u7Xaibxfx6vQE0Sb8ytrfQsA5WO6kDn6mDfKLh6KrPBjvkk7xA==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/android-arm64@0.17.19:
+    resolution: {integrity: sha512-KBMWvEZooR7+kzY0BtbTQn0OAYY7CsiydT63pVEaPtVYF0hXbUaOyZog37DKxK7NF3XacBJOpYT4adIJh+avxA==}
+    engines: {node: '>=12'}
+    cpu: [arm64]
+    os: [android]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/android-arm@0.16.17:
     resolution: {integrity: sha512-N9x1CMXVhtWEAMS7pNNONyA14f71VPQN9Cnavj1XQh6T7bskqiLLrSca4O0Vr8Wdcga943eThxnVp3JLnBMYtw==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [android]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/android-arm@0.17.12:
     resolution: {integrity: sha512-E/sgkvwoIfj4aMAPL2e35VnUJspzVYl7+M1B2cqeubdBhADV4uPon0KCc8p2G+LqSJ6i8ocYPCqY3A4GGq0zkQ==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/android-arm@0.17.19:
+    resolution: {integrity: sha512-rIKddzqhmav7MSmoFCmDIb6e2W57geRsM94gV2l38fzhXMwq7hZoClug9USI2pFRGL06f4IOPHHpFNOkWieR8A==}
+    engines: {node: '>=12'}
+    cpu: [arm]
+    os: [android]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/android-x64@0.16.17:
     resolution: {integrity: sha512-a3kTv3m0Ghh4z1DaFEuEDfz3OLONKuFvI4Xqczqx4BqLyuFaFkuaG4j2MtA6fuWEFeC5x9IvqnX7drmRq/fyAQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [android]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/android-x64@0.17.12:
     resolution: {integrity: sha512-m4OsaCr5gT+se25rFPHKQXARMyAehHTQAz4XX1Vk3d27VtqiX0ALMBPoXZsGaB6JYryCLfgGwUslMqTfqeLU0w==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/android-x64@0.17.19:
+    resolution: {integrity: sha512-uUTTc4xGNDT7YSArp/zbtmbhO0uEEK9/ETW29Wk1thYUJBz3IVnvgEiEwEa9IeLyvnpKrWK64Utw2bgUmDveww==}
+    engines: {node: '>=12'}
+    cpu: [x64]
+    os: [android]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/darwin-arm64@0.16.17:
     resolution: {integrity: sha512-/2agbUEfmxWHi9ARTX6OQ/KgXnOWfsNlTeLcoV7HSuSTv63E4DqtAc+2XqGw1KHxKMHGZgbVCZge7HXWX9Vn+w==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/darwin-arm64@0.17.12:
     resolution: {integrity: sha512-O3GCZghRIx+RAN0NDPhyyhRgwa19MoKlzGonIb5hgTj78krqp9XZbYCvFr9N1eUxg0ZQEpiiZ4QvsOQwBpP+lg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/darwin-arm64@0.17.19:
+    resolution: {integrity: sha512-80wEoCfF/hFKM6WE1FyBHc9SfUblloAWx6FJkFWTWiCoht9Mc0ARGEM47e67W9rI09YoUxJL68WHfDRYEAvOhg==}
+    engines: {node: '>=12'}
+    cpu: [arm64]
+    os: [darwin]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/darwin-x64@0.16.17:
     resolution: {integrity: sha512-2By45OBHulkd9Svy5IOCZt376Aa2oOkiE9QWUK9fe6Tb+WDr8hXL3dpqi+DeLiMed8tVXspzsTAvd0jUl96wmg==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/darwin-x64@0.17.12:
     resolution: {integrity: sha512-5D48jM3tW27h1qjaD9UNRuN+4v0zvksqZSPZqeSWggfMlsVdAhH3pwSfQIFJwcs9QJ9BRibPS4ViZgs3d2wsCA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/darwin-x64@0.17.19:
+    resolution: {integrity: sha512-IJM4JJsLhRYr9xdtLytPLSH9k/oxR3boaUIYiHkAawtwNOXKE8KoU8tMvryogdcT8AU+Bflmh81Xn6Q0vTZbQw==}
+    engines: {node: '>=12'}
+    cpu: [x64]
+    os: [darwin]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/freebsd-arm64@0.16.17:
     resolution: {integrity: sha512-mt+cxZe1tVx489VTb4mBAOo2aKSnJ33L9fr25JXpqQqzbUIw/yzIzi+NHwAXK2qYV1lEFp4OoVeThGjUbmWmdw==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [freebsd]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/freebsd-arm64@0.17.12:
     resolution: {integrity: sha512-OWvHzmLNTdF1erSvrfoEBGlN94IE6vCEaGEkEH29uo/VoONqPnoDFfShi41Ew+yKimx4vrmmAJEGNoyyP+OgOQ==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/freebsd-arm64@0.17.19:
+    resolution: {integrity: sha512-pBwbc7DufluUeGdjSU5Si+P3SoMF5DQ/F/UmTSb8HXO80ZEAJmrykPyzo1IfNbAoaqw48YRpv8shwd1NoI0jcQ==}
+    engines: {node: '>=12'}
+    cpu: [arm64]
+    os: [freebsd]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/freebsd-x64@0.16.17:
     resolution: {integrity: sha512-8ScTdNJl5idAKjH8zGAsN7RuWcyHG3BAvMNpKOBaqqR7EbUhhVHOqXRdL7oZvz8WNHL2pr5+eIT5c65kA6NHug==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [freebsd]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/freebsd-x64@0.17.12:
     resolution: {integrity: sha512-A0Xg5CZv8MU9xh4a+7NUpi5VHBKh1RaGJKqjxe4KG87X+mTjDE6ZvlJqpWoeJxgfXHT7IMP9tDFu7IZ03OtJAw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/freebsd-x64@0.17.19:
+    resolution: {integrity: sha512-4lu+n8Wk0XlajEhbEffdy2xy53dpR06SlzvhGByyg36qJw6Kpfk7cp45DR/62aPH9mtJRmIyrXAS5UWBrJT6TQ==}
+    engines: {node: '>=12'}
+    cpu: [x64]
+    os: [freebsd]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/linux-arm64@0.16.17:
     resolution: {integrity: sha512-7S8gJnSlqKGVJunnMCrXHU9Q8Q/tQIxk/xL8BqAP64wchPCTzuM6W3Ra8cIa1HIflAvDnNOt2jaL17vaW+1V0g==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/linux-arm64@0.17.12:
     resolution: {integrity: sha512-cK3AjkEc+8v8YG02hYLQIQlOznW+v9N+OI9BAFuyqkfQFR+DnDLhEM5N8QRxAUz99cJTo1rLNXqRrvY15gbQUg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/linux-arm64@0.17.19:
+    resolution: {integrity: sha512-ct1Tg3WGwd3P+oZYqic+YZF4snNl2bsnMKRkb3ozHmnM0dGWuxcPTTntAF6bOP0Sp4x0PjSF+4uHQ1xvxfRKqg==}
+    engines: {node: '>=12'}
+    cpu: [arm64]
+    os: [linux]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/linux-arm@0.16.17:
     resolution: {integrity: sha512-iihzrWbD4gIT7j3caMzKb/RsFFHCwqqbrbH9SqUSRrdXkXaygSZCZg1FybsZz57Ju7N/SHEgPyaR0LZ8Zbe9gQ==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/linux-arm@0.17.12:
     resolution: {integrity: sha512-WsHyJ7b7vzHdJ1fv67Yf++2dz3D726oO3QCu8iNYik4fb5YuuReOI9OtA+n7Mk0xyQivNTPbl181s+5oZ38gyA==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/linux-arm@0.17.19:
+    resolution: {integrity: sha512-cdmT3KxjlOQ/gZ2cjfrQOtmhG4HJs6hhvm3mWSRDPtZ/lP5oe8FWceS10JaSJC13GBd4eH/haHnqf7hhGNLerA==}
+    engines: {node: '>=12'}
+    cpu: [arm]
+    os: [linux]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/linux-ia32@0.16.17:
     resolution: {integrity: sha512-kiX69+wcPAdgl3Lonh1VI7MBr16nktEvOfViszBSxygRQqSpzv7BffMKRPMFwzeJGPxcio0pdD3kYQGpqQ2SSg==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [linux]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/linux-ia32@0.17.12:
     resolution: {integrity: sha512-jdOBXJqcgHlah/nYHnj3Hrnl9l63RjtQ4vn9+bohjQPI2QafASB5MtHAoEv0JQHVb/xYQTFOeuHnNYE1zF7tYw==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/linux-ia32@0.17.19:
+    resolution: {integrity: sha512-w4IRhSy1VbsNxHRQpeGCHEmibqdTUx61Vc38APcsRbuVgK0OPEnQ0YD39Brymn96mOx48Y2laBQGqgZ0j9w6SQ==}
+    engines: {node: '>=12'}
+    cpu: [ia32]
+    os: [linux]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/linux-loong64@0.16.17:
     resolution: {integrity: sha512-dTzNnQwembNDhd654cA4QhbS9uDdXC3TKqMJjgOWsC0yNCbpzfWoXdZvp0mY7HU6nzk5E0zpRGGx3qoQg8T2DQ==}
     engines: {node: '>=12'}
     cpu: [loong64]
     os: [linux]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/linux-loong64@0.17.12:
     resolution: {integrity: sha512-GTOEtj8h9qPKXCyiBBnHconSCV9LwFyx/gv3Phw0pa25qPYjVuuGZ4Dk14bGCfGX3qKF0+ceeQvwmtI+aYBbVA==}
     engines: {node: '>=12'}
     cpu: [loong64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/linux-loong64@0.17.19:
+    resolution: {integrity: sha512-2iAngUbBPMq439a+z//gE+9WBldoMp1s5GWsUSgqHLzLJ9WoZLZhpwWuym0u0u/4XmZ3gpHmzV84PonE+9IIdQ==}
+    engines: {node: '>=12'}
+    cpu: [loong64]
+    os: [linux]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/linux-mips64el@0.16.17:
     resolution: {integrity: sha512-ezbDkp2nDl0PfIUn0CsQ30kxfcLTlcx4Foz2kYv8qdC6ia2oX5Q3E/8m6lq84Dj/6b0FrkgD582fJMIfHhJfSw==}
     engines: {node: '>=12'}
     cpu: [mips64el]
     os: [linux]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/linux-mips64el@0.17.12:
     resolution: {integrity: sha512-o8CIhfBwKcxmEENOH9RwmUejs5jFiNoDw7YgS0EJTF6kgPgcqLFjgoc5kDey5cMHRVCIWc6kK2ShUePOcc7RbA==}
     engines: {node: '>=12'}
     cpu: [mips64el]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/linux-mips64el@0.17.19:
+    resolution: {integrity: sha512-LKJltc4LVdMKHsrFe4MGNPp0hqDFA1Wpt3jE1gEyM3nKUvOiO//9PheZZHfYRfYl6AwdTH4aTcXSqBerX0ml4A==}
+    engines: {node: '>=12'}
+    cpu: [mips64el]
+    os: [linux]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/linux-ppc64@0.16.17:
     resolution: {integrity: sha512-dzS678gYD1lJsW73zrFhDApLVdM3cUF2MvAa1D8K8KtcSKdLBPP4zZSLy6LFZ0jYqQdQ29bjAHJDgz0rVbLB3g==}
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [linux]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/linux-ppc64@0.17.12:
     resolution: {integrity: sha512-biMLH6NR/GR4z+ap0oJYb877LdBpGac8KfZoEnDiBKd7MD/xt8eaw1SFfYRUeMVx519kVkAOL2GExdFmYnZx3A==}
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/linux-ppc64@0.17.19:
+    resolution: {integrity: sha512-/c/DGybs95WXNS8y3Ti/ytqETiW7EU44MEKuCAcpPto3YjQbyK3IQVKfF6nbghD7EcLUGl0NbiL5Rt5DMhn5tg==}
+    engines: {node: '>=12'}
+    cpu: [ppc64]
+    os: [linux]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/linux-riscv64@0.16.17:
     resolution: {integrity: sha512-ylNlVsxuFjZK8DQtNUwiMskh6nT0vI7kYl/4fZgV1llP5d6+HIeL/vmmm3jpuoo8+NuXjQVZxmKuhDApK0/cKw==}
     engines: {node: '>=12'}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/linux-riscv64@0.17.12:
     resolution: {integrity: sha512-jkphYUiO38wZGeWlfIBMB72auOllNA2sLfiZPGDtOBb1ELN8lmqBrlMiucgL8awBw1zBXN69PmZM6g4yTX84TA==}
     engines: {node: '>=12'}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/linux-riscv64@0.17.19:
+    resolution: {integrity: sha512-FC3nUAWhvFoutlhAkgHf8f5HwFWUL6bYdvLc/TTuxKlvLi3+pPzdZiFKSWz/PF30TB1K19SuCxDTI5KcqASJqA==}
+    engines: {node: '>=12'}
+    cpu: [riscv64]
+    os: [linux]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/linux-s390x@0.16.17:
     resolution: {integrity: sha512-gzy7nUTO4UA4oZ2wAMXPNBGTzZFP7mss3aKR2hH+/4UUkCOyqmjXiKpzGrY2TlEUhbbejzXVKKGazYcQTZWA/w==}
     engines: {node: '>=12'}
     cpu: [s390x]
     os: [linux]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/linux-s390x@0.17.12:
     resolution: {integrity: sha512-j3ucLdeY9HBcvODhCY4b+Ds3hWGO8t+SAidtmWu/ukfLLG/oYDMaA+dnugTVAg5fnUOGNbIYL9TOjhWgQB8W5g==}
     engines: {node: '>=12'}
     cpu: [s390x]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/linux-s390x@0.17.19:
+    resolution: {integrity: sha512-IbFsFbxMWLuKEbH+7sTkKzL6NJmG2vRyy6K7JJo55w+8xDk7RElYn6xvXtDW8HCfoKBFK69f3pgBJSUSQPr+4Q==}
+    engines: {node: '>=12'}
+    cpu: [s390x]
+    os: [linux]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/linux-x64@0.16.17:
     resolution: {integrity: sha512-mdPjPxfnmoqhgpiEArqi4egmBAMYvaObgn4poorpUaqmvzzbvqbowRllQ+ZgzGVMGKaPkqUmPDOOFQRUFDmeUw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/linux-x64@0.17.12:
     resolution: {integrity: sha512-uo5JL3cgaEGotaqSaJdRfFNSCUJOIliKLnDGWaVCgIKkHxwhYMm95pfMbWZ9l7GeW9kDg0tSxcy9NYdEtjwwmA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/linux-x64@0.17.19:
+    resolution: {integrity: sha512-68ngA9lg2H6zkZcyp22tsVt38mlhWde8l3eJLWkyLrp4HwMUr3c1s/M2t7+kHIhvMjglIBrFpncX1SzMckomGw==}
+    engines: {node: '>=12'}
+    cpu: [x64]
+    os: [linux]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/netbsd-x64@0.16.17:
     resolution: {integrity: sha512-/PzmzD/zyAeTUsduZa32bn0ORug+Jd1EGGAUJvqfeixoEISYpGnAezN6lnJoskauoai0Jrs+XSyvDhppCPoKOA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [netbsd]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/netbsd-x64@0.17.12:
     resolution: {integrity: sha512-DNdoRg8JX+gGsbqt2gPgkgb00mqOgOO27KnrWZtdABl6yWTST30aibGJ6geBq3WM2TIeW6COs5AScnC7GwtGPg==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [netbsd]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/netbsd-x64@0.17.19:
+    resolution: {integrity: sha512-CwFq42rXCR8TYIjIfpXCbRX0rp1jo6cPIUPSaWwzbVI4aOfX96OXY8M6KNmtPcg7QjYeDmN+DD0Wp3LaBOLf4Q==}
+    engines: {node: '>=12'}
+    cpu: [x64]
+    os: [netbsd]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/openbsd-x64@0.16.17:
     resolution: {integrity: sha512-2yaWJhvxGEz2RiftSk0UObqJa/b+rIAjnODJgv2GbGGpRwAfpgzyrg1WLK8rqA24mfZa9GvpjLcBBg8JHkoodg==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [openbsd]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/openbsd-x64@0.17.12:
     resolution: {integrity: sha512-aVsENlr7B64w8I1lhHShND5o8cW6sB9n9MUtLumFlPhG3elhNWtE7M1TFpj3m7lT3sKQUMkGFjTQBrvDDO1YWA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [openbsd]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/openbsd-x64@0.17.19:
+    resolution: {integrity: sha512-cnq5brJYrSZ2CF6c35eCmviIN3k3RczmHz8eYaVlNasVqsNY+JKohZU5MKmaOI+KkllCdzOKKdPs762VCPC20g==}
+    engines: {node: '>=12'}
+    cpu: [x64]
+    os: [openbsd]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/sunos-x64@0.16.17:
     resolution: {integrity: sha512-xtVUiev38tN0R3g8VhRfN7Zl42YCJvyBhRKw1RJjwE1d2emWTVToPLNEQj/5Qxc6lVFATDiy6LjVHYhIPrLxzw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [sunos]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/sunos-x64@0.17.12:
     resolution: {integrity: sha512-qbHGVQdKSwi0JQJuZznS4SyY27tYXYF0mrgthbxXrZI3AHKuRvU+Eqbg/F0rmLDpW/jkIZBlCO1XfHUBMNJ1pg==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [sunos]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/sunos-x64@0.17.19:
+    resolution: {integrity: sha512-vCRT7yP3zX+bKWFeP/zdS6SqdWB8OIpaRq/mbXQxTGHnIxspRtigpkUcDMlSCOejlHowLqII7K2JKevwyRP2rg==}
+    engines: {node: '>=12'}
+    cpu: [x64]
+    os: [sunos]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/win32-arm64@0.16.17:
     resolution: {integrity: sha512-ga8+JqBDHY4b6fQAmOgtJJue36scANy4l/rL97W+0wYmijhxKetzZdKOJI7olaBaMhWt8Pac2McJdZLxXWUEQw==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/win32-arm64@0.17.12:
     resolution: {integrity: sha512-zsCp8Ql+96xXTVTmm6ffvoTSZSV2B/LzzkUXAY33F/76EajNw1m+jZ9zPfNJlJ3Rh4EzOszNDHsmG/fZOhtqDg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/win32-arm64@0.17.19:
+    resolution: {integrity: sha512-yYx+8jwowUstVdorcMdNlzklLYhPxjniHWFKgRqH7IFlUEa0Umu3KuYplf1HUZZ422e3NU9F4LGb+4O0Kdcaag==}
+    engines: {node: '>=12'}
+    cpu: [arm64]
+    os: [win32]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/win32-ia32@0.16.17:
     resolution: {integrity: sha512-WnsKaf46uSSF/sZhwnqE4L/F89AYNMiD4YtEcYekBt9Q7nj0DiId2XH2Ng2PHM54qi5oPrQ8luuzGszqi/veig==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/win32-ia32@0.17.12:
     resolution: {integrity: sha512-FfrFjR4id7wcFYOdqbDfDET3tjxCozUgbqdkOABsSFzoZGFC92UK7mg4JKRc/B3NNEf1s2WHxJ7VfTdVDPN3ng==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/win32-ia32@0.17.19:
+    resolution: {integrity: sha512-eggDKanJszUtCdlVs0RB+h35wNlb5v4TWEkq4vZcmVt5u/HiDZrTXe2bWFQUez3RgNHwx/x4sk5++4NSSicKkw==}
+    engines: {node: '>=12'}
+    cpu: [ia32]
+    os: [win32]
+    requiresBuild: true
+    optional: true
+
   /@esbuild/win32-x64@0.16.17:
     resolution: {integrity: sha512-y+EHuSchhL7FjHgvQL/0fnnFmO4T1bhvWANX6gcnqTjtnKWbTvUMCpGnv2+t+31d7RzyEAYAd4u2fnIhHL6N/Q==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
+    dev: true
     optional: true
 
   /@esbuild/win32-x64@0.17.12:
     resolution: {integrity: sha512-JOOxw49BVZx2/5tW3FqkdjSD/5gXYeVGPDcB0lvap0gLQshkh1Nyel1QazC+wNxus3xPlsYAgqU1BUmrmCvWtw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@esbuild/win32-x64@0.17.19:
+    resolution: {integrity: sha512-lAhycmKnVOuRYNtRtatQR1LPQf2oYCkRGkSFnseDAKPl8lu5SOsK/e1sXe5a0Pc5kHIHe6P2I/ilntNv2xf3cA==}
+    engines: {node: '>=12'}
+    cpu: [x64]
+    os: [win32]
+    requiresBuild: true
+    optional: true
+
   /@gar/promisify@1.1.3:
     resolution: {integrity: sha512-k2Ty1JcVojjJFwrg/ThKi2ujJ7XNLYaFGNB/bWT9wGR+oSMJHMa5w+CUq6p/pVrKeNNgA7pCqEcjSnHVoqJQFw==}
     dev: true
 
   /@jridgewell/gen-mapping@0.1.1:
     resolution: {integrity: sha512-sQXCasFk+U8lWYEe66WxRDOE9PjVz4vSM51fTu3Hw+ClTpUSQb718772vH3pyS5pShp6lvQM7SxgIDXXXmOX7w==}
     engines: {node: '>=6.0.0'}
     dependencies:
       '@jridgewell/set-array': 1.1.2
       '@jridgewell/sourcemap-codec': 1.4.14
-    dev: false
 
   /@jridgewell/gen-mapping@0.3.2:
     resolution: {integrity: sha512-mh65xKQAzI6iBcFzwv28KVWSmCkdRBWoOh+bYQGW3+6OZvbbN3TqMGo5hqYxQniRcH9F2VZIoJCm4pa3BPDK/A==}
     engines: {node: '>=6.0.0'}
     dependencies:
       '@jridgewell/set-array': 1.1.2
       '@jridgewell/sourcemap-codec': 1.4.14
@@ -1438,15 +1685,14 @@
       '@lumino/signaling': 1.11.1
     transitivePeerDependencies:
       - crypto
     dev: false
 
   /@ljharb/has-package-exports-patterns@0.0.2:
     resolution: {integrity: sha512-4/RWEeXDO6bocPONheFe6gX/oQdP/bEpv0oL4HqjPP5DCenBSt0mHgahppY49N0CpsaqffdwPq+TlX9CYOq2Dw==}
-    dev: false
 
   /@lumino/algorithm@1.9.2:
     resolution: {integrity: sha512-Z06lp/yuhz8CtIir3PNTGnuk7909eXt4ukJsCzChsGuot2l5Fbs96RJ/FOHgwCedaX74CtxPjXHXoszFbUA+4A==}
 
   /@lumino/application@1.31.3(crypto@1.0.1):
     resolution: {integrity: sha512-XnsXm5PD9QevJRl/pHJziYmhRKqJYjEOTL6Vh9dtKpPPML57uswOj59Pokxx/yCvym1xRF9iDVvujy3KallRwQ==}
     dependencies:
@@ -1589,28 +1835,14 @@
       unist-util-stringify-position: 3.0.3
       unist-util-visit: 4.1.2
       vfile: 5.3.7
     transitivePeerDependencies:
       - supports-color
     dev: false
 
-  /@mdx-js/rollup@2.3.0(rollup@3.18.0):
-    resolution: {integrity: sha512-wLvRfJS/M4UmdqTd+WoaySEE7q4BIejYf1xAHXYvtT1du/1Tl/z2450Gg2+Hu7fh05KwRRiehiTP9Yc/Dtn0fA==}
-    peerDependencies:
-      rollup: '>=2'
-    dependencies:
-      '@mdx-js/mdx': 2.3.0
-      '@rollup/pluginutils': 5.0.2(rollup@3.18.0)
-      rollup: 3.18.0
-      source-map: 0.7.4
-      vfile: 5.3.7
-    transitivePeerDependencies:
-      - supports-color
-    dev: false
-
   /@nodelib/fs.scandir@2.1.5:
     resolution: {integrity: sha512-vq24Bq3ym5HEQm2NKCr3yXDwjc7vTsEThRDnkp2DK9p1uqLR+DHurm/NOTo0KG7HYHU7eppKZj3MyqYuMBf62g==}
     engines: {node: '>= 8'}
     dependencies:
       '@nodelib/fs.stat': 2.0.5
       run-parallel: 1.2.0
 
@@ -1668,29 +1900,14 @@
   /@proload/core@0.3.3:
     resolution: {integrity: sha512-7dAFWsIK84C90AMl24+N/ProHKm4iw0akcnoKjRvbfHifJZBLhaDsDus1QJmhG12lXj4e/uB/8mB/0aduCW+NQ==}
     dependencies:
       deepmerge: 4.3.0
       escalade: 3.1.1
     dev: false
 
-  /@rollup/pluginutils@5.0.2(rollup@3.18.0):
-    resolution: {integrity: sha512-pTd9rIsP92h+B6wWwFbW8RkZv4hiR/xKsqre4SIuAOaOEQRxi0lqLke9k2/7WegC85GgUs9pjmOjCUi3In4vwA==}
-    engines: {node: '>=14.0.0'}
-    peerDependencies:
-      rollup: ^1.20.0||^2.0.0||^3.0.0
-    peerDependenciesMeta:
-      rollup:
-        optional: true
-    dependencies:
-      '@types/estree': 1.0.0
-      estree-walker: 2.0.2
-      picomatch: 2.3.1
-      rollup: 3.18.0
-    dev: false
-
   /@svitejs/changesets-changelog-github-compact@1.1.0:
     resolution: {integrity: sha512-qhUGGDHcpbY2zpjW3SwqchuW8J/5EzlPFud7xNntHKA7f3a/mx5+g+ruJKFHSAiVZYo30PALt+AyhmPUNKH/Og==}
     engines: {node: ^14.13.1 || ^16.0.0 || >=18}
     dependencies:
       '@changesets/get-github-info': 0.5.2
       dotenv: 16.0.3
     transitivePeerDependencies:
@@ -1703,51 +1920,46 @@
       '@types/estree': 1.0.0
     dev: false
 
   /@types/babel__core@7.20.0:
     resolution: {integrity: sha512-+n8dL/9GWblDO0iU6eZAwEIJVr5DWigtle+Q6HLOrh/pdbXOhOtqzq8VPPE2zvNJzSKY4vH/z3iT3tn0A3ypiQ==}
     dependencies:
       '@babel/parser': 7.21.2
-      '@babel/types': 7.21.2
+      '@babel/types': 7.22.4
       '@types/babel__generator': 7.6.4
       '@types/babel__template': 7.4.1
       '@types/babel__traverse': 7.18.3
-    dev: false
 
   /@types/babel__generator@7.6.4:
     resolution: {integrity: sha512-tFkciB9j2K755yrTALxD44McOrk+gfpIpvC3sxHjRawj6PfnQxrse4Clq5y/Rq+G3mrBurMax/lG8Qn2t9mSsg==}
     dependencies:
-      '@babel/types': 7.21.2
-    dev: false
+      '@babel/types': 7.22.4
 
   /@types/babel__template@7.4.1:
     resolution: {integrity: sha512-azBFKemX6kMg5Io+/rdGT0dkGreboUVR0Cdm3fz9QJWpaQGJRQXl7C+6hOTCZcMll7KFyEQpgbYI2lHdsS4U7g==}
     dependencies:
-      '@babel/parser': 7.21.2
-      '@babel/types': 7.21.2
-    dev: false
+      '@babel/parser': 7.22.4
+      '@babel/types': 7.22.4
 
   /@types/babel__traverse@7.18.3:
     resolution: {integrity: sha512-1kbcJ40lLB7MHsj39U4Sh1uTd2E7rLEa79kmDpI6cy+XiXsteB3POdQomoq4FxszMrO3ZYchkhYJw7A2862b3w==}
     dependencies:
-      '@babel/types': 7.21.2
-    dev: false
+      '@babel/types': 7.22.4
 
   /@types/backbone@1.4.14:
     resolution: {integrity: sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==}
     dependencies:
       '@types/jquery': 3.5.16
       '@types/underscore': 1.11.4
     dev: false
 
   /@types/debug@4.1.7:
     resolution: {integrity: sha512-9AonUzyTjXXhEOa0DnqpzZi6VHlqKMswga9EXjpXnnqxwLtdvPPtlO8evrI5D9S6asFRCQ6v+wpiUKbw+vKqyg==}
     dependencies:
       '@types/ms': 0.7.31
-    dev: false
 
   /@types/eslint-scope@3.7.4:
     resolution: {integrity: sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==}
     dependencies:
       '@types/eslint': 8.21.1
       '@types/estree': 1.0.0
     dev: true
@@ -1772,14 +1984,17 @@
   /@types/estree@1.0.0:
     resolution: {integrity: sha512-WulqXMDUTYAXCjZnk6JtIHPigp55cVtDgDrO2gHRwhyJto21+1zbVCtOYB2L1F9w4qCQ0rOGWBnBe0FNTiEJIQ==}
 
   /@types/hast@2.3.4:
     resolution: {integrity: sha512-wLEm0QvaoawEDoTRwzTXp4b4jpwiJDvR5KMnFnVodm3scufTlBOWRD6N1OBf9TZMhjlNsSfcO5V+7AF4+Vy+9g==}
     dependencies:
       '@types/unist': 2.0.6
+
+  /@types/html-escaper@3.0.0:
+    resolution: {integrity: sha512-OcJcvP3Yk8mjYwf/IdXZtTE1tb/u0WF0qa29ER07ZHCYUBZXSN29Z1mBS+/96+kNMGTFUAbSz9X+pHmHpZrTCw==}
     dev: false
 
   /@types/is-ci@3.0.0:
     resolution: {integrity: sha512-Q0Op0hdWbYd1iahB+IFNQcWXFq4O0Q5MwQP7uN0souuQ4rPg1vEYcnIOfr1gY+M+6rc8FGoRaBO1mOOvL29sEQ==}
     dependencies:
       ci-info: 3.8.0
     dev: true
@@ -1792,80 +2007,82 @@
 
   /@types/json-schema@7.0.11:
     resolution: {integrity: sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==}
     dev: true
 
   /@types/json5@0.0.30:
     resolution: {integrity: sha512-sqm9g7mHlPY/43fcSNrCYfOeX9zkTTK+euO5E6+CVijSMm5tTjkVdwdqRkY3ljjIAf8679vps5jKUoJBCLsMDA==}
-    dev: false
 
   /@types/lodash@4.14.191:
     resolution: {integrity: sha512-BdZ5BCCvho3EIXw6wUCXHe7rS53AIDPLE+JzwgT+OsJk53oBfbSmZZ7CX4VaRoN78N+TJpFi9QPlfIVNmJYWxQ==}
     dev: false
 
   /@types/mdast@3.0.10:
     resolution: {integrity: sha512-W864tg/Osz1+9f4lrGTZpCSO5/z4608eUp19tbozkq2HJK6i3z1kT0H9tlADXuYIb1YYOBByU4Jsqkk75q48qA==}
     dependencies:
       '@types/unist': 2.0.6
-    dev: false
 
   /@types/mdx@2.0.3:
     resolution: {integrity: sha512-IgHxcT3RC8LzFLhKwP3gbMPeaK7BM9eBH46OdapPA7yvuIUJ8H6zHZV53J8hGZcTSnt95jANt+rTBNUUc22ACQ==}
     dev: false
 
   /@types/minimist@1.2.2:
     resolution: {integrity: sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==}
     dev: true
 
   /@types/ms@0.7.31:
     resolution: {integrity: sha512-iiUgKzV9AuaEkZqkOLDIvlQiL6ltuZd9tGcW3gwpnX8JbuiuhFlEGmmFXEXkN50Cvq7Os88IY2v0dkDqXYWVgA==}
-    dev: false
 
   /@types/nlcst@1.0.0:
     resolution: {integrity: sha512-3TGCfOcy8R8mMQ4CNSNOe3PG66HttvjcLzCoOpvXvDtfWOTi+uT/rxeOKm/qEwbM4SNe1O/PjdiBK2YcTjU4OQ==}
     dependencies:
       '@types/unist': 2.0.6
-    dev: false
 
   /@types/node@12.20.55:
     resolution: {integrity: sha512-J8xLz7q2OFulZ2cyGTLE1TbbZcjpno7FaN6zdJNrgAdrJ+DZzh/uFR6YrTb4C+nXakvud8Q4+rbhoIWlYQbUFQ==}
     dev: true
 
   /@types/node@18.14.6:
     resolution: {integrity: sha512-93+VvleD3mXwlLI/xASjw0FzKcwzl3OdTCzm1LaRfqgS21gfFtK3zDXM5Op9TeeMsJVOaJ2VRDpT9q4Y3d0AvA==}
 
   /@types/normalize-package-data@2.4.1:
     resolution: {integrity: sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==}
     dev: true
 
   /@types/parse5@6.0.3:
     resolution: {integrity: sha512-SuT16Q1K51EAVPz1K29DJ/sXjhSQ0zjvsypYJ6tlwVsRV9jwW5Adq2ch8Dq8kDBCkYnELS7N7VNCSB5nC56t/g==}
-    dev: false
 
   /@types/prop-types@15.7.5:
     resolution: {integrity: sha512-JCB8C6SnDoQf0cNycqd/35A7MjcnK+ZTqE7judS6o7utxUCg6imJg3QK2qzHKszlTjcj2cn+NwMB2i96ubpj7w==}
     dev: false
 
-  /@types/react-dom@18.0.11:
-    resolution: {integrity: sha512-O38bPbI2CWtgw/OoQoY+BRelw7uysmXbWvw3nLWO21H1HSh+GOlqPuXshJfjmpNlKiiSDG9cc1JZAaMmVdcTlw==}
+  /@types/react-dom@18.2.4:
+    resolution: {integrity: sha512-G2mHoTMTL4yoydITgOGwWdWMVd8sNgyEP85xVmMKAPUBwQWm9wBPQUmvbeF4V3WBY1P7mmL4BkjQ0SqUpf1snw==}
     dependencies:
       '@types/react': 17.0.53
     dev: false
 
   /@types/react@17.0.53:
     resolution: {integrity: sha512-1yIpQR2zdYu1Z/dc1OxC+MA6GR240u3gcnP4l6mvj/PJiVaqHsQPmWttsvHsfnhfPbU2FuGmo0wSITPygjBmsw==}
     dependencies:
       '@types/prop-types': 15.7.5
       '@types/scheduler': 0.16.2
       csstype: 3.1.1
     dev: false
 
+  /@types/react@18.2.8:
+    resolution: {integrity: sha512-lTyWUNrd8ntVkqycEEplasWy2OxNlShj3zqS0LuB1ENUGis5HodmhM7DtCoUGbxj3VW/WsGA0DUhpG6XrM7gPA==}
+    dependencies:
+      '@types/prop-types': 15.7.5
+      '@types/scheduler': 0.16.2
+      csstype: 3.1.1
+    dev: false
+
   /@types/resolve@1.20.2:
     resolution: {integrity: sha512-60BCwRFOZCQhDncwQdxxeOEEkbc5dIMccYLwbxsS4TUNeVECQ/pBJ0j09mrHOl/JJvpRPGwO9SvE4nR2Nb/a4Q==}
-    dev: false
 
   /@types/scheduler@0.16.2:
     resolution: {integrity: sha512-hppQEBDmlwhFAXKJX2KnWLYu5yMfi91yazPb2l+lbJiwW+wdo1gNeRA+3RgNSO39WYX2euey41KEwnqesU2Jew==}
     dev: false
 
   /@types/semver@6.2.3:
     resolution: {integrity: sha512-KQf+QAMWKMrtBMsB8/24w53tEsxllMj6TuA80TT/5igJalLI/zm0L3oXRbIAl4Ohfc85gyHX/jhMwsVkmhLU4A==}
@@ -1881,41 +2098,37 @@
 
   /@types/underscore@1.11.4:
     resolution: {integrity: sha512-uO4CD2ELOjw8tasUrAhvnn2W4A0ZECOvMjCivJr4gA9pGgjv+qxKWY9GLTMVEK8ej85BxQOocUyE7hImmSQYcg==}
     dev: false
 
   /@types/unist@2.0.6:
     resolution: {integrity: sha512-PBjIUxZHOuj0R15/xuwJYjFi+KZdNFrehocChv4g5hu6aFroHue8m0lBP0POdK2nKzbw0cgV1mws8+V/JAcEkQ==}
-    dev: false
 
   /@types/webpack-sources@0.1.9:
     resolution: {integrity: sha512-bvzMnzqoK16PQIC8AYHNdW45eREJQMd6WG/msQWX5V2+vZmODCOPb4TJcbgRljTZZTwTM4wUMcsI8FftNA7new==}
     dependencies:
       '@types/node': 18.14.6
       '@types/source-list-map': 0.1.2
       source-map: 0.6.1
     dev: true
 
   /@types/yargs-parser@21.0.0:
     resolution: {integrity: sha512-iO9ZQHkZxHn4mSakYV0vFHAVDyEOIJQrV2uZ06HxEPcx+mt8swXoZHIbaaJ2crJYFfErySgktuTZ3BeLz+XmFA==}
-    dev: false
 
   /@vscode/emmet-helper@2.8.6:
     resolution: {integrity: sha512-IIB8jbiKy37zN8bAIHx59YmnIelY78CGHtThnibD/d3tQOKRY83bYVi9blwmZVUZh6l9nfkYH3tvReaiNxY9EQ==}
     dependencies:
       emmet: 2.3.6
       jsonc-parser: 2.3.1
       vscode-languageserver-textdocument: 1.0.8
       vscode-languageserver-types: 3.17.3
       vscode-uri: 2.1.2
-    dev: false
 
   /@vscode/l10n@0.0.11:
     resolution: {integrity: sha512-ukOMWnCg1tCvT7WnDfsUKQOFDQGsyR5tNgRpwmqi+5/vzU3ghdDXzvIM4IOPdSb3OeSsBNvmSL8nxIVOqi2WXA==}
-    dev: false
 
   /@webassemblyjs/ast@1.11.1:
     resolution: {integrity: sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==}
     dependencies:
       '@webassemblyjs/helper-numbers': 1.11.1
       '@webassemblyjs/helper-wasm-bytecode': 1.11.1
     dev: true
@@ -2074,33 +2287,14 @@
     resolution: {integrity: sha512-rq9s+JNhf0IChjtDXxllJ7g41oZk5SlXtp0LHwyA5cejwn7vKmKp4pPri6YEePv2PU65sAsegbXtIinmDFDXgQ==}
     peerDependencies:
       acorn: ^6.0.0 || ^7.0.0 || ^8.0.0
     dependencies:
       acorn: 8.8.2
     dev: false
 
-  /acorn-node@1.8.2:
-    resolution: {integrity: sha512-8mt+fslDufLYntIoPAaIMUe/lrbrehIiwmR3t2k9LljIzoigEPF27eLk2hy8zSGzmR/ogr7zbRKINMo1u0yh5A==}
-    dependencies:
-      acorn: 7.4.1
-      acorn-walk: 7.2.0
-      xtend: 4.0.2
-    dev: false
-
-  /acorn-walk@7.2.0:
-    resolution: {integrity: sha512-OPdCF6GsMIP+Az+aWfAAOEt2/+iVDKE7oy6lJ098aoe59oAmK76qV6Gw60SbZ8jHuG2wH058GF4pLFbYamYrVA==}
-    engines: {node: '>=0.4.0'}
-    dev: false
-
-  /acorn@7.4.1:
-    resolution: {integrity: sha512-nQyp0o1/mNdbTO1PO6kHkwSrmgZ0MT/jCCpNiwbUjGoRN4dlBhqJtoQuCnEOKzgTVwg0ZWiCoQy6SxMebQVh8A==}
-    engines: {node: '>=0.4.0'}
-    hasBin: true
-    dev: false
-
   /acorn@8.8.2:
     resolution: {integrity: sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==}
     engines: {node: '>=0.4.0'}
     hasBin: true
 
   /aggregate-error@3.1.0:
     resolution: {integrity: sha512-4I7Td01quW/RpocfNayFdFVk1qSuoh0E7JrbRJ16nH01HhKFQ88INq9Sd+nd72zqRySlr9BmDA8xlEJ6vJMrYA==}
@@ -2145,33 +2339,30 @@
       '@algolia/transporter': 4.15.0
     dev: false
 
   /ansi-align@3.0.1:
     resolution: {integrity: sha512-IOfwwBF5iczOjp/WeY4YxyjqAFMQoZufdQWDd19SEExbVLNXqvpzSJ/M7Za4/sCPmQ0+GRquoA7bGcINcxew6w==}
     dependencies:
       string-width: 4.2.3
-    dev: false
 
   /ansi-colors@4.1.3:
     resolution: {integrity: sha512-/6w/C21Pm1A7aZitlI5Ni/2J6FFQN8i1Cvz3kHABAAbw93v/NlvKdVOqz7CCWz/3iv/JplRSEEZ83XION15ovw==}
     engines: {node: '>=6'}
     dev: true
 
   /ansi-regex@5.0.1:
     resolution: {integrity: sha512-quJQXlTSUGL2LH9SUXo8VwsY4soanhgo6LNSm84E1LBcE8s3O0wpdiRzyR9z/ZZJMlMWv37qOOb9pdJlMUEKFQ==}
     engines: {node: '>=8'}
 
   /ansi-regex@6.0.1:
     resolution: {integrity: sha512-n5M855fKb2SsfMIiFFoVrABHJC8QtHwVx+mHWP3QcEqBHYienj5dHSgjbxtC0WEZXYt4wcD6zrQElDPhFuZgfA==}
     engines: {node: '>=12'}
-    dev: false
 
   /ansi-sequence-parser@1.1.0:
     resolution: {integrity: sha512-lEm8mt52to2fT8GhciPCGeCXACSz2UwIN4X2e2LJSnZ5uAbn2/dsYdOmUXq0AtWS5cpAupysIneExOgH0Vd2TQ==}
-    dev: true
 
   /ansi-styles@3.2.1:
     resolution: {integrity: sha512-VT0ZI6kZRdTh8YyJw3SMbYm/u+NqfsAxEpWO0Pf9sq8/e94WxxOpPKx9FR1FlyCtOVDNOQ+8ntlqFxiRc+r5qA==}
     engines: {node: '>=4'}
     dependencies:
       color-convert: 1.9.3
 
@@ -2180,36 +2371,40 @@
     engines: {node: '>=8'}
     dependencies:
       color-convert: 2.0.1
 
   /ansi-styles@6.2.1:
     resolution: {integrity: sha512-bN798gFfQX+viw3R7yrGWRqnrN2oRkEkUjjl4JNn4E8GxxbjtG3FbrEIIY3l8/hrwUwIeCZvi4QuOTP4MErVug==}
     engines: {node: '>=12'}
+
+  /any-promise@1.3.0:
+    resolution: {integrity: sha512-7UvmKalWRt1wgjL1RrGxoSJW/0QZFIegpeGvZG9kjp8vrRu55XTHbwnqq2GpXm9uLbcuhxm3IqX9OB4MZR1b2A==}
     dev: false
 
   /anymatch@3.1.3:
     resolution: {integrity: sha512-KMReFUr0B4t+D+OBkjR3KYqvocp2XaSzO55UcB6mgQMd3KbcE+mWTyvVV7D/zsdEbNnV6acZUutkiHQXvTr1Rw==}
     engines: {node: '>= 8'}
     dependencies:
       normalize-path: 3.0.0
       picomatch: 2.3.1
-    dev: false
 
   /arg@5.0.2:
     resolution: {integrity: sha512-PYjyFOLKQ9y57JvQ6QLo8dAgNqswh8M1RMJYdQduT6xbWSgK36P/Z/v+p888pM69jMMfS8Xd8F6I1kQ/I9HUGg==}
     dev: false
 
   /argparse@1.0.10:
     resolution: {integrity: sha512-o5Roy6tNG4SL/FOkCAN6RzjiakZS25RLYFrcMttJqbdd8BWrnA+fGz57iN5Pb06pvBGvl5gQ0B48dJlslXvoTg==}
     dependencies:
       sprintf-js: 1.0.3
 
+  /argparse@2.0.1:
+    resolution: {integrity: sha512-8+9WqebbFzpX9OR+Wa6O29asIogeRMzcGtAINdpMHHyAg10f05aSFVBbcEqGf/PXw1EjAZ+q2/bEBg3DvurK3Q==}
+
   /array-iterate@2.0.1:
     resolution: {integrity: sha512-I1jXZMjAgCMmxT4qxXfPXa6SthSoE8h6gkSI9BGGNv8mP8G/v0blc+qFnZu6K42vTOiuME596QaLO0TP3Lk0xg==}
-    dev: false
 
   /array-union@2.1.0:
     resolution: {integrity: sha512-HGyxoOTYUyCM6stUe6EJgnd4EoewAI7zMdfqO+kGjnlZmBDz/cR5pf8r/cR4Wq60sL/p0IkcjUEEPwS3GFrIyw==}
     engines: {node: '>=8'}
     dev: true
 
   /array.prototype.flat@1.3.1:
@@ -2228,106 +2423,107 @@
     dev: true
 
   /astring@1.8.4:
     resolution: {integrity: sha512-97a+l2LBU3Op3bBQEff79i/E4jMD2ZLFD8rHx9B6mXyB2uQwhJQYfiDqUwtfjF4QA1F2qs//N6Cw8LetMbQjcw==}
     hasBin: true
     dev: false
 
-  /astro@2.1.2(@types/node@18.14.6):
-    resolution: {integrity: sha512-qxBIPHfFJhwNOxI2E96XrGrUM6lGkDRkDY8iqEJNFWPGP+t5yY5SWb8H+OdYUGopexy1GGjoY7SYQCzFBkt7iw==}
+  /astro@2.5.7(@types/node@18.14.6):
+    resolution: {integrity: sha512-qYKMIN4tXAOAsm10vU4f+Q7LfC05JmEbQiJmSBqIEhp+wnQcEUFkGLrHMSsps3oBzMtjErUdDDW5tGJcn5eVlA==}
     engines: {node: '>=16.12.0', npm: '>=6.14.0'}
     hasBin: true
     peerDependencies:
-      sharp: ^0.31.3
+      sharp: '>=0.31.0'
     peerDependenciesMeta:
       sharp:
         optional: true
     dependencies:
-      '@astrojs/compiler': 1.2.0
-      '@astrojs/language-server': 0.28.3
-      '@astrojs/markdown-remark': 2.1.0(astro@2.1.2)
-      '@astrojs/telemetry': 2.1.0
-      '@astrojs/webapi': 2.1.0
-      '@babel/core': 7.21.0
+      '@astrojs/compiler': 1.5.0
+      '@astrojs/language-server': 1.0.8
+      '@astrojs/markdown-remark': 2.2.1(astro@2.5.7)
+      '@astrojs/telemetry': 2.1.1
+      '@astrojs/webapi': 2.2.0
+      '@babel/core': 7.22.1
       '@babel/generator': 7.21.1
       '@babel/parser': 7.21.2
-      '@babel/plugin-transform-react-jsx': 7.21.0(@babel/core@7.21.0)
+      '@babel/plugin-transform-react-jsx': 7.21.0(@babel/core@7.22.1)
       '@babel/traverse': 7.21.2
-      '@babel/types': 7.21.2
+      '@babel/types': 7.22.4
       '@types/babel__core': 7.20.0
       '@types/yargs-parser': 21.0.0
       acorn: 8.8.2
       boxen: 6.2.1
       chokidar: 3.5.3
       ci-info: 3.8.0
       common-ancestor-path: 1.0.1
       cookie: 0.5.0
       debug: 4.3.4
       deepmerge-ts: 4.3.0
       devalue: 4.3.0
       diff: 5.1.0
       es-module-lexer: 1.2.0
-      estree-walker: 3.0.3
+      esbuild: 0.17.19
+      estree-walker: 3.0.0
       execa: 6.1.0
       fast-glob: 3.2.12
       github-slugger: 2.0.0
       gray-matter: 4.0.3
       html-escaper: 3.0.3
-      image-size: 1.0.2
+      js-yaml: 4.1.0
       kleur: 4.1.5
       magic-string: 0.27.0
       mime: 3.0.0
       ora: 6.1.2
+      p-limit: 4.0.0
       path-to-regexp: 6.2.1
       preferred-pm: 3.0.3
       prompts: 2.4.2
       rehype: 12.0.1
       semver: 7.3.8
       server-destroy: 1.0.1
-      shiki: 0.11.1
+      shiki: 0.14.1
       slash: 4.0.0
       string-width: 5.1.2
       strip-ansi: 7.0.1
       supports-esm: 1.0.0
       tsconfig-resolver: 3.0.1
       typescript: 5.0.2
       unist-util-visit: 4.1.2
       vfile: 5.3.7
-      vite: 4.1.4(@types/node@18.14.6)
-      vitefu: 0.2.4(vite@4.1.4)
+      vite: 4.3.9(@types/node@18.14.6)
+      vitefu: 0.2.4(vite@4.3.9)
       yargs-parser: 21.1.1
       zod: 3.21.4
     transitivePeerDependencies:
       - '@types/node'
       - less
       - sass
       - stylus
       - sugarss
       - supports-color
       - terser
-    dev: false
 
   /at-least-node@1.0.0:
     resolution: {integrity: sha512-+q/t7Ekv1EDY2l6Gda6LLiX14rU9TV20Wa3ofeQmwPFZbOMo9DXrLbOjFaaclkXKWidIaopwAObQDqwWtGUjqg==}
     engines: {node: '>= 4.0.0'}
     dev: true
 
-  /autoprefixer@10.4.13(postcss@8.4.21):
-    resolution: {integrity: sha512-49vKpMqcZYsJjwotvt4+h/BCjJVnhGwcLpDt5xkcaOG3eLrG/HUYLagrihYsQ+qrIBgIzX1Rw7a6L8I/ZA1Atg==}
+  /autoprefixer@10.4.14(postcss@8.4.24):
+    resolution: {integrity: sha512-FQzyfOsTlwVzjHxKEqRIAdJx9niO6VCBCoEwax/VLSoQF29ggECcPuBqUMZ+u8jCZOPSy8b8/8KnuFbp0SaFZQ==}
     engines: {node: ^10 || ^12 || >=14}
     hasBin: true
     peerDependencies:
       postcss: ^8.1.0
     dependencies:
       browserslist: 4.21.5
-      caniuse-lite: 1.0.30001462
+      caniuse-lite: 1.0.30001494
       fraction.js: 4.2.0
       normalize-range: 0.1.2
       picocolors: 1.0.0
-      postcss: 8.4.21
+      postcss: 8.4.24
       postcss-value-parser: 4.2.0
     dev: false
 
   /available-typed-arrays@1.0.5:
     resolution: {integrity: sha512-DMD0KiN46eipeziST1LPP/STfDU0sufISXmjSgvVsoU2tqxctQeASejWcfNtxYKqETM1UxQ8sp2OrSBWpHY6sw==}
     engines: {node: '>= 0.4'}
     dev: true
@@ -2347,22 +2543,20 @@
     resolution: {integrity: sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==}
     dependencies:
       underscore: 1.13.6
     dev: false
 
   /bail@2.0.2:
     resolution: {integrity: sha512-0xO6mYd7JB2YesxDKplafRpsiOzPt9V02ddPCLbY1xYGPOX24NTyN50qnUxgCPcSoYMhKpAuBTjQoRZCAkUDRw==}
-    dev: false
 
   /balanced-match@1.0.2:
     resolution: {integrity: sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==}
 
   /base64-js@1.5.1:
     resolution: {integrity: sha512-AKpaYlHn8t4SVbOHCy+b5+KKgvR4vrsD8vbvrbiQJps7fKDTkjkDry6ji0rUJjC0kzbNePLwzxq8iypo41qeWA==}
-    dev: false
 
   /better-path-resolve@1.0.0:
     resolution: {integrity: sha512-pbnl5XzGBdrFU/wT4jqmJVPn2B6UHPBOhzMQkY/SPUPB6QtUXtmBHBIwCbXJol93mOpGMnQyP/+BB19q04xj7g==}
     engines: {node: '>=4'}
     dependencies:
       is-windows: 1.0.2
     dev: true
@@ -2370,44 +2564,40 @@
   /big.js@5.2.2:
     resolution: {integrity: sha512-vyL2OymJxmarO8gxMr0mhChsO9QGwhynfuu4+MHTAW6czfq9humCB7rKpUjDd9YUiDPU4mzpyupFSvOClAwbmQ==}
     dev: true
 
   /binary-extensions@2.2.0:
     resolution: {integrity: sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==}
     engines: {node: '>=8'}
-    dev: false
 
   /bl@5.1.0:
     resolution: {integrity: sha512-tv1ZJHLfTDnXE6tMHv73YgSJaWR2AFuPwMntBe7XL/GBFHnT0CLnsHMogfk5+GzCDC5ZWarSCYaIGATZt9dNsQ==}
     dependencies:
       buffer: 6.0.3
       inherits: 2.0.4
       readable-stream: 3.6.1
-    dev: false
 
   /boxen@6.2.1:
     resolution: {integrity: sha512-H4PEsJXfFI/Pt8sjDWbHlQPx4zL/bvSQjcilJmaulGt5mLDorHOHpmdXAJcBcmru7PhYSp/cDMWRko4ZUMFkSw==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
     dependencies:
       ansi-align: 3.0.1
       camelcase: 6.3.0
       chalk: 4.1.2
       cli-boxes: 3.0.0
       string-width: 5.1.2
       type-fest: 2.19.0
       widest-line: 4.0.1
       wrap-ansi: 8.1.0
-    dev: false
 
   /brace-expansion@1.1.11:
     resolution: {integrity: sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==}
     dependencies:
       balanced-match: 1.0.2
       concat-map: 0.0.1
-    dev: true
 
   /brace-expansion@2.0.1:
     resolution: {integrity: sha512-XnAIvQ8eM+kC6aULx6wuQiwVsnzsi9d3WxzV3FpWTGA19F621kwdbsAcFKXgKUHZWsy+mY6iL1sHTxWEFCytDA==}
     dependencies:
       balanced-match: 1.0.2
     dev: false
 
@@ -2438,22 +2628,20 @@
     dev: true
 
   /buffer@6.0.3:
     resolution: {integrity: sha512-FTiCpNxtwiZZHEZbcbTIcZjERVICn9yq/pDFkTl95/AxzD1naBctN7YO68riM/gLSDY7sdrMby8hofADYuuqOA==}
     dependencies:
       base64-js: 1.5.1
       ieee754: 1.2.1
-    dev: false
 
   /busboy@1.6.0:
     resolution: {integrity: sha512-8SFQbg/0hQ9xy3UNTB0YEnsNBbWfhf7RtnzpL7TkBiTBRfrQ9Fxcnz7VJsleJpyp6rVLvXiuORqjlHi5q+PYuA==}
     engines: {node: '>=10.16.0'}
     dependencies:
       streamsearch: 1.1.0
-    dev: false
 
   /cacache@15.3.0:
     resolution: {integrity: sha512-VVdYzXEn+cnbXpFgWs5hTT7OScegHVmLhJIR8Ufqk3iFD6A6j5iSX1KuBTfNEv4tdJWE2PzA6IVFtcLC7fN9wQ==}
     engines: {node: '>= 10'}
     dependencies:
       '@npmcli/fs': 1.1.1
       '@npmcli/move-file': 1.1.2
@@ -2502,22 +2690,24 @@
     resolution: {integrity: sha512-L28STB170nwWS63UjtlEOE3dldQApaJXZkOI1uMFfzf3rRuPegHaHesyee+YxQ+W6SvRDQV6UrdOdRiR153wJg==}
     engines: {node: '>=6'}
     dev: true
 
   /camelcase@6.3.0:
     resolution: {integrity: sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==}
     engines: {node: '>=10'}
-    dev: false
 
   /caniuse-lite@1.0.30001462:
     resolution: {integrity: sha512-PDd20WuOBPiasZ7KbFnmQRyuLE7cFXW2PVd7dmALzbkUXEP46upAuCDm9eY9vho8fgNMGmbAX92QBZHzcnWIqw==}
 
+  /caniuse-lite@1.0.30001494:
+    resolution: {integrity: sha512-sY2B5Qyl46ZzfYDegrl8GBCzdawSLT4ThM9b9F+aDYUrAG2zCOyMbd2Tq34mS1g4ZKBfjRlzOohQMxx28x6wJg==}
+    dev: false
+
   /ccount@2.0.1:
     resolution: {integrity: sha512-eyrF0jiFpY+3drT6383f1qhkbGsLSifNAjA61IUjZjmLCWjItY6LB9ft9YhoDgwfmclB2zhu51Lc7+95b8NRAg==}
-    dev: false
 
   /chalk@2.4.2:
     resolution: {integrity: sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==}
     engines: {node: '>=4'}
     dependencies:
       ansi-styles: 3.2.1
       escape-string-regexp: 1.0.5
@@ -2529,27 +2719,23 @@
     dependencies:
       ansi-styles: 4.3.0
       supports-color: 7.2.0
 
   /chalk@5.2.0:
     resolution: {integrity: sha512-ree3Gqw/nazQAPuJJEy+avdl7QfZMcUvmHIKgEZkGL+xOBzRvup5Hxo6LHuMceSxOabuJLJm5Yp/92R9eMmMvA==}
     engines: {node: ^12.17.0 || ^14.13 || >=16.0.0}
-    dev: false
 
   /character-entities-html4@2.1.0:
     resolution: {integrity: sha512-1v7fgQRj6hnSwFpq1Eu0ynr/CDEw0rXo2B61qXrLNdHZmPKgb7fqS1a2JwF0rISo9q77jDI8VMEHoApn8qDoZA==}
-    dev: false
 
   /character-entities-legacy@3.0.0:
     resolution: {integrity: sha512-RpPp0asT/6ufRm//AJVwpViZbGM/MkjQFxJccQRHmISF/22NBtsHqAWmL+/pmkPWoIUJdWyeVleTl1wydHATVQ==}
-    dev: false
 
   /character-entities@2.0.2:
     resolution: {integrity: sha512-shx7oQ0Awen/BRIdkjkvz54PnEEI/EjwXDSIZp86/KKdbafHh1Df/RYGBhn4hbe2+uKC9FnT5UCEdyPz3ai9hQ==}
-    dev: false
 
   /character-reference-invalid@2.0.1:
     resolution: {integrity: sha512-iBZ4F4wRbyORVsu0jPV7gXkOsGYjGHPmAyv+HiHG8gi5PtC9KI2j1+v8/tlibRvjoWX027ypmG/n0HtO5t7unw==}
     dev: false
 
   /chardet@0.7.0:
     resolution: {integrity: sha512-mT8iDcrh03qDGRRmoA2hmBJnxpllMR+0/0qlzjqZES6NdiWDcZkCNAk4rPFZ9Q85r27unkiNNg8ZOiwZXBHwcA==}
@@ -2564,15 +2750,14 @@
       glob-parent: 5.1.2
       is-binary-path: 2.1.0
       is-glob: 4.0.3
       normalize-path: 3.0.0
       readdirp: 3.6.0
     optionalDependencies:
       fsevents: 2.3.2
-    dev: false
 
   /chownr@2.0.0:
     resolution: {integrity: sha512-bIomtDF5KGpdogkLd9VspvFzk9KfpyyGlS8YFVZl7TGPBHL5snIOnxeshwVgPteQ9b4Eydl+pVbIyE1DcvCWgQ==}
     engines: {node: '>=10'}
     dev: true
 
   /chrome-trace-event@1.0.3:
@@ -2588,27 +2773,24 @@
     resolution: {integrity: sha512-4diC9HaTE+KRAMWhDhrGOECgWZxoevMc5TlkObMqNSsVU62PYzXZ/SMTjzyGAFF1YusgxGcSWTEXBhp0CPwQ1A==}
     engines: {node: '>=6'}
     dev: true
 
   /cli-boxes@3.0.0:
     resolution: {integrity: sha512-/lzGpEWL/8PfI0BmBOPRwp0c/wFNX1RdUML3jK/RcSBA9T8mZDdQpqYBKtCFTOfQbwPqWEOpjqW+Fnayc0969g==}
     engines: {node: '>=10'}
-    dev: false
 
   /cli-cursor@4.0.0:
     resolution: {integrity: sha512-VGtlMu3x/4DOtIUwEkRezxUZ2lBacNJCHash0N0WeZDBS+7Ux1dm3XWAgWYxLJFMMdOeXMHXorshEFhbMSGelg==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
     dependencies:
       restore-cursor: 4.0.0
-    dev: false
 
   /cli-spinners@2.7.0:
     resolution: {integrity: sha512-qu3pN8Y3qHNgE2AFweciB1IfMnmZ/fsNTEE+NOFjmGB2F/7rLhnhzppvpCnN4FovtP26k8lHyy9ptEbNwWFLzw==}
     engines: {node: '>=6'}
-    dev: false
 
   /cliui@6.0.0:
     resolution: {integrity: sha512-t6wbgtoCXvAzst7QgXxJYqPt0usEfbgQdftEPbLL/cvv6HPE5VgvqCuAIDR0NgU52ds6rFwqrgakNLrHEjCbrQ==}
     dependencies:
       string-width: 4.2.3
       strip-ansi: 6.0.1
       wrap-ansi: 6.2.0
@@ -2655,50 +2837,50 @@
 
   /colorette@2.0.19:
     resolution: {integrity: sha512-3tlv/dIP7FWvj3BsbHrGLJ6l/oKh1O3TcgBqMn+yyCagOxc23fyzDS6HypQbgxWbkpDnf52p1LuR4eWDQ/K9WQ==}
     dev: true
 
   /comma-separated-tokens@2.0.3:
     resolution: {integrity: sha512-Fu4hJdvzeylCfQPp9SGWidpzrMs7tTrlu6Vb8XGaRGck8QSNZJJp538Wrb60Lax4fPwR64ViY468OIUTbRlGZg==}
-    dev: false
 
   /commander@2.20.3:
     resolution: {integrity: sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==}
     dev: true
 
+  /commander@4.1.1:
+    resolution: {integrity: sha512-NOKm8xhkzAjzFx8B2v5OAHT+u5pRQc2UCa2Vq9jYL/31o2wi9mxBA7LIFs3sV5VSC49z6pEhfbMULvShKj26WA==}
+    engines: {node: '>= 6'}
+    dev: false
+
   /commander@6.0.0:
     resolution: {integrity: sha512-s7EA+hDtTYNhuXkTlhqew4txMZVdszBmKWSPEMxGr8ru8JXR7bLUFIAtPhcSuFdJQ0ILMxnJi8GkQL0yvDy/YA==}
     engines: {node: '>= 6'}
     dev: true
 
   /commander@7.2.0:
     resolution: {integrity: sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==}
     engines: {node: '>= 10'}
     dev: true
 
   /common-ancestor-path@1.0.1:
     resolution: {integrity: sha512-L3sHRo1pXXEqX8VU28kfgUY+YGsk09hPqZiZmLacNib6XNTCM8ubYeT7ryXQw8asB1sKgcU5lkB7ONug08aB8w==}
-    dev: false
 
   /commondir@1.0.1:
     resolution: {integrity: sha512-W9pAhw0ja1Edb5GVdIF1mjZw/ASI0AlShXM83UUGe2DVr5TdAPEA1OA8m/g8zWp9x6On7gqufY+FatDbC3MDQg==}
     dev: true
 
   /concat-map@0.0.1:
     resolution: {integrity: sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==}
-    dev: true
 
   /convert-source-map@1.9.0:
     resolution: {integrity: sha512-ASFBup0Mz1uyiIjANan1jzLQami9z1PoYSZCiiYW2FczPbenXc45FZdBZLzOT+r6+iciuEModtmCti+hjaAk0A==}
-    dev: false
 
   /cookie@0.5.0:
     resolution: {integrity: sha512-YZ3GUyn/o8gfKJlnlX7g7xq4gyO6OSuhGPKaaGssGB2qgDUS0gPgtTvoyZLTt9Ab6dC4hfc9dV5arkvc/OCmrw==}
     engines: {node: '>= 0.6'}
-    dev: false
 
   /cross-spawn@5.1.0:
     resolution: {integrity: sha512-pTgQJ5KC0d2hcY8eyL1IzlBPYjTkyH72XRZPnLyKus2mBfNjQs3klqbJU2VILqZryAZUt9JOb3h/mWMy23/f5A==}
     dependencies:
       lru-cache: 4.1.5
       shebang-command: 1.2.0
       which: 1.3.1
@@ -2785,15 +2967,14 @@
     peerDependencies:
       supports-color: '*'
     peerDependenciesMeta:
       supports-color:
         optional: true
     dependencies:
       ms: 2.1.2
-    dev: false
 
   /decamelize-keys@1.1.1:
     resolution: {integrity: sha512-WiPxgEirIV0/eIOMcnFBA3/IJZAZqKnwAwWyvvdi4lsr1WCN22nhdf/3db3DoZcUjTV2SqfzIwNyp6y2xs3nmg==}
     engines: {node: '>=0.10.0'}
     dependencies:
       decamelize: 1.2.0
       map-obj: 1.0.1
@@ -2804,20 +2985,18 @@
     engines: {node: '>=0.10.0'}
     dev: true
 
   /decode-named-character-reference@1.0.2:
     resolution: {integrity: sha512-O8x12RzrUF8xyVcY0KJowWsmaJxQbmy0/EtnNtHRpsOcT7dFk5W598coHqBVpmWo1oQQfsCqfCmkZN5DJrZVdg==}
     dependencies:
       character-entities: 2.0.2
-    dev: false
 
   /deepmerge-ts@4.3.0:
     resolution: {integrity: sha512-if3ZYdkD2dClhnXR5reKtG98cwyaRT1NeugQoAPTTfsOpV9kqyeiBF9Qa5RHjemb3KzD5ulqygv6ED3t5j9eJw==}
     engines: {node: '>=12.4.0'}
-    dev: false
 
   /deepmerge@4.3.0:
     resolution: {integrity: sha512-z2wJZXrmeHdvYJp/Ux55wIjqo81G5Bp4c+oELTW+7ar6SogWHajt5a9gO3s3IDaGSAXjDk0vlQKN3rms8ab3og==}
     engines: {node: '>=0.10.0'}
     dev: false
 
   /defaults@1.0.4:
@@ -2833,101 +3012,79 @@
     resolution: {integrity: sha512-xvqAVKGfT1+UAvPwKTVw/njhdQ8ZhXK4lI0bCIuCMrp2up9nPnaDftrLtmpTazqd1o+UY4zgzU+avtMbDP+ldA==}
     engines: {node: '>= 0.4'}
     dependencies:
       has-property-descriptors: 1.0.0
       object-keys: 1.1.1
     dev: true
 
-  /defined@1.0.1:
-    resolution: {integrity: sha512-hsBd2qSVCRE+5PmNdHt1uzyrFu5d3RwmFDKzyNZMFq/EwDNJF7Ee5+D5oEKF0hU6LhtoUF1macFvOe4AskQC1Q==}
-    dev: false
-
   /dequal@2.0.3:
     resolution: {integrity: sha512-0je+qPKHEMohvfRTCEo3CrPG6cAzAYgmzKyxRiYSSDkS6eGJdyVJm7WaYA5ECaAD9wLB2T4EEeymA5aFVcYXCA==}
     engines: {node: '>=6'}
-    dev: false
 
   /detect-indent@6.1.0:
     resolution: {integrity: sha512-reYkTUJAZb9gUuZ2RvVCNhVHdg62RHnJ7WJl8ftMi4diZ6NWlciOzQN88pUhSELEwflJht4oQDv0F0BMlwaYtA==}
     engines: {node: '>=8'}
     dev: true
 
-  /detective@5.2.1:
-    resolution: {integrity: sha512-v9XE1zRnz1wRtgurGu0Bs8uHKFSTdteYZNbIPFVhUZ39L/S79ppMpdmVOZAnoz1jfEFodc48n6MX483Xo3t1yw==}
-    engines: {node: '>=0.8.0'}
-    hasBin: true
-    dependencies:
-      acorn-node: 1.8.2
-      defined: 1.0.1
-      minimist: 1.2.8
-    dev: false
-
   /devalue@4.3.0:
     resolution: {integrity: sha512-n94yQo4LI3w7erwf84mhRUkUJfhLoCZiLyoOZ/QFsDbcWNZePrLwbQpvZBUG2TNxwV3VjCKPxkiiQA6pe3TrTA==}
-    dev: false
 
   /didyoumean@1.2.2:
     resolution: {integrity: sha512-gxtyfqMg7GKyhQmb056K7M3xszy/myH8w+B4RT+QXBQsvAOdc3XymqDDPHx1BgPgsdAA5SIifona89YtRATDzw==}
     dev: false
 
   /diff@5.1.0:
     resolution: {integrity: sha512-D+mk+qE8VC/PAUrlAU34N+VfXev0ghe5ywmpqrawphmVZc1bEfn56uo9qpyGp1p4xpzOHkSW4ztBd6L7Xx4ACw==}
     engines: {node: '>=0.3.1'}
-    dev: false
 
   /dir-glob@3.0.1:
     resolution: {integrity: sha512-WkrWp9GR4KXfKGYzOLmTuGVi1UWFfws377n9cc55/tb6DuqyF6pcQ5AbiHEshaDpY9v6oaSr2XCDidGmMwdzIA==}
     engines: {node: '>=8'}
     dependencies:
       path-type: 4.0.0
     dev: true
 
   /dlv@1.1.3:
     resolution: {integrity: sha512-+HlytyjlPKnIG8XuRG8WvmBP8xs8P71y+SKKS6ZXWoEgLuePxtDoUEiH7WkdePWrQ5JBpE6aoVqfZfJUQkjXwA==}
-    dev: false
 
   /dotenv@16.0.3:
     resolution: {integrity: sha512-7GO6HghkA5fYG9TYnNxi14/7K9f5occMlp3zXAuSxn7CKCxt9xbNWG7yF8hTCSUchlfWSe3uLmlPfigevRItzQ==}
     engines: {node: '>=12'}
     dev: true
 
   /dset@3.1.2:
     resolution: {integrity: sha512-g/M9sqy3oHe477Ar4voQxWtaPIFw1jTdKZuomOjhCcBx9nHUNn0pu6NopuFFrTh/TRZIKEj+76vLWFu9BNKk+Q==}
     engines: {node: '>=4'}
-    dev: false
 
   /duplicate-package-checker-webpack-plugin@3.0.0:
     resolution: {integrity: sha512-aO50/qPC7X2ChjRFniRiscxBLT/K01bALqfcDaf8Ih5OqQ1N4iT/Abx9Ofu3/ms446vHTm46FACIuJUmgUQcDQ==}
     dependencies:
       chalk: 2.4.2
       find-root: 1.1.0
       lodash: 4.17.21
       semver: 5.7.1
     dev: true
 
   /eastasianwidth@0.2.0:
     resolution: {integrity: sha512-I88TYZWc9XiYHRQ4/3c5rjjfgkjhLyW2luGIheGERbNQ6OY7yTybanSpDXZa8y7VUP9YmDcYa+eyq4ca7iLqWA==}
-    dev: false
 
   /electron-to-chromium@1.4.325:
     resolution: {integrity: sha512-K1C03NT4I7BuzsRdCU5RWkgZxtswnKDYM6/eMhkEXqKu4e5T+ck610x3FPzu1y7HVFSiQKZqP16gnJzPpji1TQ==}
 
   /emmet@2.3.6:
     resolution: {integrity: sha512-pLS4PBPDdxuUAmw7Me7+TcHbykTsBKN/S9XJbUOMFQrNv9MoshzyMFK/R57JBm94/6HSL4vHnDeEmxlC82NQ4A==}
     dependencies:
       '@emmetio/abbreviation': 2.2.3
       '@emmetio/css-abbreviation': 2.1.4
-    dev: false
 
   /emoji-regex@8.0.0:
     resolution: {integrity: sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==}
 
   /emoji-regex@9.2.2:
     resolution: {integrity: sha512-L18DaJsXSUk2+42pv8mLs5jJT2hqFkFE4j21wOmgbUqsZ2hL72NsUU785g9RXgo3s0ZNgVl42TiHp3ZtOv/Vyg==}
-    dev: false
 
   /emojis-list@3.0.0:
     resolution: {integrity: sha512-/kyM18EfinwXZbno9FyUGeFh87KC8HRQBQGildHZbEuRyWFOmv1U10o9BBp8XVZDVNNuQKyIGIu5ZYAAXJ0V2Q==}
     engines: {node: '>= 4'}
     dev: true
 
   /enhanced-resolve@5.12.0:
@@ -2992,25 +3149,20 @@
       string.prototype.trimend: 1.0.6
       string.prototype.trimstart: 1.0.6
       typed-array-length: 1.0.4
       unbox-primitive: 1.0.2
       which-typed-array: 1.1.9
     dev: true
 
-  /es-module-lexer@0.10.5:
-    resolution: {integrity: sha512-+7IwY/kiGAacQfY+YBhKMvEmyAJnw5grTUgjG85Pe7vcUI/6b7pZjZG8nQ7+48YhzEAEqrEgD2dCz/JIK+AYvw==}
-    dev: false
-
   /es-module-lexer@0.9.3:
     resolution: {integrity: sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==}
     dev: true
 
   /es-module-lexer@1.2.0:
     resolution: {integrity: sha512-2BMfqBDeVCcOlLaL1ZAfp+D868SczNpKArrTM3dhpd7dK/OVlogzY15qpUngt+LMTq5UC/csb9vVQAgupucSbA==}
-    dev: false
 
   /es-set-tostringtag@2.0.1:
     resolution: {integrity: sha512-g3OMbtlwY3QewlqAiMLI47KywjWZoEytKr8pf6iTC8uJq5bIAH52Z9pnQ8pVL6whrCto53JZDuUIsifGeLorTg==}
     engines: {node: '>= 0.4'}
     dependencies:
       get-intrinsic: 1.2.0
       has: 1.0.3
@@ -3056,14 +3208,15 @@
       '@esbuild/linux-x64': 0.16.17
       '@esbuild/netbsd-x64': 0.16.17
       '@esbuild/openbsd-x64': 0.16.17
       '@esbuild/sunos-x64': 0.16.17
       '@esbuild/win32-arm64': 0.16.17
       '@esbuild/win32-ia32': 0.16.17
       '@esbuild/win32-x64': 0.16.17
+    dev: true
 
   /esbuild@0.17.12:
     resolution: {integrity: sha512-bX/zHl7Gn2CpQwcMtRogTTBf9l1nl+H6R8nUbjk+RuKqAE3+8FDulLA+pHvX7aA7Xe07Iwa+CWvy9I8Y2qqPKQ==}
     engines: {node: '>=12'}
     hasBin: true
     requiresBuild: true
     optionalDependencies:
@@ -3087,26 +3240,54 @@
       '@esbuild/openbsd-x64': 0.17.12
       '@esbuild/sunos-x64': 0.17.12
       '@esbuild/win32-arm64': 0.17.12
       '@esbuild/win32-ia32': 0.17.12
       '@esbuild/win32-x64': 0.17.12
     dev: true
 
+  /esbuild@0.17.19:
+    resolution: {integrity: sha512-XQ0jAPFkK/u3LcVRcvVHQcTIqD6E2H1fvZMA5dQPSOWb3suUbWbfbRf94pjc0bNzRYLfIrDRQXr7X+LHIm5oHw==}
+    engines: {node: '>=12'}
+    hasBin: true
+    requiresBuild: true
+    optionalDependencies:
+      '@esbuild/android-arm': 0.17.19
+      '@esbuild/android-arm64': 0.17.19
+      '@esbuild/android-x64': 0.17.19
+      '@esbuild/darwin-arm64': 0.17.19
+      '@esbuild/darwin-x64': 0.17.19
+      '@esbuild/freebsd-arm64': 0.17.19
+      '@esbuild/freebsd-x64': 0.17.19
+      '@esbuild/linux-arm': 0.17.19
+      '@esbuild/linux-arm64': 0.17.19
+      '@esbuild/linux-ia32': 0.17.19
+      '@esbuild/linux-loong64': 0.17.19
+      '@esbuild/linux-mips64el': 0.17.19
+      '@esbuild/linux-ppc64': 0.17.19
+      '@esbuild/linux-riscv64': 0.17.19
+      '@esbuild/linux-s390x': 0.17.19
+      '@esbuild/linux-x64': 0.17.19
+      '@esbuild/netbsd-x64': 0.17.19
+      '@esbuild/openbsd-x64': 0.17.19
+      '@esbuild/sunos-x64': 0.17.19
+      '@esbuild/win32-arm64': 0.17.19
+      '@esbuild/win32-ia32': 0.17.19
+      '@esbuild/win32-x64': 0.17.19
+
   /escalade@3.1.1:
     resolution: {integrity: sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==}
     engines: {node: '>=6'}
 
   /escape-string-regexp@1.0.5:
     resolution: {integrity: sha512-vbRorB5FUQWvla16U8R/qgaFIya2qGzwDrNmCZuYKrbdSUMG6I1ZCGQRefkRVhuOkIGVne7BQ35DSfo1qvJqFg==}
     engines: {node: '>=0.8.0'}
 
   /escape-string-regexp@5.0.0:
     resolution: {integrity: sha512-/veY75JbMK4j1yjvuUxuVsiS/hr/4iHs9FTT6cgTexxdE0Ly/glccBAkloH/DofkjRbZU3bnoj38mOmhkZ0lHw==}
     engines: {node: '>=12'}
-    dev: false
 
   /eslint-scope@5.1.1:
     resolution: {integrity: sha512-2NxwbF/hZ0KpepYN0cNbo+FN6XoK7GaHlQhgx/hIZl6Va0bF45RQOOwhLIy8lQDbuCiadSLCBnH2CFYquit5bw==}
     engines: {node: '>=8.0.0'}
     dependencies:
       esrecurse: 4.3.0
       estraverse: 4.3.0
@@ -3163,17 +3344,16 @@
   /estree-util-visit@1.2.1:
     resolution: {integrity: sha512-xbgqcrkIVbIG+lI/gzbvd9SGTJL4zqJKBFttUl5pP27KhAjtMKbX/mQXJ7qgyXpMgVy/zvpm0xoQQaGL8OloOw==}
     dependencies:
       '@types/estree-jsx': 1.0.0
       '@types/unist': 2.0.6
     dev: false
 
-  /estree-walker@2.0.2:
-    resolution: {integrity: sha512-Rfkk/Mp/DL7JVje3u18FxFujQlTNR2q6QfMSMB7AvCBx91NGj/ba3kCfza0f6dVDbw7YlRf/nDrn7pQrCCyQ/w==}
-    dev: false
+  /estree-walker@3.0.0:
+    resolution: {integrity: sha512-s6ceX0NFiU/vKPiKvFdR83U1Zffu7upwZsGwpoqfg5rbbq1l50WQ5hCeIvM6E6oD4shUHCYMsiFPns4Jk0YfMQ==}
 
   /estree-walker@3.0.3:
     resolution: {integrity: sha512-7RUKfXgSMMkzt6ZuXmqapOurLGPPfgj6l9uRZ7lRGolvk0y2yocc35LdcxKC5PQZdn2DMqioAQ2NoWcrTKmm6g==}
     dependencies:
       '@types/estree': 1.0.0
     dev: false
 
@@ -3190,26 +3370,23 @@
       human-signals: 3.0.1
       is-stream: 3.0.0
       merge-stream: 2.0.0
       npm-run-path: 5.1.0
       onetime: 6.0.0
       signal-exit: 3.0.7
       strip-final-newline: 3.0.0
-    dev: false
 
   /extend-shallow@2.0.1:
     resolution: {integrity: sha512-zCnTtlxNoAiDc3gqY2aYAWFx7XWWiasuF2K8Me5WbN8otHKTUKBwjPtNpRs/rbUZm7KxWAaNj7P1a/p52GbVug==}
     engines: {node: '>=0.10.0'}
     dependencies:
       is-extendable: 0.1.1
-    dev: false
 
   /extend@3.0.2:
     resolution: {integrity: sha512-fjquC59cD7CyW6urNXK0FBufkZcoiGG80wTuPujX590cB5Ttln20E2UB4S/WARVqhXffZl2LNgS+gQdPIIim/g==}
-    dev: false
 
   /extendable-error@0.1.7:
     resolution: {integrity: sha512-UOiS2in6/Q0FK0R0q6UY9vYpQ21mr/Qn1KOnte7vsACuNJf514WvCCUHSRCPcgjPT2bAhNIJdlE6bVap1GKmeg==}
     dev: true
 
   /external-editor@3.1.0:
     resolution: {integrity: sha512-hMQ4CX1p1izmuLYyZqLMO/qGNw10wSv9QDCPfzXfyFrOaCSSoRfqE1Kf1s5an66J5JZC62NewG+mK49jOCtQew==}
@@ -3393,15 +3570,14 @@
   /functions-have-names@1.2.3:
     resolution: {integrity: sha512-xckBUXyTIqT97tq2x2AMb+g163b5JFysYk0x4qxNFwbfQkmNZoiRHb6sPzI9/QV33WeuvVYBUIiD4NzNIyqaRQ==}
     dev: true
 
   /gensync@1.0.0-beta.2:
     resolution: {integrity: sha512-3hN7NaskYvMDLQY55gnW3NQ+mesEAepTqlg+VEbj7zzqEMBVNhzcGYYeqFo/TlYz6eQiFcp1HcsCZO+nGgS8zg==}
     engines: {node: '>=6.9.0'}
-    dev: false
 
   /get-caller-file@2.0.5:
     resolution: {integrity: sha512-DyFP3BM/3YHTQOCUL/w0OZHR0lpKeGrxotcHWcqNEdnltqFwXVfhEBQ94eIo34AfQpo0rGki4cyIiftY06h2Fg==}
     engines: {node: 6.* || 8.* || >= 10.*}
     dev: true
 
   /get-intrinsic@1.2.0:
@@ -3411,31 +3587,28 @@
       has: 1.0.3
       has-symbols: 1.0.3
     dev: true
 
   /get-stream@6.0.1:
     resolution: {integrity: sha512-ts6Wi+2j3jQjqi70w5AlN8DFnkSwC+MqmxEzdEALB2qXZYV3X/b1CTfgPLGJNMeAWxdPfU8FO1ms3NUfaHCPYg==}
     engines: {node: '>=10'}
-    dev: false
 
   /get-symbol-description@1.0.0:
     resolution: {integrity: sha512-2EmdH1YvIQiZpltCNgkuiUnyukzxM/R6NDJX31Ke3BG1Nq5b0S2PhX59UKi9vZpPDQVdqn+1IcaAwnzTT5vCjw==}
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.2
       get-intrinsic: 1.2.0
     dev: true
 
   /github-slugger@1.5.0:
     resolution: {integrity: sha512-wIh+gKBI9Nshz2o46B0B3f5k/W+WI9ZAv6y5Dn5WJ5SK1t0TnDimB4WE5rmTD05ZAIn8HALCZVmCsvj0w0v0lw==}
-    dev: false
 
   /github-slugger@2.0.0:
     resolution: {integrity: sha512-IaOQ9puYtjrkq7Y0Ygl9KDZnrf/aiUJYUpVf89y8kyaxbRG7Y1SrX/jaumrv81vc61+kiMempujsM3Yw7w5qcw==}
-    dev: false
 
   /glob-parent@5.1.2:
     resolution: {integrity: sha512-AOIgSQCepiJYwP3ARnGx+5VnTu2HBYdzbGP45eLw1vr3zB3vZLeyed1sC9hnbcOc9/SrMyM5RPQrkGz4aS9Zow==}
     engines: {node: '>= 6'}
     dependencies:
       is-glob: 4.0.3
 
@@ -3446,14 +3619,25 @@
       is-glob: 4.0.3
     dev: false
 
   /glob-to-regexp@0.4.1:
     resolution: {integrity: sha512-lkX1HJXwyMcprw/5YUZc2s7DrpAiHB21/V+E1rHUrVNokkvB6bqMzT0VfV6/86ZNabt1k14YOIaT7nDvOX3Iiw==}
     dev: true
 
+  /glob@7.1.6:
+    resolution: {integrity: sha512-LwaxwyZ72Lk7vZINtNNrywX0ZuLyStrdDtabefZKAY5ZGJhVtgdznluResxNmPitE0SAO+O26sWTHeKSI2wMBA==}
+    dependencies:
+      fs.realpath: 1.0.0
+      inflight: 1.0.6
+      inherits: 2.0.4
+      minimatch: 3.1.2
+      once: 1.4.0
+      path-is-absolute: 1.0.1
+    dev: false
+
   /glob@7.1.7:
     resolution: {integrity: sha512-OvD9ENzPLbegENnYP5UUfJIirTg4+XwMWGaQfQTY0JenxNvvIKP3U3/tAQSPIu/lHxXYSZmpXlUHeqAIdKzBLQ==}
     dependencies:
       fs.realpath: 1.0.0
       inflight: 1.0.6
       inherits: 2.0.4
       minimatch: 3.1.2
@@ -3471,15 +3655,14 @@
       minimatch: 5.1.6
       once: 1.4.0
     dev: false
 
   /globals@11.12.0:
     resolution: {integrity: sha512-WOBp/EEGUiIsJSp7wcv/y6MO+lV9UoncWqxuFfm8eBwzWNgyfBd6Gz+IeKQ9jCmyhoH99g15M3T+QaVHFjizVA==}
     engines: {node: '>=4'}
-    dev: false
 
   /globalthis@1.0.3:
     resolution: {integrity: sha512-sFdI5LyBiNTHjRd7cGPWapiHWMOXKyuBNX/cWJ3NfzrZQVa8GI/8cofCl74AOVqq9W5kNmguTIzJ/1s2gyI9wA==}
     engines: {node: '>= 0.4'}
     dependencies:
       define-properties: 1.2.0
     dev: true
@@ -3519,15 +3702,14 @@
     resolution: {integrity: sha512-5v6yZd4JK3eMI3FqqCouswVqwugaA9r4dNZB1wwcmrD02QkV5H0y7XBQW8QwQqEaZY1pM9aqORSORhJRdNK44Q==}
     engines: {node: '>=6.0'}
     dependencies:
       js-yaml: 3.14.1
       kind-of: 6.0.3
       section-matter: 1.0.0
       strip-bom-string: 1.0.0
-    dev: false
 
   /hard-rejection@2.1.0:
     resolution: {integrity: sha512-VIZB+ibDhx7ObhAe7OVtoEbuP4h/MuOTHJ+J8h/eBXotJYl0fBgR72xDFCKgIh22OJZIOVNxBMWuhAr10r8HdA==}
     engines: {node: '>=6'}
     dev: true
 
   /has-bigints@1.0.2:
@@ -3542,15 +3724,14 @@
     resolution: {integrity: sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==}
     engines: {node: '>=8'}
 
   /has-package-exports@1.3.0:
     resolution: {integrity: sha512-e9OeXPQnmPhYoJ63lXC4wWe34TxEGZDZ3OQX9XRqp2VwsfLl3bQBy7VehLnd34g3ef8CmYlBLGqEMKXuz8YazQ==}
     dependencies:
       '@ljharb/has-package-exports-patterns': 0.0.2
-    dev: false
 
   /has-property-descriptors@1.0.0:
     resolution: {integrity: sha512-62DVLZGoiEBDHQyqG4w9xCuZ7eJEwNmJRWw2VY84Oedb7WFcA27fiEVe8oUQx9hAUJ4ekurquucTGwsyO1XGdQ==}
     dependencies:
       get-intrinsic: 1.2.0
     dev: true
 
@@ -3583,21 +3764,19 @@
       '@types/hast': 2.3.4
       '@types/unist': 2.0.6
       hastscript: 7.2.0
       property-information: 6.2.0
       vfile: 5.3.7
       vfile-location: 4.1.0
       web-namespaces: 2.0.1
-    dev: false
 
   /hast-util-parse-selector@3.1.1:
     resolution: {integrity: sha512-jdlwBjEexy1oGz0aJ2f4GKMaVKkA9jwjr4MjAAI22E5fM/TXVZHuS5OpONtdeIkRKqAaryQ2E9xNQxijoThSZA==}
     dependencies:
       '@types/hast': 2.3.4
-    dev: false
 
   /hast-util-raw@7.2.3:
     resolution: {integrity: sha512-RujVQfVsOrxzPOPSzZFiwofMArbQke6DJjnFfceiEbFh7S05CbPt0cYN+A5YeD3pso0JQk6O1aHBnx9+Pm2uqg==}
     dependencies:
       '@types/hast': 2.3.4
       '@types/parse5': 6.0.3
       hast-util-from-parse5: 7.1.2
@@ -3605,15 +3784,14 @@
       html-void-elements: 2.0.1
       parse5: 6.0.1
       unist-util-position: 4.0.4
       unist-util-visit: 4.1.2
       vfile: 5.3.7
       web-namespaces: 2.0.1
       zwitch: 2.0.4
-    dev: false
 
   /hast-util-to-estree@2.3.2:
     resolution: {integrity: sha512-YYDwATNdnvZi3Qi84iatPIl1lWpXba1MeNrNbDfJfVzEBZL8uUmtR7mt7bxKBC8kuAuvb0bkojXYZzsNHyHCLg==}
     dependencies:
       '@types/estree': 1.0.0
       '@types/estree-jsx': 1.0.0
       '@types/hast': 2.3.4
@@ -3643,60 +3821,54 @@
       hast-util-raw: 7.2.3
       hast-util-whitespace: 2.0.1
       html-void-elements: 2.0.1
       property-information: 6.2.0
       space-separated-tokens: 2.0.2
       stringify-entities: 4.0.3
       zwitch: 2.0.4
-    dev: false
 
   /hast-util-to-parse5@7.1.0:
     resolution: {integrity: sha512-YNRgAJkH2Jky5ySkIqFXTQiaqcAtJyVE+D5lkN6CdtOqrnkLfGYYrEcKuHOJZlp+MwjSwuD3fZuawI+sic/RBw==}
     dependencies:
       '@types/hast': 2.3.4
       comma-separated-tokens: 2.0.3
       property-information: 6.2.0
       space-separated-tokens: 2.0.2
       web-namespaces: 2.0.1
       zwitch: 2.0.4
-    dev: false
 
   /hast-util-whitespace@2.0.1:
     resolution: {integrity: sha512-nAxA0v8+vXSBDt3AnRUNjyRIQ0rD+ntpbAp4LnPkumc5M9yUbSMa4XDU9Q6etY4f1Wp4bNgvc1yjiZtsTTrSng==}
-    dev: false
 
   /hastscript@7.2.0:
     resolution: {integrity: sha512-TtYPq24IldU8iKoJQqvZOuhi5CyCQRAbvDOX0x1eW6rsHSxa/1i2CCiptNTotGHJ3VoHRGmqiv6/D3q113ikkw==}
     dependencies:
       '@types/hast': 2.3.4
       comma-separated-tokens: 2.0.3
       hast-util-parse-selector: 3.1.1
       property-information: 6.2.0
       space-separated-tokens: 2.0.2
-    dev: false
 
   /hosted-git-info@2.8.9:
     resolution: {integrity: sha512-mxIDAb9Lsm6DoOJ7xH+5+X4y1LU/4Hi50L9C5sIswK3JzULS4bwk1FvjdBgvYR4bzT4tuUQiC15FE2f5HbLvYw==}
     dev: true
 
   /html-escaper@3.0.3:
     resolution: {integrity: sha512-RuMffC89BOWQoY0WKGpIhn5gX3iI54O6nRA0yC124NYVtzjmFWBIiFd8M0x+ZdX0P9R4lADg1mgP8C7PxGOWuQ==}
 
   /html-void-elements@2.0.1:
     resolution: {integrity: sha512-0quDb7s97CfemeJAnW9wC0hw78MtW7NU3hqtCD75g2vFlDLt36llsYD7uB7SUzojLMP24N5IatXf7ylGXiGG9A==}
-    dev: false
 
   /human-id@1.0.2:
     resolution: {integrity: sha512-UNopramDEhHJD+VR+ehk8rOslwSfByxPIZyJRfV739NDhN5LF1fa1MqnzKm2lGTQRjNrjK19Q5fhkgIfjlVUKw==}
     dev: true
 
   /human-signals@3.0.1:
     resolution: {integrity: sha512-rQLskxnM/5OCldHo+wNXbpVgDn5A17CUoKX+7Sokwaknlq7CdSnphy0W39GU8dw59XiCXmFXDg4fRuckQRKewQ==}
     engines: {node: '>=12.20.0'}
-    dev: false
 
   /iconv-lite@0.4.24:
     resolution: {integrity: sha512-v3MXnZAcvnywkTUEZomIActle7RXXeedOR31wwl7VlyoXO4Qi9arvSenNQWne1TcRwhCL1HwLI21bEqdpj8/rA==}
     engines: {node: '>=0.10.0'}
     dependencies:
       safer-buffer: 2.1.2
     dev: true
@@ -3715,41 +3887,31 @@
       postcss: ^8.1.0
     dependencies:
       postcss: 8.4.21
     dev: true
 
   /ieee754@1.2.1:
     resolution: {integrity: sha512-dcyqhDvX1C46lXZcVqCpK+FtMRQVdIMN6/Df5js2zouUsqG7I6sFxitIC+7KYK29KdXOLHdu9zL4sFnoVQnqaA==}
-    dev: false
 
   /ignore@5.2.4:
     resolution: {integrity: sha512-MAb38BcSbH0eHNBxn7ql2NH/kX33OkB3lZ1BNdh7ENeRChHTYsTvWrMubiIAMNS2llXEEgZ1MUOBtXChP3kaFQ==}
     engines: {node: '>= 4'}
     dev: true
 
-  /image-size@1.0.2:
-    resolution: {integrity: sha512-xfOoWjceHntRb3qFCrh5ZFORYH8XCdYpASltMhZ/Q0KZiOwjdE/Yl2QCiWdwD+lygV5bMCvauzgu5PxBX/Yerg==}
-    engines: {node: '>=14.0.0'}
-    hasBin: true
-    dependencies:
-      queue: 6.0.2
-    dev: false
-
   /import-local@3.1.0:
     resolution: {integrity: sha512-ASB07uLtnDs1o6EHjKpX34BKYDSqnFerfTOJL2HvMqF70LnxpjkzDB8J44oT9pu4AMPkQwf8jl6szgvNd2tRIg==}
     engines: {node: '>=8'}
     hasBin: true
     dependencies:
       pkg-dir: 4.2.0
       resolve-cwd: 3.0.0
     dev: true
 
   /import-meta-resolve@2.2.1:
     resolution: {integrity: sha512-C6lLL7EJPY44kBvA80gq4uMsVFw5x3oSKfuMl1cuZ2RkI5+UJqQXgn+6hlUew0y4ig7Ypt4CObAAIzU53Nfpuw==}
-    dev: false
 
   /imurmurhash@0.1.4:
     resolution: {integrity: sha512-JmXMZ6wuvDmLiHEml9ykzqO6lwFbof0GG4IkcGaENdCRDDmMVnny7s5HsIgHCbaq0w2MyPhDqkhTUgS2LU2PHA==}
     engines: {node: '>=0.8.19'}
     dev: true
 
   /indent-string@4.0.0:
@@ -3818,28 +3980,26 @@
     dev: true
 
   /is-binary-path@2.1.0:
     resolution: {integrity: sha512-ZMERYes6pDydyuGidse7OsHxtbI7WVeUEozgR/g7rd0xUimYNlvZRE/K2MgZTjWy725IfelLeVcEM97mmtRGXw==}
     engines: {node: '>=8'}
     dependencies:
       binary-extensions: 2.2.0
-    dev: false
 
   /is-boolean-object@1.1.2:
     resolution: {integrity: sha512-gDYaKHJmnj4aWxyj6YHyXVpdQawtVLHU5cb+eztPGczf6cjuTdwve5ZIEfgXqH4e57An1D1AKf8CZ3kYrQRqYA==}
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.2
       has-tostringtag: 1.0.0
     dev: true
 
   /is-buffer@2.0.5:
     resolution: {integrity: sha512-i2R6zNFDwgEHJyQUtJEk0XFi1i0dPFn/oqjK3/vPCcDeJvW5NQ83V8QbicfF1SupOaB0h8ntgBC2YiE7dfyctQ==}
     engines: {node: '>=4'}
-    dev: false
 
   /is-callable@1.2.7:
     resolution: {integrity: sha512-1BC0BVFhS/p0qtw6enp8e+8OD0UrK0oFLztSjNzhcKA3WDuJxxAPXzPuPtKkjEY9UUoEWlX/8fgKeu2S8i9JTA==}
     engines: {node: '>= 0.4'}
     dev: true
 
   /is-ci@3.0.1:
@@ -3870,20 +4030,18 @@
     engines: {node: '>=8'}
     hasBin: true
 
   /is-docker@3.0.0:
     resolution: {integrity: sha512-eljcgEDlEns/7AXFosB5K/2nCM4P7FQPkGc/DWLy5rmFEWvZayGrik1d9/QIY5nJ4f9YsVvBkA6kJpHn9rISdQ==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
     hasBin: true
-    dev: false
 
   /is-extendable@0.1.1:
     resolution: {integrity: sha512-5BMULNob1vgFX6EjQw5izWDxrecWK9AM72rugNr0TFldMOi0fj6Jk+zeKIt0xGj4cEfQIJth4w3OKWOJ4f+AFw==}
     engines: {node: '>=0.10.0'}
-    dev: false
 
   /is-extglob@2.1.1:
     resolution: {integrity: sha512-SbKbANkN603Vi4jEZv49LeVJMn4yGwsbzZworEoyEiutsN3nJYdbO36zfhGJ6QEDpOZIFkDtnq5JRxmvl3jsoQ==}
     engines: {node: '>=0.10.0'}
 
   /is-fullwidth-code-point@3.0.0:
     resolution: {integrity: sha512-zymm5+u+sCsSWyD9qNaejV3DFvhCKclKdizYaJUuHA83RLjb7nSuGnddCHGv0hk+KY7BMAlsWeK4Ueg6EV6XQg==}
@@ -3898,15 +4056,14 @@
   /is-hexadecimal@2.0.1:
     resolution: {integrity: sha512-DgZQp241c8oO6cA1SbTEWiXeoxV42vlcJxgH+B3hi1AiqqKruZR3ZGF8In3fj4+/y/7rHvlOZLZtgJ/4ttYGZg==}
     dev: false
 
   /is-interactive@2.0.0:
     resolution: {integrity: sha512-qP1vozQRI+BMOPcjFzrjXuQvdak2pHNUMZoeG2eRbiSqyvbEf/wQtEOTOX1guk6E3t36RkaqiSt8A/6YElNxLQ==}
     engines: {node: '>=12'}
-    dev: false
 
   /is-negative-zero@2.0.2:
     resolution: {integrity: sha512-dqJvarLawXsFbNDeJW7zAz8ItJ9cd28YufuuFzh0G8pNHjJMnY08Dv7sYX2uF5UpQOwieAeOExEYAWWfu7ZZUA==}
     engines: {node: '>= 0.4'}
     dev: true
 
   /is-number-object@1.0.7:
@@ -3924,15 +4081,14 @@
     resolution: {integrity: sha512-yvkRyxmFKEOQ4pNXCmJG5AEQNlXJS5LaONXo5/cLdTZdWvsZ1ioJEonLGAosKlMWE8lwUy/bJzMjcw8az73+Fg==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /is-plain-obj@4.1.0:
     resolution: {integrity: sha512-+Pgi+vMuUNkJyExiMBt5IlFoMyKnr5zhJ4Uspz58WOhBF5QoIZkFyNHIbBAtHwzVAgk5RtndVNsDRN61/mmDqg==}
     engines: {node: '>=12'}
-    dev: false
 
   /is-plain-object@2.0.4:
     resolution: {integrity: sha512-h5PpgXkWitc38BBMYawTYMWJHFZJVnBquFE57xFpjB8pJFiF6gZ+bU+WyI/yqXiFR5mdLsgYNaPe8uao6Uv9Og==}
     engines: {node: '>=0.10.0'}
     dependencies:
       isobject: 3.0.1
     dev: true
@@ -3956,15 +4112,14 @@
     dependencies:
       call-bind: 1.0.2
     dev: true
 
   /is-stream@3.0.0:
     resolution: {integrity: sha512-LnQR4bZ9IADDRSkvpqMGvt/tEJWclzklNgSw48V5EAaAeDd6qGvN8ei6k5p0tvxSR171VmGyHuTiAOfxAbr8kA==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
-    dev: false
 
   /is-string@1.0.7:
     resolution: {integrity: sha512-tE2UXzivje6ofPW7l23cjDOMa09gb7xlAqG6jG5ej6uPV32TlWP3NKPigtaGeHNu9fohccRYvIiZMfOOnOYUtg==}
     engines: {node: '>= 0.4'}
     dependencies:
       has-tostringtag: 1.0.0
     dev: true
@@ -3993,15 +4148,14 @@
       gopd: 1.0.1
       has-tostringtag: 1.0.0
     dev: true
 
   /is-unicode-supported@1.3.0:
     resolution: {integrity: sha512-43r2mRvz+8JRIKnWJ+3j8JtjRKZ6GmjzfaE/qiBJnikNnYv/6bagRJ1kUhNk8R5EX/GkobD+r+sfxCPJsiKBLQ==}
     engines: {node: '>=12'}
-    dev: false
 
   /is-weakref@1.0.2:
     resolution: {integrity: sha512-qctsuLZmIQ0+vSSMfoVvyFe2+GSEvnmZ2ezTup1SBse9+twCCeial6EEi3Nc2KFcf6+qz2FBPnjXsk8xhKSaPQ==}
     dependencies:
       call-bind: 1.0.2
     dev: true
 
@@ -4038,33 +4192,43 @@
     engines: {node: '>= 10.13.0'}
     dependencies:
       '@types/node': 18.14.6
       merge-stream: 2.0.0
       supports-color: 8.1.1
     dev: true
 
+  /jiti@1.18.2:
+    resolution: {integrity: sha512-QAdOptna2NYiSSpv0O/BwoHBSmz4YhpzJHyi+fnMRTXFjp7B8i/YG5Z8IfusxB1ufjcD2Sre1F3R+nX3fvy7gg==}
+    hasBin: true
+    dev: false
+
   /jquery@3.6.4:
     resolution: {integrity: sha512-v28EW9DWDFpzcD9O5iyJXg3R3+q+mET5JhnjJzQUZMHOv67bpSIHq81GEYpPNZHG+XXHsfSme3nxp/hndKEcsQ==}
     dev: false
 
   /js-tokens@4.0.0:
     resolution: {integrity: sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==}
 
   /js-yaml@3.14.1:
     resolution: {integrity: sha512-okMH7OXXJ7YrN9Ok3/SXrnu4iX9yOk+25nqX4imS2npuvTYDmo/QEZoqwZkYaIDk3jVvBOTOIEgEhaLOynBS9g==}
     hasBin: true
     dependencies:
       argparse: 1.0.10
       esprima: 4.0.1
 
+  /js-yaml@4.1.0:
+    resolution: {integrity: sha512-wpxZs9NoxZaJESJGIZTyDEaYpl0FKSA+FB9aJiyemKhMwkxQg63h4T1KJgUGHpTqPDNRcmmYLugrRjJlBtWvRA==}
+    hasBin: true
+    dependencies:
+      argparse: 2.0.1
+
   /jsesc@2.5.2:
     resolution: {integrity: sha512-OYu7XEzjkCQ3C5Ps3QIZsQfNpqoJyZZA99wd9aWd05NCtC5pWOkShK2mkL6HXQR6/Cy2lbNdPlZBpuQHXE63gA==}
     engines: {node: '>=4'}
     hasBin: true
-    dev: false
 
   /json-parse-even-better-errors@2.3.1:
     resolution: {integrity: sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==}
     dev: true
 
   /json-schema-traverse@0.4.1:
     resolution: {integrity: sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==}
@@ -4079,15 +4243,14 @@
   /json5@2.2.3:
     resolution: {integrity: sha512-XmOWe7eyHYH14cLdVPoyg+GOH3rYX++KpzrylJwSW98t3Nk+U8XOl8FWKOgwtzdb8lXGf6zYwDUzeHMWfxasyg==}
     engines: {node: '>=6'}
     hasBin: true
 
   /jsonc-parser@2.3.1:
     resolution: {integrity: sha512-H8jvkz1O50L3dMZCsLqiuB2tA7muqbSg1AtGEkN0leAqGjsUzDJir3Zwr02BhqdcITPg3ei3mZ+HjMocAknhhg==}
-    dev: false
 
   /jsonc-parser@3.2.0:
     resolution: {integrity: sha512-gfFQZrcTc8CnKXp6Y4/CBT3fTc0OVuDofpre4aEeEpSBPV5X5v4+Vmx+8snU7RLPrNHPKSgLxGo9YuQzz20o+w==}
 
   /jsonfile@4.0.0:
     resolution: {integrity: sha512-m6F1R3z8jjlf2imQHS2Qez5sjKWQzbuuhuJ/FKYFRZvPE3PuHcSMVZzfsLhGVOkfd20obL5SWEBew5ShlquNxg==}
     optionalDependencies:
@@ -4105,15 +4268,14 @@
   /kind-of@6.0.3:
     resolution: {integrity: sha512-dcS1ul+9tmeD95T+x28/ehLgd9mENa3LsvDTtzm3vyBEO7RPptvAD+t44WVXaUjTBRcrpFeFlC8WCruUR456hw==}
     engines: {node: '>=0.10.0'}
 
   /kleur@3.0.3:
     resolution: {integrity: sha512-eTIzlVOSUR+JxdDFepEYcBMtZ9Qqdef+rnzWdRZuMbOywu5tO2w2N7rqjoANZ5k9vywhL6Br1VRjUIgTQx4E8w==}
     engines: {node: '>=6'}
-    dev: false
 
   /kleur@4.1.5:
     resolution: {integrity: sha512-o+NO+8WrRiQEE4/7nwRJhN1HWpVmJm511pBHUxPLtp0BUISzlBplORYSmTclCnJvQq2tKu/sgl3xVpkc7ZWuQQ==}
     engines: {node: '>=6'}
 
   /license-webpack-plugin@2.3.21(webpack@5.76.0):
     resolution: {integrity: sha512-rVaYU9TddZN3ao8M/0PrRSCdTp2EW6VQymlgsuScld1vef0Ou7fALx3ePe83KLP3xAEDcPK5fkqUVqGBnbz1zQ==}
@@ -4131,15 +4293,14 @@
   /lilconfig@2.1.0:
     resolution: {integrity: sha512-utWOt/GHzuUxnLKxB6dk81RoOeoNeHgbrXiuGk4yyF5qlRz+iIVWu56E2fqGHFrXz0QNUhLB/8nKqvRH66JKGQ==}
     engines: {node: '>=10'}
     dev: false
 
   /lines-and-columns@1.2.4:
     resolution: {integrity: sha512-7ylylesZQ/PV29jhEDl3Ufjo6ZX7gCqJr5F7PKrqc93v7fzSymt1BpwEU8nAUXs8qzzvqhbjhK5QZg6Mt/HkBg==}
-    dev: true
 
   /load-yaml-file@0.2.0:
     resolution: {integrity: sha512-OfCBkGEw4nN6JLtgRidPX6QxjBQGQf72q3si2uvqyFEMbycSFFHwAZeXx6cJgFM9wmLrf9zBwCP3Ivqa+LLZPw==}
     engines: {node: '>=6'}
     dependencies:
       graceful-fs: 4.2.10
       js-yaml: 3.14.1
@@ -4198,19 +4359,17 @@
 
   /log-symbols@5.1.0:
     resolution: {integrity: sha512-l0x2DvrW294C9uDCoQe1VSU4gf529FkSZ6leBl4TiqZH/e+0R7hSfHQBNut2mNygDgHwvYHfFLn6Oxb3VWj2rA==}
     engines: {node: '>=12'}
     dependencies:
       chalk: 5.2.0
       is-unicode-supported: 1.3.0
-    dev: false
 
   /longest-streak@3.1.0:
     resolution: {integrity: sha512-9Ri+o0JYgehTaVBBDoMqIl8GXtbWg711O3srftcHhZ0dqnETqLaoIK0x17fUw9rFSlK/0NlsKe0Ahhyl5pXE2g==}
-    dev: false
 
   /loose-envify@1.4.0:
     resolution: {integrity: sha512-lyuxPGr/Wfhrlem2CL/UcnUc1zcqKAImBDzukY7Y5F/yQiNdko6+fRLevlw1HgMySw7f611UIY408EtxRSoK3Q==}
     hasBin: true
     dependencies:
       js-tokens: 4.0.0
     dev: false
@@ -4222,28 +4381,26 @@
       yallist: 2.1.2
     dev: true
 
   /lru-cache@5.1.1:
     resolution: {integrity: sha512-KpNARQA3Iwv+jTA0utUVVbrh+Jlrr1Fv0e56GGzAFOXN7dk/FviaDW8LHmK52DlcH4WP2n6gI8vN1aesBFgo9w==}
     dependencies:
       yallist: 3.1.1
-    dev: false
 
   /lru-cache@6.0.0:
     resolution: {integrity: sha512-Jo6dJ04CmSjuznwJSS3pUeWmd/H0ffTlkXXgwZi+eq1UCmqQwCh+eLsYOYCwY991i2Fah4h1BEMCx4qThGbsiA==}
     engines: {node: '>=10'}
     dependencies:
       yallist: 4.0.0
 
   /magic-string@0.27.0:
     resolution: {integrity: sha512-8UnnX2PeRAPZuN12svgR9j7M1uWMovg/CEnIwIG0LFkXSJJe4PdfUGiTGl8V9bsBHFUtfVINcSyYxd7q+kx9fA==}
     engines: {node: '>=12'}
     dependencies:
       '@jridgewell/sourcemap-codec': 1.4.14
-    dev: false
 
   /make-dir@3.1.0:
     resolution: {integrity: sha512-g3FeP20LNwhALb/6Cz6Dd4F2ngze0jz7tbzrD2wAV+o9FeNHe4rL+yK2md0J/fiSf1sa1ADhXqi5+oVwOM/eGw==}
     engines: {node: '>=8'}
     dependencies:
       semver: 6.3.0
     dev: true
@@ -4261,32 +4418,29 @@
   /markdown-extensions@1.1.1:
     resolution: {integrity: sha512-WWC0ZuMzCyDHYCasEGs4IPvLyTGftYwh6wIEOULOF0HXcqZlhwRzrK0w2VUlxWA98xnvb/jszw4ZSkJ6ADpM6Q==}
     engines: {node: '>=0.10.0'}
     dev: false
 
   /markdown-table@3.0.3:
     resolution: {integrity: sha512-Z1NL3Tb1M9wH4XESsCDEksWoKTdlUafKc4pt0GRwjUyXaCFZ+dc3g2erqB6zm3szA2IUSi7VnPI+o/9jnxh9hw==}
-    dev: false
 
   /mdast-util-definitions@5.1.2:
     resolution: {integrity: sha512-8SVPMuHqlPME/z3gqVwWY4zVXn8lqKv/pAhC57FuJ40ImXyBpmO5ukh98zB2v7Blql2FiHjHv9LVztSIqjY+MA==}
     dependencies:
       '@types/mdast': 3.0.10
       '@types/unist': 2.0.6
       unist-util-visit: 4.1.2
-    dev: false
 
   /mdast-util-find-and-replace@2.2.2:
     resolution: {integrity: sha512-MTtdFRz/eMDHXzeK6W3dO7mXUlF82Gom4y0oOgvHhh/HXZAGvIQDUvQ0SuUx+j2tv44b8xTHOm8K/9OoRFnXKw==}
     dependencies:
       '@types/mdast': 3.0.10
       escape-string-regexp: 5.0.0
       unist-util-is: 5.2.1
       unist-util-visit-parents: 5.1.3
-    dev: false
 
   /mdast-util-from-markdown@1.3.0:
     resolution: {integrity: sha512-HN3W1gRIuN/ZW295c7zi7g9lVBllMgZE40RxCX37wrTPWXCWtpvOZdfnuK+1WNpvZje6XuJeI3Wnb4TJEUem+g==}
     dependencies:
       '@types/mdast': 3.0.10
       '@types/unist': 2.0.6
       decode-named-character-reference: 1.0.2
@@ -4297,15 +4451,14 @@
       micromark-util-normalize-identifier: 1.0.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       unist-util-stringify-position: 3.0.3
       uvu: 0.5.6
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
   /mdast-util-frontmatter@1.0.1:
     resolution: {integrity: sha512-JjA2OjxRqAa8wEG8hloD0uTU0kdn8kbtOWpPP94NBkfAlbxn4S8gCGf/9DwFtEeGPXrDcNXdiDjVaRdUFqYokw==}
     dependencies:
       '@types/mdast': 3.0.10
       mdast-util-to-markdown: 1.5.0
       micromark-extension-frontmatter: 1.0.1
@@ -4314,62 +4467,56 @@
   /mdast-util-gfm-autolink-literal@1.0.3:
     resolution: {integrity: sha512-My8KJ57FYEy2W2LyNom4n3E7hKTuQk/0SES0u16tjA9Z3oFkF4RrC/hPAPgjlSpezsOvI8ObcXcElo92wn5IGA==}
     dependencies:
       '@types/mdast': 3.0.10
       ccount: 2.0.1
       mdast-util-find-and-replace: 2.2.2
       micromark-util-character: 1.1.0
-    dev: false
 
   /mdast-util-gfm-footnote@1.0.2:
     resolution: {integrity: sha512-56D19KOGbE00uKVj3sgIykpwKL179QsVFwx/DCW0u/0+URsryacI4MAdNJl0dh+u2PSsD9FtxPFbHCzJ78qJFQ==}
     dependencies:
       '@types/mdast': 3.0.10
       mdast-util-to-markdown: 1.5.0
       micromark-util-normalize-identifier: 1.0.0
-    dev: false
 
   /mdast-util-gfm-strikethrough@1.0.3:
     resolution: {integrity: sha512-DAPhYzTYrRcXdMjUtUjKvW9z/FNAMTdU0ORyMcbmkwYNbKocDpdk+PX1L1dQgOID/+vVs1uBQ7ElrBQfZ0cuiQ==}
     dependencies:
       '@types/mdast': 3.0.10
       mdast-util-to-markdown: 1.5.0
-    dev: false
 
   /mdast-util-gfm-table@1.0.7:
     resolution: {integrity: sha512-jjcpmNnQvrmN5Vx7y7lEc2iIOEytYv7rTvu+MeyAsSHTASGCCRA79Igg2uKssgOs1i1po8s3plW0sTu1wkkLGg==}
     dependencies:
       '@types/mdast': 3.0.10
       markdown-table: 3.0.3
       mdast-util-from-markdown: 1.3.0
       mdast-util-to-markdown: 1.5.0
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
   /mdast-util-gfm-task-list-item@1.0.2:
     resolution: {integrity: sha512-PFTA1gzfp1B1UaiJVyhJZA1rm0+Tzn690frc/L8vNX1Jop4STZgOE6bxUhnzdVSB+vm2GU1tIsuQcA9bxTQpMQ==}
     dependencies:
       '@types/mdast': 3.0.10
       mdast-util-to-markdown: 1.5.0
-    dev: false
 
   /mdast-util-gfm@2.0.2:
     resolution: {integrity: sha512-qvZ608nBppZ4icQlhQQIAdc6S3Ffj9RGmzwUKUWuEICFnd1LVkN3EktF7ZHAgfcEdvZB5owU9tQgt99e2TlLjg==}
     dependencies:
       mdast-util-from-markdown: 1.3.0
       mdast-util-gfm-autolink-literal: 1.0.3
       mdast-util-gfm-footnote: 1.0.2
       mdast-util-gfm-strikethrough: 1.0.3
       mdast-util-gfm-table: 1.0.7
       mdast-util-gfm-task-list-item: 1.0.2
       mdast-util-to-markdown: 1.5.0
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
   /mdast-util-mdx-expression@1.3.2:
     resolution: {integrity: sha512-xIPmR5ReJDu/DHH1OoIT1HkuybIfRGYRywC+gJtI7qHjCJp/M9jrmBEJW22O8lskDWm562BX2W8TiAwRTb0rKA==}
     dependencies:
       '@types/estree-jsx': 1.0.0
       '@types/hast': 2.3.4
       '@types/mdast': 3.0.10
@@ -4423,47 +4570,43 @@
     dev: false
 
   /mdast-util-phrasing@3.0.1:
     resolution: {integrity: sha512-WmI1gTXUBJo4/ZmSk79Wcb2HcjPJBzM1nlI/OUWA8yk2X9ik3ffNbBGsU+09BFmXaL1IBb9fiuvq6/KMiNycSg==}
     dependencies:
       '@types/mdast': 3.0.10
       unist-util-is: 5.2.1
-    dev: false
 
   /mdast-util-to-hast@12.3.0:
     resolution: {integrity: sha512-pits93r8PhnIoU4Vy9bjW39M2jJ6/tdHyja9rrot9uujkN7UTU9SDnE6WNJz/IGyQk3XHX6yNNtrBH6cQzm8Hw==}
     dependencies:
       '@types/hast': 2.3.4
       '@types/mdast': 3.0.10
       mdast-util-definitions: 5.1.2
       micromark-util-sanitize-uri: 1.1.0
       trim-lines: 3.0.1
       unist-util-generated: 2.0.1
       unist-util-position: 4.0.4
       unist-util-visit: 4.1.2
-    dev: false
 
   /mdast-util-to-markdown@1.5.0:
     resolution: {integrity: sha512-bbv7TPv/WC49thZPg3jXuqzuvI45IL2EVAr/KxF0BSdHsU0ceFHOmwQn6evxAh1GaoK/6GQ1wp4R4oW2+LFL/A==}
     dependencies:
       '@types/mdast': 3.0.10
       '@types/unist': 2.0.6
       longest-streak: 3.1.0
       mdast-util-phrasing: 3.0.1
       mdast-util-to-string: 3.1.1
       micromark-util-decode-string: 1.0.2
       unist-util-visit: 4.1.2
       zwitch: 2.0.4
-    dev: false
 
   /mdast-util-to-string@3.1.1:
     resolution: {integrity: sha512-tGvhT94e+cVnQt8JWE9/b3cUQZWS732TJxXHktvP+BYo62PpYD53Ls/6cC60rW21dW+txxiM4zMdc6abASvZKA==}
     dependencies:
       '@types/mdast': 3.0.10
-    dev: false
 
   /meow@6.1.1:
     resolution: {integrity: sha512-3YffViIt2QWgTy6Pale5QpopX/IvU3LPL03jOTqp6pGj3VjesdO/U8CuHMKpnQr4shCNCM5fd5XFFvIIl6JBHg==}
     engines: {node: '>=8'}
     dependencies:
       '@types/minimist': 1.2.2
       camelcase-keys: 6.2.2
@@ -4500,15 +4643,14 @@
       micromark-util-html-tag-name: 1.1.0
       micromark-util-normalize-identifier: 1.0.0
       micromark-util-resolve-all: 1.0.0
       micromark-util-subtokenize: 1.0.2
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       uvu: 0.5.6
-    dev: false
 
   /micromark-extension-frontmatter@1.0.1:
     resolution: {integrity: sha512-9OJhCXkrpj8qIXW5AAgRZGvS8Q4GTMdH5+Ljt98kV4XQVflRGeEhNRYp6O/zCvf8c8lZ+wc4uwmbly27pS/s4Q==}
     dependencies:
       fault: 2.0.1
       micromark-util-character: 1.1.0
       micromark-util-symbol: 1.0.1
@@ -4519,78 +4661,71 @@
     resolution: {integrity: sha512-i3dmvU0htawfWED8aHMMAzAVp/F0Z+0bPh3YrbTPPL1v4YAlCZpy5rBO5p0LPYiZo0zFVkoYh7vDU7yQSiCMjg==}
     dependencies:
       micromark-util-character: 1.1.0
       micromark-util-sanitize-uri: 1.1.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       uvu: 0.5.6
-    dev: false
 
   /micromark-extension-gfm-footnote@1.0.4:
     resolution: {integrity: sha512-E/fmPmDqLiMUP8mLJ8NbJWJ4bTw6tS+FEQS8CcuDtZpILuOb2kjLqPEeAePF1djXROHXChM/wPJw0iS4kHCcIg==}
     dependencies:
       micromark-core-commonmark: 1.0.6
       micromark-factory-space: 1.0.0
       micromark-util-character: 1.1.0
       micromark-util-normalize-identifier: 1.0.0
       micromark-util-sanitize-uri: 1.1.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       uvu: 0.5.6
-    dev: false
 
   /micromark-extension-gfm-strikethrough@1.0.4:
     resolution: {integrity: sha512-/vjHU/lalmjZCT5xt7CcHVJGq8sYRm80z24qAKXzaHzem/xsDYb2yLL+NNVbYvmpLx3O7SYPuGL5pzusL9CLIQ==}
     dependencies:
       micromark-util-chunked: 1.0.0
       micromark-util-classify-character: 1.0.0
       micromark-util-resolve-all: 1.0.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       uvu: 0.5.6
-    dev: false
 
   /micromark-extension-gfm-table@1.0.5:
     resolution: {integrity: sha512-xAZ8J1X9W9K3JTJTUL7G6wSKhp2ZYHrFk5qJgY/4B33scJzE2kpfRL6oiw/veJTbt7jiM/1rngLlOKPWr1G+vg==}
     dependencies:
       micromark-factory-space: 1.0.0
       micromark-util-character: 1.1.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       uvu: 0.5.6
-    dev: false
 
   /micromark-extension-gfm-tagfilter@1.0.1:
     resolution: {integrity: sha512-Ty6psLAcAjboRa/UKUbbUcwjVAv5plxmpUTy2XC/3nJFL37eHej8jrHrRzkqcpipJliuBH30DTs7+3wqNcQUVA==}
     dependencies:
       micromark-util-types: 1.0.2
-    dev: false
 
   /micromark-extension-gfm-task-list-item@1.0.3:
     resolution: {integrity: sha512-PpysK2S1Q/5VXi72IIapbi/jliaiOFzv7THH4amwXeYXLq3l1uo8/2Be0Ac1rEwK20MQEsGH2ltAZLNY2KI/0Q==}
     dependencies:
       micromark-factory-space: 1.0.0
       micromark-util-character: 1.1.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       uvu: 0.5.6
-    dev: false
 
   /micromark-extension-gfm@2.0.1:
     resolution: {integrity: sha512-p2sGjajLa0iYiGQdT0oelahRYtMWvLjy8J9LOCxzIQsllMCGLbsLW+Nc+N4vi02jcRJvedVJ68cjelKIO6bpDA==}
     dependencies:
       micromark-extension-gfm-autolink-literal: 1.0.3
       micromark-extension-gfm-footnote: 1.0.4
       micromark-extension-gfm-strikethrough: 1.0.4
       micromark-extension-gfm-table: 1.0.5
       micromark-extension-gfm-tagfilter: 1.0.1
       micromark-extension-gfm-task-list-item: 1.0.3
       micromark-util-combine-extensions: 1.0.0
       micromark-util-types: 1.0.2
-    dev: false
 
   /micromark-extension-mdx-expression@1.0.4:
     resolution: {integrity: sha512-TCgLxqW6ReQ3AJgtj1P0P+8ZThBTloLbeb7jNaqr6mCOLDpxUiBFE/9STgooMZttEwOQu5iEcCCa3ZSDhY9FGw==}
     dependencies:
       micromark-factory-mdx-expression: 1.0.7
       micromark-factory-space: 1.0.0
       micromark-util-character: 1.1.0
@@ -4648,24 +4783,22 @@
 
   /micromark-factory-destination@1.0.0:
     resolution: {integrity: sha512-eUBA7Rs1/xtTVun9TmV3gjfPz2wEwgK5R5xcbIM5ZYAtvGF6JkyaDsj0agx8urXnO31tEO6Ug83iVH3tdedLnw==}
     dependencies:
       micromark-util-character: 1.1.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
-    dev: false
 
   /micromark-factory-label@1.0.2:
     resolution: {integrity: sha512-CTIwxlOnU7dEshXDQ+dsr2n+yxpP0+fn271pu0bwDIS8uqfFcumXpj5mLn3hSC8iw2MUr6Gx8EcKng1dD7i6hg==}
     dependencies:
       micromark-util-character: 1.1.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       uvu: 0.5.6
-    dev: false
 
   /micromark-factory-mdx-expression@1.0.7:
     resolution: {integrity: sha512-QAdFbkQagTZ/eKb8zDGqmjvgevgJH3+aQpvvKrXWxNJp3o8/l2cAbbrBd0E04r0Gx6nssPpqWIjnbHFvZu5qsQ==}
     dependencies:
       micromark-factory-space: 1.0.0
       micromark-util-character: 1.1.0
       micromark-util-events-to-acorn: 1.2.1
@@ -4677,81 +4810,71 @@
     dev: false
 
   /micromark-factory-space@1.0.0:
     resolution: {integrity: sha512-qUmqs4kj9a5yBnk3JMLyjtWYN6Mzfcx8uJfi5XAveBniDevmZasdGBba5b4QsvRcAkmvGo5ACmSUmyGiKTLZew==}
     dependencies:
       micromark-util-character: 1.1.0
       micromark-util-types: 1.0.2
-    dev: false
 
   /micromark-factory-title@1.0.2:
     resolution: {integrity: sha512-zily+Nr4yFqgMGRKLpTVsNl5L4PMu485fGFDOQJQBl2NFpjGte1e86zC0da93wf97jrc4+2G2GQudFMHn3IX+A==}
     dependencies:
       micromark-factory-space: 1.0.0
       micromark-util-character: 1.1.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       uvu: 0.5.6
-    dev: false
 
   /micromark-factory-whitespace@1.0.0:
     resolution: {integrity: sha512-Qx7uEyahU1lt1RnsECBiuEbfr9INjQTGa6Err+gF3g0Tx4YEviPbqqGKNv/NrBaE7dVHdn1bVZKM/n5I/Bak7A==}
     dependencies:
       micromark-factory-space: 1.0.0
       micromark-util-character: 1.1.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
-    dev: false
 
   /micromark-util-character@1.1.0:
     resolution: {integrity: sha512-agJ5B3unGNJ9rJvADMJ5ZiYjBRyDpzKAOk01Kpi1TKhlT1APx3XZk6eN7RtSz1erbWHC2L8T3xLZ81wdtGRZzg==}
     dependencies:
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
-    dev: false
 
   /micromark-util-chunked@1.0.0:
     resolution: {integrity: sha512-5e8xTis5tEZKgesfbQMKRCyzvffRRUX+lK/y+DvsMFdabAicPkkZV6gO+FEWi9RfuKKoxxPwNL+dFF0SMImc1g==}
     dependencies:
       micromark-util-symbol: 1.0.1
-    dev: false
 
   /micromark-util-classify-character@1.0.0:
     resolution: {integrity: sha512-F8oW2KKrQRb3vS5ud5HIqBVkCqQi224Nm55o5wYLzY/9PwHGXC01tr3d7+TqHHz6zrKQ72Okwtvm/xQm6OVNZA==}
     dependencies:
       micromark-util-character: 1.1.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
-    dev: false
 
   /micromark-util-combine-extensions@1.0.0:
     resolution: {integrity: sha512-J8H058vFBdo/6+AsjHp2NF7AJ02SZtWaVUjsayNFeAiydTxUwViQPxN0Hf8dp4FmCQi0UUFovFsEyRSUmFH3MA==}
     dependencies:
       micromark-util-chunked: 1.0.0
       micromark-util-types: 1.0.2
-    dev: false
 
   /micromark-util-decode-numeric-character-reference@1.0.0:
     resolution: {integrity: sha512-OzO9AI5VUtrTD7KSdagf4MWgHMtET17Ua1fIpXTpuhclCqD8egFWo85GxSGvxgkGS74bEahvtM0WP0HjvV0e4w==}
     dependencies:
       micromark-util-symbol: 1.0.1
-    dev: false
 
   /micromark-util-decode-string@1.0.2:
     resolution: {integrity: sha512-DLT5Ho02qr6QWVNYbRZ3RYOSSWWFuH3tJexd3dgN1odEuPNxCngTCXJum7+ViRAd9BbdxCvMToPOD/IvVhzG6Q==}
     dependencies:
       decode-named-character-reference: 1.0.2
       micromark-util-character: 1.1.0
       micromark-util-decode-numeric-character-reference: 1.0.0
       micromark-util-symbol: 1.0.1
-    dev: false
 
   /micromark-util-encode@1.0.1:
     resolution: {integrity: sha512-U2s5YdnAYexjKDel31SVMPbfi+eF8y1U4pfiRW/Y8EFVCy/vgxk/2wWTxzcqE71LHtCuCzlBDRU2a5CQ5j+mQA==}
-    dev: false
 
   /micromark-util-events-to-acorn@1.2.1:
     resolution: {integrity: sha512-mkg3BaWlw6ZTkQORrKVBW4o9ICXPxLtGz51vml5mQpKFdo9vqIX68CAx5JhTOdjQyAHH7JFmm4rh8toSPQZUmg==}
     dependencies:
       '@types/acorn': 4.0.6
       '@types/estree': 1.0.0
       estree-util-visit: 1.2.1
@@ -4759,52 +4882,45 @@
       uvu: 0.5.6
       vfile-location: 4.1.0
       vfile-message: 3.1.4
     dev: false
 
   /micromark-util-html-tag-name@1.1.0:
     resolution: {integrity: sha512-BKlClMmYROy9UiV03SwNmckkjn8QHVaWkqoAqzivabvdGcwNGMMMH/5szAnywmsTBUzDsU57/mFi0sp4BQO6dA==}
-    dev: false
 
   /micromark-util-normalize-identifier@1.0.0:
     resolution: {integrity: sha512-yg+zrL14bBTFrQ7n35CmByWUTFsgst5JhA4gJYoty4Dqzj4Z4Fr/DHekSS5aLfH9bdlfnSvKAWsAgJhIbogyBg==}
     dependencies:
       micromark-util-symbol: 1.0.1
-    dev: false
 
   /micromark-util-resolve-all@1.0.0:
     resolution: {integrity: sha512-CB/AGk98u50k42kvgaMM94wzBqozSzDDaonKU7P7jwQIuH2RU0TeBqGYJz2WY1UdihhjweivStrJ2JdkdEmcfw==}
     dependencies:
       micromark-util-types: 1.0.2
-    dev: false
 
   /micromark-util-sanitize-uri@1.1.0:
     resolution: {integrity: sha512-RoxtuSCX6sUNtxhbmsEFQfWzs8VN7cTctmBPvYivo98xb/kDEoTCtJQX5wyzIYEmk/lvNFTat4hL8oW0KndFpg==}
     dependencies:
       micromark-util-character: 1.1.0
       micromark-util-encode: 1.0.1
       micromark-util-symbol: 1.0.1
-    dev: false
 
   /micromark-util-subtokenize@1.0.2:
     resolution: {integrity: sha512-d90uqCnXp/cy4G881Ub4psE57Sf8YD0pim9QdjCRNjfas2M1u6Lbt+XZK9gnHL2XFhnozZiEdCa9CNfXSfQ6xA==}
     dependencies:
       micromark-util-chunked: 1.0.0
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       uvu: 0.5.6
-    dev: false
 
   /micromark-util-symbol@1.0.1:
     resolution: {integrity: sha512-oKDEMK2u5qqAptasDAwWDXq0tG9AssVwAx3E9bBF3t/shRIGsWIRG+cGafs2p/SnDSOecnt6hZPCE2o6lHfFmQ==}
-    dev: false
 
   /micromark-util-types@1.0.2:
     resolution: {integrity: sha512-DCfg/T8fcrhrRKTPjRrw/5LLvdGV7BHySf/1LOZx7TzWZdYRjogNtyNq885z3nNallwr3QUKARjqvHqX1/7t+w==}
-    dev: false
 
   /micromark@3.1.0:
     resolution: {integrity: sha512-6Mj0yHLdUZjHnOPgr5xfWIMqMWS12zDN6iws9SLuSz76W8jTtAv24MN4/CL7gJrl5vtxGInkkqDv/JIoRsQOvA==}
     dependencies:
       '@types/debug': 4.1.7
       debug: 4.3.4
       decode-named-character-reference: 1.0.2
@@ -4820,15 +4936,14 @@
       micromark-util-sanitize-uri: 1.1.0
       micromark-util-subtokenize: 1.0.2
       micromark-util-symbol: 1.0.1
       micromark-util-types: 1.0.2
       uvu: 0.5.6
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
   /micromatch@4.0.5:
     resolution: {integrity: sha512-DMy+ERcEW2q8Z2Po+WNXuw3c5YaUSFjAO5GsJqfEl7UjvtIuFKO6ZrKvcItdy98dwFI2N1tg3zNIdKaQT+aNdA==}
     engines: {node: '>=8.6'}
     dependencies:
       braces: 3.0.2
       picomatch: 2.3.1
@@ -4845,25 +4960,22 @@
       mime-db: 1.52.0
     dev: true
 
   /mime@3.0.0:
     resolution: {integrity: sha512-jSCU7/VB1loIWBZe14aEYHU/+1UMEHoaO7qxCOVJOw9GgH72VAWppxNcjU+x9a2k3GSIBXNKxXQFqRvvZ7vr3A==}
     engines: {node: '>=10.0.0'}
     hasBin: true
-    dev: false
 
   /mimic-fn@2.1.0:
     resolution: {integrity: sha512-OqbOk5oEQeAZ8WXWydlu9HJjz9WVdEIvamMCcXmuqUYjTknH/sqsWvhQ3vgwKFRR1HpjvNBKQ37nbJgYzGqGcg==}
     engines: {node: '>=6'}
-    dev: false
 
   /mimic-fn@4.0.0:
     resolution: {integrity: sha512-vqiC06CuhBTUdZH+RYl8sFrL096vA45Ok5ISO6sE/Mr1jRbGH4Csnhi8f3wKVl7x8mO4Au7Ir9D3Oyv1VYMFJw==}
     engines: {node: '>=12'}
-    dev: false
 
   /min-indent@1.0.1:
     resolution: {integrity: sha512-I9jwMn07Sy/IwOj3zVkVik2JTvgpaykDZEigL6Rx6N9LbMywwUSMtxET+7lVoDLLd3O3IXwJwvuuns8UB/HeAg==}
     engines: {node: '>=4'}
     dev: true
 
   /mini-css-extract-plugin@1.3.9(webpack@5.76.0):
@@ -4878,15 +4990,14 @@
       webpack-sources: 1.4.3
     dev: true
 
   /minimatch@3.1.2:
     resolution: {integrity: sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==}
     dependencies:
       brace-expansion: 1.1.11
-    dev: true
 
   /minimatch@5.1.6:
     resolution: {integrity: sha512-lKwV/1brpG6mBUFHtb7NUmtABCb2WZZmm2wNiOA5hAb8VdCS4B3dtMWyvcoViccwAW/COERjXLt0zP1zXUN26g==}
     engines: {node: '>=10'}
     dependencies:
       brace-expansion: 2.0.1
     dev: false
@@ -4958,34 +5069,45 @@
   /moment@2.29.4:
     resolution: {integrity: sha512-5LC9SOxjSc2HF6vO2CyuTDNivEdoz2IvyJJGj6X8DJ0eFyfszE0QiEd+iXmBvUP3WHxSjFH/vIsA0EN00cgr8w==}
     dev: false
 
   /mri@1.2.0:
     resolution: {integrity: sha512-tzzskb3bG8LvYGFF/mDTpq3jpI6Q9wc3LEmBaghu+DdCssd1FakN7Bc0hVNmEyGq1bq3RgfkCb3cmQLpNPOroA==}
     engines: {node: '>=4'}
-    dev: false
 
   /ms@2.1.2:
     resolution: {integrity: sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==}
+
+  /mz@2.7.0:
+    resolution: {integrity: sha512-z81GNO7nnYMEhrGh9LeymoE4+Yr0Wn5McHIZMK5cfQCl+NDX08sCZgUc9/6MHni9IWuFLm1Z3HTCXu2z9fN62Q==}
+    dependencies:
+      any-promise: 1.3.0
+      object-assign: 4.1.1
+      thenify-all: 1.6.0
     dev: false
 
   /nanoid@3.3.4:
     resolution: {integrity: sha512-MqBkQh/OHTS2egovRtLk45wEyNXwF+cokD+1YPf9u5VfJiRdAiRwB2froX5Co9Rh20xs4siNPm8naNotSD6RBw==}
     engines: {node: ^10 || ^12 || ^13.7 || ^14 || >=15.0.1}
     hasBin: true
+    dev: true
+
+  /nanoid@3.3.6:
+    resolution: {integrity: sha512-BGcqMMJuToF7i1rt+2PWSNVnWIkGCU78jBG3RxO/bZlnZPK2Cmi2QaffxGO/2RvWi9sL+FAiRiXMgsyxQ1DIDA==}
+    engines: {node: ^10 || ^12 || ^13.7 || ^14 || >=15.0.1}
+    hasBin: true
 
   /neo-async@2.6.2:
     resolution: {integrity: sha512-Yd3UES5mWCSqR+qNT93S3UoYUkqAZ9lLg8a7g9rimsWmYGK8cVToA4/sF3RrshdyV3sAGMXVUmpMYOw+dLpOuw==}
     dev: true
 
   /nlcst-to-string@3.1.1:
     resolution: {integrity: sha512-63mVyqaqt0cmn2VcI2aH6kxe1rLAmSROqHMA0i4qqg1tidkfExgpb0FGMikMCn86mw5dFtBtEANfmSSK7TjNHw==}
     dependencies:
       '@types/nlcst': 1.0.0
-    dev: false
 
   /node-fetch@2.6.9:
     resolution: {integrity: sha512-DJm/CJkZkRjKKj4Zi4BsKVZh3ValV5IR5s7LVZnW+6YMh0W1BfNA8XSs6DLMGYlId5F3KnA70uu2qepcR08Qqg==}
     engines: {node: 4.x || >=6.0.0}
     peerDependencies:
       encoding: ^0.1.0
     peerDependenciesMeta:
@@ -5005,26 +5127,29 @@
       semver: 5.7.1
       validate-npm-package-license: 3.0.4
     dev: true
 
   /normalize-path@3.0.0:
     resolution: {integrity: sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==}
     engines: {node: '>=0.10.0'}
-    dev: false
 
   /normalize-range@0.1.2:
     resolution: {integrity: sha512-bdok/XvKII3nUpklnV6P2hxtMNrCboOjAcyBuQnWEhO665FwrSNRxU+AqpsyvO6LgGYPspN+lu5CLtw4jPRKNA==}
     engines: {node: '>=0.10.0'}
     dev: false
 
   /npm-run-path@5.1.0:
     resolution: {integrity: sha512-sJOdmRGrY2sjNTRMbSvluQqg+8X7ZK61yvzBEIDhz4f8z1TZFYABsqjjCBd/0PUNE9M6QDgHJXQkGUEm7Q+l9Q==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
     dependencies:
       path-key: 4.0.0
+
+  /object-assign@4.1.1:
+    resolution: {integrity: sha512-rJgTQnkUnH1sFw8yT6VSU3zD3sWmu6sZhIseY8VX+GRu3P6F7Fu+JNDoXfklElbLJSnc3FUQHVe4cU5hj+BcUg==}
+    engines: {node: '>=0.10.0'}
     dev: false
 
   /object-hash@3.0.0:
     resolution: {integrity: sha512-RSn9F68PjH9HqtltsSnqYC1XXoWe9Bju5+213R98cNGttag9q9yAOTzdbsqvIa7aNm5WffBZFpWYr2aWrklWAw==}
     engines: {node: '>= 6'}
     dev: false
 
@@ -5053,22 +5178,20 @@
       wrappy: 1.0.2
 
   /onetime@5.1.2:
     resolution: {integrity: sha512-kbpaSSGJTWdAY5KPVeMOKXSrPtr8C8C7wodJbcsd51jRnmD+GZu8Y0VoU6Dm5Z4vWr0Ig/1NKuWRKf7j5aaYSg==}
     engines: {node: '>=6'}
     dependencies:
       mimic-fn: 2.1.0
-    dev: false
 
   /onetime@6.0.0:
     resolution: {integrity: sha512-1FlR+gjXK7X+AsAHso35MnyN5KqGwJRi/31ft6x0M194ht7S+rWAvd7PHss9xSKMzE0asv1pyIHaJYq+BbacAQ==}
     engines: {node: '>=12'}
     dependencies:
       mimic-fn: 4.0.0
-    dev: false
 
   /open@8.4.2:
     resolution: {integrity: sha512-7x81NCL719oNbsq/3mh+hVrAWmFuEYUqrq/Iw3kUzH8ReypT9QQ0BLoJS7/G9k6N81XjW4qHWtjWwe/9eLy1EQ==}
     engines: {node: '>=12'}
     dependencies:
       define-lazy-prop: 2.0.0
       is-docker: 2.2.1
@@ -5083,15 +5206,14 @@
       cli-cursor: 4.0.0
       cli-spinners: 2.7.0
       is-interactive: 2.0.0
       is-unicode-supported: 1.3.0
       log-symbols: 5.1.0
       strip-ansi: 7.0.1
       wcwidth: 1.0.1
-    dev: false
 
   /os-tmpdir@1.0.2:
     resolution: {integrity: sha512-D2FR03Vir7FIu45XBY20mTb+/ZSWB00sjU9jdQXt83gDrI4Ztz5Fs7/yy74g2N5SVQY4xY1qDr4rNddwYRVX0g==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /outdent@0.5.0:
@@ -5113,14 +5235,20 @@
 
   /p-limit@3.1.0:
     resolution: {integrity: sha512-TYOanM3wGwNGsZN2cVTYPArw454xnXj5qmWF1bEoAc4+cU/ol7GVh7odevjp1FNHduHc3KZMcFduxU5Xc6uJRQ==}
     engines: {node: '>=10'}
     dependencies:
       yocto-queue: 0.1.0
 
+  /p-limit@4.0.0:
+    resolution: {integrity: sha512-5b0R4txpzjPWVw/cXXUResoD4hb6U/x9BH08L7nw+GN1sezDzPdxeRvpc9c433fZhBan/wusjbCsqwqm4EIBIQ==}
+    engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
+    dependencies:
+      yocto-queue: 1.0.0
+
   /p-locate@3.0.0:
     resolution: {integrity: sha512-x+12w/To+4GFfgJhBEpiDcLozRJGegY+Ei7/z0tSLkMmxGZNybVMSfWj9aJn8Z5Fc7dBUNJOOVgPv2H7IwulSQ==}
     engines: {node: '>=6'}
     dependencies:
       p-limit: 2.3.0
     dev: false
 
@@ -5177,19 +5305,17 @@
 
   /parse-latin@5.0.1:
     resolution: {integrity: sha512-b/K8ExXaWC9t34kKeDV8kGXBkXZ1HCSAZRYE7HR14eA1GlXX5L8iWhs8USJNhQU9q5ci413jCKF0gOyovvyRBg==}
     dependencies:
       nlcst-to-string: 3.1.1
       unist-util-modify-children: 3.1.1
       unist-util-visit-children: 2.0.2
-    dev: false
 
   /parse5@6.0.1:
     resolution: {integrity: sha512-Ofn/CTFzRGTTxwpNEs9PP93gXShHcTq255nzRYSKe8AkVpZY7e1fpmTfOyoIvjP5HG7Z2ZM7VS9PPhQGW2pOpw==}
-    dev: false
 
   /path-browserify@1.0.1:
     resolution: {integrity: sha512-b7uo2UCUOYZcnF/3ID0lulOJi/bafxa1xPe7ZPsammBSpjSWQkjNxlt635YGS2MiR9GjvuXCtz2emr3jbsz98g==}
 
   /path-exists@3.0.0:
     resolution: {integrity: sha512-bpC7GYwiDYQ4wYLe+FA8lhRjhQCMcQGuSgGGqDkg/QerRWw9CmGRT0iSOVRSZJ29NMLZgIzqaljJ63oaL4NIJQ==}
     engines: {node: '>=4'}
@@ -5198,31 +5324,28 @@
   /path-exists@4.0.0:
     resolution: {integrity: sha512-ak9Qy5Q7jYb2Wwcey5Fpvg2KoAc/ZIhLSLOSBmRmygPsGwkVVt0fZa0qrtMz+m6tJTAHfZQ8FnmB4MG4LWy7/w==}
     engines: {node: '>=8'}
 
   /path-is-absolute@1.0.1:
     resolution: {integrity: sha512-AVbw3UJ2e9bq64vSaS9Am0fje1Pa8pbGqTTsmXfaIiMpnr5DlDhfJOuLj9Sf95ZPVDAUerDfEk88MPmPe7UCQg==}
     engines: {node: '>=0.10.0'}
-    dev: true
 
   /path-key@3.1.1:
     resolution: {integrity: sha512-ojmeN0qd+y0jszEtoY48r0Peq5dwMEkIlCOu6Q5f41lfkswXuKtYrhgoTpLnyIcHm24Uhqx+5Tqm2InSwLhE6Q==}
     engines: {node: '>=8'}
 
   /path-key@4.0.0:
     resolution: {integrity: sha512-haREypq7xkM7ErfgIyA0z+Bj4AGKlMSdlQE2jvJo6huWD1EdkKYV+G/T4nq0YEF2vgTT8kqMFKo1uHn950r4SQ==}
     engines: {node: '>=12'}
-    dev: false
 
   /path-parse@1.0.7:
     resolution: {integrity: sha512-LDJzPVEEEPR+y48z93A0Ed0yXb8pAByGWo/k5YYdYgpY2/2EsOsksJrq7lOHxryrVOn1ejG6oAp8ahvOIQD8sw==}
 
   /path-to-regexp@6.2.1:
     resolution: {integrity: sha512-JLyh7xT1kizaEvcaXOQwOc2/Yhw6KZOvPf1S8401UyLk86CU79LN3vl7ztXGm/pZ+YjoyAJ4rxmHwbkBXJX+yw==}
-    dev: false
 
   /path-type@4.0.0:
     resolution: {integrity: sha512-gDKb8aZMDeD/tZWs9P6+q0J9Mwkdl6xMV8TjnGP3qJVJ06bdMgkbBlLU8IdfOsIsFz2BW1rNVT3XuNEl8zPAvw==}
     engines: {node: '>=8'}
     dev: true
 
   /periscopic@3.1.0:
@@ -5245,80 +5368,68 @@
     engines: {node: '>=0.10.0'}
     dev: false
 
   /pify@4.0.1:
     resolution: {integrity: sha512-uB80kBFb/tfd68bVleG9T5GGsGPjJrLAUpR5PZIrhBnIaRTQRjqdJSsIKkOP6OAIFbj7GOrcudc5pNjZ+geV2g==}
     engines: {node: '>=6'}
 
+  /pirates@4.0.5:
+    resolution: {integrity: sha512-8V9+HQPupnaXMA23c5hvl69zXvTwTzyAYasnkb0Tts4XvO4CliqONMOnvlq26rkhLC3nWDFBJf73LU1e1VZLaQ==}
+    engines: {node: '>= 6'}
+    dev: false
+
   /pkg-dir@4.2.0:
     resolution: {integrity: sha512-HRDzbaKjC+AOWVXxAU/x54COGeIv9eb+6CkDSQoNTt4XyWoIJvuPsXizxu/Fr23EiekbtZwmh1IcIG/l/a10GQ==}
     engines: {node: '>=8'}
     dependencies:
       find-up: 4.1.0
 
   /pkg-up@3.1.0:
     resolution: {integrity: sha512-nDywThFk1i4BQK4twPQ6TA4RT8bDY96yeuCVBWL3ePARCiEKDRSrNGbFIgUJpLp+XeIR65v8ra7WuJOFUBtkMA==}
     engines: {node: '>=8'}
     dependencies:
       find-up: 3.0.0
     dev: false
 
-  /postcss-import@14.1.0(postcss@8.4.21):
-    resolution: {integrity: sha512-flwI+Vgm4SElObFVPpTIT7SU7R3qk2L7PyduMcokiaVKuWv9d/U+Gm/QAd8NDLuykTWTkcrjOeD2Pp1rMeBTGw==}
-    engines: {node: '>=10.0.0'}
+  /postcss-import@15.1.0(postcss@8.4.24):
+    resolution: {integrity: sha512-hpr+J05B2FVYUAXHeK1YyI267J/dDDhMU6B6civm8hSY1jYJnBXxzKDKDswzJmtLHryrjhnDjqqp/49t8FALew==}
+    engines: {node: '>=14.0.0'}
     peerDependencies:
       postcss: ^8.0.0
     dependencies:
-      postcss: 8.4.21
+      postcss: 8.4.24
       postcss-value-parser: 4.2.0
       read-cache: 1.0.0
-      resolve: 1.22.1
+      resolve: 1.22.2
     dev: false
 
-  /postcss-js@4.0.1(postcss@8.4.21):
+  /postcss-js@4.0.1(postcss@8.4.24):
     resolution: {integrity: sha512-dDLF8pEO191hJMtlHFPRa8xsizHaM82MLfNkUHdUtVEV3tgTp5oj+8qbEqYM57SLfc74KSbw//4SeJma2LRVIw==}
     engines: {node: ^12 || ^14 || >= 16}
     peerDependencies:
       postcss: ^8.4.21
     dependencies:
       camelcase-css: 2.0.1
-      postcss: 8.4.21
+      postcss: 8.4.24
     dev: false
 
-  /postcss-load-config@3.1.4(postcss@8.4.21):
-    resolution: {integrity: sha512-6DiM4E7v4coTE4uzA8U//WhtPwyhiim3eyjEMFCnUpzbrkK9wJHgKDT2mR+HbtSrd/NubVaYTOpSpjUl8NQeRg==}
-    engines: {node: '>= 10'}
-    peerDependencies:
-      postcss: '>=8.0.9'
-      ts-node: '>=9.0.0'
-    peerDependenciesMeta:
-      postcss:
-        optional: true
-      ts-node:
-        optional: true
-    dependencies:
-      lilconfig: 2.1.0
-      postcss: 8.4.21
-      yaml: 1.10.2
-    dev: false
-
-  /postcss-load-config@4.0.1(postcss@8.4.21):
+  /postcss-load-config@4.0.1(postcss@8.4.24):
     resolution: {integrity: sha512-vEJIc8RdiBRu3oRAI0ymerOn+7rPuMvRXslTvZUKZonDHFIczxztIyJ1urxM1x9JXEikvpWWTUUqal5j/8QgvA==}
     engines: {node: '>= 14'}
     peerDependencies:
       postcss: '>=8.0.9'
       ts-node: '>=9.0.0'
     peerDependenciesMeta:
       postcss:
         optional: true
       ts-node:
         optional: true
     dependencies:
       lilconfig: 2.1.0
-      postcss: 8.4.21
+      postcss: 8.4.24
       yaml: 2.2.1
     dev: false
 
   /postcss-modules-extract-imports@3.0.0(postcss@8.4.21):
     resolution: {integrity: sha512-bdHleFnP3kZ4NYDhuGlVK+CMrQ/pqUm8bx/oGL93K6gVwiclvX5x0n76fYMKuIGKzlABOy13zsvqjb0f92TEXw==}
     engines: {node: ^10 || ^12 || >= 14}
     peerDependencies:
@@ -5355,21 +5466,21 @@
     peerDependencies:
       postcss: ^8.1.0
     dependencies:
       icss-utils: 5.1.0(postcss@8.4.21)
       postcss: 8.4.21
     dev: true
 
-  /postcss-nested@6.0.0(postcss@8.4.21):
-    resolution: {integrity: sha512-0DkamqrPcmkBDsLn+vQDIrtkSbNkv5AD/M322ySo9kqFkCIYklym2xEmWkwo+Y3/qZo34tzEPNUw4y7yMCdv5w==}
+  /postcss-nested@6.0.1(postcss@8.4.24):
+    resolution: {integrity: sha512-mEp4xPMi5bSWiMbsgoPfcP74lsWLHkQbZc3sY+jWYd65CUwXrUaTp0fmNpa01ZcETKlIgUdFN/MpS2xZtqL9dQ==}
     engines: {node: '>=12.0'}
     peerDependencies:
       postcss: ^8.2.14
     dependencies:
-      postcss: 8.4.21
+      postcss: 8.4.24
       postcss-selector-parser: 6.0.11
     dev: false
 
   /postcss-selector-parser@6.0.11:
     resolution: {integrity: sha512-zbARubNdogI9j7WY4nQJBiNqQf3sLS3wCP4WfOidu+p28LofJqDH1tcXypGrcmMHhDk2t9wGhCsYe/+szLTy1g==}
     engines: {node: '>=4'}
     dependencies:
@@ -5382,14 +5493,23 @@
   /postcss@8.4.21:
     resolution: {integrity: sha512-tP7u/Sn/dVxK2NnruI4H9BG+x+Wxz6oeZ1cJ8P6G/PZY0IKk4k/63TDsQf2kQq3+qoJeLm2kIBUNlZe3zgb4Zg==}
     engines: {node: ^10 || ^12 || >=14}
     dependencies:
       nanoid: 3.3.4
       picocolors: 1.0.0
       source-map-js: 1.0.2
+    dev: true
+
+  /postcss@8.4.24:
+    resolution: {integrity: sha512-M0RzbcI0sO/XJNucsGjvWU9ERWxb/ytp1w6dKtxTKgixdtQDq4rmx/g8W1hnaheq9jgwL/oyEdH5Bc4WwJKMqg==}
+    engines: {node: ^10 || ^12 || >=14}
+    dependencies:
+      nanoid: 3.3.6
+      picocolors: 1.0.0
+      source-map-js: 1.0.2
 
   /preact-render-to-string@5.2.6(preact@10.13.0):
     resolution: {integrity: sha512-JyhErpYOvBV1hEPwIxc/fHWXPfnEGdRKxc8gFdAZ7XV4tlzyzG847XAyEZqoDnynP88akM4eaHcSOzNcLWFguw==}
     peerDependencies:
       preact: '>=10'
     dependencies:
       preact: 10.13.0
@@ -5413,28 +5533,43 @@
     resolution: {integrity: sha512-mmifnkG160BtC727gqoimoxnZT/dwr8ASxpoGGl6EHevhfblSOeu+pwH1LAm5Qu1MynizktztFujHHaijLCkww==}
     engines: {node: ^14.15.0 || >=16.0.0, pnpm: '>=7.14.0'}
     dependencies:
       '@astrojs/compiler': 0.31.4
       prettier: 2.8.4
       sass-formatter: 0.7.6
       synckit: 0.8.5
+    dev: true
+
+  /prettier-plugin-astro@0.9.1:
+    resolution: {integrity: sha512-pYZXSbdq0eElvzoIMArzv1SBn1NUXzopjlcnt6Ql8VW32PjC12NovwBjXJ6rh8qQLi7vF8jNqAbraKW03UPfag==}
+    engines: {node: ^14.15.0 || >=16.0.0, pnpm: '>=7.14.0'}
+    dependencies:
+      '@astrojs/compiler': 1.5.0
+      prettier: 2.8.8
+      sass-formatter: 0.7.6
+      synckit: 0.8.5
 
   /prettier@2.8.4:
     resolution: {integrity: sha512-vIS4Rlc2FNh0BySk3Wkd6xmwxB0FpOndW5fisM5H8hsZSxU2VWVB5CWIkIjWvrHjIhxk2g3bfMKM87zNTrZddw==}
     engines: {node: '>=10.13.0'}
     hasBin: true
+    dev: true
+
+  /prettier@2.8.8:
+    resolution: {integrity: sha512-tdN8qQGvNjw4CHbY+XXk0JgCXn9QiF21a55rBe5LJAU+kDyC4WQn4+awm2Xfk2lQMk5fKup9XgzTZtGkjBdP9Q==}
+    engines: {node: '>=10.13.0'}
+    hasBin: true
 
   /pretty-format@3.8.0:
     resolution: {integrity: sha512-WuxUnVtlWL1OfZFQFuqvnvs6MiAGk9UNsBostyBOB0Is9wb5uRESevA6rnl/rkksXaGX3GzZhPup5d6Vp1nFew==}
     dev: false
 
   /prismjs@1.29.0:
     resolution: {integrity: sha512-Kx/1w86q/epKcmte75LNrEoT+lX8pBpavuAbvJWRXar7Hz8jrtF+e3vY751p0R8H9HdArwaCTNDDzHg/ScJK1Q==}
     engines: {node: '>=6'}
-    dev: false
 
   /process@0.11.10:
     resolution: {integrity: sha512-cdGef/drWFoydD1JsMzuFf8100nZl+GT+yacc2bEced5f9Rjk4z+WtFUTBu9PhOi9j/jfmBPu0mMEY4wIdAF8A==}
     engines: {node: '>= 0.6.0'}
     dev: true
 
   /promise-inflight@1.0.1:
@@ -5448,19 +5583,17 @@
 
   /prompts@2.4.2:
     resolution: {integrity: sha512-NxNv/kLguCA7p3jE8oL2aEBsrJWgAakBpgmgK6lpPWV+WuOmY6r2/zbAVnP+T8bQlA0nzHXSJSJW0Hq7ylaD2Q==}
     engines: {node: '>= 6'}
     dependencies:
       kleur: 3.0.3
       sisteransi: 1.0.5
-    dev: false
 
   /property-information@6.2.0:
     resolution: {integrity: sha512-kma4U7AFCTwpqq5twzC1YVIDXSqg6qQK6JN0smOw8fgRy1OkMi0CYSzFmsy6dnqSenamAtj0CyXMUJ1Mf6oROg==}
-    dev: false
 
   /pseudomap@1.0.2:
     resolution: {integrity: sha512-b/YwNhb8lk1Zz2+bXXpS/LK9OisiZZ1SNsSLxN1x2OXVEhW2Ckr/7mWE5vrC1ZTiJlD9g19jWszTmJsB+oEpFQ==}
     dev: true
 
   /punycode@2.3.0:
     resolution: {integrity: sha512-rRV+zQD8tVFys26lAGR9WUuS4iUAngJScM+ZRSKtvl5tKeZ2t5bvdNFdNHBW9FWR4guGHlgmsZ1G7BSm2wTbuA==}
@@ -5469,30 +5602,19 @@
   /querystringify@2.2.0:
     resolution: {integrity: sha512-FIqgj2EUvTa7R50u0rGsyTftzjYmv/a3hO345bZNrqabNqjtgiDMgmo4mkUjd+nzU5oF3dClKqFIPUKybUyqoQ==}
     dev: false
 
   /queue-microtask@1.2.3:
     resolution: {integrity: sha512-NuaNSa6flKT5JaSYQzJok04JzTL1CA6aGhv5rfLW3PgqA+M2ChpZQnAC8h8i4ZFkBS8X5RqkDBHA7r4hej3K9A==}
 
-  /queue@6.0.2:
-    resolution: {integrity: sha512-iHZWu+q3IdFZFX36ro/lKBkSvfkztY5Y7HMiPlOUjhupPcG2JMfst2KKEpu5XndviX/3UhFbRngUPNKtgvtZiA==}
-    dependencies:
-      inherits: 2.0.4
-    dev: false
-
   /quick-lru@4.0.1:
     resolution: {integrity: sha512-ARhCpm70fzdcvNQfPoy49IaanKkTlRWF2JMzqhcJbhSFRZv7nPTvZJdcY7301IPmvW+/p0RgIWnQDLJxifsQ7g==}
     engines: {node: '>=8'}
     dev: true
 
-  /quick-lru@5.1.1:
-    resolution: {integrity: sha512-WuyALRjWPDGtt/wzJiadO5AXY+8hZ80hVpe6MyivgraREW751X3SbhRvG3eLKOYN+8VEvqLcf3wdnt44Z4S4SA==}
-    engines: {node: '>=10'}
-    dev: false
-
   /randombytes@2.1.0:
     resolution: {integrity: sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==}
     dependencies:
       safe-buffer: 5.2.1
     dev: true
 
   /raw-loader@4.0.2(webpack@5.76.0):
@@ -5561,22 +5683,20 @@
   /readable-stream@3.6.1:
     resolution: {integrity: sha512-+rQmrWMYGA90yenhTYsLWAsLsqVC8osOw6PKE1HDYiO0gdPeKe/xDHNzIAIn4C91YQ6oenEhfYqqc1883qHbjQ==}
     engines: {node: '>= 6'}
     dependencies:
       inherits: 2.0.4
       string_decoder: 1.3.0
       util-deprecate: 1.0.2
-    dev: false
 
   /readdirp@3.6.0:
     resolution: {integrity: sha512-hOS089on8RduqdbhvQ5Z37A0ESjsqz6qnRcffsMU3495FuTdqSm+7bhJ29JvIOsBDEEnan5DPu9t3To9VRlMzA==}
     engines: {node: '>=8.10.0'}
     dependencies:
       picomatch: 2.3.1
-    dev: false
 
   /rechoir@0.7.1:
     resolution: {integrity: sha512-/njmZ8s1wVeR6pjTZ+0nCnv8SpZNRMT2D1RLOJQESlYFDBvwpTA4KWJpZ+sBJ4+vhjILRcK7JIFdGCdxEAAitg==}
     engines: {node: '>= 0.10'}
     dependencies:
       resolve: 1.22.1
     dev: true
@@ -5605,40 +5725,36 @@
   /rehype-parse@8.0.4:
     resolution: {integrity: sha512-MJJKONunHjoTh4kc3dsM1v3C9kGrrxvA3U8PxZlP2SjH8RNUSrb+lF7Y0KVaUDnGH2QZ5vAn7ulkiajM9ifuqg==}
     dependencies:
       '@types/hast': 2.3.4
       hast-util-from-parse5: 7.1.2
       parse5: 6.0.1
       unified: 10.1.2
-    dev: false
 
   /rehype-raw@6.1.1:
     resolution: {integrity: sha512-d6AKtisSRtDRX4aSPsJGTfnzrX2ZkHQLE5kiUuGOeEoLpbEulFF4hj0mLPbsa+7vmguDKOVVEQdHKDSwoaIDsQ==}
     dependencies:
       '@types/hast': 2.3.4
       hast-util-raw: 7.2.3
       unified: 10.1.2
-    dev: false
 
   /rehype-stringify@9.0.3:
     resolution: {integrity: sha512-kWiZ1bgyWlgOxpqD5HnxShKAdXtb2IUljn3hQAhySeak6IOQPPt6DeGnsIh4ixm7yKJWzm8TXFuC/lPfcWHJqw==}
     dependencies:
       '@types/hast': 2.3.4
       hast-util-to-html: 8.0.4
       unified: 10.1.2
-    dev: false
 
   /rehype@12.0.1:
     resolution: {integrity: sha512-ey6kAqwLM3X6QnMDILJthGvG1m1ULROS9NT4uG9IDCuv08SFyLlreSuvOa//DgEvbXx62DS6elGVqusWhRUbgw==}
     dependencies:
       '@types/hast': 2.3.4
       rehype-parse: 8.0.4
       rehype-stringify: 9.0.3
       unified: 10.1.2
-    dev: false
 
   /remark-frontmatter@4.0.1:
     resolution: {integrity: sha512-38fJrB0KnmD3E33a5jZC/5+gGAC2WKNiPw1/fdXJvijBlhA7RCsvJklrYJakS0HedninvaCYW8lQGf9C918GfA==}
     dependencies:
       '@types/mdast': 3.0.10
       mdast-util-frontmatter: 1.0.1
       micromark-extension-frontmatter: 1.0.1
@@ -5650,15 +5766,14 @@
     dependencies:
       '@types/mdast': 3.0.10
       mdast-util-gfm: 2.0.2
       micromark-extension-gfm: 2.0.1
       unified: 10.1.2
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
   /remark-mdx@2.3.0:
     resolution: {integrity: sha512-g53hMkpM0I98MU266IzDFMrTD980gNF3BJnkyFcmN+dD873mQeD5rdMO3Y2X+x8umQfbSE0PcoEDl7ledSA+2g==}
     dependencies:
       mdast-util-mdx: 2.0.1
       micromark-extension-mdxjs: 1.0.0
     transitivePeerDependencies:
@@ -5669,33 +5784,30 @@
     resolution: {integrity: sha512-1fUyHr2jLsVOkhbvPRBJ5zTKZZyD6yZzYaWCS6BPBdQ8vEMBCH+9zNCDA6tET/zHCi/jLqjCWtlJZUPk+DbnFw==}
     dependencies:
       '@types/mdast': 3.0.10
       mdast-util-from-markdown: 1.3.0
       unified: 10.1.2
     transitivePeerDependencies:
       - supports-color
-    dev: false
 
   /remark-rehype@10.1.0:
     resolution: {integrity: sha512-EFmR5zppdBp0WQeDVZ/b66CWJipB2q2VLNFMabzDSGR66Z2fQii83G5gTBbgGEnEEA0QRussvrFHxk1HWGJskw==}
     dependencies:
       '@types/hast': 2.3.4
       '@types/mdast': 3.0.10
       mdast-util-to-hast: 12.3.0
       unified: 10.1.2
-    dev: false
 
   /remark-smartypants@2.0.0:
     resolution: {integrity: sha512-Rc0VDmr/yhnMQIz8n2ACYXlfw/P/XZev884QU1I5u+5DgJls32o97Vc1RbK3pfumLsJomS2yy8eT4Fxj/2MDVA==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
     dependencies:
       retext: 8.1.0
       retext-smartypants: 5.2.0
       unist-util-visit: 4.1.2
-    dev: false
 
   /require-directory@2.1.1:
     resolution: {integrity: sha512-fGxEI7+wsG9xrvdjsrlmL22OMTTiHRwAMroiEeMgq8gzoLC/PQr7RsRDSTLUg/bZAZtF+TVIkHc6/4RIKrui+Q==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /require-main-filename@2.0.0:
@@ -5726,56 +5838,60 @@
     resolution: {integrity: sha512-nBpuuYuY5jFsli/JIs1oldw6fOQCBioohqWZg/2hiaOybXOft4lonv85uDOKXdf8rhyK159cxU5cDcK/NKk8zw==}
     hasBin: true
     dependencies:
       is-core-module: 2.11.0
       path-parse: 1.0.7
       supports-preserve-symlinks-flag: 1.0.0
 
+  /resolve@1.22.2:
+    resolution: {integrity: sha512-Sb+mjNHOULsBv818T40qSPeRiuWLyaGMa5ewydRLFimneixmVy2zdivRl+AF6jaYPC8ERxGDmFSiqui6SfPd+g==}
+    hasBin: true
+    dependencies:
+      is-core-module: 2.11.0
+      path-parse: 1.0.7
+      supports-preserve-symlinks-flag: 1.0.0
+    dev: false
+
   /restore-cursor@4.0.0:
     resolution: {integrity: sha512-I9fPXU9geO9bHOt9pHHOhOkYerIMsmVaWB0rA2AI9ERh/+x/i7MV5HKBNrg+ljO5eoPVgCcnFuRjJ9uH6I/3eg==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
     dependencies:
       onetime: 5.1.2
       signal-exit: 3.0.7
-    dev: false
 
   /retext-latin@3.1.0:
     resolution: {integrity: sha512-5MrD1tuebzO8ppsja5eEu+ZbBeUNCjoEarn70tkXOS7Bdsdf6tNahsv2bY0Z8VooFF6cw7/6S+d3yI/TMlMVVQ==}
     dependencies:
       '@types/nlcst': 1.0.0
       parse-latin: 5.0.1
       unherit: 3.0.1
       unified: 10.1.2
-    dev: false
 
   /retext-smartypants@5.2.0:
     resolution: {integrity: sha512-Do8oM+SsjrbzT2UNIKgheP0hgUQTDDQYyZaIY3kfq0pdFzoPk+ZClYJ+OERNXveog4xf1pZL4PfRxNoVL7a/jw==}
     dependencies:
       '@types/nlcst': 1.0.0
       nlcst-to-string: 3.1.1
       unified: 10.1.2
       unist-util-visit: 4.1.2
-    dev: false
 
   /retext-stringify@3.1.0:
     resolution: {integrity: sha512-767TLOaoXFXyOnjx/EggXlb37ZD2u4P1n0GJqVdpipqACsQP+20W+BNpMYrlJkq7hxffnFk+jc6mAK9qrbuB8w==}
     dependencies:
       '@types/nlcst': 1.0.0
       nlcst-to-string: 3.1.1
       unified: 10.1.2
-    dev: false
 
   /retext@8.1.0:
     resolution: {integrity: sha512-N9/Kq7YTn6ZpzfiGW45WfEGJqFf1IM1q8OsRa1CGzIebCJBNCANDRmOrholiDRGKo/We7ofKR4SEvcGAWEMD3Q==}
     dependencies:
       '@types/nlcst': 1.0.0
       retext-latin: 3.1.0
       retext-stringify: 3.1.0
       unified: 10.1.2
-    dev: false
 
   /reusify@1.0.4:
     resolution: {integrity: sha512-U9nH88a3fc/ekCF1l0/UP1IosiuIjyTh7hBvXVMHYgVcfGvt897Xguj2UOLDeI5BG2m7/uwyaLVT6fbtCwTyzw==}
     engines: {iojs: '>=1.0.0', node: '>=0.10.0'}
 
   /rimraf@3.0.2:
     resolution: {integrity: sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==}
@@ -5786,29 +5902,36 @@
 
   /rollup@3.18.0:
     resolution: {integrity: sha512-J8C6VfEBjkvYPESMQYxKHxNOh4A5a3FlP+0BETGo34HEcE4eTlgCrO2+eWzlu2a/sHs2QUkZco+wscH7jhhgWg==}
     engines: {node: '>=14.18.0', npm: '>=8.0.0'}
     hasBin: true
     optionalDependencies:
       fsevents: 2.3.2
+    dev: true
+
+  /rollup@3.23.1:
+    resolution: {integrity: sha512-ybRdFVHOoljGEFILHLd2g/qateqUdjE6YS41WXq4p3C/WwD3xtWxV4FYWETA1u9TeXQc5K8L8zHE5d/scOvrOQ==}
+    engines: {node: '>=14.18.0', npm: '>=8.0.0'}
+    hasBin: true
+    optionalDependencies:
+      fsevents: 2.3.2
 
   /run-parallel@1.2.0:
     resolution: {integrity: sha512-5l4VyZR86LZ/lDxZTR6jqL8AFE2S0IFLMP26AbjsLVADxHdhB/c0GUsH+y39UfCi3dzz8OlQuPmnaJOMoDHQBA==}
     dependencies:
       queue-microtask: 1.2.3
 
   /s.color@0.0.15:
     resolution: {integrity: sha512-AUNrbEUHeKY8XsYr/DYpl+qk5+aM+DChopnWOPEzn8YKzOhv4l2zH6LzZms3tOZP3wwdOyc0RmTciyi46HLIuA==}
 
   /sade@1.8.1:
     resolution: {integrity: sha512-xal3CZX1Xlo/k4ApwCFrHVACi9fBqJ7V+mwhBsuf/1IOKbBy098Fex+Wa/5QMubw09pSZ/u8EY8PWgevJsXp1A==}
     engines: {node: '>=6'}
     dependencies:
       mri: 1.2.0
-    dev: false
 
   /safe-buffer@5.2.1:
     resolution: {integrity: sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==}
 
   /safe-regex-test@1.0.0:
     resolution: {integrity: sha512-JBUUzyOgEwXQY1NuPtvcj/qcBDbDmEvWufhlnXZIm75DEHp+afM1r1ujJpJsV/gSM4t59tpDyPi1sd6ZaPFfsA==}
     dependencies:
@@ -5852,15 +5975,14 @@
 
   /section-matter@1.0.0:
     resolution: {integrity: sha512-vfD3pmTzGpufjScBh50YHKzEu2lxBWhVEHsNGoEXmCmn2hKGfeNLYMzCJpe8cD7gqX7TJluOVpBkAequ6dgMmA==}
     engines: {node: '>=4'}
     dependencies:
       extend-shallow: 2.0.1
       kind-of: 6.0.3
-    dev: false
 
   /semver@5.7.1:
     resolution: {integrity: sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==}
     hasBin: true
     dev: true
 
   /semver@6.3.0:
@@ -5884,15 +6006,14 @@
     resolution: {integrity: sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==}
     dependencies:
       randombytes: 2.1.0
     dev: true
 
   /server-destroy@1.0.1:
     resolution: {integrity: sha512-rb+9B5YBIEzYcD6x2VKidaa+cqYBJQKnU4oe4E3ANwRRN56yk/ua1YCJT1n21NTS8w6CcOclAKNP3PhdCXKYtQ==}
-    dev: false
 
   /set-blocking@2.0.0:
     resolution: {integrity: sha512-KiKBS8AnWGEyLzofFfmvKwpdPzqiy16LvQfK3yv/fVH7Bj13/wl3JSR1J+rfgRE9q7xUJK4qvgS8raSOeLUehw==}
     dev: true
 
   /shallow-clone@3.0.1:
     resolution: {integrity: sha512-/6KqX+GVUdqPuPPd2LxDDxzX6CAbjJehAAOKlNpqqUpAqPM6HeL8f+o3a+JsyGjn2lv0WY8UsTgUJjU9Ok55NA==}
@@ -5919,55 +6040,44 @@
     engines: {node: '>=0.10.0'}
     dev: true
 
   /shebang-regex@3.0.0:
     resolution: {integrity: sha512-7++dFhtcx3353uBaq8DDR4NuxBetBzC7ZQOhmTQInHEd6bSrXdiEyzCvG07Z44UYdLShWUyXt5M/yhz8ekcb1A==}
     engines: {node: '>=8'}
 
-  /shiki@0.11.1:
-    resolution: {integrity: sha512-EugY9VASFuDqOexOgXR18ZV+TbFrQHeCpEYaXamO+SZlsnT/2LxuLBX25GGtIrwaEVFXUAbUQ601SWE2rMwWHA==}
-    dependencies:
-      jsonc-parser: 3.2.0
-      vscode-oniguruma: 1.7.0
-      vscode-textmate: 6.0.0
-    dev: false
-
   /shiki@0.14.1:
     resolution: {integrity: sha512-+Jz4nBkCBe0mEDqo1eKRcCdjRtrCjozmcbTUjbPTX7OOJfEbTZzlUWlZtGe3Gb5oV1/jnojhG//YZc3rs9zSEw==}
     dependencies:
       ansi-sequence-parser: 1.1.0
       jsonc-parser: 3.2.0
       vscode-oniguruma: 1.7.0
       vscode-textmate: 8.0.0
-    dev: true
 
   /side-channel@1.0.4:
     resolution: {integrity: sha512-q5XPytqFEIKHkGdiMIrY10mvLRvnQh42/+GoBlFW3b2LXLE2xxJpZFdm94we0BaoV3RwJyGqg5wS7epxTv0Zvw==}
     dependencies:
       call-bind: 1.0.2
       get-intrinsic: 1.2.0
       object-inspect: 1.12.3
     dev: true
 
   /signal-exit@3.0.7:
     resolution: {integrity: sha512-wnD2ZE+l+SPC/uoS0vXeE9L1+0wuaMqKlfz9AMUo38JsyLSBWSFcHR1Rri62LZc12vLr1gb3jl7iwQhgwpAbGQ==}
 
   /sisteransi@1.0.5:
     resolution: {integrity: sha512-bLGGlR1QxBcynn2d5YmDX4MGjlZvy2MRBDRNHLJ8VI6l6+9FUiyTFNJ0IveOSP0bcXgVDPRcfGqA0pjaqUpfVg==}
-    dev: false
 
   /slash@3.0.0:
     resolution: {integrity: sha512-g9Q1haeby36OSStwb4ntCGGGaKsaVSjQ68fBxoQcutl5fS1vuY18H3wSt3jFyFtrkx+Kz0V1G85A4MyAdDMi2Q==}
     engines: {node: '>=8'}
     dev: true
 
   /slash@4.0.0:
     resolution: {integrity: sha512-3dOsAHXXUkQTpOYcoAxLIorMTp4gIQr5IW3iVb7A7lFIp0VHhnynm9izx6TssdrIcVIESAlVjtnO2K8bg+Coew==}
     engines: {node: '>=12'}
-    dev: false
 
   /smartwrap@2.0.2:
     resolution: {integrity: sha512-vCsKNQxb7PnCNd2wY1WClWifAc2lwqsG8OaswpJkVJsvMGcnEntdTCDajZCkk93Ay1U3t/9puJmb525Rg5MZBA==}
     engines: {node: '>=6'}
     hasBin: true
     dependencies:
       array.prototype.flat: 1.3.1
@@ -6015,15 +6125,14 @@
   /source-map@0.7.4:
     resolution: {integrity: sha512-l3BikUxvPOcn5E74dZiq5BGsTb5yEwhaTSzccU6t4sDOH8NWJCstKO5QT2CvtFoK6F0saL7p9xHAqHOlCPJygA==}
     engines: {node: '>= 8'}
     dev: false
 
   /space-separated-tokens@2.0.2:
     resolution: {integrity: sha512-PEGlAwrG8yXGXRjW32fGbg66JAlOAwbObuqVoJpv/mRgoWDQfgH1wDPvtzWyUSNAXBGSk8h755YDbbcEy3SH2Q==}
-    dev: false
 
   /spawndamnit@2.0.0:
     resolution: {integrity: sha512-j4JKEcncSjFlqIwU5L/rp2N5SIPsdxaRsIv678+TZxZ0SRDJTm8JrxJMjE/XuiEZNEir3S8l0Fa3Ke339WI4qA==}
     dependencies:
       cross-spawn: 5.1.0
       signal-exit: 3.0.7
     dev: true
@@ -6065,15 +6174,14 @@
     dependencies:
       mixme: 0.5.5
     dev: true
 
   /streamsearch@1.1.0:
     resolution: {integrity: sha512-Mcc5wHehp9aXz1ax6bZUyY5afg9u2rv5cqQI3mRrYkGC8rW2hM02jWuwjtL++LS5qinSyhj2QfLyNsuc+VsExg==}
     engines: {node: '>=10.0.0'}
-    dev: false
 
   /string-width@4.2.3:
     resolution: {integrity: sha512-wKyQRQpjJ0sIp62ErSZdGsjMJWsap5oRNihHhu6G7JVO/9jIB6UyevL+tXuOqrng8j/cxKTWyWUwvSTriiZz/g==}
     engines: {node: '>=8'}
     dependencies:
       emoji-regex: 8.0.0
       is-fullwidth-code-point: 3.0.0
@@ -6082,15 +6190,14 @@
   /string-width@5.1.2:
     resolution: {integrity: sha512-HnLOCR3vjcY8beoNLtcjZ5/nxn2afmME6lhrDrebokqMap+XbeW8n9TXpPDOqdGK5qcI3oT0GKTW6wC7EMiVqA==}
     engines: {node: '>=12'}
     dependencies:
       eastasianwidth: 0.2.0
       emoji-regex: 9.2.2
       strip-ansi: 7.0.1
-    dev: false
 
   /string.prototype.trimend@1.0.6:
     resolution: {integrity: sha512-JySq+4mrPf9EsDBEDYMOb/lM7XQLulwg5R/m1r0PXEFqrV0qHvl58sdTilSXtKOflCsK2E8jxf+GKC0T07RWwQ==}
     dependencies:
       call-bind: 1.0.2
       define-properties: 1.2.0
       es-abstract: 1.21.1
@@ -6104,54 +6211,48 @@
       es-abstract: 1.21.1
     dev: true
 
   /string_decoder@1.3.0:
     resolution: {integrity: sha512-hkRX8U1WjJFd8LsDJ2yQ/wWWxaopEsABU1XfkM8A+j0+85JAGppt16cr1Whg6KIbb4okU6Mql6BOj+uup/wKeA==}
     dependencies:
       safe-buffer: 5.2.1
-    dev: false
 
   /stringify-entities@4.0.3:
     resolution: {integrity: sha512-BP9nNHMhhfcMbiuQKCqMjhDP5yBCAxsPu4pHFFzJ6Alo9dZgY4VLDPutXqIjpRiMoKdp7Av85Gr73Q5uH9k7+g==}
     dependencies:
       character-entities-html4: 2.1.0
       character-entities-legacy: 3.0.0
-    dev: false
 
   /strip-ansi@6.0.1:
     resolution: {integrity: sha512-Y38VPSHcqkFrCpFnQ9vuSXmquuv5oXOKpGeT6aGrr3o3Gc9AlVa6JBfUSOCnbxGGZF+/0ooI7KrPuUSztUdU5A==}
     engines: {node: '>=8'}
     dependencies:
       ansi-regex: 5.0.1
 
   /strip-ansi@7.0.1:
     resolution: {integrity: sha512-cXNxvT8dFNRVfhVME3JAe98mkXDYN2O1l7jmcwMnOslDeESg1rF/OZMtK0nRAhiari1unG5cD4jG3rapUAkLbw==}
     engines: {node: '>=12'}
     dependencies:
       ansi-regex: 6.0.1
-    dev: false
 
   /strip-bom-string@1.0.0:
     resolution: {integrity: sha512-uCC2VHvQRYu+lMh4My/sFNmF2klFymLX1wHJeXnbEJERpV/ZsVuonzerjfrGpIGF7LBVa1O7i9kjiWvJiFck8g==}
     engines: {node: '>=0.10.0'}
-    dev: false
 
   /strip-bom@3.0.0:
     resolution: {integrity: sha512-vavAMRXOgBVNF6nyEEmL3DBK19iRpDcoIwW+swQ+CbGiu7lju6t+JklA1MHweoWtadgt4ISVUsXLyDq34ddcwA==}
     engines: {node: '>=4'}
 
   /strip-bom@4.0.0:
     resolution: {integrity: sha512-3xurFv5tEgii33Zi8Jtp55wEIILR9eh34FAW00PZf+JnSsTmV/ioewSgQl97JHvgjoRGwPShsWm+IdrxB35d0w==}
     engines: {node: '>=8'}
-    dev: false
 
   /strip-final-newline@3.0.0:
     resolution: {integrity: sha512-dOESqjYr96iWYylGObzd39EuNTa5VJxyvVAEm5Jnh7KGo75V43Hk1odPQkNDyXNmUR6k+gEiDVXnjB8HJ3crXw==}
     engines: {node: '>=12'}
-    dev: false
 
   /strip-indent@3.0.0:
     resolution: {integrity: sha512-laJTa3Jb+VQpaC6DseHhF7dXVqHTfJPCRDaEbid/drOhgitgYku/letMUqOXFoWV0zIIUbjpdH2t+tYj4bQMRQ==}
     engines: {node: '>=8'}
     dependencies:
       min-indent: 1.0.1
     dev: true
@@ -6169,14 +6270,28 @@
 
   /style-to-object@0.4.1:
     resolution: {integrity: sha512-HFpbb5gr2ypci7Qw+IOhnP2zOU7e77b+rzM+wTzXzfi1PrtBCX0E7Pk4wL4iTLnhzZ+JgEGAhX81ebTg/aYjQw==}
     dependencies:
       inline-style-parser: 0.1.1
     dev: false
 
+  /sucrase@3.32.0:
+    resolution: {integrity: sha512-ydQOU34rpSyj2TGyz4D2p8rbktIOZ8QY9s+DGLvFU1i5pWJE8vkpruCjGCMHsdXwnD7JDcS+noSwM/a7zyNFDQ==}
+    engines: {node: '>=8'}
+    hasBin: true
+    dependencies:
+      '@jridgewell/gen-mapping': 0.3.2
+      commander: 4.1.1
+      glob: 7.1.6
+      lines-and-columns: 1.2.4
+      mz: 2.7.0
+      pirates: 4.0.5
+      ts-interface-checker: 0.1.13
+    dev: false
+
   /suf-log@2.5.3:
     resolution: {integrity: sha512-KvC8OPjzdNOe+xQ4XWJV2whQA0aM1kGVczMQ8+dStAO6KfEB140JEVQ9dE76ONZ0/Ylf67ni4tILPJB41U0eow==}
     dependencies:
       s.color: 0.0.15
 
   /supports-color@5.5.0:
     resolution: {integrity: sha512-QjVjwdXIt408MIiAqCX4oUKsgU2EqAGzs2Ppkm4aQYbjm+ZEWEcW4SfFNTr4uMNZma0ey4f5lgLrkB0aX0QMow==}
@@ -6197,15 +6312,14 @@
       has-flag: 4.0.0
     dev: true
 
   /supports-esm@1.0.0:
     resolution: {integrity: sha512-96Am8CDqUaC0I2+C/swJ0yEvM8ZnGn4unoers/LSdE4umhX7mELzqyLzx3HnZAluq5PXIsGMKqa7NkqaeHMPcg==}
     dependencies:
       has-package-exports: 1.3.0
-    dev: false
 
   /supports-preserve-symlinks-flag@1.0.0:
     resolution: {integrity: sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==}
     engines: {node: '>= 0.4'}
 
   /svg-url-loader@6.0.0(webpack@5.76.0):
     resolution: {integrity: sha512-Qr5SCKxyxKcRnvnVrO3iQj9EX/v40UiGEMshgegzV7vpo3yc+HexELOdtWcA3MKjL8IyZZ1zOdcILmDEa/8JJQ==}
@@ -6220,44 +6334,42 @@
   /synckit@0.8.5:
     resolution: {integrity: sha512-L1dapNV6vu2s/4Sputv8xGsCdAVlb5nRDMFU/E27D44l5U6cw1g0dGd45uLc+OXjNMmF4ntiMdCimzcjFKQI8Q==}
     engines: {node: ^14.18.0 || >=16.0.0}
     dependencies:
       '@pkgr/utils': 2.3.1
       tslib: 2.5.0
 
-  /tailwindcss@3.2.7(postcss@8.4.21):
-    resolution: {integrity: sha512-B6DLqJzc21x7wntlH/GsZwEXTBttVSl1FtCzC8WP4oBc/NKef7kaax5jeihkkCEWc831/5NDJ9gRNDK6NEioQQ==}
-    engines: {node: '>=12.13.0'}
+  /tailwindcss@3.3.2:
+    resolution: {integrity: sha512-9jPkMiIBXvPc2KywkraqsUfbfj+dHDb+JPWtSJa9MLFdrPyazI7q6WX2sUrm7R9eVR7qqv3Pas7EvQFzxKnI6w==}
+    engines: {node: '>=14.0.0'}
     hasBin: true
-    peerDependencies:
-      postcss: ^8.0.9
     dependencies:
+      '@alloc/quick-lru': 5.2.0
       arg: 5.0.2
       chokidar: 3.5.3
-      color-name: 1.1.4
-      detective: 5.2.1
       didyoumean: 1.2.2
       dlv: 1.1.3
       fast-glob: 3.2.12
       glob-parent: 6.0.2
       is-glob: 4.0.3
+      jiti: 1.18.2
       lilconfig: 2.1.0
       micromatch: 4.0.5
       normalize-path: 3.0.0
       object-hash: 3.0.0
       picocolors: 1.0.0
-      postcss: 8.4.21
-      postcss-import: 14.1.0(postcss@8.4.21)
-      postcss-js: 4.0.1(postcss@8.4.21)
-      postcss-load-config: 3.1.4(postcss@8.4.21)
-      postcss-nested: 6.0.0(postcss@8.4.21)
+      postcss: 8.4.24
+      postcss-import: 15.1.0(postcss@8.4.24)
+      postcss-js: 4.0.1(postcss@8.4.24)
+      postcss-load-config: 4.0.1(postcss@8.4.24)
+      postcss-nested: 6.0.1(postcss@8.4.24)
       postcss-selector-parser: 6.0.11
       postcss-value-parser: 4.2.0
-      quick-lru: 5.1.1
-      resolve: 1.22.1
+      resolve: 1.22.2
+      sucrase: 3.32.0
     transitivePeerDependencies:
       - ts-node
     dev: false
 
   /tapable@2.2.1:
     resolution: {integrity: sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==}
     engines: {node: '>=6'}
@@ -6332,14 +6444,27 @@
     dependencies:
       '@jridgewell/source-map': 0.3.2
       acorn: 8.8.2
       commander: 2.20.3
       source-map-support: 0.5.21
     dev: true
 
+  /thenify-all@1.6.0:
+    resolution: {integrity: sha512-RNxQH/qI8/t3thXJDwcstUO4zeqo64+Uy/+sNVRBx4Xn2OX+OZ9oP+iJnNFqplFra2ZUVeKCSa2oVWi3T4uVmA==}
+    engines: {node: '>=0.8'}
+    dependencies:
+      thenify: 3.3.1
+    dev: false
+
+  /thenify@3.3.1:
+    resolution: {integrity: sha512-RVZSIV5IG10Hk3enotrhvz0T9em6cyHBLkH/YAZuKqd8hRkKhSfCGIcP2KUY0EPxndzANBmNllzWPwak+bheSw==}
+    dependencies:
+      any-promise: 1.3.0
+    dev: false
+
   /tiny-glob@0.2.9:
     resolution: {integrity: sha512-g/55ssRPUjShh+xkfx9UPDXqhckHEsHr4Vd9zX55oSdGZc/MD0m3sferOkwWtp98bv+kcVfEHtRJgBVJzelrzg==}
     dependencies:
       globalyzer: 0.1.0
       globrex: 0.1.2
 
   /tmp@0.0.33:
@@ -6348,15 +6473,14 @@
     dependencies:
       os-tmpdir: 1.0.2
     dev: true
 
   /to-fast-properties@2.0.0:
     resolution: {integrity: sha512-/OaKK0xYrs3DmxRYqL/yDc+FxFUVYhDlXMhRmv3z915w2HF1tnN1omB354j8VUGO/hbRzyD6Y3sA7v7GS/ceog==}
     engines: {node: '>=4'}
-    dev: false
 
   /to-regex-range@5.0.1:
     resolution: {integrity: sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==}
     engines: {node: '>=8.0'}
     dependencies:
       is-number: 7.0.0
 
@@ -6374,35 +6498,36 @@
     engines: {node: '>=8'}
     dependencies:
       punycode: 2.3.0
     dev: true
 
   /trim-lines@3.0.1:
     resolution: {integrity: sha512-kRj8B+YHZCc9kQYdWfJB2/oUl9rA99qbowYYBtr4ui4mZyAQ2JpvVBd/6U2YloATfqBhBTSMhTpgBHtU0Mf3Rg==}
-    dev: false
 
   /trim-newlines@3.0.1:
     resolution: {integrity: sha512-c1PTsA3tYrIsLGkJkzHF+w9F2EyxfXGo4UyJc4pFL++FMjnq0HJS69T3M7d//gKrFKwy429bouPescbjecU+Zw==}
     engines: {node: '>=8'}
     dev: true
 
   /trough@2.1.0:
     resolution: {integrity: sha512-AqTiAOLcj85xS7vQ8QkAV41hPDIJ71XJB4RCUrzo/1GM2CQwhkJGaf9Hgr7BOugMRpgGUrqRg/DrBDl4H40+8g==}
+
+  /ts-interface-checker@0.1.13:
+    resolution: {integrity: sha512-Y/arvbn+rrz3JCKl9C4kVNfTfSm2/mEp5FSz5EsZSANGPSlQrpRI5M4PKF+mJnE52jOO90PnPSc3Ur3bTQw0gA==}
     dev: false
 
   /tsconfig-resolver@3.0.1:
     resolution: {integrity: sha512-ZHqlstlQF449v8glscGRXzL6l2dZvASPCdXJRWG4gHEZlUVx2Jtmr+a2zeVG4LCsKhDXKRj5R3h0C/98UcVAQg==}
     dependencies:
       '@types/json5': 0.0.30
       '@types/resolve': 1.20.2
       json5: 2.2.3
       resolve: 1.22.1
       strip-bom: 4.0.0
       type-fest: 0.13.1
-    dev: false
 
   /tslib@2.5.0:
     resolution: {integrity: sha512-336iVw3rtn2BUK7ORdIAHTyxHGRIHVReokCR3XjbckJMK7ms8FysBfhLR8IXnAgy7T0PTPNBWKiH514FOW/WSg==}
 
   /tty-table@4.1.6:
     resolution: {integrity: sha512-kRj5CBzOrakV4VRRY5kUWbNYvo/FpOsz65DzI5op9P+cHov3+IqPbo1JE1ZnQGkHdZgNFDsrEjrfqqy/Ply9fw==}
     engines: {node: '>=8.0.0'}
@@ -6430,15 +6555,14 @@
     resolution: {integrity: sha512-4dbzIzqvjtgiM5rw1k5rEHtBANKmdudhGyBEajN01fEyhaAIhsoKNy6y7+IN93IfpFtwY9iqi7kD+xwKhQsNJA==}
     engines: {node: '>=8'}
     dev: true
 
   /type-fest@2.19.0:
     resolution: {integrity: sha512-RAH822pAdBgcNMAfWnCBU3CFZcfZ/i1eZjwFU/dsLKumyuuP3niueg2UAukXYF0E2AAoc82ZSSf9J0WQBinzHA==}
     engines: {node: '>=12.20'}
-    dev: false
 
   /typed-array-length@1.0.4:
     resolution: {integrity: sha512-KjZypGq+I/H7HI5HlOoGHkWUUGq+Q0TPhQurLbyrVrvnKTBgzLhIJ7j6J/XTQOi0d1RjyZ0wdas8bKs2p0x3Ng==}
     dependencies:
       call-bind: 1.0.2
       for-each: 0.3.3
       is-typed-array: 1.1.10
@@ -6458,36 +6582,33 @@
       which-boxed-primitive: 1.0.2
     dev: true
 
   /underscore@1.13.6:
     resolution: {integrity: sha512-+A5Sja4HP1M08MaXya7p5LvjuM7K6q/2EaC0+iovj/wOcMsTzMvDFbasi/oSapiwOlt252IqsKqPjCl7huKS0A==}
     dev: false
 
-  /undici@5.20.0:
-    resolution: {integrity: sha512-J3j60dYzuo6Eevbawwp1sdg16k5Tf768bxYK4TUJRH7cBM4kFCbf3mOnM/0E3vQYXvpxITbbWmBafaDbxLDz3g==}
-    engines: {node: '>=12.18'}
+  /undici@5.22.1:
+    resolution: {integrity: sha512-Ji2IJhFXZY0x/0tVBXeQwgPlLWw13GVzpsWPQ3rV50IFMMof2I55PZZxtm4P6iNq+L5znYN9nSTAq0ZyE6lSJw==}
+    engines: {node: '>=14.0'}
     dependencies:
       busboy: 1.6.0
-    dev: false
 
   /unherit@3.0.1:
     resolution: {integrity: sha512-akOOQ/Yln8a2sgcLj4U0Jmx0R5jpIg2IUyRrWOzmEbjBtGzBdHtSeFKgoEcoH4KYIG/Pb8GQ/BwtYm0GCq1Sqg==}
-    dev: false
 
   /unified@10.1.2:
     resolution: {integrity: sha512-pUSWAi/RAnVy1Pif2kAoeWNBa3JVrx0MId2LASj8G+7AiHWoKZNTomq6LG326T68U7/e263X6fTdcXIy7XnF7Q==}
     dependencies:
       '@types/unist': 2.0.6
       bail: 2.0.2
       extend: 3.0.2
       is-buffer: 2.0.5
       is-plain-obj: 4.1.0
       trough: 2.1.0
       vfile: 5.3.7
-    dev: false
 
   /unique-filename@1.1.1:
     resolution: {integrity: sha512-Vmp0jIp2ln35UTXuryvjzkjGdRyf9b2lTXuSYUiPmzRcl3FDtYqAwOnTJkAngD9SWhnoJzDbTKwaOrZ+STtxNQ==}
     dependencies:
       unique-slug: 2.0.2
     dev: true
 
@@ -6495,74 +6616,66 @@
     resolution: {integrity: sha512-zoWr9ObaxALD3DOPfjPSqxt4fnZiWblxHIgeWqW8x7UqDzEtHEQLzji2cuJYQFCU6KmoJikOYAZlrTHHebjx2w==}
     dependencies:
       imurmurhash: 0.1.4
     dev: true
 
   /unist-util-generated@2.0.1:
     resolution: {integrity: sha512-qF72kLmPxAw0oN2fwpWIqbXAVyEqUzDHMsbtPvOudIlUzXYFIeQIuxXQCRCFh22B7cixvU0MG7m3MW8FTq/S+A==}
-    dev: false
 
   /unist-util-is@5.2.1:
     resolution: {integrity: sha512-u9njyyfEh43npf1M+yGKDGVPbY/JWEemg5nH05ncKPfi+kBbKBJoTdsogMu33uhytuLlv9y0O7GH7fEdwLdLQw==}
     dependencies:
       '@types/unist': 2.0.6
-    dev: false
 
   /unist-util-modify-children@3.1.1:
     resolution: {integrity: sha512-yXi4Lm+TG5VG+qvokP6tpnk+r1EPwyYL04JWDxLvgvPV40jANh7nm3udk65OOWquvbMDe+PL9+LmkxDpTv/7BA==}
     dependencies:
       '@types/unist': 2.0.6
       array-iterate: 2.0.1
-    dev: false
 
   /unist-util-position-from-estree@1.1.2:
     resolution: {integrity: sha512-poZa0eXpS+/XpoQwGwl79UUdea4ol2ZuCYguVaJS4qzIOMDzbqz8a3erUCOmubSZkaOuGamb3tX790iwOIROww==}
     dependencies:
       '@types/unist': 2.0.6
     dev: false
 
   /unist-util-position@4.0.4:
     resolution: {integrity: sha512-kUBE91efOWfIVBo8xzh/uZQ7p9ffYRtUbMRZBNFYwf0RK8koUMx6dGUfwylLOKmaT2cs4wSW96QoYUSXAyEtpg==}
     dependencies:
       '@types/unist': 2.0.6
-    dev: false
 
   /unist-util-remove-position@4.0.2:
     resolution: {integrity: sha512-TkBb0HABNmxzAcfLf4qsIbFbaPDvMO6wa3b3j4VcEzFVaw1LBKwnW4/sRJ/atSLSzoIg41JWEdnE7N6DIhGDGQ==}
     dependencies:
       '@types/unist': 2.0.6
       unist-util-visit: 4.1.2
     dev: false
 
   /unist-util-stringify-position@3.0.3:
     resolution: {integrity: sha512-k5GzIBZ/QatR8N5X2y+drfpWG8IDBzdnVj6OInRNWm1oXrzydiaAT2OQiA8DPRRZyAKb9b6I2a6PxYklZD0gKg==}
     dependencies:
       '@types/unist': 2.0.6
-    dev: false
 
   /unist-util-visit-children@2.0.2:
     resolution: {integrity: sha512-+LWpMFqyUwLGpsQxpumsQ9o9DG2VGLFrpz+rpVXYIEdPy57GSy5HioC0g3bg/8WP9oCLlapQtklOzQ8uLS496Q==}
     dependencies:
       '@types/unist': 2.0.6
-    dev: false
 
   /unist-util-visit-parents@5.1.3:
     resolution: {integrity: sha512-x6+y8g7wWMyQhL1iZfhIPhDAs7Xwbn9nRosDXl7qoPTSCy0yNxnKc+hWokFifWQIDGi154rdUqKvbCa4+1kLhg==}
     dependencies:
       '@types/unist': 2.0.6
       unist-util-is: 5.2.1
-    dev: false
 
   /unist-util-visit@4.1.2:
     resolution: {integrity: sha512-MSd8OUGISqHdVvfY9TPhyK2VdUrPgxkUtWSuMHF6XAAFuL4LokseigBnZtPnJMu+FbynTkFNnFlyjxpVKujMRg==}
     dependencies:
       '@types/unist': 2.0.6
       unist-util-is: 5.2.1
       unist-util-visit-parents: 5.1.3
-    dev: false
 
   /universalify@0.1.2:
     resolution: {integrity: sha512-rBJeI5CXAlmy1pV+617WB9J63U6XcazHHF2f2dbJix4XzpUF0RS3Zbj0FGIOCAva5P/d/GBOYaACQ1w+0azUkg==}
     engines: {node: '>= 4.0.0'}
     dev: true
 
   /universalify@2.0.0:
@@ -6617,45 +6730,41 @@
     engines: {node: '>=8'}
     hasBin: true
     dependencies:
       dequal: 2.0.3
       diff: 5.1.0
       kleur: 4.1.5
       sade: 1.8.1
-    dev: false
 
   /validate-npm-package-license@3.0.4:
     resolution: {integrity: sha512-DpKm2Ui/xN7/HQKCtpZxoRWBhZ9Z0kqtygG8XCgNQ8ZlDnxuQmWhj566j8fN4Cu3/JmbhsDo7fcAJq4s9h27Ew==}
     dependencies:
       spdx-correct: 3.2.0
       spdx-expression-parse: 3.0.1
     dev: true
 
   /vfile-location@4.1.0:
     resolution: {integrity: sha512-YF23YMyASIIJXpktBa4vIGLJ5Gs88UB/XePgqPmTa7cDA+JeO3yclbpheQYCHjVHBn/yePzrXuygIL+xbvRYHw==}
     dependencies:
       '@types/unist': 2.0.6
       vfile: 5.3.7
-    dev: false
 
   /vfile-message@3.1.4:
     resolution: {integrity: sha512-fa0Z6P8HUrQN4BZaX05SIVXic+7kE3b05PWAtPuYP9QLHsLKYR7/AlLW3NtOrpXRLeawpDLMsVkmk5DG0NXgWw==}
     dependencies:
       '@types/unist': 2.0.6
       unist-util-stringify-position: 3.0.3
-    dev: false
 
   /vfile@5.3.7:
     resolution: {integrity: sha512-r7qlzkgErKjobAmyNIkkSpizsFPYiUPuJb5pNW1RB4JcYVZhs4lIbVqk8XPk033CV/1z8ss5pkax8SuhGpcG8g==}
     dependencies:
       '@types/unist': 2.0.6
       is-buffer: 2.0.5
       unist-util-stringify-position: 3.0.3
       vfile-message: 3.1.4
-    dev: false
 
   /vite@4.1.4(@types/node@18.14.6):
     resolution: {integrity: sha512-3knk/HsbSTKEin43zHu7jTwYWv81f8kgAL99G5NWBcA1LKvtvcVAC4JjBH1arBunO9kQka+1oGbrMKOjk4ZrBg==}
     engines: {node: ^14.18.0 || >=16.0.0}
     hasBin: true
     peerDependencies:
       '@types/node': '>= 14'
@@ -6681,89 +6790,107 @@
       '@types/node': 18.14.6
       esbuild: 0.16.17
       postcss: 8.4.21
       resolve: 1.22.1
       rollup: 3.18.0
     optionalDependencies:
       fsevents: 2.3.2
+    dev: true
+
+  /vite@4.3.9(@types/node@18.14.6):
+    resolution: {integrity: sha512-qsTNZjO9NoJNW7KnOrgYwczm0WctJ8m/yqYAMAK9Lxt4SoySUfS5S8ia9K7JHpa3KEeMfyF8LoJ3c5NeBJy6pg==}
+    engines: {node: ^14.18.0 || >=16.0.0}
+    hasBin: true
+    peerDependencies:
+      '@types/node': '>= 14'
+      less: '*'
+      sass: '*'
+      stylus: '*'
+      sugarss: '*'
+      terser: ^5.4.0
+    peerDependenciesMeta:
+      '@types/node':
+        optional: true
+      less:
+        optional: true
+      sass:
+        optional: true
+      stylus:
+        optional: true
+      sugarss:
+        optional: true
+      terser:
+        optional: true
+    dependencies:
+      '@types/node': 18.14.6
+      esbuild: 0.17.19
+      postcss: 8.4.24
+      rollup: 3.23.1
+    optionalDependencies:
+      fsevents: 2.3.2
 
-  /vitefu@0.2.4(vite@4.1.4):
+  /vitefu@0.2.4(vite@4.3.9):
     resolution: {integrity: sha512-fanAXjSaf9xXtOOeno8wZXIhgia+CZury481LsDaV++lSvcU2R9Ch2bPh3PYFyoHW+w9LqAeYRISVQjUIew14g==}
     peerDependencies:
       vite: ^3.0.0 || ^4.0.0
     peerDependenciesMeta:
       vite:
         optional: true
     dependencies:
-      vite: 4.1.4(@types/node@18.14.6)
-    dev: false
+      vite: 4.3.9(@types/node@18.14.6)
 
   /vscode-css-languageservice@6.2.4:
     resolution: {integrity: sha512-9UG0s3Ss8rbaaPZL1AkGzdjrGY8F+P+Ne9snsrvD9gxltDGhsn8C2dQpqQewHrMW37OvlqJoI8sUU2AWDb+qNw==}
     dependencies:
       '@vscode/l10n': 0.0.11
       vscode-languageserver-textdocument: 1.0.8
       vscode-languageserver-types: 3.17.3
       vscode-uri: 3.0.7
-    dev: false
 
   /vscode-html-languageservice@5.0.4:
     resolution: {integrity: sha512-tvrySfpglu4B2rQgWGVO/IL+skvU7kBkQotRlxA7ocSyRXOZUd6GA13XHkxo8LPe07KWjeoBlN1aVGqdfTK4xA==}
     dependencies:
       '@vscode/l10n': 0.0.11
       vscode-languageserver-textdocument: 1.0.8
       vscode-languageserver-types: 3.17.3
       vscode-uri: 3.0.7
-    dev: false
 
   /vscode-jsonrpc@8.1.0:
     resolution: {integrity: sha512-6TDy/abTQk+zDGYazgbIPc+4JoXdwC8NHU9Pbn4UJP1fehUyZmM4RHp5IthX7A6L5KS30PRui+j+tbbMMMafdw==}
     engines: {node: '>=14.0.0'}
-    dev: false
 
   /vscode-languageserver-protocol@3.17.3:
     resolution: {integrity: sha512-924/h0AqsMtA5yK22GgMtCYiMdCOtWTSGgUOkgEDX+wk2b0x4sAfLiO4NxBxqbiVtz7K7/1/RgVrVI0NClZwqA==}
     dependencies:
       vscode-jsonrpc: 8.1.0
       vscode-languageserver-types: 3.17.3
-    dev: false
 
   /vscode-languageserver-textdocument@1.0.8:
     resolution: {integrity: sha512-1bonkGqQs5/fxGT5UchTgjGVnfysL0O8v1AYMBjqTbWQTFn721zaPGDYFkOKtfDgFiSgXM3KwaG3FMGfW4Ed9Q==}
-    dev: false
 
   /vscode-languageserver-types@3.17.3:
     resolution: {integrity: sha512-SYU4z1dL0PyIMd4Vj8YOqFvHu7Hz/enbWtpfnVbJHU4Nd1YNYx8u0ennumc6h48GQNeOLxmwySmnADouT/AuZA==}
-    dev: false
 
   /vscode-languageserver@8.1.0:
     resolution: {integrity: sha512-eUt8f1z2N2IEUDBsKaNapkz7jl5QpskN2Y0G01T/ItMxBxw1fJwvtySGB9QMecatne8jFIWJGWI61dWjyTLQsw==}
     hasBin: true
     dependencies:
       vscode-languageserver-protocol: 3.17.3
-    dev: false
 
   /vscode-oniguruma@1.7.0:
     resolution: {integrity: sha512-L9WMGRfrjOhgHSdOYgCt/yRMsXzLDJSL7BPrOZt73gU0iWO4mpqzqQzOz5srxqTvMBaR0XZTSrVWo4j55Rc6cA==}
 
-  /vscode-textmate@6.0.0:
-    resolution: {integrity: sha512-gu73tuZfJgu+mvCSy4UZwd2JXykjK9zAZsfmDeut5dx/1a7FeTk0XwJsSuqQn+cuMCGVbIBfl+s53X4T19DnzQ==}
-    dev: false
-
   /vscode-textmate@8.0.0:
     resolution: {integrity: sha512-AFbieoL7a5LMqcnOF04ji+rpXadgOXnZsxQr//r83kLPr7biP7am3g9zbaZIaBGwBRWeSvoMD4mgPdX3e4NWBg==}
-    dev: true
 
   /vscode-uri@2.1.2:
     resolution: {integrity: sha512-8TEXQxlldWAuIODdukIb+TR5s+9Ds40eSJrw+1iDDA9IFORPjMELarNQE3myz5XIkWWpdprmJjm1/SxMlWOC8A==}
-    dev: false
 
   /vscode-uri@3.0.7:
     resolution: {integrity: sha512-eOpPHogvorZRobNqJGhapa0JdwaxpjVvyBp0QIUMRMSf8ZAlqOdEquKuRmw9Qwu0qXtJIWqFtMkmvJjUZmMjVA==}
-    dev: false
 
   /watchpack@2.4.0:
     resolution: {integrity: sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==}
     engines: {node: '>=10.13.0'}
     dependencies:
       glob-to-regexp: 0.4.1
       graceful-fs: 4.2.10
@@ -6772,15 +6899,14 @@
   /wcwidth@1.0.1:
     resolution: {integrity: sha512-XHPEwS0q6TaxcvG85+8EYkbiCux2XtWG2mkc47Ng2A77BQu9+DqIOJldST4HgPkuea7dvKSj5VgX3P1d4rW8Tg==}
     dependencies:
       defaults: 1.0.4
 
   /web-namespaces@2.0.1:
     resolution: {integrity: sha512-bKr1DkiNa2krS7qxNtdrtHAmzuYGFQLiQ13TsorsdT6ULTkPLKuu5+GsFpDlg6JFjUTwX2DyhMPG2be8uPrqsQ==}
-    dev: false
 
   /webidl-conversions@3.0.1:
     resolution: {integrity: sha512-2JAn3z8AR6rjK8Sm8orRC0h/bcl/DqL7tRPdGZ4I1CjdF+EaMLmYxBHyXuKL849eucPFhvBoxMsflfOb8kxaeQ==}
 
   /webidl-conversions@6.1.0:
     resolution: {integrity: sha512-qBIvFLGiBpLjfwmYAaHPXsn+ho5xZnGvyGvsarywGNc8VyQJUMHJ8OBKGGrPER0okBeMDaan4mNBlgBROxuI8w==}
     engines: {node: '>=10.4'}
@@ -6914,15 +7040,14 @@
   /which-module@2.0.0:
     resolution: {integrity: sha512-B+enWhmw6cjfVC7kS8Pj9pCrKSc5txArRyaYGe088shv/FGWH+0Rjx/xPgtsWfsUtS27FkP697E4DDhgrgoc0Q==}
     dev: true
 
   /which-pm-runs@1.1.0:
     resolution: {integrity: sha512-n1brCuqClxfFfq/Rb0ICg9giSZqCS+pLtccdag6C2HyufBrh3fBOiy9nb6ggRMvWOVH5GrdJskj5iGTZNxd7SA==}
     engines: {node: '>=4'}
-    dev: false
 
   /which-pm@2.0.0:
     resolution: {integrity: sha512-Lhs9Pmyph0p5n5Z3mVnN0yWcbQYUAD7rbQUiMsQxOJ3T57k7RFe35SUwWMf7dsbDZks1uOmw4AecB/JMDj3v/w==}
     engines: {node: '>=8.15'}
     dependencies:
       load-yaml-file: 0.2.0
       path-exists: 4.0.0
@@ -6954,15 +7079,14 @@
       isexe: 2.0.0
 
   /widest-line@4.0.1:
     resolution: {integrity: sha512-o0cyEG0e8GPzT4iGHphIOh0cJOV8fivsXxddQasHPHfoZf1ZexrfeA21w2NaEN1RHE+fXlfISmOE8R9N3u3Qig==}
     engines: {node: '>=12'}
     dependencies:
       string-width: 5.1.2
-    dev: false
 
   /wildcard@2.0.0:
     resolution: {integrity: sha512-JcKqAHLPxcdb9KM49dufGXn2x3ssnfjbcaQdLlfZsL9rH9wgDQjUtDxbo8NE0F6SFvydeu1VhZe7hZuHsB2/pw==}
     dev: true
 
   /worker-loader@3.0.8(webpack@5.76.0):
     resolution: {integrity: sha512-XQyQkIFeRVC7f7uRhFdNMe/iJOdO6zxAaR3EWbDp45v3mDhrTi+++oswKNxShUNjPC/1xUp5DB29YKLhFo129g==}
@@ -6996,15 +7120,14 @@
   /wrap-ansi@8.1.0:
     resolution: {integrity: sha512-si7QWI6zUMq56bESFvagtmzMdGOtoxfR+Sez11Mobfc7tm+VkUckk9bW2UeffTGVUbOksxmSw0AA2gs8g71NCQ==}
     engines: {node: '>=12'}
     dependencies:
       ansi-styles: 6.2.1
       string-width: 5.1.2
       strip-ansi: 7.0.1
-    dev: false
 
   /wrappy@1.0.2:
     resolution: {integrity: sha512-l4Sp/DRseor9wL6EvV2+TuQn63dMkPjZ/sp9XkghTEbV9KlPS1xUsZ3u7/IQO4wxtcFB4bgpQPRcR3QCvezPcQ==}
 
   /ws@7.5.9:
     resolution: {integrity: sha512-F+P9Jil7UiSKSkppIiD94dN07AwvFixvLIj1Og1Rl9GGMuNipJnV9JzjD6XuqmAeiswGvUmNLjr5cFuXwNS77Q==}
     engines: {node: '>=8.3.0'}
@@ -7014,19 +7137,14 @@
     peerDependenciesMeta:
       bufferutil:
         optional: true
       utf-8-validate:
         optional: true
     dev: false
 
-  /xtend@4.0.2:
-    resolution: {integrity: sha512-LKYU1iAXJXUgAXn9URjiu+MWhyUXHsvfp7mcuYm9dSUKK0/CjtrUwFAxD82/mCWbtLsGjFIad0wIsod4zrTAEQ==}
-    engines: {node: '>=0.4'}
-    dev: false
-
   /y18n@4.0.3:
     resolution: {integrity: sha512-JKhqTOwSrqNA1NY5lSztJ1GrBiUodLMmIZuLiDaMRJ+itFd+ABVE8XBjOvIWL+rSqNDC74LCSFmlb/U4UZ4hJQ==}
     dev: true
 
   /y18n@5.0.8:
     resolution: {integrity: sha512-0pfFzegeDWJHJIAmTLRP2DwHjdF5s7jo9tuztdQxAhINCdvS+3nGINqPd00AphqJR/0LhANUS6/+7SCb98YOfA==}
     engines: {node: '>=10'}
@@ -7034,24 +7152,18 @@
 
   /yallist@2.1.2:
     resolution: {integrity: sha512-ncTzHV7NvsQZkYe1DW7cbDLm0YpzHmZF5r/iyP3ZnQtMiJ+pjzisCiMNI+Sj+xQF5pXhSHxSB3uDbsBTzY/c2A==}
     dev: true
 
   /yallist@3.1.1:
     resolution: {integrity: sha512-a4UGQaWPH59mOXUYnAG2ewncQS4i4F43Tv3JoAM+s2VDAmS9NsK8GpDMLrCHPksFT7h3K6TOoUNn2pb7RoXx4g==}
-    dev: false
 
   /yallist@4.0.0:
     resolution: {integrity: sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==}
 
-  /yaml@1.10.2:
-    resolution: {integrity: sha512-r3vXyErRCYJ7wg28yvBY5VSoAF8ZvlcW9/BwUzEtUsjvX/DKs24dIkuwjtuprwJJHsbyUbLApepYTR1BN4uHrg==}
-    engines: {node: '>= 6'}
-    dev: false
-
   /yaml@2.2.1:
     resolution: {integrity: sha512-e0WHiYql7+9wr4cWMx3TVQrNwejKaEe7/rHNmQmqRjazfOP5W8PB6Jpebb5o6fIapbz9o9+2ipcaTM2ZwDI6lw==}
     engines: {node: '>= 14'}
     dev: false
 
   /yargs-parser@18.1.3:
     resolution: {integrity: sha512-o50j0JeToy/4K6OZcaQmW6lyXXKhq7csREXcDwk2omFPJEwUNOVtJKvmDr9EI1fAJZUyZcRF7kxGBWmRXudrCQ==}
@@ -7095,14 +7207,16 @@
       yargs-parser: 21.1.1
     dev: true
 
   /yocto-queue@0.1.0:
     resolution: {integrity: sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==}
     engines: {node: '>=10'}
 
+  /yocto-queue@1.0.0:
+    resolution: {integrity: sha512-9bnSc/HEW2uRy67wc+T8UwauLuPJVn28jb+GtJY16iiKWyvmYJRXVT4UamsAEGQfPohgr2q4Tq0sQbQlxTfi1g==}
+    engines: {node: '>=12.20'}
+
   /zod@3.21.4:
     resolution: {integrity: sha512-m46AKbrzKVzOzs/DZgVnG5H55N1sv1M8qZU3A8RIKbs3mrACDNeIOeilDymVb2HdmP8uwshOCF4uJ8uM9rCqJw==}
-    dev: false
 
   /zwitch@2.0.4:
     resolution: {integrity: sha512-bXE4cR/kVZhKZX/RjPEflHaKVhUVl85noU3v6b8apfQEc1x4A+zBxjZ4lN8LqGd6WZ3dl98pY4o717VFmoPp+A==}
-    dev: false
```

### Comparing `anywidget-0.4.1/anywidget/_descriptor.py` & `anywidget-0.4.2/anywidget/_descriptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
     #     ...
 
     def __call__(self, **kwargs: Sequence[str]) -> tuple[dict, dict]:
         """Called when _repr_mimebundle_ is called on the python object."""
         # NOTE: this could conceivably be a method on a Comm subclass
         # (i.e. the comm knows how to represent itself as a mimebundle)
         data = {
-            "text/plain": repr(self),
+            "text/plain": repr(self._obj()),
             _WIDGET_MIME_TYPE: {
                 "version_major": _PROTOCOL_VERSION_MAJOR,
                 "version_minor": _PROTOCOL_VERSION_MINOR,
                 "model_id": self._comm.comm_id,
             },
         }
         return data, get_repr_metadata()
```

### Comparing `anywidget-0.4.1/anywidget/_file_contents.py` & `anywidget-0.4.2/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/anywidget/_protocols.py` & `anywidget-0.4.2/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/anywidget/_util.py` & `anywidget-0.4.2/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/anywidget/experimental.py` & `anywidget-0.4.2/anywidget/experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/anywidget/widget.py` & `anywidget-0.4.2/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/anywidget/labextension/package.json` & `anywidget-0.4.2/anywidget/labextension/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95703125%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9229e22154b84f74e1ee.js'}}",*

 * * "'version'": "'0.4.2'"}*

```diff
@@ -22,15 +22,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.68d0702ea589c32d2c52.js"
+            "load": "static/remoteEntry.9229e22154b84f74e1ee.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -42,9 +42,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

### Comparing `anywidget-0.4.1/anywidget/labextension/static/138.da9bcb3835f584489120.js` & `anywidget-0.4.2/anywidget/labextension/static/138.60ddf4a50d830c18a721.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -92,11 +92,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.1"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.2"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.4.1/anywidget/labextension/static/326.00a9c40e24b6392a7970.js` & `anywidget-0.4.2/anywidget/labextension/static/326.53aec23a9e055d4c6252.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -110,11 +110,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.1"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.2"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.4.1/anywidget/labextension/static/remoteEntry.68d0702ea589c32d2c52.js` & `anywidget-0.4.2/anywidget/labextension/static/remoteEntry.9229e22154b84f74e1ee.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v = {
             408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -41,49 +41,49 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        138: "da9bcb3835f584489120",
-        326: "00a9c40e24b6392a7970"
+        138: "60ddf4a50d830c18a721",
+        326: "53aec23a9e055d4c6252"
     } [e] + ".js?v=" + {
-        138: "da9bcb3835f584489120",
-        326: "00a9c40e24b6392a7970"
+        138: "60ddf4a50d830c18a721",
+        326: "53aec23a9e055d4c6252"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var f = (r, n) => {
+            var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -104,15 +104,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => m.e(138).then((() => () => m(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.4.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.4.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -161,33 +161,33 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
-                if ("u" == d) {
-                    if (!l || "u" != f) return !1
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == f) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (f == d)
+                    if (d == f)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (o ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < f != o) return !1;
+                    if (u <= n || f < d != o) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
@@ -198,20 +198,20 @@
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), d(e[t][o])
-    }, d = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, o) {
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), f(e[t][o])
+    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var a = m.I(r);
         return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, c = {
-        395: () => f("default", "@jupyter-widgets/base", [, [1, 6],
+        395: () => d("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, h = {
         326: [395]
@@ -265,10 +265,10 @@
                     u && u(m)
                 }
                 for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var b = m(408);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = b
+    var y = m(408);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = y
 })();
```

### Comparing `anywidget-0.4.1/anywidget/nbextension/index.js` & `anywidget-0.4.2/anywidget/nbextension/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.4.1";
+var version = "0.4.2";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
```

### Comparing `anywidget-0.4.1/docs/README.md` & `anywidget-0.4.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/astro.config.mjs` & `anywidget-0.4.2/docs/astro.config.js`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 00000210: 636f 6d70 6f6e 656e 742e 0a09 0972 6561  component....rea
 00000220: 6374 2829 2c0a 0909 2f2f 2053 7570 706f  ct(),...// Suppo
 00000230: 7274 202e 6970 796e 6220 7061 6765 730a  rt .ipynb pages.
 00000240: 0909 6970 796e 6228 7b20 6578 6563 7574  ..ipynb({ execut
 00000250: 653a 2066 616c 7365 207d 292c 0a09 092f  e: false }),.../
 00000260: 2f20 4164 6465 6420 666f 7220 6375 7374  / Added for cust
 00000270: 6f6d 206c 616e 6469 6e67 2070 6167 650a  om landing page.
-00000280: 0909 7461 696c 7769 6e64 2829 2c0a 0909  ..tailwind(),...
-00000290: 2f2f 2053 7570 6f72 7473 2063 6f6d 706f  // Suports compo
-000002a0: 6e65 6e74 7320 696e 206d 6172 6b64 6f77  nents in markdow
-000002b0: 6e0a 0909 6d64 7828 292c 0a09 5d2c 0a09  n...mdx(),..],..
-000002c0: 7369 7465 3a20 6068 7474 7073 3a2f 2f61  site: `https://a
-000002d0: 6e79 7769 6467 6574 2e64 6576 2f60 2c0a  nywidget.dev/`,.
-000002e0: 7d29 3b0a                                });.
+00000280: 0909 7461 696c 7769 6e64 287b 2063 6f6e  ..tailwind({ con
+00000290: 6669 673a 207b 2061 7070 6c79 4261 7365  fig: { applyBase
+000002a0: 5374 796c 6573 3a20 6661 6c73 6520 7d20  Styles: false } 
+000002b0: 7d29 2c0a 0909 2f2f 2053 7570 6f72 7473  }),...// Suports
+000002c0: 2063 6f6d 706f 6e65 6e74 7320 696e 206d   components in m
+000002d0: 6172 6b64 6f77 6e0a 0909 6d64 7828 292c  arkdown...mdx(),
+000002e0: 0a09 5d2c 0a09 7369 7465 3a20 6068 7474  ..],..site: `htt
+000002f0: 7073 3a2f 2f61 6e79 7769 6467 6574 2e64  ps://anywidget.d
+00000300: 6576 2f60 2c0a 7d29 3b0a                 ev/`,.});.
```

### Comparing `anywidget-0.4.1/docs/package.json` & `anywidget-0.4.2/docs/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9537037037037037%*

 * *Differences: {"'dependencies'": "{'@astrojs/markdown-remark': '^2.2.1', '@astrojs/mdx': '^0.19.6', "*

 * *                   "'@astrojs/preact': '^2.2.1', '@astrojs/react': '^2.2.1', '@astrojs/tailwind': "*

 * *                   "'^3.1.3', '@types/react': '^18.2.8', '@types/react-dom': '^18.2.4', 'react': "*

 * *                   "'^18.2.0', 'react-dom': '^18.2.0', 'tailwindcss': '^3.3.2', "*

 * *                   "'@types/html-escaper': '^3.0.0', delete: ['astro']}",*

 * * "'devDependencies'": "{'astro': '^2.5.7'}"}*

```diff
@@ -1,28 +1,29 @@
 {
     "dependencies": {
         "@algolia/client-search": "^4.13.1",
-        "@astrojs/markdown-remark": "^2.1.0",
-        "@astrojs/mdx": "^0.15.1",
-        "@astrojs/preact": "^2.0.0",
-        "@astrojs/react": "^2.0.1",
-        "@astrojs/tailwind": "^3.0.0",
+        "@astrojs/markdown-remark": "^2.2.1",
+        "@astrojs/mdx": "^0.19.6",
+        "@astrojs/preact": "^2.2.1",
+        "@astrojs/react": "^2.2.1",
+        "@astrojs/tailwind": "^3.1.3",
         "@docsearch/css": "^3.1.0",
         "@docsearch/react": "^3.1.0",
+        "@types/html-escaper": "^3.0.0",
         "@types/node": "^18.0.0",
-        "@types/react": "^17.0.45",
-        "@types/react-dom": "^18.0.0",
-        "astro": "^2.0.2",
+        "@types/react": "^18.2.8",
+        "@types/react-dom": "^18.2.4",
         "gray-matter": "^4.0.3",
         "preact": "^10.7.3",
-        "react": "^18.1.0",
-        "react-dom": "^18.1.0",
-        "tailwindcss": "^3.2.4"
+        "react": "^18.2.0",
+        "react-dom": "^18.2.0",
+        "tailwindcss": "^3.3.2"
     },
     "devDependencies": {
+        "astro": "^2.5.7",
         "html-escaper": "^3.0.3",
         "prettier": "^2.8.2",
         "prettier-plugin-astro": "^0.7.2",
         "shiki": "^0.14.1",
         "vite": "^4.1.4"
     },
     "name": "@anywidget/docs",
```

### Comparing `anywidget-0.4.1/docs/public/anywidget-overview.png` & `anywidget-0.4.2/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/public/banner-dark.png` & `anywidget-0.4.2/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/public/banner-light.png` & `anywidget-0.4.2/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/public/banner-minimal.png` & `anywidget-0.4.2/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/public/client-js-diagram.png` & `anywidget-0.4.2/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/public/default-og-image.png` & `anywidget-0.4.2/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/public/favicon.svg` & `anywidget-0.4.2/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/public/widget-overview.png` & `anywidget-0.4.2/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/scripts/ipynb.mjs` & `anywidget-0.4.2/docs/scripts/ipynb.mjs`

 * *Files 1% similar despite different names*

```diff
@@ -150,16 +150,16 @@
  */
 async function renderCellsMarkdown(nb, options) {
 	/** @param {string} content */
 	function _renderMarkdown(content) {
 		return renderMarkdown(content, {
 			...options.config.markdown,
 			fileURL: new URL(`file://${options.fileId}`),
-			contentDir: new URL("./content/", options.config.srcDir),
 			// @ts-expect-error
+			contentDir: new URL("./content/", options.config.srcDir),
 			frontmatter: options.frontmatter,
 		});
 	}
 	let raw = "",
 		html = "";
 	let headings;
 
@@ -184,16 +184,17 @@
  * @returns {import('vite').Plugin}
  */
 function vitePlugin(options) {
 	return {
 		name: "ipynb",
 		enforce: "pre",
 		async transform(_, id) {
-			if (!id.endsWith("ipynb")) return;
+			if (!id.endsWith(".ipynb")) return;
 			let { fileId, fileUrl } = getFileInfo(id, options.config);
+
 			let nb = await readNotebook(fileId, options.execute);
 
 			let frontmatter = {};
 
 			if (nb.cells[0].cell_type == "raw") {
 				let rawSource = extractCellSource(nb.cells.shift());
 				frontmatter = parseFrontmatter(rawSource, id).data;
```

### Comparing `anywidget-0.4.1/docs/scripts/utils.mjs` & `anywidget-0.4.2/docs/scripts/utils.mjs`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,9 @@
 // @ts-check
 import matter from "gray-matter";
-import { normalizePath } from "vite";
-import { fileURLToPath } from "node:url";
-
-// absolute path of "astro/jsx-runtime"
-let astroJsxRuntimeModulePath = normalizePath(
-	fileURLToPath(
-		new URL("../node_modules/astro/dist/jsx-runtime/index.js", import.meta.url)
-	)
-);
 
 /**
  * @param {string} code
  * @param {string} id
  * @see https://github.com/withastro/astro/blob/c53b1fca073136e1e1a6f5d0b32d7c023e98c675/packages/integrations/mdx/src/utils.ts#L45-L63
  */
 export function parseFrontmatter(code, id) {
@@ -94,20 +85,21 @@
 	headings,
 	html,
 }) {
 	let { layout } = frontmatter;
 
 	// deno-fmt-ignore
 	return `
-	import { Fragment, jsx as h } from ${JSON.stringify(astroJsxRuntimeModulePath)};
+	import { Fragment, jsx as h } from 'astro/jsx-runtime';
 	${layout ? `import Layout from ${JSON.stringify(layout)};` : ""}
 	const html = ${JSON.stringify(html)};
 	export const frontmatter = ${JSON.stringify(frontmatter)};
 	export const file = ${JSON.stringify(fileId)};
 	export const url = ${JSON.stringify(fileUrl)};
+
 	export function rawContent() {
 		return ${JSON.stringify(raw)};
 	}
 	export function compiledContent() {
 		return html;
 	}
 	export function getHeadings() {
```

### Comparing `anywidget-0.4.1/docs/src/consts.ts` & `anywidget-0.4.2/docs/src/consts.ts`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 	title: "anywidget",
 	description: "custom jupyter widgets made easy",
 	defaultLanguage: "en_US",
 };
 
 export const OPEN_GRAPH = {
 	image: {
-		// TODO: change to public/banner-minimal.png when repo is public
-		src: "https://user-images.githubusercontent.com/24403730/212561522-74377f45-45fe-4d21-b40a-bb7099f710a9.png",
+		src: "https://raw.githubusercontent.com/manzt/anywidget/main/docs/public/banner-minimal.png",
 		alt: "anywidget logo on white background",
 	},
 	twitter: "trevmanz",
 };
 
 // This is the type of the frontmatter you put in the docs markdown files.
 export type Frontmatter = {
@@ -37,28 +36,32 @@
 // See "Algolia" section of the README for more information.
 export const ALGOLIA = {
 	indexName: "anywidget",
 	appId: "5UZQUZZNXI",
 	apiKey: "f8be8ea567a2b746ccc3986f9db3a129",
 };
 
-export type Sidebar = Record<
-	(typeof KNOWN_LANGUAGE_CODES)[number],
-	Record<string, { text: string; link: string }[]>
->;
+export type Sidebar = {
+	[Code in (typeof KNOWN_LANGUAGE_CODES)[number]]: Record<
+		string,
+		{ text: string; link: string }[]
+	>;
+};
 export const SIDEBAR: Sidebar = {
 	en: {
 		Guide: [
 			{ text: "Getting Started", link: "en/getting-started" },
 			{
 				text: "Jupyter Widgets: The Good Parts",
 				link: "en/jupyter-widgets-the-good-parts",
 			},
-			{ text: "Advanced: Bundling", link: "en/bundling" },
-			{ text: "Advanced: Experimental Features", link: "en/experimental" },
+		],
+		Advanced: [
+			{ text: "Bundling", link: "en/bundling" },
+			{ text: "Experimental Features", link: "en/experimental" },
 		],
 		Notebooks: [
 			{ text: "Build a Counter Widget", link: "en/notebooks/counter" },
 		],
 		Blog: [
 			{ text: "Introducing anywidget", link: "blog/introducing-anywidget" },
 			{ text: "Modern Web Meets Jupyter", link: "blog/anywidget-02" },
```

### Comparing `anywidget-0.4.1/docs/src/components/CodeHero.astro` & `anywidget-0.4.2/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/CounterButton.astro` & `anywidget-0.4.2/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/HeadCommon.astro` & `anywidget-0.4.2/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/HeadSEO.astro` & `anywidget-0.4.2/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Hero.astro` & `anywidget-0.4.2/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.4.2/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.4.2/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.4.2/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Header/Header.astro` & `anywidget-0.4.2/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Header/HeaderButton.css` & `anywidget-0.4.2/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.4.2/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.4.2/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Header/Search.css` & `anywidget-0.4.2/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Header/Search.tsx` & `anywidget-0.4.2/docs/src/components/Header/Search.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	}, [setIsOpen]);
 
 	const onClose = useCallback(() => {
 		setIsOpen(false);
 	}, [setIsOpen]);
 
 	const onInput = useCallback(
-		(e) => {
+		(e: KeyboardEvent) => {
 			setIsOpen(true);
 			setInitialQuery(e.key);
 		},
 		[setIsOpen, setInitialQuery]
 	);
 
 	useDocSearchKeyboardEvents({
```

### Comparing `anywidget-0.4.1/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.4.2/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.4.2/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.4.2/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.4.2/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.4.2/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.4.2/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.4.2/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.4.2/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+/** @jsxImportSource preact */
+
 import { unescape } from "html-escaper";
 import type { MarkdownHeading } from "astro";
 import type { FunctionalComponent } from "preact";
 import { useEffect, useRef, useState } from "preact/hooks";
+import type { JSXInternal } from "preact/src/jsx";
 
 type ItemOffsets = {
 	id: string;
 	topOffset: number;
 };
 
 const TableOfContents: FunctionalComponent<{ headings: MarkdownHeading[] }> = ({
 	headings = [],
 }) => {
-	const toc = useRef<HTMLUListElement>();
+	const toc = useRef<HTMLUListElement>(null);
 	const onThisPageID = "on-this-page-heading";
 	const itemOffsets = useRef<ItemOffsets[]>([]);
 	const [currentID, setCurrentID] = useState("overview");
 	useEffect(() => {
 		const getItemOffsets = () => {
 			const titles = document.querySelectorAll("article :is(h1, h2, h3, h4)");
 			itemOffsets.current = Array.from(titles).map((title) => ({
@@ -63,16 +66,16 @@
 			.querySelectorAll("article :is(h1,h2,h3)")
 			.forEach((h) => headingsObserver.observe(h));
 
 		// Stop observing when the component is unmounted.
 		return () => headingsObserver.disconnect();
 	}, [toc.current]);
 
-	const onLinkClick = (e) => {
-		setCurrentID(e.target.getAttribute("href").replace("#", ""));
+	const onLinkClick: JSXInternal.MouseEventHandler<HTMLAnchorElement> = (e) => {
+		setCurrentID(e.currentTarget.getAttribute("href")!.replace("#", ""));
 	};
 
 	return (
 		<>
 			<h2 id={onThisPageID} className="heading">
 				On this page
 			</h2>
```

### Comparing `anywidget-0.4.1/docs/src/components/examples/Counter.astro` & `anywidget-0.4.2/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/layouts/MainLayout.astro` & `anywidget-0.4.2/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/layouts/SplashLayout.astro` & `anywidget-0.4.2/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.4.2/docs/src/pages/blog/anywidget-02.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ---
 title: "Modern Web Meets Jupyter"
 description: "Announcing anywidget v0.2: Modern Web Development in Jupyter"
 layout: ../../layouts/MainLayout.astro
 authors: ["Trevor Manz"]
-image: {
-  src: "https://user-images.githubusercontent.com/24403730/213607015-e3fb38f9-5e75-439b-95c9-99e1fde11955.png",
-  alt: "anywidget logo and counter example using API",
-}
+image:
+  {
+    src: "https://user-images.githubusercontent.com/24403730/213607015-e3fb38f9-5e75-439b-95c9-99e1fde11955.png",
+    alt: "anywidget logo and counter example using API",
+  }
 ---
 
 _TL;DR: **anywidget** v0.2 brings modern web development to Jupyter. You can now
 use a **file path** to enable **anywidget**'s integrated Hot Module Replacement (HMR):_
 
 ```sh
 pip install --upgrade "anywidget[dev]"
@@ -121,76 +122,73 @@
 /**
  * @typedef Model
  * @prop {number} value - the current count value
  */
 
 /** @type {import("anywidget/types").Render<Model>} */
 export function render(view) {
-  let value = view.model.get("value");
-  //^? number
+	let value = view.model.get("value");
+	//^? number
 
-  view.model.get("nope");
-  // type error, `nope` is not defined on Model
+	view.model.get("nope");
+	// type error, `nope` is not defined on Model
 
-  view.model.set("value", "not a number");
-  //^? type error, must be a number
+	view.model.set("value", "not a number");
+	//^? type error, must be a number
 }
 ```
 
 The `import("anywidget/widget").Render<Model>` utilty strictly types the `render` function such that
 `view.model.get` and `view.model.set` are typed based on the user-defined `Model`.
 
-
 This feature brings Jupyter Widgets one step closer to having **end-to-end type safety**, and
 the use of TypeScript within JSDoc comments means that widget front-end code can benefit
 from static analysis without additional compilation, much like Python's builtin type hints.
 
 ### Defining Custom Cleanup Logic
 
 Prior versions of **anywidget** did not expose a dedicated API for defining cleanup logic for a view.
 In v0.2, we're introducing an API (inspired by React's `useEffect` hook) to allow developers to define
 a callback that is executed any time the a view is removed from the DOM. This enhancement is useful
 when dealing with complex event listeners, subscriptions, or third-party libraries that require proper
 teardown.
 
-Although this feature might not be essential for all use cases, it provides a flexible and more declarative 
+Although this feature might not be essential for all use cases, it provides a flexible and more declarative
 way to ensure proper cleanup when needed:
 
 ```javascript
 export function render(view) {
-  // Create DOM elements and set up subscribers
-  return () => {
-    // Optionally cleanup
-  };
+	// Create DOM elements and set up subscribers
+	return () => {
+		// Optionally cleanup
+	};
 }
 ```
 
 This new API is particularly useful when working with third-party libraries like React
-that take control of the DOM and require proper cleanup to prevent exceptions when 
+that take control of the DOM and require proper cleanup to prevent exceptions when
 elements are unmounted. For example:
 
-
 ```javascript
 import * as React from "https://esm.sh/react@18";
 import * as ReactDOM from "https://esm.sh/react-dom@18/client";
 
 function App(props) {
-  return <h1>Hello, world</h1>
+	return <h1>Hello, world</h1>;
 }
 
 export function render(view) {
-  let root = ReactDOM.createRoot(view.el);
-  root.render(<App />)
-  return () => root.unmount();
+	let root = ReactDOM.createRoot(view.el);
+	root.render(<App />);
+	return () => root.unmount();
 }
 ```
 
-> Note: The above front-end code requires transformation with tool like `esbuild` 
-to allow for the special JSX syntax (e.g., `<App />`).
-
+> Note: The above front-end code requires transformation with tool like `esbuild`
+> to allow for the special JSX syntax (e.g., `<App />`).
 
 ## Getting Started
 
 To start using **anywidget** v0.2, upgrade your package using pip:
 
 ```sh
 pip install --upgrade "anywidget[dev]"
```

### Comparing `anywidget-0.4.1/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.4.2/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/pages/en/bundling.md` & `anywidget-0.4.2/docs/src/pages/en/bundling.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 unsupported browser syntax.
 
 If using a bundler, make sure to load the final bundled assets in your widget
 and not the original/untransformed JavaScript source files.
 
 ## esbuild
 
-[esbuild](https://esbuild.github.io/) is very fast JavaScript bundler written in Golang. 
+[esbuild](https://esbuild.github.io/) is very fast JavaScript bundler written in Golang.
 It can transform **TypeScript, JSX, and CSS files** and includes zero
 JavaScrit dependencies. Binaries can be [installed without `npm`](https://esbuild.github.io/getting-started/#other-ways-to-install),
 making it a great fit for **anywidget** projects.
 
 ### Project Setup
 
 The following project structure contains a python package (`hello_widget`) with
@@ -80,15 +80,14 @@
 watch for changes to the re-bundled outputs from `esbuild`, swapping in
 the new bundle in the front end.
 
 ```bash
 esbuild --bundle --format=esm --outdir=hello_widget/static src/index.js --watch
 ```
 
-
 ## Vite
 
 Our [Vite](https://vitejs.dev/) plugin offers a more fully featured development
 experience compared to **anywidget**'s builtin HMR, but at the cost of added
 project complexity and tooling. Vite is a good choice if you want to
 use a front-end framework like Svelte or Vue or need more fine grain control
 over your bundling.
@@ -104,21 +103,21 @@
 Create a `vite.config.js` file with the following configuration:
 
 ```javascript
 // vite.config.js
 import { defineConfig } from "vite";
 
 export default defineConfig({
-  build: {
-    outDir: "hello_widget/static",
-    lib: {
-      entry: ["src/index.js"],
-      formats: ["es"],
-    },
-  },
+	build: {
+		outDir: "hello_widget/static",
+		lib: {
+			entry: ["src/index.js"],
+			formats: ["es"],
+		},
+	},
 });
 ```
 
 Your project structure should now look like:
 
 ```bash
 hello_widget/
```

### Comparing `anywidget-0.4.1/docs/src/pages/en/experimental.md` & `anywidget-0.4.2/docs/src/pages/en/experimental.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 > This page describes experimental features and APIs which are subject to change
 > in future releases.
 
 ## A brief overview of widgets in Jupyter
 
 In order to understand the motivation and function of some features in the
 `experimental` module, it is helpful to have a brief overview of how widgets
-work in Jupyter.  This is summarized below, but for a more in-depth explanation,
+work in Jupyter. This is summarized below, but for a more in-depth explanation,
 see the [jupyter-widgets messaging
 protocol](https://github.com/jupyter-widgets/ipywidgets/blob/main/packages/schema/messages.md).
 
 ### 1. The `_repr_mimebundle_` method
 
 When representing a python object, many front-ends REPLs, [including
 IPython](https://ipython.readthedocs.io/en/stable/config/integrating.html#MyObject._repr_mimebundle_),
-will look for a `_repr_mimebundle_` method on the object.  If found, this method
+will look for a `_repr_mimebundle_` method on the object. If found, this method
 must return a dictionary of data, keyed by [MIME
 type](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types),
-that can be used to render the object in the front-end.  A super simple
+that can be used to render the object in the front-end. A super simple
 plain-text representation of an object might look like this:
 
 ```python
 class SomeDisplayableObject:
     def _repr_mimebundle_(self, **kwargs):
         return {"text/plain": repr(self)}
 ```
@@ -46,17 +46,17 @@
   }
 }
 ```
 
 ### 3. The `Comm` object
 
 A `comm.base_comm.BaseComm` object manages communication between the front end (Javascript model)
-and the backend (Python model).  When the user modifies the state of the python object, the comm
+and the backend (Python model). When the user modifies the state of the python object, the comm
 must send a message containing the updated JSON state to the front end, so that the widget view
-can be update.  Similarly, when the user interacts with the widget in the browser, the front end
+can be update. Similarly, when the user interacts with the widget in the browser, the front end
 must send a message to the backend, so that the python model can be updated.
 
 ### Summary
 
 In summary, we need the following to display a javascript-backed widget for
 a python object:
 
@@ -102,31 +102,31 @@
 ```
 
 When this descriptor is accessed on an instance, it will
 
 1. create a new `Comm` channel for this object.
 2. determine what data-class pattern the object uses, and set-up serialization
    of the object currently supporting:
-    - [`dataclasses.dataclass`](https://docs.python.org/3/library/dataclasses.html)
-    - [`pydantic.BaseModel`](https://pydantic-docs.helpmanual.io/usage/models/)
-    - [`traitlets.HasTraits`](https://traitlets.readthedocs.io/en/stable/)
-    - [`msgspec.Struct`](https://jcristharif.com/msgspec/structs.html)
-    - any class implementing a `_get_anywidget_state` method that returns the
-      object state as a `dict`.
+   - [`dataclasses.dataclass`](https://docs.python.org/3/library/dataclasses.html)
+   - [`pydantic.BaseModel`](https://pydantic-docs.helpmanual.io/usage/models/)
+   - [`traitlets.HasTraits`](https://traitlets.readthedocs.io/en/stable/)
+   - [`msgspec.Struct`](https://jcristharif.com/msgspec/structs.html)
+   - any class implementing a `_get_anywidget_state` method that returns the
+     object state as a `dict`.
 3. determine what observer pattern the object uses, and set-up two-way data
-    binding between the object and the `comm`, currently supporting:
-    - [`traitlets.HasTraits`](https://traitlets.readthedocs.io/en/stable/)
-    - a
-      [`psygnal.SignalGroup`](https://psygnal.readthedocs.io/en/latest/dataclasses/)
-      on the object (conventionally named `events`)
+   binding between the object and the `comm`, currently supporting:
+   - [`traitlets.HasTraits`](https://traitlets.readthedocs.io/en/stable/)
+   - a
+     [`psygnal.SignalGroup`](https://psygnal.readthedocs.io/en/latest/dataclasses/)
+     on the object (conventionally named `events`)
 
 ## The `widget` decorator
 
 In practice, we'd like the `MimeBundleDescriptor` to be a low-level API that most
-users don't need to interact with directly.  The `anywidget.experimental.widget`
+users don't need to interact with directly. The `anywidget.experimental.widget`
 decorator provides a higher-level API that can be used to create a widget from
 any python object that implements a known data-class pattern and observer.
 
 Here's an example of how to use the `widget` decorator to create a widget from a
 `dataclasses.dataclass`, that uses psygnal's [evented-dataclass pattern](https://psygnal.readthedocs.io/en/latest/dataclasses/) for
 observers:
```

### Comparing `anywidget-0.4.1/docs/src/pages/en/getting-started.mdx` & `anywidget-0.4.2/docs/src/pages/en/getting-started.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -76,55 +76,54 @@
 
 - `_esm` specifies a <u>**required**</u> [ECMAScript module](https://nodejs.org/api/esm.html) for the widget.
   It must _must_ export a `render` custom rendering logic and initializes dynamic updates for the custom widget.
 
 ```javascript
 /** @param view {import("@jupyter-widgets/base").DOMWidgetView} */
 export function render(view) {
-  // Render model contents and setup dynamic updates
-  // See Jupyter widgets docs for more information: https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Custom.html#Rendering-model-contents
+	// Render model contents and setup dynamic updates
+	// See Jupyter widgets docs for more information: https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Custom.html#Rendering-model-contents
 }
 ```
 
 ECMAScript modules are the offical standard format to package JavaScript code for reuse and are supported
 natively across [all major browsers](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules#javascript.statements.export).
 Therefore, dependencies can be imported directly via a fully qualified URL.
 
 ```javascript
 import * as d3 from "https://esm.sh/d3@7";
 
 /** @param view {import("@jupyter-widgets/base").DOMWidgetView} */
 export function render(view) {
-  let selection = d3.select(view.el);
-  /* ... */
+	let selection = d3.select(view.el);
+	/* ... */
 }
 ```
 
 The `render` function can also (optionally) return a callback that is executed any time the view is
 removed from the DOM. This feature is useful when dealing with complex event listeners, subscriptions,
 or third-party libraries that require proper teardwon.
 
 ```javascript
 /** @param view {import("@jupyter-widgets/base").DOMWidgetView} */
 export function render(view) {
-  // Create DOM elements and set up subscribers
-  return () => {
-    // Optionally cleanup
-  };
+	// Create DOM elements and set up subscribers
+	return () => {
+		// Optionally cleanup
+	};
 }
 ```
 
 You may optionally [bundle](/en/bundling) your code to a single ESM target so that your widget works offline.
 
 > Both `_esm` and `_css` can either be a Python string containing actual front-end code
-or alternatively **file paths**. If a file path is provided during development,
-you opt in to [**anywidget**'s native HMR](/blog/anywidget-02/#native-hot-module-replacement-hmr).
-**anywidget** will start listening for modifications to the referenced files and instantly 
-apply changes to the front-end.
-
+> or alternatively **file paths**. If a file path is provided during development,
+> you opt in to [**anywidget**'s native HMR](/blog/anywidget-02/#native-hot-module-replacement-hmr).
+> **anywidget** will start listening for modifications to the referenced files and instantly
+> apply changes to the front-end.
 
 ## Motivation
 
 Official
 [cookiecutter templates](https://github.com/jupyter-widgets/?q=cookiecutter&type=all&language=&sort=)
 provide the defacto approach for creating custom Jupyter widgets, but derived
 projects are bootstrapped with complicated packaging and distribution scripts
```

### Comparing `anywidget-0.4.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.4.2/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,38 +27,40 @@
 
 Concretely, custom widgets are traditionally defined like:
 
 ```javascript
 import { DOMWidgetModel, DOMWidgetView } from "@jupyter-widgets/base";
 
 // All boilerplate, anywidget takes care of this ...
-class CustomModel extends DOMWidgetModel { /* ... */ }
+class CustomModel extends DOMWidgetModel {
+	/* ... */
+}
 
 class CustomView extends DOMWidgetView {
-  render() {
-    let view = this;
-    let el = this.el;
-    let model = this.model;
-    /* ... */
-  }
+	render() {
+		let view = this;
+		let el = this.el;
+		let model = this.model;
+		/* ... */
+	}
 }
 
 export { CustomModel, CustomView };
 ```
 
 ... which must be transformed, bundled, and installed in multiple notebook environments.
 
 In **anywidget**, the above code simplies to just:
 
 ```javascript
 /** @param view {DOMWidgetView} view */
 export function render(view) {
-  let el = view.el;
-  let model = view.model;
-  /* ... */
+	let el = view.el;
+	let model = view.model;
+	/* ... */
 }
 ```
 
 ... which explicity defines the widget view (i.e., `CustomView`) via the `render`
 function, and (implicitly) **anywidget** defines the associated widget
 model (i.e., `CustomModel`). **anywidget** front-end code is often so
 minimal that it can easily be inlined as a Python string:
@@ -110,38 +112,38 @@
 end. The `render` function now has the ability to:
 
 - **get** `my_value`
 
 ```javascript
 // index.js
 export function render(view) {
-  let my_value = view.model.get("my_value");
+	let my_value = view.model.get("my_value");
 }
 ```
 
 - **set** `my_value`
 
 ```javascript
 // index.js
 export function render(view) {
-  view.model.set("my_value", 42);
-  view.model.save_changes(); // required to send update to Python
+	view.model.set("my_value", 42);
+	view.model.save_changes(); // required to send update to Python
 }
 ```
 
 - **listen for changes to** `my_value` (and register event handlers)
 
 ```javascript
 // index.js
 export function render(view) {
-  function on_change() {
-    let new_my_value = view.model.get("my_value");
-    console.log(`The 'my_value' changed to: ${new_my_value}`);
-  }
-  view.model.on("change:my_value", on_change);
+	function on_change() {
+		let new_my_value = view.model.get("my_value");
+		console.log(`The 'my_value' changed to: ${new_my_value}`);
+	}
+	view.model.on("change:my_value", on_change);
 }
 ```
 
 > **Note**: In the snippet above, `on_change` is called an _**event handler**_
 > because it executes any time `my_value` is updated from either Python or the
 > front-end code (i.e., a _change_ event).
```

### Comparing `anywidget-0.4.1/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.4.2/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/styles/index.css` & `anywidget-0.4.2/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/docs/src/styles/theme.css` & `anywidget-0.4.2/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/examples/Counter.ipynb` & `anywidget-0.4.2/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/examples/minimal_example.ipynb` & `anywidget-0.4.2/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/packages/anywidget/CHANGELOG.md` & `anywidget-0.4.2/packages/anywidget/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # anywidget
 
+## 0.4.2
+
+### Patch Changes
+
+- fix(descriptor): forward base obj repr for text/plain mimetype ([#131](https://github.com/manzt/anywidget/pull/131))
+
 ## 0.4.1
 
 ### Patch Changes
 
 - feat: Add `anywidget.experimental` with simple decorator ([#126](https://github.com/manzt/anywidget/pull/126))
 
   ```python
```

### Comparing `anywidget-0.4.1/packages/anywidget/build.mjs` & `anywidget-0.4.2/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/packages/anywidget/package.json` & `anywidget-0.4.2/packages/anywidget/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.4.2'"}*

```diff
@@ -38,9 +38,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

### Comparing `anywidget-0.4.1/packages/anywidget/src/widget.js` & `anywidget-0.4.2/packages/anywidget/src/widget.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/tests/test_descriptor.py` & `anywidget-0.4.2/tests/test_descriptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,22 +63,26 @@
     )
 
 
 def test_descriptor(mock_comm: MagicMock) -> None:
     """Test that the descriptor decorator makes a comm, and gets/sets state."""
 
     VAL = 1
+    REPR = "FOO"
 
     class Foo:
         _repr_mimebundle_ = MimeBundleDescriptor(autodetect_observer=False)
         value: int = VAL
 
         def _get_anywidget_state(self):
             return {"value": self.value}
 
+        def __repr__(self) -> str:
+            return REPR
+
     foo = Foo()
     mock_comm.send.assert_not_called()  # we haven't yet created a comm object
 
     repr_method = foo._repr_mimebundle_  # the comm is created here
     mock_comm.send.assert_called_once()
     assert isinstance(repr_method, ReprMimeBundle)
     bundle = repr_method()
@@ -91,14 +95,17 @@
     # test that the object responds to incoming messages
     assert _send_value(mock_comm, 3) == foo.value
 
     mock_comm.send.reset_mock()
     mock_comm.handle_msg({"content": {"data": {"method": "request_state"}}})
     mock_comm.send.assert_called()
 
+    # uses the base class repr for plain text
+    assert foo._repr_mimebundle_()[0]["text/plain"] == REPR
+
 
 def test_state_setter(mock_comm: MagicMock):
     """Test that `_set_anywidget_state` is used when present."""
     mock = MagicMock()
 
     class Foo:
         _repr_mimebundle_ = MimeBundleDescriptor(autodetect_observer=False)
```

### Comparing `anywidget-0.4.1/tests/test_experimental.py` & `anywidget-0.4.2/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/tests/test_file_contents.py` & `anywidget-0.4.2/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/tests/test_utils.py` & `anywidget-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/tests/test_widget.py` & `anywidget-0.4.2/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/LICENSE` & `anywidget-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/README.md` & `anywidget-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/pyproject.toml` & `anywidget-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.1/PKG-INFO` & `anywidget-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.4.1
+Version: 0.4.2
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
```

