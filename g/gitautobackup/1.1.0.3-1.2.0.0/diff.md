# Comparing `tmp/gitautobackup-1.1.0.3.tar.gz` & `tmp/gitautobackup-1.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitautobackup-1.1.0.3.tar", last modified: Thu Jun  1 18:35:01 2023, max compression
+gzip compressed data, was "gitautobackup-1.2.0.0.tar", last modified: Tue Jun  6 18:01:14 2023, max compression
```

## Comparing `gitautobackup-1.1.0.3.tar` & `gitautobackup-1.2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:35:01.612469 gitautobackup-1.1.0.3/
--rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-1.1.0.3/LICENSE
--rw-rw-rw-   0        0        0    45682 2023-06-01 18:35:01.605926 gitautobackup-1.1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6929 2023-05-31 14:45:35.000000 gitautobackup-1.1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 18:35:01.541103 gitautobackup-1.1.0.3/gitautobackup.egg-info/
--rw-rw-rw-   0        0        0    45682 2023-06-01 18:35:00.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-06-01 18:35:01.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:35:00.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-06-01 18:35:00.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      158 2023-06-01 18:35:00.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-01 18:35:00.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-01 18:34:59.000000 gitautobackup-1.1.0.3/gitautobackup.egg-info/zip-safe
--rw-rw-rw-   0        0        0    16843 2023-06-01 18:32:58.000000 gitautobackup-1.1.0.3/gitautobackup.py
--rw-rw-rw-   0        0        0     3198 2023-06-01 18:32:58.000000 gitautobackup-1.1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 18:35:01.613468 gitautobackup-1.1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 18:01:13.998214 gitautobackup-1.2.0.0/
+-rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-1.2.0.0/LICENSE
+-rw-rw-rw-   0        0        0    46152 2023-06-06 18:01:13.994214 gitautobackup-1.2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7399 2023-06-06 17:48:44.000000 gitautobackup-1.2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 18:01:13.967295 gitautobackup-1.2.0.0/gitautobackup.egg-info/
+-rw-rw-rw-   0        0        0    46152 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 18:01:11.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/zip-safe
+-rw-rw-rw-   0        0        0    23671 2023-06-06 18:00:36.000000 gitautobackup-1.2.0.0/gitautobackup.py
+-rw-rw-rw-   0        0        0     3198 2023-06-01 18:32:58.000000 gitautobackup-1.2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 18:01:13.999773 gitautobackup-1.2.0.0/setup.cfg
```

### Comparing `gitautobackup-1.1.0.3/LICENSE` & `gitautobackup-1.2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitautobackup-1.1.0.3/PKG-INFO` & `gitautobackup-1.2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 1.1.0.3
+Version: 1.2.0.0
 Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -436,27 +436,32 @@
 This module does not have any required arguments, as everything does have a default behaviour. The most importnant thing to note is that when not supplied with the path of the git repository, it attempts to deduce the location of a git repository (by testing if the directory is able to be loaded as a git repository) from (in this specific order):
 
 1. The console's current working direcory
 2. The directory given in the 0th arg of the command line (aka ``sys.argv[0]``'s lowest directory)
 3. The location of this file itself
    For those wanting to acess this logic when using this a  a module the ``get_default_git_location()`` function will return this value.
 
-- ``-p`` or ``--path`` specifies the repository path
-- ``-m`` or ``--message`` (or others) specifies the commit's message.
-- ``-f``, ``--force``, or ``--forcecommit`` makes a commit be made even if nothing was changed
-- ``--fc``, ``--forcecompress`` forces the repository's database to always be compressed, even if it not really necessary. This cannot be combined with ``--fnc``
-- ``--fnc``, ``--forcenocompress`` forces the repository's database to never be compressed, even if it might be beneficial. This cannot be combined with ``--fc``
-- ``-v``, ``--verbose`` makes the output of the program more noisy. This cannot be combined with ``-q``
-- ``-q``, ``--quiet`` greatly reduces the output of the program. This cannot be combined with ``-v``
+Here are a few of the possible arguments to use:
+
+- ``-p`` / ``--path`` specifies the repository path
+- ``-m`` / ``--message`` specifies the commit's message.
+- ``-t`` / ``--tag`` sets a tag for the commit
+- ``-a`` / ``--archive`` / ``--archive_path`` sets a path for a archive file to be made. If this isn't used a archive file will not be made.
+- ``-f`` / ``--force`` / ``--force_commit`` makes a commit be made even if nothing was changed
+- ``--fc`` / ``--force_compress`` forces the repository's database to always be compressed, even if its not really necessary. This cannot be combined with ``--fnc`` or ``--fca``
+- ``--fnc`` / ``--force_no_compress`` forces the repository's database to never be compressed, even if it might be beneficial. This cannot be combined with ``--fc`` or ``--fca``
+- ``--fca`` / ``--force_compress_aggressive`` forces the repository's database compressed aggressively (taking a much longer time), even if its not necessary. This cannot be combined with ``--fc`` or ``--fnc``
+- ``-v`` / ``--verbose`` makes the output of the program more noisy. This cannot be combined with ``-q``
+- ``-q`` / ``--quiet`` greatly reduces the output of the program. This cannot be combined with ``-v``
 
 There are also the traditional arguments that report various information about this software then exit:
 
-- ``--ver`` or ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
-- ``-h`` or ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
-- ``--git`` or ``--github`` prints a like to the github repository and then exits. You don't need a input file if you run this command.
+- ``--ver`` / ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
+- ``-h`` / ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
+- ``--git`` / ``--github`` prints a like to the github repository and then exits. You don't need a input file if you run this command.
 
 ### Without ``argparse``
 
 While using this on the command line without ``argparse`` is not suggested, you may still access a diminished selection of features:
 
 - The ``-m`` or ``--message`` flag still works
 - The path of the git repository does not require a flag and can simply have it path stated. If multiple paths are given, the first one thats a valid repository will be chosen. The program will explicitly fail if none where given.
```

### Comparing `gitautobackup-1.1.0.3/README.md` & `gitautobackup-1.2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,27 +31,32 @@
 This module does not have any required arguments, as everything does have a default behaviour. The most importnant thing to note is that when not supplied with the path of the git repository, it attempts to deduce the location of a git repository (by testing if the directory is able to be loaded as a git repository) from (in this specific order):
 
 1. The console's current working direcory
 2. The directory given in the 0th arg of the command line (aka ``sys.argv[0]``'s lowest directory)
 3. The location of this file itself
    For those wanting to acess this logic when using this a  a module the ``get_default_git_location()`` function will return this value.
 
-- ``-p`` or ``--path`` specifies the repository path
-- ``-m`` or ``--message`` (or others) specifies the commit's message.
-- ``-f``, ``--force``, or ``--forcecommit`` makes a commit be made even if nothing was changed
-- ``--fc``, ``--forcecompress`` forces the repository's database to always be compressed, even if it not really necessary. This cannot be combined with ``--fnc``
-- ``--fnc``, ``--forcenocompress`` forces the repository's database to never be compressed, even if it might be beneficial. This cannot be combined with ``--fc``
-- ``-v``, ``--verbose`` makes the output of the program more noisy. This cannot be combined with ``-q``
-- ``-q``, ``--quiet`` greatly reduces the output of the program. This cannot be combined with ``-v``
+Here are a few of the possible arguments to use:
+
+- ``-p`` / ``--path`` specifies the repository path
+- ``-m`` / ``--message`` specifies the commit's message.
+- ``-t`` / ``--tag`` sets a tag for the commit
+- ``-a`` / ``--archive`` / ``--archive_path`` sets a path for a archive file to be made. If this isn't used a archive file will not be made.
+- ``-f`` / ``--force`` / ``--force_commit`` makes a commit be made even if nothing was changed
+- ``--fc`` / ``--force_compress`` forces the repository's database to always be compressed, even if its not really necessary. This cannot be combined with ``--fnc`` or ``--fca``
+- ``--fnc`` / ``--force_no_compress`` forces the repository's database to never be compressed, even if it might be beneficial. This cannot be combined with ``--fc`` or ``--fca``
+- ``--fca`` / ``--force_compress_aggressive`` forces the repository's database compressed aggressively (taking a much longer time), even if its not necessary. This cannot be combined with ``--fc`` or ``--fnc``
+- ``-v`` / ``--verbose`` makes the output of the program more noisy. This cannot be combined with ``-q``
+- ``-q`` / ``--quiet`` greatly reduces the output of the program. This cannot be combined with ``-v``
 
 There are also the traditional arguments that report various information about this software then exit:
 
-- ``--ver`` or ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
-- ``-h`` or ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
-- ``--git`` or ``--github`` prints a like to the github repository and then exits. You don't need a input file if you run this command.
+- ``--ver`` / ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
+- ``-h`` / ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
+- ``--git`` / ``--github`` prints a like to the github repository and then exits. You don't need a input file if you run this command.
 
 ### Without ``argparse``
 
 While using this on the command line without ``argparse`` is not suggested, you may still access a diminished selection of features:
 
 - The ``-m`` or ``--message`` flag still works
 - The path of the git repository does not require a flag and can simply have it path stated. If multiple paths are given, the first one thats a valid repository will be chosen. The program will explicitly fail if none where given.
```

### Comparing `gitautobackup-1.1.0.3/gitautobackup.egg-info/PKG-INFO` & `gitautobackup-1.2.0.0/gitautobackup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 1.1.0.3
+Version: 1.2.0.0
 Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -436,27 +436,32 @@
 This module does not have any required arguments, as everything does have a default behaviour. The most importnant thing to note is that when not supplied with the path of the git repository, it attempts to deduce the location of a git repository (by testing if the directory is able to be loaded as a git repository) from (in this specific order):
 
 1. The console's current working direcory
 2. The directory given in the 0th arg of the command line (aka ``sys.argv[0]``'s lowest directory)
 3. The location of this file itself
    For those wanting to acess this logic when using this a  a module the ``get_default_git_location()`` function will return this value.
 
-- ``-p`` or ``--path`` specifies the repository path
-- ``-m`` or ``--message`` (or others) specifies the commit's message.
-- ``-f``, ``--force``, or ``--forcecommit`` makes a commit be made even if nothing was changed
-- ``--fc``, ``--forcecompress`` forces the repository's database to always be compressed, even if it not really necessary. This cannot be combined with ``--fnc``
-- ``--fnc``, ``--forcenocompress`` forces the repository's database to never be compressed, even if it might be beneficial. This cannot be combined with ``--fc``
-- ``-v``, ``--verbose`` makes the output of the program more noisy. This cannot be combined with ``-q``
-- ``-q``, ``--quiet`` greatly reduces the output of the program. This cannot be combined with ``-v``
+Here are a few of the possible arguments to use:
+
+- ``-p`` / ``--path`` specifies the repository path
+- ``-m`` / ``--message`` specifies the commit's message.
+- ``-t`` / ``--tag`` sets a tag for the commit
+- ``-a`` / ``--archive`` / ``--archive_path`` sets a path for a archive file to be made. If this isn't used a archive file will not be made.
+- ``-f`` / ``--force`` / ``--force_commit`` makes a commit be made even if nothing was changed
+- ``--fc`` / ``--force_compress`` forces the repository's database to always be compressed, even if its not really necessary. This cannot be combined with ``--fnc`` or ``--fca``
+- ``--fnc`` / ``--force_no_compress`` forces the repository's database to never be compressed, even if it might be beneficial. This cannot be combined with ``--fc`` or ``--fca``
+- ``--fca`` / ``--force_compress_aggressive`` forces the repository's database compressed aggressively (taking a much longer time), even if its not necessary. This cannot be combined with ``--fc`` or ``--fnc``
+- ``-v`` / ``--verbose`` makes the output of the program more noisy. This cannot be combined with ``-q``
+- ``-q`` / ``--quiet`` greatly reduces the output of the program. This cannot be combined with ``-v``
 
 There are also the traditional arguments that report various information about this software then exit:
 
-- ``--ver`` or ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
-- ``-h`` or ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
-- ``--git`` or ``--github`` prints a like to the github repository and then exits. You don't need a input file if you run this command.
+- ``--ver`` / ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
+- ``-h`` / ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
+- ``--git`` / ``--github`` prints a like to the github repository and then exits. You don't need a input file if you run this command.
 
 ### Without ``argparse``
 
 While using this on the command line without ``argparse`` is not suggested, you may still access a diminished selection of features:
 
 - The ``-m`` or ``--message`` flag still works
 - The path of the git repository does not require a flag and can simply have it path stated. If multiple paths are given, the first one thats a valid repository will be chosen. The program will explicitly fail if none where given.
```

### Comparing `gitautobackup-1.1.0.3/gitautobackup.py` & `gitautobackup-1.2.0.0/gitautobackup.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,22 +11,48 @@
     See the github repo for more info!
     
     This project is on github here:
     https://github.com/MarkusHammer/gitautobackup
 '''
 
 from pathlib import Path
-from git import Repo, InvalidGitRepositoryError, GitCommandNotFound, NoSuchPathError, RepositoryDirtyError
+from git import Repo, InvalidGitRepositoryError, GitCommandNotFound, NoSuchPathError, RepositoryDirtyError, GitError
 
 try:
     from typing import Union
 except ImportError:
     from typing_extensions import Union
 
-__version__ = "1.1.0.3"
+try:
+    from typing import List
+except ImportError:
+    from typing_extensions import List
+
+__version__ = "1.2.0.0"
+
+class InvalidArchiveFormatError(GitError, Exception):
+    """Raised when a format for git archive when that format is not a valid format for git archive"""    
+
+    def __init__(self, given_format:str, possible_formats:Union[List[str], None] = None):
+        """_summary_
+
+        Args:
+            format (str): The issue causing format.
+            repo_reference (Union[Repo, None], optional): A optional list of possible valid formats, or None if this cant be given.
+        """
+
+        self.given_format = given_format
+        self.possible_formats = []
+
+        if possible_formats is not None:
+            self.possible_formats = possible_formats
+
+    def __str__(self) -> str:
+        return f"The format {self.given_format} is not a valid format for a archive in git. {('Valid formats are ' + ' '.join(self.possible_formats)) if len(self.possible_formats) > 0 else ''}"
+
 
 def path_hunt_dir(path: Union[Path, str, None]) -> Union['Path', None]:
     """_summary_
 
     Args:
         path (Union[Path,str,None]): The path to search for the parent directory of. If this is set to None the return value will always also be None
 
@@ -156,44 +182,55 @@
             possiblepath = path_hunt_dir(__file__)
             if possiblepath is not None and possiblepath.exists():
                 return possiblepath
 
     return None
 
 
-def auto_git_backup(repo_path: Union[Path, None] = None,
+def auto_git_backup(repo_path: Union[Path, str, None] = None,
                     commit_message: Union[str, None] = None,
-                    further_guess_paths: bool = False, verbose: bool = True,
+                    further_guess_paths: bool = False,
+                    verbose: bool = True,
                     force_commit: bool = False,
-                    force_compress: Union[bool, None] = None
+                    tag:Union[str,None] = None,
+                    force_tag:bool = False,
+                    tag_message:Union[str, None] = None,
+                    force_compress: Union[bool, None] = None,
+                    compress_aggressive:bool = False,
+                    archive_path:Union[Path, str, None] = None,
+                    archive_format:Union[str, None] = None
                     ) -> bool:
     """_summary_
 
     Args:
         repo_path (Union[Path,None], optional): The path of the target git repository. If set to None and further_guess_paths is set there will be an attempts to determine this using ```get_default_file_location()```. Defaults to None.
         commit_message (Union[str,None], optional): The message of the commit being made. If None this will be automatically generated using ```default_commit_name()```. Defaults to None.
         further_guess_paths (bool, optional): If the path is set to none, should there be attempt to automatically guess the relevant path using ```get_default_file_location()```. Defaults to False.
-        verbose (bool, optional): SHould this function print out non error related messages? Defaults to True.
+        verbose (bool, optional): Should this function print out non error related messages? Defaults to True.
         force_commit (bool, optional): Should a commit be made even if there is nothing to be committed? Defaults to False.
+        tag (Union[str,None], optional): If a tag should be created, this should be the name of that tag. If no tag is to be made, this should be None, even if tag_force is True
+        force_tag (bool, optional): Create the new tag even if an old one already exists. No effect if tag is None.
+        tag_message (Union[str,None], optional): Add a message to the tag, or None if the tag should have no message. No effect if tag is None.
         force_compress (Union[bool, None], optional): Should (or shouldn't) the database be compressed despite it possibly being beneficial. True forces the database to be compressed, False forces the databest to not be compressed, and None allows for this to be automatically determined by git instead. Defaults to None.
+        compress_aggressive (bool, optional): If the repo is compressed, should it be done aggressively?
+        archive_path (Union[Path,None], optional): If set to None no archive will be made, otherwide a archive will be output to the given location.
+        archive_format (Union[str, None], optional): If set this will override the format of the archive being outputted, if set to None it will be inferred form the path.
 
     Raises:
         NOTE: This may not be a comprehensive list of all possible exceptions raised, as pathlib or git may raise various other exceptions as well, however what is stated below is the behaviour explicitly defined in raise statements.
         InvalidGitRepositoryError: Raised when the folder could not be opened as a git repo, if the path couldn't possibly be a git repo (if its not a directory and does not end with ".git"), or if it can be opened but it is a bare repo and allow_bare is False.
+        InvalidArchiveFormatError: Raised when the given archive format is not a valid format for git archive.
         NoSuchPathError: Raised when the path doesn't exist on the system.
 
     Returns:
         bool: Weather or not a commit was made.
     """
 
     made_a_backup: bool = False
 
-    if commit_message is None or commit_message.strip() == "":
-        commit_message = default_commit_name()
-
     if verbose:
         try:
             from pprint import pprint
         except ImportError:
             pprint = print
 
     if further_guess_paths and repo_path is None:
@@ -207,16 +244,23 @@
         raise NoSuchPathError()
     while not is_repo(repo_path) and len(repo_path.parents) > 0:
         repo_path = repo_path.parent
     assert_repo(repo_path)
 
     if verbose:
         print(f"Opening path as repo: {repo_path} {'and forcing a commit' if force_commit else ''}...")
+
     with Repo(repo_path) as repo:
 
+        if archive_path is not None and archive_format is not None:
+            valid_archive_formats = repo.git.archive("--list").split()
+            archive_format = archive_format.strip().lower()
+            if archive_format not in valid_archive_formats:
+                raise InvalidArchiveFormatError(archive_format, valid_archive_formats)
+
         if force_commit or repo.is_dirty(untracked_files=True):
             made_a_backup = True
 
             msg = repo.git.add("--all", "--ignore-errors")
             if verbose and msg != "":
                 pprint(msg)
 
@@ -224,26 +268,55 @@
                 pprint(repo.git.status("-s"))
 
             cmd_args = []
             if force_commit:
                 cmd_args.append("--allow-empty")
             if verbose:
                 cmd_args.append("--verbose")
+            if commit_message is None or commit_message.strip() == "":
+                commit_message = default_commit_name()
             msg = repo.git.commit(cmd_args, m=commit_message)
             if verbose and msg != "":
                 pprint(msg)
 
+            if tag is not None:
+                cmd_args = ["-a"]
+                cmd_kwargs = {}
+                if force_tag:
+                    cmd_args.append("-f")
+                if tag_message is not None:
+                    cmd_kwargs["m"] = tag_message
+                cmd_args.append(tag)
+                msg = repo.git.tag(cmd_args, **cmd_kwargs)
+                if verbose and msg != "":
+                    pprint(msg)
+
         if force_compress is None or force_compress is True:
             cmd_args = []
+            if compress_aggressive:
+                cmd_args.append("--aggressive")
             if force_compress is None:
                 cmd_args.append("--auto")
             msg = repo.git.gc(cmd_args)
             if verbose and msg != "":
                 pprint(msg)
 
+        if archive_path is not None:
+            archive_path = Path(archive_path)
+            cmd_args = []
+            cmd_kwargs = {"o": archive_path}
+            if verbose:
+                cmd_args.append("-v")
+            if archive_format is not None:
+                cmd_kwargs["format"] = archive_format
+            cmd_args.append("HEAD")
+            msg = repo.git.archive(cmd_args, **cmd_kwargs)
+            if verbose and msg != "":
+                pprint(msg)
+
     return made_a_backup
 
 
 def main(*args, prog_arg: Union[str, None] = None) -> bool:
     """A function that when used as a module acts as the main entry point of the program. This allows for you to use this as you would normally via the cli but still import this as a module.
     Please note however that argv is only intended for the cli arguments and not for the name of the script running this, thats what the optional prog_arg argument is intended for.
     Also note that this function does not handle exceptions unlike how the cli turns these into user friendly messages. This is intended as the user of a module will most likely find these exceptions usefull.
@@ -254,39 +327,64 @@
 
     Returns:
         bool: weather or not a backup was made by ```auto_git_backup```
     """
 
     path = None
     force_commit = False
+    force_tag = False
     force_compress = None
-    message = None
+    compress_aggressive = False
+    commit_message = None
+    tag = None
+    tag_message = None
     verbose = True
     further_guess_paths = True
+    archive_path = None
+    archive_format = None
 
     # parse the cli args
     try:
         from argparse import ArgumentParser
-        parser = ArgumentParser(
-            prog=prog_arg, description='A basic CLI program that allows for quick formatting of a .gitignore file')
+        parser = ArgumentParser(prog=prog_arg,
+                                description="""
+                                A basic CLI program that allows for quick formatting of a .gitignore file
+                                """)
 
         parser.add_argument('-p', '--path', '-d', '--dest', '-r', '--repo',
-                            dest='repo_path', action='store', default=None, type=str,
+                            dest='repo_path', action='store', default=path, type=str,
                             help='The location of the git repo')
         parser.add_argument('-m', '--message', '-b', '--body', '-c', '--cm', '--commit_message', '-n', '--name', '--cn', '--commit_name',
-                            dest='message', action='store', default=message, type=str,
+                            dest='commit_message', action='store', default=commit_message, type=str,
                             help="The message of the commit. Note that this defaults to the message of the form 'Autosave at DATE TIME HERE' not to None as it might say")
+        parser.add_argument('-t', '--tag', '--commit_tag', '--tn', '--tag_name',
+                            dest='tag', action='store', default=tag, type=str,
+                            help="Assign a tag of the specified name to the commit. If this flag is not used no tag will be made.")
+        parser.add_argument('--tm', '--tag_message', '--tm', '--tag_message',
+                            dest='tag_message', action='store', default=tag_message, type=str,
+                            help="Set a message for the tag of this commit. Only effective if the tag flag is also used, otherwise there is no effect.")
+
+        parser.add_argument('-a', '--archive', '--ap', '--archive_path',
+                            dest='archive_path', action='store', default=archive_path, type=str,
+                            help="A path to the location of the desired archive to be made. If not defined no archive will be made.")
+        parser.add_argument('--af', '--archive_format',
+                            dest='archive_format', action='store', default=archive_format, type=str,
+                            help="Force the given type of format to be used for the file. If not defined it will be taken from the given path.")
 
-        parser.add_argument('-f', '--force', '--forcecommit', dest='force_commit', action='store_true', default=force_commit,
+        parser.add_argument('-f', '--force', '--force_commit', dest='force_commit', action='store_true', default=force_commit,
                             help='Push a commit to the repo even if there are no changes')
+        parser.add_argument('--ft', '--force_tag', dest='force_tag', action='store_true', default=force_tag,
+                            help='If a tag is to be made, force it to overwrite any existing tags that may be in it`s way')
         force_compress_group = parser.add_mutually_exclusive_group()
-        force_compress_group.add_argument('--fc', '--forcecompress', dest='force_compress', action='store_true',
-                                          help='Compress the database even if its not quite necessary')
-        force_compress_group.add_argument('--fnc', '--forcenocompress', dest='force_no_compress', action='store_true',
+        force_compress_group.add_argument('--fnc', '--force_no_compress', dest='force_no_compress', action='store_true',
                                           help='Skip compressing the database even if it might be usefull')
+        force_compress_group.add_argument('--fc', '--force_compress', dest='force_compress', action='store_true',
+                                          help='Compress the database even if its not quite necessary')
+        force_compress_group.add_argument('--fca', '--force_compress_aggressive', dest='force_compress_aggressive', action='store_true',
+                                          help='Compress the database aggressively, even if its not quite necessary')
 
         loudness_group = parser.add_mutually_exclusive_group()
         loudness_group.add_argument("-v", "--verbose", dest="verbose",
                                     action="store_true", help="Print a verbose output of the process")
         loudness_group.add_argument("-q", "--quiet", dest="quiet", action="store_true",
                                     help="Avoid printing anything to the terminal if possible")
 
@@ -297,38 +395,54 @@
                             help="Give a link to the github repo page", version="https://github.com/MarkusHammer/gitautobackup")
 
         args = parser.parse_args(*args)
         path = args.repo_path
         if path is not None:
             path = path.strip("'").strip('"')
         force_commit = args.force_commit
+        force_tag = args.force_tag
         if args.force_compress:
             force_compress = True
         elif args.force_no_compress:
             force_compress = False
+        elif args.force_compress_aggressive:
+            force_compress = True
+            compress_aggressive = True
         else:
             force_compress = None
-        message = args.message
-        if message is not None:
-            message = message.strip("'").strip('"')
+        commit_message = args.commit_message
+        if commit_message is not None:
+            commit_message = commit_message.strip("'").strip('"')
+        tag = args.tag
+        if tag is not None:
+            tag = tag.strip("'").strip('"')
+        tag_message = args.tag_message
+        if tag_message is not None:
+            tag_message = tag_message.strip("'").strip('"')
+        archive_path = args.archive_path
+        if archive_path is not None:
+            archive_path = archive_path.strip("'").strip('"')
+        archive_format = args.archive_format
+        if archive_format is not None:
+            archive_format = archive_format.strip("'").strip('"')
 
         if args.verbose:
             verbose = True
         elif args.quiet:
             verbose = False
     except ImportError:
         print("Argparse could not be loaded/found, please note that this will mean that explicitly specifying the path form the cli is required and all other cli arguments are not available")
         further_guess_paths = False
 
         next_is_message = False
         for arglet in args:
             arglet = arglet.strip().strip('"')
 
             if next_is_message:
-                message = arglet
+                commit_message = arglet
 
             if arglet.lower() == "-p" or arglet.lower() == "--path":
                 continue
 
             if arglet.lower() == "-h" or arglet.lower() == "--help":
                 print(f"You are running {prog_arg[0]}")
                 print(
@@ -349,34 +463,38 @@
             print("No valid repository path was found")
             return False
         verbose = True
 
     if args.verbose:
         print("Making auto backup")
 
-    return auto_git_backup(path, commit_message=message, further_guess_paths=further_guess_paths, verbose=verbose, force_commit=force_commit, force_compress=force_compress)
+    return auto_git_backup(path, commit_message=commit_message, further_guess_paths=further_guess_paths, verbose=verbose, force_commit=force_commit, tag = tag, tag_message = tag_message, force_tag = force_tag, force_compress=force_compress, compress_aggressive = compress_aggressive, archive_path = archive_path, archive_format = archive_format)
 
 
 def __main__():
     from sys import (exit as end, argv)
 
     scode = -1
 
     try:
-        scode = 0 if main(argv[1:], prog_arg=argv[0]) else 1
+        scode = 0 if main(argv[1:], prog_arg=argv[0]) else 1 #1 means not error but also no changes, 0 is no error and changes where made
     except GitCommandNotFound:
         print("Your system is not set up properly for use with the GitPython module. Please refer to it's documentation for setting it up before running this script.")
+        scode = -2
     except (NoSuchPathError, FileNotFoundError, PermissionError):
         print("The given path does not exist on this system or could not be accessed by this user.")
-        scode = -2
+        scode = -3
     except InvalidGitRepositoryError:
         print("The folder given is not a git repo, or is bare.")
-        scode = -3
+        scode = -4
     except RepositoryDirtyError:
         print("The repository already has some changes that could end up being overwritten. Please Handle these first before running this.")
-        scode = -4
+        scode = -5
+    except InvalidArchiveFormatError as exc:
+        print(str(exc))
+        scode = -6
 
     end(scode)
 
 
 if __name__ == "__main__":
     __main__()
```

### Comparing `gitautobackup-1.1.0.3/pyproject.toml` & `gitautobackup-1.2.0.0/pyproject.toml`

 * *Files identical despite different names*

