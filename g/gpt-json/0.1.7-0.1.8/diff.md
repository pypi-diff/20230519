# Comparing `tmp/gpt_json-0.1.7.tar.gz` & `tmp/gpt_json-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_json-0.1.7.tar", max compression
+gzip compressed data, was "gpt_json-0.1.8.tar", max compression
```

## Comparing `gpt_json-0.1.7.tar` & `gpt_json-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-05-19 05:39:50.697158 gpt_json-0.1.7/LICENSE
--rw-r--r--   0        0        0     8612 2023-05-19 05:39:50.697158 gpt_json-0.1.7/README.md
--rw-r--r--   0        0        0       63 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/enums.py
--rw-r--r--   0        0        0      145 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/exceptions.py
--rw-r--r--   0        0        0    11846 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/gpt.py
--rw-r--r--   0        0        0      792 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/models.py
--rw-r--r--   0        0        0     1483 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/parsers.py
--rw-r--r--   0        0        0     1860 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/prompts.py
--rw-r--r--   0        0        0        0 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/__init__.py
--rw-r--r--   0        0        0      256 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/shared.py
--rw-r--r--   0        0        0     8767 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/test_gpt.py
--rw-r--r--   0        0        0      656 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/test_models.py
--rw-r--r--   0        0        0     1037 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/test_parsers.py
--rw-r--r--   0        0        0     1189 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/test_prompts.py
--rw-r--r--   0        0        0     3455 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/test_transformations.py
--rw-r--r--   0        0        0     2808 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/transformations.py
--rw-r--r--   0        0        0      534 2023-05-19 05:39:50.697158 gpt_json-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 gpt_json-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-19 18:17:05.455002 gpt_json-0.1.8/LICENSE
+-rw-r--r--   0        0        0     8963 2023-05-19 18:17:05.455002 gpt_json-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/enums.py
+-rw-r--r--   0        0        0      135 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/exceptions.py
+-rw-r--r--   0        0        0    11997 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/gpt.py
+-rw-r--r--   0        0        0      783 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/models.py
+-rw-r--r--   0        0        0     1535 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/parsers.py
+-rw-r--r--   0        0        0     2005 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/prompts.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/__init__.py
+-rw-r--r--   0        0        0      355 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/conftest.py
+-rw-r--r--   0        0        0      256 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/shared.py
+-rw-r--r--   0        0        0      292 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_fixtures.py
+-rw-r--r--   0        0        0     8987 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_gpt.py
+-rw-r--r--   0        0        0      830 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_models.py
+-rw-r--r--   0        0        0     1273 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_parsers.py
+-rw-r--r--   0        0        0     1208 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_prompts.py
+-rw-r--r--   0        0        0     4078 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_transformations.py
+-rw-r--r--   0        0        0     2822 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/transformations.py
+-rw-r--r--   0        0        0      628 2023-05-19 18:17:05.459003 gpt_json-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     9515 1970-01-01 00:00:00.000000 gpt_json-0.1.8/PKG-INFO
```

### Comparing `gpt_json-0.1.7/LICENSE` & `gpt_json-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.7/README.md` & `gpt_json-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -180,7 +180,17 @@
 Our focus is on making unit tests as robust as possible. The variability with GPT should be in its language model, not in its JSON behavior! This is still certainly a work in progress. If you see an edge case that isn't covered, please add it to the test suite.
 
 ## Comparison to Other Libraries
 
 A non-exhaustive list of other libraries that address the same problem. None of them were fully compatible with my deployment (hence this library), but check them out:
 
 [jsonformer](https://github.com/1rgs/jsonformer) - Works with any Huggingface model, whereas `gpt-json` is specifically tailored towards the GPT-X family. GPT doesn't output logit probabilities or allow fixed decoder templating so the same approach can't apply.
+
+## Formatting
+
+We use black and mypy for formatting. You can set up a pre-commit git hook to do this automatically via the `./lint.sh` helper file.
+
+If you perform a bulk reformatting to the codebase, you should add your most recent commit to the `.git-blame-ignore-revs` file and run:
+
+```
+git config blame.ignoreRevsFile .git-blame-ignore-revs
+```
```

### Comparing `gpt_json-0.1.7/gpt_json/gpt.py` & `gpt_json-0.1.8/gpt_json/gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,55 +7,57 @@
 import backoff
 import openai
 from openai.error import APIConnectionError, RateLimitError
 from openai.error import Timeout as OpenAITimeout
 from pydantic import BaseModel
 from tiktoken import encoding_for_model
 
-from gpt_json.models import (FixTransforms, GPTMessage, GPTModelVersion,
-                             ResponseType)
+from gpt_json.models import FixTransforms, GPTMessage, GPTModelVersion, ResponseType
 from gpt_json.parsers import find_json_response
 from gpt_json.prompts import generate_schema_prompt
 from gpt_json.transformations import fix_bools, fix_truncated_json
 
-logger = logging.getLogger('gptjson_logger')
+logger = logging.getLogger("gptjson_logger")
 handler = logging.StreamHandler()
-formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
 
 def handle_backoff(details):
     logger.warning(
         "Backing off {wait:0.1f} seconds after {tries} tries "
         "calling function {target} with args {args} and kwargs "
         "{kwargs}".format(**details)
     )
 
+
 SchemaType = TypeVar("SchemaType", bound=BaseModel)
 
 SCHEMA_PROMPT_TEMPLATE_KEY = "json_schema"
 
+
 class GPTJSON(Generic[SchemaType]):
     """
     A wrapper over GPT that provides basic JSON parsing and response handling.
 
     """
-    _cls_schema_model: Type[SchemaType] = None
-    schema_model: Type[SchemaType] = None
+
+    _cls_schema_model: Type[SchemaType] | None = None
+    schema_model: Type[SchemaType] | None = None
 
     def __init__(
         self,
         api_key: str | None = None,
         model: GPTModelVersion | str = GPTModelVersion.GPT_4,
         auto_trim: bool = False,
         auto_trim_response_overhead: int = 0,
         # For messages that are relatively deterministic
-        temperature = 0.2,
-        timeout = 60,
+        temperature=0.2,
+        timeout=60,
         openai_max_retries=3,
         **kwargs,
     ):
         """
         :param api_key: OpenAI API key, if `OPENAI_API_KEY` environment variable is not set
         :param model: GPTModelVersion or string model name
         :param auto_trim: If True, automatically trim messages to fit within the model's token limit
@@ -70,43 +72,49 @@
         self.model = model.value if isinstance(model, GPTModelVersion) else model
         self.auto_trim = auto_trim
         self.temperature = temperature
         self.timeout = timeout
         self.openai_max_retries = openai_max_retries
         self.openai_arguments = kwargs
         self.schema_model = self._cls_schema_model
-        GPTJSON._cls_schema_model = None
+        self.__class__._cls_schema_model = None
 
         if not self.schema_model:
-            raise ValueError("GPTJSON needs to be instantiated with a schema model, like GPTJSON[MySchema](...args).")
+            raise ValueError(
+                "GPTJSON needs to be instantiated with a schema model, like GPTJSON[MySchema](...args)."
+            )
 
         if get_origin(self.schema_model) in {list, List}:
             self.extract_type = ResponseType.LIST
         elif issubclass(self.schema_model, BaseModel):
             self.extract_type = ResponseType.DICTIONARY
         else:
-            raise ValueError("GPTJSON needs to be instantiated with either a pydantic.BaseModel schema or a list of those schemas.")
+            raise ValueError(
+                "GPTJSON needs to be instantiated with either a pydantic.BaseModel schema or a list of those schemas."
+            )
 
         if self.auto_trim:
             if "gpt-4" in self.model:
                 self.max_tokens = 8192 - auto_trim_response_overhead
             elif "gpt-3.5" in self.model:
                 self.max_tokens = 4096 - auto_trim_response_overhead
             else:
-                raise ValueError("Unknown model to infer max tokens, see https://platform.openai.com/docs/models/gpt-4 for more information on token length.")
+                raise ValueError(
+                    "Unknown model to infer max tokens, see https://platform.openai.com/docs/models/gpt-4 for more information on token length."
+                )
 
         self.schema_prompt = generate_schema_prompt(self.schema_model)
         self.api_key = api_key
 
     async def run(
         self,
         messages: list[GPTMessage],
         max_response_tokens: int | None = None,
         format_variables: dict[str, Any] | None = None,
-    ) -> tuple[SchemaType, FixTransforms] | tuple[None, None]:
+    ) -> tuple[SchemaType | list[SchemaType], FixTransforms] | tuple[None, None]:
         """
         :param messages: List of GPTMessage objects to send to the API
         :param max_response_tokens: Maximum number of tokens allowed in the response
         :param format_variables: Variables to format into the message template. Uses standard
             Python string formatting, like "Hello {name}".format(name="World")
 
         :return: Tuple of (parsed response, fix transforms). The transformations here is a object that
@@ -122,27 +130,34 @@
         # Most requests succeed on the first try but we wrap it locally here in case
         # there is some temporarily instability with the API. If there are longer periods
         # of instability, there should be system-wide retries in a daemon.
         backoff_request_submission = backoff.on_exception(
             backoff.expo,
             (RateLimitError, OpenAITimeout, APIConnectionError),
             max_tries=self.openai_max_retries,
-            on_backoff=handle_backoff
+            on_backoff=handle_backoff,
         )(self.submit_request)
 
-        response = await backoff_request_submission(messages, max_response_tokens=max_response_tokens)
+        response = await backoff_request_submission(
+            messages, max_response_tokens=max_response_tokens
+        )
         logger.debug("------- RAW RESPONSE ----------")
         logger.debug(response["choices"])
         logger.debug("------- END RAW RESPONSE ----------")
         extracted_json, fixed_payload = self.extract_json(response, self.extract_type)
 
         # Cast to schema model
         if extracted_json is None:
             return None, None
 
+        if not self.schema_model:
+            raise ValueError(
+                "GPTJSON failed to cast results into schema model. self.schema_model was unset."
+            )
+
         # Allow pydantic to handle the validation
         if isinstance(extracted_json, list):
             model = get_args(self.schema_model)[0]
             return [model(**item) for item in extracted_json], fixed_payload
         else:
             return self.schema_model(**extracted_json), fixed_payload
 
@@ -195,75 +210,67 @@
         optional_parameters = {}
 
         if max_response_tokens:
             optional_parameters["max_tokens"] = max_response_tokens
 
         return await openai.ChatCompletion.acreate(
             model=self.model,
-            messages=[
-                self.message_to_dict(message)
-                for message in messages
-            ],
+            messages=[self.message_to_dict(message) for message in messages],
             temperature=self.temperature,
             timeout=self.timeout,
             api_key=self.api_key,
             **optional_parameters,
             **self.openai_arguments,
         )
 
-    def fill_message_template(self, message: GPTMessage, format_variables: dict[str, Any]):
+    def fill_message_template(
+        self, message: GPTMessage, format_variables: dict[str, Any]
+    ):
         auto_format = {
             SCHEMA_PROMPT_TEMPLATE_KEY: self.schema_prompt,
         }
 
         # Regular quotes should passthrough to the next stage, except for our special keys
-        content = message.content.replace('{', '{{').replace('}', '}}')
+        content = message.content.replace("{", "{{").replace("}", "}}")
         for key in auto_format.keys():
             content = content.replace("{{" + key + "}}", "{" + key + "}")
         content = content.format(**auto_format)
 
         # We do this formatting in a separate pass so we can fill any template variables that might
         # have been left in the pydantic field typehints
         content = content.format(**format_variables)
 
         return replace(
             message,
             content=content,
         )
 
     def message_to_dict(self, message: GPTMessage):
-        return {
-            "role": message.role.value,
-            "content": message.content
-        }
+        return {"role": message.role.value, "content": message.content}
 
     def trim_messages(self, messages: list[GPTMessage], n: int):
         """
         Returns a list of messages with a total token count less than n tokens,
         cropping the last message if needed.
 
         Args:
             messages (list): List of strings to be checked.
             n (int): The maximum number of tokens allowed.
 
         Returns:
             list: A list of messages with a total token count less than n tokens.
         """
-        message_text = [
-            message.content
-            for message in messages
-        ]
+        message_text = [message.content for message in messages]
 
         enc = encoding_for_model("gpt-4")
         filtered_messages = []
         current_token_count = 0
-        original_token_count = sum([
-            len(enc.encode(message))
-            for message in message_text
-        ])
+        original_token_count = sum(
+            [len(enc.encode(message)) for message in message_text]
+        )
 
         for message in message_text:
             tokens = enc.encode(message)
             message_token_count = len(tokens)
 
             if current_token_count + message_token_count < n:
                 filtered_messages.append(message)
@@ -284,19 +291,19 @@
             )
             for i, content in enumerate(filtered_messages)
         ]
 
         # Log a copy of the message array if we have to crop it
         if current_token_count != original_token_count:
             logger.debug(
-                f"Trimmed message from {original_token_count} to {current_token_count} tokens",
-                new_messages,
+                f"Trimmed message from {original_token_count} to {current_token_count} tokens: {new_messages}",
             )
         else:
