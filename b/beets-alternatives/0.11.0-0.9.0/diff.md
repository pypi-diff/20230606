# Comparing `tmp/beets_alternatives-0.11.0.tar.gz` & `tmp/beets-alternatives-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beets_alternatives-0.11.0.tar", max compression
+gzip compressed data, was "dist/beets-alternatives-0.9.0.tar", last modified: Sat Nov 24 10:06:01 2018, max compression
```

## Comparing `beets_alternatives-0.11.0.tar` & `beets-alternatives-0.9.0.tar`

### file list

```diff
@@ -1,7 +1,16 @@
--rw-r--r--   0        0        0     1700 2023-06-06 09:52:08.856413 beets_alternatives-0.11.0/CHANGELOG.md
--rw-r--r--   0        0        0     1060 2015-02-01 16:31:58.782244 beets_alternatives-0.11.0/LICENSE
--rw-r--r--   0        0        0    11187 2023-05-02 09:05:47.655265 beets_alternatives-0.11.0/README.md
--rw-r--r--   0        0        0       76 2023-05-02 09:05:47.658598 beets_alternatives-0.11.0/beetsplug/__init__.py
--rw-r--r--   0        0        0    15780 2023-06-06 09:52:08.853079 beets_alternatives-0.11.0/beetsplug/alternatives.py
--rw-r--r--   0        0        0     1145 2023-06-06 09:52:08.856413 beets_alternatives-0.11.0/pyproject.toml
--rw-r--r--   0        0        0    12107 1970-01-01 00:00:00.000000 beets_alternatives-0.11.0/PKG-INFO
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2018-11-24 10:06:01.000000 beets-alternatives-0.9.0/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1060 2015-02-01 16:31:58.000000 beets-alternatives-0.9.0/LICENSE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       26 2015-02-01 16:31:58.000000 beets-alternatives-0.9.0/MANIFEST.in
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    12818 2018-11-24 10:06:01.000000 beets-alternatives-0.9.0/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     9829 2018-11-24 10:04:50.000000 beets-alternatives-0.9.0/README.md
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2018-11-24 10:06:01.000000 beets-alternatives-0.9.0/beets_alternatives.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    12818 2018-11-24 10:06:01.000000 beets-alternatives-0.9.0/beets_alternatives.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      305 2018-11-24 10:06:01.000000 beets-alternatives-0.9.0/beets_alternatives.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2018-11-24 10:06:01.000000 beets-alternatives-0.9.0/beets_alternatives.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       50 2018-11-24 10:06:01.000000 beets-alternatives-0.9.0/beets_alternatives.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       10 2018-11-24 10:06:01.000000 beets-alternatives-0.9.0/beets_alternatives.egg-info/top_level.txt
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2018-11-24 10:06:01.000000 beets-alternatives-0.9.0/beetsplug/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       75 2015-02-01 16:31:58.000000 beets-alternatives-0.9.0/beetsplug/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    12354 2018-11-24 10:04:48.000000 beets-alternatives-0.9.0/beetsplug/alternatives.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      206 2018-11-24 10:06:01.000000 beets-alternatives-0.9.0/setup.cfg
+-rwxr-xr-x   0 thomas    (1000) thomas    (1000)     1146 2018-11-24 10:04:50.000000 beets-alternatives-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `beets_alternatives-0.11.0/LICENSE` & `beets-alternatives-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beets_alternatives-0.11.0/README.md` & `beets-alternatives-0.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 beets-alternatives
 ==================
 
-[![Check and test](https://github.com/geigerzaehler/beets-alternatives/actions/workflows/main.yaml/badge.svg)](https://github.com/geigerzaehler/beets-alternatives/actions/workflows/main.yaml)
-[![Coverage Status](https://coveralls.io/repos/github/geigerzaehler/beets-alternatives/badge.svg?branch=master)](https://coveralls.io/github/geigerzaehler/beets-alternatives?branch=master)
+[![Build Status](https://travis-ci.org/geigerzaehler/beets-alternatives.svg?branch=master)](https://travis-ci.org/geigerzaehler/beets-alternatives)
+[![Coverage Status](https://coveralls.io/repos/geigerzaehler/beets-alternatives/badge.png?branch=master)](https://coveralls.io/r/geigerzaehler/beets-alternatives?branch=master)
 
 You want to manage multiple versions of your audio files with beets?
 Your favorite iPlayer has limited space and does not support Ogg Vorbis? You
 want to keep lossless versions on a large external drive? You want to
 symlink your audio to other locations?
 
 With this [beets][beets-docs] plugin every file in you music library have
 multiple alternate versions in separate locations.
 
-If you’re interested in contributing to this project, check out the [developer
-documentation](./DEVELOPING.md).
-
 Getting Started
 ---------------
 
-Install the plugin and make sure you using at least version 1.6.0 of beets and
-Python 3.8.
+You will also need at least version 1.4.7 of beets.
 
-```bash
-pip install --upgrade beets>=1.6.0 beets-alternatives
+```
+pip install --upgrade beets>=1.4.7 beets-alternatives
 ```
 
 Then, [enable the plugin][using plugins]. You may use the `beet config --edit`
 command to add the *alternatives* plugin to the configuration.
 
 ```yaml
 plugins:
@@ -65,60 +61,61 @@
 selection transparent.
 
 Let’s add some files to our selection by setting the flexible attribute
 from the `query` option. (Since we use boolean values for the
 ‘onplayer’ field it might be a good idea to set the type of this field
 to `bool` using the *types* plugin)
 
-```bash
-beet modify onplayer=true artist:Bach
+```
+$ beet modify onplayer=true artist:Bach
 ```
 
 The configured query also matches all tracks that are part of an album
 where the `onplayer` attribute is ‘true’. We could also use
 
