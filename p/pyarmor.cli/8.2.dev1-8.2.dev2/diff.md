# Comparing `tmp/pyarmor.cli-8.2.dev1-py2.py3-none-any.whl.zip` & `tmp/pyarmor.cli-8.2.dev2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 36451 bytes, number of entries: 18
--rw-r--r--  2.0 unx     1479 b- defN 23-Apr-25 01:18 pyarmor/cli/__init__.py
--rw-r--r--  2.0 unx    22591 b- defN 23-Apr-28 23:46 pyarmor/cli/__main__.py
+Zip file size: 36617 bytes, number of entries: 18
+-rw-r--r--  2.0 unx     1479 b- defN 23-Apr-29 14:32 pyarmor/cli/__init__.py
+-rw-r--r--  2.0 unx    22526 b- defN 23-Apr-29 21:18 pyarmor/cli/__main__.py
 -rw-r--r--  2.0 unx    10694 b- defN 23-Apr-20 07:01 pyarmor/cli/config.py
--rw-r--r--  2.0 unx    17255 b- defN 23-Apr-28 22:34 pyarmor/cli/context.py
--rw-r--r--  2.0 unx     7475 b- defN 23-Apr-27 00:20 pyarmor/cli/default.cfg
--rw-r--r--  2.0 unx     5553 b- defN 23-Apr-22 00:21 pyarmor/cli/generate.py
+-rw-r--r--  2.0 unx    17473 b- defN 23-Apr-30 10:02 pyarmor/cli/context.py
+-rw-r--r--  2.0 unx     8186 b- defN 23-May-01 02:05 pyarmor/cli/default.cfg
+-rw-r--r--  2.0 unx     5532 b- defN 23-Apr-30 08:53 pyarmor/cli/generate.py
 -rw-r--r--  2.0 unx     3956 b- defN 23-Apr-20 07:02 pyarmor/cli/mixer.py
 -rw-r--r--  2.0 unx     2847 b- defN 23-Apr-22 14:15 pyarmor/cli/plugin.py
 -rw-r--r--  2.0 unx     2487 b- defN 23-Mar-25 22:51 pyarmor/cli/public_capsule.zip
--rw-r--r--  2.0 unx    17413 b- defN 23-Apr-29 00:43 pyarmor/cli/register.py
+-rw-r--r--  2.0 unx    17413 b- defN 23-Apr-29 05:01 pyarmor/cli/register.py
 -rw-r--r--  2.0 unx    11386 b- defN 23-Apr-20 07:01 pyarmor/cli/repack.py
 -rw-r--r--  2.0 unx     6398 b- defN 23-Apr-13 06:46 pyarmor/cli/resource.py
 -rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 14:43 pyarmor/cli/shell.py
--rw-r--r--  2.0 unx     2407 b- defN 23-Apr-29 01:11 pyarmor.cli-8.2.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-29 01:11 pyarmor.cli-8.2.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 23-Apr-29 01:11 pyarmor.cli-8.2.dev1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 01:11 pyarmor.cli-8.2.dev1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1467 b- defN 23-Apr-29 01:11 pyarmor.cli-8.2.dev1.dist-info/RECORD
-18 files, 115760 bytes uncompressed, 34069 bytes compressed:  70.6%
+-rw-r--r--  2.0 unx     2407 b- defN 23-May-01 02:25 pyarmor.cli-8.2.dev2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-01 02:25 pyarmor.cli-8.2.dev2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-May-01 02:25 pyarmor.cli-8.2.dev2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-01 02:25 pyarmor.cli-8.2.dev2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1467 b- defN 23-May-01 02:25 pyarmor.cli-8.2.dev2.dist-info/RECORD
+18 files, 116603 bytes uncompressed, 34235 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: pyarmor/cli/resource.py
 Comment: 
 
 Filename: pyarmor/cli/shell.py
 Comment: 
 