-            logger.debug(f"Skipping trim ({original_token_count}) ({current_token_count})")
+            logger.debug(
+                f"Skipping trim ({original_token_count}) ({current_token_count})"
+            )
 
         return new_messages
 
     def __class_getitem__(cls, item):
-        new_cls = super().__class_getitem__(item)
-        new_cls._cls_schema_model = item
-        return new_cls
+        cls._cls_schema_model = item
+        return cls
```

### Comparing `gpt_json-0.1.7/gpt_json/models.py` & `gpt_json-0.1.8/gpt_json/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,49 @@
+import sys
 from dataclasses import dataclass
 from enum import Enum, unique
-import sys
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
-    EnumSuper = (StrEnum,)
+
+    EnumSuper = StrEnum
 else:
-    EnumSuper = (str, Enum)
+    EnumSuper = Enum
+
 
 @unique
-class ResponseType(*EnumSuper):
+class ResponseType(EnumSuper):
     DICTIONARY = "DICTIONARY"
     LIST = "LIST"
 
 
 @unique
-class GPTMessageRole(*EnumSuper):
+class GPTMessageRole(EnumSuper):
     SYSTEM = "system"
     USER = "user"
     ASSISTANT = "assistant"
 
 
 @unique
-class GPTModelVersion(*EnumSuper):
+class GPTModelVersion(EnumSuper):
     GPT_3_5 = "gpt-3.5-turbo"
     GPT_4 = "gpt-4-0314"
 
 
 @dataclass
 class FixTransforms:
     """
     How a gpt payload was modified to be valid
     """
