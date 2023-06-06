# Comparing `tmp/snk-0.6.8.tar.gz` & `tmp/snk-0.6.9.tar.gz`

## Comparing `snk-0.6.8.tar` & `snk-0.6.9.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.8/Dockerfile
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.6.8/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.8/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.8/docs/CNAME
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.8/docs/index.md
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.6.8/docs/managing_pipelines.md
--rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 snk-0.6.8/docs/pipeline_packages.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snk-0.6.8/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.8/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.8/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.8/docs/reference/nest.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.8/snk/__about__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.8/snk/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.8/snk/errors.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snk-0.6.8/snk/main.py
--rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 snk-0.6.8/snk/nest.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.8/snk/pipeline.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.8/snk/cli/__init__.py
--rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 snk-0.6.8/snk/cli/cli.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 snk-0.6.8/snk/cli/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.8/snk/cli/options.py
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 snk-0.6.8/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.8/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.8/tests/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.8/tests/conftest.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.8/tests/test_nest.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.8/tests/test_pipline_cli.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.8/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.8/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/.snk
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/cli.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/resources/data.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/workflow/Snakefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/workflow/envs/base.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.8/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.8/LICENSE.txt
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 snk-0.6.8/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 snk-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.9/Dockerfile
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.6.9/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.9/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.9/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.9/docs/CNAME
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 snk-0.6.9/docs/index.md
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.6.9/docs/managing_pipelines.md
+-rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 snk-0.6.9/docs/pipeline_packages.md
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 snk-0.6.9/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.9/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.9/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.9/docs/reference/nest.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 snk-0.6.9/docs/reference/pipeline.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.9/snk/__about__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.9/snk/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.9/snk/errors.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snk-0.6.9/snk/main.py
+-rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 snk-0.6.9/snk/nest.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.9/snk/pipeline.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.9/snk/cli/__init__.py
+-rw-r--r--   0        0        0    19654 2020-02-02 00:00:00.000000 snk-0.6.9/snk/cli/cli.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 snk-0.6.9/snk/cli/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.9/snk/cli/options.py
+-rw-r--r--   0        0        0     8933 2020-02-02 00:00:00.000000 snk-0.6.9/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.9/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.9/tests/__init__.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 snk-0.6.9/tests/conftest.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.9/tests/test_nest.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 snk-0.6.9/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.9/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.9/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/cli.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/resources/data.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/workflow/envs/base.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.9/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.9/LICENSE.txt
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 snk-0.6.9/README.md
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 snk-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 snk-0.6.9/PKG-INFO
```

### Comparing `snk-0.6.8/mkdocs.yml` & `snk-0.6.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/.github/workflows/publish.yml` & `snk-0.6.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/.github/workflows/tests.yml` & `snk-0.6.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/docs/managing_pipelines.md` & `snk-0.6.9/docs/managing_pipelines.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/docs/pipeline_packages.md` & `snk-0.6.9/docs/pipeline_packages.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/snk/main.py` & `snk-0.6.9/snk/main.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/snk/nest.py` & `snk-0.6.9/snk/nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/snk/pipeline.py` & `snk-0.6.9/snk/pipeline.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/snk/cli/cli.py` & `snk-0.6.9/snk/cli/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 from .config import (
     SnkConfig,
     get_config_from_pipeline_dir,
     load_pipeline_snakemake_config,
 )
-from .utils import add_dynamic_options, build_dynamic_cli_options, parse_config_args
+from .utils import add_dynamic_options, build_dynamic_cli_options, parse_config_args, dag_filetype_callback
 from snk.pipeline import Pipeline
 
 
 class CLI:
     """
     Constructor for the CLI class.
     Args:
@@ -104,15 +104,14 @@
         )
         self.register_command(
             self.info, help="Display information about current pipeline install."
         )
         self.register_command(self.config, help="Access the pipeline configuration.")
         self.register_command(self.env, help="Access the pipeline conda environments.")
         self.register_command(self.profile, help="Access the pipeline profiles.")
-        # self.register_command(self.script, help="Access the pipeline scripts.")
         self.register_command(
             add_dynamic_options(self.options)(self.run),
             help="Run the dynamically generated pipeline CLI.\n\nAll unrecognized arguments are passed onto Snakemake.",
             context_settings={
                 "allow_extra_args": True,
                 "ignore_unknown_options": True,
                 "help_option_names": ["-h", "--help"],
@@ -214,15 +213,15 @@
           ...     # do something
         """
         copied_resources = []
 
         def copy_resource(src, dst, symlink=False):
             if self.verbose:
                 typer.secho(
-                    f"- Copying resource '{src}' to '{dst}'",
+                    f"  - Copying resource '{src}' to '{dst}'",
                     fg=typer.colors.YELLOW,
                 )
             target_is_directory = src.is_dir()
             if symlink:
                 os.symlink(src, dst, target_is_directory=target_is_directory)
             elif target_is_directory:
                 shutil.copytree(src, dst)
@@ -252,30 +251,33 @@
                 destination = Path(".") / resource.name
                 if not destination.exists():
                     # make sure you don't delete files that are already there...
                     copy_resource(abs_path, destination, symlink=symlink_resources)
                     copied_resources.append(destination)
                 elif self.verbose:
                     typer.secho(
-                        f"- Resource '{resource.name}' already exists! Skipping...",
+                        f"  - Resource '{resource.name}' already exists! Skipping...",
                         fg=typer.colors.YELLOW,
                     )
             yield
         finally:
             if not cleanup:
                 return
             for copied_resource in copied_resources:
                 if copied_resource.exists():
                     if self.verbose:
                         typer.secho(
                             f"Deleting '{copied_resource.name}' resource...",
                             fg=typer.colors.YELLOW,
                         )
                     remove_resource(copied_resource)
