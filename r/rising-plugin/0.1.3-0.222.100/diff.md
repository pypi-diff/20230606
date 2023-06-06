# Comparing `tmp/rising_plugin-0.1.3.tar.gz` & `tmp/rising_plugin-0.222.100.tar.gz`

## Comparing `rising_plugin-0.1.3.tar` & `rising_plugin-0.222.100.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/.idea/.gitignore
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/.idea/Rising_Plugin.iml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/.idea/vcs.xml
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/.idea/workspace.xml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/__init__.py
--rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/csv_embed.py
--rwxr-xr-x   0        0        0     1756 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/image_embedding.py
--rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/pinecone_engine.py
--rwxr-xr-x   0        0        0     3604 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/risingplugin.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/common/__init__.py
--rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/common/utils.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/guardrails-config/__init__.py
--rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/guardrails-config/config.yml
--rwxr-xr-x   0        0        0      552 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/guardrails-config/general.co
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/guardrails-config/off-security.co
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/guardrails-config/actions/__init__.py
--rwxr-xr-x   0        0        0     3026 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/guardrails-config/actions/actions.py
--rwxr-xr-x   0        0        0     2415 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/guardrails-config/actions/phone.csv
--rwxr-xr-x   0        0        0   486145 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/src/rising_plugin/guardrails-config/actions/phone.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/tests/__init__.py
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/LICENSE
--rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/README.md
--rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 rising_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/.gitignore
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/Rising_Plugin.iml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/vcs.xml
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/workspace.xml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/__init__.py
+-rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/csv_embed.py
+-rwxr-xr-x   0        0        0     1756 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/image_embedding.py
+-rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/pinecone_engine.py
+-rwxr-xr-x   0        0        0     3604 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/risingplugin.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/common/__init__.py
+-rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/common/utils.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/__init__.py
+-rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/config.yml
+-rwxr-xr-x   0        0        0      552 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/general.co
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/off-security.co
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/__init__.py
+-rwxr-xr-x   0        0        0     3030 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/actions.py
+-rwxr-xr-x   0        0        0     2415 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/phone.csv
+-rwxr-xr-x   0        0        0   486145 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/phone.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/tests/__init__.py
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/LICENSE
+-rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/README.md
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/pyproject.toml
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 rising_plugin-0.222.100/PKG-INFO
```

### Comparing `rising_plugin-0.1.3/.idea/workspace.xml` & `rising_plugin-0.222.100/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `rising_plugin-0.1.3/.idea/workspace.xml` & `rising_plugin-0.222.100/.idea/workspace.xml`

```diff
@@ -85,15 +85,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="ed398cd8-e9f5-42d3-bcf0-bd7cc45baf32" name="Changes" comment=""/>
       <created>1685979036747</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1685979036747</updated>
-      <workItem from="1685979037968" duration="10898000"/>
+      <workItem from="1685979037968" duration="7567000"/>
     </task>
     <task id="LOCAL-00001" summary="Initial Commit">
       <created>1685979134698</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1685979134698</updated>
```

### Comparing `rising_plugin-0.1.3/.idea/inspectionProfiles/Project_Default.xml` & `rising_plugin-0.222.100/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/src/rising_plugin/csv_embed.py` & `rising_plugin-0.222.100/src/rising_plugin/csv_embed.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/src/rising_plugin/image_embedding.py` & `rising_plugin-0.222.100/src/rising_plugin/image_embedding.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/src/rising_plugin/pinecone_engine.py` & `rising_plugin-0.222.100/src/rising_plugin/pinecone_engine.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/src/rising_plugin/risingplugin.py` & `rising_plugin-0.222.100/src/rising_plugin/risingplugin.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/src/rising_plugin/common/utils.py` & `rising_plugin-0.222.100/src/rising_plugin/common/utils.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/src/rising_plugin/guardrails-config/config.yml` & `rising_plugin-0.222.100/src/rising_plugin/guardrails-config/config.yml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/src/rising_plugin/guardrails-config/general.co` & `rising_plugin-0.222.100/src/rising_plugin/guardrails-config/general.co`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/src/rising_plugin/guardrails-config/actions/actions.py` & `rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 from rising_plugin.image_embedding import (
     query_image_text,
 )
 
 from nemoguardrails.actions import action
 
-from rising_plugin.common.utils import COMMAND_BROWSER_OPEN
+from src.rising_plugin.common.utils import COMMAND_BROWSER_OPEN
 
 
 @action()
 async def general_question(query, model, uuid, image_search):
     llm = ChatOpenAI(model_name=model, temperature=0, openai_api_key=OPENAI_API_KEY)
     chain = load_qa_chain(llm, chain_type="stuff")
     file_path = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `rising_plugin-0.1.3/src/rising_plugin/guardrails-config/actions/phone.csv` & `rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/phone.csv`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/src/rising_plugin/guardrails-config/actions/phone.json` & `rising_plugin-0.222.100/src/rising_plugin/guardrails-config/actions/phone.json`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/LICENSE` & `rising_plugin-0.222.100/LICENSE`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.1.3/pyproject.toml` & `rising_plugin-0.222.100/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rising_plugin"
-version = "0.1.3"
+version = "0.222.100"
 authors = [
   { name="Thomas Richardson", email="thomasr37oss@gmail.com" },
 ]
 description = "It is a plugin for Rising GPT"
 readme = "README.md"
 dependencies = [
     "langchain >= 0.0.148",
```

### Comparing `rising_plugin-0.1.3/PKG-INFO` & `rising_plugin-0.222.100/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rising_plugin
-Version: 0.1.3
+Version: 0.222.100
 Summary: It is a plugin for Rising GPT
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Thomas Richardson <thomasr37oss@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