+
     fixed_truncation: bool = False
     fixed_bools: bool = False
 
 
 @dataclass
 class GPTMessage:
     """
     A single message in the chat sequence
     """
+
     role: GPTMessageRole
     content: str
```

### Comparing `gpt_json-0.1.7/gpt_json/parsers.py` & `gpt_json-0.1.8/gpt_json/parsers.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,29 +9,35 @@
     Takes a full response that might contain other strings and attempts to extract the JSON payload.
     Has support for truncated JSON where the JSON begins but the token window ends before the json is
     is properly closed.
 
     """
     # Deal with fully included responses as well as truncated responses that only have one
     if extract_type == ResponseType.LIST:
-        extracted_responses = list(finditer(r"(\[[^\]]*$|\[.*\])", full_response, flags=DOTALL))
+        extracted_responses = list(
+            finditer(r"(\[[^\]]*$|\[.*\])", full_response, flags=DOTALL)
+        )
     elif extract_type == ResponseType.DICTIONARY:
-        extracted_responses = list(finditer(r"({[^}]*$|{.*})", full_response, flags=DOTALL))
+        extracted_responses = list(
+            finditer(r"({[^}]*$|{.*})", full_response, flags=DOTALL)
+        )
     else:
         raise ValueError("Unknown extract_type")
 
     if not extracted_responses:
-        print(f"Unable to find any responses of the matching type `{extract_type}`: `{full_response}`")
+        print(
+            f"Unable to find any responses of the matching type `{extract_type}`: `{full_response}`"
+        )
         return None
 
     if len(extracted_responses) > 1:
         print("Unexpected response > 1, continuing anyway...", extracted_responses)
 
     extracted_response = extracted_responses[0]
 
     if is_truncated(extracted_response.group(0)):
         # Start at the same location and just expand to the end of the message
-        extracted_response = full_response[extracted_response.start():]
+        extracted_str = full_response[extracted_response.start() :]
     else:
-        extracted_response = extracted_response.group(0)
+        extracted_str = extracted_response.group(0)
 
-    return extracted_response
+    return extracted_str
```

### Comparing `gpt_json-0.1.7/gpt_json/prompts.py` & `gpt_json-0.1.8/gpt_json/prompts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 from types import UnionType
-from typing import List, get_args, get_origin
+from typing import List, Type, get_args, get_origin
 
 from pydantic import BaseModel
 
 
-def generate_schema_prompt(schema: BaseModel | list[BaseModel]) -> str:
+def generate_schema_prompt(schema: Type[BaseModel] | list[Type[BaseModel]]) -> str:
     """
     Converts the pydantic schema into a text representation that can be embedded
     into the prompt payload.
 
     """
+
     def generate_payload(model):
         payload = []
         for key, value in model.__fields__.items():
             field_annotation = model.__annotations__[key]
             annotation_origin = get_origin(field_annotation)
             annotation_arguments = get_args(field_annotation)
 
             if annotation_origin in {list, List}:
                 payload.append(f'"{key}": {annotation_arguments[0].__name__}[]')
             elif annotation_origin == UnionType:
-                payload.append(f'"{key}": {" | ".join([arg.__name__.lower() for arg in annotation_arguments])}')
+                payload.append(
+                    f'"{key}": {" | ".join([arg.__name__.lower() for arg in annotation_arguments])}'
+                )
             elif issubclass(value.type_, BaseModel):
                 payload.append(f'"{key}": {generate_payload(value.type_)}')
             else:
                 payload.append(f'"{key}": {value.type_.__name__.lower()}')
             if value.field_info.description:
-                payload[-1] += f' // {value.field_info.description}'
+                payload[-1] += f" // {value.field_info.description}"
         # All brackets are double defined so they will passthrough a call to `.format()` where we
         # pass custom variables
-        return '{{\n' + ',\n'.join(payload) + '\n}}'
+        return "{{\n" + ",\n".join(payload) + "\n}}"
 
     origin = get_origin(schema)
     args = get_args(schema)
 
     if origin == list:
         if len(args) > 1:
             raise ValueError("Only one list schema is supported at this time")
 
-        return '[' + '\n'.join(
-            [
-                generate_payload(sub_schema) + ", // Repeat for as many objects as are relevant"
-                for sub_schema in args
-            ]
-        ) + ']'
+        return (
+            "["
+            + "\n".join(
+                [
+                    generate_payload(sub_schema)
+                    + ", // Repeat for as many objects as are relevant"
+                    for sub_schema in args
+                ]
+            )
+            + "]"
+        )
     else:
         return generate_payload(schema)
```

### Comparing `gpt_json-0.1.7/gpt_json/tests/test_gpt.py` & `gpt_json-0.1.8/gpt_json/tests/test_gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-from unittest.mock import MagicMock, patch
+from unittest.mock import patch
 
 import openai
 import pytest
 from pydantic import BaseModel, Field
 
 from gpt_json.gpt import GPTJSON
-from gpt_json.models import (FixTransforms, GPTMessage, GPTMessageRole,
-                             GPTModelVersion)
+from gpt_json.models import FixTransforms, GPTMessage, GPTMessageRole, GPTModelVersion
 from gpt_json.tests.shared import MySchema, MySubSchema
 
 
 def test_throws_error_if_no_model_specified():
-    with pytest.raises(ValueError, match="needs to be instantiated with a schema model"):
+    with pytest.raises(
+        ValueError, match="needs to be instantiated with a schema model"
+    ):
         GPTJSON(None)
 
 
 @pytest.mark.parametrize(
-        "role_type,expected",
-        [
-            (GPTMessageRole.SYSTEM, "system"),
-            (GPTMessageRole.USER, "user"),
-            (GPTMessageRole.ASSISTANT, "assistant"),
-        ]
+    "role_type,expected",
+    [
+        (GPTMessageRole.SYSTEM, "system"),
+        (GPTMessageRole.USER, "user"),
+        (GPTMessageRole.ASSISTANT, "assistant"),
+    ],
 )
 def test_cast_message_to_gpt_format(role_type: GPTMessageRole, expected: str):
     parser = GPTJSON[MySchema](None)
-    assert parser.message_to_dict(
-        GPTMessage(
-            role=role_type,
-            content="test",
-        )
-    )["role"] == expected
+    assert (
+        parser.message_to_dict(
+            GPTMessage(
+                role=role_type,
+                content="test",
+            )
+        )["role"]
+        == expected
+    )
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "schema_typehint,response_raw,parsed,expected_transformations",
     [
         (
@@ -52,20 +56,18 @@
             }
             Your response is above.
             """,
             MySchema(
                 text="Test",
                 items=["Item 1", "Item 2"],
                 numerical=123,
-                sub_element=MySubSchema(
-                    name="Test"
-                ),
+                sub_element=MySubSchema(name="Test"),
                 reason=True,
             ),
