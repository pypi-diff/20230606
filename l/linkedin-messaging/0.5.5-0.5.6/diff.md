# Comparing `tmp/linkedin-messaging-0.5.5.tar.gz` & `tmp/linkedin-messaging-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedin-messaging-0.5.5.tar", last modified: Wed Mar 15 05:01:28 2023, max compression
+gzip compressed data, was "linkedin-messaging-0.5.6.tar", last modified: Tue Jun  6 04:34:28 2023, max compression
```

## Comparing `linkedin-messaging-0.5.5.tar` & `linkedin-messaging-0.5.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      386 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/.editorconfig
--rw-r--r--   0        0        0      782 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/.envrc
--rw-r--r--   0        0        0      205 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/.github/dependabot.yml
--rw-r--r--   0        0        0     2288 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/.github/workflows/python.yaml
--rw-r--r--   0        0        0     2287 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/.gitignore
--rw-r--r--   0        0        0     1132 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      240 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/.vim/coc-settings.json
--rw-r--r--   0        0        0     3615 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/CHANGELOG.md
--rw-r--r--   0        0        0    11358 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/LICENSE
--rw-r--r--   0        0        0      888 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/README.md
--rwxr-xr-x   0        0        0     1878 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/cicd/custom_style_check.py
--rw-r--r--   0        0        0     3833 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/dev-requirements.txt
--rw-r--r--   0        0        0     1284 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/examples/get-conversation.py
--rw-r--r--   0        0        0     1818 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/examples/listen-for-events.py
--rw-r--r--   0        0        0      870 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/examples/manual-login.py
--rw-r--r--   0        0        0      955 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/examples/mark-conversation-as-read.py
--rw-r--r--   0        0        0      823 2023-03-15 05:01:11.298362 linkedin-messaging-0.5.5/examples/pickle-example.py
--rw-r--r--   0        0        0     1332 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/examples/redact-message.py
--rw-r--r--   0        0        0     1478 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/examples/send-message.py
--rw-r--r--   0        0        0     1730 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/examples/send-reaction.py
--rw-r--r--   0        0        0      542 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/examples/simple-2fa.py
--rw-r--r--   0        0        0      447 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/linkedin_messaging/__init__.py
--rw-r--r--   0        0        0    16788 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/linkedin_messaging/api_objects.py
--rw-r--r--   0        0        0       48 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/linkedin_messaging/exceptions.py
--rw-r--r--   0        0        0    20911 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/linkedin_messaging/linkedin.py
--rw-r--r--   0        0        0        0 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/linkedin_messaging/py.typed
--rw-r--r--   0        0        0     1952 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1060 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/requirements.txt
--rw-r--r--   0        0        0      224 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/setup.cfg
--rw-r--r--   0        0        0      228 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/shell.nix
--rw-r--r--   0        0        0      321 2023-03-15 05:01:11.302362 linkedin-messaging-0.5.5/tests/test_urn.py
--rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 linkedin-messaging-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      386 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.editorconfig
+-rw-r--r--   0        0        0      782 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.envrc
+-rw-r--r--   0        0        0      205 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.github/dependabot.yml
+-rw-r--r--   0        0        0     2288 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     2287 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1133 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      240 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.vim/coc-settings.json
+-rw-r--r--   0        0        0     3742 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/CHANGELOG.md
+-rw-r--r--   0        0        0    11358 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/LICENSE
+-rw-r--r--   0        0        0      888 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/README.md
+-rwxr-xr-x   0        0        0     1878 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/cicd/custom_style_check.py
+-rw-r--r--   0        0        0     3832 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/dev-requirements.txt
+-rw-r--r--   0        0        0     1284 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/get-conversation.py
+-rw-r--r--   0        0        0     1818 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/listen-for-events.py
+-rw-r--r--   0        0        0      870 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/manual-login.py
+-rw-r--r--   0        0        0      955 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/mark-conversation-as-read.py
+-rw-r--r--   0        0        0      823 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/pickle-example.py
+-rw-r--r--   0        0        0     1332 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/redact-message.py
+-rw-r--r--   0        0        0     1478 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/send-message.py
+-rw-r--r--   0        0        0     1730 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/send-reaction.py
+-rw-r--r--   0        0        0      542 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/simple-2fa.py
+-rw-r--r--   0        0        0      447 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/linkedin_messaging/__init__.py
+-rw-r--r--   0        0        0    17222 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/linkedin_messaging/api_objects.py
+-rw-r--r--   0        0        0       48 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/linkedin_messaging/exceptions.py
+-rw-r--r--   0        0        0    20911 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/linkedin_messaging/linkedin.py
+-rw-r--r--   0        0        0        0 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/linkedin_messaging/py.typed
+-rw-r--r--   0        0        0     1803 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1060 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/requirements.txt
+-rw-r--r--   0        0        0      224 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/setup.cfg
+-rw-r--r--   0        0        0      228 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/shell.nix
+-rw-r--r--   0        0        0      321 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/tests/test_urn.py
+-rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 linkedin-messaging-0.5.6/PKG-INFO
```

### Comparing `linkedin-messaging-0.5.5/.envrc` & `linkedin-messaging-0.5.6/.envrc`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/.github/workflows/python.yaml` & `linkedin-messaging-0.5.6/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/.gitignore` & `linkedin-messaging-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/.pre-commit-config.yaml` & `linkedin-messaging-0.5.6/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
       - id: trailing-whitespace
         exclude_types: [markdown]
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.9.2
+    rev: 0.11.2
     hooks:
       - id: pyproject-fmt
 
   # black
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         files: ^(linkedin_messaging|tests)/.*$
 
   # isort
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
@@ -32,15 +32,15 @@
     rev: 6.0.0
     hooks:
       - id: flake8
         files: ^(linkedin_messaging|tests)/.*$
 
   # mypy
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.3.0
     hooks:
       - id: mypy
         additional_dependencies: [types-termcolor==1.1.3]
 
   # custom style checks
   - repo: local
     hooks:
```

