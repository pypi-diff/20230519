# Comparing `tmp/fastapi_soap-0.0.3-py3-none-any.whl.zip` & `tmp/fastapi_soap-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9265 bytes, number of entries: 10
+Zip file size: 8719 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      302 b- defN 80-Jan-01 00:00 fastapi_soap/__init__.py
 -rw-r--r--  2.0 unx     1056 b- defN 80-Jan-01 00:00 fastapi_soap/exceptions.py
 -rw-r--r--  2.0 unx     2966 b- defN 80-Jan-01 00:00 fastapi_soap/models.py
 -rw-r--r--  2.0 unx     2219 b- defN 80-Jan-01 00:00 fastapi_soap/request.py
 -rw-r--r--  2.0 unx     2068 b- defN 80-Jan-01 00:00 fastapi_soap/response.py
--rw-r--r--  2.0 unx     6295 b- defN 80-Jan-01 00:00 fastapi_soap/routes.py
+-rw-r--r--  2.0 unx     4112 b- defN 80-Jan-01 00:00 fastapi_soap/routes.py
 -rw-r--r--  2.0 unx     5455 b- defN 80-Jan-01 00:00 fastapi_soap/wsdl.py
--rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 fastapi_soap-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_soap-0.0.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx      780 b- defN 16-Jan-01 00:00 fastapi_soap-0.0.3.dist-info/RECORD
-10 files, 23779 bytes uncompressed, 7949 bytes compressed:  66.6%
+-rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 fastapi_soap-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_soap-0.0.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx      780 b- defN 16-Jan-01 00:00 fastapi_soap-0.0.4.dist-info/RECORD
+10 files, 21596 bytes uncompressed, 7403 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -15,17 +15,17 @@
 
 Filename: fastapi_soap/routes.py
 Comment: 
 
 Filename: fastapi_soap/wsdl.py
 Comment: 
 
-Filename: fastapi_soap-0.0.3.dist-info/METADATA
+Filename: fastapi_soap-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_soap-0.0.3.dist-info/WHEEL
+Filename: fastapi_soap-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_soap-0.0.3.dist-info/RECORD
+Filename: fastapi_soap-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapi_soap/routes.py

```diff
@@ -2,18 +2,17 @@
 
 from fastapi import Request, Response
 from fastapi.routing import APIRoute, APIRouter
 from fastapi.types import DecoratedCallable
 from pydantic_xml import BaseXmlModel
 
 from fastapi_soap.exceptions import FaultException
-from fastapi_soap.models import FaultResponse, SoapBody, SoapEnvelope, SoapHeader
+from fastapi_soap.models import FaultResponse
 from fastapi_soap.response import SoapResponse
 from fastapi_soap.wsdl import dump_etree, generate_wsdl
-from fastapi.openapi.models import XML, Schema
 
 
 class SoapRoute(APIRoute):
     """FastAPI API Route extended class.
 
     This APIRoute aims to handle any exception of an Soap WebService as a
     Soap Fault response instead of manually add a new exception handler
@@ -88,68 +87,14 @@
             '/', self._generate_wsdl, methods=['GET'], status_code=200
         )
 
     def _generate_wsdl(self):
         wsdl = generate_wsdl(self._name, self._methods, url=self.prefix)
         return SoapResponse(dump_etree(wsdl), envelope_wrap=False)
 
-    def _make_openapi_specs(self, request_model, response_model):
-        schema = request_model.schema()
-        schema["xml"] = {
-            "name": request_model.__xml_tag__
-        }
-        for field in schema["properties"].values():
-            field["xml"] = {
-                "name": field["title"]
-            }
-        envelope_model = SoapEnvelope[
-            SoapHeader, SoapBody[request_model]
-        ]
-
-        def generate_default(value):
-            if value["type"] == "array":
-                return [generate_default(value["items"])]
-            return "0"
-
-        example = {
-            key: generate_default(value)
-            for key, value
-            in request_model.schema().get("properties", {}).items()
-        }
-
-        return {
-            'requestBody': {
-                'content': {
-                    'text/xml': {
-                        "example": envelope_model.parse_obj({"header": {}, "body": {"call": example}}).to_xml(pretty_print=True),
-                        "schema": envelope_model.schema(),
-                        # 'schema': {
-                        #     'title': 'Operands1',
-                        #     'required': ['operands'],
-                        #     'type': 'object',
-                        #     'properties': {
-                        #         'operands': {
-                        #             'title': 'Operands',
-                        #             'xml': {'name': 'Operands', 'value': 1},
-                        #             'type': 'integer',
-                        #         }
-                        #     },
-                        #     'xml': {
-                        #         'name': 'Operands1',
-                        #         'namespace': 'ns',
-                        #         'attribute': 'att',
-                        #     },
-                        #     'description': 'ads',
-                        # }
-                    },
-                },
-                'required': True,
-            },
-        }
-
     def operation(
         self,
         *,
         name: str,
         request_model: Optional[Type[BaseXmlModel]] = None,
         response_model: Optional[Type[BaseXmlModel]] = None,
         status_code: int = 200,
@@ -179,12 +124,11 @@
             )
             self.add_api_route(
                 f'/{name}',
                 func,
                 methods=['POST'],
                 response_class=SoapResponse,
                 status_code=status_code,
-                openapi_extra=self._make_openapi_specs(request_model, response_model),
             )
             return func
 
         return decorator
```

## Comparing `fastapi_soap-0.0.3.dist-info/METADATA` & `fastapi_soap-0.0.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-soap
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: Cleiton Junior Mittmann
 Author-email: mittmannv8@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

