# Comparing `tmp/libretrofuzz-2.9.3.tar.gz` & `tmp/libretrofuzz-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.9.3.tar", max compression
+gzip compressed data, was "libretrofuzz-2.9.4.tar", max compression
```

## Comparing `libretrofuzz-2.9.3.tar` & `libretrofuzz-2.9.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-05 10:20:54.806003 libretrofuzz-2.9.3/LICENSE
--rw-r--r--   0        0        0     7557 2023-06-05 10:20:54.806003 libretrofuzz-2.9.3/README.rst
--rw-r--r--   0        0        0       22 2023-06-05 10:20:54.806003 libretrofuzz-2.9.3/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    49413 2023-06-05 10:20:54.806003 libretrofuzz-2.9.3/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      992 2023-06-05 10:20:54.806003 libretrofuzz-2.9.3/pyproject.toml
--rw-r--r--   0        0        0     8761 2023-06-05 10:21:04.979077 libretrofuzz-2.9.3/setup.py
--rw-r--r--   0        0        0     8786 2023-06-05 10:21:04.980087 libretrofuzz-2.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-06 01:18:02.005012 libretrofuzz-2.9.4/LICENSE
+-rw-r--r--   0        0        0     7570 2023-06-06 01:18:02.005012 libretrofuzz-2.9.4/README.rst
+-rw-r--r--   0        0        0       22 2023-06-06 01:18:02.005012 libretrofuzz-2.9.4/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    50308 2023-06-06 01:18:02.005012 libretrofuzz-2.9.4/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      992 2023-06-06 01:18:02.005012 libretrofuzz-2.9.4/pyproject.toml
+-rw-r--r--   0        0        0     8775 2023-06-06 01:18:10.423375 libretrofuzz-2.9.4/setup.py
+-rw-r--r--   0        0        0     8799 2023-06-06 01:18:10.424288 libretrofuzz-2.9.4/PKG-INFO
```

### Comparing `libretrofuzz-2.9.3/LICENSE` & `libretrofuzz-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.3/README.rst` & `libretrofuzz-2.9.4/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -54,26 +54,27 @@
   --system <NAME libretro-fuzz only>
                         Directory name in the server to download thumbnails. If not provided, asked from the user.
   --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
                         | [1<=x<=30]
   --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
                         | [1<=x<=30]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
-  --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.
+  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.
                         | [default: 200; 0<=x<=200]
   --no-fail             Download any score. Equivalent to ``--score 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
-  --verbose             Shows the failures, score and normalized local and server names in output.
+  --verbose N           | Show mininame, len N list (maxscore, server mininame).
+                        | [x>=1]
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
 
 
 
 To install the program, type on the cmd line
```

### Comparing `libretrofuzz-2.9.3/libretrofuzz/__main__.py` & `libretrofuzz-2.9.4/libretrofuzz/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -172,14 +172,24 @@
             #ignore keys in buffer before we are ready
             input.read_keys()
             input.flush_keys()
             typer.echo(typer.style(f'Press escape to quit, enter to continue and most other non-meta keys to skip downloads', bold=True))
             yield done
 
 #----------------non contextual str manipulation------------------------
+def link(uri, label=None, parameters=''):
+    '''
+    Found in github, windows console and many unix consoles trick to embeed hyperlinks/uri with text
+    '''
+    if label is None:
+        label = uri
+    # OSC 8 ; params ; URI ST <name> OSC 8 ;; ST
+    escape_mask = '\033]8;{};{}\033\\{}\033]8;;\033\\'
+    return escape_mask.format(parameters, uri, label)
+
 ppatterns = { '()': regex.compile(r'\([^)(]*\)'), '[]': regex.compile(r'\[[^][]*\]') }
 def removeparenthesis(s, open_p='(', close_p=')'):
     nb_rep = 1
     key = open_p+close_p
     try:
       pattern = ppatterns[key]
     except:
@@ -228,37 +238,37 @@
     return flips
 
 #-----------------------------------------------------------------------------------------------------------------------
 #The heart of the program, what orders titles to be 'more similar' or less to the local labels (after the normalization)
 #-----------------------------------------------------------------------------------------------------------------------
 class TitleScorer(object):
     def __init__(self):
