# Comparing `tmp/lektor-3.4.0b6.tar.gz` & `tmp/lektor-3.4.0b7.tar.gz`

## Comparing `lektor-3.4.0b6.tar` & `lektor-3.4.0b7.tar`

### file list

```diff
@@ -1,298 +1,299 @@
--rw-r--r--   0        0        0    43784 2020-02-02 00:00:00.000000 lektor-3.4.0b6/CHANGES.md
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lektor-3.4.0b6/build_frontend.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tox.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/__main__.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/assets.py
--rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/build_programs.py
--rw-r--r--   0        0        0    44698 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/builder.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/buildfailures.py
--rw-r--r--   0        0        0    19669 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/cli.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/cli_utils.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/compat.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/constants.py
--rw-r--r--   0        0        0     8091 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/context.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/databags.py
--rw-r--r--   0        0        0    23791 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/datamodel.py
--rw-r--r--   0        0        0    75332 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/db.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/devcli.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/devserver.py
--rw-r--r--   0        0        0    16718 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/editor.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/exception.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/filecontents.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/i18n.py
--rw-r--r--   0        0        0    25049 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/imagetools.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/metaformat.py
--rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/packages.py
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/pagination.py
--rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/pluginsystem.py
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/project.py
--rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/publisher.py
--rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart.py
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/reporter.py
--rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/sourceobj.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/sourcesearch.py
--rw-r--r--   0        0        0    27157 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/utils.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/videotools.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/watcher.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/__init__.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/context.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/utils.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/webui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/modules/__init__.py
--rw-r--r--   0        0        0    13890 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/modules/api.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/modules/dash.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/modules/livereload.py
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/modules/serve.py
--rw-r--r--   0        0        0   188451 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/app.css
--rw-r--r--   0        0        0    48161 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/app.css.map
--rw-r--r--   0        0        0   587740 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/app.js
--rw-r--r--   0        0        0   374972 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/app.js.map
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/fontawesome-webfont-5GKVPAEF.woff2
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-400-normal-72U6HY3C.woff2
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-700-normal-2TPID6WR.woff2
--rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-ext-400-normal-SGZKCMAU.woff2
--rw-r--r--   0        0        0    12192 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-ext-700-normal-CKGDQNG6.woff2
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-400-normal-FZE4RLDU.woff2
--rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-700-normal-5YAILM42.woff2
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-ext-400-normal-CARBXC53.woff2
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-ext-700-normal-MWV52O3F.woff2
--rw-r--r--   0        0        0    12608 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-400-normal-WDWDTZK2.woff2
--rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-700-normal-VK4QNPMO.woff2
--rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-ext-400-normal-66GAUH66.woff2
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-ext-700-normal-W2KTZJSB.woff2
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-vietnamese-400-normal-HHIQBQTZ.woff2
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/static/roboto-slab-vietnamese-700-normal-TQT4Y47C.woff2
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/base.html
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/build-failure.html
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/dash.html
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/edit-button.html
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/layout.html
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/livereload-worker.js
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/admin/templates/livereload.html
--rw-r--r--   0        0        0    14215 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/environment/__init__.py
--rw-r--r--   0        0        0     8878 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/environment/config.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/environment/expressions.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/markdown/__init__.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/markdown/controller.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/markdown/mistune0.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/markdown/mistune2.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/plugin/.gitignore.in
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/plugin/@plugin_module@.py.in
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/plugin/README.md.in
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/plugin/pyproject.toml.in
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/plugin/setup.cfg.in
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/@project_name@.lektorproject.in
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/assets/static/style.css.in
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/content/contents.lr.in
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/content/about/contents.lr.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/content/blog/contents.lr.in
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/content/blog/first-post/contents.lr.in
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/content/projects/contents.lr.in
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/models/blog-post.ini.in
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/models/blog.ini.in
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/models/page.ini.in
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/blog-post.html.in
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/blog.html.in
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/layout.html.in
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/page.html.in
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/macros/blog.html.in
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/project/templates/macros/pagination.html.in
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/theme/README.md.in
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/theme/theme.ini.in
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/theme/example-site/README.md.in
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/theme/example-site/lektor-theme-@theme_id@.lektorproject.in
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/quickstart-templates/theme/images/homepage.png
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/ca.json
--rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/de.json
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/en.json
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/es.json
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/fr.json
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/it.json
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/ja.json
--rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/ko.json
--rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/nl.json
--rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/pl.json
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/pt.json
--rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/ru.json
--rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/translations/zh.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/__init__.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/base.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/fake.py
--rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/flow.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/formats.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/multi.py
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/primitives.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 lektor-3.4.0b6/lektor/types/special.py
--rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/conftest.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_assets.py
--rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_build_frontend.py
--rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_builder.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_buildfailures.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_cli.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_cli_utils.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_compat.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_config.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_conftest.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_datamodel.py
--rw-r--r--   0        0        0    17301 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_db.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_deploy.py
--rw-r--r--   0        0        0    12560 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_devcli.py
--rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_editor.py
--rw-r--r--   0        0        0     5990 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_environment.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_filecontents.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_i18n.py
--rw-r--r--   0        0        0    21458 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_imagetools.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_imports.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_issue_410.py
--rw-r--r--   0        0        0    20914 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_markdown.py
--rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_packages.py
--rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_pagination.py
--rw-r--r--   0        0        0    12630 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_pluginsystem.py
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_prev_next_sibling.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_project.py
--rw-r--r--   0        0        0    21409 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_publisher.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_quickstart.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_sourceobj.py
--rw-r--r--   0        0        0     7342 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_themes.py
--rw-r--r--   0        0        0    13186 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_tree.py
--rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_types.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_unicode.py
--rw-r--r--   0        0        0    15464 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_urls.py
--rw-r--r--   0        0        0    10889 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_utils.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_videotools.py
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/test_watcher.py
--rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/admin/test_api.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/admin/test_dash.py
--rw-r--r--   0        0        0    20248 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/admin/test_serve.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/admin/test_webui.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/Website.lektorproject
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/content/attachment.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/content/contents.lr
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/content/filtered-page/contents.lr
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/models/bar.ini
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/models/foo.ini
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/models/page.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/templates/bar.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/templates/foo.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/child-sources-test-project/templates/page.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/Website.lektorproject
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/_include_me_despite_underscore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/foo-prefix-makes-me-excluded
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/dir_with_index_htm/index.htm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/dir_with_index_html/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/empty/.gitkeep
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/assets/static/demo.css
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/contents.lr
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/hello.txt
--rw-r--r--   0        0        0   201837 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/test-progressive.jpg
--rw-r--r--   0        0        0   208691 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/test-sof-last.jpg
--rw-r--r--   0        0        0   208691 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/test.jpg
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/test.mp4
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/blog/contents.lr
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/blog/dummy.xml/contents.lr
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/blog/post1/contents.lr
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/blog/post1/hello.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/blog/post2/contents.lr
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/colorspace-test/LICENSE.txt
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/colorspace-test/README.md
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/colorspace-test/contents.lr
--rw-r--r--   0        0        0    32912 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/colorspace-test/rgb-to-gbr-test.jpg
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/contents.lr
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/hello.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/a/contents.lr
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/b/contents.lr
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/container/contents.lr
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/container/hello.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/container/a/contents.lr
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/file.ext/contents.lr
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/paginated/contents+de.lr
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/paginated/contents.lr
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/extra/slash-slug/contents.lr
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/attachment.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/contents.lr
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/bagpipe/contents+de.lr
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/bagpipe/contents.lr
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/coffee/contents+de.lr
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/coffee/contents.lr
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/filtered/contents.lr
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/master/contents+de.lr
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/master/contents.lr
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/oven/contents+de.lr
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/oven/contents.lr
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/postage/contents+de.lr
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/postage/contents.lr
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/secret/contents.lr
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/slave/contents+de.lr
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/slave/contents.lr
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/wolf/contents.lr
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/content/projects/zaun/contents+de.lr
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/flowblocks/text.ini
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/blog-post.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/blog.ini
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/container.ini
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/page.ini
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/paginated.ini
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/project.ini
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/models/projects.ini
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/blog-post.html
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/blog.html
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/colorspace-test.html
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/dummy.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/layout.html
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/page.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/project.html
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/projects.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/demo-project/templates/blocks/text.html
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/Website.lektorproject
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/content/contents.lr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/content/post1/contents.lr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/content/post2/contents.lr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/content/post4/contents.lr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/models/blog-post.ini
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/models/blog.ini
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/templates/blog-post.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/dependency-test-project/templates/blog.html
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/pep660-dummy-plugin/lektor_dummy_plugin.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/pep660-dummy-plugin/pyproject.toml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/assets/asset.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/assets/dummy.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/flowblocks/text.ini
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/models/blog-post.ini
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/models/page.ini
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/templates/layout.html
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/templates/page.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/templates/blocks/text.html
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/theme.ini
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/assets/dummy.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/assets/dummy2.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/assets/static/blog.css
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/models/blog-post.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/models/blog.ini
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/models/project.ini
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/templates/blog-post.html
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/templates/blog.html
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/templates/dummy.html
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/blog_theme/templates/layout.html
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/theme.ini
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/assets/dummy2.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/assets/static/project.css
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/flowblocks/text.ini
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/models/project.ini
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/models/projects.ini
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/templates/dummy.html
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/templates/layout.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/templates/project.html
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/templates/projects.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/themes-project/themes/project_theme/templates/blocks/text.html
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/test.lektorproject
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/content/contents.lr
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/content/ättachment
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/content/bäd/contents.lr
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/models/page.ini
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 lektor-3.4.0b6/tests/ünicöde-project/templates/page.html
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 lektor-3.4.0b6/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 lektor-3.4.0b6/LICENSE
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 lektor-3.4.0b6/README.md
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 lektor-3.4.0b6/pyproject.toml
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 lektor-3.4.0b6/PKG-INFO
+-rw-r--r--   0        0        0    44960 2020-02-02 00:00:00.000000 lektor-3.4.0b7/CHANGES.md
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lektor-3.4.0b7/build_frontend.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tox.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/__main__.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/assets.py
+-rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/build_programs.py
+-rw-r--r--   0        0        0    44537 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/builder.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/buildfailures.py
+-rw-r--r--   0        0        0    19429 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/cli.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/cli_utils.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/compat.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/constants.py
+-rw-r--r--   0        0        0     8091 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/context.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/databags.py
+-rw-r--r--   0        0        0    23791 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/datamodel.py
+-rw-r--r--   0        0        0    75332 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/db.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/devcli.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/devserver.py
+-rw-r--r--   0        0        0    16718 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/editor.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/exception.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/filecontents.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/i18n.py
+-rw-r--r--   0        0        0    25049 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/imagetools.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/metaformat.py
+-rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/packages.py
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/pagination.py
+-rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/pluginsystem.py
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/project.py
+-rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/publisher.py
+-rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/reporter.py
+-rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/sourceobj.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/sourcesearch.py
+-rw-r--r--   0        0        0    26773 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/utils.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/videotools.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/watcher.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/__init__.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/context.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/utils.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/webui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/modules/__init__.py
+-rw-r--r--   0        0        0    13890 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/modules/api.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/modules/dash.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/modules/livereload.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/modules/serve.py
+-rw-r--r--   0        0        0   188451 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/app.css
+-rw-r--r--   0        0        0    48161 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/app.css.map
+-rw-r--r--   0        0        0   587740 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/app.js
+-rw-r--r--   0        0        0   374972 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/app.js.map
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/fontawesome-webfont-5GKVPAEF.woff2
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-cyrillic-400-normal-72U6HY3C.woff2
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-cyrillic-700-normal-2TPID6WR.woff2
+-rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-cyrillic-ext-400-normal-SGZKCMAU.woff2
+-rw-r--r--   0        0        0    12192 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-cyrillic-ext-700-normal-CKGDQNG6.woff2
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-greek-400-normal-FZE4RLDU.woff2
+-rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-greek-700-normal-5YAILM42.woff2
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-greek-ext-400-normal-CARBXC53.woff2
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-greek-ext-700-normal-MWV52O3F.woff2
+-rw-r--r--   0        0        0    12608 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-latin-400-normal-WDWDTZK2.woff2
+-rw-r--r--   0        0        0    12820 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-latin-700-normal-VK4QNPMO.woff2
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-latin-ext-400-normal-66GAUH66.woff2
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-latin-ext-700-normal-W2KTZJSB.woff2
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-vietnamese-400-normal-HHIQBQTZ.woff2
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/static/roboto-slab-vietnamese-700-normal-TQT4Y47C.woff2
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/templates/base.html
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/templates/build-failure.html
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/templates/dash.html
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/templates/edit-button.html
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/templates/layout.html
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/templates/livereload-worker.js
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/admin/templates/livereload.html
+-rw-r--r--   0        0        0    14215 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/environment/__init__.py
+-rw-r--r--   0        0        0     8878 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/environment/config.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/environment/expressions.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/markdown/__init__.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/markdown/controller.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/markdown/mistune0.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/markdown/mistune2.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/plugin/.gitignore.in
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/plugin/@plugin_module@.py.in
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/plugin/README.md.in
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/plugin/pyproject.toml.in
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/plugin/setup.cfg.in
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/@project_name@.lektorproject.in
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/assets/static/style.css.in
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/content/contents.lr.in
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/content/about/contents.lr.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/content/blog/contents.lr.in
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/content/blog/first-post/contents.lr.in
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/content/projects/contents.lr.in
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/models/blog-post.ini.in
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/models/blog.ini.in
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/models/page.ini.in
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/templates/blog-post.html.in
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/templates/blog.html.in
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/templates/layout.html.in
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/templates/page.html.in
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/templates/macros/blog.html.in
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/project/templates/macros/pagination.html.in
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/theme/README.md.in
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/theme/theme.ini.in
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/theme/example-site/README.md.in
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/theme/example-site/lektor-theme-@theme_id@.lektorproject.in
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/quickstart-templates/theme/images/homepage.png
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/ca.json
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/de.json
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/en.json
+-rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/es.json
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/fr.json
+-rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/it.json
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/ja.json
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/ko.json
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/nl.json
+-rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/pl.json
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/pt.json
+-rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/ru.json
+-rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/translations/zh.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/types/__init__.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/types/base.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/types/fake.py
+-rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/types/flow.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/types/formats.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/types/multi.py
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/types/primitives.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 lektor-3.4.0b7/lektor/types/special.py
+-rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/conftest.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_assets.py
+-rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_build_frontend.py
+-rw-r--r--   0        0        0    11901 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_builder.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_buildfailures.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_cli.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_cli_utils.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_compat.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_config.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_conftest.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_datamodel.py
+-rw-r--r--   0        0        0    17301 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_db.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_deploy.py
+-rw-r--r--   0        0        0    12560 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_devcli.py
+-rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_editor.py
+-rw-r--r--   0        0        0     5990 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_environment.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_filecontents.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_i18n.py
+-rw-r--r--   0        0        0    21458 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_imagetools.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_imports.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_issue_410.py
+-rw-r--r--   0        0        0    20914 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_markdown.py
+-rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_packages.py
+-rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_pagination.py
+-rw-r--r--   0        0        0    12630 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_pluginsystem.py
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_prev_next_sibling.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_project.py
+-rw-r--r--   0        0        0    21409 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_publisher.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_quickstart.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_reporter.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_sourceobj.py
+-rw-r--r--   0        0        0     7342 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_themes.py
+-rw-r--r--   0        0        0    13186 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_tree.py
+-rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_types.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_unicode.py
+-rw-r--r--   0        0        0    15464 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_urls.py
+-rw-r--r--   0        0        0    10889 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_utils.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_videotools.py
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/test_watcher.py
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/admin/test_api.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/admin/test_dash.py
+-rw-r--r--   0        0        0    20248 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/admin/test_serve.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/admin/test_webui.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/child-sources-test-project/Website.lektorproject
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/child-sources-test-project/content/attachment.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/child-sources-test-project/content/contents.lr
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/child-sources-test-project/content/filtered-page/contents.lr
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/child-sources-test-project/models/bar.ini
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/child-sources-test-project/models/foo.ini
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/child-sources-test-project/models/page.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/child-sources-test-project/templates/bar.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/child-sources-test-project/templates/foo.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/child-sources-test-project/templates/page.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/Website.lektorproject
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/assets/_include_me_despite_underscore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/assets/foo-prefix-makes-me-excluded
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/assets/dir_with_index_htm/index.htm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/assets/dir_with_index_html/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/assets/empty/.gitkeep
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/assets/static/demo.css
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/contents.lr
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/hello.txt
+-rw-r--r--   0        0        0   201837 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/test-progressive.jpg
+-rw-r--r--   0        0        0   208691 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/test-sof-last.jpg
+-rw-r--r--   0        0        0   208691 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/test.jpg
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/test.mp4
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/blog/contents.lr
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/blog/dummy.xml/contents.lr
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/blog/post1/contents.lr
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/blog/post1/hello.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/blog/post2/contents.lr
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/colorspace-test/LICENSE.txt
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/colorspace-test/README.md
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/colorspace-test/contents.lr
+-rw-r--r--   0        0        0    32912 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/colorspace-test/rgb-to-gbr-test.jpg
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/contents.lr
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/hello.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/a/contents.lr
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/b/contents.lr
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/container/contents.lr
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/container/hello.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/container/a/contents.lr
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/file.ext/contents.lr
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/paginated/contents+de.lr
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/paginated/contents.lr
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/extra/slash-slug/contents.lr
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/attachment.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/contents.lr
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/bagpipe/contents+de.lr
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/bagpipe/contents.lr
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/coffee/contents+de.lr
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/coffee/contents.lr
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/filtered/contents.lr
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/master/contents+de.lr
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/master/contents.lr
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/oven/contents+de.lr
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/oven/contents.lr
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/postage/contents+de.lr
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/postage/contents.lr
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/secret/contents.lr
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/slave/contents+de.lr
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/slave/contents.lr
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/wolf/contents.lr
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/content/projects/zaun/contents+de.lr
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/flowblocks/text.ini
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/models/blog-post.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/models/blog.ini
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/models/container.ini
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/models/page.ini
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/models/paginated.ini
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/models/project.ini
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/models/projects.ini
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/templates/blog-post.html
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/templates/blog.html
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/templates/colorspace-test.html
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/templates/dummy.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/templates/layout.html
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/templates/page.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/templates/project.html
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/templates/projects.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/demo-project/templates/blocks/text.html
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/dependency-test-project/Website.lektorproject
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/dependency-test-project/content/contents.lr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/dependency-test-project/content/post1/contents.lr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/dependency-test-project/content/post2/contents.lr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/dependency-test-project/content/post4/contents.lr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/dependency-test-project/models/blog-post.ini
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/dependency-test-project/models/blog.ini
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/dependency-test-project/templates/blog-post.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/dependency-test-project/templates/blog.html
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/pep660-dummy-plugin/lektor_dummy_plugin.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/pep660-dummy-plugin/pyproject.toml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/assets/asset.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/assets/dummy.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/flowblocks/text.ini
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/models/blog-post.ini
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/models/page.ini
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/templates/layout.html
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/templates/page.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/templates/blocks/text.html
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/theme.ini
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/assets/dummy.txt
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/assets/dummy2.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/assets/static/blog.css
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/models/blog-post.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/models/blog.ini
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/models/project.ini
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/templates/blog-post.html
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/templates/blog.html
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/templates/dummy.html
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/blog_theme/templates/layout.html
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/theme.ini
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/assets/dummy2.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/assets/static/project.css
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/flowblocks/text.ini
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/models/project.ini
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/models/projects.ini
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/templates/dummy.html
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/templates/layout.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/templates/project.html
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/templates/projects.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/themes-project/themes/project_theme/templates/blocks/text.html
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/ünicöde-project/test.lektorproject
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/ünicöde-project/content/contents.lr
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/ünicöde-project/content/ättachment
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/ünicöde-project/content/bäd/contents.lr
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/ünicöde-project/models/page.ini
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 lektor-3.4.0b7/tests/ünicöde-project/templates/page.html
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 lektor-3.4.0b7/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 lektor-3.4.0b7/LICENSE
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 lektor-3.4.0b7/README.md
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 lektor-3.4.0b7/pyproject.toml
+-rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 lektor-3.4.0b7/PKG-INFO
```

