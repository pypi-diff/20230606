# Comparing `tmp/git-sim-0.3.0.tar.gz` & `tmp/git-sim-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-sim-0.3.0.tar", last modified: Sat Apr 22 16:23:30 2023, max compression
+gzip compressed data, was "git-sim-0.3.1.tar", last modified: Tue Jun  6 18:46:27 2023, max compression
```

## Comparing `git-sim-0.3.0.tar` & `git-sim-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 16:23:30.907142 git-sim-0.3.0/
--rw-rw-rw-   0        0        0    18431 2023-03-09 07:57:29.000000 git-sim-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       26 2023-03-09 07:57:17.000000 git-sim-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0    25467 2023-04-22 16:23:30.907142 git-sim-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    24660 2023-04-21 21:10:02.000000 git-sim-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 16:23:30.894185 git-sim-0.3.0/git_sim/
--rw-rw-rw-   0        0        0       23 2023-04-22 16:22:56.000000 git-sim-0.3.0/git_sim/__init__.py
--rw-rw-rw-   0        0        0     8333 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/__main__.py
--rw-rw-rw-   0        0        0     2852 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/add.py
--rw-rw-rw-   0        0        0     3680 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/animations.py
--rw-rw-rw-   0        0        0     1511 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/branch.py
--rw-rw-rw-   0        0        0     4415 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/checkout.py
--rw-rw-rw-   0        0        0     2302 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/cherrypick.py
--rw-rw-rw-   0        0        0     3921 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/clean.py
--rw-rw-rw-   0        0        0     2974 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/clone.py
--rw-rw-rw-   0        0        0     8586 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/commands.py
--rw-rw-rw-   0        0        0     3175 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/commit.py
--rw-rw-rw-   0        0        0      572 2023-04-21 21:10:02.000000 git-sim-0.3.0/git_sim/enums.py
--rw-rw-rw-   0        0        0     2842 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/fetch.py
--rw-rw-rw-   0        0        0    46789 2023-04-21 21:10:02.000000 git-sim-0.3.0/git_sim/git_sim_base_command.py
--rw-rw-rw-   0        0        0     1415 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/log.py
--rw-rw-rw-   0        0        0    63319 2023-03-09 07:57:17.000000 git-sim-0.3.0/git_sim/logo.png
--rw-rw-rw-   0        0        0     7251 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/merge.py
--rw-rw-rw-   0        0        0     2937 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/mv.py
--rw-rw-rw-   0        0        0     3844 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/pull.py
--rw-rw-rw-   0        0        0     7226 2023-04-21 21:10:02.000000 git-sim-0.3.0/git_sim/push.py
--rw-rw-rw-   0        0        0     6057 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/rebase.py
--rw-rw-rw-   0        0        0     5042 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/reset.py
--rw-rw-rw-   0        0        0     2467 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/restore.py
--rw-rw-rw-   0        0        0     5607 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/revert.py
--rw-rw-rw-   0        0        0     4541 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/rm.py
--rw-rw-rw-   0        0        0     1380 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/settings.py
--rw-rw-rw-   0        0        0     6505 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/stash.py
--rw-rw-rw-   0        0        0      829 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/status.py
--rw-rw-rw-   0        0        0     4413 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/switch.py
--rw-rw-rw-   0        0        0     1469 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/tag.py
-drwxrwxrwx   0        0        0        0 2023-04-22 16:23:30.906145 git-sim-0.3.0/git_sim.egg-info/
--rw-rw-rw-   0        0        0    25467 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      770 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 16:23:30.907142 git-sim-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1468 2023-04-21 20:23:21.000000 git-sim-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:46:27.922754 git-sim-0.3.1/
+-rw-rw-rw-   0        0        0    18431 2023-03-09 07:57:29.000000 git-sim-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-03-09 07:57:17.000000 git-sim-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    25490 2023-06-06 18:46:27.922754 git-sim-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    24683 2023-06-06 18:44:43.000000 git-sim-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 18:46:27.914290 git-sim-0.3.1/git_sim/
+-rw-rw-rw-   0        0        0       23 2023-06-06 18:44:43.000000 git-sim-0.3.1/git_sim/__init__.py
+-rw-rw-rw-   0        0        0     8333 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/__main__.py
+-rw-rw-rw-   0        0        0     2852 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/add.py
+-rw-rw-rw-   0        0        0     3680 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/animations.py
+-rw-rw-rw-   0        0        0     1511 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/branch.py
+-rw-rw-rw-   0        0        0     4415 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/checkout.py
+-rw-rw-rw-   0        0        0     2302 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/cherrypick.py
+-rw-rw-rw-   0        0        0     3921 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/clean.py
+-rw-rw-rw-   0        0        0     2974 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/clone.py
+-rw-rw-rw-   0        0        0     8586 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/commands.py
+-rw-rw-rw-   0        0        0     3175 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/commit.py
+-rw-rw-rw-   0        0        0      572 2023-04-21 21:10:02.000000 git-sim-0.3.1/git_sim/enums.py
+-rw-rw-rw-   0        0        0     2842 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/fetch.py
+-rw-rw-rw-   0        0        0    46330 2023-06-06 18:44:43.000000 git-sim-0.3.1/git_sim/git_sim_base_command.py
+-rw-rw-rw-   0        0        0     1415 2023-06-06 18:37:54.000000 git-sim-0.3.1/git_sim/log.py
+-rw-rw-rw-   0        0        0    63319 2023-03-09 07:57:17.000000 git-sim-0.3.1/git_sim/logo.png
+-rw-rw-rw-   0        0        0     7251 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/merge.py
+-rw-rw-rw-   0        0        0     2937 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/mv.py
+-rw-rw-rw-   0        0        0     3844 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/pull.py
+-rw-rw-rw-   0        0        0     7226 2023-04-21 21:10:02.000000 git-sim-0.3.1/git_sim/push.py
+-rw-rw-rw-   0        0        0     6057 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/rebase.py
+-rw-rw-rw-   0        0        0     5042 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/reset.py
+-rw-rw-rw-   0        0        0     2467 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/restore.py
+-rw-rw-rw-   0        0        0     5607 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/revert.py
+-rw-rw-rw-   0        0        0     4541 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/rm.py
+-rw-rw-rw-   0        0        0     1380 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/settings.py
+-rw-rw-rw-   0        0        0     6505 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/stash.py
+-rw-rw-rw-   0        0        0      829 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/status.py
+-rw-rw-rw-   0        0        0     4413 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/switch.py
+-rw-rw-rw-   0        0        0     1469 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/tag.py
+drwxrwxrwx   0        0        0        0 2023-06-06 18:46:27.921754 git-sim-0.3.1/git_sim.egg-info/
+-rw-rw-rw-   0        0        0    25490 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 18:46:27.922754 git-sim-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2023-04-21 20:23:21.000000 git-sim-0.3.1/setup.py
```

### Comparing `git-sim-0.3.0/LICENSE` & `git-sim-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/PKG-INFO` & `git-sim-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-sim
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
 Home-page: https://initialcommit.com/tools/git-sim
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-sim
 Project-URL: Source, https://github.com/initialcommit-com/git-sim
 Keywords: git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run
