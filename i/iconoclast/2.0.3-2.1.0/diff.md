# Comparing `tmp/iconoclast-2.0.3.tar.gz` & `tmp/iconoclast-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iconoclast-2.0.3.tar", max compression
+gzip compressed data, was "iconoclast-2.1.0.tar", max compression
```

## Comparing `iconoclast-2.0.3.tar` & `iconoclast-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1091 2023-05-17 02:01:47.563876 iconoclast-2.0.3/LICENSE.md
--rw-r--r--   0        0        0     1254 2023-05-17 02:01:47.563876 iconoclast-2.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-17 02:01:47.567876 iconoclast-2.0.3/iconoclast/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 02:01:47.567876 iconoclast-2.0.3/iconoclast/cli/__init__.py
--rw-r--r--   0        0        0     3876 2023-05-17 02:01:47.567876 iconoclast-2.0.3/iconoclast/cli/app.py
--rw-r--r--   0        0        0      247 2023-05-17 02:01:47.567876 iconoclast-2.0.3/iconoclast/cli/context.py
--rw-r--r--   0        0        0      285 2023-05-17 02:01:47.567876 iconoclast-2.0.3/iconoclast/cli/exceptions.py
--rw-r--r--   0        0        0       96 2023-05-17 02:01:47.567876 iconoclast-2.0.3/iconoclast/cli/graphql/__init__.py
--rw-r--r--   0        0        0    12875 2023-05-17 02:01:47.567876 iconoclast-2.0.3/iconoclast/cli/graphql/schema.py
--rw-r--r--   0        0        0      298 2023-05-17 02:01:47.571876 iconoclast-2.0.3/iconoclast/cli/iconokit/iconokit/__init__.py
--rw-r--r--   0        0        0      209 2023-05-17 02:01:47.571876 iconoclast-2.0.3/iconoclast/cli/iconokit/pyproject.toml
--rw-r--r--   0        0        0     1665 2023-05-17 02:01:47.571876 iconoclast-2.0.3/iconoclast/cli/prompts.py
--rw-r--r--   0        0        0      189 2023-05-17 02:01:47.571876 iconoclast-2.0.3/iconoclast/plugins/__init__.py
--rw-r--r--   0        0        0     1752 2023-05-17 02:01:47.571876 iconoclast-2.0.3/iconoclast/plugins/iconocards.py
--rw-r--r--   0        0        0     3403 2023-05-17 02:01:47.571876 iconoclast-2.0.3/iconoclast/plugins/iconoclast.py
--rw-r--r--   0        0        0     1891 2023-05-17 02:01:47.571876 iconoclast-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 iconoclast-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-06-06 14:29:59.893450 iconoclast-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1254 2023-06-06 14:29:59.893450 iconoclast-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/cli/__init__.py
+-rw-r--r--   0        0        0     5460 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/cli/app.py
+-rw-r--r--   0        0        0      247 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/cli/context.py
+-rw-r--r--   0        0        0      285 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/cli/exceptions.py
+-rw-r--r--   0        0        0       96 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/cli/graphql/__init__.py
+-rw-r--r--   0        0        0    12875 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/cli/graphql/schema.py
+-rw-r--r--   0        0        0      298 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/cli/iconokit/iconokit/__init__.py
+-rw-r--r--   0        0        0      209 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/cli/iconokit/pyproject.toml
+-rw-r--r--   0        0        0     1665 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/cli/prompts.py
+-rw-r--r--   0        0        0       37 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/plugins/__init__.py
+-rw-r--r--   0        0        0     1723 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/plugins/cards.py
+-rw-r--r--   0        0        0     3256 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/plugins/main.py
+-rw-r--r--   0        0        0      838 2023-06-06 14:29:59.901450 iconoclast-2.1.0/iconoclast/plugins/utils.py
+-rw-r--r--   0        0        0     1686 2023-06-06 14:29:59.901450 iconoclast-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 iconoclast-2.1.0/PKG-INFO
```

### Comparing `iconoclast-2.0.3/LICENSE.md` & `iconoclast-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.3/README.md` & `iconoclast-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.3/iconoclast/cli/app.py` & `iconoclast-2.1.0/iconoclast/cli/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,108 @@
 import subprocess
