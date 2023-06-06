# Comparing `tmp/ez_cqrs-0.2.1.tar.gz` & `tmp/ez_cqrs-0.2.2.tar.gz`

## Comparing `ez_cqrs-0.2.1.tar` & `ez_cqrs-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.tool-versions
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/components.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/error.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/handler.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/ops.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/py.typed
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/shared_state.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/LICENSE
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/README.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/.tool-versions
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/ez_cqrs/handler.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/ez_cqrs/ops.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/ez_cqrs/py.typed
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/ez_cqrs/shared_state.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/ez_cqrs/testing.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/tests/integration/conftest.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/LICENSE
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/README.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ez_cqrs-0.2.2/PKG-INFO
```

### Comparing `ez_cqrs-0.2.1/.github/workflows/release.yml` & `ez_cqrs-0.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/.github/workflows/test.yml` & `ez_cqrs-0.2.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/.vscode/settings.json` & `ez_cqrs-0.2.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/ez_cqrs/acid_exec.py` & `ez_cqrs-0.2.2/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/ez_cqrs/components.py` & `ez_cqrs-0.2.2/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/ez_cqrs/error.py` & `ez_cqrs-0.2.2/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/ez_cqrs/handler.py` & `ez_cqrs-0.2.2/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/ez_cqrs/ops.py` & `ez_cqrs-0.2.2/ez_cqrs/ops.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     config: Config,
 ) -> Result[list[E], ExecutionError | ValidationError]:
     """Validate and execute command."""
     validated = cmd_handler.validate(command=command, schema=schema)
     if not isinstance(validated, Ok):
         return Err(validated.err())
 
+    ops_registry = OpsRegistry[Any](max_lenght=max_transactions)
     resultant_events = await cmd_handler.handle(
         command=command,
-        ops_registry=OpsRegistry[Any](max_lenght=max_transactions),
+        ops_registry=ops_registry,
         config=config,
     )
     if not isinstance(resultant_events, Ok):
         return Err(resultant_events.err())
+
     return Ok(resultant_events.unwrap())
```

### Comparing `ez_cqrs-0.2.1/ez_cqrs/shared_state.py` & `ez_cqrs-0.2.2/ez_cqrs/shared_state.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/requirements/core.txt` & `ez_cqrs-0.2.2/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/requirements/dev.txt` & `ez_cqrs-0.2.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/scripts/new_release.py` & `ez_cqrs-0.2.2/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/tests/integration/conftest.py` & `ez_cqrs-0.2.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/tests/integration/test_execution.py` & `ez_cqrs-0.2.2/tests/integration/test_execution.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from result import Err, Ok, Result
 
 from ez_cqrs import ops
 from ez_cqrs.acid_exec import OpsRegistry
 from ez_cqrs.components import Command, CommandValidator, DomainEvent
 from ez_cqrs.handler import CommandHandler
 from ez_cqrs.shared_state import Config
+from ez_cqrs.testing import Framework
 
 if TYPE_CHECKING:
     import sys
 
     if sys.version_info >= (3, 10):
         from typing import TypeAlias
     else:
@@ -139,34 +140,70 @@
         resultant_events = await cmd_handler.handle(
             command=command,
             ops_registry=OpsRegistry[Any](max_lenght=0),
             config=app_config,
         )
         assert resultant_events.unwrap() == expected_events
 
+    @pytest.mark.parametrize(
+        argnames=["cmd_handler", "cmd", "validator", "expected_events"],
+        argvalues=[
+            (
+                BankAccountCommandHandler(),
+                OpenAccount(account_id="123", amount=1),
+                OpenAccountValidator,
+                [AccountOpened(account_id="123", amount=1)],
+            ),
+        ],
+    )
+    async def test_validate_and_execute_cmd(
+        self,
+        cmd_handler: BankAccountCommandHandler,
+        cmd: BankAccountCommand,
+        validator: type[BankAccountValidator],
+        expected_events: list[BankAccountEvent],
+    ) -> None:
+        """Test validate and execution cmd operation."""
+        resultant_events = await ops.validate_and_execute_cmd(
+            cmd_handler=cmd_handler,
+            command=cmd,
+            schema=validator,
+            max_transactions=0,
+            config=Config(),
+        )
+        assert resultant_events.unwrap() == expected_events
 
-@pytest.mark.parametrize(
-    argnames=["cmd_handler", "cmd", "validator", "expected_events"],
-    argvalues=[
-        (
-            BankAccountCommandHandler(),
-            OpenAccount(account_id="123", amount=1),
-            OpenAccountValidator,
-            [AccountOpened(account_id="123", amount=1)],
-        ),
-    ],
-)
-async def test_validate_and_execute_cmd(
-    cmd_handler: BankAccountCommandHandler,
-    cmd: BankAccountCommand,
-    validator: type[BankAccountValidator],
-    expected_events: list[BankAccountEvent],
-) -> None:
-    """Test validate and execution cmd operation."""
-    resultant_events = await ops.validate_and_execute_cmd(
-        cmd_handler=cmd_handler,
-        command=cmd,
-        schema=validator,
-        max_transactions=0,
-        config=Config(),
+    @pytest.mark.parametrize(
+        argnames=["cmd_handler", "cmd", "validator", "expected_events"],
+        argvalues=[
+            (
+                BankAccountCommandHandler(),
+                OpenAccount(account_id="123", amount=1),
+                OpenAccountValidator,
+                [AccountOpened(account_id="123", amount=1)],
+            ),
+        ],
     )
-    assert resultant_events.unwrap() == expected_events
+    async def test_with_framework(
+        self,
+        cmd_handler: BankAccountCommandHandler,
+        cmd: BankAccountCommand,
+        validator: type[BankAccountValidator],
+        expected_events: list[BankAccountEvent],
+    ) -> None:
+        """Test validate command with testing framework."""
+        framework = Framework[
+            BankAccountCommand,
+            BankAccountEvent,
+            BankAccountValidator,
+        ](
+            cmd_handler=cmd_handler,
+            cmd=cmd,
+            schema_validator=validator,
+        )
+
+        assert framework.validate().then_expect_is_valid()
+        await framework.execute(
+            max_transactions=0,
+            config=Config(),
+        )
+        assert framework.then_expect_events(expected_events=expected_events)
```

### Comparing `ez_cqrs-0.2.1/tests/unit/test_acid_exec.py` & `ez_cqrs-0.2.2/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/.gitignore` & `ez_cqrs-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/LICENSE` & `ez_cqrs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.1/pyproject.toml` & `ez_cqrs-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-0.2.1/PKG-INFO` & `ez_cqrs-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 0.2.1
+Version: 0.2.2
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