@@ -27,31 +27,31 @@
 Visually simulate Git operations in your own repos with a single terminal command.
 
 This generates an image (default) or video visualization depicting the Git command's behavior.
 
 Command syntax is based directly on Git's command-line syntax, so using git-sim is as familiar as possible.
 
 Example: `$ git-sim merge <branch>`
-
-![git-sim-merge_01-05-23_09-44-46](https://user-images.githubusercontent.com/49353917/210939840-1d51493a-6cac-43fd-9d12-3d2948d32c61.jpg)
+<br/><br/>
+![git-sim-merge_04-22-23_21-04-32_cropped](https://user-images.githubusercontent.com/49353917/233821875-a7bb640d-10be-4433-a8fb-bd25646eeff4.jpg)
 
 ## Use cases
 - Visualize Git commands to understand their effects on your repo before actually running them
 - Prevent unexpected working directory and repository states by simulating before running
 - Share visualizations (jpg/png image or mp4/webm video) of your Git commands with your team, or the world
 - Save visualizations as a part of your team documentation to document workflow and prevent recurring issues
 - Create static Git diagrams (jpg/png) or dynamic animated videos (mp4/webm) to speed up content creation
 - Help visual learners understand how Git commands work
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 
 ## Features
 - Run a one-liner git-sim command in the terminal to generate a custom Git command visualization (.jpg) from your repo
 - Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`, `rm`, `mv`, `clean`
 - Generate an animated video (.mp4) instead of a static image using the `--animate` flag (note: significant performance slowdown, it is recommended to use `--low-quality` to speed up testing and remove when ready to generate presentation-quality video)
-- Color commits by parameter, such as author the `--color-by=author` option
+- Color commits by parameter, such as author with the `--color-by=author` option
 - Choose between dark mode (default) and light mode
 - Specify output formats of either jpg, png, mp4, or webm
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 - Animation only: Add custom branded intro/outro sequences if desired
 - Animation only: Speed up or slow down animation speed as desired
 
 ## Quickstart
```

### Comparing `git-sim-0.3.0/README.md` & `git-sim-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 Visually simulate Git operations in your own repos with a single terminal command.
 
 This generates an image (default) or video visualization depicting the Git command's behavior.
 
 Command syntax is based directly on Git's command-line syntax, so using git-sim is as familiar as possible.
 
 Example: `$ git-sim merge <branch>`
-
-![git-sim-merge_01-05-23_09-44-46](https://user-images.githubusercontent.com/49353917/210939840-1d51493a-6cac-43fd-9d12-3d2948d32c61.jpg)
+<br/><br/>
+![git-sim-merge_04-22-23_21-04-32_cropped](https://user-images.githubusercontent.com/49353917/233821875-a7bb640d-10be-4433-a8fb-bd25646eeff4.jpg)
 
 ## Use cases
 - Visualize Git commands to understand their effects on your repo before actually running them
 - Prevent unexpected working directory and repository states by simulating before running
 - Share visualizations (jpg/png image or mp4/webm video) of your Git commands with your team, or the world
 - Save visualizations as a part of your team documentation to document workflow and prevent recurring issues
 - Create static Git diagrams (jpg/png) or dynamic animated videos (mp4/webm) to speed up content creation
 - Help visual learners understand how Git commands work
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 
 ## Features
 - Run a one-liner git-sim command in the terminal to generate a custom Git command visualization (.jpg) from your repo
 - Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`, `rm`, `mv`, `clean`
 - Generate an animated video (.mp4) instead of a static image using the `--animate` flag (note: significant performance slowdown, it is recommended to use `--low-quality` to speed up testing and remove when ready to generate presentation-quality video)
-- Color commits by parameter, such as author the `--color-by=author` option
+- Color commits by parameter, such as author with the `--color-by=author` option
 - Choose between dark mode (default) and light mode
 - Specify output formats of either jpg, png, mp4, or webm
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 - Animation only: Add custom branded intro/outro sequences if desired
 - Animation only: Speed up or slow down animation speed as desired
 
 ## Quickstart
```

### Comparing `git-sim-0.3.0/git_sim/__main__.py` & `git-sim-0.3.1/git_sim/__main__.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/add.py` & `git-sim-0.3.1/git_sim/add.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/animations.py` & `git-sim-0.3.1/git_sim/animations.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/branch.py` & `git-sim-0.3.1/git_sim/branch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/checkout.py` & `git-sim-0.3.1/git_sim/checkout.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/cherrypick.py` & `git-sim-0.3.1/git_sim/cherrypick.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/clean.py` & `git-sim-0.3.1/git_sim/clean.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/clone.py` & `git-sim-0.3.1/git_sim/clone.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/commands.py` & `git-sim-0.3.1/git_sim/commands.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/commit.py` & `git-sim-0.3.1/git_sim/commit.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/enums.py` & `git-sim-0.3.1/git_sim/enums.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/fetch.py` & `git-sim-0.3.1/git_sim/fetch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/git_sim_base_command.py` & `git-sim-0.3.1/git_sim/git_sim_base_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,25 +463,25 @@
         )
 
         for selected_branch in self.selected_branches:
             branches.insert(0, branches.pop(branches.index(selected_branch)))
 
         for branch in branches:
             if (
-                not self.is_remote_tracking_branch(branch)  # local branch
+                branch not in remote_tracking_branches # local branch
                 and commit.hexsha == self.repo.heads[branch].commit.hexsha
             ) or (
-                self.is_remote_tracking_branch(branch)  # remote tracking branch
+                branch in remote_tracking_branches # remote tracking branch
                 and commit.hexsha == remote_tracking_branches[branch]
             ):
                 text = (
                     (make_branches_remote + "/" + branch)
                     if (
                         make_branches_remote
-                        and not self.is_remote_tracking_branch(branch)
+                        and branch not in remote_tracking_branches 
                     )
                     else branch
                 )
 
                 branchText = m.Text(
                     text,
                     font="Monospace",
@@ -1174,23 +1174,14 @@
         remote_tracking_branches = {}
         for reflist in remote_refs:
             for ref in reflist:
                 if "HEAD" not in ref.name and ref.name not in remote_tracking_branches:
                     remote_tracking_branches[ref.name] = ref.commit.hexsha
         return remote_tracking_branches
 
-    def is_remote_tracking_branch(self, branch):
-        remote_refs = [remote.refs for remote in self.repo.remotes]
-        remote_tracking_branches = {}
-        for reflist in remote_refs:
-            for ref in reflist:
-                if "HEAD" not in ref.name and ref.name not in remote_tracking_branches:
-                    remote_tracking_branches[ref.name] = ref.commit.hexsha
-        return branch in remote_tracking_branches
-
     def create_zone_text(
         self,
         firstColumnFileNames,
         secondColumnFileNames,
         thirdColumnFileNames,
         firstColumnFiles,
         secondColumnFiles,
```

### Comparing `git-sim-0.3.0/git_sim/log.py` & `git-sim-0.3.1/git_sim/log.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/logo.png` & `git-sim-0.3.1/git_sim/logo.png`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/merge.py` & `git-sim-0.3.1/git_sim/merge.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/mv.py` & `git-sim-0.3.1/git_sim/mv.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/pull.py` & `git-sim-0.3.1/git_sim/pull.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/push.py` & `git-sim-0.3.1/git_sim/push.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/rebase.py` & `git-sim-0.3.1/git_sim/rebase.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/reset.py` & `git-sim-0.3.1/git_sim/reset.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/restore.py` & `git-sim-0.3.1/git_sim/restore.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/revert.py` & `git-sim-0.3.1/git_sim/revert.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/rm.py` & `git-sim-0.3.1/git_sim/rm.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/settings.py` & `git-sim-0.3.1/git_sim/settings.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/stash.py` & `git-sim-0.3.1/git_sim/stash.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/status.py` & `git-sim-0.3.1/git_sim/status.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/switch.py` & `git-sim-0.3.1/git_sim/switch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim/tag.py` & `git-sim-0.3.1/git_sim/tag.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/git_sim.egg-info/PKG-INFO` & `git-sim-0.3.1/git_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-sim
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
 Home-page: https://initialcommit.com/tools/git-sim
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-sim
 Project-URL: Source, https://github.com/initialcommit-com/git-sim
 Keywords: git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run
@@ -27,31 +27,31 @@
 Visually simulate Git operations in your own repos with a single terminal command.
 
 This generates an image (default) or video visualization depicting the Git command's behavior.
 
 Command syntax is based directly on Git's command-line syntax, so using git-sim is as familiar as possible.
 
 Example: `$ git-sim merge <branch>`
-
-![git-sim-merge_01-05-23_09-44-46](https://user-images.githubusercontent.com/49353917/210939840-1d51493a-6cac-43fd-9d12-3d2948d32c61.jpg)
+<br/><br/>
+![git-sim-merge_04-22-23_21-04-32_cropped](https://user-images.githubusercontent.com/49353917/233821875-a7bb640d-10be-4433-a8fb-bd25646eeff4.jpg)
 
 ## Use cases
 - Visualize Git commands to understand their effects on your repo before actually running them
 - Prevent unexpected working directory and repository states by simulating before running
 - Share visualizations (jpg/png image or mp4/webm video) of your Git commands with your team, or the world
 - Save visualizations as a part of your team documentation to document workflow and prevent recurring issues
 - Create static Git diagrams (jpg/png) or dynamic animated videos (mp4/webm) to speed up content creation
 - Help visual learners understand how Git commands work
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 
 ## Features
 - Run a one-liner git-sim command in the terminal to generate a custom Git command visualization (.jpg) from your repo
 - Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`, `rm`, `mv`, `clean`
 - Generate an animated video (.mp4) instead of a static image using the `--animate` flag (note: significant performance slowdown, it is recommended to use `--low-quality` to speed up testing and remove when ready to generate presentation-quality video)
-- Color commits by parameter, such as author the `--color-by=author` option
+- Color commits by parameter, such as author with the `--color-by=author` option
 - Choose between dark mode (default) and light mode
 - Specify output formats of either jpg, png, mp4, or webm
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 - Animation only: Add custom branded intro/outro sequences if desired
 - Animation only: Speed up or slow down animation speed as desired
 
 ## Quickstart
```

### Comparing `git-sim-0.3.0/git_sim.egg-info/SOURCES.txt` & `git-sim-0.3.1/git_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.0/setup.py` & `git-sim-0.3.1/setup.py`

 * *Files identical despite different names*

