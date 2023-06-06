# Comparing `tmp/colt-0.9.2.tar.gz` & `tmp/colt-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colt-0.9.2.tar", max compression
+gzip compressed data, was "colt-0.9.3.tar", max compression
```

## Comparing `colt-0.9.2.tar` & `colt-0.9.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-02-04 06:38:14.964125 colt-0.9.2/LICENSE
--rw-r--r--   0        0        0     3330 2023-02-04 06:38:14.964125 colt-0.9.2/README.md
--rw-r--r--   0        0        0     1225 2023-02-04 06:38:14.964125 colt-0.9.2/colt/__init__.py
--rw-r--r--   0        0        0     9366 2023-02-04 06:38:14.964125 colt-0.9.2/colt/builder.py
--rw-r--r--   0        0        0      695 2023-02-04 06:38:14.964125 colt-0.9.2/colt/default_registry.py
--rw-r--r--   0        0        0       67 2023-02-04 06:38:14.964125 colt-0.9.2/colt/error.py
--rw-r--r--   0        0        0      631 2023-02-04 06:38:14.964125 colt-0.9.2/colt/lazy.py
--rw-r--r--   0        0        0        0 2023-02-04 06:38:14.964125 colt-0.9.2/colt/py.typed
--rw-r--r--   0        0        0     2391 2023-02-04 06:38:14.964125 colt-0.9.2/colt/registrable.py
--rw-r--r--   0        0        0     1136 2023-02-04 06:38:14.964125 colt-0.9.2/colt/utils.py
--rw-r--r--   0        0        0     1880 2023-02-04 06:38:14.968125 colt-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     4021 1970-01-01 00:00:00.000000 colt-0.9.2/setup.py
--rw-r--r--   0        0        0     4043 1970-01-01 00:00:00.000000 colt-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-27 15:56:11.419594 colt-0.9.3/LICENSE
+-rw-r--r--   0        0        0     8075 2023-05-27 15:56:11.419594 colt-0.9.3/README.md
+-rw-r--r--   0        0        0     1225 2023-05-27 15:56:11.419594 colt-0.9.3/colt/__init__.py
+-rw-r--r--   0        0        0     9411 2023-05-27 15:56:11.419594 colt-0.9.3/colt/builder.py
+-rw-r--r--   0        0        0      695 2023-05-27 15:56:11.419594 colt-0.9.3/colt/default_registry.py
+-rw-r--r--   0        0        0       67 2023-05-27 15:56:11.419594 colt-0.9.3/colt/error.py
+-rw-r--r--   0        0        0      724 2023-05-27 15:56:11.419594 colt-0.9.3/colt/lazy.py
+-rw-r--r--   0        0        0        0 2023-05-27 15:56:11.419594 colt-0.9.3/colt/py.typed
+-rw-r--r--   0        0        0     2391 2023-05-27 15:56:11.419594 colt-0.9.3/colt/registrable.py
+-rw-r--r--   0        0        0     1136 2023-05-27 15:56:11.419594 colt-0.9.3/colt/utils.py
+-rw-r--r--   0        0        0     1868 2023-05-27 15:56:11.423594 colt-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     8788 1970-01-01 00:00:00.000000 colt-0.9.3/PKG-INFO
```

### Comparing `colt-0.9.2/LICENSE` & `colt-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `colt-0.9.2/colt/__init__.py` & `colt-0.9.3/colt/__init__.py`

 * *Files identical despite different names*

### Comparing `colt-0.9.2/colt/builder.py` & `colt-0.9.3/colt/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
                 )
 
             return tuple(
                 self._build(value_config, self._catname(param_name, i), value_cls)
                 for i, (value_config, value_cls) in enumerate(zip(config, args))
             )
 
-        if origin in (Dict, dict):
+        if origin in (Dict, dict, abc.Mapping, abc.MutableMapping):
             key_cls = args[0] if args else None
             value_cls = args[1] if args else None
             return {
                 self._build(
                     key_config, self._catname(param_name, f"[key:{i}]"), key_cls
                 ): self._build(
                     value_config, self._catname(param_name, key_config), value_cls
@@ -250,15 +250,15 @@
                 "\n\n"
                 + "\n".join(indent(msg) for msg in trial_messages)
                 + f"\n[{param_name}] Failed to construct object with type {annotation}"
             )
 
         if origin == Lazy:
             value_cls = args[0] if args else None
-            return Lazy(config, value_cls, self)
+            return Lazy(config, param_name, value_cls, self)
 
         if isinstance(config, (list, set, tuple)):
             cls = type(config)
             value_cls = args[0] if args else None
             return cls(
                 self._build(x, self._catname(param_name, i), value_cls)
                 for i, x in enumerate(config)
```

### Comparing `colt-0.9.2/colt/default_registry.py` & `colt-0.9.3/colt/default_registry.py`

 * *Files identical despite different names*

### Comparing `colt-0.9.2/colt/lazy.py` & `colt-0.9.3/colt/lazy.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 T = TypeVar("T")
 
 
 class Lazy(Generic[T]):
     def __init__(
         self,
         config: Any,
+        param_name: str = "",
         cls: Optional[Type[T]] = None,
         builder: Optional["ColtBuilder"] = None,
     ) -> None:
         from colt.builder import ColtBuilder
 
         self._cls = cls
         self._config = config or {}
+        self._param_name = param_name
         self._builder = builder or ColtBuilder()
 
     def construct(self, **kwargs: Any) -> T:
         config = {**self._config, **kwargs}
-        return self._builder(config, self._cls)
+        return self._builder._build(config, self._param_name, self._cls)
```

### Comparing `colt-0.9.2/colt/registrable.py` & `colt-0.9.3/colt/registrable.py`

 * *Files identical despite different names*

### Comparing `colt-0.9.2/colt/utils.py` & `colt-0.9.3/colt/utils.py`

 * *Files identical despite different names*

### Comparing `colt-0.9.2/pyproject.toml` & `colt-0.9.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "colt"
-version = "0.9.2"
+version = "0.9.3"
 description = "A configuration utility for Python object."
 authors = ["altescy <altescy@fastmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/altescy/colt"
 keywords=["config", "python", "object"]
 classifiers=[
@@ -19,20 +19,20 @@
 "Issues" = "https://github.com/altescy/colt/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 
 [tool.poetry.dev-dependencies]
 python-language-server = "^0.36.2"
-pytest = "^7.1.2"
-pysen = {version = "^0.10.1"}
-black = "^22.3.0"
-isort = "^5.10.1"
-flake8 = "^4.0.1"
-mypy = "^0.950"
+pytest = "^7.3.1"
+pysen = "^0.10.4"
+black = "^23.3.0"
+isort = "^5.12.0"
+flake8 = "^5.0.4"
+mypy = "^1.2.0"
 
 [tool.pysen]
 version = "0.10"
 
 [tool.pysen-cli]
 settings_dir = "."
```

