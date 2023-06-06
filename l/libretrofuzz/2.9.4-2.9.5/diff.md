# Comparing `tmp/libretrofuzz-2.9.4.tar.gz` & `tmp/libretrofuzz-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.9.4.tar", max compression
+gzip compressed data, was "libretrofuzz-2.9.5.tar", max compression
```

## Comparing `libretrofuzz-2.9.4.tar` & `libretrofuzz-2.9.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-06 01:18:02.005012 libretrofuzz-2.9.4/LICENSE
--rw-r--r--   0        0        0     7570 2023-06-06 01:18:02.005012 libretrofuzz-2.9.4/README.rst
--rw-r--r--   0        0        0       22 2023-06-06 01:18:02.005012 libretrofuzz-2.9.4/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    50308 2023-06-06 01:18:02.005012 libretrofuzz-2.9.4/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      992 2023-06-06 01:18:02.005012 libretrofuzz-2.9.4/pyproject.toml
--rw-r--r--   0        0        0     8775 2023-06-06 01:18:10.423375 libretrofuzz-2.9.4/setup.py
--rw-r--r--   0        0        0     8799 2023-06-06 01:18:10.424288 libretrofuzz-2.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-06 12:37:05.877101 libretrofuzz-2.9.5/LICENSE
+-rw-r--r--   0        0        0     7570 2023-06-06 12:37:05.877101 libretrofuzz-2.9.5/README.rst
+-rw-r--r--   0        0        0       22 2023-06-06 12:37:05.877101 libretrofuzz-2.9.5/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    50675 2023-06-06 12:37:05.877101 libretrofuzz-2.9.5/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      992 2023-06-06 12:37:05.877101 libretrofuzz-2.9.5/pyproject.toml
+-rw-r--r--   0        0        0     8775 2023-06-06 12:37:29.654121 libretrofuzz-2.9.5/setup.py
+-rw-r--r--   0        0        0     8799 2023-06-06 12:37:29.655128 libretrofuzz-2.9.5/PKG-INFO
```

### Comparing `libretrofuzz-2.9.4/LICENSE` & `libretrofuzz-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.4/README.rst` & `libretrofuzz-2.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.4/libretrofuzz/__main__.py` & `libretrofuzz-2.9.5/libretrofuzz/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,16 +174,19 @@
             input.flush_keys()
             typer.echo(typer.style(f'Press escape to quit, enter to continue and most other non-meta keys to skip downloads', bold=True))
             yield done
 
 #----------------non contextual str manipulation------------------------
 def link(uri, label=None, parameters=''):
     '''
-    Found in github, windows console and many unix consoles trick to embeed hyperlinks/uri with text
+    Found in https://gist.github.com/egmontkob/eb114294efbcd5adb1944c9f3cb5feda
     '''
+    if type(uri) is str: #just hover text and show same hyperlinks if possible
+        import urllib.parse
+        uri = urllib.parse.quote(uri)
     if label is None:
         label = uri
     # OSC 8 ; params ; URI ST <name> OSC 8 ;; ST
     escape_mask = '\033]8;{};{}\033\\{}\033]8;;\033\\'
     return escape_mask.format(parameters, uri, label)
 
 ppatterns = { '()': regex.compile(r'\([^)(]*\)'), '[]': regex.compile(r'\[[^][]*\]') }
@@ -668,14 +671,16 @@
     norm = nosubtitle_normalizer if nosubtitle else normalizer
     #we choose the highest similarity of all 3 directories, since no mixed matches are allowed
     remote_names = set()
     remote_names.update(thumbs.Named_Boxarts.keys(), thumbs.Named_Titles.keys(), thumbs.Named_Snaps.keys())
     #turn into a set, original key and normalized value.
     remote_names = { x : norm(x, nometa, hack) for x in remote_names }
     for (name,destination) in names:
+        #allow a slighty async pause to be able to update the key status if never won a single score
+        await asyncio.sleep(0)
         #if called escape without being in a download zone, exit right away without a cancel print
         checkEscape()
         #if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x : fnmatch.fnmatch(name, x), filters)):
             continue
         #to simplify this code, the forbidden characters are replaced twice,
         #on the string that is going to be the filename and the modified string copy of that that is going to be matched.
@@ -715,33 +720,35 @@
         #build the verbose format and decompose the first result, with a optimization if verbose is not on
         thumb_normal, thumb_score, thumb_name = (None, 0, None)
         verbose_format = []
         if verbose:
           for r in reversed(result):
             thumb_normal, thumb_score, thumb_name = r
             color = typer.colors.RED if thumb_score < score else typer.colors.GREEN
-            verbose_format.insert(0, f"{typer.style(f'{int(thumb_score)}', fg=f'{color}', bold=True)} {thumb_normal}")
-          verbose_format = '|'.join(verbose_format)
+            linke = link(thumb_name, thumb_normal)
+            verbose_format.insert(0, f"{typer.style(f'{int(thumb_score)}', fg=f'{color}', bold=True)} {linke}")
+          verbose_format = ', '.join(verbose_format)
         elif len(result) > 0:
           thumb_normal, thumb_score, thumb_name = result[0]
         #hack, if result 1 and 2 have equal scores use the second thumbnail as a alternative if missing a thumb type
         #this is done because it's relatively common for the server to have a case mistake on thumb types
         thumb_name2 = None
         if len(result) >= 2:
           if result[0][1] == result[1][1]:
             thumb_name2 = result[1][2]
         #formating legos
-        name_format    = f'{nameaux} -> {verbose_format}' if verbose else f'{name} -> {thumb_name}'
+        name_format    = link(name,nameaux) + ' -> ' + verbose_format if verbose else f'{name} -> {thumb_name}'
         success_format = f'{typer.style("Success",   fg=typer.colors.GREEN, bold=True)}: {name_format}'
         failure_format = f'{typer.style("Failure",     fg=typer.colors.RED, bold=True)}: {name_format}'
         missing_format = f'{typer.style("Missing",     fg=typer.colors.RED, bold=True)}: {name_format}'
         cancel_format  = f'{typer.style("Skipped",        fg=(135,135,135), bold=True)}: {name_format}'
         nomerge_format = f'{typer.style("Nomerge",        fg=(128,128,128), bold=True)}: {name_format}'
         getting_format = f'{typer.style("Getting",    fg=typer.colors.BLUE, bold=True)}: {name_format}'
-        waiting_format = f'{typer.style("Waiting",  fg=typer.colors.YELLOW, bold=True)}: {name_format}' '{bar:-9b} {remaining_s:2.1f}s: {bar:10u}'
+        waiting_format = f'{typer.style("Waiting",  fg=typer.colors.YELLOW, bold=True)}: {name_format}' \
+                         + typer.style(' {remaining_s:2.1f}s', fg=typer.colors.RED, bold=True)
         if thumb_name and thumb_score >= score:
             allow = True
             #these parent directories were created when reading the playlist, more efficient than doing it a playlist game loop
             real_thumb_dir = Path(thumbnails_dir,destination)
             down_thumb_dir = Path(tmpdir,destination)
             if not filters and nomerge:
                 #to implement no-merge you have to disable downloads on 'at least one' thumbnail (including user added ones)
```

### Comparing `libretrofuzz-2.9.4/pyproject.toml` & `libretrofuzz-2.9.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.9.4"
+version = "2.9.5"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.9.4/setup.py` & `libretrofuzz-2.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.9.4',
+    'version': '2.9.5',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show mininame, len N list (maxscore, server mininame).\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-2.9.4/PKG-INFO` & `libretrofuzz-2.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.9.4
+Version: 2.9.5
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

