# Comparing `tmp/sbo-create-2.0.4.tar.gz` & `tmp/sbo-create-2.0.5.tar.gz`

## Comparing `sbo-create-2.0.4.tar` & `sbo-create-2.0.5.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-10 10:05:03.000000 sbo-create-2.0.4/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/
--rw-r--r--   0 dslackw   (1000) users      (100)     6461 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/cmake-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)     6816 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/autotools-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)      521 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/template.info
--rw-r--r--   0 dslackw   (1000) users      (100)     6786 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/meson-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)     1047 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)     6138 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/rubygem-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)     6018 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/haskell-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)     5992 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/perl-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)     1803 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      683 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/README
--rw-r--r--   0 dslackw   (1000) users      (100)     5514 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_scripts_templates/python-template.SlackBuild
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-10 10:04:59.000000 sbo-create-2.0.4/sbo_create.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-02-10 10:04:59.000000 sbo-create-2.0.4/sbo_create.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-02-10 10:04:59.000000 sbo-create-2.0.4/sbo_create.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       11 2023-02-10 10:04:59.000000 sbo-create-2.0.4/sbo_create.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-02-10 10:04:59.000000 sbo-create-2.0.4/sbo_create.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     3018 2023-02-10 10:04:59.000000 sbo-create-2.0.4/sbo_create.egg-info/PKG-INFO
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-01 20:57:05.000000 sbo-create-2.0.4/slackbuild/
--rwxr-xr-x   0 dslackw   (1000) users      (100)     3078 2023-02-01 20:57:05.000000 sbo-create-2.0.4/slackbuild/sbo-create.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)      802 2023-02-01 20:57:05.000000 sbo-create-2.0.4/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      129 2023-02-01 20:57:05.000000 sbo-create-2.0.4/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-02-01 20:57:05.000000 sbo-create-2.0.4/slackbuild/README
--rw-r--r--   0 dslackw   (1000) users      (100)      316 2023-02-01 20:57:05.000000 sbo-create-2.0.4/slackbuild/sbo-create.info
--rwxr-xr-x   0 dslackw   (1000) users      (100)      945 2023-02-01 20:57:05.000000 sbo-create-2.0.4/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2465 2023-02-01 20:57:05.000000 sbo-create-2.0.4/README.rst
--rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-02-01 20:57:05.000000 sbo-create-2.0.4/requirements.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-02-01 20:57:05.000000 sbo-create-2.0.4/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1770 2023-02-01 20:57:05.000000 sbo-create-2.0.4/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)     2300 2023-02-01 20:57:05.000000 sbo-create-2.0.4/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-10 10:04:59.000000 sbo-create-2.0.4/sbo_create/
--rw-r--r--   0 dslackw   (1000) users      (100)    29050 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_create/templates.py
--rw-r--r--   0 dslackw   (1000) users      (100)      311 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_create/__metadata__.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-10 10:04:59.000000 sbo-create-2.0.4/sbo_create/__pycache__/
--rw-r--r--   0 dslackw   (1000) users      (100)      154 2023-02-10 10:04:59.000000 sbo-create-2.0.4/sbo_create/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)      444 2023-02-10 10:04:59.000000 sbo-create-2.0.4/sbo_create/__pycache__/__metadata__.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_create/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)    39658 2023-02-01 20:57:05.000000 sbo-create-2.0.4/sbo_create/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)       81 2023-02-01 20:57:05.000000 sbo-create-2.0.4/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-01 20:57:05.000000 sbo-create-2.0.4/bin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      233 2023-02-01 20:57:05.000000 sbo-create-2.0.4/bin/sbo-create
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:43:00.000000 sbo-create-2.0.5/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6461 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/cmake-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)     6816 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/autotools-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)      521 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/template.info
+-rw-r--r--   0 dslackw   (1000) users      (100)     6786 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/meson-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)     1047 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)     6138 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/rubygem-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)     6018 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/haskell-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)     5992 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/perl-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)     1803 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      683 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     5514 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/python-template.SlackBuild
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-06-06 17:42:54.000000 sbo-create-2.0.5/sbo_create.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       11 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     3936 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create.egg-info/PKG-INFO
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     3078 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/sbo-create.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)      802 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      129 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/README
+-rw-r--r--   0 dslackw   (1000) users      (100)      316 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/sbo-create.info
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      945 2023-06-06 17:42:34.000000 sbo-create-2.0.5/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3388 2023-06-06 17:42:34.000000 sbo-create-2.0.5/README.rst
+-rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-06-06 17:42:34.000000 sbo-create-2.0.5/requirements.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-06-06 17:42:34.000000 sbo-create-2.0.5/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1765 2023-06-06 17:42:34.000000 sbo-create-2.0.5/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)     2422 2023-06-06 17:42:34.000000 sbo-create-2.0.5/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create/
+-rw-r--r--   0 dslackw   (1000) users      (100)    30138 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_create/templates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      350 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_create/__metadata__.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create/__pycache__/
+-rw-r--r--   0 dslackw   (1000) users      (100)      154 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)      580 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create/__pycache__/__metadata__.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_create/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    44512 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_create/main.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:34.000000 sbo-create-2.0.5/bin/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      238 2023-06-06 17:42:34.000000 sbo-create-2.0.5/bin/sbo-create
```

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/cmake-template.SlackBuild` & `sbo-create-2.0.5/sbo_scripts_templates/cmake-template.SlackBuild`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/autotools-template.SlackBuild` & `sbo-create-2.0.5/sbo_scripts_templates/autotools-template.SlackBuild`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/template.info` & `sbo-create-2.0.5/sbo_scripts_templates/template.info`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/meson-template.SlackBuild` & `sbo-create-2.0.5/sbo_scripts_templates/meson-template.SlackBuild`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/slack-desc` & `sbo-create-2.0.5/sbo_scripts_templates/slack-desc`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/rubygem-template.SlackBuild` & `sbo-create-2.0.5/sbo_scripts_templates/rubygem-template.SlackBuild`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/haskell-template.SlackBuild` & `sbo-create-2.0.5/sbo_scripts_templates/haskell-template.SlackBuild`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/perl-template.SlackBuild` & `sbo-create-2.0.5/sbo_scripts_templates/perl-template.SlackBuild`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/doinst.sh` & `sbo-create-2.0.5/sbo_scripts_templates/doinst.sh`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/README` & `sbo-create-2.0.5/sbo_scripts_templates/README`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/sbo_scripts_templates/python-template.SlackBuild` & `sbo-create-2.0.5/sbo_scripts_templates/python-template.SlackBuild`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/slackbuild/sbo-create.SlackBuild` & `sbo-create-2.0.5/slackbuild/sbo-create.SlackBuild`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/slackbuild/slack-desc` & `sbo-create-2.0.5/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/setup.py` & `sbo-create-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/README.rst` & `sbo-create-2.0.5/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 .. contents:: Table of Contents:
 
 
 About
 -----
 
-sbo-create it's a tool that creates easy, fast and safe SlackBuilds files scripts.
+sbo-create, it's a tool that creates easy, fast and safe SlackBuilds files scripts.
 
-This tool is for everyone, but package maintainers will be going to love it!
+This tool is for everyone, but maintainers will be going to love it!
 
 Enjoy!
 
 
 Features
 ________
 
 - Preloaded SlackBuilds templates.
 - Checking for already SlackBuilds in the repository and the distribution.
 - Autocorrect the quote marks for the .info file.
 - Auto-importing the SlackBuild script name.
-- Auto-importing the description project from the slack-desc file.
+- Auto-importing the text from the slack-desc file into the README.
 - Auto-importing the maintainer data to the .SlackBuild script.
 - Auto-importing the version to the .SlackBuild script.
 - Auto-importing and checking the checksum signature to the .info file.
 
 
 Screenshot
 __________
@@ -39,64 +39,84 @@
 
 
 Install
 -------
 
 .. code-block:: bash
 
-    $ tar xvf sbo-create-2.0.4.tar.gz
-    $ cd sbo-create-2.0.4
+    $ tar xvf sbo-create-2.0.5.tar.gz
+    $ cd sbo-create-2.0.5
     $ ./install.sh
 
     or
 
     $ slpkg install sbo-create
 
 
 Requirements
 ------------
 
-- Requires Python 3.9+
-
 - python3-pythondialog >= 3.5.3
 
 
 Usage
 -----
 
 .. code-block:: bash
 
-    Usage: sbo-create <sbo_name>
+    Usage: sbo-create [OPTIONS]
 
     Optional arguments:
-      -h, --help           Display this message and exit.
-      -v, --version        Show version and exit.
-
+      -n, --prgnam NAME          Set the name of the SlackBuild.
+      -e, --prg-version VERSION  Set the version of the SlackBuild.
+      -t, --template TEMPLATE    Set the SlackBuild template:
+                                 templates={autotools, cmake, perl, python,
+                                            rubygem, haskell, meson}
+      -f, --create-files         Creates the necessary files and exit:
+                                 files={<prgnam>.SlackBuild, <prgnam>.info,
+                                        README, slack-desc}.
+      -m, --maintainer           Edit the maintainer file.
+      -d, --download             Download source files listed in the .info file.
+      -c, --check NAME           Check if the SBo exist in the repository.
+      -h, --help                 Display this message and exit.
+      -v, --version              Show version and exit.
 
 For a new project, you should create at first a new folder with the same name as
 the project.
 For an existing project, come into the folder and start to edit, just run `sbo-create`.
 
+Alternative you can run the below command to create all the necessary files:
+
+.. code-block:: bash
+
+    $ sbo-create --prgnam sboname --prg-version 1.0.0 --template python --create-files
+    Files created:
+
+      > slack-desc
+      > sboname.info
+      > README
+      > sboname.slackbuild
+
+
 It's good you know before you start, please visit here: `HOWTO <https://slackbuilds.org/howto/>`_
 
 
 Note
 ----