### Comparing `lektor-3.4.0b6/CHANGES.md` & `lektor-3.4.0b7/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 # Changelog
 
 These are all the changes in Lektor since the first public release.
 
+## 3.4.0b7 (2023-06-04)
+
+### Slightly Breaking Changes
+
+- The `--profile` option has been removed from the `lektor build` command. ([#1137])
+
+### Bugs Fixed
+
+- Pin `watchfiles>=0.12`. (Our tests use the `stop_event` parameter of `watchfiles.watch`.)
+- Fix exception from `describe_build_func` when building thumbnails with verbose logging enabled.
+- Fix "FATAL: exception not rethrown" message when `lektor server` is stopped. ([#1145])
+- Fix multiple browser new tabs when `lektor server --browse` is used with `LEKTOR_DEV` set ([#1145])
+- Fix mypy errors in `lektor.admin.modules`.
+- Fix `Builder.touch_site_config` so that it actually touches the site
+  config. This fixes the _Refresh Build_ button of the admin
+  UI. ([#1146])
+- Ensure that `Artifact.open` respects the value of its `encoding` argument when opening files. ([#1146])
+- Fix logic flaw in `FileInfo.unchanged` which, under certain
+  circumstances, causes source files to be considered unchanged even
+  if their size (or mtime) is changed. ([#1146])
+
+[#1137]: https://github.com/lektor/lektor/pull/1137
+[#1145]: https://github.com/lektor/lektor/pull/1145
+[#1146]: https://github.com/lektor/lektor/pull/1146
+
 ## 3.4.0b6 (2023-05-05)
 
 ### Possibly Breaking Changes
 
 - Our Publisher API has changed. This will eventually require updates
   to any custom Publisher classes provided by Lektor
   plugins. Previously, the `publish` method of `Publisher` subclasses
```

### Comparing `lektor-3.4.0b6/build_frontend.py` & `lektor-3.4.0b7/build_frontend.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tox.ini` & `lektor-3.4.0b7/tox.ini`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/assets.py` & `lektor-3.4.0b7/lektor/assets.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/build_programs.py` & `lektor-3.4.0b7/lektor/build_programs.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/builder.py` & `lektor-3.4.0b7/lektor/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import sys
 import tempfile
 from collections import deque
 from collections import namedtuple
 from contextlib import contextmanager
 from dataclasses import dataclass
 from itertools import chain
+from typing import Any
+from typing import IO
 
 import click
 
 from lektor.build_programs import builtin_build_programs
 from lektor.buildfailures import FailureController
 from lektor.constants import PRIMARY_ALT
 from lektor.context import Context
@@ -569,20 +571,21 @@
     def unchanged(self, other):
         """Given another file info checks if the are similar enough to
         not consider it changed.
         """
         if not isinstance(other, FileInfo):
             raise TypeError("'other' must be a FileInfo, not %r" % other)
 
+        if self.mtime != other.mtime or self.size != other.size:
+            return False
         # If mtime and size match, we skip the checksum comparison which
         # might require a file read which we do not want in those cases.
         # (Except if it's a directory, then we won't do that)
-        if not self.is_dir and self.mtime == other.mtime and self.size == other.size:
+        if not self.is_dir:
             return True
-
         return self.checksum == other.checksum
 
     def is_changed(self, build_state: BuildState) -> bool:
         other = build_state.get_file_info(self.filename)
         return not self.unchanged(other)
 
 
@@ -706,34 +709,34 @@
         """Creates the directory if it does not exist yet."""
         dst_dir = os.path.dirname(self.dst_filename)
         try:
             os.makedirs(dst_dir)
         except OSError:
             pass
 
-    def open(self, mode="rb", encoding=None, ensure_dir=None):
+    def open(
+        self, mode: str = "rb", encoding: str | None = None, ensure_dir: bool = True
+    ) -> IO[Any]:
         """Opens the artifact for reading or writing.  This is transaction
         safe by writing into a temporary file and by moving it over the
         actual source in commit.
         """
-        if ensure_dir is None:
-            ensure_dir = "r" not in mode
+        if self._new_artifact_file is not None:
+            return open(self._new_artifact_file, mode, encoding=encoding)
+
+        if "r" in mode:
+            return open(self.dst_filename, mode, encoding=encoding)
+
         if ensure_dir:
             self.ensure_dir()
-        if "r" in mode:
-            fn = self._new_artifact_file or self.dst_filename
-            return open(fn, mode=mode, encoding=encoding)
-        if self._new_artifact_file is None:
-            fd, tmp_filename = tempfile.mkstemp(
-                dir=os.path.dirname(self.dst_filename), prefix=".__trans"
-            )
-            os.chmod(tmp_filename, 0o644)
-            self._new_artifact_file = tmp_filename
-            return os.fdopen(fd, mode)
-        return open(self._new_artifact_file, mode=mode, encoding=encoding)
+        fd, self._new_artifact_file = tempfile.mkstemp(
+            dir=os.path.dirname(self.dst_filename),
+            prefix=".__trans",
+        )
+        return open(fd, mode, encoding=encoding)
 
     def replace_with_file(self, filename, ensure_dir=True, copy=False):
         """This is similar to open but it will move over a given named
         file.  The file will be deleted by a rollback or renamed by a
         commit.
         """
         if ensure_dir:
@@ -742,17 +745,15 @@
             with self.open("wb") as df:
                 with open(filename, "rb") as sf:
                     shutil.copyfileobj(sf, df)
         else:
             self._new_artifact_file = filename
 
     def render_template_into(self, template_name, this, **extra):
-        """Renders a template into the artifact.  The default behavior is to
-        catch the error and render it into the template with a failure marker.
-        """
+        """Renders a template into the artifact."""
         rv = self.build_state.env.render_template(
             template_name, self.build_state.pad, this=this, **extra
         )
         with self.open("wb") as f:
             f.write(rv.encode("utf-8") + b"\n")
 
     def _memorize_dependencies(
@@ -1126,16 +1127,17 @@
         cur.execute("pragma synchronous=NORMAL")
         con.commit()
         cur.close()
         return con
 
     def touch_site_config(self):
         """Touches the site config which typically will trigger a rebuild."""
+        project_file = self.env.project.project_file
         try:
-            os.utime(os.path.join(self.env.root_path, "site.ini"), None)
+            os.utime(project_file)
         except OSError:
             pass
 
     def find_files(self, query, alt=PRIMARY_ALT, lang=None, limit=50, types=None):
         """Returns a list of files that match the query.  This requires that
         the source info is up to date and is primarily used by the admin to
         show files that exist.
```

### Comparing `lektor-3.4.0b6/lektor/buildfailures.py` & `lektor-3.4.0b7/lektor/buildfailures.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/cli.py` & `lektor-3.4.0b7/lektor/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from lektor.cli_utils import extraflag
 from lektor.cli_utils import pass_context
 from lektor.cli_utils import pruneflag
 from lektor.cli_utils import ResolvedPath
 from lektor.cli_utils import validate_language
 from lektor.compat import importlib_metadata as metadata
 from lektor.project import Project
-from lektor.utils import profile_func
 from lektor.utils import secure_url
 
 
 version = metadata.version("Lektor")
 
 
 @click.group(cls=AliasedGroup)
@@ -86,25 +85,23 @@
     type=click.Path(writable=True, file_okay=False),
     default=None,
     help="Path to a directory that Lektor will use for coordinating "
     "the state of the build. Defaults to a directory named "
     "`.lektor` inside the output path.",
 )
 @extraflag
-@click.option("--profile", is_flag=True, help="Enable build profiler.")
 @pass_context
 def build_cmd(
     ctx,
     output_path,
     watch,
     prune,
     verbosity,
     source_info_only,
     buildstate_path,
-    profile,
     extra_flags,
 ):
     """Builds the entire project into the final artifacts.
 
     The default behavior is to build the project into the default build
     output path which can be discovered with the `project-info` command
     but an alternative output folder can be provided with the `--output-path`
@@ -148,18 +145,15 @@
                 buildstate_path=buildstate_path,
                 extra_flags=extra_flags,
             )
             if source_info_only:
                 builder.update_all_source_infos()
                 success = True
             else:
-                if profile:
-                    failures = profile_func(builder.build_all)
-                else:
-                    failures = builder.build_all()
+                failures = builder.build_all()
                 if prune:
                     builder.prune()
                 success = failures == 0
 
         return sys.exit(0 if success else 1)
```

### Comparing `lektor-3.4.0b6/lektor/cli_utils.py` & `lektor-3.4.0b7/lektor/cli_utils.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/compat.py` & `lektor-3.4.0b7/lektor/compat.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/context.py` & `lektor-3.4.0b7/lektor/context.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/databags.py` & `lektor-3.4.0b7/lektor/databags.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/datamodel.py` & `lektor-3.4.0b7/lektor/datamodel.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/db.py` & `lektor-3.4.0b7/lektor/db.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/devcli.py` & `lektor-3.4.0b7/lektor/devcli.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/devserver.py` & `lektor-3.4.0b7/lektor/devserver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,152 @@
-import os
+from __future__ import annotations
+
+import logging
 import threading
-import time
 import traceback
-from itertools import chain
+import webbrowser
+from contextlib import ExitStack
+from typing import NamedTuple
+from typing import TYPE_CHECKING
 
+from werkzeug.serving import is_running_from_reloader
 from werkzeug.serving import run_simple
-from werkzeug.serving import WSGIRequestHandler
 
 from lektor.admin import WebAdmin
 from lektor.builder import Builder
 from lektor.db import Database
 from lektor.reporter import CliReporter
 from lektor.utils import process_extra_flags
 from lektor.watcher import watch_project
 
-
-class SilentWSGIRequestHandler(WSGIRequestHandler):
-    def log(self, type, message, *args):
-        pass
+if TYPE_CHECKING:
+    from _typeshed import StrPath
+    from lektor.environment import Environment
 
 
 class BackgroundBuilder(threading.Thread):
-    def __init__(self, env, output_path, prune=True, verbosity=0, extra_flags=None):
+    """Run a thread to watch the project tree and rebuild when changes are noticed.
+
+    This is a contextmanager. On entry, the watcher thread is started, on exit it is
+    stopped.
+
+    """
+
+    def __init__(
+        self,
+        env: Environment,
+        output_path: StrPath,
+        prune: bool = True,
+        verbosity: int = 0,
+        extra_flags: dict[str, str] | None = None,
+    ):
         threading.Thread.__init__(self)
         self.env = env
         self.output_path = output_path
         self.prune = prune
         self.verbosity = verbosity
         self.extra_flags = extra_flags
 
-    def build(self, update_source_info_first=False):
+        # See https://github.com/samuelcolvin/watchfiles/pull/132
+        self.stop_event = threading.Event()
+
+    def __enter__(self) -> BackgroundBuilder:
+        self.start()
+        return self
+
+    def __exit__(self, *args: object) -> None:
+        self.stop_event.set()
+
+    def build(self, update_source_info_first: bool = False) -> None:
         try:
             db = Database(self.env)
             builder = Builder(
                 db.new_pad(), self.output_path, extra_flags=self.extra_flags
             )
             if update_source_info_first:
                 builder.update_all_source_infos()
             builder.build_all()
             if self.prune:
                 builder.prune()
         except Exception:
             traceback.print_exc()
 
-    def run(self):
-        builds = chain(["first"], watch_project(self.env, self.output_path))
+    def run(self) -> None:
+        watch = watch_project(self.env, self.output_path, stop_event=self.stop_event)
         with CliReporter(self.env, verbosity=self.verbosity):
-            for n, _ in enumerate(builds):
-                is_first_build = n == 0
-                self.build(update_source_info_first=is_first_build)
-
-
-def browse_to_address(addr):
-    # pylint: disable=import-outside-toplevel
-    import webbrowser
-
-    def browse():
-        time.sleep(1)
-        webbrowser.open("http://%s:%s" % addr)
-
-    t = threading.Thread(target=browse)
-    t.daemon = True
-    t.start()
+            self.build(update_source_info_first=True)
+            for _changes in watch:
+                self.build()
+
+
+class BindAddr(NamedTuple):
+    host: str
+    port: int
+
+
+def browse_to_address(addr: BindAddr) -> None:
+    timer = threading.Timer(1.0, webbrowser.open, (f"http://{addr.host}:{addr.port}",))
+    timer.daemon = True
+    timer.start()
 
 
 def run_server(
-    bindaddr,
-    env,
-    output_path,
-    prune=True,
-    verbosity=0,
-    lektor_dev=False,
-    ui_lang="en",
-    browse=False,
-    extra_flags=None,
-    reload=True,
-):
+    bindaddr: BindAddr,
+    env: Environment,
+    output_path: StrPath,
+    prune: bool = True,
+    verbosity: int = 0,
+    lektor_dev: bool = False,
+    ui_lang: str = "en",
+    browse: bool = False,
+    extra_flags: dict[str, str] | None = None,
+    reload: bool = True,
+) -> None:
     """This runs a server but also spawns a background process.  It's
     not safe to call this more than once per python process!
     """
-    wz_as_main = os.environ.get("WERKZEUG_RUN_MAIN") == "true"
-    in_main_process = not lektor_dev or wz_as_main
+    bindaddr = BindAddr._make(bindaddr)
+
+    in_main_process = is_running_from_reloader() or not lektor_dev
     extra_flags = process_extra_flags(extra_flags)
     if lektor_dev:
         env.jinja_env.add_extension("jinja2.ext.debug")
-
-    if in_main_process:
-        background_builder = BackgroundBuilder(
-            env,
-            output_path=output_path,
-            prune=prune,
-            verbosity=verbosity,
-            extra_flags=extra_flags,
-        )
-        background_builder.daemon = True
-        background_builder.start()
-        env.plugin_controller.emit(
-            "server-spawn", bindaddr=bindaddr, extra_flags=extra_flags
-        )
+    else:
+        logging.getLogger("werkzeug").setLevel(logging.WARNING)
 
     app = WebAdmin(
         env,
         output_path=output_path,
         verbosity=verbosity,
         debug=lektor_dev,
         ui_lang=ui_lang,
         extra_flags=extra_flags,
         reload=reload,
     )
 
-    if browse:
+    if browse and not is_running_from_reloader():
         browse_to_address(bindaddr)
 
-    try:
-        return run_simple(
-            bindaddr[0],
-            bindaddr[1],
+    with ExitStack() as stack:
+        if in_main_process:
+            env.plugin_controller.emit(
+                "server-spawn", bindaddr=bindaddr, extra_flags=extra_flags
+            )
+            stack.callback(env.plugin_controller.emit, "server-stop")
+
+            background_builder = BackgroundBuilder(
+                env,
+                output_path=output_path,
+                prune=prune,
+                verbosity=verbosity,
+                extra_flags=extra_flags,
+            )
+            stack.enter_context(background_builder)
+
+        run_simple(
+            bindaddr.host,
+            bindaddr.port,
             app,
             use_debugger=True,
             threaded=True,
             use_reloader=lektor_dev,
-            request_handler=WSGIRequestHandler
-            if lektor_dev
-            else SilentWSGIRequestHandler,
         )
-    finally:
-        if in_main_process:
-            env.plugin_controller.emit("server-stop")
```

### Comparing `lektor-3.4.0b6/lektor/editor.py` & `lektor-3.4.0b7/lektor/editor.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/exception.py` & `lektor-3.4.0b7/lektor/exception.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/filecontents.py` & `lektor-3.4.0b7/lektor/filecontents.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/i18n.py` & `lektor-3.4.0b7/lektor/i18n.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/imagetools.py` & `lektor-3.4.0b7/lektor/imagetools.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/metaformat.py` & `lektor-3.4.0b7/lektor/metaformat.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/packages.py` & `lektor-3.4.0b7/lektor/packages.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/pagination.py` & `lektor-3.4.0b7/lektor/pagination.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/pluginsystem.py` & `lektor-3.4.0b7/lektor/pluginsystem.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/project.py` & `lektor-3.4.0b7/lektor/project.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/publisher.py` & `lektor-3.4.0b7/lektor/publisher.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/quickstart.py` & `lektor-3.4.0b7/lektor/quickstart.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/reporter.py` & `lektor-3.4.0b7/lektor/reporter.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,20 +9,25 @@
 
 
 _reporter_stack = LocalStack()
 _build_buffer_stack = LocalStack()
 
 
 def describe_build_func(func):
-    self = getattr(func, "__self__", None)
-    if self is not None and any(
-        x.__name__ == "BuildProgram" for x in self.__class__.__mro__
-    ):
-        return self.__class__.__module__ + "." + self.__class__.__name__
-    return func.__module__ + "." + func.__name__
+    if hasattr(func, "func"):
+        func = func.func  # unwrap functools.partial
+    try:
+        qualname = func.__qualname__
+        class_name, _, method = qualname.rpartition(".")
+        if class_name and method == "build_artifact":
+            # Strip method name from methods of BuildProgram instances
+            qualname = class_name
+        return f"{func.__module__}.{qualname}"
+    except AttributeError:
+        return repr(func)
 
 
 class Reporter:
     _change_callbacks = set()
 
     def __init__(self, env, verbosity=0):
         self.env = env
@@ -399,13 +404,16 @@
     def report_pruned_artifact(self, artifact_name):
         self._write_line("%s %s" % (style("D", fg="red"), artifact_name))
 
 
 null_reporter = NullReporter(None)
 
 
+reporter: Reporter
+
+
 @LocalProxy
 def reporter():
     rv = _reporter_stack.top
     if rv is None:
         rv = null_reporter
     return rv
```

### Comparing `lektor-3.4.0b6/lektor/sourceobj.py` & `lektor-3.4.0b7/lektor/sourceobj.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/sourcesearch.py` & `lektor-3.4.0b7/lektor/sourcesearch.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/utils.py` & `lektor-3.4.0b7/lektor/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -660,32 +660,14 @@
             # prepend the distance to the common ancestor
             return distance / relpath
     # We should never get here.  (The last ancestor in source.parents will
     # be '.' — target.relative_to('.') will always succeed.)
     raise AssertionError("This should not happen")
 
 
-def profile_func(func):
-    # pylint: disable=import-outside-toplevel
-
-    from cProfile import Profile
-    from pstats import Stats
-
-    p = Profile()
-    rv = []
-    p.runcall(lambda: rv.append(func()))
-    p.dump_stats("/tmp/lektor-%s.prof" % func.__name__)
-
-    stats = Stats(p, stream=sys.stderr)
-    stats.sort_stats("time", "calls")
-    stats.print_stats()
-
-    return rv[0]
-
-
 def deg_to_dms(deg):
     d = int(deg)
     md = abs(deg - d) * 60
     m = int(md)
     sd = (md - m) * 60
     return (d, m, sd)
```

### Comparing `lektor-3.4.0b6/lektor/videotools.py` & `lektor-3.4.0b7/lektor/videotools.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/watcher.py` & `lektor-3.4.0b7/lektor/watcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import os
-from pathlib import Path
 from typing import Any
 from typing import Generator
 from typing import TYPE_CHECKING
 
 import watchfiles
 
 from lektor.utils import get_cache_dir
 
 if TYPE_CHECKING:
+    from _typeshed import StrPath
     from lektor.environment import Environment
 
 
 def watch_project(
-    env: Environment, output_path: str | Path, **kwargs: Any
-) -> Generator[[watchfiles.Change, str], None, None]:
+    env: Environment, output_path: StrPath, **kwargs: Any
+) -> Generator[set[watchfiles.FileChange], None, None]:
     """Watch project source files for changes.
 
     Returns an generator that yields sets of changes as they are noticed.
 
     Changes to files within ``output_path`` are ignored, along with other files
     deemed not to be Lektor source files.
```

### Comparing `lektor-3.4.0b6/lektor/admin/context.py` & `lektor-3.4.0b7/lektor/admin/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+from __future__ import annotations
+
 from typing import Any
 from typing import NamedTuple
-from typing import Optional
-from typing import Sequence
 from typing import TYPE_CHECKING
-from typing import Union
 
 from flask import current_app
 from flask import Flask
 from flask import g
 from werkzeug.utils import cached_property
 
 from lektor.builder import Builder
@@ -16,22 +15,22 @@
 from lektor.db import Pad
 from lektor.db import Tree
 from lektor.environment import Environment
 from lektor.environment.config import Config
 from lektor.reporter import CliReporter
 
 if TYPE_CHECKING:
-    import os
+    from _typeshed import StrPath
 
 
 class LektorInfo(NamedTuple):
     env: Environment
-    output_path: Union[str, "os.PathLike[Any]"]
+    output_path: StrPath
     verbosity: int = 0
-    extra_flags: Optional[Sequence[str]] = None
+    extra_flags: dict[str, str] | None = None
 
 
 class LektorContext(LektorInfo):
     """Per-request object which provides the interface to Lektor for the Flask app(s).
 
     This does not provide any logic.  It just provides access to the
     needed Lektor internals and instances.
```

### Comparing `lektor-3.4.0b6/lektor/admin/utils.py` & `lektor-3.4.0b7/lektor/admin/utils.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/webui.py` & `lektor-3.4.0b7/lektor/admin/webui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-from typing import Optional
-from typing import Sequence
+from __future__ import annotations
+
 from typing import TYPE_CHECKING
-from typing import Union
 from wsgiref.util import shift_path_info
 
 from flask import Flask
 from flask import request
 
 from lektor.admin.context import LektorApp
 from lektor.admin.context import LektorInfo
 from lektor.admin.modules import api
 from lektor.admin.modules import dash
 from lektor.admin.modules import livereload
 from lektor.admin.modules import serve
 from lektor.environment import Environment
 
 if TYPE_CHECKING:
-    import os
-    from typing import Any
+    from _typeshed import StrPath
     from _typeshed.wsgi import WSGIApplication
 
 
 def _common_configuration(app: Flask, debug: bool = False) -> None:
     app.debug = debug
     app.config["PROPAGATE_EXCEPTIONS"] = True
 
 
 def make_app(
     env: Environment,
     debug: bool = False,
-    output_path: Optional[Union[str, "os.PathLike[Any]"]] = None,
+    output_path: StrPath | None = None,
     ui_lang: str = "en",
     verbosity: int = 0,
-    extra_flags: Optional[Sequence[str]] = None,
+    extra_flags: dict[str, str] | None = None,
     reload: bool = True,
     *,
     admin_path: str = "/admin",
-    static_folder: Optional[Union[str, "os.PathLike[Any]"]] = "static",  # testing
+    static_folder: StrPath | None = "static",  # testing
 ) -> LektorApp:
     if output_path is None:
         output_path = env.project.get_output_path()
 
     lektor_info = LektorInfo(env, output_path, verbosity, extra_flags)
 
     # The top-level app has a route that matches anything
```

### Comparing `lektor-3.4.0b6/lektor/admin/modules/api.py` & `lektor-3.4.0b7/lektor/admin/modules/api.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/modules/dash.py` & `lektor-3.4.0b7/lektor/admin/modules/dash.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/modules/serve.py` & `lektor-3.4.0b7/lektor/admin/modules/serve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,48 @@
+from __future__ import annotations
+
 import mimetypes
 import os
 import re
 from pathlib import Path
 from typing import Match
 from typing import Optional
 from typing import Tuple
+from typing import TYPE_CHECKING
 from typing import Union
 from zlib import adler32
 
 from flask import abort
 from flask import Blueprint
 from flask import current_app
 from flask import render_template
 from flask import request
 from flask import Response
 from flask import send_file
 from flask import url_for
-from flask.typing import ResponseReturnValue
 from werkzeug.exceptions import NotFound
 from werkzeug.security import safe_join
 from werkzeug.utils import append_slash_redirect
 
 from lektor.admin.context import get_lektor_context
 from lektor.admin.context import LektorApp
 from lektor.admin.context import LektorContext
 from lektor.assets import Asset
 from lektor.assets import Directory
-from lektor.builder import Artifact
-from lektor.buildfailures import BuildFailure
 from lektor.constants import PRIMARY_ALT
 from lektor.db import Record
-from lektor.sourceobj import SourceObject
+
+if TYPE_CHECKING:
+    from flask.typing import ResponseReturnValue
+    from flask.typing import ResponseValue
+
+    from lektor.builder import Artifact
+    from lektor.buildfailures import BuildFailure
+    from lektor.sourceobj import SourceObject
+
 
 bp = Blueprint("serve", __name__)
 
 
 Filename = Union[str, os.PathLike]
 
 
@@ -53,15 +61,15 @@
         return button.encode("utf-8") + m.group(0)
 
     return re.sub(rb"(?i)</\s*head\s*>|\Z", extras, html, count=1)
 
 
 def _send_html_for_editing(
     artifact: Artifact, edit_url: str, mimetype: str = "text/html"
-) -> Response:
+) -> ResponseValue:
     """Serve an HTML file, after mangling it to add an "edit pencil" button."""
     try:
         with open(artifact.dst_filename, "rb") as fp:
             html = fp.read()
             st = os.stat(fp.fileno())
     except (FileNotFoundError, IsADirectoryError, PermissionError):
         abort(404)
@@ -75,15 +83,17 @@
 def _deduce_mimetype(filename: Filename) -> str:
     mimetype = mimetypes.guess_type(filename)[0]
     if mimetype is None:
         mimetype = "application/octet-stream"
     return mimetype
 
 
-def _checked_send_file(filename: Filename, mimetype: Optional[str] = None) -> Response:
+def _checked_send_file(
+    filename: Filename, mimetype: Optional[str] = None
+) -> ResponseValue:
     """Same as flask.send_file, except raises NotFound on file errors."""
     # NB: flask.send_file interprets relative paths relative to
     # current_app.root_path. We don't want that.
     try:
         resp = send_file(os.path.abspath(filename), mimetype=mimetype)
     except (FileNotFoundError, IsADirectoryError, PermissionError):
         abort(404)
@@ -174,15 +184,15 @@
             return None
         record = source.record
         alt = (
             record.alt if record.alt not in (PRIMARY_ALT, primary_alternative) else None
         )
         return url_for("url.edit", path=record.path, alt=alt)
 
-    def serve_artifact(self, url_path: str) -> Response:
+    def serve_artifact(self, url_path: str) -> ResponseValue:
         source = self.resolve_url_path(url_path)
 
         # If the request path does not end with a slash but we
         # requested a URL that actually wants a trailing slash, we
         # append it.  This is consistent with what apache and nginx do
         # and it ensures our relative urls work.
         if (
@@ -210,20 +220,20 @@
 
         mimetype = _deduce_mimetype(artifact.dst_filename)
         if mimetype == "text/html" and edit_url is not None:
             return _send_html_for_editing(artifact, edit_url, mimetype)
         return _checked_send_file(artifact.dst_filename, mimetype=mimetype)
 
 
-def serve_artifact(path: str) -> Response:
+def serve_artifact(path: str) -> ResponseValue:
     lektor_context = get_lektor_context()
     return ArtifactServer(lektor_context).serve_artifact(path)
 
 
-def serve_file(path: str) -> Response:
+def serve_file(path: str) -> ResponseValue:
     """Serve file directly from Lektor's output directory."""
     assert isinstance(current_app, LektorApp)
     output_path = current_app.lektor_info.output_path
 
     safe_path = safe_join("", *(path.strip("/").split("/")))
     if safe_path is None:
         abort(404)
@@ -238,15 +248,15 @@
         abort(404)
 
     return _checked_send_file(filename, mimetype=_deduce_mimetype(filename.name))
 
 
 @bp.route("/", defaults={"path": ""})
 @bp.route("/<path:path>")
-def serve_artifact_or_file(path: str) -> Response:
+def serve_artifact_or_file(path: str) -> ResponseReturnValue:
     try:
         return serve_artifact(path)
     except HiddenRecordException:
         raise
     except NotFound:
         return serve_file(path)
```

### Comparing `lektor-3.4.0b6/lektor/admin/static/app.css` & `lektor-3.4.0b7/lektor/admin/static/app.css`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/app.css.map` & `lektor-3.4.0b7/lektor/admin/static/app.css.map`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/app.js` & `lektor-3.4.0b7/lektor/admin/static/app.js`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/app.js.map` & `lektor-3.4.0b7/lektor/admin/static/app.js.map`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/fontawesome-webfont-5GKVPAEF.woff2` & `lektor-3.4.0b7/lektor/admin/static/fontawesome-webfont-5GKVPAEF.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-400-normal-72U6HY3C.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-cyrillic-400-normal-72U6HY3C.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-700-normal-2TPID6WR.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-cyrillic-700-normal-2TPID6WR.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-ext-400-normal-SGZKCMAU.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-cyrillic-ext-400-normal-SGZKCMAU.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-cyrillic-ext-700-normal-CKGDQNG6.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-cyrillic-ext-700-normal-CKGDQNG6.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-400-normal-FZE4RLDU.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-greek-400-normal-FZE4RLDU.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-700-normal-5YAILM42.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-greek-700-normal-5YAILM42.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-ext-400-normal-CARBXC53.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-greek-ext-400-normal-CARBXC53.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-greek-ext-700-normal-MWV52O3F.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-greek-ext-700-normal-MWV52O3F.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-400-normal-WDWDTZK2.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-latin-400-normal-WDWDTZK2.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-700-normal-VK4QNPMO.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-latin-700-normal-VK4QNPMO.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-ext-400-normal-66GAUH66.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-latin-ext-400-normal-66GAUH66.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-latin-ext-700-normal-W2KTZJSB.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-latin-ext-700-normal-W2KTZJSB.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-vietnamese-400-normal-HHIQBQTZ.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-vietnamese-400-normal-HHIQBQTZ.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/static/roboto-slab-vietnamese-700-normal-TQT4Y47C.woff2` & `lektor-3.4.0b7/lektor/admin/static/roboto-slab-vietnamese-700-normal-TQT4Y47C.woff2`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/templates/dash.html` & `lektor-3.4.0b7/lektor/admin/templates/dash.html`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/templates/edit-button.html` & `lektor-3.4.0b7/lektor/admin/templates/edit-button.html`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/templates/livereload-worker.js` & `lektor-3.4.0b7/lektor/admin/templates/livereload-worker.js`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/admin/templates/livereload.html` & `lektor-3.4.0b7/lektor/admin/templates/livereload.html`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/environment/__init__.py` & `lektor-3.4.0b7/lektor/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/environment/config.py` & `lektor-3.4.0b7/lektor/environment/config.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/environment/expressions.py` & `lektor-3.4.0b7/lektor/environment/expressions.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/markdown/__init__.py` & `lektor-3.4.0b7/lektor/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/markdown/controller.py` & `lektor-3.4.0b7/lektor/markdown/controller.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/markdown/mistune0.py` & `lektor-3.4.0b7/lektor/markdown/mistune0.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/markdown/mistune2.py` & `lektor-3.4.0b7/lektor/markdown/mistune2.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/quickstart-templates/plugin/setup.cfg.in` & `lektor-3.4.0b7/lektor/quickstart-templates/plugin/setup.cfg.in`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/quickstart-templates/project/assets/static/style.css.in` & `lektor-3.4.0b7/lektor/quickstart-templates/project/assets/static/style.css.in`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/quickstart-templates/project/templates/layout.html.in` & `lektor-3.4.0b7/lektor/quickstart-templates/project/templates/layout.html.in`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/quickstart-templates/project/templates/macros/blog.html.in` & `lektor-3.4.0b7/lektor/quickstart-templates/project/templates/macros/blog.html.in`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/quickstart-templates/theme/images/homepage.png` & `lektor-3.4.0b7/lektor/quickstart-templates/theme/images/homepage.png`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/ca.json` & `lektor-3.4.0b7/lektor/translations/ca.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/de.json` & `lektor-3.4.0b7/lektor/translations/de.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/en.json` & `lektor-3.4.0b7/lektor/translations/en.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/es.json` & `lektor-3.4.0b7/lektor/translations/es.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/fr.json` & `lektor-3.4.0b7/lektor/translations/fr.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/it.json` & `lektor-3.4.0b7/lektor/translations/it.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/ja.json` & `lektor-3.4.0b7/lektor/translations/ja.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/ko.json` & `lektor-3.4.0b7/lektor/translations/ko.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/nl.json` & `lektor-3.4.0b7/lektor/translations/nl.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/pl.json` & `lektor-3.4.0b7/lektor/translations/pl.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/pt.json` & `lektor-3.4.0b7/lektor/translations/pt.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/ru.json` & `lektor-3.4.0b7/lektor/translations/ru.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/translations/zh.json` & `lektor-3.4.0b7/lektor/translations/zh.json`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/types/__init__.py` & `lektor-3.4.0b7/lektor/types/__init__.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/types/base.py` & `lektor-3.4.0b7/lektor/types/base.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/types/fake.py` & `lektor-3.4.0b7/lektor/types/fake.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/types/flow.py` & `lektor-3.4.0b7/lektor/types/flow.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/types/formats.py` & `lektor-3.4.0b7/lektor/types/formats.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/types/multi.py` & `lektor-3.4.0b7/lektor/types/multi.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/types/primitives.py` & `lektor-3.4.0b7/lektor/types/primitives.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/lektor/types/special.py` & `lektor-3.4.0b7/lektor/types/special.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/conftest.py` & `lektor-3.4.0b7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_assets.py` & `lektor-3.4.0b7/tests/test_assets.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_build_frontend.py` & `lektor-3.4.0b7/tests/test_build_frontend.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_builder.py` & `lektor-3.4.0b7/tests/test_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 
 import pytest
 
+from lektor.builder import FileInfo
 from lektor.reporter import NullReporter
 
 
 def get_child_sources(prog):
     return sorted(list(prog.iter_child_sources()), key=lambda x: x["_id"])
 
 
@@ -382,7 +383,34 @@
         "{{ this.get_siblings() }}"
     )
 
     scratch_builder.build_all()
 
     with AssertBuildsNothingReporter():
         scratch_builder.build_all()
+
+
+################################################################
+
+
+def test_Artifact_open_encoding(builder):
+    build_state = builder.new_build_state()
+    artifact = build_state.new_artifact("dummy-artifact", sources=())
+    with artifact.open("w", encoding="iso-8859-1") as fp:
+        fp.write("Ciarán")
+    with artifact.open("r", encoding="iso-8859-1") as fp:
+        assert fp.read() == "Ciarán"
+
+
+def test_FileInfo_unchanged(env, tmp_path):
+    file_path = tmp_path / "file"
+    file_path.write_text("foo")
+
+    file_info = FileInfo(env, file_path)
+    # cache size, mtime, but *not* checksum
+    assert file_info.size == 3
+
+    file_path.write_text("foobar")
+    file_info2 = FileInfo(env, file_path)
+    assert file_info2.size != 3
+
+    assert not file_info.unchanged(file_info2)
```

### Comparing `lektor-3.4.0b6/tests/test_buildfailures.py` & `lektor-3.4.0b7/tests/test_buildfailures.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_cli.py` & `lektor-3.4.0b7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_cli_utils.py` & `lektor-3.4.0b7/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_compat.py` & `lektor-3.4.0b7/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_config.py` & `lektor-3.4.0b7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_conftest.py` & `lektor-3.4.0b7/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_datamodel.py` & `lektor-3.4.0b7/tests/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_db.py` & `lektor-3.4.0b7/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_deploy.py` & `lektor-3.4.0b7/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_devcli.py` & `lektor-3.4.0b7/tests/test_devcli.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_editor.py` & `lektor-3.4.0b7/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_environment.py` & `lektor-3.4.0b7/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_imagetools.py` & `lektor-3.4.0b7/tests/test_imagetools.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_imports.py` & `lektor-3.4.0b7/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_issue_410.py` & `lektor-3.4.0b7/tests/test_issue_410.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_markdown.py` & `lektor-3.4.0b7/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_packages.py` & `lektor-3.4.0b7/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_pagination.py` & `lektor-3.4.0b7/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_pluginsystem.py` & `lektor-3.4.0b7/tests/test_pluginsystem.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_prev_next_sibling.py` & `lektor-3.4.0b7/tests/test_prev_next_sibling.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_project.py` & `lektor-3.4.0b7/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_publisher.py` & `lektor-3.4.0b7/tests/test_publisher.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_quickstart.py` & `lektor-3.4.0b7/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_sourceobj.py` & `lektor-3.4.0b7/tests/test_sourceobj.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_themes.py` & `lektor-3.4.0b7/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_tree.py` & `lektor-3.4.0b7/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_types.py` & `lektor-3.4.0b7/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_unicode.py` & `lektor-3.4.0b7/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_urls.py` & `lektor-3.4.0b7/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_utils.py` & `lektor-3.4.0b7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_videotools.py` & `lektor-3.4.0b7/tests/test_videotools.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/test_watcher.py` & `lektor-3.4.0b7/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/admin/test_api.py` & `lektor-3.4.0b7/tests/admin/test_api.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/admin/test_dash.py` & `lektor-3.4.0b7/tests/admin/test_dash.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/admin/test_serve.py` & `lektor-3.4.0b7/tests/admin/test_serve.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/admin/test_webui.py` & `lektor-3.4.0b7/tests/admin/test_webui.py`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/demo-project/content/test-progressive.jpg` & `lektor-3.4.0b7/tests/demo-project/content/test-progressive.jpg`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/demo-project/content/test-sof-last.jpg` & `lektor-3.4.0b7/tests/demo-project/content/test-sof-last.jpg`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/demo-project/content/test.jpg` & `lektor-3.4.0b7/tests/demo-project/content/test.jpg`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/demo-project/content/test.mp4` & `lektor-3.4.0b7/tests/demo-project/content/test.mp4`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/demo-project/content/colorspace-test/LICENSE.txt` & `lektor-3.4.0b7/tests/demo-project/content/colorspace-test/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/demo-project/content/colorspace-test/rgb-to-gbr-test.jpg` & `lektor-3.4.0b7/tests/demo-project/content/colorspace-test/rgb-to-gbr-test.jpg`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/tests/demo-project/templates/page.html` & `lektor-3.4.0b7/tests/demo-project/templates/page.html`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/LICENSE` & `lektor-3.4.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/README.md` & `lektor-3.4.0b7/README.md`

 * *Files identical despite different names*

### Comparing `lektor-3.4.0b6/pyproject.toml` & `lektor-3.4.0b7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     "mistune>=0.7.0,<3",
     "Pillow>=6",
     "pip",
     "python-slugify",
     "pytz; python_version<'3.9'",  # favor zoneinfo for python>=3.9
     "requests",
     "tzdata; python_version>='3.9' and sys_platform == 'win32'",
-    "watchfiles",
+    "watchfiles>=0.12",
     "Werkzeug>=2.1.0,<3",
 ]
 optional-dependencies.ipython = [
     "ipython",
     "traitlets",
 ]
 
@@ -123,14 +123,15 @@
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     '^\s*\.\.\.\s*$',
     '^\s*raise\s+NotImplementedError\(\)\s*$',
+    '^if TYPE_CHECKING:\s*',
 ]
 
 ################################################################
 #
 # pylint
 #
 [tool.pylint.main]
@@ -194,14 +195,15 @@
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 # Packages and modules we want to check
 module = [
     "lektor.constants",
+    "lektor.devserver",
     "lektor.packages",
     "lektor.admin.*",
     "lektor.imagetools",
     "test_packages",
 ]
 ignore_errors = false
 
@@ -211,14 +213,15 @@
 ]
 disallow_untyped_defs = false
 disallow_untyped_calls = false
 
 [[tool.mypy.overrides]]
 module = [
     "lektor.admin.*",
+    "lektor.devserver",
     "lektor.imagetools",
 ]
 disallow_untyped_calls = false
 warn_return_any = false
 
 [[tool.mypy.overrides]]
 module = [
```

### Comparing `lektor-3.4.0b6/PKG-INFO` & `lektor-3.4.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lektor
-Version: 3.4.0b6
+Version: 3.4.0b7
 Summary: A static content management system.
 Project-URL: Homepage, https://www.getlektor.com/
 Project-URL: Source, https://github.com/lektor/lektor/
 Project-URL: Documentation, https://www.getlektor.com/docs/
 Project-URL: Changelog, https://github.com/lektor/lektor/blob/master/CHANGES.md
 Author-email: Armin Ronacher <armin.ronacher@active-4.com>
 License: Copyright (c) 2015-2016 by the Armin Ronacher.
@@ -66,15 +66,15 @@
 Requires-Dist: mistune<3,>=0.7.0
 Requires-Dist: pillow>=6
 Requires-Dist: pip
 Requires-Dist: python-slugify
 Requires-Dist: pytz; python_version < '3.9'
 Requires-Dist: requests
 Requires-Dist: tzdata; python_version >= '3.9' and sys_platform == 'win32'
-Requires-Dist: watchfiles
+Requires-Dist: watchfiles>=0.12
 Requires-Dist: werkzeug<3,>=2.1.0
 Provides-Extra: ipython
 Requires-Dist: ipython; extra == 'ipython'
 Requires-Dist: traitlets; extra == 'ipython'
 Description-Content-Type: text/markdown
 
 # Lektor
```

