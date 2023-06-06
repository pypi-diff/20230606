# Comparing `tmp/garden_ai-0.4.1.tar.gz` & `tmp/garden_ai-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-0.4.1.tar", max compression
+gzip compressed data, was "garden_ai-0.4.2.tar", max compression
```

## Comparing `garden_ai-0.4.1.tar` & `garden_ai-0.4.2.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0     1078 2023-05-15 16:28:06.427582 garden_ai-0.4.1/LICENSE
--rw-r--r--   0        0        0      797 2023-05-15 16:28:06.431582 garden_ai-0.4.1/README.md
--rw-r--r--   0        0        0      356 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/__init__.py
--rw-r--r--   0        0        0       54 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/__main__.py
--rw-r--r--   0        0        0       97 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/_version.py
--rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/__init__.py
--rw-r--r--   0        0        0       54 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/console.py
--rw-r--r--   0        0        0    10478 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/garden.py
--rw-r--r--   0        0        0      828 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/main.py
--rw-r--r--   0        0        0     3076 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/model.py
--rw-r--r--   0        0        0     6862 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/pipeline.py
--rw-r--r--   0        0        0    17674 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/client.py
--rw-r--r--   0        0        0     9398 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/datacite.py
--rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/funcx_bandaid/__init__.py
--rw-r--r--   0        0        0     1247 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/funcx_bandaid/serialization_patch.py
--rw-r--r--   0        0        0    12872 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_compute/__init__.py
--rw-r--r--   0        0        0     2803 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_compute/containers.py
--rw-r--r--   0        0        0     1451 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_compute/login_manager.py
--rw-r--r--   0        0        0      801 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_compute/remote_functions.py
--rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_search/__init__.py
--rw-r--r--   0        0        0     3011 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_search/garden_search.py
--rw-r--r--   0        0        0     7498 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/local_data.py
--rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/mlflow_bandaid/__init__.py
--rw-r--r--   0        0        0     1064 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/mlflow_bandaid/binary_header_provider.py
--rw-r--r--   0        0        0     9999 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/mlmodel.py
--rw-r--r--   0        0        0    15864 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/pipelines.py
--rw-r--r--   0        0        0    11963 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/steps.py
--rw-r--r--   0        0        0     2017 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/templates/pipeline
--rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/utils/__init__.py
--rw-r--r--   0        0        0     1241 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/utils/filesystem.py
--rw-r--r--   0        0        0    11588 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/utils/misc.py
--rw-r--r--   0        0        0     2784 2023-05-15 16:28:20.635941 garden_ai-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 garden_ai-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-06 16:06:37.386640 garden_ai-0.4.2/LICENSE
+-rw-r--r--   0        0        0      797 2023-06-06 16:06:37.386640 garden_ai-0.4.2/README.md
+-rw-r--r--   0        0        0      418 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/__main__.py
+-rw-r--r--   0        0        0       97 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/_version.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/console.py
+-rw-r--r--   0        0        0    10707 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/garden.py
+-rw-r--r--   0        0        0      828 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/main.py
+-rw-r--r--   0        0        0     3076 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/model.py
+-rw-r--r--   0        0        0     7184 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/app/pipeline.py
+-rw-r--r--   0        0        0    17556 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/client.py
+-rw-r--r--   0        0        0       76 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/constants.py
+-rw-r--r--   0        0        0     9398 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/datacite.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/funcx_bandaid/__init__.py
+-rw-r--r--   0        0        0     1247 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/funcx_bandaid/serialization_patch.py
+-rw-r--r--   0        0        0    14373 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_compute/__init__.py
+-rw-r--r--   0        0        0     2803 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_compute/containers.py
+-rw-r--r--   0        0        0     1451 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_compute/login_manager.py
+-rw-r--r--   0        0        0      801 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_compute/remote_functions.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_search/__init__.py
+-rw-r--r--   0        0        0     3011 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/globus_search/garden_search.py
+-rw-r--r--   0        0        0     7498 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/local_data.py
+-rw-r--r--   0        0        0    10512 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0    21264 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/pipelines.py
+-rw-r--r--   0        0        0    11909 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/steps.py
+-rw-r--r--   0        0        0     2022 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/templates/pipeline
+-rw-r--r--   0        0        0        0 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     2185 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/utils/filesystem.py
+-rw-r--r--   0        0        0    11186 2023-06-06 16:06:37.386640 garden_ai-0.4.2/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0     2874 2023-06-06 16:06:49.994663 garden_ai-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2419 1970-01-01 00:00:00.000000 garden_ai-0.4.2/PKG-INFO
```

### Comparing `garden_ai-0.4.1/LICENSE` & `garden_ai-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/README.md` & `garden_ai-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/garden_ai/app/garden.py` & `garden_ai-0.4.2/garden_ai/app/garden.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,14 +137,22 @@
     )
 
     local_data.put_local_garden(garden)
 
     if verbose:
         metadata = json.dumps(local_data.get_local_garden_by_uuid(garden.uuid))
         rich.print_json(metadata)