-            FixTransforms()
+            FixTransforms(),
         ),
         (
             list[MySchema],
             """
             Your response is as follows:
             [
                 {
@@ -81,21 +83,19 @@
             Your response is above.
             """,
             [
                 MySchema(
                     text="Test",
                     items=["Item 1", "Item 2"],
                     numerical=123,
-                    sub_element=MySubSchema(
-                        name="Test"
-                    ),
+                    sub_element=MySubSchema(name="Test"),
                     reason=True,
-                )                
+                )
             ],
-            FixTransforms()
+            FixTransforms(),
         ),
         (
             MySchema,
             """
             Your response is as follows:
             {
                 "text": "Test",
@@ -107,24 +107,24 @@
                 "items": ["Item 1", "Item 2
 
             """,
             MySchema(
                 text="Test",
                 items=["Item 1", "Item 2"],
                 numerical=123,
-                sub_element=MySubSchema(
-                    name="Test"
-                ),
+                sub_element=MySubSchema(name="Test"),
                 reason=True,
             ),
             FixTransforms(fixed_bools=True, fixed_truncation=True),
         ),
-    ]
+    ],
 )
-async def test_acreate(schema_typehint, response_raw, parsed, expected_transformations: FixTransforms):
+async def test_acreate(
+    schema_typehint, response_raw, parsed, expected_transformations: FixTransforms
+):
     model_version = GPTModelVersion.GPT_3_5
     messages = [
         GPTMessage(
             role=GPTMessageRole.USER,
             content="Input prompt",
         )
     ]
