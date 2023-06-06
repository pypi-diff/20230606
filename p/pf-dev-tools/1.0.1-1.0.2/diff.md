# Comparing `tmp/pf_dev_tools-1.0.1.tar.gz` & `tmp/pf_dev_tools-1.0.2.tar.gz`

## Comparing `pf_dev_tools-1.0.1.tar` & `pf_dev_tools-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/.flake8
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/Exceptions.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/__about__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/__init__.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfBuildCore.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfConfig.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfSconsEnvironment.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfUtils.py
--rwxr-xr-x   0        0        0     1077 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/__main__.py
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfBuild.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfClean.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfClone.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfCommand.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfConvert.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfDelete.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfDryRun.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfEject.py
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfInstall.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfMake.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfQfs.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pfTools/pfCommand/pfReverse.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/LICENSE
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/README.md
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/.flake8
+-rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/.nova/Artwork
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/.nova/Configuration.json
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/Exceptions.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/__about__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/__init__.py
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfBuildCore.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfConfig.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfSconsEnvironment.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfUtils.py
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/__main__.py
+-rw-r--r--   0        0        0     9974 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfBuild.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfClean.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfClone.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfCommand.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfConvert.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfDelete.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfDryRun.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfEject.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfInstall.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfMake.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfQfs.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfReverse.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/README.md
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.2/PKG-INFO
```

### Comparing `pf_dev_tools-1.0.1/pfTools/__init__.py` & `pf_dev_tools-1.0.2/pfDevTools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 from .pfUtils import pfUtils
 
 from semver import Version
 
 from .__about__ import __version__
 
 
-# --- Makes sure current pfTools versions is supported
+# --- Makes sure current pfDevTools versions is supported
 def requires(version: str) -> bool:
     current = Version.parse(__version__, optional_minor_and_patch=True)
     required = Version.parse(version, optional_minor_and_patch=True)
 
     if not (required.major == current.major) and ((current.minor > required.minor) or ((current.minor == required.minor) and (current.patch >= required.patch))) and (required.prerelease == current.prerelease):
-        raise RuntimeError(f'pfTools v{str(current)} is not compatible with the required version v{str(required)}')
+        raise RuntimeError(f'pfDevTools v{str(current)} is not compatible with the required version v{str(required)}')
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfBuildCore.py` & `pf_dev_tools-1.0.2/pfDevTools/pfBuildCore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import shutil
-import pfTools
+import pfDevTools
 
 from typing import List
 from pathlib import Path
 
 
 # -- Classes
 class pfBuildCore:
@@ -24,34 +24,37 @@
 
         tag = env.get('PF_CORE_TEMPLATE_REPO_TAG', None)
         if tag is not None:
             command_line += ['tag', tag]
 
         command_line.append(env['PF_BUILD_FOLDER'])
 
-        pfTools.pfClone(command_line).run()
+        pfDevTools.pfClone(command_line).run()
 
     @classmethod
     def _updateQsfFile(cls, target, source, env):
         core_fpga_folder = env['PF_CORE_FPGA_FOLDER']
         core_verilog_files = [str(Path(str(f)).relative_to(core_fpga_folder)) for f in source]
 
-        # -- Let's find out how many CPU cores the docker container is set up with
-        result = pfTools.pfUtils.shellCommand(f'docker run --platform linux/amd64 -t --rm {env["PF_DOCKER_IMAGE"]} grep --count ^processor /proc/cpuinfo'.split(' '),
-                                              silent_mode=True, capture_output=True)
+        try:
+            # -- Let's find out how many CPU cores the docker container is set up with
+            result = pfDevTools.pfUtils.shellCommand(f'docker run --platform linux/amd64 -t --rm {env["PF_DOCKER_IMAGE"]} grep --count ^processor /proc/cpuinfo',
+                                                     silent_mode=True, capture_output=True)
+        except RuntimeError:
+            raise RuntimeError("Cannot start docker container. Are you sure the docker engine is running?")
 
-        pfTools.pfQfs([str(source[0]), str(target[0]), f'cpus={"max" if len(result) != 1 else result[0]}'] + core_verilog_files[1:]).run()
+        pfDevTools.pfQfs([str(source[0]), str(target[0]), f'cpus={"max" if len(result) != 1 else result[0]}'] + core_verilog_files[1:]).run()
 
     @classmethod
     def _installCore(cls, target, source, env):
         # -- If PF_CORE_INSTALL_VOLUME is not defined, we default to POCKET
         core_install_volume = os.environ.get('PF_CORE_INSTALL_VOLUME', 'POCKET')
 
