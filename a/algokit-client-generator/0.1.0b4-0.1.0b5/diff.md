# Comparing `tmp/algokit_client_generator-0.1.0b4-py3-none-any.whl.zip` & `tmp/algokit_client_generator-0.1.0b5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 15158 bytes, number of entries: 14
+Zip file size: 15096 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 algokit_client_generator/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 algokit_client_generator/__main__.py
 -rw-r--r--  2.0 unx     2132 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
 -rw-r--r--  2.0 unx     3199 b- defN 80-Jan-01 00:00 algokit_client_generator/document.py
--rw-r--r--  2.0 unx    22548 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
+-rw-r--r--  2.0 unx    22974 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_client_generator/py.typed
--rw-r--r--  2.0 unx     5986 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
+-rw-r--r--  2.0 unx     5549 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
 -rw-r--r--  2.0 unx     3938 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
 -rw-r--r--  2.0 unx      890 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b4.dist-info/LICENSE
--rw-r--r--  2.0 unx     4585 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b4.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b4.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1299 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b4.dist-info/RECORD
-14 files, 46041 bytes uncompressed, 12942 bytes compressed:  71.9%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4585 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b5.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1299 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b5.dist-info/RECORD
+14 files, 46030 bytes uncompressed, 12880 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: algokit_client_generator/utils.py
 Comment: 
 
 Filename: algokit_client_generator/writer.py
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b4.dist-info/LICENSE
+Filename: algokit_client_generator-0.1.0b5.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b4.dist-info/METADATA
+Filename: algokit_client_generator-0.1.0b5.dist-info/METADATA
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b4.dist-info/WHEEL
+Filename: algokit_client_generator-0.1.0b5.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b4.dist-info/entry_points.txt
+Filename: algokit_client_generator-0.1.0b5.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b4.dist-info/RECORD
+Filename: algokit_client_generator-0.1.0b5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_client_generator/generator.py

```diff
@@ -130,43 +130,52 @@
     @staticmethod
     @abstractmethod
     def method() -> str:
         ..."""
         )
     yield Part.Gap2
     if has_abi_create or has_abi_update or has_abi_delete:
-        yield '_TArgs = typing.TypeVar("_TArgs", bound=_ArgsBase)'
+        yield '_TArgs = typing.TypeVar("_TArgs", bound=_ArgsBase[typing.Any])'
         yield Part.Gap2
-    if has_abi_create:
         yield utils.indented(
             """
 @dataclasses.dataclass(kw_only=True)
-class _TypedDeployCreateArgs(algokit_utils.DeployCreateCallArgs, typing.Generic[_TArgs]):
+class _TArgsHolder(typing.Generic[_TArgs]):
     args: _TArgs
 """
         )
         yield Part.Gap2
+
+    if has_abi_create:
+        yield utils.indented(
+            """
+@dataclasses.dataclass(kw_only=True)
+class _TypedDeployCreateArgs(algokit_utils.DeployCreateCallArgs, _TArgsHolder[_TArgs], typing.Generic[_TArgs]):
+    pass
+"""
+        )
+        yield Part.Gap2
     if has_abi_update or has_abi_delete:
         yield utils.indented(
             """
 @dataclasses.dataclass(kw_only=True)
-class _TypedDeployArgs(algokit_utils.DeployCallArgs, typing.Generic[_TArgs]):
-    args: _TArgs"""
+class _TypedDeployArgs(algokit_utils.DeployCallArgs, _TArgsHolder[_TArgs], typing.Generic[_TArgs]):
+    pass"""
         )
         yield Part.Gap2
 
     yield Part.Gap2
     yield utils.indented(
         """
 def _as_dict(data: _T | None) -> dict[str, typing.Any]:
     if data is None:
         return {}
     if not dataclasses.is_dataclass(data):
         raise TypeError(f"{data} must be a dataclass")
-    return {f.name: getattr(data, f.name) for f in dataclasses.fields(data)}
+    return {f.name: getattr(data, f.name) for f in dataclasses.fields(data) if getattr(data, f.name) is not None}
 """
     )
     yield Part.Gap2
     yield utils.indented(
         """
 def _convert_on_complete(on_complete: algokit_utils.OnCompleteActionName) -> algosdk.transaction.OnComplete:
     on_complete_enum = on_complete.replace("_", " ").title().replace(" ", "") + "OC"
@@ -288,59 +297,63 @@
         algod_client: algosdk.v2client.algod.AlgodClient,
         *,
         app_id: int = 0,
         signer: TransactionSigner | algokit_utils.Account | None = None,
         sender: str | None = None,
         suggested_params: algosdk.transaction.SuggestedParams | None = None,
         template_values: algokit_utils.TemplateValueMapping | None = None,
-    ):
+        app_name: str | None = None,
+    ) -> None:
         ...
 
     @typing.overload
     def __init__(
         self,
         algod_client: algosdk.v2client.algod.AlgodClient,
         *,
         creator: str | algokit_utils.Account,
         indexer_client: algosdk.v2client.indexer.IndexerClient | None = None,
         existing_deployments: algokit_utils.AppLookup | None = None,
         signer: TransactionSigner | algokit_utils.Account | None = None,
         sender: str | None = None,
         suggested_params: algosdk.transaction.SuggestedParams | None = None,
         template_values: algokit_utils.TemplateValueMapping | None = None,
-    ):
+        app_name: str | None = None,
+    ) -> None:
         ...
 
     def __init__(
         self,
         algod_client: algosdk.v2client.algod.AlgodClient,
         *,
         creator: str | algokit_utils.Account | None = None,
         indexer_client: algosdk.v2client.indexer.IndexerClient | None = None,
         existing_deployments: algokit_utils.AppLookup | None = None,
         app_id: int = 0,
         signer: TransactionSigner | algokit_utils.Account | None = None,
         sender: str | None = None,
         suggested_params: algosdk.transaction.SuggestedParams | None = None,
         template_values: algokit_utils.TemplateValueMapping | None = None,
-    ):
+        app_name: str | None = None,
+    ) -> None:
         self.app_spec = APP_SPEC
 
         # calling full __init__ signature, so ignoring mypy warning about overloads
         self.app_client = algokit_utils.ApplicationClient(  # type: ignore[call-overload, misc]
             algod_client=algod_client,
             app_spec=self.app_spec,
             app_id=app_id,
             creator=creator,
             indexer_client=indexer_client,
             existing_deployments=existing_deployments,
             signer=signer,
             sender=sender,
             suggested_params=suggested_params,
             template_values=template_values,
+            app_name=app_name,
         )"""
     )
     yield Part.Gap1
     yield Part.IncIndent
     yield get_global_state_method(context)
     yield Part.Gap1
     yield get_local_state_method(context)
```