+
+    if garden.doi:
+        rich.print(f"Garden '{garden.title}' created with DOI: {garden.doi}")
+    else:
+        rich.print(
+            f"Garden '{garden.title}' created but missing DOI. Given UUID: {garden.uuid}"
+        )
+
     return
 
 
 @garden_app.command(no_args_is_help=True)
 def search(
     title: Optional[str] = typer.Option(
         None, "-t", "--title", help="Title of a Garden"
```

### Comparing `garden_ai-0.4.1/garden_ai/app/main.py` & `garden_ai-0.4.2/garden_ai/app/main.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/garden_ai/app/model.py` & `garden_ai-0.4.2/garden_ai/app/model.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/garden_ai/app/pipeline.py` & `garden_ai-0.4.2/garden_ai/app/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,45 @@
 import jinja2
 import typer
 from rich import print
 from rich.prompt import Prompt
 
 from garden_ai import GardenClient, Pipeline, step
 from garden_ai.app.console import console
+from garden_ai import GardenConstants
 
+from garden_ai.mlmodel import PipelineLoadScaffoldedException
 from garden_ai.utils.filesystem import (
     load_pipeline_from_python_file,
     PipelineLoadException,
+    PipelineLoadMlFlowException,
 )
+
 from garden_ai.utils.misc import clean_identifier
 
+
 logger = logging.getLogger()
 
 pipeline_app = typer.Typer(name="pipeline", no_args_is_help=True)
 
 
 def parse_full_name(name: str) -> str:
     """(this will probably eventually use some 3rd party name parsing library)"""
     return name.strip() if name else ""
 
 
 def template_pipeline(short_name: str, pipeline: Pipeline) -> str:
     """populate jinja2 template with starter code for creating a pipeline"""
     env = jinja2.Environment(loader=jinja2.PackageLoader("garden_ai"))
     template = env.get_template("pipeline")
-    return template.render(short_name=short_name, pipeline=pipeline)
+    return template.render(
+        short_name=short_name,
+        pipeline=pipeline,
+        scaffolded_model_name=GardenConstants.SCAFFOLDED_MODEL_NAME,
+    )
 
 
 @pipeline_app.callback()
 def pipeline():
     """
     sub-commands for creating and manipulating Pipelines
     """
@@ -199,15 +208,19 @@
     ):
         console.log(
             f"{pipeline_file} is not a valid Python file. Please provide a valid Python file (.py)."
         )
         raise typer.Exit(code=1)
     try:
         user_pipeline = load_pipeline_from_python_file(pipeline_file)
-    except PipelineLoadException as e:
+    except (
+        PipelineLoadException,
+        PipelineLoadMlFlowException,
+        PipelineLoadScaffoldedException,
+    ) as e:
         console.log(f"Could not parse {pipeline_file} as a Garden pipeline. " + str(e))
         raise typer.Exit(code=1) from e
 
     with console.status(
         "[bold green]Building container. This operation times out after 30 minutes."
     ):
         container_uuid = client.build_container(user_pipeline)
```

### Comparing `garden_ai-0.4.1/garden_ai/client.py` & `garden_ai-0.4.2/garden_ai/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,31 +17,31 @@
     NativeAppAuthClient,
     RefreshTokenAuthorizer,
     SearchClient,
     GlobusHTTPResponse,
 )
 from globus_sdk.scopes import AuthScopes, ScopeBuilder, SearchScopes
 from globus_sdk.tokenstorage import SimpleJSONFileAdapter
-from mlflow.tracking.request_header.registry import _request_header_provider_registry
 from rich import print
 from rich.prompt import Prompt
 
 import garden_ai.funcx_bandaid.serialization_patch  # type: ignore # noqa: F401
 from garden_ai import local_data
 from garden_ai.gardens import Garden
 from garden_ai.globus_compute.containers import build_container
 from garden_ai.globus_compute.login_manager import ComputeLoginManager
 from garden_ai.globus_compute.remote_functions import register_pipeline
 from garden_ai.globus_search import garden_search
 
 from garden_ai.local_data import GardenNotFoundException, PipelineNotFoundException