-        pfTools.pfInstall([str(source[0]), core_install_volume]).run()
-        pfTools.pfEject([core_install_volume]).run()
+        pfDevTools.pfInstall([str(source[0]), core_install_volume]).run()
+        pfDevTools.pfEject([core_install_volume]).run()
 
     @classmethod
     def _copyFile(cls, target, source, env):
         source_file = str(source[0])
         target_file = str(target[0])
         parent_dest_dir = Path(target_file).parent
         os.makedirs(parent_dest_dir, exist_ok=True)
@@ -81,23 +84,28 @@
             extra_dest_files.append(dest_path)
 
             env.Command(dest_path, file, pfBuildCore._copyFile)
 
         return extra_dest_files
 
     @classmethod
+    def _compileBitStream(cls, target, source, env):
+        pfDevTools.pfUtils.shellCommand(f'docker run --platform linux/amd64 -t --rm -v {os.path.realpath(env["PF_CORE_FPGA_FOLDER"])}:/build {env["PF_DOCKER_IMAGE"]} quartus_sh --flow compile pf_core')
+
+    @classmethod
     def _packageCore(cls, target, source, env):
-        build_process: pfTools.pfBuild = pfTools.pfBuild([env['PF_CORE_CONFIG_FILE'], env['PF_BUILD_FOLDER'], env['PF_CORE_BITSTREAM_FILE']])
+        build_process: pfDevTools.pfBuild = pfDevTools.pfBuild([env['PF_CORE_CONFIG_FILE'], env['PF_BUILD_FOLDER'], env['PF_CORE_BITSTREAM_FILE']])
         print('Building core...')
         build_process.run()
 
     @classmethod
     def build(cls, env, config_file: str, extra_files: List[str] = []):
+        pfDevTools.pfUtils.requireCommand('docker')
+
         env.SetDefault(PF_DOCKER_IMAGE='didiermalenfant/quartus:22.1-apple-silicon')
-        docker_image = env['PF_DOCKER_IMAGE']
 
         if env.get('PF_SRC_FOLDER', None) is None:
             env.SetDefault(PF_SRC_FOLDER=Path(config_file).parent)
 
         src_folder: str = env['PF_SRC_FOLDER']
 
         env.SetDefault(PF_BUILD_FOLDER='_build')
@@ -121,18 +129,17 @@
         env.Command(core_input_qsf_file, '', pfBuildCore._cloneRepo)
 
         dest_verilog_files: List[str] = pfBuildCore._searchSourceFiles(env, src_folder, dest_verilog_folder)
         extra_dest_files: List[str] = pfBuildCore._addExtraFiles(env, src_folder, dest_verilog_folder, extra_files)
 
         env.Command(core_output_qsf_file, [core_input_qsf_file] + dest_verilog_files, pfBuildCore._updateQsfFile)
 
-        env.Command(core_output_bitstream_file, [core_output_qsf_file] + extra_dest_files,
-                    f'docker run --platform linux/amd64 -t --rm -v {os.path.realpath(core_fpga_folder)}:/build {docker_image} quartus_sh --flow compile pf_core')
+        env.Command(core_output_bitstream_file, [core_output_qsf_file] + extra_dest_files, pfBuildCore._compileBitStream)
 
-        build_process: pfTools.pfBuild = pfTools.pfBuild([config_file, build_folder, core_output_bitstream_file])
+        build_process: pfDevTools.pfBuild = pfDevTools.pfBuild([config_file, build_folder, core_output_bitstream_file])
         packaged_core = os.path.join(build_folder, build_process.packagedFilename())
         p = env.Command(packaged_core, build_process.dependencies(), pfBuildCore._packageCore)
 
         env.Default(packaged_core)
         env.Clean(packaged_core, build_folder)
 
         install_command = env.Command(None, packaged_core, pfBuildCore._installCore)
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfConfig.py` & `pf_dev_tools-1.0.2/pfDevTools/pfConfig.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/__main__.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
 import traceback
 
 from .pfCommand import pfCommand
