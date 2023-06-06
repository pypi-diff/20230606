# Comparing `tmp/algokit_client_generator-0.1.0b7-py3-none-any.whl.zip` & `tmp/algokit_client_generator-0.1.0b8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 16361 bytes, number of entries: 14
+Zip file size: 17693 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       91 b- defN 80-Jan-01 00:00 algokit_client_generator/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 algokit_client_generator/__main__.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
 -rw-r--r--  2.0 unx     3199 b- defN 80-Jan-01 00:00 algokit_client_generator/document.py
--rw-r--r--  2.0 unx    26188 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
+-rw-r--r--  2.0 unx    31397 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_client_generator/py.typed
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
 -rw-r--r--  2.0 unx     4303 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
 -rw-r--r--  2.0 unx      995 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4585 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b7.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b7.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1298 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b7.dist-info/RECORD
-14 files, 51960 bytes uncompressed, 14145 bytes compressed:  72.8%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4585 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1298 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b8.dist-info/RECORD
+14 files, 57169 bytes uncompressed, 15477 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: algokit_client_generator/utils.py
 Comment: 
 
 Filename: algokit_client_generator/writer.py
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b7.dist-info/LICENSE
+Filename: algokit_client_generator-0.1.0b8.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b7.dist-info/METADATA
+Filename: algokit_client_generator-0.1.0b8.dist-info/METADATA
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b7.dist-info/WHEEL
+Filename: algokit_client_generator-0.1.0b8.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b7.dist-info/entry_points.txt
+Filename: algokit_client_generator-0.1.0b8.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b7.dist-info/RECORD
+Filename: algokit_client_generator-0.1.0b8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_client_generator/generator.py