-        #rapidfuzz says to use range 0-100, but this doesn't (it's much easier that way), so it uses internal api to prevent a possible early exit at == 100
-        self._RF_ScorerPy = { 'get_scorer_flags': lambda **kwargs: {'optimal_score': MAX_SCORE, 'worst_score': 0, 'flags': (1 << 6)} }
+      #rapidfuzz says to use range 0-100, but this doesn't (it's much easier that way)
+      #so it uses internal api to prevent a possible early exit at == 100
+      self._RF_ScorerPy = { 'get_scorer_flags': lambda **kwargs: {'optimal_score': MAX_SCORE, 'worst_score': 0, 'flags': (1 << 6)} }
 
     def __call__(self, s1, s2, processor=None, score_cutoff=None):
-        prefix = len(os.path.commonprefix([s1, s2]))
-        if prefix <= 2 and len(s1) != len(s2):
-            #ideally this branch wouldn't exist, but since many games do not have
-            #images, they get caught up on a short title 'score' from token_set_ratio
-            #without the real title to win the similarity+prefix heuristic
-            #this removes many false positives and causes few false negatives.
-            return 0
-        else:
-            if s1 == s2:
-                return MAX_SCORE
-            #score_cutoff needs to be 0 from a combination of 3 factors that create a bug:
-            #1. the caller of this, extractOne passes the 'current best score' as score_cutoff
-            #2. the token_set_ratio function returns 0 if the calculated score < score_cutoff
-            #3. 'current best score' includes the prefix, which this call can't include in 2.
-            similarity = fuzz.token_set_ratio(s1,s2,processor=None,score_cutoff=0)
-            #Combine the scorer with a common prefix heuristic to give priority to longer similar
-            #names, this helps prevents false positives for shorter strings which token set ratio
-            #is prone because it sets score to 100 if one string words are completely on the other.
-            return min(MAX_SCORE-1,similarity + prefix)
+      if (min(len(s1),len(s2)) / max(len(s1),len(s2))) < 0.3:
+        #ideally this branch wouldn't exist, but since many games do not have
+        #images, they get caught up on a short title being completely contained in another
+        #token_set_ratio gives that 100. Skip if the smaller name length is less than 30%
+        return 0
+      #names are whitespace and case normalized
+      if s1 == s2:
+        return MAX_SCORE
+      prefix = len(os.path.commonprefix([s1, s2]))
+      #score_cutoff needs to be 0 from a combination of 3 factors that create a bug:
+      #1. the caller of this, extract passes the 'current best score' as score_cutoff
+      #2. the token_set_ratio function returns 0 if the calculated score < score_cutoff
+      #3. 'current best score' includes the prefix, which this call can't include in 2.
+      similarity = fuzz.token_set_ratio(s1,s2,processor=None,score_cutoff=0)
+      #Combine the scorer with a common prefix heuristic to give priority to longer similar
+      #names, this helps prevents false positives for shorter strings which token set ratio
+      #is prone because it sets score to 100 if one string words are completely on the other.
+      return min(MAX_SCORE-1,similarity + prefix)
 
 #-----------------------------------------------------------------------------------------------------------------------------
 # Normalization functions, part of the functions that change both local labels and remote names to be more similar to compare
 #-----------------------------------------------------------------------------------------------------------------------------
 camelcase_pattern = regex.compile(r'(\p{Lu}\p{Ll}+)')
 #number sequences in the middle (not start or end) of a string that start with 0
 zero_lead_pattern = regex.compile(r'([^\d])0+([1-9])')
@@ -314,17 +324,14 @@
     t = removefirst(t, ', a')
     t = removeprefix(t, 'a ')
     #remove the symbols used in the definite article normalization
     t = replacemany(t, ',\'', '')
     #this makes sure that if a remote name has ' and ' instead of ' _ ' to replace ' & ' it works
     #': ' doesn't need this because ':' is a forbidden character and both '_' and '-' turn to ''
     t = t.replace(' and ',  '')
-    #although all names have spaces (now), the local names may have weird spaces,
-    #so to equalize them after the space dependent checks (this also strips)
-    t = ''.join(t.split())
     #Tries to make roman numerals in the range 1-20 equivalent to normal numbers (to handle names that change it).
     #If both sides are roman numerals there is no harm done if XXIV gets turned into 204 in both sides.
     t = t.replace('xviii', '18')
     t = t.replace('xvii',  '17')
     t = t.replace('xvi' ,  '16')
     t = t.replace('xiii',  '13')
     t = t.replace('xii' ,  '12')