-The :code:`sbo-create` tool checks before you create a slackbuild and if the package exists in your distribution that
-you have installed, you get a warning message before you proceed.
+The :code:`sbo-create` tool, checks for installed SlackBuilds.
 
 
 Donate
 ------
 
-If you feel satisfied with this project and want to thanks me make a donation.
+If you feel satisfied with this project and want to thank me, treat me to a coffee ☕ !
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/donate/paypaldonate.png
    :target: https://www.paypal.me/dslackw
 
 
 Copyright 
 ---------
 
-- Copyright © 2015-2022 Dimitris Zlatanidis
+- Copyright © 2015-2023 Dimitris Zlatanidis
 - Slackware ® is a Registered Trademark of Patrick Volkerding.
 - Linux is a Registered Trademark of Linus Torvalds.
```

### Comparing `sbo-create-2.0.4/LICENSE` & `sbo-create-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.4/install.sh` & `sbo-create-2.0.5/install.sh`

 * *Files 7% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 #  WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 #  OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 #  ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 __version() {
 # Grab version from __metadata__.py file
-cat sbo_create/__metadata__.py | grep "__version_info__ = (" \
-    | tr -d "[:space:]" | cut -c19-23 | tr , .
+cat sbo_create/__metadata__.py | grep "__version_info__: tuple = (" \
+    | tr -d "[:space:]" | cut -c25-29 | tr , .
 }
 
 PRGNAM=sbo-create
 VERSION=${VERSION:-$(__version)} 
 TAG=${TAG:-_dsw}
 
-ARCHIVES="$PRGNAM-$VERSION.tar.gz $PRGNAM-$VERSION.zip \
-    v$VERSION.tar.gz v$VERSION.zip"
+ARCHIVES="$PRGNAM-$VERSION.tar.gz $PRGNAM-$VERSION.tar.bz2 $PRGNAM-$VERSION.zip"
 cd ..
 for file in $ARCHIVES; do
     if [ -f $file ]; then
         cp $file $PRGNAM-$VERSION/slackbuild
         cd $PRGNAM-$VERSION/slackbuild
         chmod +x $PRGNAM.SlackBuild
         ./$PRGNAM.SlackBuild
```