@@ -195,90 +195,115 @@
         (
             [
                 GPTMessage(role=GPTMessageRole.SYSTEM, content="Hello"),
                 GPTMessage(role=GPTMessageRole.USER, content="World" * 10000),
             ],
             [
                 GPTMessage(role=GPTMessageRole.SYSTEM, content="Hello"),
-                GPTMessage(role=GPTMessageRole.USER, content="World" * (8192-1)),
+                GPTMessage(role=GPTMessageRole.USER, content="World" * (8192 - 1)),
             ],
         ),
     ],
 )
 def test_trim_messages(input_messages, expected_output_messages):
     gpt = GPTJSON[MySchema](None, auto_trim=True, auto_trim_response_overhead=0)
 
     output_messages = gpt.trim_messages(input_messages, n=8192)
 
     assert len(output_messages) == len(expected_output_messages)
 
-    for output_message, expected_output_message in zip(output_messages, expected_output_messages):
+    for output_message, expected_output_message in zip(
+        output_messages, expected_output_messages
+    ):
         assert output_message.role == expected_output_message.role
         assert output_message.content == expected_output_message.content
 
+
 def test_two_gptjsons():
     class TestSchema1(BaseModel):
         field1: str
+
     class TestSchema2(BaseModel):
         field2: str
-    
+
     gptjson1 = GPTJSON[TestSchema1](None)
 