-from garden_ai.mlflow_bandaid.binary_header_provider import (
-    BinaryContentTypeHeaderProvider,
+from garden_ai.mlmodel import (
+    LocalModel,
+    RegisteredModel,
+    upload_to_model_registry,
 )
-from garden_ai.mlmodel import LocalModel, RegisteredModel, upload_to_model_registry
 from garden_ai.pipelines import Pipeline, RegisteredPipeline
 from garden_ai.utils.misc import extract_email_from_globus_jwt
 
 GARDEN_ENDPOINT = os.environ.get(
     "GARDEN_ENDPOINT",
     "https://nu3cetwc84.execute-api.us-east-1.amazonaws.com/garden_prod",
 )
@@ -108,18 +108,21 @@
         self.garden_authorizer = self._create_authorizer(
             GardenClient.scopes.resource_server
         )
 
         self.compute_client = self._make_compute_client()
         self._set_up_mlflow_env()
 
+    def _get_garden_access_token(self):
+        self.garden_authorizer.ensure_valid_token()
+        return self.garden_authorizer.access_token
+
     def _set_up_mlflow_env(self):
-        os.environ["MLFLOW_TRACKING_TOKEN"] = self.garden_authorizer.access_token
+        os.environ["MLFLOW_TRACKING_TOKEN"] = self._get_garden_access_token()
         os.environ["MLFLOW_TRACKING_URI"] = GARDEN_ENDPOINT + "/mlflow"
-        _request_header_provider_registry.register(BinaryContentTypeHeaderProvider)
 
     def _make_compute_client(self):
         scope_to_authorizer = {
             AuthScopes.openid: self.openid_authorizer,
             SearchScopes.all: self.search_authorizer,
             Client.FUNCX_SCOPE: self.compute_authorizer,
         }
@@ -221,15 +224,15 @@
             gc = GardenClient()
             pea_garden = gc.create_garden(
                 authors=["Mendel, Gregor"],
                 title="Experiments on Plant Hybridization",
                 subjects=["Peas"]
             )
             pea_garden.year = 1863
-            pea_garden.subjects += ["Genetics"] # (didn't have the word for it earlier)
+            pea_garden.tags += ["Genetics"] # (didn't have the word for it earlier)
         """
         data = dict(kwargs)
         if authors:
             data["authors"] = authors
         if title:
             data["title"] = title
         return Garden(**data)
```

### Comparing `garden_ai-0.4.1/garden_ai/datacite.py` & `garden_ai-0.4.2/garden_ai/datacite.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/garden_ai/funcx_bandaid/serialization_patch.py` & `garden_ai-0.4.2/garden_ai/funcx_bandaid/serialization_patch.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/garden_ai/gardens.py` & `garden_ai-0.4.2/garden_ai/gardens.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,95 +21,92 @@
 )
 from .pipelines import RegisteredPipeline
 
 logger = logging.getLogger()
 
 
 class Garden(BaseModel):
-    """Object representation of a Garden™.
+    """Object representation of a Garden.
 
-    Required Attributes
-    --------------------
-    authors: List[str]
-        The main researchers involved in producing the Garden. At least one
-        author is required in order to register a DOI. Personal name format
-        should be: "Family, Given".
-
-    title: str
-        An official name or title for the Garden. This attribute must be set
-        in order to register a DOI.
-
-
-    Recommended Attributes
-    --------------------
-    description: str
-        A brief summary of the Garden and/or its purpose, to aid discovery by
-        other Gardeners.
-
-    pipelines: List[Pipeline]
-        TODO
-
-    Optional Attributes
-    --------------------
-    doi: str
-        A garden's doi can be manually set by the user, or generated automatically via the
-        DataCite rest api using the required fields.
-
-    language: str
-        Recommended values are IETF BCP 47, ISO 639-1 language codes, such as:
-        "en", "de", "fr". Defaults to "en".
-
-    tags: List[str]
-        Tags, keywords, classification codes, or key phrases pertaining to the Garden.
-
-    year: str
-        Defaults to current year. This attribute should be formatted 'YYYY'.
-
-    Examples
-    --------
-    Creating a new Garden with a ``GardenClient`` instance::
+    Attributes:
+        authors (list[str]):
+            The main researchers involved in producing the Garden. At least one \
+            author is required in order to register a DOI. Personal name format \
+            should be: "Family, Given".
 
+        contributors (list[str]):
+            Acknowledge contributors to the development of this Garden. These\
+            should be distinct from `authors`.
+
+        title (str):
+            An official name or title for the Garden. This attribute must be set \
+            in order to register a DOI.
+
+        description (str):
+            A brief summary of the Garden and/or its purpose, to aid discovery by \
+            other Gardeners.
+
+        pipelines (list[RegisteredPipeline]):
+            List of the pipelines associated with this garden, built dynamically \
+            from the `pipeline_ids` attribute. Note that these pipelines can \
+            also be accessed directly by their `short_name` (or alias) - see \
+            also `pipeline_names` attribute.
+
+        pipeline_names (list[str]):
+            List of python identifiers (i.e. variable names) usable for this \
+            garden's pipelines.  Takes aliases into account (set when adding \
+            pipeline via CLI or using `rename_pipeline` method.)
+
+        pipeline_ids: List[UUID] = Field(default_factory=list)
+        pipeline_aliases: Dict[str, str] = Field(default_factory=dict)
+
+        doi (str):
+            A garden's doi usable for citations, generated automatically via \
+            DataCite using the required fields.
+
+        version (str):
+            optional, defaults to "0.0.1".
+
+        language (str):
+            Recommended values are IETF BCP 47, ISO 639-1 language codes, such as:\
+            "en", "de", "fr". Defaults to "en".
+
+        tags (List[str]):
+            Tags, keywords, classification codes, or key phrases pertaining to the Garden.
+
+        year (str):
+            Defaults to current year. This attribute should be formatted 'YYYY'.
+
+    Examples:
+        Creating a new Garden with a ``GardenClient`` instance::
+
+        ```python
         gc = GardenClient()
         pea_garden = gc.create_garden(
             authors=["Mendel, Gregor"], title="Experiments on Plant Hybridization"
         )
-        pea_garden.year = 1863
+        pea_garden.year = '1863'
         pea_garden.description = '''This Garden houses sophisticated ML pipelines
-                                  for Big Pea Data extraction and classification.
-                                  It consists of a 2-hectare plot behind the monastery,
-                                  and a 30,000-plant dataset.'''
-
-        gc.register(pea_garden)
-
-    Notes
-    --------
-    Mendel's work was ignored by the scientific community during his lifetime,
-    presumably due to the lack of a working DOI.
-    To remedy this, if the `doi` field is unset when registering the garden, we
-    build one for the user with the datacite api.
+                                    for Big Pea Data extraction and classification.
+                                    It consists of a 2-hectare plot behind the monastery,
+                                    and a 30,000-plant dataset.'''
+        ```
+    Notes:
+        Mendel's work was ignored by the scientific community during his lifetime, \
+        presumably due to the lack of a working DOI. \
+        To remedy this, if the `doi` field is unset when publishing a garden, we \
+        build one for the user with the datacite api.
     """
 
-    class Config:
-        """
-        Configure pydantic per-model settings.
-
-        We disable validate_all so that pydantic ignores temporarily-illegal defaults
-        We enable validate_assignment to make validation occur naturally even after object construction
-        """
-
-        validate_all = False  # (this is the default)
-        validate_assignment = True  # validators invoked on assignment
-        underscore_attrs_are_private = True
-
     title: str = cast(str, Field(default_factory=lambda: None))
     authors: List[str] = Field(default_factory=list, min_items=1, unique_items=True)
     contributors: List[str] = Field(default_factory=list, unique_items=True)
     doi: Optional[str] = Field(default=None)
     description: Optional[str] = Field(None)
-    publisher: str = "Garden"
+    publisher: str = "Garden-AI"
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     language: str = "en"
     tags: List[str] = Field(default_factory=list, unique_items=True)
     version: str = "0.0.1"
     uuid: UUID = Field(default_factory=uuid4, allow_mutation=False)
     pipeline_ids: List[UUID] = Field(default_factory=list)
     pipeline_aliases: Dict[str, str] = Field(default_factory=dict)
@@ -120,26 +117,27 @@
     def valid_year(cls, year):
         if len(str(year)) != 4:
             raise ValueError("year must be formatted `YYYY`")
         return str(year)
 
     @property
     def pipelines(self) -> List[RegisteredPipeline]:
-        """Read-only list of the pipelines registered to a garden.
-
-        Note that these pipelines can also be accessed from the garden as attributes,
-        according to their short_name -- see also ``rename_pipeline``.
-        """
+        """Read-only list of the pipelines registered to a garden."""
         if not self._pipelines:
             self._pipelines = self._collect_pipelines()
         return self._pipelines
 
     @property
     def pipeline_names(self) -> List[str]:
-        """Read-only list of short_names of pipelines registered to a garden."""
+        """Read-only list of short_names of pipelines registered to a garden.
+        Tip:
+            Any of these names can be used like attributes on the garden to \
+            access the pipeline directly -- to use a different name for a \
+            pipeline, see `Garden.rename_pipeline` .
+        """
         names = []
         for pipeline in self.pipelines:
             name = self.pipeline_aliases.get(pipeline.short_name) or pipeline.short_name
             names += [name]
         return names
 
     def _set_pipelines_from_remote_metadata(self, pipeline_metadata: List[dict]):
@@ -163,22 +161,23 @@
                     f"Could not parse pipeline: {json.dumps(meta)}. {e.__str__()}"
                 )
 
         self._pipelines = pipelines
 
     def _collect_pipelines(self) -> List[RegisteredPipeline]:
         """
-        Collect the pipeline objects which have been registered to this garden from local database.
+        Collects the pipeline objects that have been registered to this garden from the local database.
 
-        Note: prefer the ``garden.pipelines` computed property to avoid running this many times.
+        Note:
+            It is recommended to use the `garden.pipelines` computed property to avoid running this method multiple times.
 
-        Returns
-        -------
-        List[RegisteredPipeline]
+        Returns:
+            A list of RegisteredPipeline objects.
         """