-from pfTools.Exceptions import ArgumentError
+from pfDevTools.Exceptions import ArgumentError
 
 # -- This enables more debugging information for exceptions.
 _debug_on: bool = False
 
 
 def main():
     global _debug_on
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfBuild.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfBuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil
 import zipfile
 
 from typing import List
 from pathlib import Path
 from datetime import date
 
-from pfTools.pfConfig import pfConfig
+from pfDevTools.pfConfig import pfConfig
 
 from .pfConvert import pfConvert
 from .pfReverse import pfReverse
 
 
 # -- Classes
 class pfBuild:
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfClean.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfClean.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-from pfTools.pfUtils import pfUtils
+from pfDevTools.pfUtils import pfUtils
 
 
 # -- Classes
 class pfClean:
     """A tool to clean the local project."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         if len(arguments) != 0:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
     def run(self) -> None:
-        pfUtils.shellCommand(['scons', '-c', '-Q', '-s'])
+        pfUtils.shellCommand('scons -c -Q -s')
 
     @classmethod
     def name(cls) -> str:
         return 'clean'
 
     @classmethod
     def usage(cls) -> None:
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfClone.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfClone.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
-import shutil
 
-from pfTools.pfUtils import pfUtils
-from pfTools.Exceptions import ArgumentError
+from pfDevTools.pfUtils import pfUtils
+from pfDevTools.Exceptions import ArgumentError
 
 
 # -- Classes
 class pfClone:
     """A tool to clone the Github core template."""
 
     def __init__(self, arguments):
@@ -41,34 +40,32 @@
 
     def run(self) -> None:
         if pfUtils.commandExists('git') is False:
             raise RuntimeError('You must have git installed on your machine to continue.')
 
         repo_folder = os.path.join(self._destination_folder, 'pfCoreTemplate')
         if os.path.exists(repo_folder):
-            shutil.rmtree(repo_folder)
+            pfUtils.deleteFolder(repo_folder, force_delete=True)
 
         print('Cloning core template in \'' + repo_folder + '\'.')
 
-        command_line = ['git', 'clone', '--depth', '1']
+        command_line = 'git clone --depth 1 '
 
         if self._branch_name is not None:
-            command_line.append('--branch')
-            command_line.append(self._branch_name)
+            command_line += f'--branch {self._branch_name} '
         elif self._tag_name is not None:
-            command_line.append('--branch')
-            command_line.append(self._tag_name)
+            command_line += f'--branch {self._tag_name} '
 
-        command_line.append(self._url)
+        command_line += self._url
 
         pfUtils.shellCommand(command_line, from_dir=self._destination_folder, silent_mode=True)
 
         git_folder = os.path.join(repo_folder, '.git')
         if os.path.exists(git_folder):
-            shutil.rmtree(git_folder)
+            pfUtils.deleteFolder(git_folder, force_delete=True)
 
     @classmethod
     def name(cls) -> str:
         return 'clone'
 
     @classmethod
     def usage(cls) -> None:
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfCommand.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfCommand.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # import os
 import sys
 import getopt
 
-from pfTools.__about__ import __version__
-from pfTools.Exceptions import ArgumentError
+from pfDevTools.__about__ import __version__
+from pfDevTools.Exceptions import ArgumentError
 
 from .pfBuild import pfBuild
 from .pfClean import pfClean
 from .pfClone import pfClone
 from .pfConvert import pfConvert
 from .pfDelete import pfDelete
 from .pfDryRun import pfDryRun
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfConvert.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfConvert.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfDelete.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfDelete.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfDryRun.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfMake.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-from pfTools.pfUtils import pfUtils
+from pfDevTools.pfUtils import pfUtils
 
 
 # -- Classes
-class pfDryRun:
-    """A tool to clean the local project."""
+class pfMake:
+    """A tool to make the local project."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         if len(arguments) != 0:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
     def run(self) -> None:
-        pfUtils.shellCommand(['scons', '--dry-run', '--tree=all', '--debug=explain'])
+        pfUtils.shellCommand('scons -Q -s')
 
     @classmethod
     def name(cls) -> str:
-        return 'dryrun'
+        return 'make'
 
     @classmethod
     def usage(cls) -> None:
-        print('   dryrun                                - Simulate building the local project.')
+        print('   make                                  - Make the local project.')
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfEject.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfEject.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 
 from sys import platform
 
