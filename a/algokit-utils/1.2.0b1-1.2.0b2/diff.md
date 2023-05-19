# Comparing `tmp/algokit_utils-1.2.0b1-py3-none-any.whl.zip` & `tmp/algokit_utils-1.2.0b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 33938 bytes, number of entries: 15
--rw-r--r--  2.0 unx     3697 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
+Zip file size: 34246 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
--rw-r--r--  2.0 unx    53906 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
+-rw-r--r--  2.0 unx    53723 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
--rw-r--r--  2.0 unx    32559 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
--rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
--rw-r--r--  2.0 unx     4883 b- defN 80-Jan-01 00:00 algokit_utils/models.py
+-rw-r--r--  2.0 unx    34159 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
+-rw-r--r--  2.0 unx     2000 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
+-rw-r--r--  2.0 unx     5876 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     4841 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b1.dist-info/RECORD
-15 files, 129140 bytes uncompressed, 31846 bytes compressed:  75.3%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b2.dist-info/RECORD
+15 files, 131963 bytes uncompressed, 32154 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.2.0b1.dist-info/LICENSE
+Filename: algokit_utils-1.2.0b2.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.2.0b1.dist-info/METADATA
+Filename: algokit_utils-1.2.0b2.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.2.0b1.dist-info/WHEEL
+Filename: algokit_utils-1.2.0b2.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.2.0b1.dist-info/RECORD
+Filename: algokit_utils-1.2.0b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/__init__.py

```diff
@@ -38,14 +38,18 @@
     ABICallArgsDict,
     ABICreateCallArgs,
     ABICreateCallArgsDict,
     AppDeployMetaData,
     AppLookup,
     AppMetaData,
     AppReference,
+    DeployCallArgs,
+    DeployCallArgsDict,
+    DeployCreateCallArgs,
+    DeployCreateCallArgsDict,
     DeploymentFailedError,
     DeployResponse,
     OnSchemaBreak,
     OnUpdate,
     OperationPerformed,
     TemplateValueDict,
     TemplateValueMapping,
@@ -59,16 +63,19 @@
     ABIMethod,
     ABITransactionResponse,
     Account,
     CommonCallParameters,
     CommonCallParametersDict,
     CreateCallParameters,
     CreateCallParametersDict,
+    CreateTransactionParameters,
     OnCompleteCallParameters,
     OnCompleteCallParametersDict,
+    RawTransactionParameters,
+    TransactionParameters,
     TransactionResponse,
 )
 from algokit_utils.network_clients import (
     AlgoClientConfig,
     get_algod_client,
     get_algonode_config,
     get_default_localnet_config,
@@ -102,16 +109,23 @@
     "ABICreateCallArgs",
     "ABICreateCallArgsDict",
     "ABIMethod",
     "CommonCallParameters",
     "CommonCallParametersDict",
     "CreateCallParameters",
     "CreateCallParametersDict",
+    "CreateTransactionParameters",
+    "DeployCallArgs",
+    "DeployCreateCallArgs",
+    "DeployCallArgsDict",
+    "DeployCreateCallArgsDict",
     "OnCompleteCallParameters",
     "OnCompleteCallParametersDict",
+    "RawTransactionParameters",
+    "TransactionParameters",
     "ApplicationClient",
     "DeployResponse",
     "OnUpdate",
     "OnSchemaBreak",
     "OperationPerformed",
     "TemplateValueDict",
     "TemplateValueMapping",
```

## algokit_utils/application_client.py