+
         from .local_data import PipelineNotFoundException, get_local_pipeline_by_uuid
 
         pipelines = []
         for uuid in self.pipeline_ids:
             pipeline = get_local_pipeline_by_uuid(uuid)
             if pipeline is None:
                 raise PipelineNotFoundException(
@@ -188,54 +187,48 @@
             pipeline._env_vars = self._env_vars
 
             pipelines += [pipeline]
 
         return pipelines
 
     def expanded_metadata(self) -> Dict[str, Any]:
-        """Helper: build the "complete" metadata dict with nested ``Pipeline`` and ``step`` metadata.
-
-        Notes
-        ------
-        When serializing normally with ``garden.{dict(), json()}``, only the
-        uuids of the pipelines in the garden are included.
+        """
+        Helper method: builds the "complete" metadata dictionary with nested `Pipeline` and `step` metadata.
 
-        This returns a superset of ``garden.dict()``, so that the following holds:
+        When serializing normally with `garden.{dict(), json()}`, only the UUIDs of the pipelines in the garden are included.
 
+        This method returns a superset of `garden.dict()`, so that the following holds:
             valid_garden == Garden(**valid_garden.expanded_metadata()) == Garden(**valid_garden.dict())
 
-        Returns
-        -------
-        Dict[str, Any]  ``Garden`` metadata dict augmented with a list of ``RegisteredPipeline`` metadata
-
-        Raises
-        ------
-        PipelineNotFoundException  if ``garden.pipeline_ids`` references an unknown pipeline id.
-        """
+        Returns:
+            A dictionary containing the `Garden` metadata augmented with a list of `RegisteredPipeline` metadata.
 
+        Raises:
+            PipelineNotFoundException: If `garden.pipeline_ids` references an unknown pipeline ID.
+        """
         data = self.dict()
         data["pipelines"] = [p.expanded_metadata() for p in self.pipelines]
         return data
 
     def expanded_json(self) -> JSON:
         """Helper: return the expanded garden metadata as JSON.
 
         See: ``Garden.expanded_metadata`` method
         """
         data = self.expanded_metadata()
         return json.dumps(data, default=garden_json_encoder)
 
     def datacite_json(self) -> JSON:
-        """Parse this `Garden`s metadata into a DataCite-schema-compliant JSON string.
+        """Parse this `Garden`s metadata into a DataCite-schema-compliant JSON string."""
 
-        Leverages a pydantic class `DataCiteSchema`, which was automatically generated from:
-        https://github.com/datacite/schema/blob/master/source/json/kernel-4.3/datacite_4.3_schema.json
+        # Leverages a pydantic class `DataCiteSchema`, which was automatically generated from:
+        # https://github.com/datacite/schema/blob/master/source/json/kernel-4.3/datacite_4.3_schema.json
+        #
+        # The JSON returned by this method would be the "attributes" part of a DataCite request body.
 
-        The JSON returned by this method would be the "attributes" part of a DataCite request body.
-        """
         self._sync_author_metadata()
         return DataciteSchema(  # type: ignore
             types=Types(resourceType="AI/ML Garden", resourceTypeGeneral="Software"),
             creators=[Creator(name=name) for name in self.authors],
             titles=[Title(title=self.title)],
             publisher="thegardens.ai",
             publicationYear=self.year,
@@ -257,44 +250,42 @@
                 Description(description=self.description, descriptionType="Other")
             ]
             if self.description
             else None,
         ).json()
 
     def validate(self):
-        """Perform validation on all fields, even fields which are still defaults.
-
-        This is useful for catching fields with a default value which would not
-        otherwise be valid, (e.g.  `None` for any required field), in particular
-        as a sanity check before committing to publishing/registering the user's
-        Garden.
-
-        This is mostly redundant for any already-set fields, as the validators
-        for those would have (hopefully) already run when they were set. However,
-        (because this is still python), it's relatively easy to *modify* some
-        fields without ever *assigning* to them, which wouldn't trigger
-        validation.
-
-        Examples
-        --------
-        gc = GardenClient()
-        pea_garden = gc.create_garden(
-            authors=["Mendel, Gregor"], title="Experiments on Plant Hybridization"
-        )
-
-        # NOTE: pydantic won't see this, as it's neither construction nor assignment
-        pea_garden.authors.append(None)         # no complaints
-
-        # checks all fields, even those smuggled in without triggering validation.
-        pea_garden.validate()
-        # ...
-        # ValidationError: 1 validation error for Garden
-        # authors -> 1
-        #   none is not an allowed value (type=type_error.none.not_allowed)
-        """
+        """Helper: perform validation on all fields, even fields which are still defaults."""
+        # This is useful for catching fields with a default value which would not
+        # otherwise be valid, (e.g.  `None` for any required field), in particular
+        # as a sanity check before committing to publishing/registering the user's
+        # Garden.
+
+        # This is mostly redundant for any already-set fields, as the validators
+        # for those would have (hopefully) already run when they were set. However,
+        # (because this is still python), it's relatively easy to *modify* some
+        # fields without ever *assigning* to them, which wouldn't trigger
+        # validation.
+
+        # Examples
+        # --------
+        # gc = GardenClient()
+        # pea_garden = gc.create_garden(
+        #     authors=["Mendel, Gregor"], title="Experiments on Plant Hybridization"
+        # )
+
+        # # NOTE: pydantic won't see this, as it's neither construction nor assignment
+        # pea_garden.authors.append(None)         # no complaints
+
+        # # checks all fields, even those smuggled in without triggering validation.
+        # pea_garden.validate()
+        # # ...
+        # # ValidationError: 1 validation error for Garden
+        # # authors -> 1
+        # #   none is not an allowed value (type=type_error.none.not_allowed)
         try:
             _ = self.__class__(**self.dict())
         except ValidationError as err:
             logger.error(err)
             raise
 
     def _sync_author_metadata(self):
@@ -328,15 +319,38 @@
         )
 
     def __dir__(self):
         # this gets us jupyter/ipython/repl tab-completion of pipeline names
         return list(super().__dir__()) + self.pipeline_names
 
     def rename_pipeline(self, old_name: str, new_name: str):
+        """Rename a pipeline in this garden.
+
+        Parameters:
+            old_name (str): the current short_name of the pipeline
+            new_name (str): the new short_name of the pipeline
+        Raises:
+            ValueError: if the new_name is already in use, or if the old_name is \
+            not found, or if the new_name is not a valid identifier.
+        """
         if hasattr(self, new_name):
             raise ValueError(
                 f"Error: found existing {new_name} attribute on this garden."
             )
+        if not hasattr(self, old_name):
+            raise ValueError(
+                f"Error: could not find pipeline {old_name} on this garden."
+            )
         if not new_name.isidentifier():
             raise ValueError("new_name must be a valid identifier.")
         self.pipeline_aliases[old_name] = new_name
         return