### Comparing `linkedin-messaging-0.5.5/CHANGELOG.md` & `linkedin-messaging-0.5.6/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# v0.5.6
+
+* Added objects to support voice messages.
+* Updated versions of many dependencies and all of the pre-commit hooks.
+
 # v0.5.5
 
 * Add back support for the `TIMEOUT` special event. All other errors still need
   to be handled by API consumers.
 
 # v0.5.4
```

### Comparing `linkedin-messaging-0.5.5/LICENSE` & `linkedin-messaging-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/README.md` & `linkedin-messaging-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/cicd/custom_style_check.py` & `linkedin-messaging-0.5.6/cicd/custom_style_check.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/dev-requirements.txt` & `linkedin-messaging-0.5.6/dev-requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,41 +12,41 @@
     # via aiohttp
 attrs==22.2.0
     # via
     #   aiohttp
     #   flake8-annotations
     #   flake8-bugbear
     #   pytest
-beautifulsoup4==4.11.2
+beautifulsoup4==4.12.2
     # via linkedin_messaging (pyproject.toml)
-black==23.1.0
+black==23.3.0
     # via linkedin_messaging (pyproject.toml)
 build==0.10.0
     # via pip-tools
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   aiohttp
     #   requests
 click==8.1.3
     # via
     #   black
     #   pip-tools
-coverage[toml]==7.2.1
+coverage[toml]==7.2.5
     # via pytest-cov
 dataclasses-json==0.5.7
     # via linkedin_messaging (pyproject.toml)
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via flit
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 filelock==3.9.0
     # via virtualenv
 flake8==6.0.0
     # via
     #   flake8-annotations
     #   flake8-bugbear
@@ -55,15 +55,15 @@
     #   flake8-pep3101
     #   flake8-print
     #   linkedin_messaging (pyproject.toml)
 flake8-annotations==3.0.0
     # via linkedin_messaging (pyproject.toml)
 flake8-bugbear==23.3.12
     # via linkedin_messaging (pyproject.toml)
-flake8-comprehensions==3.10.1
+flake8-comprehensions==3.12.0
     # via linkedin_messaging (pyproject.toml)
 flake8-isort==6.0.0
     # via linkedin_messaging (pyproject.toml)
 flake8-pep3101==2.0.0
     # via linkedin_messaging (pyproject.toml)
 flake8-print==5.0.0
     # via linkedin_messaging (pyproject.toml)
@@ -71,15 +71,15 @@
     # via linkedin_messaging (pyproject.toml)
 flit-core==3.8.0
     # via flit
 frozenlist==1.3.3
     # via
     #   aiohttp
     #   aiosignal
-identify==2.5.20
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   requests
     #   yarl
 iniconfig==2.0.0
     # via pytest
@@ -95,40 +95,40 @@
     # via dataclasses-json
 mccabe==0.7.0
     # via flake8
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
-mypy==1.0.1
+mypy==1.3.0
     # via linkedin_messaging (pyproject.toml)
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
     #   typing-inspect
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   marshmallow
     #   pytest
-pathspec==0.11.0
+pathspec==0.11.1
     # via black
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via linkedin_messaging (pyproject.toml)
 platformdirs==3.1.1
     # via
     #   black
     #   virtualenv
 pluggy==1.0.0
     # via pytest
-pre-commit==3.1.1
+pre-commit==3.3.2
     # via linkedin_messaging (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   flake8
     #   flake8-print
 pyflakes==3.0.1
     # via flake8
@@ -154,28 +154,28 @@
     #   build
     #   coverage
     #   mypy
     #   pyproject-hooks
     #   pytest
 tomli-w==1.0.0
     # via flit
-types-termcolor==1.1.6.1
+types-termcolor==1.1.6.2
     # via linkedin_messaging (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   black
     #   mypy
     #   typing-inspect
-typing-inspect==0.8.0
+typing-inspect==0.9.0
     # via dataclasses-json
-urllib3==1.26.14
+urllib3==1.26.15
     # via requests
 virtualenv==20.21.0
     # via pre-commit