### Comparing `sbo-create-2.0.4/ChangeLog.txt` & `sbo-create-2.0.5/ChangeLog.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2.0.5 - 04/06/2023
+Updated:
+- Improved code quality
+Fixed:
+- Checksum in the .info file
+Added:
+- Options to the cli menu
+
 2.0.4 - 31/01/2023
 Fixed:
 - IndexError: list index out of range #1
 
 2.0.3 - 29/12/2022
 Fixed:
 - SlackBuild script (Thanks to A.Rozell) !1
```

### Comparing `sbo-create-2.0.4/sbo_create/templates.py` & `sbo-create-2.0.5/sbo_create/templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 
-bg = "\x1b[48;5;4m"
-fg = "\x1b[38;5;7m"
-cl = bg + fg
+def doinst_template():
+    bg = "\x1b[48;5;4m"
+    fg = "\x1b[38;5;7m"
+    cl = f"{bg}{fg}"
 
-doinst = """
+    template: str = """
 %s################################################################################
 %s#             COPY A TEMPLATE AND PASTE IT INTO THE TEXT EDITOR                #
 %s#                          PRESS \"q or Q\" TO EXIT                              #
 %s################################################################################
 
 config() {
   NEW="$1"
@@ -74,23 +75,63 @@
 
 if [ -x /usr/bin/install-info ]; then
   chroot . /usr/bin/install-info --info-dir=/usr/info /usr/info/blah.gz 2> /dev/null
 fi
 
 %s################################################################################
 """ % (cl, cl, cl, cl, cl)
+    return template
+
+
+def slack_desc_template(name: str) -> str:
+    if not name:
+        name: str = f"{'None':4}"
+    template: str = f"""# HOW TO EDIT THIS FILE:
+# The "handy ruler" below makes it easier to edit a package description.
+# Line up the first '|' above the ':' following the base package name, and
+# the '|' on the right side marks the last column you can put a character in.
+# You must make exactly 11 lines for the formatting to be correct.  It's also
+# customary to leave one space after the ':' except on otherwise blank lines.
+
+{' ':{len(name)}}|-----handy-ruler------------------------------------------------------|
+{name}: {name} (short description of app)
+{name}:
+{name}:
+{name}:
+{name}:
+{name}:
+{name}:
+{name}:
+{name}:
+{name}:
+{name}:"""
+    return template
+
+
+def info_template(name: str, version: str, maintainer: str, email: str) -> str:
+    template: str = f'''PRGNAM="{name}"
+VERSION="{version}"
+HOMEPAGE=""
+DOWNLOAD=""
+MD5SUM=""
+DOWNLOAD_x86_64=""
+MD5SUM_x86_64=""
+REQUIRES=""
+MAINTAINER="{maintainer}"
+EMAIL="{email}"'''
+    return template
 
 
 class SlackBuilds(object):
 
-    def __init__(self, app_name, version, year, maint_name, live):
+    def __init__(self, app_name, version, year, maintainer, live):
         self.app_name = app_name
         self.version = version
         self.year = year
-        self.maint_name = maint_name
+        self.maintainer = maintainer
         self.live = live
 
     def autotools(self):
 
         autotools_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -208,16 +249,16 @@
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maint_name, self.live, self.app_name,
-            self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
+       self.version)
         return autotools_template
 
     def cmake(self):
 
         cmake_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -331,16 +372,16 @@
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maint_name, self.live, self.app_name,
-            self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
+       self.version)
         return cmake_template
 
     def perl(self):
 
         perl_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -460,16 +501,16 @@
 cat $CWD/$PRGNAM.SlackBuild > $PKG/usr/doc/$PRGNAM-$VERSION/$PRGNAM.SlackBuild
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maint_name, self.live, self.app_name,
-            self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
+       self.version)
         return perl_template
 
     def python(self):
 
         python_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -569,16 +610,16 @@
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maint_name, self.live, self.app_name,
-            self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
+       self.version)
         return python_template
 
     def rubygem(self):
 
         rubygem_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -703,16 +744,16 @@
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maint_name, self.live, self.app_name,
-            self.version, "%s", "%s", "%s", "%s", "%s", "%s")
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
+       self.version, "%s", "%s", "%s", "%s", "%s", "%s")
         return rubygem_template
 
 
     def haskell(self):
 
         haskell_template = """#!/bin/bash
 
@@ -828,16 +869,16 @@
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maint_name, self.live, self.app_name,
-           self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
+       self.version)
         return haskell_template
 
     def meson(self):
 
         autotools_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -959,10 +1000,10 @@
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maint_name, self.live, self.app_name,
-            self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
+       self.version)
         return autotools_template
```

