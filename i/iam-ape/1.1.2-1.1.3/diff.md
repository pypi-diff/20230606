# Comparing `tmp/iam_ape-1.1.2.tar.gz` & `tmp/iam_ape-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_ape-1.1.2.tar", max compression
+gzip compressed data, was "iam_ape-1.1.3.tar", max compression
```

## Comparing `iam_ape-1.1.2.tar` & `iam_ape-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-27 15:26:26.770889 iam_ape-1.1.2/LICENSE
--rw-r--r--   0        0        0     3031 2023-04-27 15:26:26.771008 iam_ape-1.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771631 iam_ape-1.1.2/iam_ape/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771725 iam_ape-1.1.2/iam_ape/aws_iam_actions/__init__.py
--rw-r--r--   0        0        0   261088 2023-05-15 10:16:11.384423 iam_ape-1.1.2/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz
--rw-r--r--   0        0        0     2854 2023-05-15 10:16:11.386023 iam_ape-1.1.2/iam_ape/aws_iam_actions/scrape_iam_actions.py
--rw-r--r--   0        0        0     1748 2023-05-10 17:34:00.350992 iam_ape-1.1.2/iam_ape/consts.py
--rw-r--r--   0        0        0    32182 2023-05-15 10:16:11.386282 iam_ape-1.1.2/iam_ape/evaluator.py
--rw-r--r--   0        0        0    15833 2023-05-15 10:16:11.386516 iam_ape-1.1.2/iam_ape/expand_policy.py
--rw-r--r--   0        0        0     3422 2023-05-10 17:34:00.351308 iam_ape-1.1.2/iam_ape/helper_classes.py
--rw-r--r--   0        0        0     7858 2023-05-10 17:34:00.351446 iam_ape-1.1.2/iam_ape/helper_functions.py
--rw-r--r--   0        0        0     1224 2023-04-27 15:26:26.773011 iam_ape-1.1.2/iam_ape/helper_types.py
--rw-r--r--   0        0        0     9999 2023-05-10 17:34:00.351593 iam_ape-1.1.2/iam_ape/main.py
--rw-r--r--   0        0        0        0 2023-04-27 15:26:26.773181 iam_ape-1.1.2/iam_ape/py.typed
--rw-r--r--   0        0        0     1257 2023-05-15 10:16:11.387011 iam_ape-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 iam_ape-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 15:26:26.770889 iam_ape-1.1.3/LICENSE
+-rw-r--r--   0        0        0     3031 2023-04-27 15:26:26.771008 iam_ape-1.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771631 iam_ape-1.1.3/iam_ape/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771725 iam_ape-1.1.3/iam_ape/aws_iam_actions/__init__.py
+-rw-r--r--   0        0        0   261088 2023-05-15 10:16:11.384423 iam_ape-1.1.3/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz
+-rw-r--r--   0        0        0     2854 2023-05-15 10:16:11.386023 iam_ape-1.1.3/iam_ape/aws_iam_actions/scrape_iam_actions.py
+-rw-r--r--   0        0        0     1748 2023-05-10 17:34:00.350992 iam_ape-1.1.3/iam_ape/consts.py
+-rw-r--r--   0        0        0    31189 2023-06-06 14:28:48.009240 iam_ape-1.1.3/iam_ape/evaluator.py
+-rw-r--r--   0        0        0    15833 2023-05-15 10:16:11.386516 iam_ape-1.1.3/iam_ape/expand_policy.py
+-rw-r--r--   0        0        0     3435 2023-06-06 14:28:48.009997 iam_ape-1.1.3/iam_ape/helper_classes.py
+-rw-r--r--   0        0        0     7808 2023-06-06 14:28:48.010292 iam_ape-1.1.3/iam_ape/helper_functions.py
+-rw-r--r--   0        0        0     1224 2023-04-27 15:26:26.773011 iam_ape-1.1.3/iam_ape/helper_types.py
+-rw-r--r--   0        0        0     9999 2023-05-10 17:34:00.351593 iam_ape-1.1.3/iam_ape/main.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:26:26.773181 iam_ape-1.1.3/iam_ape/py.typed
+-rw-r--r--   0        0        0     1257 2023-06-06 14:28:48.010532 iam_ape-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 iam_ape-1.1.3/PKG-INFO
```

### Comparing `iam_ape-1.1.2/LICENSE` & `iam_ape-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.2/README.md` & `iam_ape-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.2/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz` & `iam_ape-1.1.3/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.2/iam_ape/aws_iam_actions/scrape_iam_actions.py` & `iam_ape-1.1.3/iam_ape/aws_iam_actions/scrape_iam_actions.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.2/iam_ape/consts.py` & `iam_ape-1.1.3/iam_ape/consts.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.2/iam_ape/evaluator.py` & `iam_ape-1.1.3/iam_ape/evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -554,84 +554,63 @@
             ),
             "ineffective_permissions": defaultdict(
                 lambda: defaultdict(
                     lambda: defaultdict(lambda: defaultdict(lambda: defaultdict(set)))
                 )
             ),
         }