## algokit_client_generator/spec.py

```diff
@@ -93,32 +93,21 @@
     return result.values()
 
 
 def use_method_name(method: Method) -> str:
     return method.name
 
 
-def use_method_name_and_return(method: Method) -> str:
-    return f"{method.name}_{method.returns}"
-
-
-def use_method_name_and_arg_count(method: Method) -> str:
-    return f"{method.name}_{len(method.args)}_args"
-
-
 def use_method_signature(method: Method) -> str:
     return method.get_signature().replace("(", "_").replace(")", "_").replace(",", "_")
 
 
 def find_naming_strategy(methods: list[Method]) -> Callable[[Method], str]:
-    for strategy in (use_method_name, use_method_name_and_return, use_method_name_and_arg_count):
-        transformed = set(map(strategy, methods))
-        if len(transformed) == len(methods):  # unique mappings found
-            return strategy
-    # fall back to full signature
+    if len(methods) == 1:
+        return use_method_name
     return use_method_signature
 
 
 def get_contract_methods(
     app_spec: ApplicationSpecification, used_module_symbols: set[str], used_client_symbols: set[str]
 ) -> ContractMethods:
     result = ContractMethods()
```

## Comparing `algokit_client_generator-0.1.0b4.dist-info/LICENSE` & `algokit_client_generator-0.1.0b5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_client_generator-0.1.0b4.dist-info/METADATA` & `algokit_client_generator-0.1.0b5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: algokit-client-generator
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: Algorand typed client Generator
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: algokit-utils (>=1.2.0b2,<2.0.0)
+Requires-Dist: algokit-utils (>=1.2.0b3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # AlgoKit Python client generator (algokit-client-generator-py)
 
 This project generates a type-safe smart contract client in Python for the Algorand Blockchain that wraps the 
 [application client](https://algorandfoundation.github.io/algokit-utils-py/html/apidocs/algokit_utils/algokit_utils.html#algokit_utils.ApplicationClient) in 
 [AlgoKit Utils](https://github.com/algorandfoundation/algokit-utils-py). It does this by reading an [ARC-0032](https://github.com/algorandfoundation/ARCs/blob/main/ARCs/arc-0032.md) application spec file.
```

## Comparing `algokit_client_generator-0.1.0b4.dist-info/RECORD` & `algokit_client_generator-0.1.0b5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 algokit_client_generator/__init__.py,sha256=KHVr3rMTN2T146gjOpaF3fc5cqoLoVs01ueXn-p9QHI,179
 algokit_client_generator/__main__.py,sha256=MlkUdDAWa2XH1QDdjvayVR_WaZEGkA9voNutHzWEfFo,54
 algokit_client_generator/cli.py,sha256=S9YxyLIpzDvSGLbxP7QJz8b-otpzX-lgHRJzvEzFC6Q,2132
 algokit_client_generator/document.py,sha256=X4xMvu_LfDcaosEy3AtjRoXpiLZoXRVCIoPNo8b-h08,3199
-algokit_client_generator/generator.py,sha256=bJc3FlvS2RnEG4FBMgVWMbneNunBlA3-SeCs4mLVSro,22548
+algokit_client_generator/generator.py,sha256=PaNn4f0PfnWr0unmrU--I_OA-ERv9GY8xcQbejCno0Y,22974
 algokit_client_generator/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_client_generator/spec.py,sha256=LcPiMhvnnscvnACk_YGzweEnzQ7V7kQyDvQ94Uo9Nlo,5986
+algokit_client_generator/spec.py,sha256=wa4sHpbDRk7UQJsUDMdJ6NP8CCKiqBazbPrQg9khzjw,5549
 algokit_client_generator/utils.py,sha256=omhCEOXmxc523oiOcM6TL0IpbR6MqdM5Sy-o3o9VQTw,3938
 algokit_client_generator/writer.py,sha256=MF46CQ8q1nW-K66RcKcXYE1uArrNRKHWF-uKQT8eziU,890
-algokit_client_generator-0.1.0b4.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
-algokit_client_generator-0.1.0b4.dist-info/METADATA,sha256=GugMRsLKRIOGpYLumIAzbmPHFRcE2TNCxpN6aQmhzac,4585
-algokit_client_generator-0.1.0b4.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_client_generator-0.1.0b4.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
-algokit_client_generator-0.1.0b4.dist-info/RECORD,,
+algokit_client_generator-0.1.0b5.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
+algokit_client_generator-0.1.0b5.dist-info/METADATA,sha256=lKUyLA1aAOkukiz0kpVPjvHA-86-6UMccWeWSUyp4AA,4585
+algokit_client_generator-0.1.0b5.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_client_generator-0.1.0b5.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
+algokit_client_generator-0.1.0b5.dist-info/RECORD,,
```

