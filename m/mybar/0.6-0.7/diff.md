# Comparing `tmp/mybar-0.6.tar.gz` & `tmp/mybar-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybar-0.6.tar", last modified: Thu May 25 10:20:50 2023, max compression
+gzip compressed data, was "mybar-0.7.tar", last modified: Tue Jun  6 10:38:21 2023, max compression
```

## Comparing `mybar-0.6.tar` & `mybar-0.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-25 10:20:50.149733 mybar-0.6/
--rw-r--r--   0 sam       (1000) sam       (1000)     1077 2023-03-16 08:41:11.000000 mybar-0.6/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-05-25 10:20:50.149733 mybar-0.6/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      155 2023-03-16 08:41:11.000000 mybar-0.6/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-25 10:20:50.149733 mybar-0.6/mybar/
--rw-r--r--   0 sam       (1000) sam       (1000)      634 2023-05-25 10:17:15.000000 mybar-0.6/mybar/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1254 2023-05-23 09:48:03.000000 mybar-0.6/mybar/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1898 2023-05-03 22:40:40.000000 mybar-0.6/mybar/_setups.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6381 2023-04-30 05:49:24.000000 mybar-0.6/mybar/_types.py
--rw-r--r--   0 sam       (1000) sam       (1000)    41160 2023-05-25 09:53:23.000000 mybar-0.6/mybar/bar.py
--rw-r--r--   0 sam       (1000) sam       (1000)     9230 2023-04-30 05:26:06.000000 mybar-0.6/mybar/cli.py
--rw-r--r--   0 sam       (1000) sam       (1000)      668 2023-03-21 09:17:30.000000 mybar-0.6/mybar/constants.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3554 2023-03-16 08:41:11.000000 mybar-0.6/mybar/errors.py
--rw-r--r--   0 sam       (1000) sam       (1000)    26274 2023-05-25 09:51:04.000000 mybar-0.6/mybar/field.py
--rw-r--r--   0 sam       (1000) sam       (1000)    16948 2023-05-25 09:55:29.000000 mybar-0.6/mybar/field_funcs.py
--rw-r--r--   0 sam       (1000) sam       (1000)    16853 2023-05-23 12:13:22.000000 mybar-0.6/mybar/formatting.py
--rw-r--r--   0 sam       (1000) sam       (1000)      284 2023-03-16 08:41:11.000000 mybar-0.6/mybar/log.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13368 2023-05-03 06:07:43.000000 mybar-0.6/mybar/sync.py
--rw-r--r--   0 sam       (1000) sam       (1000)      124 2023-03-16 08:41:11.000000 mybar-0.6/mybar/templates.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5690 2023-03-16 08:41:11.000000 mybar-0.6/mybar/utils.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-25 10:20:50.149733 mybar-0.6/mybar.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-05-25 10:20:50.000000 mybar-0.6/mybar.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      450 2023-05-25 10:20:50.000000 mybar-0.6/mybar.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-05-25 10:20:50.000000 mybar-0.6/mybar.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-05-25 10:20:50.000000 mybar-0.6/mybar.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-05-25 10:20:50.000000 mybar-0.6/mybar.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-03-16 08:41:11.000000 mybar-0.6/pyproject.toml
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-16 08:41:11.000000 mybar-0.6/requirements.txt
--rw-r--r--   0 sam       (1000) sam       (1000)      890 2023-05-25 10:20:50.149733 mybar-0.6/setup.cfg
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-06 10:38:21.409394 mybar-0.7/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1077 2023-03-16 08:41:11.000000 mybar-0.7/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-06-06 10:38:21.409394 mybar-0.7/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      155 2023-03-16 08:41:11.000000 mybar-0.7/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-06 10:38:21.409394 mybar-0.7/mybar/
+-rw-r--r--   0 sam       (1000) sam       (1000)      599 2023-06-06 10:20:26.000000 mybar-0.7/mybar/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      336 2023-06-01 10:53:22.000000 mybar-0.7/mybar/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1863 2023-05-30 09:20:33.000000 mybar-0.7/mybar/_setups.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3846 2023-05-31 09:01:05.000000 mybar-0.7/mybar/_types.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    46651 2023-06-06 10:30:53.000000 mybar-0.7/mybar/bar.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    12944 2023-06-06 10:17:47.000000 mybar-0.7/mybar/cli.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      861 2023-06-02 05:55:18.000000 mybar-0.7/mybar/constants.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2112 2023-05-29 11:58:23.000000 mybar-0.7/mybar/defaults.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3439 2023-06-02 11:18:30.000000 mybar-0.7/mybar/errors.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    28629 2023-06-06 09:58:42.000000 mybar-0.7/mybar/field.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    15856 2023-05-31 09:45:55.000000 mybar-0.7/mybar/field_funcs.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    25593 2023-05-30 10:50:38.000000 mybar-0.7/mybar/formatting.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      361 2023-05-31 11:58:31.000000 mybar-0.7/mybar/log.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13368 2023-05-03 06:07:43.000000 mybar-0.7/mybar/sync.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1929 2023-05-30 10:32:04.000000 mybar-0.7/mybar/templates.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5685 2023-05-29 15:02:35.000000 mybar-0.7/mybar/utils.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-06 10:38:21.409394 mybar-0.7/mybar.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)      998 2023-06-06 10:38:21.000000 mybar-0.7/mybar.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      468 2023-06-06 10:38:21.000000 mybar-0.7/mybar.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-06-06 10:38:21.000000 mybar-0.7/mybar.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-06-06 10:38:21.000000 mybar-0.7/mybar.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-06-06 10:38:21.000000 mybar-0.7/mybar.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-03-16 08:41:11.000000 mybar-0.7/pyproject.toml
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-16 08:41:11.000000 mybar-0.7/requirements.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)      890 2023-06-06 10:38:21.409394 mybar-0.7/setup.cfg
```

### Comparing `mybar-0.6/LICENSE` & `mybar-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mybar-0.6/PKG-INFO` & `mybar-0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.6
+Version: 0.7
 Summary: An async status bar with a highly customizable API.
 Home-page: https://github.com/lonelyabsol/mybar
 Author: lonelyabsol
 License: MIT
 Project-URL: GitHub: repo, https://github.com/lonelyabsol/mybar
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mybar-0.6/mybar/_setups.py` & `mybar-0.7/mybar/_setups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # import psutil
 
 from .errors import (
     BrokenFormatStringError,
     FailedSetup,
     IncompatibleArgsError,
-    InvalidFormatStringFieldError,
 )
 from .formatting import ConditionalFormatStr
 from .utils import join_options, make_error_message 
 from ._types import FormatStr
 
 async def setup_uptime(
     fmt: FormatStr,
```

### Comparing `mybar-0.6/mybar/bar.py` & `mybar-0.7/mybar/bar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,93 @@
-#TODO: {'uptime1': {'dft': 'uptime', ...}, 'uptime2': {'dft': 'uptime', ...}}
-#TODO: Bar(synchronous=True)!
-#TODO: Bar.as_generator()!
+#TODO: Implement dynamic icons!
 #TODO: Finish Mocp line!
 
 
 __all__ = (
     'Bar',
     'run',
+    'write_initial_config'
 )
 
 
 import asyncio
 import json
 import os
 import sys
 import threading
 import time
 from copy import deepcopy
-from string import Formatter
 
-from .constants import CONFIG_FILE, DEBUG
+from .constants import (
+    CLEAR_LINE,
+    CONFIG_FILE,
+    CSI,
+    DEBUG,
+    HIDE_CURSOR,
+    UNHIDE_CURSOR,
+)
+
 from . import cli
+from . import field_funcs
 from . import utils
 from .errors import *
-from .field import Field, FieldPrecursor
-from .formatting import FormatterFieldSig
+from .field import Field, FieldPrecursor, FieldSpec
+from .formatting import FormatStr, FmtStrStructure, FormatterFieldSig
+from .templates import BarConfigSpec, BarSpec, FieldSpec
 from ._types import (
     Args,
-    BarSpec,
-    BarTemplateSpec,
     ConsoleControlCode,
     FieldName,
     FieldOrder,
-    FmtStrStructure,
-    FormatStr,
     Icon,
     JSONText,
     Kwargs,
     Line,
     PTY_Icon,
     PTY_Separator,
     Pattern,
     Separator,
     TTY_Icon,
     TTY_Separator,
 )
 
-from collections.abc import Iterable, Iterator, Sequence
+from collections.abc import Container, Iterable, Iterator, Sequence
 from os import PathLike
-from typing import IO, NoReturn, Required, Self, TypeAlias, TypedDict, TypeVar
+from typing import (
+    IO,
+    NoReturn,
+    Required,
+    Self,
+    TypeVar
+)
 
 Bar = TypeVar('Bar')
 
 
-# Unix terminal escape code (control sequence introducer):
-CSI: ConsoleControlCode = '\033['
-CLEAR_LINE: ConsoleControlCode = '\x1b[2K'  # VT100 escape code to clear line
-HIDE_CURSOR: ConsoleControlCode = '?25l'
-UNHIDE_CURSOR: ConsoleControlCode = '?25h'
-
-
-class BarTemplate(dict):
+class BarConfig(dict):
     '''
     Build and transport Bar configs between files, dicts and command line args.
 
-    :param options: Optional :class:`_types.BarTemplateSpec` parameters
+    :param options: Optional :class:`_types.BarConfigSpec` parameters
         that override those of `defaults`
-    :type options: :class:`_types.BarTemplateSpec`
+    :type options: :class:`_types.BarConfigSpec`
 
     :param defaults: Parameters to use by default,
         defaults to :attr:`Bar._default_params`
     :type defaults: :class:`dict`
 
     .. note:: `options` and `defaults` must be :class:`dict` instances
-        of form :class:`_types.BarTemplateSpec`
+        of form :class:`_types.BarConfigSpec`
 
     '''
 
     def __init__(
         self,
-        options: BarTemplateSpec = {},
-        defaults: BarTemplateSpec = None,
+        options: BarConfigSpec = {},
+        defaults: BarConfigSpec = None,
     ) -> None:
         if defaults is None:
             self.defaults = Bar._default_params.copy()
         else:
             self.defaults = defaults.copy()
         self.options = options.copy()
 
@@ -101,175 +104,284 @@
         return f"<{cls} {maybe_file}{params}>"
 
     @classmethod
     def from_file(
         cls,
         file: PathLike = None,
         *,
-        defaults: BarTemplateSpec = None,
-        overrides: BarTemplateSpec = {},
+        defaults: BarConfigSpec = None,
+        overrides: BarConfigSpec = {},
     ) -> Self:
         '''
-        Return a new :class:`BarTemplate` from a config file path.
+        Return a new :class:`BarConfig` from a config file path.
 
         :param file: The filepath to the config file,
             defaults to ``'~/.mybar.json'``
         :type file: :class:`PathLike`
 
-        :param defaults: The base :class:`_types.BarTemplateSpec` dict whose
-            params the new :class:`BarTemplate` will override,
+        :param defaults: The base :class:`_types.BarConfigSpec` dict whose
+            params the new :class:`BarConfig` will override,
             defaults to :attr:`Bar._default_params`
-        :type defaults: :class:`_types.BarTemplateSpec`
+        :type defaults: :class:`_types.BarConfigSpec`
 
         :param overrides: Additional param overrides to the config file
-        :type overrides: :class:`_types.BarTemplateSpec`
+        :type overrides: :class:`_types.BarConfigSpec`
 
-        :returns: A new :class:`BarTemplate` instance
-        :rtype: :class:`BarTemplate`
+        :returns: A new :class:`BarConfig` instance
+        :rtype: :class:`BarConfig`
         :raises: :exc:`OSError` for issues with accessing the file
         '''
         if defaults is None:
             defaults = Bar._default_params
         overrides = overrides.copy()
 
         if file is None:
             file = overrides.pop('config_file', CONFIG_FILE)
-
-        file_spec = {}
         absolute = os.path.abspath(os.path.expanduser(file))
+        file_spec = {}
         try:
-            file_spec, text = cls.read_file(absolute)
+            file_spec, text = cls._read_file(absolute)
         except OSError as e:
             raise e.with_traceback(None)
 
         options = file_spec | overrides
-        t = cls(options, defaults)
-        t.file = absolute
-        return t
+        config = cls(options, defaults)
+        config.file = absolute
+        return config
 
     @classmethod
     def from_stdin(
         cls,
         write_new_file_dft: bool = True
     ) -> Self:
-        '''Return a new :class:`BarTemplate` using args from STDIN.
+        '''Return a new :class:`BarConfig` using args from STDIN.
         Prompt the user before writing a new config file if one does
         not exist.
 
-        :param write_new_file_dft: Automatically write new files,
-            defaults to ``False``
+        :param write_new_file_dft: Write new files by default,
+            defaults to ``True``
         :type write_new_file_dft: :class:`bool`
 
-        :returns: A new :class:`BarTemplate`
-        :rtype: :class:`BarTemplate`
+        :returns: A new :class:`BarConfig`
+        :rtype: :class:`BarConfig`
         '''
         parser = cli.Parser()
         try:
             bar_options = parser.parse_args()
-        except FatalError as e:
+        except CLIUsageError as e:
             parser.error(e.msg)  # Shows usage
 
-##        except OSError as e:
-##            parser.quit(e)
+        if 'field_options' in bar_options:
+            fields = parser.process_field_options(
+                bar_options.pop('field_options')
+            )
+            bar_options['field_definitions'] = fields
+
+        # Handle missing config files:
+        if 'config_file' not in bar_options:
+            if (first_use := (not os.path.exists(CONFIG_FILE))):
+                cls.welcome_new_users()
+                cls.maybe_make_config_dir()
+                wants_to_write = cls.write_with_approval(overrides=bar_options)
+                if not wants_to_write:
+                    # Forget all this config file business.
+                    # Our new user is in a rush. Let's give them a bar.
+                    return cls(bar_options)
+
+        file = bar_options.pop('config_file', None)
 
         try:
-            template = cls.from_file(overrides=bar_options)
-        except OSError as e:
+            # config_file is in overrides or it defaults to CONFIG_FILE:
+            config = cls.from_file(file, overrides=bar_options)
+
+        except FileNotFoundError as e:
             file = e.filename
-            msg = (f"The config file at {file!r} does not exist.")
-            question = "Would you like to make it now?"
-            write_options = {'y': True, 'n': False}
-            default = 'ny'[write_new_file_dft]
-            handler = cli.OptionsAsker(write_options, default, question)
-
-            print(msg)
-            write_new_file = handler.ask()
-            if write_new_file:
-                cls.write_file(file, bar_options)
-                print(f"Wrote new config file at {file!r}")
-                template = cls.from_file(file)
-            else:
-                parser.quit()
+            cls.maybe_make_config_dir()
+            write_ok = cls.write_with_approval(file, overrides=bar_options)
+            if not write_ok:
+                parser.quit("Exiting...")
+            config = cls.from_file(file, overrides=bar_options)
+
+        except OSError as e:
+            e.add_note("Exiting...")
+            raise e from None
+
+        except KeyboardInterrupt:
+            parser.quit()
+
+        return config
+
+    @classmethod
+    def write_with_approval(
+        cls,
+        file: PathLike = None,
+        overrides: BarSpec = {},
+    ) -> bool:
+        '''
+        Write a config file to `file`.
+        Prompt the user for approval before writing.
+
+        :param file: Write to this file, defaults to :obj:`CONFIG_FILE`
+        :type file: :class:`PathLike`
+
+        :returns: ``True`` if the file was written, ``False`` if not
+        '''
+        if file is None:
+            file = CONFIG_FILE
+
+        approved = cls._get_write_new_approval(
+            file,
+            dft_choice=True
+        )
+        if approved:
+            try:
+                cls._write_file(file, overrides)
+            except FileNotFoundError as e:
+                try:
+                    path = os.path.dirname(e.filename)
+                    os.mkdir(path)
+                    print(f"Made new directory {path!r}")
+                    cls._write_file(file, overrides)
+                except OSError as e:
+                    raise e from None
+
+            print(f"Wrote new config file to {file!r}")
+            return True
+
+        return False
+
+    @classmethod
+    def _get_write_new_approval(
+        cls,
+        file: PathLike,
+        dft_choice: bool
+    ) -> bool:
+        '''
+        Get approval to write a new config file using
+            :class:`cli.OptionsAsker`.
+
+        :param file: The path to the config file
+        :type file: :class:`PathLike`
+
+        :param dft_choice: The default option to present to the user
+        :type dft_choice: :class:``
+        '''
+        dft = (file == CONFIG_FILE)
+        msg = (
+            f"The {'default' if dft else ''}"
+            f" config file at {file!r} does not exist."
+        )
+        question = "Would you like to make it now?"
+        write_options = {'y': True, 'n': False}
+        default = 'ny'[dft_choice]
+        handler = cli.OptionsAsker(write_options, default, question)
+
+        print(msg)
+        write_new_file_ok = handler.ask()
+        return write_new_file_ok
+
+    @classmethod
+    def maybe_make_config_dir(cls) -> None:
+        '''
+        Make a config directory in the default location if nonexistent.
+        '''
+        directory = os.path.dirname(CONFIG_FILE)
+        if not os.path.exists(directory):
+            os.mkdir(directory)
 
-        return template
+    @classmethod
+    def welcome_new_users(cls) -> None:
+        msg = (
+            f"-- {__package__} --"
+        )
+        print(msg)
 
     @staticmethod
-    def read_file(file: PathLike) -> tuple[BarTemplateSpec, JSONText]:
+    def _read_file(file: PathLike) -> tuple[BarConfigSpec, JSONText]:
         '''
         Read a given config file.
         Convert its JSON contents to a dict and return it along with the
         raw text of the file.
 
         :param file: The file to convert
         :type file: :class:`PathLike`
 
         :returns: The converted file and its raw text
-        :rtype: tuple[:class:`_types.BarTemplateSpec`, :class:`_types.JSONText`]
+        :rtype: tuple[:class:`_types.BarConfigSpec`, :class:`_types.JSONText`]
         '''
-        with open(file, 'r') as f:
+        absolute = os.path.abspath(os.path.expanduser(file))
+        with open(absolute, 'r') as f:
             data = json.load(f)
             text = f.read()
         return data, text
 
-    @staticmethod
-    def write_file(
+    @classmethod
+    def _write_file(
+        cls,
         file: PathLike,
-        obj: BarTemplateSpec = {},
+        obj: BarSpec = {},
         *,
         defaults: BarSpec = None
     ) -> None:
-        '''Write :class:`BarTemplate` params to a JSON file.
+        '''Write :class:`BarConfig` params to a JSON file.
 
         :param file: The file to write to
         :type file: :class:`PathLike`
 
-        :param obj: The :class:`_types.BarTemplateSpec` to write
-        :type obj: :class:`_types.BarTemplateSpec`, optional
+        :param obj: The :class:`_types.BarConfigSpec` to write
+        :type obj: :class:`_types.BarConfigSpec`, optional
 
         :param defaults: Any default parameters that `obj` should override,
             defaults to :attr:`Bar._default_params`
         :type defaults: :class:`_types.BarSpec`
         '''
         if defaults is None:
             defaults = Bar._default_params.copy()
 
-        obj = obj.copy()
-        obj.pop('config_file', None)
-        obj = defaults | obj
+        newobj = obj.copy()
+        newobj.pop('config_file', None)
+        newobj = defaults | obj
 
         fields = Field._default_fields.copy()
 
         # Clean the dict of irrelevant Field implementation details:
         for name, field in fields.items():
             new = fields[name] = field.copy()
             for param in ('name', 'func', 'setup'):
                 try:
                     del new[param]
                 except KeyError:
                     pass
 
-        obj['field_definitions'] = fields
+        newobj['field_definitions'] = fields
 
-        with open(os.path.expanduser(file), 'w') as f:
-            json.dump(obj, f, indent=4, ) #separators=(',\n', ': '))
+        absolute = os.path.abspath(os.path.expanduser(file))
+        if absolute == CONFIG_FILE and not os.path.exists(absolute):
+            cls.maybe_make_config_dir()
+        with open(os.path.expanduser(absolute), 'w') as f:
+            json.dump(newobj, f, indent=4, ) #separators=(',\n', ': '))
 
 
 class Bar:
     '''
     Create highly customizable status bars.
 
     :param fields: An iterable of default field names or :class:`Field` instances, defaults to ``None``
     :type fields: :class:`Iterable[Field | str]`
 
-    :param fmt: A curly-brace format string with field names, defaults to ``None``
-    :type fmt: :class:`_types.FormatStr`
+    :param template: A curly-brace format string with field names, defaults to ``None``
+    :type template: :class:`formatting.FormatStr`
 
     :param separator: The field separator when `fields` is given, defaults to ``'|'``
     :type separator: :class:`_types.PTY_Separator` | :class:`_types.TTY_Separator`
 
+    :param count: Only print the bar this many times, or never stop
+        when ``None``, defaults to ``None``
+    :type count: :class:`int`
+
     :param run_once: Whether the bar should print once and return, defaults to ``False``
     :type run_once: :class:`bool`
 
     :param refresh_rate: How often in seconds the bar automatically redraws itself, defaults to ``1.0``
     :type refresh_rate: :class:`float`
 
     :param align_to_seconds: Whether to synchronize redraws at the start of each new second (updates to the clock are shown accurately), defaults to ``True``
@@ -300,18 +412,18 @@
     :param stream: The bar's output stream, defaults to :attr:`sys.stdout`
     :type stream: :class:`IO`
 
 
     :raises: :exc:`errors.InvalidOutputStreamError` when `stream` does
         not implement the IO protocol
     :raises: :exc:`errors.IncompatibleArgsError` when
-        neither `fmt` nor `fields` are given
+        neither `template` nor `fields` are given
     :raises: :exc:`errors.IncompatibleArgsError` when
-        `fmt` is ``None`` but no `separator` or `separators` are given
-    :raises: :exc:`TypeError` when `fields` is not iterable, or when `fmt` is not a string
+        `template` is ``None`` but no `separator` or `separators` are given
+    :raises: :exc:`TypeError` when `fields` is not iterable, or when `template` is not a string
     '''
 
     _default_field_order = [
         'hostname',
         'uptime',
         'cpu_usage',
         'cpu_temp',
@@ -326,21 +438,22 @@
         'separator': '|',
         'refresh_rate': 1.0,
         'field_order': list(_default_field_order)
     }
 
     def __init__(
         self,
-        fmt: str = None,
-        fields: Iterable[Field | str] = None,
+        template: FormatStr = None,
+        fields: Iterable[Field | FieldName] = None,
         *,
         field_order: Iterable[FieldName] = None,
         separator: str = '|',
         refresh_rate: float = 1.0,
         stream: IO = sys.stdout,
+        count: int = None,
         run_once: bool = False,
         align_to_seconds: bool = True,
         join_empty_fields: bool = False,
         override_cooldown: float = 1/8,
         thread_cooldown: float = 1/8,
 
         # Set this to use different seps for different output streams:
@@ -352,63 +465,73 @@
         self._check_stream(stream)
         self._stream = stream
 
 
         # Check all the required parameters.
         if fields is None:
 
-            if fmt is None:
+            if template is None:
                 raise IncompatibleArgsError(
                     f"Either a list of Fields 'fields' "
-                    f"or a format string 'fmt' is required."
+                    f"or a format string 'template' is required."
                 )
 
-            elif not isinstance(fmt, str):
+            elif not isinstance(template, str):
                 raise TypeError(
-                    f"Format string 'fmt' must be a string, not {type(fmt)}"
+                    f"Format string 'template' must be a string, "
+                    f"not {type(template)}"
                 )
 
-            # Good to use fmt:
+            # Good to use template:
             else:
-                #NOTE: `fields` here are :class:`FormatterFieldSig`
-                # _normalize_fields() takes care of this later.
-                field_order, fields = self.parse_fmt(fmt)
+                parsed = FmtStrStructure.from_str(template)
+                parsed.validate_fields(Field._default_fields, True, True)
+                # names = parsed.get_names()
+                fields = parsed
 
         # Fall back to using fields.
         elif not hasattr(fields, '__iter__'):
             raise TypeError("The 'fields' argument must be iterable.")
 
         elif separator is None and separators is None:
             raise IncompatibleArgsError(
-                "A separator is required when 'fmt' is None."
+                "A separator is required when 'template' is None."
             )
 
-        names, fields = self._normalize_fields(fields)
+        field_names, fields = self._normalize_fields(fields)
 
         # Preserve custom field order, enabling duplicates:
-        if fmt is None and field_order is None:
-            field_order = names
+        if field_order is None:
+            field_order = field_names
 
         self._fields = fields
         self._field_order = field_order
         self._buffers = dict.fromkeys(self._fields, '')
 
-        self.fmt = fmt
+        self.template = template
 
         if separators is None:
             separators = (separator, separator)
         self._separators = separators
 
-        # Whether empty fields are joined when fmt is None:
+        # Whether empty fields are joined when template is None:
         # (True shows two separators together for every blank field.)
         self.join_empty_fields = join_empty_fields
 
         # How often in seconds the bar is regularly printed:
         self.refresh_rate = refresh_rate
 
+
+        if count == 0 or count == 1:
+            run_once = True
+        self.count = count
+        self._print_countdown = count
+        # self._count_queue = asyncio.Queue()
+
+
         # Whether the bar should exit after printing once:
         self.run_once = run_once
 
         # Whether the bar is printed at the top of every clock second:
         self.align_to_seconds = align_to_seconds
 
         # Make a queue to which fields with overrides_refresh send updates.
@@ -421,56 +544,58 @@
 
         # Staggering a thread's refresh interval across several sleeps with the
         # length of this cooldown prevents it from blocking for the entire
         # interval when the bar stops.
         # (A shorter cooldown means faster exits):
         self._thread_cooldown = thread_cooldown
 
-        # The set of field threads the bar must wait to join before
-        # printing a line with run_once:
-        self._threads = set()
+        # The dict mapping Field names to the threads running them.
+        # The bar must join each before printing a line with `run_once`:
+        self._threads = {}
+        # self._threads = set()
         self._printer_thread = None
+        self._printer_loop = None
+        self._funcs = {}
 
-        self._coros = []
+        self._coros = {}
         self._timely_fields = []
 
         # Calling run() sets this Event. Unsetting it stops all fields:
         self._can_run = threading.Event()
-        self.running = self._can_run.is_set
+        self._running = self._can_run.is_set
 
         # The bar's async event loop:
+        # self._thread_loop = asyncio.new_event_loop()
         self._loop = asyncio.new_event_loop()
 
     def __contains__(self, other: FieldPrecursor) -> bool:
         if isinstance(other, str):
             weak_test = (other in self._field_order)
             return weak_test
 
         elif isinstance(other, Field):
             less_weak_test = (other.name in self._field_order)
             return less_weak_test
 
-        # Shall we test for identical objects?
         else:
-            # No, too specific for a dunder-method.
             return False
 
     def __eq__(self, other: Bar) -> bool:
         if not all(
             getattr(self, attr) == getattr(other, attr)
             for attr in (
                 '_fields',
                 '_field_order',
                 '_separators',
                 'join_empty_fields',
             )
         ):
             return False
 
-        if self.fmt == other.fmt:
+        if self.template == other.template:
             return True
         return False
 
     def __iter__(self) -> Iterator:
         return iter(field for field in self._fields.values())
 
     def __len__(self) -> int:
@@ -479,88 +604,100 @@
     def __repr__(self) -> str:
         names = self._field_order
         fields = utils.join_options(names, final_sep='', limit=3)
         cls = type(self).__name__
         return f"{cls}(fields=[{fields}])"
 
     @classmethod
-    def from_template(
+    def from_config(
         cls,
-        tmpl: BarTemplate,
+        config: BarConfig,
         *,
+        overrides: BarSpec = {},
         ignore_with: Pattern | tuple[Pattern] | None = '//'
     ) -> Self:
         '''
-        Return a new :class:`Bar` from a :class:`BarTemplate`
+        Return a new :class:`Bar` from a :class:`BarConfig`
         or a dict of :class:`Bar` parameters.
         Ignore keys and list elements starting with `ignore_with`,
         which is ``'//'`` by default.
         If :param ignore_with: is ``None``, do not remove any values.
 
-        :param tmpl: The :class:`dict` to convert
-        :type tmpl: :class:`dict`
+        :param config: The :class:`dict` to convert
+        :type config: :class:`dict`
+
+        :param overrides: Replace items in `config` with these parameters,
+            defaults to ``{}``
+        :type overrides: :class:`BarSpec`
 
         :param ignore_with: A pattern to ignore, defaults to ``'//'``
         :type ignore_with: :class:`_types.Pattern` | tuple[:class:`_types.Pattern`] | ``None``, optional
 
         :returns: A new :class:`Bar`
         :rtype: :class:`Bar`
 
         :raises: :exc:`errors.IncompatibleArgsError` when
             no `field_order` is defined
-            or when no `fmt` is defined
+            or when no `template` is defined
         :raises: :exc:`errors.DefaultFieldNotFoundError` when either
             a field in `field_order` or
-            a field in `fmt`
+            a field in `template`
             cannot be found in :attr:`Field._default_fields`
         :raises: :exc:`errors.UndefinedFieldError` when
             a custom field name in `field_order` or
-            a custom field name in `fmt`
+            a custom field name in `template`
             is not properly defined in `field_definitions`
         :raises: :exc:`errors.InvalidFieldSpecError` when
             a field definition is not of the form :class:`_types.FieldSpec`
 
-        .. note:: `tmpl` can be a regular :class:`dict`
+        .. note:: `config` can be a regular :class:`dict`
         as long as it matches the form of :class:`_types.BarSpec`.
 
         '''
         if ignore_with is None:
-            data = deepcopy(tmpl)
+            data = deepcopy(config)
         else:
-            data = utils.scrub_comments(tmpl, ignore_with)
+            data = utils.scrub_comments(config, ignore_with)
+
+        data.update(overrides)
 
         bar_params = cls._default_params | data
         field_order = bar_params.pop('field_order', None)
         field_icons = bar_params.pop('field_icons', {})  # From the CLI
         field_defs = bar_params.pop('field_definitions', {})
 
-        if (fmt := bar_params.get('fmt')) is None:
+        if (template := bar_params.get('template')) is None:
             if field_order is None:
                 raise IncompatibleArgsError(
-                    "A bar format string 'fmt' is required when field "
-                    "order list 'field_order' is undefined."
+                    "A bar format string 'template' is required "
+                    "when field order list 'field_order' is undefined."
                 )
         else:
-            field_order, field_sigs = cls.parse_fmt(fmt)
+            parsed = FmtStrStructure.from_str(template)
+            parsed.validate_fields(Field._default_fields, True, True)
+            if field_order is None:
+                field_order = parsed.get_names()
 
         # Ensure icon assignments correspond to valid fields:
         for name in field_icons:
             if name not in field_order:
                 deduped = dict.fromkeys(field_order)  # Preserve order
                 expctd_from_icons = utils.join_options(deduped)
                 exc = utils.make_error_message(
                     InvalidFieldError,
                     doing_what="parsing custom Field icons",
                     blame=f"{name!r}",
                     expected=f"a Field name from among {expctd_from_icons}",
-                    epilogue="Only assign icons to Fields that will be in the Bar."
+                    epilogue=(
+                        "Only assign icons to Fields that will be in the Bar."
+                    )
                 )
                 raise exc from None
 
-        # Gather Field parameters and instantiate them:
+        # Gather Field parameters and instantiate new Fields:
         fields = {}
         expctd_name="the name of a default or properly defined `custom` Field"
 
         for name in field_order:
             field_params = field_defs.get(name)
 
             match field_params:
@@ -585,19 +722,24 @@
                     # 'field_definitions' and will not be found as a default.
                     name = field_params.pop('name', name)
                     del field_params['custom']
                     field = Field(**field_params, name=name)
 
                 case {}:
                     # The field is a default overridden by the user.
-                    # Are there custom icons given from the CLI?
-                    if name in field_icons:
+                    # Are there custom icons from --icons in the CLI?
+                    if field_icons and name in field_icons:
                         cust_icon = field_icons.pop(name)
                         field_params['icons'] = (cust_icon, cust_icon)
 
+                    # When one icon is given, override the default icons:
+                    elif 'icon' in field_params:
+                        cust_icon = field_params['icon']
+                        field_params['icons'] = (cust_icon, cust_icon)
+
                     try:
                         field = Field.from_default(name, overrides=field_params)
                     except DefaultFieldNotFoundError:
                         exc = utils.make_error_message(
                             UndefinedFieldError,
                             # doing_what="parsing 'field_order'",
                             blame=f"{name!r}",
@@ -629,37 +771,46 @@
             fields=tuple(fields.values()),
             field_order=field_order,
             **bar_params
         )
         return bar
 
     @classmethod
-    def from_file(cls, file: PathLike = None) -> Self:
+    def from_file(
+        cls,
+        file: PathLike = None,
+        overrides: BarSpec = {}
+    ) -> Self:
         '''
         Generate a new :class:`Bar` by reading a config file.
 
-        :param file: The config file to read, defaults to :obj:`constants.CONFIG_FILE`
+        :param file: The config file to read,
+            defaults to :obj:`constants.CONFIG_FILE`
         :type file: :class:`PathLike`
 
+        :param overrides: Replace items in `config` with these parameters,
+            defaults to ``{}``
+        :type overrides: :class:`BarSpec`
+
         :returns: A new :class:`Bar`
         :rtype: :class:`Bar`
         '''
-        template = BarTemplate.from_file(file)
-        return cls.from_template(template)
+        config = BarConfig.from_file(file)
+        return cls.from_config(config, overrides=overrides)
 
     @classmethod
     def from_cli(cls) -> Self:
         '''
         Return a new :class:`Bar` using command line arguments.
 
         :returns: a new :class:`Bar` using command line arguments
         :rtype: :class:`Bar`
         '''
-        template = BarTemplate.from_stdin()
-        return cls.from_template(template)
+        config = BarConfig.from_stdin()
+        return cls.from_config(config)
 
 ##    @classmethod
 ##    def as_generator(cls, 
 
     @property
     def clearline_char(self) -> str:
         '''
@@ -680,14 +831,18 @@
     def in_a_tty(self) -> bool:
         '''True if the bar was run from a terminal, otherwise False.'''
         if self._stream is None:
             return False
         return self._stream.isatty()
 
     @property
+    def running(self) -> bool:
+        return self._running()
+
+    @property
     def separator(self) -> Separator:
         '''
         The field separator as determined by the output stream.
         It defaults to the TTY sep (self._separators[1]) if no stream is set.
         '''
         if self._stream is None:
             # Default to using the terminal separator:
@@ -696,15 +851,15 @@
 
     def append(self, field: FieldPrecursor) -> Self:
         '''
         Append a new Field to the bar.
 
         `field` will be converted to :class:`Field`,
         appended to the field list and joined to the end of the bar output.
-        If :attr:`Bar.fmt` is defined, it will override the new field order.
+        If :attr:`Bar.template` is defined, it will override the new field order.
 
         :param field: The field to append
         :type field: :class:`FieldPrecursor`
 
         :returns: The modified bar
         :rtype: :class:`Bar`
         '''
@@ -715,83 +870,62 @@
         return self
 
     def extend(self, fields: Iterable[FieldPrecursor]) -> Self:
         '''
         Append several new Fields to the bar.
         Field precursors in `fields` will be converted to :class:`Field`,
         appended to the field list and joined to the end of the bar output.
-        If :attr:`Bar.fmt` is defined, it will override the new field order.
+        If :attr:`Bar.template` is defined, it will override the new field order.
         the fields are displayed.
 
         :param field: The fields to append
         :type field: :class:`FieldPrecursor`
 
         :returns: The modified bar
         :rtype: :class:`Bar`
         '''
-        #TODO: Consider Bar.fmt += FormatterFieldSig(field).as_string()
+        #TODO: Consider Bar.template += FormatterFieldSig(field).as_string()
         names, normalized = self._normalize_fields(fields)
         self._fields.update(normalized)
         self._buffers.update(dict.fromkeys(names, ''))
         self._field_order.extend(names)
         return self
 
-
     @staticmethod
-    def parse_fmt(
-        fmt: FormatStr
-    ) -> tuple[FieldOrder, FmtStrStructure]:
-        '''
-        Return a dict mapping field names to :class:`FormatterFieldSig`.
-        Keys of the dict can act as a field order.
-
-        :param fmt: A format string to parse
-        :type fmt: :class:`FormatStr`
-
-        :returns: A dict of fields found in the format string
-        :rtype: :class:`dict[FieldName, FormatterFieldSig]`
-
-        :raises: :exc:`errors.BrokenFormatStringError` when `fmt`
-            is malformed
-        :raises: :exc:`errors.MissingFieldnameError` when `fmt`
-            contains positional fields
-        '''
-        try:
-            sigs = tuple(
-                FormatterFieldSig(*field)
-                for field in Formatter().parse(fmt)
-            )
+    def _check_stream(
+        stream: IO,
+        raise_on_fail: bool = True
+    ) -> NoReturn | None:
+        '''
+        Check if an IO stream has proper methods for use by :class:`Bar`.
+        If any methods are missing,
+            return ``False`` if `raise_on_fail` is ``False``, or
+            raise :exc:`InvalidBarError` if `raise_on_fail` is ``True``.
+        Otherwise, return ``True``.
 
-        except ValueError:
-            err = f"Invalid bar format string: {fmt!r}"
-            raise BrokenFormatStringError(err) from None
-
-        if any(sig.name == '' for sig in sigs):
-            # There's a positional field somewhere.
-            # Issue an actionable error message:
-            epilogue = (
-                "Bar format string fields must all have fieldnames."
-                "\nPositional fields ('{}' for example) are not allowed."
-            )
-            raise MissingFieldnameError.with_highlighting(sigs, epilogue)
-
-        names = tuple(name for sig in sigs if (name := sig.name) is not None)
+        :param stream: The IO stream object to test
+        :type stream: :class:`IO`
 
-        return names, sigs
+        :param raise_on_fail: Raise exception if `stream` fails the check,
+            defaults to ``True``
+        :type raise_on_fail: :class:`bool`
 
-    @staticmethod
-    def _check_stream(stream: IO) -> None | NoReturn:
-        '''Raise TypeError if the output stream has the required methods.'''
+        :raises: :exc:`InvalidOutputStreamError` if the stream fails the
+            test and lacks required instance methods
+        '''
         io_methods = ('write', 'flush', 'isatty')
         if not all(hasattr(stream, a) for a in io_methods):
+            if not raise_on_fail:
+                return False
             io_method_calls = [a + '()' for a in io_methods]
             joined = utils.join_options(io_method_calls, final_sep='and')
-            raise TypeError(
+            raise InvalidOutputStreamError(
                 f"Output stream {stream!r} needs {joined} methods."
-            )
+            ) from None
+        return True
 
     def _normalize_fields(
         self,
         fields: Iterable[FieldPrecursor],
     ) -> tuple[FieldOrder, dict[FieldName, Field]]:
         '''
         Convert :class:`Field` precursors to :class:`Field` instances.
@@ -810,27 +944,31 @@
 
         :raises: :exc:`errors.InvalidFieldError` when an element
             of `fields` is not a :class:`FieldPrecursor`
         '''
         normalized = {}
         names = []
 
+##        if isinstance(fields, FmtStrStructure):
+##            names = parsed.get_names()
+
         for field in fields:
             if isinstance(field, Field):
                 new_field = field
                 new_field._bar = self
 
             elif isinstance(field, str):
                 new_field = Field.from_default(
                     name=field,
                     overrides={'bar': self},
                 )
 
             elif isinstance(field, FormatterFieldSig):
                 if field.name is None:
+                    # Skip sigs that lack fields:
                     continue
                 new_field = Field.from_default(
                     name=field.name,
                     overrides={'bar': self}
                 )
                 new_field._fmtsig = field.as_string()
 
@@ -841,72 +979,97 @@
             names.append(new_field.name)
 
         return names, normalized
 
     def line_generator(self) -> Iterator:
         '''
         Return a generator yielding status lines.
+        This requires running the Fields in a separate thread,
+        which has yet to be implemented.
         '''
-        while self.running():
+        while self._running():
             if self._timely_fields:
                 self._preload_timely_fields()
             line = self._make_one_line()
             yield line
 
-    def run(self, once: bool = None, stream: IO = None) -> None:
+    def current_line(self) -> Line:
+        '''
+        Return the most recently printed line.
+        '''
+        return self._make_one_line()
+
+    def run(
+        self,
+        once: bool = None,
+        stream: IO = None,
+        *,
+        bg: bool = False
+    ) -> None:
         '''
         Run the bar in the specified output stream.
         Block until an exception is raised and exit smoothly.
 
         :param stream: The IO stream in which to run the bar,
             defaults to :attr:`Bar._stream`
         :type stream: :class:`IO`
 
-        :param once: Whether to print the bar only once, defaults to ``False``
+        :param once: Run the bar only once,
+            defaults to :attr:`Bar.run_once`
         :type once: :class:`bool`
 
+        :param bg: (Not fully implemented)
+            Run the bar in the background without printing,
+            defaults to ``False``
+            This is used for :func:`Bar.line_generator` and for testing.
+        :type bg: :class:`bool`
+
         :returns: ``None``
 
         .. note::
             This method cannot be called within an async event loop.
         '''
-        if stream is not None:
-            self._stream = stream
-        if once is None:
-            once = self.run_once
-        else:
-            self.run_once = once
-
-        # Allow the bar to run repeatedly in the same interpreter:
-        if self._loop.is_closed():
-            self._loop = asyncio.new_event_loop()
-
         try:
-            # The following must be done in a very specific order.
-            self._can_run.set()
+            if stream is not None:
+                self._stream = stream
+            if once is None:
+                once = self.run_once
+            else:
+                self.run_once = once
+
+            # Allow the bar to run repeatedly in the same interpreter:
+            if self._loop.is_closed():
+                self._loop = asyncio.new_event_loop()
+            #NOTE: Need a way to handle stale coroutines.
+            # Like, run prepare_fields() again.
+
+##            self._coros = {}
+##            self._threads = {}
+##            self._timely_fields = []
             self._prepare_fields()
+            self._can_run.set()
+            for thread in tuple(self._threads.values()):
+                thread.start()
+            self._preload_timely_fields()
 
-            # When printing indefinitely, if the line printer is not
-            # started before coros, the bar is blank the whole time.
             if not once:
                 self._start_printer()
 
-            self._loop.run_until_complete(self._start_coros())
-
-            # Wait for threads to finish to get a full line, then print.
-            while self._threads:
-                time.sleep(self._thread_cooldown)
-            self._print_one_line()
+            # This blocks:
+            self._loop.run_until_complete(self._gather_coros())
 
             if once:
+                # Wait for threads to finish to get a full line, then print.
+                while self._threads:
+                    time.sleep(self._thread_cooldown)
+                self._print_one_line()
                 self._can_run.clear()
 
-            # Block the main thread while other threads run, if there
-            # are no coroutines.
-            while self.running():
+            # Prevent the bar from exiting when there are no coroutines:
+            while self._running():
                 time.sleep(self._thread_cooldown)
 
         except KeyboardInterrupt:
             pass
 
         finally:
             self._shutdown()
@@ -914,227 +1077,230 @@
     def _prepare_fields(self) -> None:
         overriding = False
         for field in self:
             if field.overrides_refresh:
                 overriding = True
 
             if field.threaded:
-                field.send_to_thread(run_once=self.run_once)
+                thread = field.make_thread(bar=self, run_once=self.run_once)
+                self._threads[thread.name] = thread
             elif field.timely:
                 self._timely_fields.append(field)
             else:
-                self._coros.append(field.run(self.run_once))
+                self._coros[field.name] = field.run(
+                    bar=self, once=self.run_once
+                )
+
 ##        if overriding:  # Currently disabled!
 ##            self._coros.append(self._handle_overrides())
 
-    async def _start_coros(self) -> None:
-        await asyncio.gather(*self._coros)
+    async def _gather_coros(self) -> None:
+        '''
+        Run :class:`Bar` coroutines in parallel.
+        '''
+        await asyncio.gather(*self._coros.values())
 
     def _preload_timely_fields(self) -> None:
         '''
         Update the bar buffers for Fields with :attr:`Field.timely`.
         This is used most often right before printing a line.
         '''
         for f in self._timely_fields:
             if f.is_async:
-                result = asyncio.run(f._func(*f.args, **f.kwargs))
+                result = self._loop.run_until_complete(
+                    f._func(*f.args, **f.kwargs)
+                )
             else:
                 result = f._func(*f.args, **f.kwargs)
-            self._buffers[f.name] = result
+
+            if f.template is not None:
+                contents = f.template.format(result, icon=f.icon)
+            else:
+                if f.always_show_icon or result:
+                    contents = f.icon + result
+                else:
+                    contents = result
+            self._buffers[f.name] = contents
 
     def _start_printer(self, end: str = '\r') -> None:
+        '''
+        Make a thread in which to run
+            :meth:`Bar._threaded_continuous_line_printer` and start it.
+        '''
+        thread_name = 'PRINTER'
         self._printer_thread = threading.Thread(
             target=self._threaded_continuous_line_printer,
-            name='PRINTER',
+            name=thread_name,
             args=(end,)
         )
-        self._threads.add(self._printer_thread)
+        self._threads[thread_name] = self._printer_thread
         self._printer_thread.start()
 
     def _threaded_continuous_line_printer(self, end: str = '\r') -> None:
         '''
         The bar's primary line-printing mechanism.
         Fields with the ``timely`` attribute get run here.
         Other fields are responsible for sending data to bar buffers.
         This only writes using the current buffer contents.
 
         :param end: The string appended to the end of each line
         :type end: :class:`str`
         '''
-        using_format_str = (self.fmt is not None)
-        sep = self.separator
-        clock = time.monotonic
+        # Make an event loop for this thread:
+        self._printer_loop = asyncio.new_event_loop()
+
+        # Flushing the buffer before writing to it fixes poor i3bar
+        # alignment.
+        self._stream.flush()
 
         if self.in_a_tty:
             beginning = self.clearline_char + end
             self._stream.write(CSI + HIDE_CURSOR)
         else:
             beginning = self.clearline_char
 
-        # Flushing the buffer before writing to it fixes poor i3bar alignment.
-        self._stream.flush()
+        # Print something right away just so that the bar is not empty,
+        # but not if the print count matters:
+        if not self.count:
+            line = self._make_one_line()
+            self._stream.write(beginning + line + end)
+            self._stream.flush()
 
-        # Print something right away just so that the bar is not empty:
-        self._print_one_line()
+        using_format_str = (self.template is not None)
+        sep = self.separator
+        clock = time.monotonic
+        step = self._thread_cooldown
+        needed = round(self.refresh_rate / step)
+        count = 0
+        first_cycle = True
 
         if self.align_to_seconds:
-            # Begin every refresh at the start of a clock second:
+            # Sleep until the beginning of the next second.
             clock = time.time
             time.sleep(1 - (clock() % 1))
 
-        step = self._thread_cooldown
-        count = 0
-        needed = round(self.refresh_rate / step)
-
         start_time = clock()
-        while self.running():
+        while self._running():
 
-            # Sleep until the next refresh cycle, pausing for a bit in
-            # case the bar stops.
-            if count < needed:
+            # Sleep until the next refresh cycle in little steps to
+            # check if the bar has stopped.
+            if count < needed and not first_cycle:
                 count += 1
 
                 # Latency from nonzero execution times causes drift,
                 # where sleeps become out-of-sync and the bar skips
                 # field updates.
                 # This is especially noticeable in fields that update
                 # routinely, such as the time.
 
                 # To negate drift, when sleeping until the beginning of
                 # the next cycle, we must also compensate for latency.
                 time.sleep(
                     step - (
                         # Get the current latency, which can vary:
                         clock() % step
+                        # (clock() - start_time) % step To preserve offset
                     )
                 )
                 continue
 
             count = 0
+            if first_cycle:
+                first_cycle = False
 
             # Run time-sensitive fields right away:
             for f in self._timely_fields:
                 if f.is_async:
-                    result = asyncio.run(f._func(*f.args, **f.kwargs))
+                    result = self._printer_loop.run_until_complete(
+                        f._func(*f.args, **f.kwargs)
+                    )
                 else:
                     result = f._func(*f.args, **f.kwargs)
-                self._buffers[f.name] = result
+
+                if f.template is not None:
+                    contents = f.template.format(result, icon=f.icon)
+                else:
+                    if f.always_show_icon or result:
+                        contents = f.icon + result
+                    else:
+                        contents = result
+                self._buffers[f.name] = contents
 
             if using_format_str:
-                line = self.fmt.format_map(self._buffers)
+                line = self.template.format_map(self._buffers)
             else:
                 line = sep.join(
                     buf for field in self._field_order
                         if (buf := self._buffers[field])
                         or self.join_empty_fields
                 )
 
             self._stream.write(beginning + line + end)
             self._stream.flush()
 
+            if self.count:
+                self._print_countdown -= 1
+                if self._print_countdown == 0:
+                    self._can_run.clear()
+                    self._printer_loop.stop()
+                    self._printer_loop.close()
+                    return
+
+        self._printer_loop.stop()
+        self._printer_loop.close()
+
     def _shutdown(self) -> None:
         '''
         Notify fields that the bar has stopped and join threads.
         Also print a newline and unhide the cursor if the bar was
-        running in a TTY.
+        running in a terminal.
         '''
         self._can_run.clear()
-        for thread in self._threads:
+
+        threads = tuple(self._threads.items())
+        for thread_name, thread in threads:
             thread.join()
+            self._threads.pop(thread_name)
 
         if self.in_a_tty:
             self._stream.write('\n')
             self._stream.write(CSI + UNHIDE_CURSOR)
 
-    async def _continuous_line_printer(self, end: str = '\r') -> None:
-        '''
-        The bar's primary line-printing mechanism.
-        Fields are responsible for sending data to the bar buffers.
-        This only writes using the current buffer contents.
-
-        :param end: The string appended to the end of each line
-        :type end: :class:`str`
-        '''
-        using_format_str = (self.fmt is not None)
-        sep = self.separator
-        clock = time.monotonic
-
-        if self.in_a_tty:
-            beginning = self.clearline_char + end
-            self._stream.write(CSI + HIDE_CURSOR)
-        else:
-            beginning = self.clearline_char
-
-        # Flushing the buffer before writing to it fixes poor i3bar alignment.
-        self._stream.flush()
-
-        # Print something right away just so that the bar is not empty:
-        self._print_one_line()
-
-        if self.align_to_seconds:
-            # Begin every refresh at the start of a clock second:
-            clock = time.time
-            await asyncio.sleep(1 - (clock() % 1))
-
-        start_time = clock()
-        while self.running():
-            if using_format_str:
-                line = self.fmt.format_map(self._buffers)
-            else:
-                line = sep.join(
-                    buf for field in self._field_order
-                        if (buf := self._buffers[field])
-                        or self.join_empty_fields
-                )
-
-            self._stream.write(beginning + line + end)
-            self._stream.flush()
-
-            # Sleep only until the next possible refresh to keep the
-            # refresh cycle length consistent and prevent drifting.
-            await asyncio.sleep(
-                # Time until next refresh:
-                self.refresh_rate - (
-                    # Get the current latency, which can vary:
-                    (clock() - start_time) % self.refresh_rate  # Preserve offset
-                )
-            )
-
     async def _handle_overrides(self, end: str = '\r') -> None:
         '''
         Print a line when fields with overrides_refresh send new data.
 
         :param end: The string appended to the end of each line
         :type end: :class:`str`
         '''
         sep = self.separator
-        using_format_str = (self.fmt is not None)
+        using_format_str = (self.template is not None)
 
         if self.in_a_tty:
             beginning = self.clearline_char + end
         else:
             beginning = self.clearline_char
 
         start_time = time.time()
-        while self.running():
+        while self._running():
 
             try:
                 # Wait until a field with overrides_refresh sends new
                 # data to be printed:
                 field, contents = await self._override_queue.get()
                 # if DEBUG:
                     # logger.debug(f"handler: {field} {time.time() - start_time}")
 
             except RuntimeError:
                 # asyncio raises RuntimeError if the event loop closes
                 # while queue.get() is waiting for a value.
                 return
 
             if using_format_str:
-                line = self.fmt.format_map(self._buffers)
+                line = self.template.format_map(self._buffers)
             else:
                 line = sep.join(
                     buf for field in self._field_order
                         if (buf := self._buffers[field])
                         or self.join_empty_fields
                 )
 
@@ -1142,16 +1308,16 @@
             self._stream.flush()
             await asyncio.sleep(self._override_cooldown)
 
     def _make_one_line(self) -> Line:
         '''Make a line using the bar's field buffers.
         This method is not meant to be called from within a loop.
         '''
-        if self.fmt is not None:
-            line = self.fmt.format_map(self._buffers)
+        if self.template is not None:
+            line = self.template.format_map(self._buffers)
         else:
             line = self.separator.join(
                 buf for field in self._field_order
                     if (buf := self._buffers[field])
                     or self.join_empty_fields
             )
         return line
@@ -1164,31 +1330,52 @@
         :type end: :class:`str`
         '''
         if self.in_a_tty:
             beginning = self.clearline_char + end
         else:
             beginning = self.clearline_char
 
-        # Flushing the buffer before writing to it fixes poor i3bar alignment.
-        self._stream.flush()
-
         if self._timely_fields:
             self._preload_timely_fields()
         self._stream.write(beginning + self._make_one_line() + end)
 
         self._stream.flush()
 
 
 def run(once: bool = False, file: PathLike = None) -> NoReturn | None:
     '''
-    Generate a new :class:`Bar` and run it in STDOUT.
-    Optionally generate the bar from a config file.
+    Generate a new :class:`Bar` from a config file and run it in STDOUT.
+    Ask to write the file if it doesn't exist.
 
     :param once: Print the bar only once, defaults to ``False``
     :type once: :class:`bool`
 
-    :param file: The config file to source, defaults to :obj:`constants.CONFIG_FILE`
+    :param file: The config file to source,
+        defaults to :obj:`constants.CONFIG_FILE`
     :type file: :class:`PathLike`
     '''
-    bar = Bar.from_file(file)
-    bar.run(once=once)
+##    import __main__ as possibly_repl
+##    if not hasattr(possibly_repl, '__file__'):
+##        # User is in a REPL
+    try:
+
+        try:
+            bar = Bar.from_file(file)
+        except FileNotFoundError as e:
+            _p_ = __package__
+            msg = (
+                f"Try running `{_p_}.write_initial_config()`"
+                f" if this is your first time using {_p_}."
+            )
+            e.add_note(msg)
+            raise e from None
+
+        bar.run(once=once)
+
+    except KeyboardInterrupt:
+        print()
+        return
+
+
+def write_initial_config() -> None:
+    BarConfig.write_with_approval(CONFIG_FILE)
```

### Comparing `mybar-0.6/mybar/cli.py` & `mybar-0.7/mybar/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,24 @@
     'OptionsAsker',
 )
 
 
 from argparse import ArgumentParser, SUPPRESS, Namespace, HelpFormatter
 from enum import Enum
 
-from .errors import AskWriteNewFile, FatalError, CLIUsageError
-from ._types import BarTemplateSpec, FieldName, OptName, OptSpec
+from .errors import AskWriteNewFile, CLIFatalError, CLIUsageError
+from .templates import BarConfigSpec, FieldSpec
+from ._types import (
+    AssignmentOption,
+    FieldName,
+    OptName,
+    OptSpec,
+)
 
-from typing import Any, Callable, NoReturn
+from typing import Any, Callable, Iterable, NoReturn
 
 
 PROG = __package__
 
 
 class ArgFormatter:
     '''
@@ -46,15 +52,15 @@
     def __init__(self) -> None:
         super().__init__(
             prog=PROG,
             argument_default=SUPPRESS,
         )
         self.add_arguments()
 
-    def parse_args(self, args: None | list[str] = None) -> BarTemplateSpec:
+    def parse_args(self, args: None | list[str] = None) -> BarConfigSpec:
         '''
         Parse command line arguments and return a dict of options.
         This will additionally process args with key-value pairs.
         If `args` is None, process from STDIN.
 
         :param args: The args to parse, get from STDIN by default
         :type args: :class:`list[str]`
@@ -62,17 +68,17 @@
         # Use vars() because dict items are more portable than attrs.
         opts = vars(super().parse_args(args))
         params = self.process_assignment_args(opts)
         return params
 
     def process_assignment_args(
         self,
-        opts: BarTemplateSpec,
+        opts: BarConfigSpec,
         assignments: dict[FieldName, str] = None
-    ) -> BarTemplateSpec:
+    ) -> BarConfigSpec:
         '''
         Make dicts from key-value pairs in assignment args.
         How does it work?
         I don't remember!
         '''
         if assignments is None:
             assignments = self.assignment_arg_map
@@ -82,37 +88,119 @@
                 opts[new_dest] = dict(
                     pair for item in vals
                     # Only use items that are pairs:
                     if len(pair := item.split('=', 1)) == 2
                 )
         return opts
 
+    @staticmethod
+    def process_field_options(
+        options: Iterable[AssignmentOption]
+    ) -> dict[FieldName, FieldSpec]:
+        '''
+        Parse variable assignment args given for Field definitions.
+        Each option in `options` should look like 'key=val'.
+        We specifically handle Field options. To that end, parse nested
+        options with emulated dotted attribute access by ignoring all
+        options not of the form 'field.key=val'.
+        After parsing options, return a dict mapping them to Field names,
+        similar to `field_definitions` in :meth:`Bar.from_config()`.
+
+        I think this has some logical chinks. Definitely overengineered.
+
+        :param options: Assignment option 'key=val' pairs to parse
+        :type options: Iterable[:class:`AssignmentOption`]
+
+        :returns: a dict mapping Field names to dicts of options
+        :rtype: :class:`dict`[:class:`FieldName`, :class:`FieldSpec`]
+        '''
+        field_definitions = {}
+        for opt in options:
+            match (pair := opt.split('=', 1)):
+
+                case [positional]:
+                    # Looks like '--opt'
+                    # Skip command options.
+                    continue
+
+                case [field_and_opt, val]:  # Looks like 'key=val'
+                    if field_and_opt.isidentifier():
+                        # No dots means it's an option for the Bar.
+                        # Not our problem.
+                        continue
+
+                    if val == "''":  # Looks like "key=''"
+                        val = ''
+                    elif not val:  # Looks like 'key='
+                        val = None
+
+                    # Looks like 'field.key=val'
+                    # An option for a Field.
+                    # Handle attribute access through dots:
+                    field_name, field_opt = field_and_opt.split('.', 1)
+                    if field_name not in field_definitions:
+                        field_definitions[field_name] = {}
+
+                    maybe_kwargs = field_opt.split('.', 1)
+
+                    match maybe_kwargs:
+
+                        case ['kwargs']:
+                            # Looks like 'field.kwargs={"k": "v", ...}'
+                            val = {} if val is None else eval(val)
+                            # Yes, I know, it's eval.
+
+                        case ['kwargs', nested]:
+                            if nested.isidentifier():
+                                # Looks like 'field.kwargs.k=v'
+                                kwarg = {nested: val}
+                                val = kwarg
+                                field_opt = 'kwargs'
+
+                            else:
+                                pass
+
+                        case [not_kwargs]:
+                            # field_opt is valid.
+                            pass
+
+                        case _:
+                            # Nonsense
+                            msg = (
+                                f"{opt !r} is invalid option syntax."
+                            )
+                            raise CLIUsageError(msg)
+
+                    field_definitions[field_name].update({field_opt: val})
+
+        return field_definitions
+
     def add_arguments(self) -> None:
         '''Equip the parser with all its arguments.'''
         fields_or_fmt = self.add_mutually_exclusive_group()
         fields_or_fmt.add_argument(
-            '-m', '--format',
-            metavar="'FORMAT_STRING'",
-            dest='fmt',
+            '-t', '--template',
+            metavar="'TEMPLATE'",
+            dest='template',
             help=(
-                "A curly-brace-delimited format string. "
-                "Not valid with --fields/-f options."
+                "A curly-brace-delimited format string."
+                " Not valid with --fields/-f options."
             ),
         )
 
         fields_or_fmt.add_argument(
             '-f', '--fields',
             action='extend',
             nargs='+',
             metavar=('FIELDNAME1', 'FIELDNAME2'),
             dest='field_order',
             # type=ArgFormatter.SplitFirst(','),
             help=(
-                "A list of fields to be displayed. "
-                "Not valid with --format/-m options."
+                "A list of fields to be displayed."
+                " Not valid with --format/-m options."
             ),
         )
 
         fields_group = self.add_argument_group(
             title="Options for fields",
             description="These options are not valid when using --format/-m."
         )
@@ -128,29 +216,41 @@
 
         fields_group.add_argument(
             '-s', '--separator',
             type=ArgFormatter.ToTuple(length=2),
             metavar="'FIELD_SEPARATOR'",
             dest='separators',
             help=(
-                "The character used for joining fields. "
-                "Only valid with --field/-f options."
+                "The character used for joining fields."
+                " Only valid with --field/-f options."
             ),
         )
 
         fields_group.add_argument(
             '--join-empty', '-j',
             action='store_true',
             dest='join_empty_fields',
             help=(
-                "Include empty field contents instead of hiding them. "
-                "Only valid with --field/-f options."
+                "Include empty field contents instead of hiding them."
+                " Only valid with --field/-f options."
             ),
         )
 
+        fields_group.add_argument(
+            '--options', '-o',
+            action='extend',
+            nargs='+',
+            metavar=("'FIELD1.OPTION=VAL'", "'FIELD2.OPTION=VAL'"),
+            dest='field_options',
+            help=(
+                "Set arbitrary options for discrete Fields using"
+                " dot-attribute syntax.",
+            )
+        )
+
         self.add_argument(
             '-r', '--refresh',
             type=float,
             dest='refresh_rate',
             help=(
                 "The bar's refresh rate in seconds per cycle."
             ),
@@ -162,26 +262,27 @@
             dest='config_file',
             help=(
                 "The config file to use for default settings."
             ),
         )
 
         self.add_argument(
-            '--once', '-o',
-            action='store_true',
-            dest='run_once',
+            '--count', '-n',
+            type=int,
+            metavar='TIMES',
+            dest='count',
             help=(
-                "Run the bar once rather than continuously."
+                "Print the bar this many times, then exit."
             ),
         )
 
         self.add_argument(
             '--debug',
             action='store_true',
-            help="Use debug mode.",
+            help="Use debug mode. (Not implemented)",
         )
 
     def quit(self, message: str = "Exiting...") -> NoReturn:
         '''Print a message and exit the program.'''
         self.exit(1, message + '\n')
```

### Comparing `mybar-0.6/mybar/constants.py` & `mybar-0.7/mybar/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 __all__ = (
     'CONFIG_FILE',
-    'DEBUG'
+    'DEBUG',
+    'CSI',
+    'CLEAR_LINE',
+    'HIDE_CURSOR',
+    'UNHIDE_CURSOR',
+    'FONTAWESOME_ICONS',
+    'USING_FONTAWESOME'
 )
 
 
 from ._types import ConsoleControlCode
+import os.path
 
 
-CONFIG_FILE: str = '~/.mybar.json'
+CONFIG_FILE: str = os.path.abspath(os.path.expanduser(
+    '~/.config/mybar/conf.json'
+))
 '''The default bar config file path.'''
+
 DEBUG: bool = False
 '''The default debug state.'''
 
 
 # Used by Bar:
 CSI: ConsoleControlCode = '\033['
 '''Unix terminal escape code (control sequence introducer).'''
+
 CLEAR_LINE: ConsoleControlCode = '\x1b[2K'
 '''VT100 escape code to clear the line.'''
+
 HIDE_CURSOR: ConsoleControlCode = '?25l'
 '''VT100 escape code to hide the cursor.'''
+
 UNHIDE_CURSOR: ConsoleControlCode = '?25h'
 '''VT100 escape code to unhide the cursor.'''
 
 
 FONTAWESOME_ICONS = tuple('')
 USING_FONTAWESOME = False
```

### Comparing `mybar-0.6/mybar/errors.py` & `mybar-0.7/mybar/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 __all__ = (
     'AskWriteNewFile',
     'BrokenFormatStringError',
+    'CLIFatalError',
     'CLIUsageError',
     'DefaultFieldNotFoundError',
     'FailedSetup',
-    'FatalError',
     'FormatStringError',
     'IncompatibleArgsError',
     'InvalidArgError',
+    'InvalidBarError',
     'InvalidFieldError',
     'InvalidFieldSpecError',
-    'InvalidFormatStringFieldError',
+    'InvalidFormatStringFieldNameError',
     'InvalidOutputStreamError',
-    'MissingBarError',
     'MissingFieldnameError',
     'UndefinedFieldError',
 )
 
 
 from os import PathLike
-from typing import Any, IO
 
-from ._types import (
+from .formatting import (
     Contents,
-    FieldSpec,
     FormatStringError,
     BrokenFormatStringError,
+    InvalidFormatStringFieldNameError,
+    InvalidFormatStringFormatSpecError,
     MissingFieldnameError
 )
 
+from typing import Any, IO
 
 
 class DefaultFieldNotFoundError(LookupError):
     '''
     Raised for references to an undefined default :class:`Field`.
     '''
     pass
@@ -59,56 +60,52 @@
 
 class InvalidFieldSpecError(TypeError):
     '''
     Raised when an expected :class:`FieldSpec` has the wrong type or an invalid structure.
     '''
     pass
 
-class InvalidFormatStringFieldError(LookupError):
+class InvalidBarError(AttributeError):
     '''
-    Raised when a format string has a field name not allowed or
-    not defined by kwargs in a :meth:`str.format()` call.
+    Raised when Field._check_bar() finds missing attributes in a
+    potential status bar.
     '''
-    pass
 
 class InvalidOutputStreamError(AttributeError):
     '''
     Raised when an :class:`IO` stream lacks ``write()``,
     ``flush()`` and ``isatty()`` methods.
     '''
     pass
 
-class MissingBarError(AttributeError):
-    '''
-    Raised when :meth:`Field.run()` is called before its instance is passed to the
-    `fields` parameter in :meth:`Bar.__init__()`.
-    '''
-    pass
-
 class UndefinedFieldError(LookupError):
     '''
     Raised if, when parsing a config file, a field name appears in the
     `field_order` item of the :class:`dict` passed to :meth:`Bar.from_dict()` that is neither
     found in its `field_definitions` parameter nor in :attr:`Field._default_fields`.
     '''
     pass
 
 
-class FatalError(Exception):
+class CLIFatalError(Exception):
     '''
     Base class for errors that cause the CLI program to exit.
 
     :param msg: The error message to issue when exiting
     :type msg: :class:`str`
     '''
     def __init__(self, msg: str) -> None:
-        super().__init__()
+        super().__init__(self)
         self.msg = msg
 
-class CLIUsageError(FatalError):
+    def __str__(self):
+        return self.msg
+
+
+class CLIUsageError(CLIFatalError):
     '''
     Raised when the CLI program is used incorrectly.
     '''
     pass
 
 
 class AskWriteNewFile(Exception):
```

### Comparing `mybar-0.6/mybar/field.py` & `mybar-0.7/mybar/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,64 +7,71 @@
 )
 
 
 import asyncio
 import threading
 import time
 
-from . import DEBUG
 from . import field_funcs
 from . import _setups
 from . import utils
+from .constants import DEBUG
 from .errors import *
+from .formatting import FormatterFieldSig
+from .templates import FieldSpec
 from ._types import (
     FieldName,
-    FieldSpec,
-    FormatterFieldSig,
     Icon,
     PTY_Icon,
     TTY_Icon,
     FormatStr,
     Args,
     Kwargs,
 )
 
 from collections.abc import Callable, Sequence
-from typing import NamedTuple, NoReturn, ParamSpec, Required, TypeAlias, TypeVar
+from typing import (
+    NamedTuple,
+    NoReturn,
+    ParamSpec,
+    Required,
+    TypeAlias,
+    TypeVar
+)
 
 Bar_T = TypeVar('Bar')
 Field = TypeVar('Field')
 P = ParamSpec('P')
 
 
 class Field:
     '''
     Continuously generates and formats one bit of information in a :class:`Bar`.
     Pre-existing default Fields can be looked up by name.
-    # Custom fields used with functions to display the output of a function
 
     :param name: A unique identifier for the new field, defaults to `func.`:attr:`__name__`
     :type name: :class:`str`
 
     :param func: The Python function to run at every `interval` if no `constant_output` is set
     :type func: :class:`Callable[[*Args, **Kwargs], str]`
 
     :param icon: The field icon, defaults to ``''``.
-        Placed before field contents or in place of ``{icon}`` in `fmt`, if provided
+        Placed before field contents or in place
+        of ``{icon}`` in `template`, if provided
     :type icon: :class:`str`
 
-    :param fmt: A curly-brace format string.
+    :param template: A curly-brace format string.
         This parameter is **required** if `icon` is ``None``.
         Valid placeholders:
             - ``{icon}`` references `icon`
             - ``{}`` references field contents
         Example:
             When the field's current contents are ``'69F'`` and its icon is ``'TEMP'``,
-            ``fmt='[{icon}]: {}'`` shows as ``'[TEMP]: 69F'``
-    :type fmt: :class:`_types.FormatStr`
+            ``template='[{icon}]: {}'`` shows as ``'[TEMP]: 69F'``
+    :type template: :class:`_types.FormatStr`
 
     :param interval: How often in seconds field contents are updated, defaults to ``1.0``
     :type interval: :class:`float`
 
     :param align_to_seconds: Update contents at the start of each second, defaults to ``False``
     :type align_to_seconds: :class:`bool`
 
@@ -105,15 +112,15 @@
         This enables the same :class:`Field` instance to use the most optimal icon automatically.
     :type icons: tuple[:class:`_types.PTY_Icon`, :class:`_types.TTY_Icon`], optional
 
 
     :raises: :exc:`errors.IncompatibleArgsError` when
         neither `func` nor `constant_output` are given
     :raises: :exc:`errors.IncompatibleArgsError` when
-        neither `icon` nor `fmt` are given
+        neither `icon` nor `template` are given
     :raises: :exc:`TypeError` when `func` is not callable
     :raises: :exc:`TypeError` when `setup`, if given, is not callable
     '''
     _default_fields = {
 
         'hostname': {
             'name': 'hostname',
@@ -130,68 +137,69 @@
             'run_once': True
         },
 
         'uptime': {
             'name': 'uptime',
             'func': field_funcs.get_uptime,
             'setup': _setups.setup_uptime,
+            'timely': True,
+            'align_to_seconds': True,
             'kwargs': {
                 'fmt': '{days}d:{hours}h:{mins}m',
                 'sep': ':'
             },
             'icons': [' ', 'Up '],
         },
 
         'cpu_usage': {
             'name': 'cpu_usage',
             'func': field_funcs.get_cpu_usage,
-            'interval': 2,
+            'interval': 5,
             'threaded': True,
             'icons': [' ', 'CPU '],
         },
 
         'cpu_temp': {
             'name': 'cpu_temp',
             'func': field_funcs.get_cpu_temp,
-            'interval': 2,
+            'interval': 5,
             'threaded': True,
             'icons': [' ', ''],
         },
 
         'mem_usage': {
             'name': 'mem_usage',
             'func': field_funcs.get_mem_usage,
-            'interval': 2,
+            'interval': 5,
             'icons': [' ', 'Mem '],
         },
 
         'disk_usage': {
             'name': 'disk_usage',
             'func': field_funcs.get_disk_usage,
-            'interval': 4,
+            'interval': 5,
             'icons': [' ', '/:'],
         },
 
         'battery': {
             'name': 'battery',
             'func': field_funcs.get_battery_info,
+            'threaded': True,
             'icons': [' ', 'Bat '],
         },
 
         'net_stats': {
             'name': 'net_stats',
             'func': field_funcs.get_net_stats,
-            'interval': 4,
-            'threaded': True,
+            'interval': 5,
             'icons': [' ', ''],
         },
 
         'datetime': {
             'name': 'datetime',
-            # 'func': field_funcs.precision_datetime,
             'func': field_funcs.get_datetime,
             'align_to_seconds': True,
             'timely': True,
             'kwargs': {
                 'fmt': "%Y-%m-%d %H:%M:%S"
             },
         }
@@ -200,15 +208,15 @@
 
     def __init__(
         self,
         *,
         name: FieldName = None,
         func: Callable[P, str] = None,
         icon: str = '',
-        fmt: FormatStr = None,
+        template: FormatStr = None,
         interval: float = 1.0,
         align_to_seconds: bool = False,
         timely: bool = False,
         overrides_refresh: bool = False,
         threaded: bool = False,
         always_show_icon: bool = False,
         run_once: bool = False,
@@ -219,15 +227,15 @@
         setup: Callable[P, P.kwargs] = None,
 
         # Set this to use different icons for different output streams:
         icons: Sequence[PTY_Icon, TTY_Icon] = None,
     ) -> None:
 
         if constant_output is None:
-            #NOTE: This will change when dynamic icons and fmts are implemented.
+            #NOTE: This will change when dynamic icons and templates are implemented.
             if func is None:
                 raise IncompatibleArgsError(
                     f"Either a function that returns a string or "
                     f"a constant output string is required."
                 )
             if not callable(func):
                 raise TypeError(
@@ -249,42 +257,40 @@
             )
         self._setupfunc = setup
 
         if icons is None:
             icons = (icon, icon)
         self._icons = icons
 
-        if fmt is None and icons is None:
+        if template is None and icons is None:
             raise IncompatibleArgsError(
-                "An icon is required when fmt is None."
+                "An icon is required when `template` is None."
             )
-        self.fmt = fmt
+        self.template = template
 
         self.is_async = asyncio.iscoroutinefunction(func)
 
         if self.is_async or threaded or timely:
             self._callback = func
         else:
             # Wrap synchronous functions if they aren't special:
             self._callback = self._asyncify
 
         self._bar = bar
 
-        self.timely = timely
-        self.align_to_seconds = align_to_seconds
-        self.always_show_icon = always_show_icon
+        self.timely = utils.str_to_bool(timely)
+        self.align_to_seconds = utils.str_to_bool(align_to_seconds)
+        self.always_show_icon = utils.str_to_bool(always_show_icon)
         self._buffer = None
         self.constant_output = constant_output
-        self.interval = interval
-        self.overrides_refresh = overrides_refresh
-        self.run_once = run_once
-
-        self.threaded = threaded
-        self._thread = None
+        self.interval = float(interval)
+        self.overrides_refresh = utils.str_to_bool(overrides_refresh)
+        self.run_once = utils.str_to_bool(run_once)
 
+        self.threaded = utils.str_to_bool(threaded)
         self._do_setup()
 
     def __repr__(self) -> str:
         cls = type(self).__name__
         name = self.name
         # attrs = utils.join_options(...)
         return f"{cls}({name=})"
@@ -292,15 +298,15 @@
     def __eq__(self, other: Field) -> bool:
         if not all(
             getattr(self, attr) == getattr(other, attr)
             for attr in (
                 'align_to_seconds',
                 'always_show_icon',
                 'constant_output',
-                'fmt',
+                'template',
                 '_icons',
             )
         ):
             return False
 
         if self._func is None:
             if self.constant_output == other.constant_output:
@@ -359,16 +365,16 @@
         return field
 
     @classmethod
     def from_format_string(cls, fmt: FormatStr) -> Field:
         '''
         Get a :class:`Field` from a curly-brace field in a format string.
 
-        :param fmt: The format string to convert
-        :type fmt: :class`FormatStr`
+        :param template: The format string to convert
+        :type template: :class`FormatStr`
         '''
         sig = FormatterFieldSig.from_str(fmt)
         field = cls.from_default(sig.name)
         field._fmtsig = fmt
         return field
 
     @property
@@ -384,35 +390,35 @@
         '''Wrap a synchronous function in a coroutine for simplicity.'''
         return self._func(*args, **kwargs)
 
     @staticmethod
     def _format_contents(
         text: str,
         icon: str,
-        fmt: FormatStr = None,
+        template: FormatStr = None,
         always_show_icon: bool = False
     ) -> str:
         '''A helper function that formats field contents.'''
-        if fmt is None:
+        if template is None:
             if always_show_icon or text:
                 return icon + text
             else:
                 return text
         else:
-            return fmt.format(text, icon=icon)
+            return template.format(text, icon=icon)
 
     def _auto_format(self, text: str) -> 'Contents':
         '''Non-staticmethod _format_contents...'''
-        if self.fmt is None:
+        if self.template is None:
             if self.always_show_icon or text:
                 return self.icon + text
             else:
                 return text
         else:
-            return self.fmt.format(text, icon=self.icon)
+            return self.template.format(text, icon=self.icon)
 
     def as_generator(self, once: bool = False) :
         yield self._func
 
     def _do_setup(self, args: Args = None, kwargs: Kwargs = None) -> None:
         # Use the pre-defined _setupfunc() to gather constant variables
         # for func() which might only be evaluated at runtime:
@@ -422,15 +428,15 @@
         if args is None:
             args = self.args
         if kwargs is None:
             kwargs = self.kwargs
 
         try:
             if asyncio.iscoroutinefunction(self._setupfunc):
-                setupvars = asyncio.run(
+                setupvars = asyncio.get_event_loop().run_until_complete(
                     self._setupfunc(*self.args, **self.kwargs)
                 )
             else:
                 setupvars = self._setupfunc(*self.args, **self.kwargs)
 
         # If _setupfunc raises FailedSetup with a backup value,
         # use it as the field's new constant_output:
@@ -449,15 +455,15 @@
     def sync_run(self, once: bool = None) -> 'Contents':
         # Do not run fields which have a constant output;
         # only set their bar buffer.
         if self.constant_output is not None:
             return self._auto_format(self.constant_output)
 
         if self.is_async:
-            result = asyncio.run(self._func(*self.args, **self.kwargs))
+            result = asyncio.get_event_loop().run_until_complete(self._func(*self.args, **self.kwargs))
         else:
             result = self._func(*self.args, **self.kwargs)
         contents = self._auto_format(result)
 
         return contents
 
     def gen_run(self, once: bool = None) -> 'Contents':
@@ -466,41 +472,47 @@
         if self.constant_output is not None:
             return self._auto_format(self.constant_output)
 
         while True:
             if self.is_async:
                 result = self._func(*self.args, **self.kwargs)
             else:
-                result = asyncio.run(self._func(*self.args, **self.kwargs))
+                result = asyncio.get_event_loop().run_until_complete(self._func(*self.args, **self.kwargs))
             contents = self._auto_format(result)
 
             yield contents
 
-    async def run(self, once: bool = False) -> None:
+    async def run(self, bar: Bar_T, once: bool) -> None:
         '''
-        Run an asynchronous field callback and send updates to the bar.
+        Run an async :class:`Field` callback and send its output to a
+        status bar.
+
+        :param bar: Send results to this status bar
+        :type bar: :class:`Bar`
+
+        :param once: Run the Field function once
+        :type once: :class:`bool`
         '''
-        self._check_bar()
-        bar = self._bar
+        self._check_bar(bar)
         # Do not run fields which have a constant output;
         # only set their bar buffer.
         if self.constant_output is not None:
-            bar._buffers[self.name] = self._format_contents(
+            contents = self._format_contents(
                 self.constant_output,
                 self.icon,
-                self.fmt,
+                self.template,
                 self.always_show_icon
             )
+            bar._buffers[self.name] = contents
             return
 
-        running = self._bar._can_run.is_set
-
         func = self._callback
+        running = bar._can_run.is_set
         clock = time.monotonic
-        using_format_str = (self.fmt is not None)
+        using_format_str = (self.template is not None)
         last_val = None
 
         # Use the pre-defined _setupfunc() to gather constant variables
         # for func() which might only be evaluated at runtime:
         if self._setupfunc is not None:
             try:
                 if asyncio.iscoroutinefunction(self._setupfunc):
@@ -508,31 +520,31 @@
                         await self._setupfunc(*self.args, **self.kwargs)
                     )
                 else:
                     setupvars = self._setupfunc(*self.args, **self.kwargs)
 
             # If _setupfunc raises FailedSetup with a backup value,
             # use it as the field's new constant_output and update the
-            # bar buffer:
+            # bar's buffer:
             except FailedSetup as e:
                 backup = e.backup
                 contents = self._format_contents(
                     backup,
                     self.icon,
-                    self.fmt,
+                    self.template,
                     self.always_show_icon
                 )
                 self.constant_output = contents
                 bar._buffers[self.name] = str(contents)
                 return
 
             # On success, give new values to kwargs to pass to func().
             self.kwargs['setupvars'] = setupvars
 
-        # Run at least once at the start to ensure the bar is not empty:
+        # Run at least once at the start to ensure bars have contents:
         result = await func(*self.args, **self.kwargs)
         last_val = result
         contents = self._auto_format(result)
         bar._buffers[self.name] = contents
 
         if self.run_once or once:
             return
@@ -541,14 +553,26 @@
             # Sleep until the beginning of the next second.
             clock = time.time
             await asyncio.sleep(1 - (clock() % 1))
         start_time = clock()
 
         # The main loop:
         while running():
+
+            if bar.count:
+                # Stop before running a cycle that could last too long:
+                if (
+                    bar._print_countdown == 0
+                    or self.interval > (
+                        bar._print_countdown * bar.refresh_rate 
+                    )
+                ):
+                    bar._coros.pop(self.name, None)
+                    return
+
             result = await func(*self.args, **self.kwargs)
             # Latency from nonzero execution times causes drift, where
             # sleeps become out-of-sync and the bar skips field updates.
             # This is especially noticeable in fields that update
             # routinely, such as the time.
 
             # To negate drift, when sleeping until the beginning of the
@@ -563,15 +587,15 @@
             )
 
             if result == last_val:
                 continue
             last_val = result
 
             if using_format_str:
-                contents = self.fmt.format(result, icon=self.icon)
+                contents = self.template.format(result, icon=self.icon)
             else:
                 if self.always_show_icon or result:
                     contents = self.icon + result
                 else:
                     contents = result
 
             bar._buffers[self.name] = contents
@@ -585,36 +609,43 @@
                 except asyncio.QueueFull:
                     # Since the bar buffer was just updated, do nothing if the
                     # queue is full. The update may still show while the queue
                     # handles the current override.
                     # If not, the line will update at the next refresh cycle.
                     pass
 
-    def run_threaded(self, once: bool = False) -> None:
-        '''Run a blocking function in a thread
-        and send its updates to the bar.'''
-        self._check_bar()
-        bar = self._bar
+    def run_threaded(self, bar: Bar_T, once: bool) -> None:
+        '''
+        Run a blocking :class:`Field` func and send its output to a
+        status bar.
+
+        :param bar: Send results to this status bar
+        :type bar: :class:`Bar`
+
+        :param once: Run the Field function once
+        :type once: :class:`bool`
+        '''
+        self._check_bar(bar)
+
         # Do not run fields which have a constant output;
         # only set their bar buffer.
         if self.constant_output is not None:
-            bar._buffers[self.name] = self._format_contents(
+            contents = self._format_contents(
                 self.constant_output,
                 self.icon,
-                self.fmt,
+                self.template,
                 self.always_show_icon
             )
+            bar._buffers[self.name] = contents
             return
 
-        running = self._bar._can_run.is_set
-
-        clock = time.monotonic
-        step = bar._thread_cooldown
         func = self._callback
-        using_format_str = (self.fmt is not None)
+        running = bar._can_run.is_set
+        clock = time.monotonic
+        using_format_str = (self.template is not None)
         last_val = None
 
         # If the field's callback is asynchronous,
         # it must be run in a new event loop.
         local_loop = asyncio.new_event_loop()
 
         # Use the pre-defined _setupfunc() to gather constant variables
@@ -632,98 +663,112 @@
             # use it as the field's new constant_output and update the
             # bar buffer:
             except FailedSetup as e:
                 backup = e.args[0]
                 contents = self._format_contents(
                     backup,
                     self.icon,
-                    self.fmt,
+                    self.template,
                     self.always_show_icon
                 )
                 self.constant_output = contents
                 bar._buffers[self.name] = str(contents)
                 return
 
             # On success, give new values to kwargs to pass to func().
             self.kwargs['setupvars'] = setupvars
 
-        # Run at least once at the start to ensure the bar is not empty:
+        # Run at least once at the start to ensure bar is not empty:
         if self.is_async:
             result = local_loop.run_until_complete(
                 func(*self.args, **self.kwargs)
             )
         else:
             result = func(*self.args, **self.kwargs)
         last_val = result
         contents = self._format_contents(
             result,
             self.icon,
-            self.fmt,
+            self.template,
             self.always_show_icon
         )
         bar._buffers[self.name] = contents
 
         if self.run_once or once:
             local_loop.stop()
             local_loop.close()
-            self._bar._threads.remove(self._thread)
+            bar._threads.pop(self.name)  # Eventually, id(self)
             return
 
-        count = 0
+        step = bar._thread_cooldown
         needed = round(self.interval / step)
+        count = 0
+        first_cycle = True
 
         if self.align_to_seconds:
             # Sleep until the beginning of the next second.
             clock = time.time
             time.sleep(1 - (clock() % 1))
-        start_time = clock()
 
-        # The main loop:
+        start_time = clock()
         while running():
-            # Rather than block for the whole interval,
-            # use tiny steps to check if the bar is still running.
-            # A shorter step means more chances to check if the bar stops.
-            # Thus, threads usually cancel `step` seconds after `func`
-            # returns when the bar stops rather than after `interval` seconds.
 
-            if count < needed:
+            if bar.count:
+                # Stop before running a cycle that could last too long:
+                if (
+                    bar._print_countdown == 0
+                    or self.interval > (
+                        bar._print_countdown * bar.refresh_rate 
+                    )
+                ):
+                    local_loop.stop()
+                    local_loop.close()
+                    bar._coros.pop(self.name, None)
+                    return
+
+
+            # Sleep until the next refresh cycle in little steps to
+            # check if the bar has stopped.
+            if count < needed and not first_cycle:
                 count += 1
 
                 # Latency from nonzero execution times causes drift,
                 # where sleeps become out-of-sync and the bar skips
                 # field updates.
                 # This is especially noticeable in fields that update
                 # routinely, such as the time.
 
                 # To negate drift, when sleeping until the beginning of
                 # the next cycle, we must also compensate for latency.
                 time.sleep(
                     step - (
                         # Get the current latency, which can vary:
                         clock() % step
-                        # (clock() - start_time) % step  # Preserve offset
+                        # (clock() - start_time) % step To preserve offset
                     )
                 )
                 continue
 
             count = 0
+            if first_cycle:
+                first_cycle = False
 
             if self.is_async:
                 result = local_loop.run_until_complete(
                     func(*self.args, **self.kwargs)
                 )
             else:
                 result = func(*self.args, **self.kwargs)
 
             if result == last_val:
                 continue
             last_val = result
 
             if using_format_str:
-                contents = self.fmt.format(result, icon=self.icon)
+                contents = self.template.format(result, icon=self.icon)
             else:
                 if self.always_show_icon or result:
                     contents = self.icon + result
                 else:
                     contents = result
 
             bar._buffers[self.name] = contents
@@ -742,37 +787,66 @@
                     # handles the current override.
                     # If not, the line will update at the next refresh cycle.
                     pass
 
         local_loop.stop()
         local_loop.close()
 
-    def _check_bar(self, no_error: bool = False) -> NoReturn | bool:
-        '''Raises MissingBarError if self._bar is None.'''
-        if self._bar is None:
-            if no_error:
+    @staticmethod
+    def _check_bar(
+        bar: Bar_T,
+        raise_on_fail: bool = True
+    ) -> NoReturn | bool:
+        '''
+        Check if a bar has the right attributes to use a run() function.
+        If these attributes are missing,
+            return ``False`` if `raise_on_fail` is ``True``,
+            or raise :exc:`InvalidBarError` if `raise_on_fail` is ``False``.
+
+        :param bar: The status bar object to test
+        :type bar: :class:`Bar`
+
+        :param raise_on_fail: Raise an exception if `bar` fails the check,
+            defaults to ``False``
+        :type raise_on_fail: :class:`bool`
+
+        :raises: :exc:`InvalidBarError` if the stream fails the test
+            and lacks required attributes
+        '''
+        required_attrs = (
+            '_buffers',
+            '_can_run',
+            '_override_queue',
+            '_stream',
+        )
+        if not all(hasattr(bar, a) for a in required_attrs):
+            if not raise_on_fail:
                 return False
-            raise MissingBarError(
-                "Fields cannot run until they belong to a Bar."
-            )
+            raise InvalidBarError(
+                f"Status bar {bar!r} is missing certain attributes"
+                f" required to run `Field.run()`"
+                f" and `Field.run_threaded()`."
+            ) from None
         return True
 
-    def send_to_thread(self, *, run_once: bool = True) -> None:
+    def make_thread(self, bar: Bar_T, run_once: bool) -> None:
         '''
-        Make and start a thread in which to run the :class:`Field` callback.
+        Return a thread that runs the :class:`Field`'s callback.
+
+        :param bar: Send results to this status bar
+        :type bar: :class:`Bar`
 
-        :param run_once: Only run the :class:`Field` callback once,
-            defaults to ``True`` to prevent uncontrolled thread spawning
-        :type run_once: :class:`bool`
+        :param once: Run the Field function once
+        :type once: :class:`bool`
         '''
-        self._check_bar()
-        self._thread = threading.Thread(
+        thread = threading.Thread(
             target=self.run_threaded,
-            name=self.name,
-            args=(run_once,)
+            args=(bar, run_once),
+            name=self.name  # #NOTE Eventually, id(self)
         )
-        self._bar._threads.add(self._thread)
-        self._thread.start()
+        return thread
 
 
 FieldPrecursor: TypeAlias = FieldName | Field | FormatterFieldSig
+from . import _types
+_types.FieldPrecursor = FieldPrecursor
```

### Comparing `mybar-0.6/mybar/field_funcs.py` & `mybar-0.7/mybar/field_funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,55 +17,34 @@
 import re
 import shlex
 import time
 from asyncio import subprocess as aiosp
 from datetime import datetime
 from string import Formatter
 
+# if not embedded system:
 import psutil
 
 from .errors import *
 from .formatting import ElapsedTime, ConditionalFormatStr
 from .utils import join_options
-from ._types import Contents, FormatStr, NmConnFilterSpec
+from ._types import (
+    Contents,
+    DiskMeasure,
+    FormatStr,
+    POWERS_OF_1024,
+    MetricSymbol,
+    NmConnFilterSpec
+)
 
 from collections.abc import Callable, Iterable
 from typing import Literal, TypeAlias, NamedTuple, Any
 from enum import Enum
 
 
-FormatterLiteral: TypeAlias = str|None
-FormatterFname: TypeAlias = str|None
-FormatterFormatSpec: TypeAlias = str|None
-FormatterConversion: TypeAlias = str|None
-FmtStrStructure: TypeAlias = tuple[tuple[tuple[
-    FormatterLiteral,
-    FormatterFname,
-    FormatterFormatSpec,
-    FormatterConversion
-]]]
-
-POWERS_OF_1024 = {
-    'K': 1024**1,
-    'M': 1024**2,
-    'G': 1024**3,
-    'T': 1024**4,
-    'P': 1024**5,
-}
-MetricSymbol = Literal[*POWERS_OF_1024.keys()]
-
-DiskMeasure = Literal['total', 'used', 'free', 'percent']
-
-
-##class Func:
-##    f: Callable
-##    s: Setup
-##    pass
-
-
 # Field functions
 
 async def get_audio_volume(
     fmt: FormatStr = "{:02.0f}{state}",
     *args, **kwargs
 ) -> Contents:
     '''Currently awaiting a more practical implementation that supports
@@ -89,60 +68,52 @@
     avg_pct = sum(int(p) for p in pcts) // len(pcts)
     is_on = any(s == 'on' for s in states)
     # return is_on, avg_pct
     state = "" if is_on else "M"
     return fmt.format(avg_pct, state=state)
 
 
-class Context(NamedTuple):
-    contents: str = None
-    state: Any = None
-
-class BatteryStates(Enum):
-    CHARGING = 'charging'
-    DISCHARGING = 'discharging'
-
-def ctx_get_battery_info(
-    fmt: FormatStr = "{icon}{pct:02.0f}",
-    # fmt: FormatStr = "{icon}{pct:02.0f}{state}",
-    *args, **kwargs
-) -> Context:
-    '''
-    Battery capacity as a percent and whether or not it is charging.
-    '''
-
-    # if not (battery := psutil.sensors_battery()):
-    battery = psutil.sensors_battery()
-    if not battery:
-        return Context()
-##        # return (None, None)
-    # state = "CHG" if battery.power_plugged else ''
-
-    # Progressive/dynamic battery icons!
-    icon_bank = "    ".split()
-    # return icon_bank
-
-    def mapper(n):
-        icon = ""
-        for i, test in enumerate((10, 25, 50, 75, 100)):
-            if n <= test:
-                icon = icon_bank[i]
-                return icon + " "
-
-    if battery.power_plugged:
-        icon = ""
-        # state = "CHG"
-    else:
-        icon = mapper(battery.percent)
-        # state = ""
-    # print(repricon)
-
-    info = fmt.format_map({'icon': icon, 'pct': battery.percent, 'state': battery.power_plugged})
-##    return battery.power_plugged, info
-    return info
+##def ctx_get_battery_info(
+##    fmt: FormatStr = "{icon}{pct:02.0f}",
+##    # fmt: FormatStr = "{icon}{pct:02.0f}{state}",
+##    *args, **kwargs
+##) -> Context:
+##    '''
+##    Battery capacity as a percent and whether or not it is charging.
+##    '''
+##
+##    # if not (battery := psutil.sensors_battery()):
+##    battery = psutil.sensors_battery()
+##    if not battery:
+##        return Context()
+####        # return (None, None)
+##    # state = "CHG" if battery.power_plugged else ''
+##
+##    # Progressive/dynamic battery icons!
+##    icon_bank = "    ".split()
+##    # return icon_bank
+##
+##    def mapper(n):
+##        icon = ""
+##        for i, test in enumerate((10, 25, 50, 75, 100)):
+##            if n <= test:
+##                icon = icon_bank[i]
+##                return icon + " "
+##
+##    if battery.power_plugged:
+##        icon = ""
+##        # state = "CHG"
+##    else:
+##        icon = mapper(battery.percent)
+##        # state = ""
+##    # print(repricon)
+##
+##    info = fmt.format_map({'icon': icon, 'pct': battery.percent, 'state': battery.power_plugged})
+####    return battery.power_plugged, info
+##    return info
 
 
 async def get_battery_info(
     fmt: FormatStr = "{pct:02.0f}{state}",
     *args, **kwargs
 ) -> Contents:
     '''
@@ -151,34 +122,26 @@
     :param fmt: A curly-brace format string with
         two optional named fields:
             - ``pct``: Current battery percent as a :class:`float`
             - ``state``: Whether or not the battery is charging
         Defaults to ``"{pct:02.0f}{state}"``
     :type fmt: :class:`FormatStr`
     '''
-
-    # Progressive/dynamic battery icons!
-        # 
-        # 
-        # 
-        # 
-        # 
-
     # if not (battery := psutil.sensors_battery()):
     battery = psutil.sensors_battery()
     if not battery:
         return ""
 ##        # return (None, None)
     state = "CHG" if battery.power_plugged else ''
     info = fmt.format_map({'pct': battery.percent, 'state': state})
 ##    return battery.power_plugged, info
     return info
 
 
-async def get_cpu_temp(
+def get_cpu_temp(
     fmt: str = "{temp:02.0f}{scale}",
     in_fahrenheit=False,
     *args, **kwargs
 ) -> Contents:
     '''
     Current CPU temperature in Celcius or Fahrenheit.
 
@@ -201,15 +164,15 @@
         case {'k10temp': t} | {'coretemp': t}:
             current = t[0].current
         case _:
             current = '??'
     return fmt.format_map({'temp': current, 'scale': scale})
 
 
-async def get_cpu_usage(
+def get_cpu_usage(
     fmt: FormatStr = "{:02.0f}%",
     interval: float = None,
     *args, **kwargs
 ) -> Contents:
     '''
     System CPU usage in percent over a specified interval.
 
@@ -237,25 +200,14 @@
 
     .. seealso:: `strftime() format codes <https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes>`_
 
     '''
     return datetime.now().strftime(fmt)
 
 
-def precision_datetime(
-    fmt: str = "%Y-%m-%d %H:%M:%S.%f",
-    *args, **kwargs
-) -> Contents:
-    '''Return the current time as formatted with `fmt`.
-    Being synchronous, a threaded Field can run this with
-    align_to_seconds and see less than a millisecond of offset.
-    '''
-    return datetime.now().strftime(fmt)
-
-
 async def get_disk_usage(
     fmt: FormatStr = "{free:.1f}{unit}",
     path: os.PathLike = '/',
     unit: MetricSymbol = 'G',
     *args, **kwargs
 ) -> Contents:
     '''
@@ -292,15 +244,15 @@
         for meas, val in disk._asdict().items()
     }
     converted['unit'] = unit
     usage = fmt.format_map(converted)
     return usage
 
 
-async def get_host(
+def get_host(
     fmt: FormatStr = "{nodename}",
     *args, **kwargs
 ) -> Contents:
     '''
     System host information using :func:`os.uname()`.
 
     :param fmt: A curly-brace format string with
@@ -314,20 +266,20 @@
     :type fmt: :class:`FormatStr`
     '''
     keys = ('sysname', 'nodename', 'release', 'version', 'machine')
     host = fmt.format_map(dict(zip(keys, os.uname())))
     return host
 
 
-async def get_hostname(*args, **kwargs) -> Contents:
+def get_hostname(*args, **kwargs) -> Contents:
     '''System hostname.'''
     return os.uname().nodename
 
 
-async def get_mem_usage(
+def get_mem_usage(
     fmt: FormatStr = "{used:.1f}{unit}",
     unit: MetricSymbol = 'G',
     *args, **kwargs
 ) -> Contents:
     '''
     Disk usage of a partition at a given path.
 
@@ -356,15 +308,14 @@
         for meas, val in memory._asdict().items()
     }
     converted['unit'] = unit
     usage = fmt.format_map(converted)
     return usage
 
 
-#NOTE: This is most optimal as a threaded function.
 async def get_net_stats(
     # device: str = None,
     fmt: FormatStr = "{name}",
     nm: bool = True,
     nm_filt: NmConnFilterSpec = None,
     default: str = "",
     *args, **kwargs
```

### Comparing `mybar-0.6/mybar/formatting.py` & `mybar-0.7/mybar/sync.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,539 +1,390 @@
+from .bar import Bar, BarTemplate
+import asyncio
+import json
+import os
+import sys
+import threading
+import time
+from copy import deepcopy
 from string import Formatter
 
-from .errors import InvalidFormatStringFieldError
-from .utils import join_options, make_error_message
+from .constants import CONFIG_FILE, DEBUG
+from . import cli
+from . import utils
+from .errors import *
+from .field import Field, FieldPrecursor
+from .formatting import FormatterFieldSig
 from ._types import (
-    Duration,
+    Args,
+    BarSpec,
+    BarTemplateSpec,
+    ConsoleControlCode,
+    FieldName,
+    FieldOrder,
     FmtStrStructure,
-    FormatterFname,
-    FormatterConversion,
-    FormatterFname,
-    FormatterFormatSpec,
-    FormatterLiteral,
     FormatStr,
+    Icon,
+    JSONText,
+    Kwargs,
+    Line,
+    PTY_Icon,
+    PTY_Separator,
+    Pattern,
+    Separator,
+    TTY_Icon,
+    TTY_Separator,
 )
 
-from collections.abc import Callable, Hashable, Iterable
-from typing import Any, NamedTuple, Self, TypeAlias
+from collections.abc import Iterable, Iterator, Sequence
+from os import PathLike
+from typing import IO, NoReturn, Required, Self, TypeAlias, TypedDict, TypeVar
 
 
-class FormatterFieldSig(NamedTuple):
-    '''
-    A format replacement field as generated by Formatter().parse().
+# Unix terminal escape code (control sequence introducer):
+CSI: ConsoleControlCode = '\033['
+CLEAR_LINE: ConsoleControlCode = '\x1b[2K'  # VT100 escape code to clear line
+HIDE_CURSOR: ConsoleControlCode = '?25l'
+UNHIDE_CURSOR: ConsoleControlCode = '?25h'
 
-    :param lit: Literal text preceding a replacement field
-    :type lit: :class:`FormatterLiteral`
 
-    :param name: The name of such a field, found inside curly braces
-    :type name: :class:`FormatterFname`
 
-    :param spec: The field's format spec, found inside curly braces
-    :type spec: :class:`FormatterFormatSpec`
+class SyncField(Field):
+    # For threaded fields, still run continuously!!!
 
-    :param conv: The field's conversion value, found inside curly braces
-    :type conv: :class:`FormatterConversion`, optional
-    '''
+    def _do_setup(self,) : #-> SetupVars|Content?  # side-effects?
 
-    lit: FormatterLiteral
-    name: FormatterFname
-    spec: FormatterFormatSpec
-    conv: FormatterConversion
-
-    @classmethod
-    def from_str(cls, fmt: FormatStr) -> Self:
-        '''
-        Convert a replacement field to tuple of its elements.
-        If there are multiple fields in the format string, only process the first one.
+        # Use the pre-defined _setupfunc() to gather constant variables
+        # for func() which might only be evaluated at runtime:
+        if self._setupfunc is not None:
+            try:
+##                if asyncio.iscoroutinefunction(self._setupfunc):
+##                    setupvars = (
+##                        await self._setupfunc(*self.args, **self.kwargs)
+##                    )
+##                else:
+                setupvars = self._setupfunc(*self.args, **self.kwargs)
+
+            # If _setupfunc raises FailedSetup with a backup value,
+            # use it as the field's new constant_output:
+            except FailedSetup as e:
+                backup = e.backup
+                contents = self._auto_format(backup)
+                self.constant_output = contents  # strcontents() everywhere?
+##                return contents
+
+            # On success, give new values to kwargs to pass to func().
+            return setupvars
+            self.kwargs['setupvars'] = setupvars  # Do we want side-effects???
+
+
+    def _auto_format(self, text: str) -> 'Contents':
+        '''Non-staticmethod _format_contents...'''
+        if self.fmt is None:
+            if self.always_show_icon or text:
+                return self.icon + text
+            else:
+                return text
+        else:
+            return self.fmt.format(text, icon=self.icon)
+
+    def run(self, once: bool = None) -> 'Contents':
+        # hook into setup() beforehand
+        if asyncio.iscoroutinefunction(self._func):
+            return asyncio.run(self._func(*self.args, **self.kwargs))
+        return self._func(*self.args, **self.kwargs)
+
+        # Do not run fields which have a constant output;
+        # only set their bar buffer.
+        if self.constant_output is not None:
+            return self._auto_contents(self.constant_output)
 
-        :param fmt: The format string to convert
-        :type fmt: :class:`FormatStr`
-        '''
-        try:
-            parsed = tuple(Formatter().parse(fmt))
+        result = _func(*self.args, **self.kwargs)
+        contents = self._auto_format(result)
 
-        except ValueError:
-            err = f"Invalid format string: {fmt!r}"
-            raise BrokenFormatStringError(err) from None
-
-        if not parsed:
-            err = f"The format string {fmt!r} contains no fields."
-            raise FormatStringError(err)
-
-        field = parsed[0]
-
-        # Does the field have a fieldname?
-        if field[1] == '':
-            # No; it's positional.
-            start = len(field[0])
-            err = (
-                f"The format string field at character {start} in {fmt!r} is "
-                f"missing a fieldname.\n"
-                 "Positional fields ('{}' for example) are not allowed "
-                 "for this operation."
-            )
-            raise MissingFieldnameError(err)
+        return contents
 
-        sig = cls(*field)
-        return sig
 
-    def as_string(self,
-        with_literal: bool = True,
-        with_conv: bool = True,
-    ) -> FormatStr:
+class SyncBar(Bar):
+    @classmethod
+    def from_template(
+        cls,
+        tmpl: BarTemplate,
+        *,
+        ignore_with: Pattern | tuple[Pattern] | None = '//'
+    ) -> Self:
         '''
-        Recreate a format string field from a single field signature.
+        Return a new :class:`Bar` from a :class:`BarTemplate`
+        or a dict of :class:`Bar` parameters.
+        Ignore keys and list elements starting with `ignore_with`,
+        which is ``'//'`` by default.
+        If :param ignore_with: is ``None``, do not remove any values.
+
+        :param tmpl: The :class:`dict` to convert
+        :type tmpl: :class:`dict`
+
+        :param ignore_with: A pattern to ignore, defaults to ``'//'``
+        :type ignore_with: :class:`_types.Pattern` | tuple[:class:`_types.Pattern`] | ``None``, optional
+
+        :returns: A new :class:`Bar`
+        :rtype: :class:`Bar`
+
+        :raises: :exc:`errors.IncompatibleArgsError` when
+            no `field_order` is defined
+            or when no `fmt` is defined
+        :raises: :exc:`errors.DefaultFieldNotFoundError` when either
+            a field in `field_order` or
+            a field in `fmt`
+            cannot be found in :attr:`Field._default_fields`
+        :raises: :exc:`errors.UndefinedFieldError` when
+            a custom field name in `field_order` or
+            a custom field name in `fmt`
+            is not properly defined in `field_definitions`
+        :raises: :exc:`errors.InvalidFieldSpecError` when
+            a field definition is not of the form :class:`_types.FieldSpec`
 
-        :param with_literal: Include the signature's :class:`FormatterLiteral`,
-            defaults to ``True``
-        :type with_literal: :class:`bool`
-
-        :param with_conv: Include the signature's :class:`FormatterConversion`,
-            defaults to ``True``
-        :type with_conv: :class:`bool`
+        .. note:: `tmpl` can be a regular :class:`dict`
+        as long as it matches the form of :class:`_types.BarSpec`.
 
-        :returns: The format string represented by the signature
-        :rtype: :class:`FormatStr`
         '''
-        inside_braces = self.name
-        if with_conv and self.conv is not None:
-            inside_braces += '!' + self.conv
-        inside_braces += ':' + self.spec if self.spec else self.spec
-        fmt = '{' + inside_braces + '}'
-        if with_literal:
-            return self.lit + fmt
-        return fmt
-
-
-class ConditionalFormatStr:
-    '''
-    Reinterpret format strings based on the data they reference.
-    Values in a mapping which are predicated ``False`` have their
-    groupings shown blank when the mapping is formatted.
-
-    :param fmt: The initial format string
-    :type fmt: :class:`FormatStr`
-
-    :param sep: Surrounds related fields and literal text that should be
-        grouped together, defaults to ``":"``
-    '''
-    def __init__(self,
-        fmt: FormatStr,
-        sep: str = ':'  # Other common values are , /
-    ) -> None:
-        self.fmt = fmt
-        self.sep = sep
-        self.fnames, self.groups = self.parse()
-
-    def parse(self,
-        sep: str = None
-    ) -> tuple[tuple[FormatterFname], FmtStrStructure]:
-        '''
-        Parse a format string using its format fields and a separator.
 
-        :param sep: Surrounds related fields and literal text that should be
-            grouped together, defaults to ``self.sep``
-        :type sep: :class:`str`, optional
-
-        :returns: A nested tuple of the string's fieldnames
-            and its :class:`FmtStrStructure`
-        :rtype: :class:`tuple[tuple[FormatterFname], FmtStrStructure]`
-        '''
-        if sep is None:
-            sep = self.sep
 
-        sections = []
-        # Split fmt for parsing, but join any format specs that get broken:
-        pieces = (p for p in self.fmt.split(sep))
+##        if SYNC:
+##            Field = SyncField
 
-        def _is_malformed(piece: FormatStr):
-            '''Return whether a format string is malformed.'''
-            try:
-                tuple(Formatter().parse(piece))
-            except ValueError:
-                return True
-            else:
-                return False
 
-        try:
-            for piece in pieces:
-                while _is_malformed(piece):
-                    # Raise StopIteration if a valid field end is not found:
-                    piece = sep.join((piece, next(pieces)))
-                sections.append(piece)
-
-        except StopIteration:
-            exc = make_error_message(
-                BrokenFormatStringError,
-                doing_what=f"parsing {self!r} format string {self.fmt!r}",
-                details=[
-                    f"Invalid fmt substring begins near ->{piece!r}"
-                ]
-            )
-            raise exc from None
+        if ignore_with is None:
+            data = deepcopy(tmpl)
+        else:
+            data = utils.scrub_comments(tmpl, ignore_with)
+
+        bar_params = cls._default_params | data
+        field_order = bar_params.pop('field_order', None)
+        field_icons = bar_params.pop('field_icons', {})  # From the CLI
+        field_defs = bar_params.pop('field_definitions', {})
+
+        if (fmt := bar_params.get('fmt')) is None:
+            if field_order is None:
+                raise IncompatibleArgsError(
+                    "A bar format string 'fmt' is required when field "
+                    "order list 'field_order' is undefined."
+                )
+        else:
+            field_order, field_sigs = cls.parse_fmt(fmt)
+
+        # Ensure icon assignments correspond to valid fields:
+        for name in field_icons:
+            if name not in field_order:
+                deduped = dict.fromkeys(field_order)  # Preserve order
+                expctd_from_icons = utils.join_options(deduped)
+                exc = utils.make_error_message(
+                    InvalidFieldError,
+                    doing_what="parsing custom Field icons",
+                    blame=f"{name!r}",
+                    expected=f"a Field name from among {expctd_from_icons}",
+                    epilogue="Only assign icons to Fields that will be in the Bar."
+                )
+                raise exc from None
+
+        # Gather Field parameters and instantiate them:
+        fields = {}
+        expctd_name="the name of a default or properly defined `custom` Field"
+
+        for name in field_order:
+            field_params = field_defs.get(name)
+
+            match field_params:
+                case None:
+                    # The field is strictly default.
+                    if name in fields:
+                        continue
+
+                    try:
+                        field = SyncField.from_default(name)
+                    except DefaultFieldNotFoundError:
+                        exc = utils.make_error_message(
+                            DefaultFieldNotFoundError,
+                            # doing_what="parsing 'field_order'",  # Only relevant to config file parsing
+                            blame=f"{name!r}",
+                            expected=expctd_name
+                        )
+                        raise exc from None
 
-        groups = tuple(
-            tuple(Formatter().parse(section))
-            for section in sections
-        )
+                case {'custom': True}:
+                    # The field is custom, so it is only defined in
+                    # 'field_definitions' and will not be found as a default.
+                    name = field_params.pop('name', name)
+                    del field_params['custom']
+                    field = SyncField(**field_params, name=name)
+
+                case {}:
+                    # The field is a default overridden by the user.
+                    # Are there custom icons given from the CLI?
+                    if name in field_icons:
+                        cust_icon = field_icons.pop(name)
+                        field_params['icons'] = (cust_icon, cust_icon)
+
+                    try:
+                        field = SyncField.from_default(name, overrides=field_params)
+                    except DefaultFieldNotFoundError:
+                        exc = utils.make_error_message(
+                            UndefinedFieldError,
+                            # doing_what="parsing 'field_order'",
+                            blame=f"{name!r}",
+                            expected=expctd_name,
+                            epilogue=(
+                                f"(In config files, remember to set "
+                                f"`custom=true` "
+                                f"for custom field definitions.)"
+                            ),
+                        )
+                        raise exc from None
 
-        fnames = tuple(
-            name
-            for section in groups
-            for parsed in section
-            if (name := parsed[1])
+                case _:
+                    # Edge cases.
+                    exc = utils.make_error_message(
+                        InvalidFieldSpecError,
+                        # doing_what="parsing 'field_definitions'",
+                        doing_what=f"parsing {name!r} definition",
+                        details=(
+                            f"Invalid Field specification: {field_params!r}",
+                        ),
+                        indent_level=1
+                    )
+                    raise exc from None
+
+            fields[name] = field
+
+        bar = cls(
+            fields=tuple(fields.values()),
+            field_order=field_order,
+            **bar_params
         )
+        return bar
 
-        return fnames, groups
-
-    def format(self,
-        namespace: dict[FormatterFname, Any],
-        predicate: Callable[[Any], bool] = bool,
-        sep: str = None,
-        substitute: str = None,
-        round_by_default: bool = True,
-    ) -> str:
-        '''Format a dict of numbers according to a format string by parsing
-        fields delineated by a separator `sep`.
-        Field groups which fail the `predicate` are not shown in the
-        final output string.
-        If specified, `substitute` will replace invalid fields instead.
-
-        :param namespace: A mapping with values to which fieldnames refer
-        :type namespace: :class:`dict[FormatterFname]`
-
-        :param predicate: A callable to determine whether a field should be
-            printed, defaults to :func:`bool`
-        :type predicate: :class:`Callable[[Any], bool]`
-
-        :param sep: Used to join field groups into the final string,
-            defaults to ``self.sep``
-        :type sep: :class:`str`
-
-        :param substitute: When set, replaces a field group that fails `predicate`
-        :type substitute: :class:`str`, optional
-
-        :param round_by_default: Round values if they are floats,
-            defaults to ``True``
-        :type round_by_default: :class:`bool`
-
-        :returns: A string with field groups hidden which don't pass `predicate`
-        :rtype: :class:`str`
+    def run(self, once: bool = None, stream: IO = None) -> None:
         '''
-        if sep is None:
-            sep = self.sep
-
-        newgroups = []
-        for i, group in enumerate(self.deconstructed):
-            if not group:
-                # Just an extraneous separator.
-                newgroups.append(())
-                continue
-
-            newgroup = []
-
-            for maybe_field in group:
-                # Handle sections that do not pass the predicate:
-                if not predicate(val := namespace[maybe_field[1]]):
-
-                    ##
-                    # Maybe check the length to see if a regular .format() can be used!
-                    ##
-
-                    if substitute is not None:
-                        newgroups.append(substitute)
-                    break
-
-                buf = ""
-
-                match maybe_field:
-                    case [lit, None, None, None]:
-                        # A trailing literal.
-                        # Only append if the previous field was valid:
-                        buf += lit
-
-                    case [lit, field, spec, conv]:
-                        # A veritable format string field!
-                        # Add the text right before the field:
-                        if lit is not None:
-                            buf += lit
-
-                        # Format the value if necessary:
-                        if spec:
-                            buf += format(val, spec)
-                        elif round_by_default and isinstance(val, float):
-                            buf += str(round(val))
-                        else:
-                            buf += str(val)
-
-                    case weird:
-                        raise ValueError(
-                            f"\n"
-                            f"Invalid structure in tuple\n"
-                            f"  {i} {maybe_field}:\n"
-                            f"  {weird!r}"
-                        )
-
-                if buf:
-                    newgroup.append(buf)
-            if newgroup:
-                newgroups.append(newgroup)
-
-        # Join everything.
-        return sep.join(''.join(g) for g in newgroups)
-
-
-
-Icon: TypeAlias = str
-from typing import NamedTuple
-# class Context(NamedTuple):
-    # value: str
-class Context(dict):
-    def __init__(
-        self,
-        *args,
-        value: str = None,
-    ) -> None: 
-        super().__init__(self)
-        self.value = value
-        # self.
-
-class IconFactory:
-    def __init__(
-        self,
-        func: Callable[[Context], Icon],
-        default: Icon = "",
-    ) -> None:
-        self.func = func
-        self.default = default
-
-    def interpret(self, ctx: Context = None, default: Icon = None) -> Icon:
-        if default is None:
-            default = self.default
-        if ctx is None:
-            return default
-        try:
-            return self.func(ctx)
-        except Exception:
-            return default
-
-
-# class Icon:
-# class IconMatcher(dict):
-# class IconDict(dict):
-class EasyIcon(dict):
-
-    def __init__(
-        self,
-        map: dict[Hashable, Icon] = {},
-        default: Icon = "",
-        # picker = None
-    ) -> None:
-        # self._registry = statemap
-        if statemap:
-            self.update(statemap)
-        self.default = default
-        # if callable(picker):
-            # self.picker = picker
-        # return self
-
-##    def __setitem__(self, state: Any, var: str) -> None:
-##        self._registry[id(state)] = var
-        # self[id(state)] = var
-
-##    def __getitem__(self, state: Any, ) -> str:
-##        return self._registry.get(state)
-    def choose(self, obj: Any):
-        return self.get(obj, self.default)
-
-    def interpret(self, key: Any):
-        return self.get(self.picker(key), self.default)
-
-
-    def __repr__(self) -> str:
-        # return self._registry[self._default]
-        stuff = ', '.join(' on '.join((repr(v), repr(k))) for k, v in self.items())
-        cls = type(self).__name__
-        return f"{cls}({stuff}, default={self.default!r})"
-
-    # def __str__(self) -> str:
-        # return self._registry[self._default]
-
-##cb = Callable[[Kwargs], State1|State2]
-##result, state = cb()
-##form = self.fmt.interpret(result, state)
-##form = self.format(result, state)
-
-
-class Format:
-    content_key: str = '$'
-    def __init__(
-        self,
-        # statemap: dict = {},
-        icon="",
-        default_fmt: str = "{icon}{"+content_key+'}',
-        fallback: str = "",
-        # custom_does_it_all: Callable[['result', 'context'], str] = None
-    ) -> None:
-        # self.statemap = statemap
-        self.icon = icon
-        self.default_fmt = default_fmt
-        self.fallback = fallback
-
-
-# class 
-class FormatSwitcher(dict):
-# class FormatSwitcher(Format):
-    content_key: str = '$'
-    def __init__(self,
-        statemap: dict['result', str] = {},
-        default: str = "{"+content_key+"}",
-        only_switch_icons: bool = True,
-        fallback: str = "",
-    ) -> None:
-        # self.statemap = statemap
-        self.icon = icon
-        self.default = default
-        self.fallback = fallback
-        self.update(statemap)
-
-    def format(self, result) -> str:
-        if isinstance(result, str):
-            return self.get(result, self.defaul)
-
-        icon, fmt = self.statemap.get(context, (self.icon, self.default_fmt))
-        contents = fmt.format_map({self.content_key: result, 'icon': icon})
-        return contents
+        Run the bar in the specified output stream.
+        Block until an exception is raised and exit smoothly.
 
+        :param stream: The IO stream in which to run the bar,
+            defaults to :attr:`Bar._stream`
+        :type stream: :class:`IO`
 
-class FormatMaker(Format):
-    def __init__(self,
-        fallback: str = "",
-        custom_does_it_all: Callable[['result'], str] = None
-    ) -> None:  
-        super().__init__(icon, default_fmt, fallback)
-
-        # if custom_does_it_all is None:
-            # custom_does_it_all = self._default_thingy
-
-    @staticmethod
-    def _default_thingy(fmt, result, context) -> str:
-        contents = fmt.format_map({content_key: result, 'icon': icon})
-        return
-
-    def format(self, result, context):
-        icon, fmt = self.statemap.get(context, (self.icon, self.default_fmt))
-        contents = fmt.format_map({self.content_key: result, 'icon': icon})
-        return contents
-
-def check_battery(ctx):
-    chrg_icn = ""
-    if ctx.get('charging'):
-        return chrg_icn + " "
-
-    icon_bank = """
-    
-    
-    
-    
-    
-    """.split()
-    def mapper(n):
-        icon = ""
-        for i, test in enumerate((10, 25, 50, 75, 100)):
-            if n <= test:
-                icon = icon_bank[i]
-                return icon + " "
-
-
-class ElapsedTime:
-    '''
-    Represent elapsed time in seconds with a variety of larger units.
-    '''
-    conversions_to_secs = {
-        'years': 12*4*7*24*60*60,
-        'months': 4*7*24*60*60,
-        'weeks': 7*24*60*60,
-        'days': 24*60*60,
-        'hours': 60*60,
-        'mins': 60,
-        'secs': 1,
-        'femtofortnights': 14*24*60*60 * 10**-15  # You can't see this.
-        }
+        :param once: Whether to print the bar only once, defaults to ``False``
+        :type once: :class:`bool`
 
-    @classmethod
-    def in_desired_units(cls,
-        secs: int,
-        units: tuple[Duration]
-    ) -> dict[Duration, int]:
+        :returns: ``None``
         '''
-        Convert seconds to multiple units of time.
+        if stream is not None:
+            self._stream = stream
+        if once is None:
+            once = self.run_once
 
-        The resulting value of the smallest unit in `units` is kept as
-        a :class:`float`.
-        Smaller units overflow into larger units when they meet or exceed
-        the threshold given by
-        :obj:`ElapsedTime.conversions_to_secs[larger_unit]`,
-        but only if a larger unit is present in `units`.
-
-        For example...
-
-            - Running ``in_desired_units(12345, ('mins', 'hours'))``
-                | yields ``{'hours': 3, 'mins': 25.75}``,
-            - but ``in_desired_units(12345, ('mins', 'days'))``
-                | yields ``{'days': 0, 'mins': 205.75}``,
-            - and ``in_desired_units(12345, ('hours',))``
-                | yields ``{'hours': 3.4291666666666667}``.
-
-        :param secs: Seconds to be converted
-        :type secs: :class:`int`
+        try:
+            self._can_run.set()
+            overriding = False
 
-        :param units: Units to convert
-        :type units: :class:`tuple[Duration]`
+            for field in self:
+                if field.overrides_refresh:
+                    overriding = True
+
+                if field.threaded:
+                    field.sync_send_to_thread(run_once=once)
+
+            if once:
+                for field in self:
+                    field.run()
+                # Wait for threads to finish:
+                while self._threads:
+                    time.sleep(self._thread_cooldown)
+                self._print_one_line()
 
-        :returns: A mapping of unit names to amount of time in those units
-        :rtype: :class:`dict[Duration, int]`
-        '''
-        if not all(u in cls.conversions_to_secs for u in units):
-            # At least one unit wasn't recognized. Raise an error:
-            valid = cls.conversions_to_secs._safe()
-            exptd = join_options(valid)
-            unrec = join_options(set(units) - set(valid))
-            exc = make_error_message(
-                LookupError,
-                blame=repr(units),
-                expected=f"a sequence of unit names from {exptd}",
-                details=[
-                    f"The following unit names are not recognized:",
-                    f"{unrec}",
-                ]
+            else:
+                if overriding:
+                    self._handle_overrides()
+                self._continuous_line_printer()
+
+        except KeyboardInterrupt:
+            pass
+
+        finally:
+            self._shutdown()
+
+
+    def _continuous_line_printer(self, end: str = '\r') -> None:
+        using_format_str = (self.fmt is not None)
+        sep = self.separator
+        running = self._can_run.is_set
+        clock = time.monotonic
+
+        if self.in_a_tty:
+            beginning = self.clearline_char + end
+            self._stream.write(CSI + HIDE_CURSOR)
+        else:
+            beginning = self.clearline_char
+
+        # fields = set(self._fields) - self._threads
+        fields = tuple(f for f in self if not f.threaded)
+        print(fields)
+
+        # Flushing the buffer before writing to it fixes poor i3bar alignment.
+        self._stream.flush()
+
+##        # Print something right away just so that the bar is not empty:
+##        self._print_one_line()
+
+        if self.align_to_seconds:
+            # Begin every refresh at the start of a clock second:
+            clock = time.time
+            time.sleep(1 - (clock() % 1))
+
+        start_time = clock()
+        for f in fields:
+            print(f._func)
+        while running():
+            self._buffers.update((f.name, f.run()) for f in fields)
+                
+            if using_format_str:
+                line = self.fmt.format_map(self._buffers)
+            else:
+                line = sep.join(
+                    buf for field in fields
+                        if (buf := self._buffers[field.name])
+                        or self.join_empty_fields
+                )
+
+            self._stream.write(beginning + line + end)
+            self._stream.flush()
+
+            # Sleep only until the next possible refresh to keep the
+            # refresh cycle length consistent and prevent drifting.
+            time.sleep(
+                # Time until next refresh:
+                self.refresh_rate - (
+                    # Get the current latency, which can vary:
+                    (clock() - start_time) % self.refresh_rate  # Preserve offset
+                )
             )
-            raise exc
 
-        # Get the units in order of largest first:
-        ordered = tuple(u for u in cls.conversions_to_secs if u in units)
-
-        table = {}
-        if len(ordered) == 1:
-            unit = ordered[0]
-            # Avoid robbing the only unit of its precision. Just divide:
-            table[unit] = secs / cls.conversions_to_secs[unit]
-            return table
-
-        for unit in ordered[:-1]:
-            table[unit], secs = divmod(secs, cls.conversions_to_secs[unit])
-        # Give the least significant unit a precise value:
-        last_u = ordered[-1]
-        table[last_u] = secs / cls.conversions_to_secs[last_u]
-        return table
-
-    class _Special_Obfuscating_Dict(dict):
-        def _safe(self) -> Self:
-            meme_hidden = self.copy()
-            meme_hidden.pop('femtofortnights')  # Shhh, it's a secret.
-            return meme_hidden
+        if self.in_a_tty:
+            self._stream.write('\n')
+            self._stream.write(CSI + UNHIDE_CURSOR)
+
+    def line_generator(self):
+        using_format_str = (self.fmt is not None)
+        sep = self.separator
+        running = self._can_run.is_set
+
+        while running():
+            if using_format_str:
+                line = self.fmt.format_map(self._buffers)
+            else:
+                line = sep.join(
+                    buf for field in self._field_order
+                        if (buf := self._buffers[field])
+                        or self.join_empty_fields
+                )
+            yield line
 
-        def __repr__(self) -> str:
-            return repr(self._safe())
 
-    conversions_to_secs = _Special_Obfuscating_Dict(conversions_to_secs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mybar-0.6/mybar/utils.py` & `mybar-0.7/mybar/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 '''Utility functions'''
 
 #TODO Examples!
 
 from copy import deepcopy
 
-from ._types import FmtStrStructure, FormatStr, FormatterFname 
-
 from collections.abc import Callable, Iterable
 from typing import Any
 
 
 def join_options(
     it: Iterable[object],
     /,
@@ -69,16 +67,18 @@
     elif oxford:
         opts[-1] = metasep.join((final_sep, opts[-1]))
     else:
         opts[-1] = metasep.join((opts.pop(-2), final_sep, opts[-1]))
     return sep.join(opts)
 
 
-def str_to_bool(value: str, /) -> bool:
+def str_to_bool(value: str | bool, /) -> bool:
     '''Returns `True` or `False` bools for truthy or falsy strings.'''
+    if isinstance(value, bool):
+        return value
     truthy = "true t yes y on 1".split()
     falsy = "false f no n off 0".split()
     pattern = value.lower()
     if pattern not in truthy + falsy:
         raise ValueError(f"Invalid argument: {value!r}")
     return (pattern in truthy or not pattern in falsy)
```

### Comparing `mybar-0.6/mybar.egg-info/PKG-INFO` & `mybar-0.7/mybar.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.6
+Version: 0.7
 Summary: An async status bar with a highly customizable API.
 Home-page: https://github.com/lonelyabsol/mybar
 Author: lonelyabsol
 License: MIT
 Project-URL: GitHub: repo, https://github.com/lonelyabsol/mybar
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mybar-0.6/setup.cfg` & `mybar-0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mybar
-version = 0.6
+version = 0.7
 description = An async status bar with a highly customizable API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = lonelyabsol
 url = https://github.com/lonelyabsol/mybar
 project_urls = 
 	GitHub: repo = https://github.com/lonelyabsol/mybar
```

