# Comparing `tmp/ez_cqrs-0.2.0.tar.gz` & `tmp/ez_cqrs-0.2.1.tar.gz`

## Comparing `ez_cqrs-0.2.0.tar` & `ez_cqrs-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.tool-versions
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/components.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/error.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/handler.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/ops.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/ez_cqrs/py.typed
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/tests/integration/test_execution.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/tests/unit/test_something.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/LICENSE
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/README.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ez_cqrs-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.tool-versions
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/handler.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/ops.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/py.typed
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/ez_cqrs/shared_state.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/LICENSE
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/README.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 ez_cqrs-0.2.1/PKG-INFO
```

### Comparing `ez_cqrs-0.2.0/.github/workflows/release.yml` & `ez_cqrs-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.0/.github/workflows/test.yml` & `ez_cqrs-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.0/.vscode/settings.json` & `ez_cqrs-0.2.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.0/ez_cqrs/components.py` & `ez_cqrs-0.2.1/ez_cqrs/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """CQRS core components."""
 from __future__ import annotations
 
-from abc import ABC
+import abc
 from dataclasses import dataclass
 from typing import TypeVar
 
 from mashumaro import DataClassDictMixin
 from mashumaro.mixins.orjson import DataClassORJSONMixin
 from pydantic import BaseModel
 
 
 @dataclass(frozen=True)
-class Command(DataClassDictMixin):
+class Command(abc.ABC, DataClassDictMixin):
     """
     Command baseclass.
 
     In order to make changes to our system we'll need commands. These
     are the simplest components of any CQRS system and consist of little more than
     packaged data.
     """
 
 
-class CommandValidator(BaseModel):
+class CommandValidator(abc.ABC, BaseModel):
     """Command input validator."""
 
     class Config:
         """Custom configuration."""
 
         allow_mutation = False
 
 
 @dataclass(frozen=True)
-class DomainEvent(ABC, DataClassORJSONMixin):
+class DomainEvent(abc.ABC, DataClassORJSONMixin):
     """
     Domain Event base class.
 
     A `DomainEvent` represents any business change in the state of an `Aggregate`.
     `DomainEvents` are inmutable, and when [event sourcing](https://martinfowler.com/eaaDev/EventSourcing.html)
     is used they are the single source of truth.
```

### Comparing `ez_cqrs-0.2.0/ez_cqrs/error.py` & `ez_cqrs-0.2.1/ez_cqrs/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 """Error base class."""
 from __future__ import annotations
 
+import abc
 from typing import TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     import sys
 
     if sys.version_info >= (3, 10):
         from typing import TypeAlias
     else:
         from typing_extensions import TypeAlias
 
 
-class DomainError(Exception):
+class DomainError(abc.ABC, Exception):
     """
     Raised when a user violates a business rule.
 
     This is the error returned when a user violates a business rule. The payload passed
     should be used to inform the user of the nature of a problem.
 
     This translates into a `Bad Request` status.
     """
 
 
+class DatabaseError(Exception):
+    """Raised whwne that's an error interacting with system's database."""
+
+    def __init__(self, database_error: Exception) -> None:  # noqa: D107
+        super().__init__(f"An error ocurred with database {database_error}")
+
+
 class UnexpectedError(Exception):
     """
     Raised when an unexpected error was encountered.
 
     A technical error was encountered teht prevented the command from being applied to
     the aggregate. In general the accompanying message should be logged for
     investigation rather than returned to the user.
@@ -34,9 +42,10 @@
 
     def __init__(self, unexpected_error: Exception) -> None:  # noqa: D107
         super().__init__(f"Unexpected error {unexpected_error}")
 
 
 ExecutionError: TypeAlias = Union[
     DomainError,
+    DatabaseError,
     UnexpectedError,
 ]
```

### Comparing `ez_cqrs-0.2.0/ez_cqrs/handler.py` & `ez_cqrs-0.2.1/ez_cqrs/handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 """Command handler definition."""
 from __future__ import annotations
 
 import abc
-from typing import TYPE_CHECKING, Generic
+from typing import TYPE_CHECKING, Any, Generic
 
 from ez_cqrs.components import C, E, V
 
 if TYPE_CHECKING:
     from pydantic import ValidationError
     from result import Result
 