```diff
@@ -152,28 +152,18 @@
         :param TemplateValueMapping template_values: Values to use for TMPL_* template variables, dictionary keys should
         *NOT* include the TMPL_ prefix
         """
         self.algod_client = algod_client
         self.app_spec = (
             au_spec.ApplicationSpecification.from_json(app_spec.read_text()) if isinstance(app_spec, Path) else app_spec
         )
-        self._approval_program: Program | None
-        self._clear_program: Program | None
-
-        if template_values:
-            self._approval_program, self._clear_program = substitute_template_and_compile(
-                self.algod_client, self.app_spec, template_values
-            )
-        elif not au_deploy.has_template_vars(self.app_spec):
-            self._approval_program = Program(self.app_spec.approval_program, self.algod_client)
-            self._clear_program = Program(self.app_spec.clear_program, self.algod_client)
-        else:  # can't compile programs yet
-            self._approval_program = None
-            self._clear_program = None
+        self._approval_program: Program | None = None
+        self._clear_program: Program | None = None
 
+        self.template_values: au_deploy.TemplateValueMapping = template_values or {}
         self.approval_source_map: SourceMap | None = None
         self.existing_deployments = existing_deployments
         self._indexer_client = indexer_client
         if creator is not None:
             if not self.existing_deployments and not self._indexer_client:
                 raise Exception(
                     "If using the creator parameter either existing_deployments or indexer_client must also be provided"
@@ -239,33 +229,33 @@
         app_id: int | None = None,
         template_values: au_deploy.TemplateValueDict | None = None,
     ) -> None:
         target.app_id = self.app_id if app_id is None else app_id
         target.signer, target.sender = target.get_signer_sender(
             AccountTransactionSigner(signer.private_key) if isinstance(signer, Account) else signer, sender
         )
-        if template_values:
-            target._approval_program, target._clear_program = substitute_template_and_compile(  # noqa: SLF001
-                target.algod_client, target.app_spec, template_values
-            )
+        target.template_values = self.template_values | (template_values or {})
 
     def deploy(
         self,
         version: str | None = None,
         *,
         signer: TransactionSigner | None = None,
         sender: str | None = None,
         allow_update: bool | None = None,
         allow_delete: bool | None = None,
         on_update: au_deploy.OnUpdate = au_deploy.OnUpdate.Fail,
         on_schema_break: au_deploy.OnSchemaBreak = au_deploy.OnSchemaBreak.Fail,
         template_values: au_deploy.TemplateValueMapping | None = None,
-        create_args: au_deploy.ABICreateCallArgs | au_deploy.ABICreateCallArgsDict | None = None,
-        update_args: au_deploy.ABICallArgs | au_deploy.ABICallArgsDict | None = None,
-        delete_args: au_deploy.ABICallArgs | au_deploy.ABICallArgsDict | None = None,
+        create_args: au_deploy.ABICreateCallArgs
+        | au_deploy.ABICreateCallArgsDict
+        | au_deploy.DeployCreateCallArgs
+        | None = None,
+        update_args: au_deploy.ABICallArgs | au_deploy.ABICallArgsDict | au_deploy.DeployCallArgs | None = None,
+        delete_args: au_deploy.ABICallArgs | au_deploy.ABICallArgsDict | au_deploy.DeployCallArgs | None = None,
     ) -> au_deploy.DeployResponse:
         """Deploy an application and update client to reference it.
 
         Idempotently deploy (create, update/delete if changed) an app against the given name via the given creator
         account, including deploy-time template placeholder substitutions.
         To understand the architecture decisions behind this functionality please see
         <https://github.com/algorandfoundation/algokit-cli/blob/main/docs/architecture-decisions/2023-01-12_smart-contract-deployment.md>
@@ -313,15 +303,15 @@
         if self._creator != resolved_sender:
             raise au_deploy.DeploymentFailedError(
                 f"Attempt to deploy contract with a sender address {resolved_sender} that differs "
                 f"from the given creator address for this application client: {self._creator}"
             )
 
         # make a copy and prepare variables
-        template_values = dict(template_values or {})
+        template_values = self.template_values | dict(template_values or {})
         au_deploy.add_deploy_template_variables(template_values, allow_update=allow_update, allow_delete=allow_delete)
 
         existing_app_metadata_or_reference = self._load_app_reference()
 
         self._approval_program, self._clear_program = substitute_template_and_compile(
             self.algod_client, self.app_spec, template_values
         )
@@ -602,17 +592,16 @@
             transaction_parameters=_parameters,
             **abi_kwargs,
         )
 
         method = self._resolve_method(
             call_abi_method, abi_kwargs, _parameters.on_complete or transaction.OnComplete.NoOpOC
         )
-        # If its a read-only method, use dryrun (TODO: swap with simulate later?)
         if method:
-            response = self._try_dry_run_call(method, atc)
+            response = self._try_simulate_call(method, atc)
             if response:
                 return response
 
         return self._execute_atc_tr(atc)
 
     def compose_opt_in(
         self,
@@ -840,31 +829,35 @@
                 version = get_next_version(app.version)
         return au_deploy.AppDeployMetaData(
             self.app_spec.contract.name, version, updatable=updatable, deletable=deletable
         )
 
     def _check_is_compiled(self) -> tuple[Program, Program]:
         if self._approval_program is None or self._clear_program is None:
-            raise Exception(
-                "Compiled programs are not available, please provide template_values before creating or updating"
+            self._approval_program, self._clear_program = substitute_template_and_compile(
+                self.algod_client, self.app_spec, self.template_values
             )
         return self._approval_program, self._clear_program
 
-    def _try_dry_run_call(self, method: Method, atc: AtomicTransactionComposer) -> ABITransactionResponse | None:
+    def _try_simulate_call(
+        self, method: Method, atc: AtomicTransactionComposer
+    ) -> ABITransactionResponse | TransactionResponse | None:
         hints = self._method_hints(method)
         if hints and hints.read_only:
-            dr_req = transaction.create_dryrun(self.algod_client, atc.gather_signatures())  # type: ignore[arg-type]
-            dr_result = self.algod_client.dryrun(dr_req)  # type: ignore[arg-type]
-            for txn in dr_result["txns"]:
-                if "app-call-messages" in txn and "REJECT" in txn["app-call-messages"]:
-                    msg = ", ".join(txn["app-call-messages"])
-                    raise Exception(f"Dryrun for readonly method failed: {msg}")
+            simulate_response = atc.simulate(self.algod_client)
+            if not simulate_response.would_succeed:
+                raise _try_convert_to_logic_error(
+                    simulate_response.failure_message,
+                    self.app_spec.approval_program,
+                    self._get_approval_source_map(),
+                ) or Exception(
+                    f"Simulate failed for readonly method {method.get_signature()}: {simulate_response.failure_message}"
+                )
 
-            method_results = _parse_result({0: method}, dr_result["txns"], atc.tx_ids)
-            return ABITransactionResponse(**method_results[0].__dict__, confirmed_round=None)
+            return TransactionResponse.from_atr(simulate_response)
         return None
 
     def _load_reference_and_check_app_id(self) -> None:
         self._load_app_reference()
         self._check_app_id()
 
     def _load_app_reference(self) -> au_deploy.AppReference | au_deploy.AppMetaData:
@@ -1095,15 +1088,15 @@
         result = self.execute_atc(atc)
         return TransactionResponse.from_atr(result)
 
     def execute_atc(self, atc: AtomicTransactionComposer) -> AtomicTransactionResponse:
         return execute_atc_with_logic_error(
             atc,
             self.algod_client,
-            approval_program=self.approval.teal if self.approval else self.app_spec.approval_program,
+            approval_program=self.app_spec.approval_program,
             approval_source_map=self._get_approval_source_map(),
         )
 
     def get_signer_sender(
         self, signer: TransactionSigner | None = None, sender: str | None = None
     ) -> tuple[TransactionSigner | None, str | None]:
         """Return signer and sender, using default values on client if not specified
@@ -1177,14 +1170,33 @@
 
         return re.sub(pattern, replacement, current_version)
     raise au_deploy.DeploymentFailedError(
         f"Could not auto increment {current_version}, please specify the next version using the version parameter"
     )
 
 
+def _try_convert_to_logic_error(
+    source_ex: Exception | str,
+    approval_program: str | None = None,
+    approval_source_map: SourceMap | None = None,
+) -> Exception | None:
+    if approval_source_map and approval_program:
+        source_ex_str = str(source_ex)
+        logic_error_data = parse_logic_error(source_ex_str)
+        if logic_error_data is not None:
+            return LogicError(
+                logic_error_str=source_ex_str,
+                logic_error=source_ex if isinstance(source_ex, Exception) else None,
+                program=approval_program,
+                source_map=approval_source_map,
+                **logic_error_data,
+            )
+    return None
+
+
 def execute_atc_with_logic_error(
     atc: AtomicTransactionComposer,
     algod_client: "AlgodClient",
     wait_rounds: int = 4,
     approval_program: str | None = None,
     approval_source_map: SourceMap | None = None,
 ) -> AtomicTransactionResponse:
@@ -1195,23 +1207,17 @@
     `approval_program` and `approval_source_map` are required to be able to parse any errors into a
     {py:class}`LogicError`
     ```
     """
     try:
         return atc.execute(algod_client, wait_rounds=wait_rounds)
     except Exception as ex:
-        if approval_source_map and approval_program:
-            logic_error_data = parse_logic_error(str(ex))
-            if logic_error_data is not None:
-                raise LogicError(
-                    logic_error=ex,
-                    program=approval_program,
-                    source_map=approval_source_map,
-                    **logic_error_data,
-                ) from ex
+        logic_error = _try_convert_to_logic_error(ex, approval_program, approval_source_map)
+        if logic_error:
+            raise logic_error from ex
         raise ex
 
 
 def _convert_call_parameters(args: CommonCallParameters | CommonCallParametersDict | None) -> CreateCallParameters:
     _args = args.__dict__ if isinstance(args, CommonCallParameters) else (args or {})
     return CreateCallParameters(**_args)
```

## algokit_utils/deploy.py

```diff
@@ -1,11 +1,12 @@
 import base64
 import dataclasses
 import json
 import logging
+import re
 from collections.abc import Iterable, Mapping, Sequence
 from enum import Enum
 from typing import TYPE_CHECKING, TypeAlias, TypedDict
 
 from algosdk import transaction
 from algosdk.atomic_transaction_composer import AtomicTransactionComposer, TransactionSigner
 from algosdk.logic import get_application_address
@@ -41,14 +42,18 @@
     "ABICallArgsDict",
     "ABICreateCallArgsDict",
     "DeploymentFailedError",
     "AppReference",
     "AppDeployMetaData",
     "AppMetaData",
     "AppLookup",
+    "DeployCallArgs",
+    "DeployCreateCallArgs",
+    "DeployCallArgsDict",
+    "DeployCreateCallArgsDict",
     "Deployer",
     "DeployResponse",
     "OnUpdate",
     "OnSchemaBreak",
     "OperationPerformed",
     "TemplateValueDict",
     "TemplateValueMapping",
@@ -62,14 +67,15 @@
 DEFAULT_INDEXER_MAX_API_RESOURCES_PER_ACCOUNT = 1000
 _UPDATABLE = "UPDATABLE"
 _DELETABLE = "DELETABLE"
 UPDATABLE_TEMPLATE_NAME = f"TMPL_{_UPDATABLE}"
 """Template variable name used to control if a smart contract is updatable or not at deployment"""
 DELETABLE_TEMPLATE_NAME = f"TMPL_{_DELETABLE}"
 """Template variable name used to control if a smart contract is deletable or not at deployment"""
+_TOKEN_PATTERN = re.compile(r"TMPL_[A-Z]+")
 TemplateValue: TypeAlias = int | str | bytes
 TemplateValueDict: TypeAlias = dict[str, TemplateValue]
 """Dictionary of `dict[str, int | str | bytes]` representing template variable names and values"""
 TemplateValueMapping: TypeAlias = Mapping[str, TemplateValue]
 """Mapping of `str` to `int | str | bytes` representing template variable names and values"""
 
 NOTE_PREFIX = "ALGOKIT_DEPLOYER:j"
@@ -378,24 +384,32 @@
     for line in program_without_comments.splitlines():
         token_idx = _find_template_token(line, token)
         if token_idx is not None:
             return True
     return False
 
 
+def _find_tokens(stripped_approval_program: str) -> list[str]:
+    return _TOKEN_PATTERN.findall(stripped_approval_program)
+
+
 def check_template_variables(approval_program: str, template_values: TemplateValueDict) -> None:
     approval_program = strip_comments(approval_program)
     if _has_token(approval_program, UPDATABLE_TEMPLATE_NAME) and _UPDATABLE not in template_values:
         raise DeploymentFailedError(
             "allow_update must be specified if deploy time configuration of update is being used"
         )
     if _has_token(approval_program, DELETABLE_TEMPLATE_NAME) and _DELETABLE not in template_values:
         raise DeploymentFailedError(
             "allow_delete must be specified if deploy time configuration of delete is being used"
         )
+    all_tokens = _find_tokens(approval_program)
+    missing_values = [token for token in all_tokens if token[len("TMPL_") :] not in template_values]
+    if missing_values:
+        raise DeploymentFailedError(f"The following template values were not provided: {', '.join(missing_values)}")
 
     for template_variable_name in template_values:
         tmpl_variable = f"TMPL_{template_variable_name}"
         if not _has_token(approval_program, tmpl_variable):
             if template_variable_name == _UPDATABLE:
                 raise DeploymentFailedError(
                     "allow_update must only be specified if deploy time configuration of update is being used"
@@ -508,72 +522,100 @@
     create_response: TransactionResponse | None = None
     delete_response: TransactionResponse | None = None
     update_response: TransactionResponse | None = None
     action_taken: OperationPerformed = OperationPerformed.Nothing
 
 
 @dataclasses.dataclass(kw_only=True)
-class ABICallArgs:
+class DeployCallArgs:
     """Parameters used to update or delete an application when calling
     {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
 
-    method: ABIMethod | bool | None = None
-    args: ABIArgsDict = dataclasses.field(default_factory=dict)
     suggested_params: transaction.SuggestedParams | None = None
     lease: bytes | str | None = None
     accounts: list[str] | None = None
     foreign_apps: list[int] | None = None
     foreign_assets: list[int] | None = None
     boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
     rekey_to: str | None = None
 
 
 @dataclasses.dataclass(kw_only=True)
-class ABICreateCallArgs(ABICallArgs):
+class ABICall:
+    method: ABIMethod | bool | None = None
+    args: ABIArgsDict = dataclasses.field(default_factory=dict)
+
+
+@dataclasses.dataclass(kw_only=True)
+class DeployCreateCallArgs(DeployCallArgs):
     """Parameters used to create an application when calling {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
 
     extra_pages: int | None = None
     on_complete: transaction.OnComplete | None = None
 
 
-class ABICallArgsDict(TypedDict, total=False):
+@dataclasses.dataclass(kw_only=True)
+class ABICallArgs(DeployCallArgs, ABICall):
+    """ABI Parameters used to update or delete an application when calling
+    {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
+
+
+@dataclasses.dataclass(kw_only=True)
+class ABICreateCallArgs(DeployCreateCallArgs, ABICall):
+    """ABI Parameters used to create an application when calling {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
+
+
+class DeployCallArgsDict(TypedDict, total=False):
     """Parameters used to update or delete an application when calling
     {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
 
-    method: ABIMethod | bool
-    args: ABIArgsDict
     suggested_params: transaction.SuggestedParams
     lease: bytes | str
     accounts: list[str]
     foreign_apps: list[int]
     foreign_assets: list[int]
     boxes: Sequence[tuple[int, bytes | bytearray | str | int]]
     rekey_to: str
 
 
-class ABICreateCallArgsDict(TypedDict, ABICallArgsDict, total=False):
+class ABICallArgsDict(DeployCallArgsDict, TypedDict, total=False):
+    """ABI Parameters used to update or delete an application when calling
+    {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
+
+    method: ABIMethod | bool
+    args: ABIArgsDict
+
+
+class DeployCreateCallArgsDict(DeployCallArgsDict, TypedDict, total=False):
     """Parameters used to create an application when calling {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
 
     extra_pages: int | None
     on_complete: transaction.OnComplete
 
 
+class ABICreateCallArgsDict(DeployCreateCallArgsDict, TypedDict, total=False):
+    """ABI Parameters used to create an application when calling {py:meth}`~algokit_utils.ApplicationClient.deploy`"""
+
+    method: ABIMethod | bool
+    args: ABIArgsDict
+
+
 @dataclasses.dataclass(kw_only=True)
 class Deployer:
     app_client: "ApplicationClient"
     creator: str
     signer: TransactionSigner
     sender: str
     existing_app_metadata_or_reference: AppReference | AppMetaData
     new_app_metadata: AppDeployMetaData
     on_update: OnUpdate
     on_schema_break: OnSchemaBreak
-    create_args: ABICreateCallArgs | ABICreateCallArgsDict | None
-    update_args: ABICallArgs | ABICallArgsDict | None
-    delete_args: ABICallArgs | ABICallArgsDict | None
+    create_args: ABICreateCallArgs | ABICreateCallArgsDict | DeployCreateCallArgs | None
+    update_args: ABICallArgs | ABICallArgsDict | DeployCallArgs | None
+    delete_args: ABICallArgs | ABICallArgsDict | DeployCallArgs | None
 
     def deploy(self) -> DeployResponse:
         """Ensures app associated with app client's creator is present and up to date"""
         assert self.app_client.approval
         assert self.app_client.clear
 
         if self.existing_app_metadata_or_reference.app_id == 0:
@@ -790,20 +832,20 @@
         deletable=app_spec_note.deletable,
         updatable=app_spec_note.updatable,
         deleted=False,
     )
 
 
 def _convert_deploy_args(
-    _args: ABICallArgs | ABICallArgsDict | None,
+    _args: DeployCallArgs | DeployCallArgsDict | None,
     note: AppDeployMetaData,
     signer: TransactionSigner | None,
     sender: str | None,
 ) -> tuple[ABIMethod | bool | None, ABIArgsDict, CreateCallParameters]:
-    args = _args.__dict__ if isinstance(_args, ABICallArgs) else (_args or {})
+    args = _args.__dict__ if isinstance(_args, DeployCallArgs) else (_args or {})
 
     # return most derived type, unused parameters are ignored
     parameters = CreateCallParameters(
         note=note.encode(),
         signer=signer,
         sender=sender,
         suggested_params=args.get("suggested_params"),
```

## algokit_utils/logic_error.py

```diff
@@ -7,15 +7,15 @@
 
 __all__ = [
     "LogicError",
     "parse_logic_error",
 ]
 
 LOGIC_ERROR = (
-    "TransactionPool.Remember: transaction (?P<transaction_id>[A-Z0-9]+): "
+    ".*transaction (?P<transaction_id>[A-Z0-9]+): "
     "logic eval error: (?P<message>.*). Details: pc=(?P<pc>[0-9]+), opcodes=.*"
 )
 
 
 class LogicErrorData(TypedDict):
     transaction_id: str
     message: str
@@ -36,23 +36,24 @@
     }
 
 
 class LogicError(Exception):
     def __init__(
         self,
         *,
-        logic_error: Exception,
+        logic_error_str: str,
         program: str,
         source_map: "AlgoSourceMap",
         transaction_id: str,
         message: str,
         pc: int,
+        logic_error: Exception | None = None,
     ):
         self.logic_error = logic_error
-        self.logic_error_str = str(logic_error)
+        self.logic_error_str = logic_error_str
         self.program = program
         self.source_map = source_map
         self.lines = program.split("\n")
         self.transaction_id = transaction_id
         self.message = message
         self.pc = pc
```

## algokit_utils/models.py

```diff
@@ -1,16 +1,23 @@
 import dataclasses
 from collections.abc import Sequence
-from typing import Any, Protocol, TypeAlias, TypedDict
+from typing import Any, Generic, Protocol, TypeAlias, TypedDict, TypeVar
 
 from algosdk import transaction
 from algosdk.abi import Method
-from algosdk.atomic_transaction_composer import AccountTransactionSigner, AtomicTransactionResponse, TransactionSigner
+from algosdk.atomic_transaction_composer import (
+    AccountTransactionSigner,
+    AtomicTransactionResponse,
+    SimulateAtomicTransactionResponse,
+    TransactionSigner,
+)
 from algosdk.encoding import decode_address
 
+ReturnType = TypeVar("ReturnType")
+
 
 @dataclasses.dataclass(kw_only=True)
 class Account:
     """Holds the private_key and address for an account"""
 
     private_key: str
     """Base64 encoded private key"""
@@ -36,46 +43,49 @@
 
     tx_id: str
     """Transaction Id"""
     confirmed_round: int | None
     """Round transaction was confirmed, `None` if call was a from a dry-run"""
 
     @staticmethod
-    def from_atr(result: AtomicTransactionResponse, transaction_index: int = -1) -> "TransactionResponse":
+    def from_atr(
+        result: AtomicTransactionResponse | SimulateAtomicTransactionResponse, transaction_index: int = -1
+    ) -> "TransactionResponse":
         """Returns either an ABITransactionResponse or a TransactionResponse based on the type of the transaction
         referred to by transaction_index
         :param AtomicTransactionResponse result: Result containing one or more transactions
         :param int transaction_index: Which transaction in the result to return, defaults to -1 (the last transaction)
         """
         tx_id = result.tx_ids[transaction_index]
         abi_result = next((r for r in result.abi_results if r.tx_id == tx_id), None)
+        confirmed_round = None if isinstance(result, SimulateAtomicTransactionResponse) else result.confirmed_round
         if abi_result:
             return ABITransactionResponse(
                 tx_id=tx_id,
                 raw_value=abi_result.raw_value,
                 return_value=abi_result.return_value,
                 decode_error=abi_result.decode_error,
                 tx_info=abi_result.tx_info,
                 method=abi_result.method,
-                confirmed_round=result.confirmed_round,
+                confirmed_round=confirmed_round,
             )
         else:
             return TransactionResponse(
                 tx_id=tx_id,
-                confirmed_round=result.confirmed_round,
+                confirmed_round=confirmed_round,
             )
 
 
 @dataclasses.dataclass(kw_only=True)
-class ABITransactionResponse(TransactionResponse):
+class ABITransactionResponse(TransactionResponse, Generic[ReturnType]):
     """Response for an ABI call"""
 
     raw_value: bytes
     """The raw response before ABI decoding"""
-    return_value: Any
+    return_value: ReturnType
     """Decoded ABI result"""
     decode_error: Exception | None
     """Details of error that occurred when attempting to decode raw_value"""
     tx_info: dict
     """Details of transaction"""
     method: Method
     """ABI method used to make call"""
@@ -90,26 +100,45 @@
         ...
 
 
 ABIMethod: TypeAlias = ABIReturnSubroutine | Method | str
 
 
 @dataclasses.dataclass(kw_only=True)
-class CommonCallParameters:
-    """Common transaction parameters used when making update, delete, opt_in, close_out or clear_state calls"""
+class TransactionParameters:
+    """Transaction parameters that can be used on ABI and non-ABI calls"""
 
     signer: TransactionSigner | None = None
     sender: str | None = None
     suggested_params: transaction.SuggestedParams | None = None
     note: bytes | str | None = None
     lease: bytes | str | None = None
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
+
+
+@dataclasses.dataclass(kw_only=True)
+class CreateTransactionParameters(TransactionParameters):
+    """Transaction parameters that can be used on ABI and non-ABI create calls"""
+
+    extra_pages: int | None = None
+
+
+@dataclasses.dataclass(kw_only=True)
+class RawTransactionParameters(TransactionParameters):
+    """Transaction parameters that can be used on non-ABI calls"""
+
     accounts: list[str] | None = None
     foreign_apps: list[int] | None = None
     foreign_assets: list[int] | None = None
-    boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
+
+
+@dataclasses.dataclass(kw_only=True)
+class CommonCallParameters(RawTransactionParameters):
+    """Transaction parameters used when making update, delete, opt_in, close_out or clear_state calls"""
+
     rekey_to: str | None = None
 
 
 @dataclasses.dataclass(kw_only=True)
 class OnCompleteCallParameters(CommonCallParameters):
     """Transaction parameters used when making any call to an Application"""
 
@@ -127,14 +156,19 @@
     """Common transaction parameters used when making update, delete, opt_in, close_out or clear_state calls"""
 
     signer: TransactionSigner
     sender: str
     suggested_params: transaction.SuggestedParams
     note: bytes | str
     lease: bytes | str
+    accounts: list[str]
+    foreign_apps: list[int]
+    foreign_assets: list[int]
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]]
+    rekey_to: str
 
 
 class OnCompleteCallParametersDict(TypedDict, CommonCallParametersDict, total=False):
     """Transaction parameters used when making any call to an Application"""
 
     on_complete: transaction.OnComplete
```

## Comparing `algokit_utils-1.2.0b1.dist-info/LICENSE` & `algokit_utils-1.2.0b2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.2.0b1.dist-info/METADATA` & `algokit_utils-1.2.0b2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.2.0b1
+Version: 1.2.0b2
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.2.0b1.dist-info/RECORD` & `algokit_utils-1.2.0b2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-algokit_utils/__init__.py,sha256=XFpWqRXQgnT9JCh6ZOlI2strJgbaZeaykfM2JZgBz9E,3697
+algokit_utils/__init__.py,sha256=wuh-p9PubCj9Bj2tpxP3tQ5qZPs_nUHzB16BHi9Aq2c,4091
 algokit_utils/_ensure_funded.py,sha256=DjwGnCC_6USLQV5wIMJZRVQFlQ1uLrGDMxRF471atsQ,4410
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
-algokit_utils/application_client.py,sha256=3oON9YJ-fU3rFhxacSPNxrpmnHUgG349oMH_Id9NdIA,53906
+algokit_utils/application_client.py,sha256=0m7Ff3y-4KVsqTs-r1EQxkdanm8_9mxwAwsXitB7H74,53723
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
-algokit_utils/deploy.py,sha256=qJDgrHpoZMZA0upQ8QnriO62b5OnRkJHBULpRdQ4khc,32559
-algokit_utils/logic_error.py,sha256=ypu2DSyus-Kjy51_1oE8T3LHVhRSOrc21Gpbau_WjAc,1981
-algokit_utils/models.py,sha256=qd2hy1ZIijD2yVs_1Zj_c8NZCk42FbEF5D6-m-eIB0g,4883
+algokit_utils/deploy.py,sha256=fcG7bZf-GIV37U1R3UdkrcqeUhvtzjOzGuPeXPVdnZA,34159
+algokit_utils/logic_error.py,sha256=IxsAGS11kuFhPhEHvhheZamQ2KQxb3LQdxiTOvnKKAA,2000
+algokit_utils/models.py,sha256=1IXNhibqtZ7cmuH31mLvNLcpJzaMl9lOD0EqsTPyglU,5876
 algokit_utils/network_clients.py,sha256=0cbUHCEWycFnduEu5cJ4dY6pfDOOzvHO1cXmcxAe83M,4841
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.2.0b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.2.0b1.dist-info/METADATA,sha256=EvMKL1LdA028HF_bbC8EtAJXqNxW8N8eIoNqQegFSCs,2037
-algokit_utils-1.2.0b1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.2.0b1.dist-info/RECORD,,
+algokit_utils-1.2.0b2.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.2.0b2.dist-info/METADATA,sha256=gSQuOhbzsDE1jrfje9zbkIrQneEjCwli7WomuO3dabI,2037
+algokit_utils-1.2.0b2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_utils-1.2.0b2.dist-info/RECORD,,
```