+
+    class Config:
+        # Configure pydantic per-model settings.
+
+        # We disable validate_all so that pydantic ignores temporarily-illegal defaults
+        # We enable validate_assignment to make validation occur naturally even after object construction
+
+        validate_all = False  # (this is the default)
+        validate_assignment = True  # validators invoked on assignment
+        underscore_attrs_are_private = True
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `garden_ai-0.4.1/garden_ai/globus_compute/containers.py` & `garden_ai-0.4.2/garden_ai/globus_compute/containers.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/garden_ai/globus_compute/login_manager.py` & `garden_ai-0.4.2/garden_ai/globus_compute/login_manager.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/garden_ai/globus_compute/remote_functions.py` & `garden_ai-0.4.2/garden_ai/globus_compute/remote_functions.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/garden_ai/globus_search/garden_search.py` & `garden_ai-0.4.2/garden_ai/globus_search/garden_search.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/garden_ai/local_data.py` & `garden_ai-0.4.2/garden_ai/local_data.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.1/garden_ai/mlmodel.py` & `garden_ai-0.4.2/garden_ai/mlmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,34 @@
+import os
 import pathlib
 import pickle
 from enum import Enum
 from functools import lru_cache
 from typing import List
 
 import mlflow  # type: ignore
 from mlflow.pyfunc import load_model  # type: ignore
-import os
 from pydantic import BaseModel, Field, validator
 
 from garden_ai.utils.misc import read_conda_deps
+from garden_ai import GardenConstants
 
 
 class ModelUploadException(Exception):
     """Exception raised when an attempt to upload a model to ML Flow fails"""
 
     pass
 
 
+class PipelineLoadScaffoldedException(Exception):
+    """Exception raised when a user attempts to load model with the name SCAFFOLDED_MODEL_NAME"""
+
+    pass
+
+
 class ModelFlavor(Enum):
     SKLEARN = "sklearn"
     PYTORCH = "pytorch"
     TENSORFLOW = "tensorflow"
 
 
 class DatasetConnection(BaseModel):
@@ -34,25 +41,27 @@
     doi: str = Field(...)
     repository: str = "Foundry"
     url: str = Field(...)
 
 
 class LocalModel(BaseModel):
     """
-    The ``LocalModel`` class represents a trained ML model
-    that a user wants to register with Garden.
+    The ``LocalModel`` class represents a pre-trained ML model that a user wants to register with Garden.
 
-    Args:
-    model_name (str) A short and descriptive name of the model
-    flavor (str): The framework used for this model. One of "sklearn", "tensorflow", or "torch".
-    extra_pip_requirements (List[str]), optional
-        A list of additional pip requirements needed to load and/or run the model.
-        Defaults to None.
-    local_path (str): Where the model is located on disk. Can be a file or a directory depending on the flavor.
-    user_email (str): The email address of the user uploading the model.
+    Attributes:
+        model_name (str):
+            A short and descriptive name of the model. Model names can only contain alphanumeric characters, hyphens, and underscores.
+        flavor (str):
+            The framework used for this model. One of "sklearn", "tensorflow", or "torch".
+        extra_pip_requirements (List[str]):
+            A list of additional pip requirements needed to load and/or run the model.
+        local_path (str):
+            Where the model is located on disk. Can be a file or a directory depending on the flavor.
+        user_email (str):
+            The email address of the user uploading the model.
 
     """
 
     model_name: str = Field(...)
     flavor: str = Field(...)
     extra_pip_requirements: List[str] = Field(default_factory=list)
     local_path: str = Field(...)
@@ -80,25 +89,25 @@
             )
             raise ValueError(error_message)
         return model_name
 
 
 class RegisteredModel(BaseModel):
     """
-    The ``RegisteredModel`` class represents all the metadata
-    we want to publicly expose about an ML model that has been registered with Garden.
+    The ``RegisteredModel`` class represents all the metadata we want to \
+    publicly expose about an ML model that has been registered with Garden.
 
-    Args:
-    model_name (str): A short and descriptive name of the model
-    version (str): Version string like "1" or "2" for this model.
-    flavor (str): The framework used for this model. One of "sklearn", "tensorflow", or "torch".
-    connections (List[DatasetConnection]):
-        A list of dataset records that the model was trained on.
-    local_path (str): Where the model is located on disk. Can be a file or a directory depending on the flavor.
-    user_email (str): The email address of the user uploading the model.
+    Attributes:
+        model_name (str): A short and descriptive name of the model
+        version (str): Version string like "1" or "2" for this model.
+        flavor (str): The framework used for this model. One of "sklearn", "tensorflow", or "torch".
+        connections (List[DatasetConnection]):
+            A list of dataset records that the model was trained on.
+        local_path (str): Where the model is located on disk. Can be a file or a directory depending on the flavor.
+        user_email (str): The email address of the user uploading the model.
 
     """
 
     model_name: str = Field(...)
     version: str = Field(...)
     user_email: str = Field(...)
     flavor: str = Field(...)
@@ -111,50 +120,47 @@
         self.namespaced_model_name = f"{self.user_email}-{self.model_name}"
         self.model_uri = f"{self.namespaced_model_name}/{self.version}"
 
 
 def upload_to_model_registry(local_model: LocalModel) -> RegisteredModel:
     """Upload a model to Garden-AI's MLflow model registry.
 
-    Parameters
-    ----------
-    local_model : LocalModel
-        The model to upload.
-
-    Returns
-    -------
-    RegisteredModel
-        Includes the full model_uri, which can be used to fetch the model with a call to ``Model(...)``.
-
-    Raises
-    ------
-    ModelUploadException
-        If an error occurs during the upload process, such as failure to open or
-        parse the model, or failure to retrieve the latest version of the model.
+    Args:
+        local_model: The model to upload.
+
+    Returns:
+        RegisteredModel with the full model_uri, which can be used to fetch the \
+        model with a call to ``Model(...)``.
+
+    Raises:
+        ModelUploadException:
+            If an error occurs during the upload process, such as failure to \
+            open or parse the model, or failure to retrieve the latest version \
+            of the model.
     """
     _push_model_to_registry(local_model)
     return _assemble_metadata(local_model)
 
 
 def _push_model_to_registry(local_model: LocalModel):
     flavor, local_path = local_model.flavor, local_model.local_path
     try:
         if flavor == ModelFlavor.SKLEARN.value and pathlib.Path(local_path).is_file:
             with open(local_path, "rb") as f:
                 loaded_model = pickle.load(f)
                 log_model_variant = mlflow.sklearn.log_model
-        elif flavor == ModelFlavor.TENSORFLOW.value and pathlib.Path(local_path).is_dir:
+        elif flavor == ModelFlavor.TENSORFLOW.value:
             os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
             # ignore cpu guard info on tf import require before tf import
             from tensorflow import keras  # type: ignore
 
             loaded_model = keras.models.load_model(local_path)
             log_model_variant = (
                 mlflow.tensorflow.log_model
-            )  # TODO explore artifact path, sigs, and HDf5
+            )  # TODO explore artifact path and sigs
         elif flavor == ModelFlavor.PYTORCH.value and pathlib.Path(local_path).is_file:
             import torch  # type: ignore
 
             loaded_model = torch.load(local_path)
             log_model_variant = mlflow.pytorch.log_model  # TODO explore signatures
         else:
             raise ModelUploadException(f"Unsupported model flavor {flavor}")
@@ -190,14 +196,19 @@
     def __init__(
         self,
         model_full_name: str,
     ):
         self.model = None
         self.model_full_name = model_full_name
         self.model_uri = f"models:/{model_full_name}"
+
+        # raises error if user trys to load model with the name SCAFFOLDED_MODEL_NAME
+        if self.model_full_name == GardenConstants.SCAFFOLDED_MODEL_NAME:
+            raise PipelineLoadScaffoldedException("Invalid model name.")
+
         # extract dependencies without loading model into memory
         # make it easier for steps to infer
         conda_yml = mlflow.pyfunc.get_model_dependencies(self.model_uri, format="conda")
         python_version, conda_dependencies, pip_dependencies = read_conda_deps(
             conda_yml
         )
         self.python_version = python_version
@@ -238,43 +249,42 @@
         return self.model.predict(data)
 
 
 @lru_cache
 def Model(full_model_name: str) -> _Model:
     """Load a registered model from Garden-AI's (MLflow) tracking server.
 
-    Tip: This is meant to be used as a "default argument" in a
-    ``@step``-decorated function. This allows the step to collect model-specific
-    dependencies, including any user-specified dependencies when the model was
-    registered.
+    Tip:
+        This is meant to be used as a "default argument" in a `@step`-decorated \
+        function. This allows the step to collect model-specific dependencies, \
+        including any user-specified dependencies when the model was registered.
 
     Example:
-    --------
-        ```python
-        import garden_ai
-        from garden_ai import step
-        ....
-        # OK for preceding step to return only a DataFrame
-        @step
-        def run_inference(
-            my_data: pd.DataFrame,  # no default
-            my_model = garden_ai.Model("me@uni.edu-myModel/2"),  # NOTE: used as default
-        ) -> MyResultType:
-        '''Run inference on DataFrame `my_data`, returned by previous step.'''
-
-            result = my_model.predict(my_data)
-            return result
-        ```
+    ```python
+    import garden_ai
+    from garden_ai import step
+    ....
+    # OK for preceding step to return only a DataFrame
+    @step
+    def run_inference(
+        my_data: pd.DataFrame,  # no default
+        my_model = garden_ai.Model("me@uni.edu-myModel/2"),  # NOTE: used as default
+    ) -> MyResultType:
+    '''Run inference on DataFrame `my_data`, returned by previous step.'''
+
+        result = my_model.predict(my_data)
+        return result
+    ```
 
     Notes:
-    ------
-    The object returned by this function waits as long as possible - i.e. until
-    the model actually needs to make a prediction - to actually deserialize the
-    registered model. This is done so that ``Model('me@uni.edu-myModel/2)`` in a
-    step (like above) an argument default is lighter-weight when the function itself
-    is serialized for remote execution of a pipeline.
-
-    This function is also memoized, so the same object (which, being lazy, may
-    or may not have actually loaded the model yet) will be returned if it is
-    called multiple times with the same model_full_name.
+        The object returned by this function waits as long as possible - i.e. \
+        until the model actually needs to make a prediction - to actually \
+        deserialize the registered model. This is done so that \
+        ``Model('me@uni.edu-myModel/2)`` in a step (like above) an argument \
+        default is lighter-weight when the function itself is serialized for \
+        remote execution of a pipeline.
+
+        This function is also memoized, so the same object (which, being lazy, \
+        may or may not have actually loaded the model yet) will be returned if \
+        it is called multiple times with the same model_full_name.
     """
     return _Model(full_model_name)
```