-    # shouldn't allow instantion without a schema
+    # Shouldn't allow instantion without a schema
+    # We already expect a mypy error here, which is why we need a `type ignore`
+    # butr we also want to make sure that the error is raised at runtime
     with pytest.raises(ValueError):
-        gptjson2 = GPTJSON(None)
-    
+        gptjson2 = GPTJSON(None)  # type: ignore
+
     gptjson2 = GPTJSON[TestSchema2](None)
 
     assert gptjson1.schema_model == TestSchema1
     assert gptjson2.schema_model == TestSchema2
 
 
-
 def test_fill_message_template():
     class TestTemplateSchema(BaseModel):
         template_field: str = Field(description="Max length {max_length}")
 
     gpt = GPTJSON[TestTemplateSchema](None)
     assert gpt.fill_message_template(
         GPTMessage(
             role=GPTMessageRole.USER,
-            content="Variable: {max_length}\nMy schema is here: {json_schema}"
+            content="Variable: {max_length}\nMy schema is here: {json_schema}",
         ),
         dict(
             max_length=100,
-        )
+        ),
     ) == GPTMessage(
         role=GPTMessageRole.USER,
-        content="Variable: 100\nMy schema is here: {\n\"template_field\": str // Max length 100\n}"
+        content='Variable: 100\nMy schema is here: {\n"template_field": str // Max length 100\n}',
     )
 
+
 @pytest.mark.asyncio
 async def test_extracted_json_is_None():
     gpt = GPTJSON[MySchema](None)
 
-    with patch.object(gpt, 'submit_request', return_value={'choices': [{'message': {'content': 'some content'}}]}), \
-         patch.object(gpt, 'extract_json', return_value=(None, FixTransforms(False, False))):
-        result, _ = await gpt.run([GPTMessage('system', 'message content')])
+    with patch.object(
+        gpt,
+        "submit_request",
+        return_value={"choices": [{"message": {"content": "some content"}}]},
+    ), patch.object(
+        gpt, "extract_json", return_value=(None, FixTransforms(False, False))
+    ):
+        result, _ = await gpt.run(
+            [GPTMessage(GPTMessageRole.SYSTEM, "message content")]
+        )
         assert result is None
 
+
 @pytest.mark.asyncio
 async def test_no_valid_results_from_remote_request():
     gpt = GPTJSON[MySchema](None)
 
-    with patch.object(gpt, 'submit_request', return_value={'choices': []}):
-        result, _ = await gpt.run([GPTMessage('system', 'message content')])
+    with patch.object(gpt, "submit_request", return_value={"choices": []}):
+        result, _ = await gpt.run(
+            [GPTMessage(GPTMessageRole.SYSTEM, "message content")]
+        )
         assert result is None
 
+
 @pytest.mark.asyncio
 async def test_unable_to_find_valid_json_payload():
     gpt = GPTJSON[MySchema](None)
 
-    with patch.object(gpt, 'submit_request', return_value={'choices': [{'message': {'content': 'some content'}}]}), \
-         patch.object(gpt, 'extract_json', return_value=(None, FixTransforms(False, False))):
-        result, _ = await gpt.run([GPTMessage('system', 'message content')])
+    with patch.object(
+        gpt,
+        "submit_request",
+        return_value={"choices": [{"message": {"content": "some content"}}]},
+    ), patch.object(
+        gpt, "extract_json", return_value=(None, FixTransforms(False, False))
+    ):
+        result, _ = await gpt.run(
+            [GPTMessage(GPTMessageRole.SYSTEM, "message content")]
+        )
         assert result is None
 
+
 @pytest.mark.asyncio
 async def test_unknown_model_to_infer_max_tokens():
     with pytest.raises(ValueError):
         GPTJSON[MySchema](model="UnknownModel", auto_trim=True)