```diff
@@ -325,80 +325,120 @@
         )
         yield Part.Gap2
     yield state_type(context, "GlobalState", global_schema)
     yield state_type(context, "LocalState", local_schema)
 
 
 def typed_client(context: GenerateContext) -> DocumentParts:
+    yield f"class {context.client_name}:"
+    yield Part.IncIndent
+    yield utils.docstring(
+        (f"{context.app_spec.contract.desc}\n\n" if context.app_spec.contract.desc else "")
+        + f"""A class for interacting with the {context.app_spec.contract.name} app providing high productivity and
+strongly typed methods to deploy and call the app"""
+    )
+    yield Part.Gap1
     yield utils.indented(
-        f"""
-class {context.client_name}:
-    @typing.overload
-    def __init__(
-        self,
-        algod_client: algosdk.v2client.algod.AlgodClient,
-        *,
-        app_id: int = 0,
-        signer: TransactionSigner | algokit_utils.Account | None = None,
-        sender: str | None = None,
-        suggested_params: algosdk.transaction.SuggestedParams | None = None,
-        template_values: algokit_utils.TemplateValueMapping | None = None,
-        app_name: str | None = None,
-    ) -> None:
-        ...
-
-    @typing.overload
-    def __init__(
-        self,
-        algod_client: algosdk.v2client.algod.AlgodClient,
-        *,
-        creator: str | algokit_utils.Account,
-        indexer_client: algosdk.v2client.indexer.IndexerClient | None = None,
-        existing_deployments: algokit_utils.AppLookup | None = None,
-        signer: TransactionSigner | algokit_utils.Account | None = None,
-        sender: str | None = None,
-        suggested_params: algosdk.transaction.SuggestedParams | None = None,
-        template_values: algokit_utils.TemplateValueMapping | None = None,
-        app_name: str | None = None,
-    ) -> None:
-        ...
-
-    def __init__(
-        self,
-        algod_client: algosdk.v2client.algod.AlgodClient,
-        *,
-        creator: str | algokit_utils.Account | None = None,
-        indexer_client: algosdk.v2client.indexer.IndexerClient | None = None,
-        existing_deployments: algokit_utils.AppLookup | None = None,
-        app_id: int = 0,
-        signer: TransactionSigner | algokit_utils.Account | None = None,
-        sender: str | None = None,
-        suggested_params: algosdk.transaction.SuggestedParams | None = None,
-        template_values: algokit_utils.TemplateValueMapping | None = None,
-        app_name: str | None = None,
-    ) -> None:
-        self.app_spec = APP_SPEC
-
-        # calling full __init__ signature, so ignoring mypy warning about overloads
-        self.app_client = algokit_utils.ApplicationClient(  # type: ignore[call-overload, misc]
-            algod_client=algod_client,
-            app_spec=self.app_spec,
-            app_id=app_id,
-            creator=creator,
-            indexer_client=indexer_client,
-            existing_deployments=existing_deployments,
-            signer=signer,
-            sender=sender,
-            suggested_params=suggested_params,
-            template_values=template_values,
-            app_name=app_name,
-        )"""
+        """
+@typing.overload
+def __init__(
+    self,
+    algod_client: algosdk.v2client.algod.AlgodClient,
+    *,
+    app_id: int = 0,
+    signer: TransactionSigner | algokit_utils.Account | None = None,
+    sender: str | None = None,
+    suggested_params: algosdk.transaction.SuggestedParams | None = None,
+    template_values: algokit_utils.TemplateValueMapping | None = None,
+    app_name: str | None = None,
+) -> None:
+    ..."""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
+@typing.overload
+def __init__(
+    self,
+    algod_client: algosdk.v2client.algod.AlgodClient,
+    *,
+    creator: str | algokit_utils.Account,
+    indexer_client: algosdk.v2client.indexer.IndexerClient | None = None,
+    existing_deployments: algokit_utils.AppLookup | None = None,
+    signer: TransactionSigner | algokit_utils.Account | None = None,
+    sender: str | None = None,
+    suggested_params: algosdk.transaction.SuggestedParams | None = None,
+    template_values: algokit_utils.TemplateValueMapping | None = None,
+    app_name: str | None = None,
+) -> None:
+    ..."""
     )
     yield Part.Gap1
+    yield utils.indented(
+        """
+def __init__(
+    self,
+    algod_client: algosdk.v2client.algod.AlgodClient,
+    *,
+    creator: str | algokit_utils.Account | None = None,
+    indexer_client: algosdk.v2client.indexer.IndexerClient | None = None,
+    existing_deployments: algokit_utils.AppLookup | None = None,
+    app_id: int = 0,
+    signer: TransactionSigner | algokit_utils.Account | None = None,
+    sender: str | None = None,
+    suggested_params: algosdk.transaction.SuggestedParams | None = None,
+    template_values: algokit_utils.TemplateValueMapping | None = None,
+    app_name: str | None = None,
+) -> None:"""
+    )
     yield Part.IncIndent
+    yield utils.docstring(
+        f"""
+{context.client_name} can be created with an app_id to interact with an existing application, alternatively
+it can be created with a creator and indexer_client specified to find existing applications by name and creator.
+
+:param AlgodClient algod_client: AlgoSDK algod client
+:param int app_id: The app_id of an existing application, to instead find the application by creator and name
+use the creator and indexer_client parameters
+:param str | Account creator: The address or Account of the app creator to resolve the app_id
+:param IndexerClient indexer_client: AlgoSDK indexer client, only required if deploying or finding app_id by
+creator and app name
+:param AppLookup existing_deployments:
+:param TransactionSigner | Account signer: Account or signer to use to sign transactions, if not specified and
+creator was passed as an Account will use that.
+:param str sender: Address to use as the sender for all transactions, will use the address associated with the
+signer if not specified.
+:param TemplateValueMapping template_values: Values to use for TMPL_* template variables, dictionary keys should
+*NOT* include the TMPL_ prefix
+:param str | None app_name: Name of application to use when deploying, defaults to name defined on the
+Application Specification
+    """
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
+self.app_spec = APP_SPEC
+
+# calling full __init__ signature, so ignoring mypy warning about overloads
+self.app_client = algokit_utils.ApplicationClient(  # type: ignore[call-overload, misc]
+    algod_client=algod_client,
+    app_spec=self.app_spec,
+    app_id=app_id,
+    creator=creator,
+    indexer_client=indexer_client,
+    existing_deployments=existing_deployments,
+    signer=signer,
+    sender=sender,
+    suggested_params=suggested_params,
+    template_values=template_values,
+    app_name=app_name,
+)"""
+    )
+    yield Part.Gap1
+    yield Part.DecIndent
     yield forwarded_client_properties(context)
     yield Part.Gap1
     if _get_declared_schema(context.app_spec, "global"):
         yield get_global_state_method(context)
         yield Part.Gap1
     if _get_declared_schema(context.app_spec, "local"):
         yield get_local_state_method(context)
@@ -421,48 +461,75 @@
 
 
 def forwarded_client_properties(context: GenerateContext) -> DocumentParts:
     yield utils.indented(
         """
 @property
 def algod_client(self) -> algosdk.v2client.algod.AlgodClient:
-    return self.app_client.algod_client
-
+    return self.app_client.algod_client"""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
 @property
 def app_id(self) -> int:
-    return self.app_client.app_id
-
+    return self.app_client.app_id"""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
 @app_id.setter
 def app_id(self, value: int) -> None:
-    self.app_client.app_id = value
-
+    self.app_client.app_id = value"""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
 @property
 def app_address(self) -> str:
-    return self.app_client.app_address
-
+    return self.app_client.app_address"""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
 @property
 def sender(self) -> str | None:
-    return self.app_client.sender
-
+    return self.app_client.sender"""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
 @sender.setter
 def sender(self, value: str) -> None:
-    self.app_client.sender = value
-
+    self.app_client.sender = value"""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
 @property
 def signer(self) -> TransactionSigner | None:
-    return self.app_client.signer
-
+    return self.app_client.signer"""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
 @signer.setter
 def signer(self, value: TransactionSigner) -> None:
-    self.app_client.signer = value
-
+    self.app_client.signer = value"""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
 @property
 def suggested_params(self) -> algosdk.transaction.SuggestedParams | None:
-    return self.app_client.suggested_params
-
+    return self.app_client.suggested_params"""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
 @suggested_params.setter
 def suggested_params(self, value: algosdk.transaction.SuggestedParams | None) -> None:
     self.app_client.suggested_params = value"""
     )
 
 
 def embed_app_spec(context: GenerateContext) -> DocumentParts:
@@ -634,33 +701,44 @@
     yield utils.indented(
         """
 def clear_state(
     self,
     transaction_parameters: algokit_utils.TransactionParameters | None = None,
     app_args: list[bytes] | None = None,
 ) -> algokit_utils.TransactionResponse:
+    \"""Calls the application with on completion set to ClearState
+
+    :param algokit_utils.TransactionParameters transaction_parameters: (optional) Additional transaction parameters
+    :param list[bytes] | None app_args: (optional) Application args to pass
+    :returns algokit_utils.TransactionResponse: The result of the transaction\"""
+
     return self.app_client.clear_state(_convert_transaction_parameters(transaction_parameters), app_args)"""
     )
 
 
-def deploy_method_args(context: GenerateContext, arg_name: str, methods: list[ContractMethod]) -> DocumentParts:
-    yield Part.InlineMode
+def deploy_method_args_type(arg_name: str, methods: list[ContractMethod]) -> str:
     has_bare = any(not m.abi for m in methods) or not methods
     typed_args = [m.abi.args_class_name for m in methods if m.abi]
     args = []
     if typed_args:
         deploy_type = "DeployCreate" if arg_name == "create_args" else "Deploy"
         args.append(f"{deploy_type}[{' | '.join(typed_args)}]")
     if has_bare:
         args.append("algokit_utils.DeployCallArgs")
         args.append("None")
 
+    return " | ".join(args)
+
+
+def deploy_method_args(context: GenerateContext, arg_name: str, methods: list[ContractMethod]) -> DocumentParts:
+    yield Part.InlineMode
+
     yield f"{arg_name}: "
-    yield utils.join(" | ", args)
-    if has_bare:
+    yield deploy_method_args_type(arg_name, methods)
+    if any(not m.abi for m in methods) or not methods:
         yield " = None"
     yield ","
     yield Part.RestoreLineMode
 
 
 def deploy_method(context: GenerateContext) -> DocumentParts:
     yield utils.indented(
@@ -680,28 +758,74 @@
     yield Part.IncIndent
     yield deploy_method_args(context, "create_args", context.methods.create)
     yield deploy_method_args(context, "update_args", context.methods.update_application)
     yield deploy_method_args(context, "delete_args", context.methods.delete_application)
     yield Part.DecIndent
     yield utils.indented(
         """
-) -> algokit_utils.DeployResponse:
-    return self.app_client.deploy(
-        version,
-        signer=signer,
-        sender=sender,
-        allow_update=allow_update,
-        allow_delete=allow_delete,
-        on_update=on_update,
-        on_schema_break=on_schema_break,
-        template_values=template_values,
-        create_args=_convert_deploy_args(create_args),
-        update_args=_convert_deploy_args(update_args),
-        delete_args=_convert_deploy_args(delete_args),
-    )"""
+) -> algokit_utils.DeployResponse:"""
+    )
+    yield Part.IncIndent
+
+    create_args_type = deploy_method_args_type("create_args", context.methods.create)
+    update_args_type = deploy_method_args_type("update_args", context.methods.update_application)
+    delete_args_type = deploy_method_args_type("delete_args", context.methods.delete_application)
+    yield utils.docstring(
+        f"""Deploy an application and update client to reference it.
+
+Idempotently deploy (create, update/delete if changed) an app against the given name via the given creator
+account, including deploy-time template placeholder substitutions.
+To understand the architecture decisions behind this functionality please see
+<https://github.com/algorandfoundation/algokit-cli/blob/main/docs/architecture-decisions/2023-01-12_smart-contract-deployment.md>
+
+```{{note}}
+If there is a breaking state schema change to an existing app (and `on_schema_break` is set to
+'ReplaceApp' the existing app will be deleted and re-created.
+```
+
+```{{note}}
+If there is an update (different TEAL code) to an existing app (and `on_update` is set to 'ReplaceApp')
+the existing app will be deleted and re-created.
+```
+
+:param str version: version to use when creating or updating app, if None version will be auto incremented
+:param algosdk.atomic_transaction_composer.TransactionSigner signer: signer to use when deploying app
+, if None uses self.signer
+:param str sender: sender address to use when deploying app, if None uses self.sender
+:param bool allow_delete: Used to set the `TMPL_DELETABLE` template variable to conditionally control if an app
+can be deleted
+:param bool allow_update: Used to set the `TMPL_UPDATABLE` template variable to conditionally control if an app
+can be updated
+:param OnUpdate on_update: Determines what action to take if an application update is required
+:param OnSchemaBreak on_schema_break: Determines what action to take if an application schema requirements
+has increased beyond the current allocation
+:param dict[str, int|str|bytes] template_values: Values to use for `TMPL_*` template variables, dictionary keys
+should *NOT* include the TMPL_ prefix
+:param {create_args_type} create_args: Arguments used when creating an application
+:param {update_args_type} update_args: Arguments used when updating an application
+:param {delete_args_type} delete_args: Arguments used when deleting an application
+:return DeployResponse: details action taken and relevant transactions
+:raises DeploymentError: If the deployment failed"""
+    )
+    yield Part.Gap1
+    yield utils.indented(
+        """
+return self.app_client.deploy(
+    version,
+    signer=signer,
+    sender=sender,
+    allow_update=allow_update,
+    allow_delete=allow_delete,
+    on_update=on_update,
+    on_schema_break=on_schema_break,
+    template_values=template_values,
+    create_args=_convert_deploy_args(create_args),
+    update_args=_convert_deploy_args(update_args),
+    delete_args=_convert_deploy_args(delete_args),
+)"""
     )
 
 
 def get_global_state_method(context: GenerateContext) -> DocumentParts:
     if not context.app_spec.schema.get("global", {}).get("declared", {}):
         return
     yield "def get_global_state(self) -> GlobalState:"
```

## Comparing `algokit_client_generator-0.1.0b7.dist-info/LICENSE` & `algokit_client_generator-0.1.0b8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_client_generator-0.1.0b7.dist-info/METADATA` & `algokit_client_generator-0.1.0b8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-client-generator
-Version: 0.1.0b7
+Version: 0.1.0b8
 Summary: Algorand typed client Generator
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_client_generator-0.1.0b7.dist-info/RECORD` & `algokit_client_generator-0.1.0b8.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 algokit_client_generator/__init__.py,sha256=ikLxrMdPVjpmrVYDdHbunvzUwiXqrCdvp8Qi5x0gC0c,91
 algokit_client_generator/__main__.py,sha256=MlkUdDAWa2XH1QDdjvayVR_WaZEGkA9voNutHzWEfFo,54
 algokit_client_generator/cli.py,sha256=XwuLZUhym9ntuHRIayPZsfv2-vTSbEykt3evF7EdVq4,2550
 algokit_client_generator/document.py,sha256=X4xMvu_LfDcaosEy3AtjRoXpiLZoXRVCIoPNo8b-h08,3199
-algokit_client_generator/generator.py,sha256=IIoCVPQmAwdq4CDoEdRQVN6Zp4QmpB3DHOFJWCKuGNI,26188
+algokit_client_generator/generator.py,sha256=YJ1ul4f0TtEOzVEH3JL5dA-veVCge-Iu13Hbk0NihQA,31397
 algokit_client_generator/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 algokit_client_generator/spec.py,sha256=apgef1qcRbm2akT1ogF23d6HnSncPwnLdrqaVzJAKmo,7466
 algokit_client_generator/utils.py,sha256=LQ3wXw_1IlnkKKNzDetIbAIBqEgYrRRjI6Bu_42Yzpc,4303
 algokit_client_generator/writer.py,sha256=CynBYWnHlO1E4Ubcpjvzq8kRcgfYCpnO3nEAslBEr-s,995
-algokit_client_generator-0.1.0b7.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
-algokit_client_generator-0.1.0b7.dist-info/METADATA,sha256=cYlTVKkvu77UHYj3EXl50bCrrXrzQkzT6-pOvPxcLNs,4585
-algokit_client_generator-0.1.0b7.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-algokit_client_generator-0.1.0b7.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
-algokit_client_generator-0.1.0b7.dist-info/RECORD,,
+algokit_client_generator-0.1.0b8.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
+algokit_client_generator-0.1.0b8.dist-info/METADATA,sha256=ymmsQJhkOT6oMNRfBnugK2NNZ_5pQn3B_nThMT-Fgoo,4585
+algokit_client_generator-0.1.0b8.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+algokit_client_generator-0.1.0b8.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
+algokit_client_generator-0.1.0b8.dist-info/RECORD,,
```