+    from ez_cqrs.acid_exec import OpsRegistry
     from ez_cqrs.error import ExecutionError
+    from ez_cqrs.shared_state import Config
 
 
 class CommandHandler(abc.ABC, Generic[C, E, V]):
     """Command handler handles every command to complete one user intent."""
 
     @abc.abstractmethod
     def validate(
         self,
         command: C,
         schema: type[V],
     ) -> Result[None, ValidationError]:
         """Validate command data."""
 
     @abc.abstractmethod
-    async def handle(self, command: C) -> Result[list[E], ExecutionError]:
+    async def handle(
+        self,
+        command: C,
+        ops_registry: OpsRegistry[Any],
+        config: Config,
+    ) -> Result[list[E], ExecutionError]:
         """
         Consume and process commands.
 
         The result should be either a vector of events if the command is successful,
         or an error is the command is rejected.
 
         _All business logic belongs in this method_.
@@ -42,9 +49,9 @@
 
     Some examples of tasks that event dispatcher can handle:
     - updated application state views in downstream services.
     - publish events to messaging services.
     """
 
     @abc.abstractmethod
-    async def dispatch(self, event: E) -> None:
+    async def dispatch(self, event: E, config: Config) -> None:
         """Dispatch events generated by command."""
```

### Comparing `ez_cqrs-0.2.0/requirements/core.txt` & `ez_cqrs-0.2.1/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.0/requirements/dev.txt` & `ez_cqrs-0.2.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.0/scripts/new_release.py` & `ez_cqrs-0.2.1/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.0/tests/integration/conftest.py` & `ez_cqrs-0.2.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.0/tests/integration/test_execution.py` & `ez_cqrs-0.2.1/tests/integration/test_execution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Test handler."""
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Any, Union
 
 import pydantic
 import pytest
 from pydantic import ValidationError
 from result import Err, Ok, Result
 
 from ez_cqrs import ops
+from ez_cqrs.acid_exec import OpsRegistry
 from ez_cqrs.components import Command, CommandValidator, DomainEvent
 from ez_cqrs.handler import CommandHandler
+from ez_cqrs.shared_state import Config
 
 if TYPE_CHECKING:
     import sys
 
     if sys.version_info >= (3, 10):
         from typing import TypeAlias
     else:
@@ -75,15 +77,19 @@
             return Err(e)
 
         return Ok()
 
     async def handle(  # noqa: D102
         self,
         command: BankAccountCommand,
+        ops_registry: OpsRegistry[Any],
+        config: Config,
     ) -> Result[list[BankAccountEvent], ExecutionError]:
+        _ = ops_registry
+        _ = config
         if isinstance(command, OpenAccount):
             return Ok(
                 [AccountOpened(account_id=command.account_id, amount=command.amount)],
             )
         if isinstance(command, DepositMoney):
             return Ok(
                 [MoneyDeposited(account_id=command.account_id, amount=command.amount)],
@@ -125,15 +131,20 @@
     async def test_handle(
         self,
         command: BankAccountCommand,
         expected_events: list[BankAccountEvent],
     ) -> None:
         """Test handle method."""
         cmd_handler = BankAccountCommandHandler()
-        resultant_events = await cmd_handler.handle(command=command)
+        app_config = Config()
+        resultant_events = await cmd_handler.handle(
+            command=command,
+            ops_registry=OpsRegistry[Any](max_lenght=0),
+            config=app_config,
+        )
         assert resultant_events.unwrap() == expected_events
 
 
 @pytest.mark.parametrize(
     argnames=["cmd_handler", "cmd", "validator", "expected_events"],
     argvalues=[
         (
@@ -151,9 +162,11 @@
     expected_events: list[BankAccountEvent],
 ) -> None:
     """Test validate and execution cmd operation."""
     resultant_events = await ops.validate_and_execute_cmd(
         cmd_handler=cmd_handler,
         command=cmd,
         schema=validator,
+        max_transactions=0,
+        config=Config(),
     )
     assert resultant_events.unwrap() == expected_events
```

### Comparing `ez_cqrs-0.2.0/.gitignore` & `ez_cqrs-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.0/LICENSE` & `ez_cqrs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-0.2.0/pyproject.toml` & `ez_cqrs-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-0.2.0/PKG-INFO` & `ez_cqrs-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 0.2.0
+Version: 0.2.1
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