```

### Comparing `gpt_json-0.1.7/gpt_json/tests/test_models.py` & `gpt_json-0.1.8/gpt_json/tests/test_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-import pytest
-import gpt_json.models as models_file   
-from json import loads as json_loads, dumps as json_dumps
+import sys
 from enum import Enum
 
+import pytest
+
+import gpt_json.models as models_file
+
+
 @pytest.mark.parametrize("model_file", [models_file])
-def test_serializable_enums(model_file):
-    """
-    All our enums should be serializable as JSON
-
-    """
-    found_enums = 0
-    for obj in model_file.__dict__.values():
-        if isinstance(obj, type) and issubclass(obj, Enum):
-            found_enums += 1
-            for enum_value in obj:
-                assert enum_value.value == json_loads(json_dumps(enum_value))
+def test_string_enums(model_file):
+    if sys.version_info < (3, 11):
+        pytest.skip("Only Python 3.11+ has native support for string-based enums")
+        return
+    else:
+        from enum import StrEnum
+
+        found_enums = 0
+        for obj in model_file.__dict__.values():
+            if (
+                isinstance(obj, type)
+                and issubclass(obj, Enum)
+                and not obj in {Enum, StrEnum}
+            ):
+                found_enums += 1
+                assert issubclass(obj, StrEnum), f"{obj} is not a StrEnum"
 
-    # Every file listed in pytest should have at least one enum
-    assert found_enums > 0
+        # Every file listed in pytest should have at least one enum
+        assert found_enums > 0, f"No enums found in {model_file}"
```

### Comparing `gpt_json-0.1.7/gpt_json/tests/test_parsers.py` & `gpt_json-0.1.8/gpt_json/tests/test_parsers.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,16 +3,36 @@
 from gpt_json.models import ResponseType
 from gpt_json.parsers import find_json_response
 
 
 @pytest.mark.parametrize(
     "input_string,expected,extract_type",
     [
-        ('This message is truncated: [{"key1": [123]', '[{"key1": [123]', ResponseType.LIST),
-        ('This message is truncated: [{"key1": [123', '[{"key1": [123', ResponseType.LIST),
-        ('This message is truncated: [{"key1": "abc"', '[{"key1": "abc"', ResponseType.LIST),
-        ('This message is truncated: {"key": "value", "list": [1, 2, 3', '{"key": "value", "list": [1, 2, 3', ResponseType.DICTIONARY),
-        ('This message is truncated: {"text": "Test", "numerical": 123, "reason": true, "sub_element": { "name": "Test" }, "items": ["Item 1", "Item 2', '{"text": "Test", "numerical": 123, "reason": true, "sub_element": { "name": "Test" }, "items": ["Item 1", "Item 2', ResponseType.DICTIONARY),
-    ]
+        (
+            'This message is truncated: [{"key1": [123]',
+            '[{"key1": [123]',
+            ResponseType.LIST,
+        ),
+        (
+            'This message is truncated: [{"key1": [123',
+            '[{"key1": [123',
+            ResponseType.LIST,
+        ),
+        (
+            'This message is truncated: [{"key1": "abc"',
+            '[{"key1": "abc"',
+            ResponseType.LIST,
+        ),
+        (
+            'This message is truncated: {"key": "value", "list": [1, 2, 3',
+            '{"key": "value", "list": [1, 2, 3',
+            ResponseType.DICTIONARY,
+        ),
+        (
+            'This message is truncated: {"text": "Test", "numerical": 123, "reason": true, "sub_element": { "name": "Test" }, "items": ["Item 1", "Item 2',
+            '{"text": "Test", "numerical": 123, "reason": true, "sub_element": { "name": "Test" }, "items": ["Item 1", "Item 2',
+            ResponseType.DICTIONARY,
+        ),
+    ],
 )
 def test_find_json_response(input_string, expected, extract_type):
     assert find_json_response(input_string, extract_type) == expected
```

### Comparing `gpt_json-0.1.7/gpt_json/tests/test_prompts.py` & `gpt_json-0.1.8/gpt_json/tests/test_prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from gpt_json.prompts import generate_schema_prompt
 from gpt_json.tests.shared import MySchema
 
 
 def strip_whitespace(input_string: str):
     return sub(r"\s+", "", input_string)
 
+
 @pytest.mark.parametrize(
     "schema_definition,expected",
     [
         (
             MySchema,
             """
             {{
@@ -20,15 +21,15 @@
                 "items": str[],
                 "numerical": int | float,
                 "sub_element": {{
                     "name": str
                 }},
                 "reason": bool // Explanation
             }}
-            """
+            """,
         ),
         (
             list[MySchema],
             """
             [
             {{
             "text": str,
@@ -36,13 +37,15 @@
             "numerical": int | float,
             "sub_element": {{
                 "name": str
             }},
             "reason": bool // Explanation
             }}, // Repeat for as many objects as are relevant
             ]
-            """
-        )
-    ]
+            """,
+        ),
+    ],
 )
 def test_generate_schema_prompt(schema_definition, expected: str):