+import sys
 from datetime import datetime
 from pathlib import Path as StdPath
 from tempfile import TemporaryDirectory
+from typing import Callable
 
 import requests
 import typer
 from dict_deep import deep_get
-from halo import Halo
+from log_symbols import LogSymbols
+from merge_args import merge_args
 from mkdocs.config.base import load_config
 from path import Path
 from sgqlc.endpoint.requests import RequestsEndpoint
 from sgqlc.operation import Operation
 from yarl import URL
 
 from iconoclast.cli.context import set_context
 from iconoclast.cli.exceptions import Iconoquit
 from iconoclast.cli.graphql.schema import fontawesome_schema as schema
-from iconoclast.plugins.iconoclast import IconokitConfig
+from iconoclast.plugins.main import IconoclastConfig, IconokitConfig
 
 app = typer.Typer(rich_markup_mode="rich")
 
 here = Path(__file__).parent
 
+pip = [sys.executable, "-m", "pip", "--disable-pip-version-check"]
+
+
+def common_options(func: Callable):
+    # noinspection PyUnusedLocal
+    @merge_args(func)
+    def wrapper(
+        ctx: typer.Context,
+        config_file: StdPath = typer.Option(
+            None,
+            "--config-file",
+            "-F",
+            exists=True,
+            dir_okay=False,
+            help="The path to your MkDocs configuration file.",
+            show_default=False,
+        ),
+        **kwargs,
+    ):
+        return func(ctx=ctx, **kwargs)
+
+    return wrapper
+
+
+@app.command(
+    name="setup",
+    context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
+    epilog="This command supports all options of [cyan]pip install[/cyan] in addition to the ones above.",
+)
+@set_context
+@common_options
+def setup(ctx: typer.Context):
+    """
+    Downlod Font Awesome Pro.
+    """
+    forbidden = {"--index-url", "-i"}.intersection(ctx.args)
+
+    if forbidden:
+        raise Iconoquit(
+            f"The {forbidden.pop()} option is not supported by this command."
+        )
+
+    config_file = ctx.params.get("config_file")
+    config = load_config(str(config_file) if config_file else None)
+    plugin_config: IconoclastConfig = config.plugins["iconoclast"].config
+    token = plugin_config.token
+
+    if not token:
+        raise Iconoquit(
+            "You must specify a Font Awesome package manager token in Iconoclast's plugin configuration to use this "
+            "command."
+        )
+
+    index_url = f"https://dl.fontawesome.com/{token}/fontawesome-pro/python/simple"
+
+    subprocess.run(
+        [*pip, "install", "fontawesomepro", "--index-url", index_url, *ctx.args],
+    )
+
 
 @app.command(
     name="install",
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
+    epilog="This command supports all options of [cyan]pip install[/cyan] in addition to the ones above.",
 )
 @set_context
+@common_options
 def install(
     ctx: typer.Context,
-    config_file: StdPath = typer.Option(
-        None,
-        "--config-file",
-        exists=True,
-        dir_okay=False,
-        help="The path to your MkDocs configuration file.",
-    ),
 ):
     """
-    Install a kit. This command supports all options of [cyan]pip install[/cyan] in addition to the ones listed
-    below.
+    Install a kit.
     """