-```bash
-beet modify -a onplayer=true albumartist:Bach
+```
+$ beet modify -a onplayer=true albumartist:Bach
 ```
 
 We then tell beets to create the external files.
 
 ```
 $ beet alt update myplayer
 Collection at '/player' does not exists. Maybe you forgot to mount it.
 Do you want to create the collection? (y/N)
 ```
 
 The question makes sure that you don’t recreate a external collection
 if the device is not mounted. Since this is our first go, we answer the
 question with yes.
 
-The command will copy all files with the artist ‘Bach’ and format either ‘AAC’
-or ‘MP3’ to the `/player` directory. All other formats will be transcodec to the
-‘AAC’ format unsing the [*convert* plugin][convert plugin]. The transcoding
-process can be configured through [*convert’s* configuration][convert config].
+The command will copy all files with the artist ‘Bach’ and format
+either ‘AAC’ or ‘MP3’ to the `/player` directory. All other formats
+will be transcodec to the ‘AAC’ format unsing the [*convert* plugin][].
+The transcoding process can be configured through [*convert’s*
+configuration][convert config].
 
 If you update some tracks in your main collection, the `alt update`
 command will propagate the changes to your external collection.  Since
 we don’t need to convert the files but just update the tags, this will
 be much faster the second time.
 
-```bash
-beet modify composer="Johann Sebastian Bach" artist:Bach
-beet alt update myplayer
+```
+$ beet modify composer="Johann Sebastian Bach" artist:Bach
+$ beet alt update myplayer
 ```
 
 After going for a run you mitght realize that Bach is probably not the
 right thing to work out to. So you decide to put Beethoven on your
 player.
 
-```bash
-beet modify onplayer! artist:Bach
-beet modify onplayer=true artist:Beethoven
-beet alt update myplayer
+```
+$ beet modify onplayer! artist:Bach
+$ beet modify onplayer=true artist:Beethoven
+$ beet alt update myplayer
 ```
 
 This removes all Bach tracks from the player and adds Beethoven’s.
 
 ### Symlink Views
 
 Instead of copying and converting files this plugin can also create
@@ -146,46 +143,24 @@
 to the collection’s name. Finally, we omitted the `query` option. This
 means that we want to create symlinks for all files. Of course you can
 still add a query to select only parts of your collection.
 
 The `beet alt update by-year` command will now create the symlinks. For
 example
 
-```plain
-/music/by-year/1982/Thriller/Beat It.mp3
--> /music/Michael Jackson/Thriller/Beat It.mp3
 ```
-
-You can also specify if you want absolute symlinks (default) or relative ones
-with `link_type`. The option `link_type` must be `absolute` or `relative`
-
-```yaml
-alternatives:
-  by-year:
-    directory: by-year
-    paths:
-      default: $year/$album/$title
-    formats: link
-    link_type: relative
-```
-
-With this config, the `beet alt update by-year` command will create relative symlinks. E.g:
-
-```plain
 /music/by-year/1982/Thriller/Beat It.mp3
--> ../../../Michael Jackson/Thriller/Beat It.mp3
+-> /music/Michael Jackson/Thriller/Beat It.mp3
 ```
 
-Now, if you move the `/music/` folder to another location, the links
-will continue working
 
 CLI Reference
 -------------
 
-```plain
+```
 beet alt update [--create|--no-create] NAME
 ```
 
 Updates the external collection configured under `alternatives.NAME`.
 
 * Add missing files. Convert them to the configured format or copy
   them.
@@ -201,25 +176,14 @@
 The command accepts the following option.
 
 * **`--[no-]create`** If the `removable` configuration option
   is set and the external base directory does not exist, then the
   command will ask you to confirm the creation of the external
   collection. These options specify the answer as a cli option.
 
-```
-beet alt list-tracks [--format=FORMAT] NAME
-```
-
-Lists all tracks that are currently included in the collection.
-
-The `--format` option accepts a [beets path format][path-format] string that is
-used to format each track.
-
-[path-format]: https://beets.readthedocs.io/en/latest/reference/pathformat.html
-
 Configuration
 -------------
 
 An external collection is configured as a name-settings-pair under the
 `alternatives` configuration. The name is used to reference the
 collection from the command line. The settings is a map of the
 following settings.
@@ -242,27 +206,23 @@
   audio file formats in the external collection. If the ‘format’ field
   of a track is included in the list, the file is copied. Otherwise,
   the file is transcoded to the first format in the list. The name of
   the first format must correpond to a key in the
   [`convert.formats`][convert plugin] configuration. This configuration
   controls the transcoding process.
 
-  The special format ‘link’ is used to create symbolic links instead of
+  The special format ‘link’ is used to create symbolik links instead of
   transcoding the file. It can not be combined with other formats.
 
   By default no transcoding is done.
 
 * **`removable`** If this is `true` (the default) and `directory` does
   not exist, the `update` command will ask you to confirm the creation
   of the external collection. (optional)
 