@@ -341,15 +348,16 @@
     t = t.replace('iv' ,  '4')
     t = t.replace('v'  ,  '5')
     t = t.replace('ix',   '9')
     t = t.replace('x',   '10')
     t = t.replace('i',    '1')
     #remove diacritics (does nothing to asian languages diacritics, only for 2 to 1 character combinations)
     t = u''.join([c for c in unicodedata.normalize('NFKD', t) if not unicodedata.combining(c)])
-    return t
+    #normalize spaces (don't remove them for other later score methods to be able to reorder tokens
+    return ' '.join(t.split())
 
 def nosubtitle_normalizer(t, nometa, hack):
     return normalizer(nosubtitle_aux(t), nometa, hack)
 
 #---------------------------------------------------------------------------------
 # Initalization functions, since there are two main programs so the code is reused
 #---------------------------------------------------------------------------------
@@ -450,14 +458,20 @@
     return Path(fdir)
 
 def error(error: str):
     typer.echo(typer.style(error, fg=typer.colors.RED, bold=True))
 
 def test_common_errors(cfg: Path, playlist: str, system: str, address: str):
     '''returns a tuple with (playlist_dir: Path, thumbnail_dir: Path, PLAYLISTS: [Path], SYSTEMS: [str]) '''
+    #stop showing the variables - a library installed this behind my back
+    try:
+      from rich.traceback import install
+      install(show_locals=False)
+    except ImportError:
+      pass
     global ADDRESS
     ADDRESS = address.rstrip('/')
     global viewer
     viewer = which('chafa')
     if not viewer:
         typer.echo(f'Shell image viewer chafa was not found')
     if not cfg or not cfg.is_file():