-Filename: pyarmor.cli-8.2.dev1.dist-info/METADATA
+Filename: pyarmor.cli-8.2.dev2.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli-8.2.dev1.dist-info/WHEEL
+Filename: pyarmor.cli-8.2.dev2.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli-8.2.dev1.dist-info/entry_points.txt
+Filename: pyarmor.cli-8.2.dev2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyarmor.cli-8.2.dev1.dist-info/top_level.txt
+Filename: pyarmor.cli-8.2.dev2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli-8.2.dev1.dist-info/RECORD
+Filename: pyarmor.cli-8.2.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/__init__.py

```diff
@@ -1,10 +1,10 @@
 import logging
 
-__VERSION__ = '8.1'
+__VERSION__ = '8.2'
 
 logger = logging.getLogger('cli')
 
 
 class CliError(Exception):
     pass
```

## pyarmor/cli/__main__.py

```diff
@@ -102,17 +102,14 @@
         options['use_runtime'] = args.use_runtime
 
     if options.get('assert_call') or options.get('assert_import'):
         if options.get('restrict_module', 0) < 2:
             logger.debug('implicitly set restrict_module = 2')
             options['restrict_module'] = 2
 
-    if options.get('restrict_module', 0) > 1:
-        options['mix_coname'] = 1
-
     if args.enables:
         for x in args.enables:
             options['enable_' + x] = True
     if options.get('enable_themida'):
         raise NotImplementedError('--enable_themida is still not implemented')
 
     if args.prefix:
@@ -166,15 +163,15 @@
             raise CliError('--enable_themida only works for Windows')
         if enable_bcc:
             raise CliError('bcc mode does not support cross platform')
         check_cross_platform(ctx, ctx.runtime_platforms)
 
     if enable_bcc:
         plat, arch = ctx.pyarmor_platform.split('.')
-        if arch not in ('x86_64', 'aarch64'):
+        if arch not in ('x86_64', 'aarch64', 'x86', 'armv7'):
             raise CliError('bcc mode still not support arch "%s"' % arch)
 
     if ctx.cmd_options['no_runtime'] and not ctx.runtime_outer:
         raise CliError('--no_runtime must be used with --outer')
 
     if ctx.use_runtime and not ctx.runtime_outer:
         if os.path.exists(ctx.use_runtime):
```

## pyarmor/cli/context.py

```diff
@@ -97,15 +97,15 @@
 
         # self.encoding is just for reading config file
         self.encoding = encoding
         cfglist = self.default_config, self.global_config, self.local_config
         self.cfg = self._read_config(cfglist, encoding=encoding)
 
         self.inline_plugin_marker = '# pyarmor: '
-        self.runtime_package = 'pyarmor_runtime'
+        # self.runtime_package = 'pyarmor_runtime'
         # self.runtime_suffix = '_000000'
         # default inner key filename within runtime package
         self.runtime_keyfile = '.pyarmor.ikey'
 
         self.bootstrap_template = bootstrap_template
         self.runtime_package_templates = (
             runtime_package_template,
@@ -218,14 +218,15 @@
         rev = '.'.join([str(x) for x in self.version])
         if not verbose:
             return rev
 
         licinfo = self.license_info
         lictype = 'basic' if licinfo['features'] == 1 else \
             'pro' if licinfo['features'] == 7 else \
+            'group' if licinfo['features'] == 15 else \
             'trial' if licinfo['token'] == 0 else 'unknown'
         verinfo = ['%s (%s)' % (rev, lictype)]
 
         if verbose > 1:
             verinfo.append(licinfo['licno'][-6:])
 
         if verbose > 2:
@@ -284,18 +285,14 @@
 
     @property
     def license_info(self):
         from .register import parse_token
         return parse_token(self.read_token())
 
     @property
-    def runtime_suffix(self):
-        return '_' + self.license_info['licno'][-6:]
-
-    @property
     def native_platform(self):
         from platform import system, machine
         return '.'.join([system().lower(), machine().lower()])
 
     @property
     def pyarmor_platform(self):
         platname = os.getenv('PYARMOR_PLATFORM', self.native_platform)
@@ -444,14 +441,23 @@
     #
     # runtime configuration
     #
     def _rt_opt(self, opt):
         return self.cmd_options.get(opt, self.cfg['runtime'].get(opt))
 
     @property
+    def runtime_suffix(self):
+        return self.license_info['licno'][-6:]
+
+    @property
+    def runtime_package_name(self):
+        fmt = self.cfg.get('runtime', 'package_name_format')
+        return fmt.format(suffix=self.runtime_suffix)
+
+    @property
     def runtime_platforms(self):
         return self._rt_opt('platforms')
 
     @property
     def runtime_on_error(self):
         return self._opti('runtime', 'on_error')
```