### Comparing `garden_ai-0.4.1/garden_ai/steps.py` & `garden_ai-0.4.2/garden_ai/steps.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import inspect
 import json
 import logging
 import typing
 from functools import update_wrapper, wraps
 from inspect import Parameter, Signature, signature
 from typing import Any, Callable, Dict, List, Optional
 
@@ -23,116 +24,84 @@
     validate_assignment = True
 
 
 @dataclass(config=DataclassConfig)
 class Step:
     """The ``Step`` class (via the ``@step`` decorator) wraps a callable for use as a single step in a ``Pipeline``.
 
-    **IMPORTANT**: When included in a ``Pipeline``, all ``Step``s will be checked
-    for composability with respect to their argument- and return-type
-    annotations.  This requires that the decorated function has complete
-    argument- and return-type annotations; a ``Step`` will fail to initialize with
-    an exception if this condition is not met. Note that there is (currently) no
-    type-checking at runtime; annotations are taken in good faith.
-
-    See "Notes" below for additional discussion on composing steps with multiple
-    arguments by returning a properly-typed ``tuple`` as a result.
-
-    Attributes
-    ----------
-    func: Callable
-        ``func`` is whatever should be called when this ``Step`` is reached in its
-        ``Pipeline``, and is passed the output of the previous step (if one
-        exists) as argument(s).  Typically a plain python function, but a
-        callable object with a sufficiently-annotated ``__call__`` magic method is
-        also acceptable. When the ``@step`` decorator is used, ``func`` will be the
-        decorated function. To be composable as a Step, the following are
-        *required*:
-            1. For all but the first Step in a pipeline, ``func`` must only
-               require positional arguments, each of which must be annotated
-            2. For any but the last Step in a pipeline, ``func`` must return
-               either a single object (if subsequent Step has a single
-               positional arg) or a tuple (if subsequent Step has multiple
-               positional args)
-
-    title: str
-        An official name or title for the Step. Currently, ``func.__name__`` is
-        used as a default.
-
-    description: str
-        A human-readable description of the step. Currently, ``func.__doc__`` is
-        used as a default.
-
-    input_info: str
-        Human-readable description of the input data and/or relevant
-        characteristics that *should* hold true for this step's input (e.g.
-        dimensions of a matrix or column names of a dataframe). Currently,
-        ``typing.get_type_hints(func, include_extras=True)`` is used for the
-        default.
-
-    output_info: str
-        Human-readable description of the output data and/or relevant
-        characteristics that *will* hold true for this step's output (e.g.
-        dimensions of a matrix or column names of a dataframe). Currently,
-        ``typing.get_type_hints(func, include_extras=True)`` is used for the
-        default.
-
-
-    authors: List[str]
-        The main researchers involved in producing the Step, for citation and discoverability
-        purposes.
-
-    model_uris: List[str]
-        A reference to the models used in this step, if any.
-        Model identifiers as stored in MLFlow (not including the 'models:/' prefix).
-
-    uuid: UUID
-        short for "uuid"
-
-    Raises
-    ------
-    TypeError
-        If ``func`` has any arguments without annotations, is missing a return
-        annotation, or uses ``None`` or ``Any`` as annotation.
-
-    Notes
-    -----
-    We require annotations because we need ``Step``s to be composable functions
-    in their respective ``Pipeline``s. However, due to python's highly flexible
-    ``*args`` syntax, function composition is inherently ambiguous -- e.g. if we
-    wish to compose ``f`` with ``g`,` and ``g` returns a tuple of values, should
-    that tuple be passed to ``f`` as a tuple (i.e. ``f(g(*args))``), or should
-    it be unpacked as individual arguments to ``f`` (i.e. ``f(*g(*args))``,
-    noting the extra ``*``)?
-
-    To resolve this ambiguity, we could either (a) restrict the set of acceptable
-    callables to be only those with a single argument and a single return value, or
-    (b) rely on thorough function annotations to disambiguate. While best practices
-    are likely to stick to single-input-single-output ``Step``s, we currently try
-    to support (b) by composing steps together differently if ``g` seems to be
-    returning an "argument tuple" for ``f`` as follows:
-        - ``g` has a return annotation indicating the types within the tuple:
-            e.g. ``def g(...) -> tuple[str, int, pd.DataFrame]``
-        - ``f`` has exactly those argument annotations, in the same order:
-            e.g. ``def f(x: str, y: int, z: pd.DataFrame) -> ...``
-        - if both are true, compose ``f`` with ``g`` by **unpacking the tuple when it returns**:
-            e.g. ``f(*g(*args))`` (noting the extra ``*``), otherwise ``f(g(*args))`` - like any other Step.
+    IMPORTANT:
+        When included in a ``Pipeline``, all steps will be checked for \
+        composability with respect to their argument- and return-type \
+        annotations.  This requires that the decorated function has complete \
+        argument- and return-type annotations; a ``Step`` will fail to \
+        initialize with an exception if this condition is not met. Note that \
+        there is (currently) no type-checking at runtime. \
+        See "Notes" below for additional discussion on composing steps which \
+        may take multiple arguments by returning a properly-typed `tuple` as a result.
+
+    Attributes:
+        func (Callable):
+            The well-annotated function that should be called when this ``Step`` \
+            is reached in its ``Pipeline``, which is passed the output of the \
+            previous step (if one exists) as input. This is the only required \
+            attribute, all others are optional or should not be modified.
+        title (str):
+            An official name or title for the Step. Currently, ``func.__name__`` is used as a default.
+        description (str):
+            A human-readable description of the step. Currently, ``func.__doc__`` is used as a default.
+        input_info (str):
+            Human-readable description of the input data and/or relevant
+            characteristics that *should* hold true for this step's input (e.g.
+            dimensions of a matrix or column names of a dataframe).
+        output_info (str):
+            Human-readable description of the output data and/or relevant
+            characteristics that *will* hold true for this step's output (e.g.
+            dimensions of a matrix or column names of a dataframe).
+        authors (List[str]):
+            The main researchers involved in producing the Step, for citation and discoverability purposes.
+        model_uris (List[str]):
+            A reference to the models used in this step, if any. Model identifiers are as stored in MLFlow (not including the 'models:/' prefix).
+        source (Optional[str]):
+            Should not be set by users. Consists of the plain python source code \
+            used to define `func`, if possible.
+
+    Raises:
+        TypeError:
+            If ``func`` has any arguments without annotations, is missing a return annotation, or uses ``None`` or ``Any`` as annotation.
+
+    Notes:
+        Due to python's flexible `*args` syntax, function composition can be \
+        ambiguous -- e.g. if we wish to compose `f` with `g`, and `g` returns a \
+        tuple of values, should that tuple be passed to `f` as a tuple (i.e. \
+        ``f(g(*args))``), or should it be unpacked as individual arguments to \
+        `f` (i.e. `f(*g(*args))`, noting the extra `*`)?
+
+        To resolve this ambiguity, we could either (a) restrict the set of \
+        acceptable  callables to be only those with a single argument and a \
+        single return value, or  (b) rely on function annotations to \
+        disambiguate. While best practices  are likely to stick to simpler, \
+        single-input-single-output `Step`s, we currently try  to support (b) by \
+        composing steps together differently if `g` seems to be returning an \
+        "argument tuple" for `f`. For example, if `g` returns `... -> tuple[T1, \
+        T2, T3]` and `f` is annotated `def f(a: T1, b: T2, c: T3)`, we unpack \
+        `g`'s output before passing it to `f`.
     """
 
     func: Callable
     authors: List[str] = Field(default_factory=list)
     contributors: List[str] = Field(default_factory=list)
     title: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     input_info: Optional[str] = Field(None)
     output_info: Optional[str] = Field(None)
     conda_dependencies: List[str] = Field(default_factory=list)
     pip_dependencies: List[str] = Field(default_factory=list)
     python_version: Optional[str] = Field(None)
     model_uris: List[str] = Field(default_factory=list)