@@ -497,24 +511,24 @@
 #####################
 def mainfuzzsingle(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
         playlist: str = typer.Option(None, metavar='NAME', help='Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.'),
         system: str = typer.Option(None, metavar='NAME', help='Directory name in the server to download thumbnails. If not provided, asked from the user.'),
         wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
         wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
         filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
-        score: int = typer.Option(MAX_SCORE, '--score', min=0, max=MAX_SCORE, metavar='FUZZ', help='Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with --no-fail.'),
+        score: int = typer.Option(MAX_SCORE, '--min', min=0, max=MAX_SCORE, metavar='SCORE', help=f'0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.'),
         nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
         noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
         nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
         nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
         nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
         hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
         before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
         address: Optional[str] = typer.Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
-        verbose: bool = typer.Option(False, '--verbose', help='Shows the failures, score and normalized local and server names in output.')
+        verbose: Optional[int] = typer.Option(None, '--verbose', min=1, metavar='N', help=f'Show mininame, len N list (maxscore, server mininame).')
     ):
     if playlist and not playlist.lower().endswith('.lpl'):
         playlist = playlist + '.lpl'
     
     playlist_dir, thumbnails_dir, PLAYLISTS, SYSTEMS = test_common_errors(cfg, playlist, system, address)
     
     custom_style = Style([
@@ -553,24 +567,24 @@
             raise typer.Exit()
     asyncio.run(runit(), debug=False)
 
 def mainfuzzall(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
         wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
         wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
         filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
-        score: int = typer.Option(MAX_SCORE, '--score', min=0, max=MAX_SCORE, metavar='FUZZ', help='Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with --no-fail.'),
+        score: int = typer.Option(MAX_SCORE, '--min', min=0, max=MAX_SCORE, metavar='SCORE', help=f'0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.'),
         nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
         noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
         nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
         nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
         nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
         hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
         before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
         address: Optional[str] = typer.Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
-        verbose: bool = typer.Option(False, '--verbose', help='Shows the failures, score and normalized local and server names in output.')
+        verbose: Optional[int] = typer.Option(None, '--verbose', min=1, metavar='N', help=f'Show mininame, len N list (maxscore, server mininame).')
     ):
     playlist_dir, thumbnails_dir, PLAYLISTS, SYSTEMS = test_common_errors(cfg, None, None, address)
     
     notInSystems = [ (playlist, os.path.basename(playlist)[:-4]) for playlist in PLAYLISTS if os.path.basename(playlist)[:-4] not in SYSTEMS]
     for playlist, system in notInSystems:
         PLAYLISTS.remove(playlist)
     inSystems = [ (playlist, os.path.basename(playlist)[:-4]) for playlist in PLAYLISTS ]
@@ -626,15 +640,15 @@
 
 async def downloader(names: [(str,str)],
                system: str,
                wait_before: Optional[float],
                wait_after: Optional[float],
                filters: Optional[List[str]],
                score: int,
-               noimage : bool, nomerge: bool, nofail: bool, nometa: bool, hack: bool, nosubtitle: bool, verbose: bool,
+               noimage : bool, nomerge: bool, nofail: bool, nometa: bool, hack: bool, nosubtitle: bool, verbose: Optional[int],
                before: Optional[str],
                tmpdir: Path,
                thumbnails_dir: Path,
                client: AsyncClient
                ):
     #not a error to pass a empty playlist
     if len(names) == 0:
@@ -693,48 +707,55 @@
 
         #unlike the server thumbnails, normalization wasn't done yet
         nameaux = norm(nameaux, nometa, hack)
         
         #operate on cache (to speed up by not applying normalization every iteration)
         #the normalization can make it so that the winner has the same score as the runner up(s) so to make sure we catch at least
         #two thumbnails for cases where that happens, we check both best scores if we can't find a thumb in a server directory
-        result = process.extract(nameaux, remote_names, scorer=title_scorer,processor=None,limit=2,score_cutoff=None)
-        norm_thumbnail, i_max, thumbnail = (None, 0, None)
-        thumbnail2 = None
-        if len(result) == 1:
-            norm_thumbnail, i_max, thumbnail = result[0]
-        elif len(result) == 2:
-            norm_thumbnail, i_max, thumbnail = result[0]
-            if result[0][1] == result[1][1]: #equal scores
-                thumbnail2 = result[1][2]
+        result = process.extract(nameaux, remote_names, scorer=title_scorer,processor=None,limit=verbose or 1,score_cutoff=None)
+        #build the verbose format and decompose the first result, with a optimization if verbose is not on
+        thumb_normal, thumb_score, thumb_name = (None, 0, None)
+        verbose_format = []
+        if verbose:
+          for r in reversed(result):
+            thumb_normal, thumb_score, thumb_name = r
+            color = typer.colors.RED if thumb_score < score else typer.colors.GREEN
+            verbose_format.insert(0, f"{typer.style(f'{int(thumb_score)}', fg=f'{color}', bold=True)} {thumb_normal}")
+          verbose_format = '|'.join(verbose_format)
+        elif len(result) > 0:
+          thumb_normal, thumb_score, thumb_name = result[0]
+        #hack, if result 1 and 2 have equal scores use the second thumbnail as a alternative if missing a thumb type
+        #this is done because it's relatively common for the server to have a case mistake on thumb types
+        thumb_name2 = None
+        if len(result) >= 2:
+          if result[0][1] == result[1][1]:
+            thumb_name2 = result[1][2]
         #formating legos
-        zeroth_format  = '  0 ' if verbose else ''
-        prefix_format  = '{:>3} '.format(str(int(i_max))) if verbose else ''
-        name_format    = f'{nameaux} -> {norm_thumbnail}' if verbose else f'{name} -> {thumbnail}'
-        success_format = f'{prefix_format}{typer.style("Success",   fg=typer.colors.GREEN, bold=True)}: {name_format}'
-        failure_format = f'{prefix_format}{typer.style("Failure",     fg=typer.colors.RED, bold=True)}: {name_format}'
-        missing_format = f'{prefix_format}{typer.style("Missing",     fg=typer.colors.RED, bold=True)}:'
-        cancel_format  = f'{prefix_format}{typer.style("Skipped",        fg=(135,135,135), bold=True)}: {name_format}'
-        nomerge_format = f'{zeroth_format}{typer.style("Nomerge",        fg=(128,128,128), bold=True)}: {name_format}'
-        getting_format = f'{prefix_format}{typer.style("Getting",    fg=typer.colors.BLUE, bold=True)}: {name_format}'
-        waiting_format = f'{prefix_format}{typer.style("Waiting",  fg=typer.colors.YELLOW, bold=True)}: {name_format}' '{bar:-9b} {remaining_s:2.1f}s: {bar:10u}'
-        if thumbnail and i_max >= score:
+        name_format    = f'{nameaux} -> {verbose_format}' if verbose else f'{name} -> {thumb_name}'
+        success_format = f'{typer.style("Success",   fg=typer.colors.GREEN, bold=True)}: {name_format}'
+        failure_format = f'{typer.style("Failure",     fg=typer.colors.RED, bold=True)}: {name_format}'
+        missing_format = f'{typer.style("Missing",     fg=typer.colors.RED, bold=True)}: {name_format}'
+        cancel_format  = f'{typer.style("Skipped",        fg=(135,135,135), bold=True)}: {name_format}'
+        nomerge_format = f'{typer.style("Nomerge",        fg=(128,128,128), bold=True)}: {name_format}'
+        getting_format = f'{typer.style("Getting",    fg=typer.colors.BLUE, bold=True)}: {name_format}'
+        waiting_format = f'{typer.style("Waiting",  fg=typer.colors.YELLOW, bold=True)}: {name_format}' '{bar:-9b} {remaining_s:2.1f}s: {bar:10u}'
+        if thumb_name and thumb_score >= score:
             allow = True
             #these parent directories were created when reading the playlist, more efficient than doing it a playlist game loop
             real_thumb_dir = Path(thumbnails_dir,destination)
             down_thumb_dir = Path(tmpdir,destination)
             if not filters and nomerge:
                 #to implement no-merge you have to disable downloads on 'at least one' thumbnail (including user added ones)
                 missing_thumbs = 0
                 missing_server_thumbs = 0
                 for dirname in Thumbs._fields:
                     real = Path(real_thumb_dir, dirname, name + '.png')
                     if not real.exists():
                         missing_thumbs += 1
-                        if thumbnail in getattr(thumbs, dirname) or thumbnail2 in getattr(thumbs, dirname):
+                        if thumb_name in getattr(thumbs, dirname) or thumb_name2 in getattr(thumbs, dirname):
                             missing_server_thumbs += 1
                 allow = missing_thumbs == 3
                 #despite the above, print only for when it would download if it was allowed, otherwise it is confusing
                 if not allow and missing_server_thumbs > 0:
                     typer.echo(nomerge_format)
             if allow:
                 first_wait      = wait_before is not None
@@ -743,15 +764,15 @@
                 try:
                     for dirname in Thumbs._fields:
                         real = Path(real_thumb_dir, dirname, name + '.png')
                         temp = Path(down_thumb_dir, dirname, name + '.png')
                         downloaded_dict[dirname] = (real, temp)
                         #something to download
                         thumbmap = getattr(thumbs, dirname)
-                        url = thumbmap[thumbnail] if thumbnail in thumbmap else thumbmap.get(thumbnail2, None)
+                        url = thumbmap[thumb_name] if thumb_name in thumbmap else thumbmap.get(thumb_name2, None)
                         #with filters/reset you always download, and without only if it doesn't exist already.
                         if url and (filters or not real.exists()):
                             download_format = f'{getting_format}' '{bar:-9b}' f'{dirname[6:-1]}' ' {percentage:3.0f}%: {bar:10u}'
                             if await download(client,url,temp,download_format,missing_format,waiting_format,first_wait,wait_before,MAX_RETRIES):
                                 first_wait = False
                                 downloaded_once = True
                         elif filters:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `libretrofuzz-2.9.3/pyproject.toml` & `libretrofuzz-2.9.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.9.3"
+version = "2.9.4"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.9.3/setup.py` & `libretrofuzz-2.9.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.9.3',
+    'version': '2.9.4',
     'description': 'Fuzzy Retroarch thumbnail downloader',
-    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose             Shows the failures, score and normalized local and server names in output.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
+    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show mininame, len N list (maxscore, server mininame).\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libretrofuzz-2.9.3/PKG-INFO` & `libretrofuzz-2.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.9.3
+Version: 2.9.4
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -84,26 +84,27 @@
   --system <NAME libretro-fuzz only>
                         Directory name in the server to download thumbnails. If not provided, asked from the user.
   --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
                         | [1<=x<=30]
   --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
                         | [1<=x<=30]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
-  --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.
+  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.
                         | [default: 200; 0<=x<=200]
   --no-fail             Download any score. Equivalent to ``--score 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
-  --verbose             Shows the failures, score and normalized local and server names in output.
+  --verbose N           | Show mininame, len N list (maxscore, server mininame).
+                        | [x>=1]
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
 
 
 
 To install the program, type on the cmd line
```