## pyarmor/cli/default.cfg

```diff
@@ -129,17 +129,23 @@
 ;; assert: call import
 assert_call = 0
 assert_import = 0
 
 ;; mix string constant
 mix_str = 0
 
+;; hide function name in traceback
+;;   1: hide function.__name__
+;;   2: also hide function.__qualname__ (not implemented)
 mix_coname = 0
+
+;; mix local variables
 mix_localnames = 1
-;; Enable it may result in annotations error
+
+;; mix argument names, it also clears annotations
 mix_argnames = 0
 
 obf_module = 1
 obf_code = 1
 wrap_mode = 1
 
 restrict_module = 1
@@ -173,14 +179,17 @@
 rft_mix_import_name = 0
 
 [runtime]
 
 ;; Generate extension for all Python3.7+
 universal = 0
 
+;; Default runtime package name
+package_name_format = pyarmor_runtime_{suffix}
+
 ;; The file ext only keep .so/.pyd, for example
 ;;     pyarmor_runtime.cpython-37m-darwin.so
 ;;     if simple_extension_name == 1 then
 ;;     pyarmor_runtime.so
 simple_extension_name = 1
 
 ;; Enable outer runtime key
@@ -307,18 +316,28 @@
 ;; Convert comprehensions to bcc code
 enable_comprehension = 1
 
 [windows.x86_64.bcc]
 cc = clang.exe
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-windows -c
 
+[windows.x86.bcc]
+cc = clang.exe
+cflags = --target=i686-elf-linux -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -fPIC -mno-sse -std=c99 -c
+
 [linux.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
 
 [linux.aarch64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -Tlinux.aarch64.ldscript
 
+[linux.x86.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -fPIC -c
+
+[linux.armv7.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -shared -nostdlib -Tlinux.armv7.ldscript
+
 [darwin.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-gnu_linux -fPIC -c
 
 [darwin.aarch64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=arm64-macho-darwin -fPIC -fno-addrsig -fno-stack-protector -shared -nostdlib -lsystem
```

## pyarmor/cli/generate.py

```diff
@@ -90,15 +90,15 @@
         repacker(bundle, output, buildpath, entry=entry, codesign=codesign)
         shutil.rmtree(buildpath)
 
     def _obfuscate_scripts(self):
         rev = self.ctx.version_info()
         template = self.ctx.bootstrap_template
         relative = self.ctx.import_prefix
-        pkgname = self.ctx.runtime_package + self.ctx.runtime_suffix
+        pkgname = self.ctx.runtime_package_name
         bootpath = self.ctx.cfg.get('builder', 'bootstrap_file')
 
         namelist = []
         for res in self.ctx.resources:
             logger.info('process resource "%s"', res.fullname)
             name = res.name
             path = self.format_output(self.ctx.outputs, namelist.count(name))
```

## Comparing `pyarmor.cli-8.2.dev1.dist-info/METADATA` & `pyarmor.cli-8.2.dev2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli
-Version: 8.2.dev1
+Version: 8.2.dev2
 Summary: A comand line tool to obfuscate python scripts
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Keywords: protect obfuscate encrypt obfuscation distribute
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Software Distribution
-Requires-Dist: pyarmor.core (~=2.1.0)
+Requires-Dist: pyarmor.core (~=3.2.0)
 
 Protect Python Scripts By Pyarmor
 =================================
 
 Pyarmor is a command line tool used to obfuscate python scripts, bind
 obfuscated scripts to fixed machine or expire obfuscated scripts.
```