-        # for section in ("allowed_permissions", "denied_permissions"):
-        for action_tuple_set in permissions_container.allowed_permissions.values():
-            for action_tuple in action_tuple_set:
-                service = action_to_service(action_tuple.action)
-                resource = action_tuple.resource or "*"
-                if action_tuple.not_resource:
-                    if res["allowed_permissions"][service][resource].get("NotResource"):
-                        res["allowed_permissions"][service][resource][
-                            "NotResource"
-                        ].append(action_tuple.not_resource)
-                    else:
-                        res["allowed_permissions"][service][resource]["NotResource"] = [
-                            action_tuple.not_resource
-                        ]
-                access_level = self.policy_expander.get_action_access_level(
-                    action_tuple.action
-                )
-                if cond := merge_condition(
-                    res["allowed_permissions"][service][resource][access_level]
-                    .get(action_tuple.action, {})
-                    .get("Condition", {}),
-                    action_tuple.condition,
-                    negate=False,
-                ):
-                    res["allowed_permissions"][service][resource][access_level][
-                        action_tuple.action
-                    ]["Condition"] = cond
-                res["allowed_permissions"][service][resource][access_level][
-                    action_tuple.action
-                ]["source"].add(action_tuple.source)
-
-        for action_tuple_set in permissions_container.denied_permissions.values():
-            for action_tuple in action_tuple_set:
-                service = action_to_service(action_tuple.action)
-                resource = action_tuple.resource or "*"
-                if action_tuple.not_resource:
-                    if res["denied_permissions"][service][resource].get("NotResource"):
-                        res["denied_permissions"][service][resource][
-                            "NotResource"
-                        ].append(action_tuple.not_resource)
-                    else:
-                        res["denied_permissions"][service][resource]["NotResource"] = [
-                            action_tuple.not_resource
-                        ]
-                access_level = self.policy_expander.get_action_access_level(
-                    action_tuple.action
-                )
-                if cond := merge_condition(
-                    res["denied_permissions"][service][resource][access_level]
-                    .get(action_tuple.action, {})
-                    .get("Condition", {}),
-                    action_tuple.condition,
-                    negate=False,
-                ):
-                    res["denied_permissions"][service][resource][access_level][
+        sections = ("allowed_permissions", "denied_permissions")
+        for section in sections:
+            for action_tuple_set in getattr(permissions_container, section).values():
+                for action_tuple in action_tuple_set:
+                    service = action_to_service(action_tuple.action)
+                    resource = action_tuple.resource or "*"
+                    if action_tuple.not_resource:
+                        if res[section][service][resource].get("NotResource"):  # type: ignore[literal-required]
+                            res[section][service][resource]["NotResource"].add(  # type: ignore[literal-required]
+                                action_tuple.not_resource
+                            )
+                        else:
+                            res[section][service][resource]["NotResource"] = {  # type: ignore[literal-required]
+                                action_tuple.not_resource
+                            }
+                    access_level = self.policy_expander.get_action_access_level(
                         action_tuple.action
-                    ]["Condition"] = cond
+                    )
+                    if cond := merge_condition(
+                        res[section][service][resource][access_level]  # type: ignore[literal-required]
+                        .get(action_tuple.action, {})
+                        .get("Condition", {}),
+                        action_tuple.condition,
+                        negate=False,
+                        hashable=False,
+                    ):
+                        res[section][service][resource][access_level][  # type: ignore[literal-required]
+                            action_tuple.action
+                        ][
+                            "Condition"
+                        ] = cond
+                    res[section][service][resource][access_level][action_tuple.action][  # type: ignore
+                        "source"
+                    ].add(
+                        action_tuple.source
+                    )
 
         for action_tuple in permissions_container.ineffective_permissions:
             service = action_to_service(action_tuple.action)
             resource = action_tuple.resource or "*"
             if action_tuple.not_resource:
                 if res["ineffective_permissions"][service][resource].get("NotResource"):
                     res["ineffective_permissions"][service][resource][
                         "NotResource"
-                    ].append(action_tuple.not_resource)
+                    ].add(action_tuple.not_resource)
                 else:
-                    res["ineffective_permissions"][service][resource]["NotResource"] = [
+                    res["ineffective_permissions"][service][resource]["NotResource"] = {
                         action_tuple.not_resource
-                    ]
+                    }
             access_level = self.policy_expander.get_action_access_level(
                 action_tuple.action
             )
             res["ineffective_permissions"][service][resource][access_level][
                 action_tuple.action
             ]["denied_by"].add(action_tuple.denied_by)
```

### Comparing `iam_ape-1.1.2/iam_ape/expand_policy.py` & `iam_ape-1.1.3/iam_ape/expand_policy.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.2/iam_ape/helper_classes.py` & `iam_ape-1.1.3/iam_ape/helper_classes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 from collections import namedtuple
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Set
+from typing import Any, Dict, Optional, Set
 
 from iam_ape.consts import PolicyElement
 from iam_ape.helper_types import (
     ActionDict,
     AwsPolicyType,
     IneffectiveActionDict,
     PermissionsContainerDict,
 )
 
 
-class HashableList(List[Any]):
+class HashableList(list):
     def __hash__(self) -> int:  # type: ignore[override]
-        return hash(tuple(self))
+        return hash(tuple(sorted(self)))
 
 
-class HashableDict(Dict[Any, Any]):
+class HashableDict(dict):
     def __hash__(self) -> int:  # type: ignore[override]
-        return hash(tuple(self.items()))
+        return hash(tuple(sorted(self.items())))
 
     @classmethod
     def recursively(cls, dict_obj: Optional[Dict[Any, Any]]):
         if dict_obj is None:
-            return dict_obj
+            return None
+        new_dict = {}
         for key, value in dict_obj.items():
             if isinstance(value, dict):
-                dict_obj[key] = cls.recursively(value)
+                new_dict[key] = cls.recursively(value)
             elif isinstance(value, list):
-                dict_obj[key] = HashableList(value)
+                new_dict[key] = HashableList(value)
             else:
                 assert hasattr(value, "__hash__"), f"Unhashable type: {type(value)}"
-                dict_obj[key] = value
-        return cls(dict_obj)
+                new_dict[key] = value
+        return cls(new_dict)
 
 
 @dataclass(unsafe_hash=True)
 class Action:
     action: str
     resource: Optional[str]
     not_resource: Optional[str]