-wheel==0.38.4
+wheel==0.40.0
     # via pip-tools
 yarl==1.8.2
     # via aiohttp
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `linkedin-messaging-0.5.5/examples/get-conversation.py` & `linkedin-messaging-0.5.6/examples/get-conversation.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/examples/listen-for-events.py` & `linkedin-messaging-0.5.6/examples/listen-for-events.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/examples/manual-login.py` & `linkedin-messaging-0.5.6/examples/manual-login.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/examples/mark-conversation-as-read.py` & `linkedin-messaging-0.5.6/examples/mark-conversation-as-read.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/examples/pickle-example.py` & `linkedin-messaging-0.5.6/examples/pickle-example.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/examples/redact-message.py` & `linkedin-messaging-0.5.6/examples/redact-message.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/examples/send-message.py` & `linkedin-messaging-0.5.6/examples/send-message.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/examples/send-reaction.py` & `linkedin-messaging-0.5.6/examples/send-reaction.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/examples/simple-2fa.py` & `linkedin-messaging-0.5.6/examples/simple-2fa.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/linkedin_messaging/api_objects.py` & `linkedin-messaging-0.5.6/linkedin_messaging/api_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,29 @@
     media_type: str = ""
     name: str = ""
     reference: Optional[MessageAttachmentReference] = None
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL, undefined=Undefined.EXCLUDE)
 @dataclass
+class AudioMetadata:
+    urn: Optional[URN]
+    duration: int = 0
+    url: str = ""
+
+
+@dataclass_json(letter_case=LetterCase.CAMEL, undefined=Undefined.EXCLUDE)
+@dataclass
+class MediaAttachment:
+    media_type: str = ""
+    audio_metadata: Optional[AudioMetadata] = None
+
+
+@dataclass_json(letter_case=LetterCase.CAMEL, undefined=Undefined.EXCLUDE)
+@dataclass
 class GifInfo:
     original_height: int = 0
     original_width: int = 0
     url: str = ""
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL, undefined=Undefined.EXCLUDE)
@@ -388,14 +403,15 @@
     body: str = ""
     feed_update: Optional[FeedUpdate] = None
     message_body_render_format: str = ""
     subject: Optional[str] = None
     recalled_at: Optional[datetime] = None
     attributed_body: Optional[AttributedBody] = None
     attachments: list[MessageAttachment] = field(default_factory=list)
+    media_attachments: list[MediaAttachment] = field(default_factory=list)
     custom_content: Optional[MessageCustomContent] = None
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL, undefined=Undefined.EXCLUDE)
 @dataclass
 class EventContent:
     message_event: Optional[MessageEvent] = field(
```

### Comparing `linkedin-messaging-0.5.5/linkedin_messaging/linkedin.py` & `linkedin-messaging-0.5.6/linkedin_messaging/linkedin.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.5/pyproject.toml` & `linkedin-messaging-0.5.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -11,29 +11,26 @@
   "LinkedIn",
   "messaging",
 ]
 license = { file = "LICENSE" }
 authors = [
     { name = "Sumner Evans", email = "sumner@beeper.com" },
 ]
-requires-python = ">=3.9,<4"
+requires-python = ">=3.9"
 classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Framework :: AsyncIO",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Topic :: Communications :: Chat",
-    "Topic :: Software Development :: Libraries",
+  "Development Status :: 3 - Alpha",
+  "Framework :: AsyncIO",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: Apache Software License",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Topic :: Communications :: Chat",
+  "Topic :: Software Development :: Libraries",
 ]
 dynamic = [
   "description",
   "version",
 ]
 dependencies = [
   "aiohttp",
```

### Comparing `linkedin-messaging-0.5.5/requirements.txt` & `linkedin-messaging-0.5.6/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via linkedin_messaging (pyproject.toml)
 aiosignal==1.3.1
     # via aiohttp
 async-timeout==4.0.2
     # via aiohttp
 attrs==22.2.0
     # via aiohttp
-beautifulsoup4==4.11.2
+beautifulsoup4==4.12.2
     # via linkedin_messaging (pyproject.toml)
 charset-normalizer==3.1.0
     # via aiohttp
 dataclasses-json==0.5.7
     # via linkedin_messaging (pyproject.toml)
 frozenlist==1.3.3
     # via
@@ -32,17 +32,17 @@
     # via dataclasses-json
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
 mypy-extensions==1.0.0
     # via typing-inspect
-packaging==23.0
+packaging==23.1
     # via marshmallow
 soupsieve==2.4
     # via beautifulsoup4
 typing-extensions==4.5.0
     # via typing-inspect
-typing-inspect==0.8.0
+typing-inspect==0.9.0
     # via dataclasses-json
 yarl==1.8.2
     # via aiohttp
```

### Comparing `linkedin-messaging-0.5.5/PKG-INFO` & `linkedin-messaging-0.5.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: linkedin-messaging
-Version: 0.5.5
+Version: 0.5.6
 Summary: An unofficial API for interacting with LinkedIn Messaging
 Keywords: LinkedIn,messaging
 Author-email: Sumner Evans <sumner@beeper.com>
-Requires-Python: >=3.9,<4
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiohttp
 Requires-Dist: beautifulsoup4
 Requires-Dist: dataclasses-json
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
```