+    source: Optional[str] = Field(None)
 
     def __post_init_post_parse__(self):
         # like __post_init__, but called after pydantic validation
         # copies e.g. __doc__ and __name__ from
         # the underlying callable to this object
         # (also handy for signature/annotations)
         update_wrapper(self, self.func)
@@ -210,32 +179,51 @@
                 "before being published as a Pipeline. Please try again with a more descriptive type hint.\n"
                 "We use `beartype` to resolve type hints -- for a full list of supported annotations \n "
                 "(including 3rd party type hints, like `numpy.typing`), see:\n "
                 "https://github.com/beartype/beartype#compliance"
             )
         return f
 
+    @validator("source", always=True, pre=False)
+    def has_findable_source(cls, _, values):
+        # ignores any prior value for the "source" field, populating it with the
+        # found source of `func`.  There are tons of edge cases if the user is
+        # passing an arbitrary callable directly to the Step constructor, but
+        # because only plain python can be decorated, if they're using the
+        # decorator this shouldn't be problematic.
+        if "func" in values:
+            func = values["func"]
+            try:
+                return inspect.getsource(func)
+            except (OSError, TypeError) as e:
+                raise ValueError(
+                    f"Could not find python source code for {func}. If using a \
+builtin or externally-defined function as a step, best practice is \
+to use @step to decorate a minimal function that invokes it, rather \
+than using it as a step directly."
+                ) from e
+
     def json(self) -> JSON:
         return json.dumps(self, default=garden_json_encoder)
 
     def dict(self) -> Dict[str, Any]:
         d = {}
         for key in self.__dataclass_fields__:
             val = getattr(self, key)
             d[key] = val
         return d
 
 
 def step(func: Callable = None, **kwargs):