```

### Comparing `iam_ape-1.1.2/iam_ape/helper_functions.py` & `iam_ape-1.1.3/iam_ape/helper_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,17 +145,17 @@
         if negated := CONDITIONS_NEGATIONS.get(condition_key):
             return {f"{negated}IfExists": condition_value}
 
     if condition_key.lower() in ("bool", "null"):
         condition_value = {
             _condition: (
                 HashableList(["true"])
-                if all(v.lower() == "false" for v in _values)
+                if all(str(v).lower() == "false" for v in _values)
                 else HashableList(["false"])
-                if all(v.lower() == "true" for v in _values)
+                if all(str(v).lower() == "true" for v in _values)
                 else HashableList(["true", "false"])
             )
             for _condition, _values in condition_value.items()
         }
 
     if condition_key == "BinaryEquals":  # there is no bloody negation
         logger.info(f"BinaryEquals used in a deny condition: {condition}")
@@ -166,33 +166,34 @@
     return {condition_key: condition_value}
 
 
 def merge_condition(
     allow_cond: Optional[Dict[str, Any]],
     deny_cond: Optional[Dict[str, Any]],
     negate: Optional[bool] = True,
+    hashable: Optional[bool] = True,
 ) -> Optional[Dict[str, Any]]:
     res = None
 
     if allow_cond and not deny_cond:
         res = allow_cond
 
     elif negate:
         if allow_cond and deny_cond:
             res = deep_update(allow_cond, negate_condition(deny_cond))
-        elif deny_cond and not allow_cond:
+        elif deny_cond:
             res = negate_condition(deny_cond)
 
     else:
         if allow_cond and deny_cond:
             res = deep_update(allow_cond, deny_cond)
         else:
             res = deny_cond
 
-    return HashableDict.recursively(res)
+    return HashableDict.recursively(res) if hashable else res
 
 
 def get_default_policy_for_managed_policy(
     managed_policy_obj: Dict[str, Any]
 ) -> AwsPolicyType:
     for policy in managed_policy_obj.get("PolicyVersionList", []):
         if policy.get("IsDefaultVersion", False):
@@ -204,22 +205,15 @@
 
 def deep_update(
     mapping: Dict[KeyType, Any], *updating_mappings: Dict[KeyType, Any]
 ) -> Dict[KeyType, Any]:
     updated_mapping = mapping.copy()
     for updating_mapping in updating_mappings:
         for k, v in updating_mapping.items():
-            if (
-                k in updated_mapping
-                and isinstance(updated_mapping[k], dict)
-                and isinstance(v, dict)
-            ):
-                updated_mapping[k] = deep_update(updated_mapping[k], v)
-            elif (
-                k in updated_mapping
-                and isinstance(updated_mapping[k], list)
-                and isinstance(v, list)
-            ):
-                updated_mapping[k].extend(v)
+            if k in updated_mapping:
+                if isinstance(updated_mapping[k], dict) and isinstance(v, dict):
+                    updated_mapping[k] = deep_update(updated_mapping[k], v)
+                elif isinstance(updated_mapping[k], list) and isinstance(v, list):
+                    updated_mapping[k] = list(set(updated_mapping[k] + v))
             else:
                 updated_mapping[k] = v
     return updated_mapping
```

### Comparing `iam_ape-1.1.2/iam_ape/helper_types.py` & `iam_ape-1.1.3/iam_ape/helper_types.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.2/iam_ape/main.py` & `iam_ape-1.1.3/iam_ape/main.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.2/pyproject.toml` & `iam_ape-1.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-ape"
-version = "1.1.2"
+version = "1.1.3"
 description = "IAM AWS Permissions Evaluator"
 authors = ["Tohar Braun, Orca Security <tohar@orca.security>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/"
 repository = "https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/"
 keywords = ["aws", "iam"]
```

### Comparing `iam_ape-1.1.2/PKG-INFO` & `iam_ape-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-ape
-Version: 1.1.2
+Version: 1.1.3
 Summary: IAM AWS Permissions Evaluator
 Home-page: https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/
 License: GPL-3.0-or-later
 Keywords: aws,iam
 Author: Tohar Braun, Orca Security
 Author-email: tohar@orca.security
 Requires-Python: >=3.8,<4.0
```