-from pfTools.pfUtils import pfUtils
+from pfDevTools.pfUtils import pfUtils
 
 
 # -- Classes
 class pfEject:
     """A tool to eject given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, arguments):
@@ -23,15 +23,15 @@
 
     def run(self) -> None:
         if platform == "darwin":
             if not os.path.exists(os.path.join('/Volumes', self._volume_name)):
                 raise RuntimeError(f'Volume {self._volume_name} is not mounted.')
 
             print('Ejecting \'' + self._volume_name + '\'.')
-            pfUtils.shellCommand(['diskutil', 'eject', self._volume_name])
+            pfUtils.shellCommand(f'diskutil eject {self._volume_name}')
         else:
             print('Ejecting volumes is only supported on macOS right now.')
 
     @classmethod
     def name(cls) -> str:
         return 'eject'
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfInstall.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfInstall.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import zipfile
 import tempfile
 import contextlib
 
 from sys import platform
 
 from distutils.dir_util import copy_tree
-from pfTools.pfUtils import pfUtils
+from pfDevTools.pfUtils import pfUtils
 
 
 # -- Classes
 class pfInstall:
     """A tool to install a zipped up core file onto a given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, arguments):
@@ -56,15 +56,15 @@
 
     def _deleteFile(self, filepath) -> None:
         with contextlib.suppress(FileNotFoundError):
             os.remove(filepath)
 
     def run(self) -> None:
         if self._volume_name is None:
-            pfUtils.shellCommand(['scons', '-Q', '-s', 'install'])
+            pfUtils.shellCommand('scons -Q -s install')
             return
 
         # -- In a temporary folder.
         with tempfile.TemporaryDirectory() as tmp_dir:
             # -- Unzip the file.
             with zipfile.ZipFile(self._zip_filename, 'r') as zip_ref:
                 zip_ref.extractall(tmp_dir)
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfQfs.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfQfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 
 from typing import List
 from enum import Enum
 
-from pfTools.Exceptions import ArgumentError
+from pfDevTools.Exceptions import ArgumentError
 
 
 # -- Classes
 class EditingState(Enum):
     BEFORE_EDIT = 1
     DURING_EDIT = 2
     AFTER_EDIT = 3
@@ -64,15 +64,15 @@
             if file.endswith('.v'):
                 dest_file.write('VERILOG_FILE ')
             elif file.endswith('.sv'):
                 dest_file.write('SYSTEMVERILOG_FILE ')
             else:
                 raise ArgumentError('Unknown file type for \'' + file + '\'.')
 