-    """Helper: provide ``@step(...)`` decorator for creation of ``Step``s."""
+    """Helper: provide `@step` /`@step(...)` decorator for creation of `Steps`."""
     # note:
-    # The ``Step`` class itself could also technically be used as a decorator,
+    # The capital-S `Step class itself could also technically be used as a decorator,
     # but would run into trouble as soon as you tried passing any arguments:
-    # this definition means ``@step`` and ``@step(...)`` are equivalent decorators,
-    # because ``@Step`` and ``@Step(...)`` could not be.
+    # this definition means `@step` and `@step(...)` are equivalent decorators,
+    # because `@Step` and `@Step(...)` could not be.
     if func is not None:
         # called like ``@step``
         # (or ``my_func = step(my_func, **kwargs)``)
         data = {**kwargs, "func": func}
         return Step(**data)  # type: ignore
 
     else:
```

### Comparing `garden_ai-0.4.1/garden_ai/templates/pipeline` & `garden_ai-0.4.2/garden_ai/templates/pipeline`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     # TODO
     pass
 
 
 @step
 def run_inference(
     input_arg: object,
-    model=Model("YOUR MODEL's NAME HERE"),
+    model=Model("{{ scaffolded_model_name }}"),
 ) -> object:
     pass
 
 # the step functions will be composed in order by the pipeline:
 ALL_STEPS = (
     preprocessing_step,
     another_step,
```

### Comparing `garden_ai-0.4.1/garden_ai/utils/misc.py` & `garden_ai-0.4.2/garden_ai/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,21 +255,14 @@
         try:
             r = Requirement(line)
             requirements += [r]
         except InvalidRequirement:
             logger.warning(f"Could not parse requirement line: {line}")
             raise
 
-    # hack: user-dependencies like `examol @ git+https://github.com/exalearn/ExaMol.git`,
-    # which are not on pypi, should be read _before_ a line saying
-    # `examol==0.0.1` so pip won't worry that it's not on pypi, otherwise
-    # pip will claim it could not be installed.
-
-    # sorts s.t. url-based installs are read first
-    requirements.sort(key=lambda requirement: requirement.url is None)
     return [str(r) for r in requirements]
 
 
 def inject_env_kwarg(func: Callable):
     """
     Helper: modify a function so that it will accept an ``_env_vars`` keyword argument.
```

### Comparing `garden_ai-0.4.1/pyproject.toml` & `garden_ai-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "garden-ai"
-version = "0.4.1" # placeholder
+version = "0.4.2" # placeholder
 description = "Garden: tools to simplify access to scientific AI advances."
 # note to contributors: feel free to add yourselves to this list 🌱
 maintainers = [
+  "Globus Labs <labs@globus.org>",
   "Owen Price Skelly",
   "Will Engler",
   "Ben Blaiszik",
   "Ben Galewsky",
   "Eric Blau",
   "Steve Barnard"
 ]
@@ -29,15 +30,15 @@
 python = "^3.8"
 requests = "^2.20.0"
 globus-sdk = "^3.12.0"
 pydantic = "^1.10.2"
 typer = { extras = ["all"], version = "^0.7.0" }
 beartype = "^0.12.0"
 jinja2 = "^3.1.2"
-mlflow = "2.2.1"
+mlflow = "^2.3.2"
 # numba is an indirect dep of ML Flow.
 # Specifying a recent version of it helps avoid install issues on M1 Macs
 numba = "^0.56"
 boto3 = "^1.26.77"
 dparse = { extras = ["conda"], version = "^0.6.2" }
 pyyaml = "^6.0"
 packaging = "^23.0"
@@ -57,24 +58,26 @@
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
 mypy = "^0.981"
 types-requests = "^2.20.0"
 safety = "^2.3.1"
 types-pyyaml = "^6.0.12.8"
-torch = { version = "^2.0.0" }
-tensorflow = { version = "^2.11.0", python = ">=3.8,<3.12" }
 coverage = { extras = ["toml"], version = "^7.2.3" }
 
 [tool.poetry.group.develop.dependencies]
-sphinx = "4.3.2"
-sphinx-rtd-theme = "^1.0.0"
 pre-commit = "^3.1.1"
 black = "^23.1.0"
 isort = "^5.12.0"
+mkdocs = "^1.4.3"
+mkdocs-callouts = "^1.9.0"
+mkdocs-extensions = "^0.1.2"
+pymdown-extensions = "^10.0.1"
+mkdocs-material = "^9.1.13"
+mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 
 [tool.poetry.extras]
 # Be sure to add additional flavors to below as support is added and in the flavors array
 # Optional dependencies that can be added through `poetry install --extras "torch tensorflow"` etc. or `poetry install --extras "flavors"`
 # `poetry install --all-extras` will install all extras located in tool.poetry.extras
 torch = ["torch"]
 tensorflow = ["tensorflow"]
```

### Comparing `garden_ai-0.4.1/PKG-INFO` & `garden_ai-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 0.4.1
+Version: 0.4.2
 Summary: Garden: tools to simplify access to scientific AI advances.
 Home-page: https://thegardens.ai
 License: MIT
 Author: Garden Team
 Author-email: labs@globus.org
-Maintainer: Owen Price Skelly
+Maintainer: Globus Labs
+Maintainer-email: labs@globus.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,15 +20,15 @@
 Provides-Extra: torch
 Requires-Dist: beartype (>=0.12.0,<0.13.0)
 Requires-Dist: boto3 (>=1.26.77,<2.0.0)
 Requires-Dist: dparse[conda] (>=0.6.2,<0.7.0)
 Requires-Dist: globus-compute-sdk (>=2.0.0,<3.0.0)
 Requires-Dist: globus-sdk (>=3.12.0,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: mlflow (==2.2.1)
+Requires-Dist: mlflow (>=2.3.2,<3.0.0)
 Requires-Dist: numba (>=0.56,<0.57)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: tensorflow (>=2.11.0,<3.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "tensorflow" or extra == "flavors")
 Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "torch" or extra == "flavors"
```

