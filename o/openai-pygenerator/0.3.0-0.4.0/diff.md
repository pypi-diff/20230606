# Comparing `tmp/openai-pygenerator-0.3.0.tar.gz` & `tmp/openai-pygenerator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-pygenerator-0.3.0.tar", last modified: Wed May 24 10:24:15 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.4.0.tar", last modified: Tue Jun  6 11:15:07 2023, max compression
```

## Comparing `openai-pygenerator-0.3.0.tar` & `openai-pygenerator-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.696676 openai-pygenerator-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-24 10:24:15.704676 openai-pygenerator-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/src/openai_pygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/src/openai_pygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/src/openai_pygenerator/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/src/openai_pygenerator/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 10:24:15.000000 openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:24:15.700676 openai-pygenerator-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-24 10:24:03.000000 openai-pygenerator-0.3.0/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-06 11:15:07.395856 openai-pygenerator-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/src/openai_pygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/src/openai_pygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/src/openai_pygenerator/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/src/openai_pygenerator/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 11:15:07.000000 openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:15:07.391857 openai-pygenerator-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-06 11:14:57.000000 openai-pygenerator-0.4.0/tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.3.0/.github/workflows/python-package.yml` & `openai-pygenerator-0.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.3.0/.github/workflows/python-publish.yml` & `openai-pygenerator-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.3.0/.pre-commit-config.yaml` & `openai-pygenerator-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.3.0/.pylintrc` & `openai-pygenerator-0.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.3.0/LICENSE.txt` & `openai-pygenerator-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.3.0/pyproject.toml` & `openai-pygenerator-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.3.0/src/openai_pygenerator/openai_pygenerator.py` & `openai-pygenerator-0.4.0/src/openai_pygenerator/openai_pygenerator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import logging
 import os
 import time
-from typing import Callable, Dict, Iterable, Iterator, List, NewType, TypeVar
+from enum import Enum, auto
+from typing import Callable, Dict, Iterable, Iterator, List, NewType, Optional, TypeVar
 
 import openai
 from openai.error import APIError, RateLimitError
 
 Completion = Dict[str, str]
 Seconds = NewType("Seconds", int)
 Completions = Iterator[Completion]
 History = Iterable[Completion]
 Completer = Callable[[History, int], Completions]
 T = TypeVar("T")
 
 
+class Role(Enum):
+    USER = auto()
+    ASSISTANT = auto()
+
+
 def var(name: str, to_type: Callable[[str], T], default: T) -> T:
     result = os.environ.get(name)
     if result is None:
         return default
     return to_type(result)
 
 
@@ -102,20 +108,49 @@
             ):
                 yield completion
         else:
             logger.error("Maximum retries reached, aborting.")
             raise
 
 
-def user_message(content: str) -> Completion:
-    return {"role": "user", "content": content}
+def next_completion(completions: Completions) -> Optional[Completion]:
+    try:
+        return next(completions)
+    except StopIteration:
+        return None
+
+
+def user_message(text: str) -> Completion:
+    return {"role": "user", "content": text}
+
+
+def content(completion: Completion) -> str:
+    return completion["content"]
+
+
+def role(completion: Completion) -> Role:
+    r = completion["role"]
+    if r == "user":
+        return Role.USER
+    elif r == "assistant":
+        return Role.ASSISTANT
+    else:
+        raise ValueError(f"Cannot determine role from {r}")
+
+
+def is_user_role(completion: Completion) -> bool:
+    return role(completion) == Role.USER
+
+
+def is_assistant_role(completion: Completion) -> bool:
+    return role(completion) == Role.ASSISTANT
 
 
 def transcript(messages: History) -> List[str]:
-    return [r["content"] for r in messages]
+    return [content(r) for r in messages]
 
 
 class ChatSession:
     """Encapsulates chat session state
 
     :param generate: A function to generate completions from a history
     """
```

### Comparing `openai-pygenerator-0.3.0/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.4.0/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.3.0/tests/test_gpt.py` & `openai-pygenerator-0.4.0/tests/test_gpt.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,16 +6,22 @@
 from openai.error import APIError, RateLimitError
 from openai.openai_object import OpenAIObject
 
 from openai_pygenerator import (
     GPT_MAX_RETRIES,
     ChatSession,
     Completer,
+    Completion,
     Completions,
+    Role,
+    content,
     gpt_completions,
+    is_assistant_role,
+    is_user_role,
+    role,
     transcript,
     user_message,
 )
 
 
 def aio(text: str) -> OpenAIObject:
     result = OpenAIObject()
@@ -35,14 +41,24 @@
 
 
 @pytest.fixture
 def mock_sleep(mocker):
     return mocker.patch("time.sleep", return_value=None)
 
 
+@pytest.fixture
+def assistant_completion():
+    return {"role": "assistant", "content": "testing"}
+
+
+@pytest.fixture
+def user_completion():
+    return {"role": "user", "content": "testing"}
+
+
 @pytest.mark.parametrize(
     "error",
     [
         RateLimitError("rate limited", http_status=429),
         APIError("Gateway Timeout", http_status=524),
     ],
 )
@@ -107,7 +123,19 @@
     assert result == "response2"
     assert session.transcript == [
         "First question",
         "response1",
         "Second question",
         "response2",
     ]
+
+
+def test_content(user_completion: Completion, assistant_completion: Completion):
+    assert content(user_completion) == "testing"
+    assert content(assistant_completion) == "testing"
+
+
+def test_role(user_completion: Completion, assistant_completion: Completion):
+    assert role(user_completion) == Role.USER
+    assert role(assistant_completion) == Role.ASSISTANT
+    assert is_user_role(user_completion)
+    assert is_assistant_role(assistant_completion)
```