-
+    def error(self, msg):
+        typer.secho(msg, fg="red")
+        raise typer.Exit(1)
+    
     def run(
         self,
         ctx: typer.Context,
         target: str = typer.Argument(
             None, help="File to generate. If None will run the pipeline 'all' rule."
         ),
         configfile: Path = typer.Option(
@@ -314,14 +316,21 @@
         ),
         keep_snakemake: bool = typer.Option(
             False,
             "--keep-snakemake",
             "-S",
             help="Keep .snakemake folder after pipeline completes.",
         ),
+        dag: Optional[Path] = typer.Option(
+            None, 
+            "--dag",
+            "-d",
+            help="Save directed acyclic graph to file. Must end in .pdf, .png or .svg", 
+            callback=dag_filetype_callback,
+        ),
         cores: int = typer.Option(
             None,
             "--cores",
             "-c",
             help="Set the number of cores to use. If None will use all cores.",
         ),
         verbose: Optional[bool] = typer.Option(
@@ -423,33 +432,35 @@
             f"{list(c.keys())[0]}={list(c.values())[0]}" for c in config_dict_list
         ]
         if configs:
             args.extend(["--config", *configs])
         if verbose:
             typer.secho(f"snakemake {' '.join(args)}\n", fg=typer.colors.MAGENTA)
 
-        self.snk_config.add_resources(resource, self.pipeline.path)
         try:
-            with self.copy_resources(
-                self.snk_config.resources, 
-                cleanup=not keep_resources, 
-                symlink_resources=self.snk_config.symlink_resources
-            ):
-                try:
-                    snakemake.main(args)
-                except SystemExit as e:
-                    status = int(str(e))
-                    if status:
-                        sys.exit(status)
-            if not keep_snakemake and Path(".snakemake").exists():
-                if verbose:
-                    typer.secho("Deleting '.snakemake' folder...", fg="yellow")
-                shutil.rmtree(".snakemake")
-        except FileExistsError as e:
-            typer.secho(e, fg=typer.colors.RED)
+            self.snk_config.add_resources(resource, self.pipeline.path)
+        except FileNotFoundError as e:
+            self.error(str(e))
+        with self.copy_resources(
+            self.snk_config.resources, 
+            cleanup=not keep_resources, 
+            symlink_resources=self.snk_config.symlink_resources
+        ):
+            if dag:
+                return self.save_dag(snakemake_args=args, filename=dag)
+            try:
+                snakemake.main(args)
+            except SystemExit as e:
+                status = int(str(e))
+                if status:
+                    sys.exit(status)
+        if not keep_snakemake and Path(".snakemake").exists():
+            if verbose:
+                typer.secho("Deleting '.snakemake' folder...", fg="yellow")
+            shutil.rmtree(".snakemake")
 
     def info(self):
         """
         Display information about current pipeline install.
         Returns:
           str: A JSON string containing information about the current pipeline install.
         Examples:
@@ -510,19 +521,42 @@
         )
         typer.echo(
             f"Found {len(self.pipeline.profiles)} profiles in {profiles_dir_yellow}"
         )
         for profile in self.pipeline.profiles:
             typer.echo(f"- {profile.name}")
 
-    # def script(
-    #     self,
-    #     name: Optional[str] = typer.Argument(None)
-    # ):
-    #     """
-    #     Access the pipeline scripts.
-    #     Args:
-    #       name (str): The name of the script.
-    #     Examples:
-    #       >>> CLI.script(name='my_script')
-    #     """
-    #     raise NotImplementedError
+    
+    def save_dag(
+        self,
+        snakemake_args: List[str],
+        filename: Path
+    ):
+        from contextlib import redirect_stdout
+        import io
+
+        snakemake_args.append("--dag")
+        
+        fileType = filename.suffix.lstrip('.')
+        
+        # Create a file-like object to redirect the stdout
+        snakemake_output = io.StringIO()
+        # Use redirect_stdout to redirect stdout to the file-like object
+        with redirect_stdout(snakemake_output):
+            # Capture the output of snakemake.main(args) using a try-except block
+            try:
+                snakemake.main(snakemake_args)
+            except SystemExit:  # Catch SystemExit exception to prevent termination
+                pass
+        try:
+            echo_process = subprocess.Popen(['echo', snakemake_output.getvalue()], stdout=subprocess.PIPE)
+            dot_process = subprocess.Popen(['dot', f'-T{fileType}'], stdin=echo_process.stdout, stdout=subprocess.PIPE)
+            with open(filename, 'w') as output_file:
+                if self.verbose:
+                    typer.secho(
+                        f"Saving dag to {filename}", fg=typer.colors.YELLOW
+                    )
+                subprocess.run(['cat'], stdin=dot_process.stdout, stdout=output_file)
+        except (subprocess.CalledProcessError, FileNotFoundError):
+            typer.secho(
+                "dot command not found!", fg=typer.colors.RED
+            )
```

### Comparing `snk-0.6.8/snk/cli/config.py` & `snk-0.6.9/snk/cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,16 @@
             resources (List[Path]): List of resources to validate.
         Raises:
             FileNotFoundError: If a resource is not found.
         Notes:
             This function does not modify the resources list.
         """
         for resource in resources:
-            assert resource.exists(), FileNotFoundError(
-                f"Could not find resource: {resource}"
-            )
+            if not resource.exists(): 
+                raise FileNotFoundError(f"Could not find resource: {resource}")
 
     def add_resources(self, resources: List[Path], pipeline_dir_path: Path = None):
         processed = []
         for resource in resources:
             if pipeline_dir_path and not resource.is_absolute():
                 resource = pipeline_dir_path / resource
             processed.append(resource)
```

### Comparing `snk-0.6.8/snk/cli/utils.py` & `snk-0.6.9/snk/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,7 +243,16 @@
                 "help": help,
                 "type": param_type,
                 "required": required,
             }
         )
     # TODO: find annotations missing from config and add them to options
     return options
+
+
+def dag_filetype_callback(ctx: typer.Context, file: Path):
+    allowed=[".pdf", ".png", ".svg"]
+    if ctx.resilient_parsing or not file:
+        return
+    if file.suffix not in allowed:
+        raise typer.BadParameter(f"Dag file suffix must be one of {','.join(allowed)}!")
+    return file
```

### Comparing `snk-0.6.8/tests/.DS_Store` & `snk-0.6.9/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/tests/conftest.py` & `snk-0.6.9/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,8 +37,18 @@
     (path / 'bin').mkdir()
     nest = Nest(path / 'home', path / 'bin')
     print(nest.bin_dir)
     print(nest.snk_home)
     local_pipeline = nest.install("tests/data/pipeline")
     expected = nest.pipelines_dir / 'pipeline'
     assert expected.exists()
-    return local_pipeline
+    return local_pipeline
+
+@pytest.fixture()
+def local_runner(tmp_path_factory):
+    path = Path(tmp_path_factory.mktemp("snk"))
+    (path / 'home').mkdir()
+    (path / 'bin').mkdir()
+    nest = Nest(path / 'home', path / 'bin')
+    local_pipeline = nest.install("tests/data/pipeline")
+    runner = CLIRunner([local_pipeline.executable])
+    return runner
```

### Comparing `snk-0.6.8/tests/test_nest.py` & `snk-0.6.9/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/tests/test_pipline_cli.py` & `snk-0.6.9/tests/test_pipline_cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 
 def test_info(basic_runner):
     res = basic_runner(['info'])
     assert 'snk-basic-pipeline' in res.stdout, res.stderr
     assert 'version' in res.stdout
     assert 'pipeline_dir_path' in res.stdout
 
-def test_run(basic_runner):
+def test_run_cli(basic_runner):
     res = basic_runner(['run', '-h'])
     assert 'snk-basic-pipeline' in res.stdout, res.stderr
     assert 'samples' in res.stdout
     assert 'genome' in res.stdout
-    res = basic_runner(['run'])
-
 
+@pytest.mark.parametrize("filetype", ['pdf', 'svg', 'png'])
+def test_dag(local_runner, tmp_path, filetype):
+    res = local_runner(['run', '--dag', f'{tmp_path}/dag.{filetype}'])
+    assert 'DAG' in res.stderr, res.stderr
+    assert Path(f'{tmp_path}/dag.{filetype}').exists()
```

### Comparing `snk-0.6.8/tests/test_snk.py` & `snk-0.6.9/tests/test_snk.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/tests/utils.py` & `snk-0.6.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/tests/data/artic_v4.1.bed` & `snk-0.6.9/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/tests/data/config.yaml` & `snk-0.6.9/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/tests/data/cov.fasta` & `snk-0.6.9/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/LICENSE.txt` & `snk-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.6.8/pyproject.toml` & `snk-0.6.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -55,17 +55,17 @@
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=snk --cov=tests"
 test = "cov --no-cov"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311"]
 
 # requires hatch-containers
-[tool.hatch.envs.docker]
-type = "container"
-image = "wytamma/snk"
+# [tool.hatch.envs.docker]
+# type = "container"
+# image = "wytamma/snk"
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "snk/__about__.py",
 ]
```

### Comparing `snk-0.6.8/PKG-INFO` & `snk-0.6.9/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,208 +1,196 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 736e 6b0a  : 2.1.Name: snk.
-00000020: 5665 7273 696f 6e3a 2030 2e36 2e38 0a50  Version: 0.6.8.P
-00000030: 726f 6a65 6374 2d55 524c 3a20 446f 6375  roject-URL: Docu
-00000040: 6d65 6e74 6174 696f 6e2c 2068 7474 7073  mentation, https
-00000050: 3a2f 2f67 6974 6875 622e 636f 6d2f 7779  ://github.com/wy
-00000060: 7461 6d6d 612f 736e 6b23 7265 6164 6d65  tamma/snk#readme
-00000070: 0a50 726f 6a65 6374 2d55 524c 3a20 4973  .Project-URL: Is
-00000080: 7375 6573 2c20 6874 7470 733a 2f2f 6769  sues, https://gi
-00000090: 7468 7562 2e63 6f6d 2f77 7974 616d 6d61  thub.com/wytamma
-000000a0: 2f73 6e6b 2f69 7373 7565 730a 5072 6f6a  /snk/issues.Proj
-000000b0: 6563 742d 5552 4c3a 2053 6f75 7263 652c  ect-URL: Source,
-000000c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000000d0: 636f 6d2f 7779 7461 6d6d 612f 736e 6b0a  com/wytamma/snk.
-000000e0: 4175 7468 6f72 2d65 6d61 696c 3a20 5779  Author-email: Wy
-000000f0: 7461 6d6d 6120 5769 7274 6820 3c77 7974  tamma Wirth <wyt
-00000100: 616d 6d61 2e77 6972 7468 406d 652e 636f  amma.wirth@me.co
-00000110: 6d3e 0a4c 6963 656e 7365 2d45 7870 7265  m>.License-Expre
-00000120: 7373 696f 6e3a 204d 4954 0a4c 6963 656e  ssion: MIT.Licen
-00000130: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-00000140: 2e74 7874 0a43 6c61 7373 6966 6965 723a  .txt.Classifier:
-00000150: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
-00000160: 7475 7320 3a3a 2034 202d 2042 6574 610a  tus :: 4 - Beta.
-00000170: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000190: 203a 3a20 5079 7468 6f6e 0a43 6c61 7373   :: Python.Class
-000001a0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000001b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001c0: 7974 686f 6e20 3a3a 2033 2e37 0a43 6c61  ython :: 3.7.Cla
-000001d0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000001e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001f0: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
-00000200: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000210: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000220: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-00000230: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000250: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000260: 2e31 300a 436c 6173 7369 6669 6572 3a20  .10.Classifier: 
-00000270: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000280: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000290: 3a20 332e 3131 0a43 6c61 7373 6966 6965  : 3.11.Classifie
-000002a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000002b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002c0: 6e20 3a3a 2049 6d70 6c65 6d65 6e74 6174  n :: Implementat
-000002d0: 696f 6e20 3a3a 2043 5079 7468 6f6e 0a43  ion :: CPython.C
-000002e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000002f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000300: 3a3a 2050 7974 686f 6e20 3a3a 2049 6d70  :: Python :: Imp
-00000310: 6c65 6d65 6e74 6174 696f 6e20 3a3a 2050  lementation :: P
-00000320: 7950 790a 5265 7175 6972 6573 2d50 7974  yPy.Requires-Pyt
-00000330: 686f 6e3a 203e 3d33 2e37 0a52 6571 7569  hon: >=3.7.Requi
-00000340: 7265 732d 4469 7374 3a20 6172 740a 5265  res-Dist: art.Re
-00000350: 7175 6972 6573 2d44 6973 743a 2067 6974  quires-Dist: git
-00000360: 7079 7468 6f6e 0a52 6571 7569 7265 732d  python.Requires-
-00000370: 4469 7374 3a20 6d61 6b65 6675 6e0a 5265  Dist: makefun.Re
-00000380: 7175 6972 6573 2d44 6973 743a 2073 6e61  quires-Dist: sna
-00000390: 6b65 6d61 6b65 0a52 6571 7569 7265 732d  kemake.Requires-
-000003a0: 4469 7374 3a20 7479 7065 725b 616c 6c5d  Dist: typer[all]
-000003b0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-000003c0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-000003d0: 6d61 726b 646f 776e 0a0a 2320 534e 4b20  markdown..# SNK 
-000003e0: 2853 6e65 6b29 0a0a 5b21 5b50 7950 4920  (Snek)..[![PyPI 
-000003f0: 2d20 5665 7273 696f 6e5d 2868 7474 7073  - Version](https
-00000400: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000410: 6f2f 7079 7069 2f76 2f73 6e6b 2e73 7667  o/pypi/v/snk.svg
-00000420: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
-00000430: 6f72 672f 7072 6f6a 6563 742f 736e 6b29  org/project/snk)
-00000440: 0a5b 215b 5079 5049 202d 2050 7974 686f  .[![PyPI - Pytho
-00000450: 6e20 5665 7273 696f 6e5d 2868 7474 7073  n Version](https
-00000460: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000470: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
-00000480: 732f 736e 6b2e 7376 6729 5d28 6874 7470  s/snk.svg)](http
-00000490: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000004a0: 6a65 6374 2f73 6e6b 290a 5b21 5b77 7269  ject/snk).[![wri
-000004b0: 7465 2d74 6865 202d 2064 6f63 735d 2868  te-the - docs](h
-000004c0: 7474 7073 3a2f 2f62 6164 6765 6e2e 6e65  ttps://badgen.ne
-000004d0: 742f 6261 6467 652f 7772 6974 652d 7468  t/badge/write-th
-000004e0: 652f 646f 6373 2f62 6c75 653f 6963 6f6e  e/docs/blue?icon
-000004f0: 3d68 7474 7073 3a2f 2f72 6177 2e67 6974  =https://raw.git
-00000500: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000510: 6f6d 2f57 7974 616d 6d61 2f77 7269 7465  om/Wytamma/write
-00000520: 2d74 6865 2f6d 6173 7465 722f 696d 6167  -the/master/imag
-00000530: 6573 2f77 7269 7465 2d74 6865 2d69 636f  es/write-the-ico
-00000540: 6e2e 7376 6729 5d28 6874 7470 733a 2f2f  n.svg)](https://
-00000550: 7772 6974 652d 7468 652e 7779 7461 6d6d  write-the.wytamm
-00000560: 612e 636f 6d2f 290a 2d2d 2d2d 2d0a 0a2a  a.com/).-----..*
-00000570: 2a54 6162 6c65 206f 6620 436f 6e74 656e  *Table of Conten
-00000580: 7473 2a2a 0a0a 2d20 5b49 6e73 7461 6c6c  ts**..- [Install
-00000590: 6174 696f 6e5d 2823 696e 7374 616c 6c61  ation](#installa
-000005a0: 7469 6f6e 290a 2d20 5b41 626f 7574 5d28  tion).- [About](
-000005b0: 2361 626f 7574 290a 2d20 5b4c 6963 656e  #about).- [Licen
-000005c0: 7365 5d28 236c 6963 656e 7365 290a 0a23  se](#license)..#
-000005d0: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
-000005e0: 6060 6063 6f6e 736f 6c65 0a70 6970 2069  ```console.pip i
-000005f0: 6e73 7461 6c6c 2073 6e6b 0a60 6060 0a0a  nstall snk.```..
-00000600: 2323 2041 626f 7574 0a0a 536e 6b20 2870  ## About..Snk (p
-00000610: 726f 6e6f 756e 6365 6420 736e 656b 2920  ronounced snek) 
-00000620: 6973 2061 2053 4e61 4b65 6d61 6b65 2070  is a SNaKemake p
-00000630: 6970 656c 696e 6520 6d61 6e61 6765 6d65  ipeline manageme
-00000640: 6e74 2073 7973 7465 6d2e 2053 6e6b 2061  nt system. Snk a
-00000650: 6c6c 6f77 7320 796f 7520 746f 2069 6e73  llows you to ins
-00000660: 7461 6c6c 2053 6e61 6b65 6d61 6b65 2070  tall Snakemake p
-00000670: 6970 656c 696e 6573 2061 7320 436f 6d6d  ipelines as Comm
-00000680: 616e 6420 4c69 6e65 2049 6e74 6572 6661  and Line Interfa
-00000690: 6365 7320 2843 4c49 7329 2e20 5573 696e  ces (CLIs). Usin
-000006a0: 6720 6120 7069 7065 6c69 6e65 2061 7320  g a pipeline as 
-000006b0: 6120 434c 4920 696e 6372 6561 7365 7320  a CLI increases 
-000006c0: 6974 7320 696e 7465 726f 7065 7261 6269  its interoperabi
-000006d0: 6c69 7479 2061 6e64 2061 6c6c 6f77 7320  lity and allows 
-000006e0: 636f 6d70 6c65 7820 7069 7065 6c69 6e65  complex pipeline
-000006f0: 7320 746f 2062 6520 7573 6564 2061 7320  s to be used as 
-00000700: 6d6f 6475 6c61 7220 636f 6d70 6f6e 656e  modular componen
-00000710: 7473 2069 6e20 6120 6c61 7267 6572 2073  ts in a larger s
-00000720: 7973 7465 6d2e 2053 6e6b 2c20 7573 696e  ystem. Snk, usin
-00000730: 6720 7079 7468 6f6e 206d 6167 6963 2c20  g python magic, 
-00000740: 7769 6c6c 2064 796e 616d 6963 2067 656e  will dynamic gen
-00000750: 7261 7465 2074 6865 2070 6970 656c 696e  rate the pipelin
-00000760: 6520 434c 4920 7573 696e 6720 7468 6520  e CLI using the 
-00000770: 7069 7065 6c69 6e65 2063 6f6e 6669 6775  pipeline configu
-00000780: 7261 7469 6f6e 2066 696c 652e 0a0a 2323  ration file...##
-00000790: 2042 6173 6963 2055 7365 0a0a 2323 2320   Basic Use..### 
-000007a0: 496e 7374 616c 6c20 6120 7069 7065 6c69  Install a pipeli
-000007b0: 6e65 2061 7320 6120 434c 490a 0a60 6060  ne as a CLI..```
-000007c0: 0a73 6e6b 2069 6e73 7461 6c6c 2073 6e61  .snk install sna
-000007d0: 6b65 6d61 6b65 2d77 6f72 6b66 6c6f 7773  kemake-workflows
-000007e0: 2f72 6e61 2d73 6571 2d73 7461 722d 6465  /rna-seq-star-de
-000007f0: 7365 7132 0a60 6060 0a0a 2323 2320 496e  seq2.```..### In
-00000800: 7370 6563 7420 7468 6520 434c 4920 2020  spect the CLI   
-00000810: 0a0a 6060 600a 726e 612d 7365 712d 7374  ..```.rna-seq-st
-00000820: 6172 2d64 6573 6571 3220 2d2d 6865 6c70  ar-deseq2 --help
-00000830: 0a60 6060 0a3c 696d 6720 7769 6474 683d  .```.<img width=
-00000840: 2237 3437 2220 616c 743d 2269 6d61 6765  "747" alt="image
-00000850: 2220 7372 633d 2268 7474 7073 3a2f 2f75  " src="https://u
-00000860: 7365 722d 696d 6167 6573 2e67 6974 6875  ser-images.githu
-00000870: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000880: 2f31 3337 3236 3030 352f 3231 3331 3230  /13726005/213120
-00000890: 3437 352d 6130 3235 6537 3431 2d63 3962  475-a025e741-c9b
-000008a0: 652d 3461 6161 2d61 6536 322d 3337 6564  e-4aaa-ae62-37ed
-000008b0: 3663 3339 6236 3938 2e70 6e67 223e 0a0a  6c39b698.png">..
-000008c0: 0a23 2323 2056 6965 7720 7468 6520 6461  .### View the da
-000008d0: 6720 200a 0a60 6060 0a72 6e61 2d73 6571  g  ..```.rna-seq
-000008e0: 2d73 7461 722d 6465 7365 7132 2064 6167  -star-deseq2 dag
-000008f0: 202d 2d70 6466 200a 6060 600a 0a23 2323   --pdf .```..###
-00000900: 2052 756e 2074 6865 2070 6970 656c 696e   Run the pipelin
-00000910: 6520 0a0a 6060 600a 726e 612d 7365 712d  e ..```.rna-seq-
-00000920: 7374 6172 2d64 6573 6571 3220 7275 6e0a  star-deseq2 run.
-00000930: 6060 600a 0a23 2323 2043 6f6e 6669 6775  ```..### Configu
-00000940: 7265 200a 0a53 6e6b 2077 696c 6c20 6479  re ..Snk will dy
-00000950: 6e61 6d69 6361 6c6c 7920 6765 6e65 7261  namically genera
-00000960: 7465 2063 6f6e 6669 6720 6f70 7469 6f6e  te config option
-00000970: 7320 666f 7220 7468 6520 434c 492e 2046  s for the CLI. F
-00000980: 6f72 2065 7861 6d70 6c65 2069 6620 796f  or example if yo
-00000990: 7572 2063 6f6e 6669 672e 7961 6d6c 2066  ur config.yaml f
-000009a0: 696c 6520 6861 7320 7468 6520 6f70 7469  ile has the opti
-000009b0: 6f6e 2060 6661 7374 613a 206e 756c 6c60  on `fasta: null`
-000009c0: 2079 6f75 2063 616e 2073 6574 2074 6869   you can set thi
-000009d0: 7320 6f70 7469 6f6e 2077 6974 6820 602d  s option with `-
-000009e0: 2d66 6173 7461 602e 0a0a 6060 600a 726e  -fasta`...```.rn
-000009f0: 612d 7365 712d 7374 6172 2d64 6573 6571  a-seq-star-deseq
-00000a00: 3220 7275 6e20 2d2d 6661 7374 6120 6578  2 run --fasta ex
-00000a10: 616d 706c 652e 6661 0a60 6060 0a0a 596f  ample.fa.```..Yo
-00000a20: 7520 6361 6e20 616c 736f 2063 6f6e 6669  u can also confi
-00000a30: 6775 7265 2074 6865 2070 6970 656c 696e  gure the pipelin
-00000a40: 6520 7573 696e 6720 6120 636f 6e66 6967  e using a config
-00000a50: 2066 696c 652e 200a 0a60 6060 0a72 6e61   file. ..```.rna
-00000a60: 2d73 6571 2d73 7461 722d 6465 7365 7132  -seq-star-deseq2
-00000a70: 2063 6f6e 6669 6720 2320 7072 696e 7420   config # print 
-00000a80: 7468 6520 636f 6e66 6967 200a 726e 612d  the config .rna-
-00000a90: 7365 712d 7374 6172 2d64 6573 6571 3220  seq-star-deseq2 
-00000aa0: 636f 6e66 6967 203e 2063 6f6e 6669 672e  config > config.
-00000ab0: 796d 6c20 2320 7361 7665 2074 6865 2063  yml # save the c
-00000ac0: 6f6e 6669 6720 0a72 6e61 2d73 6571 2d73  onfig .rna-seq-s
-00000ad0: 7461 722d 6465 7365 7132 2072 756e 202d  tar-deseq2 run -
-00000ae0: 2d63 6f6e 6669 6720 636f 6e66 6967 2e79  -config config.y
-00000af0: 6d6c 2023 2072 756e 2077 6974 6820 636f  ml # run with co
-00000b00: 6e66 6967 200a 6060 600a 0a23 2068 6f77  nfig .```..# how
-00000b10: 2069 7420 776f 726b 730a 0a57 6865 6e20   it works..When 
-00000b20: 696e 7374 616c 6c69 6e67 2061 2070 6970  installing a pip
-00000b30: 656c 696e 6520 736e 6b20 7769 6c6c 0a0a  eline snk will..
-00000b40: 2d20 6372 6561 7465 2064 6972 6563 746f  - create directo
-00000b50: 7279 2060 2450 5954 484f 4e5f 4249 4e5f  ry `$PYTHON_BIN_
-00000b60: 4449 522f 2e2e 2f73 6e6b 2f70 6970 656c  DIR/../snk/pipel
-00000b70: 696e 6573 2f50 4950 454c 494e 4560 0a2d  ines/PIPELINE`.-
-00000b80: 2069 6e73 7461 6c6c 2074 6865 2070 6970   install the pip
-00000b90: 656c 696e 6520 696e 746f 2074 6869 7320  eline into this 
-00000ba0: 6469 7265 6374 6f72 790a 2d20 6578 706f  directory.- expo
-00000bb0: 7365 2043 4c49 2061 7420 6024 5059 5448  se CLI at `$PYTH
-00000bc0: 4f4e 5f42 494e 5f44 4952 6020 7468 6174  ON_BIN_DIR` that
-00000bd0: 2070 6f69 6e74 2074 6f20 7069 7065 6c69   point to pipeli
-00000be0: 6e65 2064 6972 6563 746f 7279 2069 6e20  ne directory in 
-00000bf0: 6073 6e6b 2f70 6970 656c 696e 6573 2f50  `snk/pipelines/P
-00000c00: 4950 454c 494e 452f 6269 6e60 0a2d 2041  IPELINE/bin`.- A
-00000c10: 7320 6c6f 6e67 2061 7320 6024 5059 5448  s long as `$PYTH
-00000c20: 4f4e 5f42 494e 5f44 4952 6020 6973 206f  ON_BIN_DIR` is o
-00000c30: 6e20 796f 7572 2050 4154 482c 2079 6f75  n your PATH, you
-00000c40: 2063 616e 206e 6f77 2069 6e76 6f6b 6520   can now invoke 
-00000c50: 7468 6520 7069 7065 6c69 6e65 2067 6c6f  the pipeline glo
-00000c60: 6261 6c6c 790a 0a23 2068 6579 2077 6861  bally..# hey wha
-00000c70: 7420 6162 6f75 7420 736e 616b 6564 6570  t about snakedep
-00000c80: 6c6f 793f 3f0a 7965 730a 0a23 2320 4c69  loy??.yes..## Li
-00000c90: 6365 6e73 650a 0a60 736e 6b60 2069 7320  cense..`snk` is 
-00000ca0: 6469 7374 7269 6275 7465 6420 756e 6465  distributed unde
-00000cb0: 7220 7468 6520 7465 726d 7320 6f66 2074  r the terms of t
-00000cc0: 6865 205b 4d49 545d 2868 7474 7073 3a2f  he [MIT](https:/
-00000cd0: 2f73 7064 782e 6f72 672f 6c69 6365 6e73  /spdx.org/licens
-00000ce0: 6573 2f4d 4954 2e68 746d 6c29 206c 6963  es/MIT.html) lic
-00000cf0: 656e 7365 2e0a                           ense..
+00000000: 2320 534e 4b20 2853 6e65 6b29 0a0a 5b21  # SNK (Snek)..[!
+00000010: 5b50 7950 4920 2d20 5665 7273 696f 6e5d  [PyPI - Version]
+00000020: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000030: 656c 6473 2e69 6f2f 7079 7069 2f76 2f73  elds.io/pypi/v/s
+00000040: 6e6b 2e73 7667 295d 2868 7474 7073 3a2f  nk.svg)](https:/
+00000050: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000060: 742f 736e 6b29 0a5b 215b 5079 5049 202d  t/snk).[![PyPI -
+00000070: 2050 7974 686f 6e20 5665 7273 696f 6e5d   Python Version]
+00000080: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000090: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+000000a0: 6572 7369 6f6e 732f 736e 6b2e 7376 6729  ersions/snk.svg)
+000000b0: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+000000c0: 7267 2f70 726f 6a65 6374 2f73 6e6b 290a  rg/project/snk).
+000000d0: 5b21 5b77 7269 7465 2d74 6865 202d 2064  [![write-the - d
+000000e0: 6f63 735d 2868 7474 7073 3a2f 2f62 6164  ocs](https://bad
+000000f0: 6765 6e2e 6e65 742f 6261 6467 652f 7772  gen.net/badge/wr
+00000100: 6974 652d 7468 652f 646f 6373 2f62 6c75  ite-the/docs/blu
+00000110: 653f 6963 6f6e 3d68 7474 7073 3a2f 2f72  e?icon=https://r
+00000120: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000130: 7465 6e74 2e63 6f6d 2f57 7974 616d 6d61  tent.com/Wytamma
+00000140: 2f77 7269 7465 2d74 6865 2f6d 6173 7465  /write-the/maste
+00000150: 722f 696d 6167 6573 2f77 7269 7465 2d74  r/images/write-t
+00000160: 6865 2d69 636f 6e2e 7376 6729 5d28 6874  he-icon.svg)](ht
+00000170: 7470 733a 2f2f 7772 6974 652d 7468 652e  tps://write-the.
+00000180: 7779 7461 6d6d 612e 636f 6d2f 290a 5b21  wytamma.com/).[!
+00000190: 5b48 6974 735d 2868 7474 7073 3a2f 2f68  [Hits](https://h
+000001a0: 6974 732e 7365 6579 6f75 6661 726d 2e63  its.seeyoufarm.c
+000001b0: 6f6d 2f61 7069 2f63 6f75 6e74 2f69 6e63  om/api/count/inc
+000001c0: 722f 6261 6467 652e 7376 673f 7572 6c3d  r/badge.svg?url=
+000001d0: 6874 7470 7325 3341 2532 4625 3246 6769  https%3A%2F%2Fgi
+000001e0: 7468 7562 2e63 6f6d 2532 4657 7974 616d  thub.com%2FWytam
+000001f0: 6d61 2532 4673 6e6b 2663 6f75 6e74 5f62  ma%2Fsnk&count_b
+00000200: 673d 2532 3337 3943 3833 4426 7469 746c  g=%2379C83D&titl
+00000210: 655f 6267 3d25 3233 3535 3535 3535 2669  e_bg=%23555555&i
+00000220: 636f 6e3d 2669 636f 6e5f 636f 6c6f 723d  con=&icon_color=
+00000230: 2532 3345 3745 3745 3726 7469 746c 653d  %23E7E7E7&title=
+00000240: 6869 7473 2665 6467 655f 666c 6174 3d66  hits&edge_flat=f
+00000250: 616c 7365 295d 2868 7474 7073 3a2f 2f67  alse)](https://g
+00000260: 6974 6875 622e 636f 6d2f 5779 7461 6d6d  ithub.com/Wytamm
+00000270: 612f 736e 6b29 0a0a 2d2d 2d0a 0a2a 2a44  a/snk)..---..**D
+00000280: 6f63 756d 656e 7461 7469 6f6e 2a2a 3a20  ocumentation**: 
+00000290: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000002a0: 2f73 6e6b 2e77 7974 616d 6d61 2e63 6f6d  /snk.wytamma.com
+000002b0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+000002c0: 223e 6874 7470 733a 2f2f 736e 6b2e 7779  ">https://snk.wy
+000002d0: 7461 6d6d 612e 636f 6d3c 2f61 3e0a 0a2a  tamma.com</a>..*
+000002e0: 2a53 6f75 7263 6520 436f 6465 2a2a 3a20  *Source Code**: 
+000002f0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000300: 2f67 6974 6875 622e 636f 6d2f 5779 7461  /github.com/Wyta
+00000310: 6d6d 612f 736e 6b22 2074 6172 6765 743d  mma/snk" target=
+00000320: 225f 626c 616e 6b22 3e68 7474 7073 3a2f  "_blank">https:/
+00000330: 2f67 6974 6875 622e 636f 6d2f 5779 7461  /github.com/Wyta
+00000340: 6d6d 612f 736e 6b3c 2f61 3e0a 0a2d 2d2d  mma/snk</a>..---
+00000350: 0a0a 536e 6b20 2870 726f 6e6f 756e 6365  ..Snk (pronounce
+00000360: 6420 736e 656b 2920 6973 2061 2053 4e61  d snek) is a SNa
+00000370: 4b65 6d61 6b65 2070 6970 656c 696e 6520  Kemake pipeline 
+00000380: 6d61 6e61 6765 6d65 6e74 2073 7973 7465  management syste
+00000390: 6d2e 2053 6e6b 2061 6c6c 6f77 7320 796f  m. Snk allows yo
+000003a0: 7520 746f 2069 6e73 7461 6c6c 2053 6e61  u to install Sna
+000003b0: 6b65 6d61 6b65 2070 6970 656c 696e 6573  kemake pipelines
+000003c0: 2061 7320 436f 6d6d 616e 6420 4c69 6e65   as Command Line
+000003d0: 2049 6e74 6572 6661 6365 7320 2843 4c49   Interfaces (CLI
+000003e0: 7329 2e20 5573 696e 6720 6120 7069 7065  s). Using a pipe
+000003f0: 6c69 6e65 2061 7320 6120 434c 4920 696e  line as a CLI in
+00000400: 6372 6561 7365 7320 6974 7320 696e 7465  creases its inte
+00000410: 726f 7065 7261 6269 6c69 7479 2061 6e64  roperability and
+00000420: 2061 6c6c 6f77 7320 636f 6d70 6c65 7820   allows complex 
+00000430: 7069 7065 6c69 6e65 7320 746f 2062 6520  pipelines to be 
+00000440: 7573 6564 2061 7320 6d6f 6475 6c61 7220  used as modular 
+00000450: 636f 6d70 6f6e 656e 7473 2069 6e20 6120  components in a 
+00000460: 6c61 7267 6572 2073 7973 7465 6d2e 2053  larger system. S
+00000470: 6e6b 2c20 7573 696e 6720 7079 7468 6f6e  nk, using python
+00000480: 206d 6167 6963 2c20 7769 6c6c 2064 796e   magic, will dyn
+00000490: 616d 6963 2067 656e 7261 7465 2074 6865  amic genrate the
+000004a0: 2070 6970 656c 696e 6520 434c 4920 7573   pipeline CLI us
+000004b0: 696e 6720 7468 6520 7069 7065 6c69 6e65  ing the pipeline
+000004c0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+000004d0: 696c 652e 0a0a 2323 2049 6e73 7461 6c6c  ile...## Install
+000004e0: 6174 696f 6e0a 0a60 6060 636f 6e73 6f6c  ation..```consol
+000004f0: 650a 7069 7020 696e 7374 616c 6c20 736e  e.pip install sn
+00000500: 6b0a 6060 600a 0a23 2320 4261 7369 6320  k.```..## Basic 
+00000510: 5573 650a 0a23 2323 2049 6e73 7461 6c6c  Use..### Install
+00000520: 2061 2070 6970 656c 696e 6520 6173 2061   a pipeline as a
+00000530: 2043 4c49 0a0a 496e 7374 616c 6c20 7468   CLI..Install th
+00000540: 6520 646e 612d 7365 712d 6761 746b 2d76  e dna-seq-gatk-v
+00000550: 6172 6961 6e74 2d63 616c 6c69 6e67 2070  ariant-calling p
+00000560: 6970 656c 696e 6520 2876 322e 312e 3129  ipeline (v2.1.1)
+00000570: 2061 7320 6076 6172 6961 6e74 2d63 616c   as `variant-cal
+00000580: 6c69 6e67 602e 0a0a 6060 600a 736e 6b20  ling`...```.snk 
+00000590: 696e 7374 616c 6c20 736e 616b 656d 616b  install snakemak
+000005a0: 652d 776f 726b 666c 6f77 732f 646e 612d  e-workflows/dna-
+000005b0: 7365 712d 6761 746b 2d76 6172 6961 6e74  seq-gatk-variant
+000005c0: 2d63 616c 6c69 6e67 202d 2d6e 616d 6520  -calling --name 
+000005d0: 7661 7269 616e 742d 6361 6c6c 696e 6720  variant-calling 
+000005e0: 2d74 2076 322e 312e 310a 6060 600a 5375  -t v2.1.1.```.Su
+000005f0: 6363 6573 7366 756c 6c79 2069 6e73 7461  ccessfully insta
+00000600: 6c6c 6564 2076 6172 6961 6e74 2d63 616c  lled variant-cal
+00000610: 6c69 6e67 2028 7632 2e31 2e31 2921 0a0a  ling (v2.1.1)!..
+00000620: 2323 2320 496e 7370 6563 7420 7468 6520  ### Inspect the 
+00000630: 434c 4920 2020 0a0a 6060 600a 7661 7269  CLI   ..```.vari
+00000640: 616e 742d 6361 6c6c 696e 6720 2d2d 6865  ant-calling --he
+00000650: 6c70 0a60 6060 0a3c 696d 6720 7769 6474  lp.```.<img widt
+00000660: 683d 2238 3632 2220 616c 743d 226d 6169  h="862" alt="mai
+00000670: 6e20 636c 6922 2073 7263 3d22 6874 7470  n cli" src="http
+00000680: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f57  s://github.com/W
+00000690: 7974 616d 6d61 2f73 6e6b 2f61 7373 6574  ytamma/snk/asset
+000006a0: 732f 3133 3732 3630 3035 2f62 6233 3939  s/13726005/bb399
+000006b0: 3763 352d 3965 6536 2d34 3635 642d 3866  7c5-9ee6-465d-8f
+000006c0: 3739 2d63 3934 3036 3763 6539 3939 3722  79-c94067ce9997"
+000006d0: 3e0a 0a23 2323 2056 6965 7720 7275 6e20  >..### View run 
+000006e0: 6f70 7469 6f6e 730a 0a60 6060 0a76 6172  options..```.var
+000006f0: 6961 6e74 2d63 616c 6c69 6e67 2072 756e  iant-calling run
+00000700: 202d 680a 6060 600a 3c69 6d67 2077 6964   -h.```.<img wid
+00000710: 7468 3d22 3836 3222 2061 6c74 3d22 7275  th="862" alt="ru
+00000720: 6e20 636c 6922 2073 7263 3d22 6874 7470  n cli" src="http
+00000730: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f57  s://github.com/W
+00000740: 7974 616d 6d61 2f73 6e6b 2f61 7373 6574  ytamma/snk/asset
+00000750: 732f 3133 3732 3630 3035 2f33 3463 3430  s/13726005/34c40
+00000760: 6137 632d 3732 6332 2d34 3234 352d 3935  a7c-72c2-4245-95
+00000770: 3839 2d37 6333 6338 3938 3262 6530 3822  89-7c3c8982be08"
+00000780: 3e0a 0a0a 2323 2320 4372 6561 7465 2061  >...### Create a
+00000790: 2044 4147 0a0a 4865 7265 2077 6520 7573   DAG..Here we us
+000007a0: 6520 7468 6520 602e 7465 7374 6020 7265  e the `.test` re
+000007b0: 736f 7572 6365 7320 696e 636c 7564 6564  sources included
+000007c0: 2069 6e20 7468 6520 7069 7065 6c69 6e65   in the pipeline
+000007d0: 2074 6f20 6372 6561 7465 2074 6865 2044   to create the D
+000007e0: 4147 2e0a 0a60 6060 0a76 6172 6961 6e74  AG...```.variant
+000007f0: 2d63 616c 6c69 6e67 2072 756e 202d 7220  -calling run -r 
+00000800: 2e74 6573 742f 636f 6e66 6967 202d 7220  .test/config -r 
+00000810: 2e74 6573 742f 6461 7461 202d 2d64 6167  .test/data --dag
+00000820: 2064 6167 2e70 6466 0a60 6060 0a3c 696d   dag.pdf.```.<im
+00000830: 6720 7769 6474 683d 2238 3632 2220 616c  g width="862" al
+00000840: 743d 2264 6167 2220 7372 633d 2268 7474  t="dag" src="htt
+00000850: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000860: 5779 7461 6d6d 612f 736e 6b2f 6173 7365  Wytamma/snk/asse
+00000870: 7473 2f31 3337 3236 3030 352f 6637 3962  ts/13726005/f79b
+00000880: 6366 6433 2d66 3663 642d 3430 3165 2d62  cfd3-f6cd-401e-b
+00000890: 3564 382d 3930 3465 3764 3566 3138 3335  5d8-904e7d5f1835
+000008a0: 223e 0a0a 0a23 2323 2043 6f6e 6669 6775  ">...### Configu
+000008b0: 7265 200a 0a53 6e6b 2077 696c 6c20 6479  re ..Snk will dy
+000008c0: 6e61 6d69 6361 6c6c 7920 6765 6e65 7261  namically genera
+000008d0: 7465 2063 6f6e 6669 6720 6f70 7469 6f6e  te config option
+000008e0: 7320 666f 7220 7468 6520 434c 492e 2046  s for the CLI. F
+000008f0: 6f72 2065 7861 6d70 6c65 2069 6620 796f  or example if yo
+00000900: 7572 2063 6f6e 6669 672e 7961 6d6c 2066  ur config.yaml f
+00000910: 696c 6520 6861 7320 7468 6520 6f70 7469  ile has the opti
+00000920: 6f6e 2060 6661 7374 613a 206e 756c 6c60  on `fasta: null`
+00000930: 2079 6f75 2063 616e 2073 6574 2074 6869   you can set thi
+00000940: 7320 6f70 7469 6f6e 2077 6974 6820 602d  s option with `-
+00000950: 2d66 6173 7461 602e 0a0a 6060 600a 7661  -fasta`...```.va
+00000960: 7269 616e 742d 6361 6c6c 696e 6720 7275  riant-calling ru
+00000970: 6e20 2d2d 6661 7374 6120 6578 616d 706c  n --fasta exampl
+00000980: 652e 6661 0a60 6060 0a0a 596f 7520 6361  e.fa.```..You ca
+00000990: 6e20 616c 736f 2063 6f6e 6669 6775 7265  n also configure
+000009a0: 2074 6865 2070 6970 656c 696e 6520 7573   the pipeline us
+000009b0: 696e 6720 6120 636f 6e66 6967 2066 696c  ing a config fil
+000009c0: 652e 200a 0a60 6060 0a76 6172 6961 6e74  e. ..```.variant
+000009d0: 2d63 616c 6c69 6e67 2063 6f6e 6669 6720  -calling config 
+000009e0: 2d2d 7072 6574 7479 2023 2070 7269 6e74  --pretty # print
+000009f0: 2074 6865 2063 6f6e 6669 6720 0a76 6172   the config .var
+00000a00: 6961 6e74 2d63 616c 6c69 6e67 2063 6f6e  iant-calling con
+00000a10: 6669 6720 3e20 636f 6e66 6967 2e79 6d6c  fig > config.yml
+00000a20: 2023 2073 6176 6520 7468 6520 636f 6e66   # save the conf
+00000a30: 6967 200a 7661 7269 616e 742d 6361 6c6c  ig .variant-call
+00000a40: 696e 6720 7275 6e20 2d2d 636f 6e66 6967  ing run --config
+00000a50: 2063 6f6e 6669 672e 796d 6c20 2320 7275   config.yml # ru
+00000a60: 6e20 7769 7468 2063 6f6e 6669 6720 0a60  n with config .`
+00000a70: 6060 0a0a 2323 2068 6f77 2069 7420 776f  ``..## how it wo
+00000a80: 726b 730a 0a57 6865 6e20 696e 7374 616c  rks..When instal
+00000a90: 6c69 6e67 2061 2070 6970 656c 696e 6520  ling a pipeline 
+00000aa0: 736e 6b20 7769 6c6c 0a0a 2d20 6372 6561  snk will..- crea
+00000ab0: 7465 2064 6972 6563 746f 7279 2060 2450  te directory `$P
+00000ac0: 5954 484f 4e5f 4249 4e5f 4449 522f 2e2e  YTHON_BIN_DIR/..
+00000ad0: 2f73 6e6b 2f70 6970 656c 696e 6573 2f50  /snk/pipelines/P
+00000ae0: 4950 454c 494e 4560 0a2d 2069 6e73 7461  IPELINE`.- insta
+00000af0: 6c6c 2074 6865 2070 6970 656c 696e 6520  ll the pipeline 
+00000b00: 696e 746f 2074 6869 7320 6469 7265 6374  into this direct
+00000b10: 6f72 790a 2d20 6578 706f 7365 2043 4c49  ory.- expose CLI
+00000b20: 2061 7420 6024 5059 5448 4f4e 5f42 494e   at `$PYTHON_BIN
+00000b30: 5f44 4952 6020 7468 6174 2070 6f69 6e74  _DIR` that point
+00000b40: 2074 6f20 7069 7065 6c69 6e65 2064 6972   to pipeline dir
+00000b50: 6563 746f 7279 2069 6e20 6073 6e6b 2f70  ectory in `snk/p
+00000b60: 6970 656c 696e 6573 2f50 4950 454c 494e  ipelines/PIPELIN
+00000b70: 452f 6269 6e60 0a2d 2041 7320 6c6f 6e67  E/bin`.- As long
+00000b80: 2061 7320 6024 5059 5448 4f4e 5f42 494e   as `$PYTHON_BIN
+00000b90: 5f44 4952 6020 6973 206f 6e20 796f 7572  _DIR` is on your
+00000ba0: 2050 4154 482c 2079 6f75 2063 616e 206e   PATH, you can n
+00000bb0: 6f77 2069 6e76 6f6b 6520 7468 6520 7069  ow invoke the pi
+00000bc0: 7065 6c69 6e65 2067 6c6f 6261 6c6c 790a  peline globally.
+00000bd0: 0a0a 2323 204c 6963 656e 7365 0a0a 6073  ..## License..`s
+00000be0: 6e6b 6020 6973 2064 6973 7472 6962 7574  nk` is distribut
+00000bf0: 6564 2075 6e64 6572 2074 6865 2074 6572  ed under the ter
+00000c00: 6d73 206f 6620 7468 6520 5b4d 4954 5d28  ms of the [MIT](
+00000c10: 6874 7470 733a 2f2f 7370 6478 2e6f 7267  https://spdx.org
+00000c20: 2f6c 6963 656e 7365 732f 4d49 542e 6874  /licenses/MIT.ht
+00000c30: 6d6c 2920 6c69 6365 6e73 652e 0a         ml) license..
```