-* **`link_type`** Can be `absolute` (default) or `relative`. If
-  **`formats`** is `link`, it sets the type of links to create. For
-  differences between link types and examples see [Symlink Views](#symlink-views).
-
 
 Feature Requests
 ----------------
 
 If you have an idea or a use case this plugin is missing, feel free to
 [open an issue](https://github.com/geigerzaehler/beets-alternatives/issues/new).
 
@@ -271,15 +231,15 @@
 * Symbolic links for each artist in a multiple artists release (see the
   [beets issue][beets-issue-split-symlinks])
 
 
 License
 -------
 
-Copyright (c) 2014-2023 Thomas Scholtes.
+Copyright (c) 2014 Thomas Scholtes.
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `beets_alternatives-0.11.0/beetsplug/alternatives.py` & `beets-alternatives-0.9.0/beetsplug/alternatives.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,223 +1,149 @@
 # Copyright (c) 2014 Thomas Scholtes
-# -*- coding: utf-8 -*-
 
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"), to
 # deal in the Software without restriction, including without limitation the
 # rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 # sell copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in
 # all copies or substantial portions of the Software.
 
 
-import argparse
 import os.path
 import threading
-import traceback
+from argparse import ArgumentParser
 from concurrent import futures
+import six
 
 import beets
-import six
-from beets import art, util
-from beets.library import Item, parse_query_string
+from beets import util, art
 from beets.plugins import BeetsPlugin
-from beets.ui import Subcommand, UserError, decargs, get_path_formats, input_yn, print_
-from beets.util import FilesystemError, bytestring_path, displayable_path, syspath
+from beets.ui import Subcommand, get_path_formats, input_yn, UserError, print_
+from beets.library import parse_query_string, Item
+from beets.util import syspath, displayable_path, cpu_count, bytestring_path
 
 from beetsplug import convert
 
 
-def _remove(path, soft=True):
-    """Remove the file. If `soft`, then no error will be raised if the
-    file does not exist.
-    In contrast to beets' util.remove, this uses lexists such that it can
-    actually remove symlink links.
-    """
-    path = syspath(path)
-    if soft and not os.path.lexists(path):
-        return
-    try:
-        os.remove(path)
-    except (OSError, IOError) as exc:
-        raise FilesystemError(exc, "delete", (path,), traceback.format_exc())
-
-
 class AlternativesPlugin(BeetsPlugin):
+
     def __init__(self):
         super(AlternativesPlugin, self).__init__()
 
     def commands(self):
         return [AlternativesCommand(self)]
 
     def update(self, lib, options):
         try:
             alt = self.alternative(options.name, lib)
         except KeyError as e:
-            raise UserError("Alternative collection '{0}' not found.".format(e.args[0]))
+            raise UserError(u"Alternative collection '{0}' not found."
+                            .format(e.args[0]))
         alt.update(create=options.create)
 
-    def list_tracks(self, lib, options):
-        if options.format is not None:
-            (fmt,) = decargs([options.format])
-            beets.config[beets.library.Item._format_config_key].set(fmt)
-
-        alt = self.alternative(options.name, lib)
-
-        # This is slow but we cannot use a native SQL query since the
-        # path key is a flexible attribute
-        for item in lib.items():
-            if alt.path_key in item:
-                print_(format(item))
-
     def alternative(self, name, lib):
         conf = self.config[name]
         if not conf.exists():
             raise KeyError(name)
 
-        if conf["formats"].exists():
-            fmt = conf["formats"].as_str()
-            if fmt == "link":
+        if conf['formats'].exists():
+            fmt = conf['formats'].as_str()
+            if fmt == u'link':
                 return SymlinkView(self._log, name, lib, conf)
             else:
                 return ExternalConvert(self._log, name, fmt.split(), lib, conf)
         else:
             return External(self._log, name, lib, conf)
 
 
 class AlternativesCommand(Subcommand):
-    name = "alt"
-    help = "manage alternative files"
+
+    name = 'alt'
+    help = 'manage alternative files'
 
     def __init__(self, plugin):
         parser = ArgumentParser()
-        subparsers = parser.add_subparsers(prog=parser.prog + " alt")
-        subparsers.required = True
-
-        update = subparsers.add_parser("update")
+        subparsers = parser.add_subparsers()
+        update = subparsers.add_parser('update')
         update.set_defaults(func=plugin.update)
-        update.add_argument("name", metavar="NAME")
-        update.add_argument("--create", action="store_const", dest="create", const=True)
-        update.add_argument(
-            "--no-create", action="store_const", dest="create", const=False
-        )
-
-        list_tracks = subparsers.add_parser(
-            "list-tracks",
-            description="""
-                List all tracks that are currently part of an alternative
-                collection""",
-        )
-        list_tracks.set_defaults(func=plugin.list_tracks)
-        list_tracks.add_argument(
-            "name",
-            metavar="NAME",
-            help="Name of the alternative",
-        )
-        list_tracks.add_argument(
-            "-f",
-            "--format",
-            metavar="FORMAT",
-            dest="format",
-            help="""Format string to print for each track. See beets’
-                Path Formats for more information.""",
-        )
-
+        update.add_argument('name')
+        update.add_argument('--create', action='store_const',
+                            dest='create', const=True)
+        update.add_argument('--no-create', action='store_const',
+                            dest='create', const=False)
         super(AlternativesCommand, self).__init__(self.name, parser, self.help)
 
     def func(self, lib, opts, _):
         opts.func(lib, opts)
 
     def parse_args(self, args):
         return self.parser.parse_args(args), []
 
 
-class ArgumentParser(argparse.ArgumentParser):
-    """
-    Facade for ``argparse.ArgumentParser`` so that beets can call
-    `_get_all_options()` to generate shell completion.
-    """
-
-    def _get_all_options(self):
-        # FIXME return options like ``OptionParser._get_all_options``.
-        return []
-
-
 class External(object):
+
     ADD = 1
     REMOVE = 2
     WRITE = 3
     MOVE = 4
     SYNC_ART = 5
 
     def __init__(self, log, name, lib, config):
         self._log = log
         self.name = name
         self.lib = lib
-        self.path_key = "alt.{0}".format(name)
-        self.max_workers = int(str(beets.config["convert"]["threads"]))
+        self.path_key = u'alt.{0}'.format(name)
         self.parse_config(config)
 
     def parse_config(self, config):
-        if "paths" in config:
-            path_config = config["paths"]
+        if 'paths' in config:
+            path_config = config['paths']
         else:
-            path_config = beets.config["paths"]
+            path_config = beets.config['paths']
         self.path_formats = get_path_formats(path_config)
-        query = config["query"].as_str()
+        query = config['query'].as_str()
         self.query, _ = parse_query_string(query, Item)
 
-        self.removable = config.get(dict).get("removable", True)
+        self.removable = config.get(dict).get('removable', True)
 
-        if "directory" in config:
-            dir = config["directory"].as_str()
+        if 'directory' in config:
+            dir = config['directory'].as_str()
         else:
             dir = self.name
         dir = bytestring_path(dir)
         if not os.path.isabs(syspath(dir)):
             dir = os.path.join(self.lib.directory, dir)
         self.directory = dir
 
-    def item_change_actions(self, item, path, dest):
-        """Returns the necessary actions for items that were previously in the
-        external collection, but might require metadata updates.
-        """
-        actions = []
-
-        if not util.samefile(path, dest):
-            actions.append(self.MOVE)
-
-        item_mtime_alt = os.path.getmtime(syspath(path))
-        if item_mtime_alt < os.path.getmtime(syspath(item.path)):
-            actions.append(self.WRITE)
-        album = item.get_album()
-
-        if album:
-            if (
-                album.artpath
-                and os.path.isfile(syspath(album.artpath))
-                and (item_mtime_alt < os.path.getmtime(syspath(album.artpath)))
-            ):
-                actions.append(self.SYNC_ART)
-
-        return actions
-
     def matched_item_action(self, item):
         path = self.get_path(item)
-        if path and os.path.lexists(syspath(path)):
+        if path and os.path.isfile(syspath(path)):
             dest = self.destination(item)
             _, path_ext = os.path.splitext(path)
             _, dest_ext = os.path.splitext(dest)
             if not path_ext == dest_ext:
                 # formats config option changed
                 return (item, [self.REMOVE, self.ADD])
-            else:
-                return (item, self.item_change_actions(item, path, dest))
+            actions = []
+            if not util.samefile(path, dest):
+                actions.append(self.MOVE)
+            item_mtime_alt = os.path.getmtime(syspath(path))
+            if (item_mtime_alt < os.path.getmtime(syspath(item.path))):
+                actions.append(self.WRITE)
+            album = item.get_album()
+            if album:
+                if (album.artpath and
+                        os.path.isfile(syspath(album.artpath)) and
+                        (item_mtime_alt
+                         < os.path.getmtime(syspath(album.artpath)))):
+                    actions.append(self.SYNC_ART)
+            return (item, actions)
         else:
             return (item, [self.ADD])
 
     def items_actions(self):
         matched_ids = set()
         for album in self.lib.albums():
             if self.query.match(album):
@@ -232,114 +158,111 @@
 
     def ask_create(self, create=None):
         if not self.removable:
             return True
         if create is not None:
             return create
 
-        msg = (
-            "Collection at '{0}' does not exists. "
-            "Maybe you forgot to mount it.\n"
-            "Do you want to create the collection? (y/n)".format(
-                displayable_path(self.directory)
-            )
-        )
+        msg = u"Collection at '{0}' does not exists. " \
+              "Maybe you forgot to mount it.\n" \
+              "Do you want to create the collection? (y/n)" \
+              .format(displayable_path(self.directory))
         return input_yn(msg, require=True)
 
     def update(self, create=None):
-        if not os.path.isdir(syspath(self.directory)) and not self.ask_create(create):
-            print_("Skipping creation of {0}".format(displayable_path(self.directory)))
+        if (not os.path.isdir(syspath(self.directory))
+                and not self.ask_create(create)):
+            print_(u'Skipping creation of {0}'
+                   .format(displayable_path(self.directory)))
             return
 
         converter = self.converter()
-        for item, actions in self.items_actions():
+        for (item, actions) in self.items_actions():
             dest = self.destination(item)
             path = self.get_path(item)
             for action in actions:
                 if action == self.MOVE:
-                    print_(
-                        ">{0} -> {1}".format(
-                            displayable_path(path), displayable_path(dest)
-                        )
-                    )
+                    print_(u'>{0} -> {1}'.format(displayable_path(path),
+                                                 displayable_path(dest)))
                     util.mkdirall(dest)
                     util.move(path, dest)
                     util.prune_dirs(os.path.dirname(path), root=self.directory)
                     self.set_path(item, dest)
                     item.store()
                     path = dest
                 elif action == self.WRITE:
-                    print_("*{0}".format(displayable_path(path)))
+                    print_(u'*{0}'.format(displayable_path(path)))
                     item.write(path=path)
                 elif action == self.SYNC_ART:
-                    print_("~{0}".format(displayable_path(path)))
+                    print_(u'~{0}'.format(displayable_path(path)))
                     self.sync_art(item, path)
                 elif action == self.ADD:
-                    print_("+{0}".format(displayable_path(dest)))
+                    print_(u'+{0}'.format(displayable_path(dest)))
                     converter.submit(item)
                 elif action == self.REMOVE:
-                    print_("-{0}".format(displayable_path(path)))
+                    print_(u'-{0}'.format(displayable_path(path)))
                     self.remove_item(item)
                     item.store()
 
         for item, dest in converter.as_completed():
             self.set_path(item, dest)
             item.store()
         converter.shutdown()
 
     def destination(self, item):
-        return item.destination(basedir=self.directory, path_formats=self.path_formats)
+        return item.destination(basedir=self.directory,
+                                path_formats=self.path_formats)
 
     def set_path(self, item, path):
-        item[self.path_key] = six.text_type(path, "utf8")
+        item[self.path_key] = six.text_type(path, 'utf8')
 
     @staticmethod
     def _get_path(item, path_key):
         try:
-            return item[path_key].encode("utf8")
+            return item[path_key].encode('utf8')
         except KeyError:
             return None
 
     def get_path(self, item):
         return self._get_path(item, self.path_key)
 
     def remove_item(self, item):
         path = self.get_path(item)
-        _remove(path)
+        util.remove(path)
         util.prune_dirs(path, root=self.directory)
         del item[self.path_key]
 
     def converter(self):
         def _convert(item):
             dest = self.destination(item)
             util.mkdirall(dest)
             util.copy(item.path, dest, replace=True)
             return item, dest
-
-        return Worker(_convert, self.max_workers)
+        return Worker(_convert)
 
     def sync_art(self, item, path):
-        """Embed artwork in the destination file."""
+        """ Embed artwork in the destination file.
+        """
         album = item.get_album()
         if album:
             if album.artpath and os.path.isfile(syspath(album.artpath)):
-                self._log.debug(
-                    "Embedding art from {} into {}".format(
-                        displayable_path(album.artpath), displayable_path(path)
-                    )
-                )
-                art.embed_item(self._log, item, album.artpath, itempath=path)
+                self._log.debug("Embedding art from {} into {}".format(
+                                displayable_path(album.artpath),
+                                displayable_path(path)))
+                art.embed_item(self._log, item, album.artpath,
+                               itempath=path)
 
 
 class ExternalConvert(External):
+
     def __init__(self, log, name, formats, lib, config):
         super(ExternalConvert, self).__init__(log, name, lib, config)
         convert_plugin = convert.ConvertPlugin()
         self._encode = convert_plugin.encode
-        self._embed = convert_plugin.config["embed"].get(bool)
+        self._embed = convert_plugin.config['embed'].get(bool)
         formats = [f.lower() for f in formats]
         self.formats = [convert.ALIASES.get(f, f) for f in formats]
         self.convert_cmd, self.ext = convert.get_format(self.formats[0])
 
     def converter(self):
         fs_lock = threading.Lock()
 
@@ -349,108 +272,71 @@
                 util.mkdirall(dest)
 
             if self.should_transcode(item):
                 self._encode(self.convert_cmd, item.path, dest)
                 # Don't rely on the converter to write correct/complete tags.
                 item.write(path=dest)
             else:
-                self._log.debug("copying {0}".format(displayable_path(dest)))
+                self._log.debug(u'copying {0}'.format(displayable_path(dest)))
                 util.copy(item.path, dest, replace=True)
             if self._embed:
                 self.sync_art(item, dest)
             return item, dest
-
-        return Worker(_convert, self.max_workers)
+        return Worker(_convert)
 
     def destination(self, item):
         dest = super(ExternalConvert, self).destination(item)
         if self.should_transcode(item):
-            return os.path.splitext(dest)[0] + b"." + self.ext
+            return os.path.splitext(dest)[0] + b'.' + self.ext
         else:
             return dest
 
     def should_transcode(self, item):
         return item.format.lower() not in self.formats
 
 
 class SymlinkView(External):
-    LINK_ABSOLUTE = 0
-    LINK_RELATIVE = 1
 
     def parse_config(self, config):
-        if "query" not in config:
-            config["query"] = ""  # This is a TrueQuery()
-        if "link_type" not in config:
-            # Default as absolute so it doesn't break previous implementation
-            config["link_type"] = "absolute"
-
-        self.relativelinks = config["link_type"].as_choice(
-            {"relative": self.LINK_RELATIVE, "absolute": self.LINK_ABSOLUTE}
-        )
-
+        if 'query' not in config:
+            config['query'] = u''  # This is a TrueQuery()
         super(SymlinkView, self).parse_config(config)
 
-    def item_change_actions(self, item, path, dest):
-        """Returns the necessary actions for items that were previously in the
-        external collection, but might require metadata updates.
-        """
-        actions = []
-
-        if not path == dest:
-            # The path of the link itself changed
-            actions.append(self.MOVE)
-        elif not util.samefile(path, item.path):
-            # link target changed
-            actions.append(self.MOVE)
-
-        return actions
-
     def update(self, create=None):
-        for item, actions in self.items_actions():
+        for (item, actions) in self.items_actions():
             dest = self.destination(item)
             path = self.get_path(item)
             for action in actions:
                 if action == self.MOVE:
-                    print_(
-                        ">{0} -> {1}".format(
-                            displayable_path(path), displayable_path(dest)
-                        )
-                    )
+                    print_(u'>{0} -> {1}'.format(displayable_path(path),
+                                                 displayable_path(dest)))
                     self.remove_item(item)
                     self.create_symlink(item)
                     self.set_path(item, dest)
                 elif action == self.ADD:
-                    print_("+{0}".format(displayable_path(dest)))
+                    print_(u'+{0}'.format(displayable_path(dest)))
                     self.create_symlink(item)
                     self.set_path(item, dest)
                 elif action == self.REMOVE:
-                    print_("-{0}".format(displayable_path(path)))
+                    print_(u'-{0}'.format(displayable_path(path)))
                     self.remove_item(item)
                 else:
                     continue
                 item.store()
 
     def create_symlink(self, item):
         dest = self.destination(item)
         util.mkdirall(dest)
-        link = (
-            os.path.relpath(item.path, os.path.dirname(dest))
-            if self.relativelinks == self.LINK_RELATIVE
-            else item.path
-        )
-        util.link(link, dest)
-
-    def sync_art(self, item, path):
-        # FIXME: symlink art
-        pass
+        util.link(item.path, dest)
 
 
 class Worker(futures.ThreadPoolExecutor):
-    def __init__(self, fn, max_workers):
-        super(Worker, self).__init__(max_workers)
+
+    def __init__(self, fn, max_workers=None):
+        super(Worker, self).__init__(max_workers or cpu_count())
         self._tasks = set()
         self._fn = fn
 
     def submit(self, *args, **kwargs):
         fut = super(Worker, self).submit(self._fn, *args, **kwargs)
         self._tasks.add(fut)
         return fut
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `beets_alternatives-0.11.0/PKG-INFO` & `beets-alternatives-0.9.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,330 +1,288 @@
 Metadata-Version: 2.1
 Name: beets-alternatives
-Version: 0.11.0
+Version: 0.9.0
 Summary: beets plugin to manage multiple files
 Home-page: http://www.github.com/geigerzaehler/beets-alternatives
-License: MIT
 Author: Thomas Scholtes
-Author-email: geigerzaehler@axiom.fm
-Requires-Python: >=3.8.1,<4.0.0
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Author-email: thomas-scholtes@gmx.de
+License: MIT
+Description: beets-alternatives
+        ==================
+        
+        [![Build Status](https://travis-ci.org/geigerzaehler/beets-alternatives.svg?branch=master)](https://travis-ci.org/geigerzaehler/beets-alternatives)
+        [![Coverage Status](https://coveralls.io/repos/geigerzaehler/beets-alternatives/badge.png?branch=master)](https://coveralls.io/r/geigerzaehler/beets-alternatives?branch=master)
+        
+        You want to manage multiple versions of your audio files with beets?
+        Your favorite iPlayer has limited space and does not support Ogg Vorbis? You
+        want to keep lossless versions on a large external drive? You want to
+        symlink your audio to other locations?
+        
+        With this [beets][beets-docs] plugin every file in you music library have
+        multiple alternate versions in separate locations.
+        
+        Getting Started
+        ---------------
+        
+        You will also need at least version 1.4.7 of beets.
+        
+        ```
+        pip install --upgrade beets>=1.4.7 beets-alternatives
+        ```
+        
+        Then, [enable the plugin][using plugins]. You may use the `beet config --edit`
+        command to add the *alternatives* plugin to the configuration.
+        
+        ```yaml
+        plugins:
+        - ...
+        - alternatives
+        ```
+        
+        Now, you can get rolling with one of the use cases below.
+        
+        ### External Files
+        
+        Suppose your favorite portable player only supports MP3 and MP4, has
+        limited disk space and is mounted at `/player`. Instead of selecting
+        its content manually and using the `convert` plugin to transcode it, you
+        want to sync it automatically. First we give this external collection
+        the name ‘myplayer’ and start configuring beets.
+        
+        ```yaml
+        alternatives:
+          myplayer:
+            directory: /player
+            paths:
+              default: $album/$title
+            formats: aac mp3
+            query: "onplayer:true"
+            removable: true
+        ```
+        
+        The first two options determine the location of the external files and
+        correspond to the global [`directory`][config-directory] and
+        [`paths`][config-paths] settings.  The `format` option specifies the
+        formats we transcode the files to (more on that below).  Finally, the
+        `query` option tells the plugin which files you want to put in the
+        external location. The value is a [query string][] as used for the
+        beets command line. In our case we use a flexible attribute to make the
+        selection transparent.
+        
+        Let’s add some files to our selection by setting the flexible attribute
+        from the `query` option. (Since we use boolean values for the
+        ‘onplayer’ field it might be a good idea to set the type of this field
+        to `bool` using the *types* plugin)
+        
+        ```
+        $ beet modify onplayer=true artist:Bach
+        ```
+        
+        The configured query also matches all tracks that are part of an album
+        where the `onplayer` attribute is ‘true’. We could also use
+        
+        ```
+        $ beet modify -a onplayer=true albumartist:Bach
+        ```
+        
+        We then tell beets to create the external files.
+        
+        ```
+        $ beet alt update myplayer
+        Collection at '/player' does not exists. Maybe you forgot to mount it.
+        Do you want to create the collection? (y/N)
+        ```
+        
+        The question makes sure that you don’t recreate a external collection
+        if the device is not mounted. Since this is our first go, we answer the
+        question with yes.
+        
+        The command will copy all files with the artist ‘Bach’ and format
+        either ‘AAC’ or ‘MP3’ to the `/player` directory. All other formats
+        will be transcodec to the ‘AAC’ format unsing the [*convert* plugin][].
+        The transcoding process can be configured through [*convert’s*
+        configuration][convert config].
+        
+        If you update some tracks in your main collection, the `alt update`
+        command will propagate the changes to your external collection.  Since
+        we don’t need to convert the files but just update the tags, this will
+        be much faster the second time.
+        
+        ```
+        $ beet modify composer="Johann Sebastian Bach" artist:Bach
+        $ beet alt update myplayer
+        ```
+        
+        After going for a run you mitght realize that Bach is probably not the
+        right thing to work out to. So you decide to put Beethoven on your
+        player.
+        
+        ```
+        $ beet modify onplayer! artist:Bach
+        $ beet modify onplayer=true artist:Beethoven
+        $ beet alt update myplayer
+        ```
+        
+        This removes all Bach tracks from the player and adds Beethoven’s.
+        
+        ### Symlink Views
+        
+        Instead of copying and converting files this plugin can also create
+        symbolic links to the files in your library. For example you want to
+        have a directory containing all music sorted by year and album.
+        
+        ```yaml
+        directory: /music
+        paths:
+          default: $artist/$album/$title
+        
+        alternatives:
+          by-year:
+            directory: by-year
+            paths:
+              default: $year/$album/$title
+            formats: link
+        ```
+        
+        The first thing to note here is the `link` format. Instead of
+        converting the files this tells the plugin to create symbolic links to
+        the original audio file.  We also note that the directory is a relative
+        path: it will be resolved with respect to the global `directory`
+        option. We could also omit the directory configuration as it defaults
+        to the collection’s name. Finally, we omitted the `query` option. This
+        means that we want to create symlinks for all files. Of course you can
+        still add a query to select only parts of your collection.
+        
+        The `beet alt update by-year` command will now create the symlinks. For
+        example
+        
+        ```
+        /music/by-year/1982/Thriller/Beat It.mp3
+        -> /music/Michael Jackson/Thriller/Beat It.mp3
+        ```
+        
+        
+        CLI Reference
+        -------------
+        
+        ```
+        beet alt update [--create|--no-create] NAME
+        ```
+        
+        Updates the external collection configured under `alternatives.NAME`.
+        
+        * Add missing files. Convert them to the configured format or copy
+          them.
+        
+        * Remove files that don’t match the query but are still in the
+          external collection
+        
+        * Move files to the path determined from the `paths` configuration.
+        
+        * Update tags if the modification time of the external file is older
+          than that of the source file from the library.
+        
+        The command accepts the following option.
+        
+        * **`--[no-]create`** If the `removable` configuration option
+          is set and the external base directory does not exist, then the
+          command will ask you to confirm the creation of the external
+          collection. These options specify the answer as a cli option.
+        
+        Configuration
+        -------------
+        
+        An external collection is configured as a name-settings-pair under the
+        `alternatives` configuration. The name is used to reference the
+        collection from the command line. The settings is a map of the
+        following settings.
+        
+        * **`directory`** The root directory to store the external files under.
+          Relative paths are resolved with respect to the global `directory`
+          configuration. If omitted it defaults to the name of the collection
+          and is therefore relative to the library directory. (optional)
+        
+        * **`paths`** Path templates for audio files under `directory`. Configured
+          like the [global paths option][config-paths] and defaults to it if
+          not given. (optional)
+        
+        * **`query`** A [query string][] that determine which tracks belong to the
+          collection. A track belongs to the collection if itself or the album
+          it is part of matches the query. To match all items, specify an empty
+          string. (required)
+        
+        * **`formats`** A list of space separated strings that determine the
+          audio file formats in the external collection. If the ‘format’ field
+          of a track is included in the list, the file is copied. Otherwise,
+          the file is transcoded to the first format in the list. The name of
+          the first format must correpond to a key in the
+          [`convert.formats`][convert plugin] configuration. This configuration
+          controls the transcoding process.
+        
+          The special format ‘link’ is used to create symbolik links instead of
+          transcoding the file. It can not be combined with other formats.
+        
+          By default no transcoding is done.
+        
+        * **`removable`** If this is `true` (the default) and `directory` does
+          not exist, the `update` command will ask you to confirm the creation
+          of the external collection. (optional)
+        
+        
+        Feature Requests
+        ----------------
+        
+        If you have an idea or a use case this plugin is missing, feel free to
+        [open an issue](https://github.com/geigerzaehler/beets-alternatives/issues/new).
+        
+        The following is a list of things I might add in the feature.
+        
+        * Symbolic links for each artist in a multiple artists release (see the
+          [beets issue][beets-issue-split-symlinks])
+        
+        
+        License
+        -------
+        
+        Copyright (c) 2014 Thomas Scholtes.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a
+        copy of this software and associated documentation files (the "Software"), to
+        deal in the Software without restriction, including without limitation the
+        rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+        sell copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+        
+        [beets-docs]: https://beets.readthedocs.io/en/latest/index.html
+        [beets-issue-split-symlinks]: https://github.com/sampsyo/beets/issues/153
+        [config-directory]: http://beets.readthedocs.org/en/latest/reference/config.html#directory
+        [config-paths]: http://beets.readthedocs.org/en/latest/reference/config.html#path-format-configuration
+        [convert config]: http://beets.readthedocs.org/en/latest/plugins/convert.html#configuring-the-transcoding-command
+        [convert plugin]: http://beets.readthedocs.org/en/latest/plugins/convert.html
+        [query string]: http://beets.readthedocs.org/en/latest/reference/query.html
+        [using plugins]: http://beets.readthedocs.org/en/latest/plugins/index.html#using-plugins
+        
+Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
-Requires-Dist: beets (>=1.6.0,<2.0.0)
-Requires-Dist: six (>=1.16.0,<2.0.0)
-Project-URL: Repository, http://www.github.com/geigerzaehler/beets-alternatives
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
-
-beets-alternatives
-==================
-
-[![Check and test](https://github.com/geigerzaehler/beets-alternatives/actions/workflows/main.yaml/badge.svg)](https://github.com/geigerzaehler/beets-alternatives/actions/workflows/main.yaml)
-[![Coverage Status](https://coveralls.io/repos/github/geigerzaehler/beets-alternatives/badge.svg?branch=master)](https://coveralls.io/github/geigerzaehler/beets-alternatives?branch=master)
-
-You want to manage multiple versions of your audio files with beets?
-Your favorite iPlayer has limited space and does not support Ogg Vorbis? You
-want to keep lossless versions on a large external drive? You want to
-symlink your audio to other locations?
-
-With this [beets][beets-docs] plugin every file in you music library have
-multiple alternate versions in separate locations.
-
-If you’re interested in contributing to this project, check out the [developer
-documentation](./DEVELOPING.md).
-
-Getting Started
----------------
-
-Install the plugin and make sure you using at least version 1.6.0 of beets and
-Python 3.8.
-
-```bash
-pip install --upgrade beets>=1.6.0 beets-alternatives
-```
-
-Then, [enable the plugin][using plugins]. You may use the `beet config --edit`
-command to add the *alternatives* plugin to the configuration.
-
-```yaml
-plugins:
-- ...
-- alternatives
-```
-
-Now, you can get rolling with one of the use cases below.
-
-### External Files
-
-Suppose your favorite portable player only supports MP3 and MP4, has
-limited disk space and is mounted at `/player`. Instead of selecting
-its content manually and using the `convert` plugin to transcode it, you
-want to sync it automatically. First we give this external collection
-the name ‘myplayer’ and start configuring beets.
-
-```yaml
-alternatives:
-  myplayer:
-    directory: /player
-    paths:
-      default: $album/$title
-    formats: aac mp3
-    query: "onplayer:true"
-    removable: true
-```
-
-The first two options determine the location of the external files and
-correspond to the global [`directory`][config-directory] and
-[`paths`][config-paths] settings.  The `format` option specifies the
-formats we transcode the files to (more on that below).  Finally, the
-`query` option tells the plugin which files you want to put in the
-external location. The value is a [query string][] as used for the
-beets command line. In our case we use a flexible attribute to make the
-selection transparent.
-
-Let’s add some files to our selection by setting the flexible attribute
-from the `query` option. (Since we use boolean values for the
-‘onplayer’ field it might be a good idea to set the type of this field
-to `bool` using the *types* plugin)
-
-```bash
-beet modify onplayer=true artist:Bach
-```
-
-The configured query also matches all tracks that are part of an album
-where the `onplayer` attribute is ‘true’. We could also use
-
-```bash
-beet modify -a onplayer=true albumartist:Bach
-```
-
-We then tell beets to create the external files.
-
-```
-$ beet alt update myplayer
-Collection at '/player' does not exists. Maybe you forgot to mount it.
-Do you want to create the collection? (y/N)
-```
-
-The question makes sure that you don’t recreate a external collection
-if the device is not mounted. Since this is our first go, we answer the
-question with yes.
-
-The command will copy all files with the artist ‘Bach’ and format either ‘AAC’
-or ‘MP3’ to the `/player` directory. All other formats will be transcodec to the
-‘AAC’ format unsing the [*convert* plugin][convert plugin]. The transcoding
-process can be configured through [*convert’s* configuration][convert config].
-
-If you update some tracks in your main collection, the `alt update`
-command will propagate the changes to your external collection.  Since
-we don’t need to convert the files but just update the tags, this will
-be much faster the second time.
-
-```bash
-beet modify composer="Johann Sebastian Bach" artist:Bach
-beet alt update myplayer
-```
-
-After going for a run you mitght realize that Bach is probably not the
-right thing to work out to. So you decide to put Beethoven on your
-player.
-
-```bash
-beet modify onplayer! artist:Bach
-beet modify onplayer=true artist:Beethoven
-beet alt update myplayer
-```
-
-This removes all Bach tracks from the player and adds Beethoven’s.
-
-### Symlink Views
-
-Instead of copying and converting files this plugin can also create
-symbolic links to the files in your library. For example you want to
-have a directory containing all music sorted by year and album.
-
-```yaml
-directory: /music
-paths:
-  default: $artist/$album/$title
-
-alternatives:
-  by-year:
-    directory: by-year
-    paths:
-      default: $year/$album/$title
-    formats: link
-```
-
-The first thing to note here is the `link` format. Instead of
-converting the files this tells the plugin to create symbolic links to
-the original audio file.  We also note that the directory is a relative
-path: it will be resolved with respect to the global `directory`
-option. We could also omit the directory configuration as it defaults
-to the collection’s name. Finally, we omitted the `query` option. This
-means that we want to create symlinks for all files. Of course you can
-still add a query to select only parts of your collection.
-
-The `beet alt update by-year` command will now create the symlinks. For
-example
-
-```plain
-/music/by-year/1982/Thriller/Beat It.mp3
--> /music/Michael Jackson/Thriller/Beat It.mp3
-```
-
-You can also specify if you want absolute symlinks (default) or relative ones
-with `link_type`. The option `link_type` must be `absolute` or `relative`
-
-```yaml
-alternatives:
-  by-year:
-    directory: by-year
-    paths:
-      default: $year/$album/$title
-    formats: link
-    link_type: relative
-```
-
-With this config, the `beet alt update by-year` command will create relative symlinks. E.g:
-
-```plain
-/music/by-year/1982/Thriller/Beat It.mp3
--> ../../../Michael Jackson/Thriller/Beat It.mp3
-```
-
-Now, if you move the `/music/` folder to another location, the links
-will continue working
-
-CLI Reference
--------------
-
-```plain
-beet alt update [--create|--no-create] NAME
-```
-
-Updates the external collection configured under `alternatives.NAME`.
-
-* Add missing files. Convert them to the configured format or copy
-  them.
-
-* Remove files that don’t match the query but are still in the
-  external collection
-
-* Move files to the path determined from the `paths` configuration.
-
-* Update tags if the modification time of the external file is older
-  than that of the source file from the library.
-
-The command accepts the following option.
-
-* **`--[no-]create`** If the `removable` configuration option
-  is set and the external base directory does not exist, then the
-  command will ask you to confirm the creation of the external
-  collection. These options specify the answer as a cli option.
-
-```
-beet alt list-tracks [--format=FORMAT] NAME
-```
-
-Lists all tracks that are currently included in the collection.
-
-The `--format` option accepts a [beets path format][path-format] string that is
-used to format each track.
-
-[path-format]: https://beets.readthedocs.io/en/latest/reference/pathformat.html
-
-Configuration
--------------
-
-An external collection is configured as a name-settings-pair under the
-`alternatives` configuration. The name is used to reference the
-collection from the command line. The settings is a map of the
-following settings.
-
-* **`directory`** The root directory to store the external files under.
-  Relative paths are resolved with respect to the global `directory`
-  configuration. If omitted it defaults to the name of the collection
-  and is therefore relative to the library directory. (optional)
-
-* **`paths`** Path templates for audio files under `directory`. Configured
-  like the [global paths option][config-paths] and defaults to it if
-  not given. (optional)
-
-* **`query`** A [query string][] that determine which tracks belong to the
-  collection. A track belongs to the collection if itself or the album
-  it is part of matches the query. To match all items, specify an empty
-  string. (required)
-
-* **`formats`** A list of space separated strings that determine the
-  audio file formats in the external collection. If the ‘format’ field
-  of a track is included in the list, the file is copied. Otherwise,
-  the file is transcoded to the first format in the list. The name of
-  the first format must correpond to a key in the
-  [`convert.formats`][convert plugin] configuration. This configuration
-  controls the transcoding process.
-
-  The special format ‘link’ is used to create symbolic links instead of
-  transcoding the file. It can not be combined with other formats.
-
-  By default no transcoding is done.
-
-* **`removable`** If this is `true` (the default) and `directory` does
-  not exist, the `update` command will ask you to confirm the creation
-  of the external collection. (optional)
-
-* **`link_type`** Can be `absolute` (default) or `relative`. If
-  **`formats`** is `link`, it sets the type of links to create. For
-  differences between link types and examples see [Symlink Views](#symlink-views).
-
-
-Feature Requests
-----------------
-
-If you have an idea or a use case this plugin is missing, feel free to
-[open an issue](https://github.com/geigerzaehler/beets-alternatives/issues/new).
-
-The following is a list of things I might add in the feature.
-
-* Symbolic links for each artist in a multiple artists release (see the
-  [beets issue][beets-issue-split-symlinks])
-
-
-License
--------
-
-Copyright (c) 2014-2023 Thomas Scholtes.
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-[beets-docs]: https://beets.readthedocs.io/en/latest/index.html
-[beets-issue-split-symlinks]: https://github.com/sampsyo/beets/issues/153
-[config-directory]: http://beets.readthedocs.org/en/latest/reference/config.html#directory
-[config-paths]: http://beets.readthedocs.org/en/latest/reference/config.html#path-format-configuration
-[convert config]: http://beets.readthedocs.org/en/latest/plugins/convert.html#configuring-the-transcoding-command
-[convert plugin]: http://beets.readthedocs.org/en/latest/plugins/convert.html
-[query string]: http://beets.readthedocs.org/en/latest/reference/query.html
-[using plugins]: http://beets.readthedocs.org/en/latest/plugins/index.html#using-plugins
-
```