+    config_file = ctx.params.get("config_file")
     config = load_config(str(config_file) if config_file else None)
     kit_config: IconokitConfig = config.plugins["iconoclast"].config.kit
 
     if not kit_config.enabled:
         raise Iconoquit(
             "You must specify a kit name and Font Awesome API token in "
             "Iconoclast's plugin configuration to use this command."
@@ -99,26 +156,28 @@
             for icon in icons:
                 svg = (
                     f"<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 {icon['width']} "
                     f"{icon['height']}\"><path d=\"{icon['path']}\"/></svg>"
                 )
                 (icons_dir / icon["name"]).with_suffix(".svg").write_text(svg)
 
-            with Halo(
-                text=f"Installing {kit_config.name}...", spinner="dots"
-            ) as spinner:
-                subprocess.run(
-                    f"pip install {iconokit_root.abspath()} {' '.join(ctx.args)}".split(),
-                    stdout=subprocess.DEVNULL,
-                    stderr=subprocess.STDOUT,
-                )
-                spinner.succeed(f"Kit installed!")
+            subprocess.run(
+                [*pip, "install", iconokit_root.abspath(), *ctx.args],
+            )
+
+            if not {"--quiet", "-q"}.intersection(ctx.args):
+                print(f"{LogSymbols.SUCCESS.value} Installed {kit_config.name}.")
 
 
 @app.callback(
     no_args_is_help=True,
     epilog=f"Iconoclast © {datetime.now().year} celsius narhwal. Thank you kindly for your attention.",
 )
 def main():
     """
     Iconoclast integrates Font Awesome Pro with Material for MkDocs.
     """
+
+
+if __name__ == "__main__":
+    # For debugging only.
+    app()
```

### Comparing `iconoclast-2.0.3/iconoclast/cli/graphql/schema.py` & `iconoclast-2.1.0/iconoclast/cli/graphql/schema.py`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.3/iconoclast/cli/prompts.py` & `iconoclast-2.1.0/iconoclast/cli/prompts.py`

 * *Files identical despite different names*

### Comparing `iconoclast-2.0.3/iconoclast/plugins/iconoclast.py` & `iconoclast-2.1.0/iconoclast/plugins/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,79 @@
 from __future__ import annotations
 
-import inspect
 import logging
 import os
 import sys
 from typing import Optional, Tuple
 
 from dict_deep import deep_get, deep_set
 from mkdocs.commands.build import DuplicateFilter
 from mkdocs.config import config_options as c
 from mkdocs.config.base import Config, ConfigErrors, ConfigWarnings
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from path import Path
 
-from iconoclast.plugins import new_console
+from iconoclast.plugins import utils
 
 symlink = Path(__file__).parent / ".overrides" / ".icons" / "fontawesome"
 
 
 class IconokitConfig(Config):
     name = c.Type(str, default="")
-    token = c.Type(str, default=os.getenv("FONTAWESOME_API_TOKEN") or "")
+    token = c.Type(str, default=os.getenv("FONTAWESOME_API_TOKEN", ""))
     enabled = c.Private()
 
     def validate(self) -> Tuple[ConfigWarnings, ConfigErrors]:
         warnings, errors = super().validate()
-        self.enabled = bool(self.name and self.token)
+        self.enabled = self.name and self.token
         return warnings, errors
 
 
 class IconoclastConfig(Config):
     css = c.Type(bool, default=False)
+    token = c.Type(
+        str,
+        default=os.getenv(
+            "FONTAWESOME_PKG_TOKEN", os.getenv("FONTAWESOME_NPM_AUTH_TOKEN", "")
+        ),
+    )
     kit: IconokitConfig = c.SubConfig(IconokitConfig)
 
 
 class IconoclastPlugin(BasePlugin[IconoclastConfig]):
     def on_config(self, config: MkDocsConfig) -> Optional[Config]:
+        if config.theme.name != "material":
+            log.error(
+                utils.ansify(
+                    "Iconoclast requires requires that your MkDocs theme "
+                    "be set to [bold underline green]Material for MkDocs[/].",
+                )
+            )
+            sys.exit(1)
+
         icon_dirs = [symlink]
-        css = "iconoclast.min.css"
+        css = "fontawesome.min.css"
 
         symlink.unlink_p()
         symlink.parent.makedirs_p()
 
-        (get_package_path() / "svgs").symlink(symlink)
+        (utils.get_package_path() / "svgs").symlink(symlink)
 
         if self.config.kit.enabled:
             try:
                 import iconokit
             except ImportError:
-                with new_console() as console:
-                    console.print(
-                        "You haven't installed a Font Awesome kit. "
-                        "Run [cyan]iconoclast install[/] or change your settings "
-                        "for the [magenta]iconoclast[/] plugin.",
+                log.error(
+                    utils.ansify(
+                        "You've configured a Font Awesome kit, but haven't installed it. "
+                        "Run [bold underline cyan]iconoclast install[/], then try again."
                     )
-                    log.error(console.export_text(styles=True))
-                    sys.exit(1)
+                )
+                sys.exit(1)
             else:
                 icon_dirs.append(iconokit.icons())
                 css = iconokit.kit("css")
 
         key = "mdx_configs|pymdownx.emoji|options|custom_icons"
 
         for icon_dir in icon_dirs:
@@ -76,32 +89,16 @@
 
         return config
 
     def on_post_build(self, *, config: MkDocsConfig) -> None:
         symlink.parent.parent.rmtree_p()
 
         if self.config.css and not self.config.kit.enabled:
-            fa_path = get_package_path()
+            fa_path = utils.get_package_path()
             site_dir = Path(config.site_dir)
 
-            (fa_path / "css" / "all.min.css").copy(site_dir / "iconoclast.min.css")
+            (fa_path / "css" / "all.min.css").copy(site_dir / "fontawesome.min.css")
             (fa_path / "webfonts").copytree(site_dir / "webfonts")
 
 
-def get_package_path() -> Path:
-    try:
-        import fontawesomepro
-    except ImportError:
-        with new_console() as console:
-            console.print(
-                "Font Awesome Pro is not installed. Install it or remove the [magenta]iconoclast[/] plugin."
-            )
-            log.error(console.export_text(styles=True))
-            sys.exit(1)
-    else:
-        return (
-            Path(inspect.getfile(fontawesomepro)).parent / "static" / "fontawesomepro"
-        )
-
-
 log = logging.getLogger("mkdocs")
 log.addFilter(DuplicateFilter())
```

### Comparing `iconoclast-2.0.3/pyproject.toml` & `iconoclast-2.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "iconoclast"
-version = "2.0.3"
+version = "2.1.0"
 description = "Font Awesome Pro integration for Material for MkDocs"
 authors = ["celsius narhwal <hello@celsiusnarhwal.dev>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 decorator = "^5.1.1"
 dict-deep = "^4.1.2"
 halo = "^0.0.31"
 importlib-metadata = "^6.6.0"
+merge-args = "^0.1.5"
 mkdocs = "^1.4"
 path = "^16.6.0"
 semver = "^3.0.0"
 sgqlc = "^16.1"
 yarl = "^1.9.2"
 typer = { extras = ["all"], version = "^0.9.0" }
 
@@ -24,29 +25,23 @@
 mkdocs-material = "^9.1.8"
 rich-tracebacks = "^1.2.1"
 
 [tool.poetry.group.docs.dependencies]
 cairosvg = "^2.7.0"
 pillow = "^9.5.0"
 poethepoet = "^0.19.0"
-fontawesomepro = { version = "^6.4.0", source = "fontawesome" }
 mkdocs-material = { git = "https://github.com/squidfunk/mkdocs-material-insiders" }
 
-[[tool.poetry.source]]
-name = "fontawesome"
-url = "https://dl.fontawesome.com/${FONTAWESOME_PKG_TOKEN}/fontawesome-pro/python/simple"
-secondary = true
-
 [tool.poetry.scripts]
 iconoclast = "iconoclast.cli.app:app"
 icl = "iconoclast.cli.app:app"
 
 [tool.poetry.plugins."mkdocs.plugins"]
-iconoclast = "iconoclast.plugins.iconoclast:IconoclastPlugin"
-iconocards = "iconoclast.plugins.iconocards:IconocardsPlugin"
+iconoclast = "iconoclast.plugins.main:IconoclastPlugin"
+iconocards = "iconoclast.plugins.cards:IconocardsPlugin"
 
 [tool.black]
 target-version = ["py37"]
 line-length = 88
 
 [tool.isort]
 profile = "black"
```

### Comparing `iconoclast-2.0.3/PKG-INFO` & `iconoclast-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconoclast
-Version: 2.0.3
+Version: 2.1.0
 Summary: Font Awesome Pro integration for Material for MkDocs
 License: MIT
 Author: celsius narhwal
 Author-email: hello@celsiusnarhwal.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: dict-deep (>=4.1.2,<5.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
+Requires-Dist: merge-args (>=0.1.5,<0.2.0)
 Requires-Dist: mkdocs (>=1.4,<2.0)
 Requires-Dist: path (>=16.6.0,<17.0.0)
 Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: sgqlc (>=16.1,<17.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Description-Content-Type: text/markdown
```