-    assert strip_whitespace(generate_schema_prompt(schema_definition)) == strip_whitespace(expected)
+    assert strip_whitespace(
+        generate_schema_prompt(schema_definition)
+    ) == strip_whitespace(expected)
```

### Comparing `gpt_json-0.1.7/gpt_json/transformations.py` & `gpt_json-0.1.8/gpt_json/transformations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 def build_stack(json_str):
     stack = []
-    fixed_str = ''
+    fixed_str = ""
     open_quotes = False
 
     for i, char in enumerate(json_str):
         if not open_quotes:
             # opening a new nested
             if char in "{[":
                 stack.append(char)
             # closing a nested
             elif char in "}]":
                 stack.pop()
         # opening or closing a string, only it's not escaped
-        if char == '"' and i > 0 and json_str[i-1] != "\\":
+        if char == '"' and i > 0 and json_str[i - 1] != "\\":
             open_quotes = not open_quotes
 
         fixed_str += char
 
     return (stack, fixed_str, open_quotes)
 
+
 def is_truncated(json_str):
     """
     Check if the json string is truncated by checking if the number of opening
     brackets is greater than the number of closing brackets.
 
     """
     stack, _, _ = build_stack(json_str)
     return len(stack) > 0
 
+
 def fix_truncated_json(json_str):
     """
     Simple json parser that attempts to fix truncated json that might
     be caused by the API response being too long.
 
     """
     stack, fixed_str, open_quotes = build_stack(json_str)
@@ -49,44 +51,44 @@
 
     # If we still have nested items remaining in our stack,
     # unwind it into the fixed string
     if stack:
         # Unwind the stack by filling it with the closing character
         # of the current nested level
         close_stack = ["]" if char == "[" else "}" for char in stack]
-        fixed_str += ''.join(close_stack[::-1])
+        fixed_str += "".join(close_stack[::-1])
 
     return fixed_str, True
 
 
 def fix_bools(json_str):
     """
     The model will relatively commonly return booleans as capitalized values because of the
     usage of caps in other languages common in the training set (like Python).
 
     """
     modified = False
     open_quotes = False
-    fixed_str = ''
+    fixed_str = ""
 
     i = 0
     while i < len(json_str):
         char = json_str[i]
 
         # Check if the current character is an opening or closing quote
-        if char == '"' and i > 0 and json_str[i-1] != "\\":
+        if char == '"' and i > 0 and json_str[i - 1] != "\\":
             open_quotes = not open_quotes
 
         # If not inside a string, check for "True" or "False" to replace
         if not open_quotes:
-            if json_str[i:i+4] == "True":
+            if json_str[i : i + 4] == "True":
                 fixed_str += "true"
                 modified = True
                 i += 3  # Skip the remaining characters of "True"
-            elif json_str[i:i+5] == "False":
+            elif json_str[i : i + 5] == "False":
                 fixed_str += "false"
                 modified = True
                 i += 4  # Skip the remaining characters of "False"
             else:
                 fixed_str += char
         else:
             fixed_str += char
```

### Comparing `gpt_json-0.1.7/pyproject.toml` & `gpt_json-0.1.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-json"
-version = "0.1.7"
+version = "0.1.8"
 description = "Structured and typehinted GPT responses in Python."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 packages = [{include = "gpt_json"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -14,11 +14,17 @@
 backoff = "^2.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 isort = "^5.12.0"
 pytest-asyncio = "^0.21.0"
+autoflake = "^2.1.1"
+black = "^23.3.0"
+mypy = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.mypy]
+check_untyped_defs = true
```

### Comparing `gpt_json-0.1.7/PKG-INFO` & `gpt_json-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-json
-Version: 0.1.7
+Version: 0.1.8
 Summary: Structured and typehinted GPT responses in Python.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -197,7 +197,17 @@
 
 ## Comparison to Other Libraries
 
 A non-exhaustive list of other libraries that address the same problem. None of them were fully compatible with my deployment (hence this library), but check them out:
 
 [jsonformer](https://github.com/1rgs/jsonformer) - Works with any Huggingface model, whereas `gpt-json` is specifically tailored towards the GPT-X family. GPT doesn't output logit probabilities or allow fixed decoder templating so the same approach can't apply.
 
+## Formatting
+
+We use black and mypy for formatting. You can set up a pre-commit git hook to do this automatically via the `./lint.sh` helper file.
+
+If you perform a bulk reformatting to the codebase, you should add your most recent commit to the `.git-blame-ignore-revs` file and run:
+
+```
+git config blame.ignoreRevsFile .git-blame-ignore-revs
+```
+
```

