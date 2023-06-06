# Comparing `tmp/openai-pygenerator-0.4.0.tar.gz` & `tmp/openai-pygenerator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-pygenerator-0.4.0.tar", last modified: Tue Jun  6 11:15:07 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.4.1.tar", last modified: Tue Jun  6 18:45:23 2023, max compression
```

## Comparing `openai-pygenerator-0.4.0.tar` & `openai-pygenerator-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-06 11:15:07.395856 openai-pygenerator-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/src/openai_pygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/src/openai_pygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/src/openai_pygenerator/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/src/openai_pygenerator/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.666353 openai-pygenerator-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.662352 openai-pygenerator-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.662352 openai-pygenerator-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-06 18:45:23.666353 openai-pygenerator-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-06 18:45:23.666353 openai-pygenerator-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.662352 openai-pygenerator-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.662352 openai-pygenerator-0.4.1/src/openai_pygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/src/openai_pygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/src/openai_pygenerator/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/src/openai_pygenerator/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.666353 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.666353 openai-pygenerator-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.4.0/.github/workflows/python-package.yml` & `openai-pygenerator-0.4.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.0/.github/workflows/python-publish.yml` & `openai-pygenerator-0.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.0/.pre-commit-config.yaml` & `openai-pygenerator-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.0/.pylintrc` & `openai-pygenerator-0.4.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.0/LICENSE.txt` & `openai-pygenerator-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.0/PKG-INFO` & `openai-pygenerator-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.4.0/README.md` & `openai-pygenerator-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.0/pyproject.toml` & `openai-pygenerator-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.0/src/openai_pygenerator/example.py` & `openai-pygenerator-0.4.1/src/openai_pygenerator/example.py`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.0/src/openai_pygenerator/openai_pygenerator.py` & `openai-pygenerator-0.4.1/src/openai_pygenerator/openai_pygenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 Completer = Callable[[History, int], Completions]
 T = TypeVar("T")
 
 
 class Role(Enum):
     USER = auto()
     ASSISTANT = auto()
+    SYSTEM = auto()
 
 
 def var(name: str, to_type: Callable[[str], T], default: T) -> T:
     result = os.environ.get(name)
     if result is None:
         return default
     return to_type(result)
@@ -129,14 +130,16 @@
 
 def role(completion: Completion) -> Role:
     r = completion["role"]
     if r == "user":
         return Role.USER
     elif r == "assistant":
         return Role.ASSISTANT
+    elif r == "system":
+        return Role.SYSTEM
     else:
         raise ValueError(f"Cannot determine role from {r}")
 
 
 def is_user_role(completion: Completion) -> bool:
     return role(completion) == Role.USER
 
@@ -168,15 +171,15 @@
         :return: The assistant response
         """
         message = user_message(prompt)
         self._messages.append(message)
         completions = self._generate(self.messages, 1)
         response = next(completions)
         self._messages.append(response)
-        return response["content"]
+        return content(response)
 
     @property
     def transcript(self) -> List[str]:
         return transcript(self.messages)
 
     @property
     def messages(self) -> History:
```

### Comparing `openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/PKG-INFO` & `openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.0/tests/test_gpt.py` & `openai-pygenerator-0.4.1/tests/test_gpt.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,16 +11,14 @@
     ChatSession,
     Completer,
     Completion,
     Completions,
     Role,
     content,
     gpt_completions,
-    is_assistant_role,
-    is_user_role,
     role,
     transcript,
     user_message,
 )
 
 
 def aio(text: str) -> OpenAIObject:
@@ -41,22 +39,16 @@
 
 
 @pytest.fixture
 def mock_sleep(mocker):
     return mocker.patch("time.sleep", return_value=None)
 
 
-@pytest.fixture
-def assistant_completion():
-    return {"role": "assistant", "content": "testing"}
-
-
-@pytest.fixture
-def user_completion():
-    return {"role": "user", "content": "testing"}
+def make_test_completion(role: str) -> Completion:
+    return {"role": role, "content": "testing"}
 
 
 @pytest.mark.parametrize(
     "error",
     [
         RateLimitError("rate limited", http_status=429),
         APIError("Gateway Timeout", http_status=524),
@@ -125,17 +117,20 @@
         "First question",
         "response1",
         "Second question",
         "response2",
     ]
 
 
-def test_content(user_completion: Completion, assistant_completion: Completion):
-    assert content(user_completion) == "testing"
-    assert content(assistant_completion) == "testing"
+@pytest.mark.parametrize("role", ["user", "system", "assistant"])
+def test_content(role: str):
+    completion = make_test_completion(role)
+    assert content(completion) == "testing"
 
 
-def test_role(user_completion: Completion, assistant_completion: Completion):
-    assert role(user_completion) == Role.USER
-    assert role(assistant_completion) == Role.ASSISTANT
-    assert is_user_role(user_completion)
-    assert is_assistant_role(assistant_completion)
+@pytest.mark.parametrize(
+    "test_role_str, expected",
+    [("user", Role.USER), ("system", Role.SYSTEM), ("assistant", Role.ASSISTANT)],
+)
+def test_role(test_role_str: str, expected: Role):
+    completion = make_test_completion(test_role_str)
+    assert role(completion) == expected
```