-            dest_file.write(file + '\n')
+            dest_file.write(file.replace('\\', '/') + '\n')
 
         dest_file.write('\n' + editing_wrappers[1])
 
     def run(self) -> None:
         print('Updating QSF file...')
 
         editing_wrappers: List[str] = ['# Additions made by pf command\n',
```

### Comparing `pf_dev_tools-1.0.1/pfTools/pfCommand/pfReverse.py` & `pf_dev_tools-1.0.2/pfDevTools/pfCommand/pfReverse.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.1/LICENSE` & `pf_dev_tools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.1/README.md` & `pf_dev_tools-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# pfTools
+# pfDevTools
 
-[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfTools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pf-dev-tools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pf-dev-tools.svg)](https://pypi.org/project/pf-dev-tools)
+[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfDevTools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pf-dev-tools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pf-dev-tools.svg)](https://pypi.org/project/pf-dev-tools)
 
 A collection of tools for [Project Freedom](https://didier.malenfant.net/ProjectFreedom/) projects.
 
 Copyright (c) 2023-present **Didier Malenfant**.
 
 -----
 
 ### Pre-requistes
 
-**pfTools** requires at least [Python](https://python.org) 3.10. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
+**pfDevTools** requires at least [Python](https://python.org) 3.10. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
 
 It also uses the [git](https://git-scm.com) command. This should come built in on **macOS** and **Linux**.
 
 ### Installation
 
-You can install **pfTools** by typing the following in a terminal window:
+You can install **pfDevTools** by typing the following in a terminal window:
 ```console
 pip install pf-dev-tools
 ```
 
 ### Usage
 
-**pfTools**'s functionality is centered around the `pf` command.
+**pfDevTools**'s functionality is centered around the `pf` command.
 
 To get more information on its use, just type:
 ```console
 pf --help
 ```
 
 ### Trademarks
@@ -35,8 +35,8 @@
 **openFPGA** and the **openFPGA** logo are trademarks of [**Analogue**](https://www.analogue.co/) Enterprises Ltd.
 **Quartus** is a registered trademark of [**Intel**](https://intel.com/).
 
 This project is not affiliated, associated with, sponsored or supported by neither **Analogue** nor **Intel**.
 
 ### License
 
-**pfTools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
+**pfDevTools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
```

### Comparing `pf_dev_tools-1.0.1/pyproject.toml` & `pf_dev_tools-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 ]
 dependencies = ['semver >= 3', 'Pillow', 'scons',
                 'tomli >= 1.1.0 ; python_version < "3.11"']
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://didier.malenfant.net/ProjectFreedom/"
-Documentation = "https://github.com/DidierMalenfant/pfTools#readme"
-"Bug Tracker" = "https://github.com/DidierMalenfant/pfTools/issues"
-"Source Code" = "https://github.com/DidierMalenfant/pfTools"
+Documentation = "https://github.com/DidierMalenfant/pfDevTools#readme"
+"Bug Tracker" = "https://github.com/DidierMalenfant/pfDevTools/issues"
+"Source Code" = "https://github.com/DidierMalenfant/pfDevTools"
 
 [tool.hatch.version]
-path = "pfTools/__about__.py"
+path = "pfDevTools/__about__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["pfTools"]
+packages = ["pfDevTools"]
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
 ]
 
 [project.scripts]
-pf = "pfTools.pfCommand.__main__:main"
+pf = "pfDevTools.pfCommand.__main__:main"
```

### Comparing `pf_dev_tools-1.0.1/PKG-INFO` & `pf_dev_tools-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pf-dev-tools
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of tools for Project Freedom projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
-Project-URL: Documentation, https://github.com/DidierMalenfant/pfTools#readme
-Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pfTools/issues
-Project-URL: Source Code, https://github.com/DidierMalenfant/pfTools
+Project-URL: Documentation, https://github.com/DidierMalenfant/pfDevTools#readme
+Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pfDevTools/issues
+Project-URL: Source Code, https://github.com/DidierMalenfant/pfDevTools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: ProjectFreedom,analoguepocket,fpga,openFPGA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
@@ -18,40 +18,40 @@
 Requires-Python: >=3.10
 Requires-Dist: pillow
 Requires-Dist: scons
 Requires-Dist: semver>=3
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
-# pfTools
+# pfDevTools
 
-[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfTools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pf-dev-tools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pf-dev-tools.svg)](https://pypi.org/project/pf-dev-tools)
+[![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfDevTools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pf-dev-tools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pf-dev-tools.svg)](https://pypi.org/project/pf-dev-tools)
 
 A collection of tools for [Project Freedom](https://didier.malenfant.net/ProjectFreedom/) projects.
 
 Copyright (c) 2023-present **Didier Malenfant**.
 
 -----
 
 ### Pre-requistes
 
-**pfTools** requires at least [Python](https://python.org) 3.10. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
+**pfDevTools** requires at least [Python](https://python.org) 3.10. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
 
 It also uses the [git](https://git-scm.com) command. This should come built in on **macOS** and **Linux**.
 
 ### Installation
 
-You can install **pfTools** by typing the following in a terminal window:
+You can install **pfDevTools** by typing the following in a terminal window:
 ```console
 pip install pf-dev-tools
 ```
 
 ### Usage
 
-**pfTools**'s functionality is centered around the `pf` command.
+**pfDevTools**'s functionality is centered around the `pf` command.
 
 To get more information on its use, just type:
 ```console
 pf --help
 ```
 
 ### Trademarks
@@ -59,8 +59,8 @@
 **openFPGA** and the **openFPGA** logo are trademarks of [**Analogue**](https://www.analogue.co/) Enterprises Ltd.
 **Quartus** is a registered trademark of [**Intel**](https://intel.com/).
 
 This project is not affiliated, associated with, sponsored or supported by neither **Analogue** nor **Intel**.
 
 ### License
 
-**pfTools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
+**pfDevTools** is distributed under the terms of the [GPLv3.0](https://spdx.org/licenses/GPL-3.0-or-later.html) or later license.
```

