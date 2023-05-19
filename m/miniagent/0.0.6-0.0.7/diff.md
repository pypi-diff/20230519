# Comparing `tmp/miniagent-0.0.6-py3-none-any.whl.zip` & `tmp/miniagent-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 13280 bytes, number of entries: 18
+Zip file size: 17124 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-29 08:47 miniadmin/__init__.py
 -rw-rw-r--  2.0 unx     2440 b- defN 23-Apr-29 08:47 miniadmin/admin.py
--rw-rw-r--  2.0 unx     2925 b- defN 23-May-01 23:47 miniagent/__init__.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-May-01 23:47 miniagent/adapter.py
--rw-rw-r--  2.0 unx     3296 b- defN 23-May-01 23:47 miniagent/app_config.py
--rw-rw-r--  2.0 unx     1405 b- defN 23-May-01 23:47 miniagent/command_reciever.py
--rw-rw-r--  2.0 unx      863 b- defN 23-May-01 23:47 miniagent/common.py
--rw-rw-r--  2.0 unx      791 b- defN 23-May-01 23:47 miniagent/event_reciever.py
--rw-rw-r--  2.0 unx     3389 b- defN 23-May-01 23:47 miniagent/executer.py
--rw-rw-r--  2.0 unx      528 b- defN 23-May-01 23:47 miniagent/job_reciever.py
--rw-rw-r--  2.0 unx     2452 b- defN 23-May-01 23:47 miniagent/message_reciever.py
--rw-rw-r--  2.0 unx      275 b- defN 23-May-01 23:47 miniagent/models.py
--rw-rw-r--  2.0 unx     1063 b- defN 23-May-01 23:49 miniagent-0.0.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4078 b- defN 23-May-01 23:49 miniagent-0.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-01 23:49 miniagent-0.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       71 b- defN 23-May-01 23:49 miniagent-0.0.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       20 b- defN 23-May-01 23:49 miniagent-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1442 b- defN 23-May-01 23:49 miniagent-0.0.6.dist-info/RECORD
-18 files, 27088 bytes uncompressed, 10924 bytes compressed:  59.7%
+-rw-rw-r--  2.0 unx     3177 b- defN 23-May-19 08:01 miniagent/__init__.py
+-rw-rw-r--  2.0 unx     1760 b- defN 23-May-19 08:01 miniagent/adapter.py
+-rw-rw-r--  2.0 unx     3296 b- defN 23-May-19 08:01 miniagent/app_config.py
+-rw-rw-r--  2.0 unx     2018 b- defN 23-May-19 08:01 miniagent/command_reciever.py
+-rw-rw-r--  2.0 unx     1718 b- defN 23-May-19 08:01 miniagent/common.py
+-rw-rw-r--  2.0 unx      752 b- defN 23-May-19 08:01 miniagent/event_reciever.py
+-rw-rw-r--  2.0 unx     3310 b- defN 23-May-19 08:01 miniagent/executer.py
+-rw-rw-r--  2.0 unx    11633 b- defN 23-May-19 08:01 miniagent/flask_zipkin.py
+-rw-rw-r--  2.0 unx     1076 b- defN 23-May-19 08:01 miniagent/job_reciever.py
+-rw-rw-r--  2.0 unx     3449 b- defN 23-May-19 08:01 miniagent/message_reciever.py
+-rw-rw-r--  2.0 unx      275 b- defN 23-May-19 08:01 miniagent/models.py
+-rw-rw-r--  2.0 unx     1063 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4395 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       71 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       20 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1527 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/RECORD
+19 files, 42072 bytes uncompressed, 14642 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -21,35 +21,38 @@
 
 Filename: miniagent/event_reciever.py
 Comment: 
 
 Filename: miniagent/executer.py
 Comment: 
 
+Filename: miniagent/flask_zipkin.py
+Comment: 
+
 Filename: miniagent/job_reciever.py
 Comment: 
 
 Filename: miniagent/message_reciever.py
 Comment: 
 
 Filename: miniagent/models.py
 Comment: 
 
-Filename: miniagent-0.0.6.dist-info/LICENSE
+Filename: miniagent-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: miniagent-0.0.6.dist-info/METADATA
+Filename: miniagent-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: miniagent-0.0.6.dist-info/WHEEL
+Filename: miniagent-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: miniagent-0.0.6.dist-info/entry_points.txt
+Filename: miniagent-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: miniagent-0.0.6.dist-info/top_level.txt
+Filename: miniagent-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: miniagent-0.0.6.dist-info/RECORD
+Filename: miniagent-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## miniagent/__init__.py

```diff
@@ -7,22 +7,22 @@
 from flask import Flask
 from flask_cors import CORS
 from flask_restful import Api
 from flask_apscheduler import APScheduler
 from flask_sqlalchemy import SQLAlchemy
 import logging
 import logging.handlers
-from datetime import datetime
 from .app_config import AppConfig
 from .executer import ExecuterCaller
 from .command_reciever import CommandsReciever
 from .event_reciever import Command
 from .message_reciever import MessageReciever
+from .flask_zipkin import Zipkin
 
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 
 #Load configuration
 configure = AppConfig(os.getcwd())
 configure.from_pyfile('config.py')
 
 #Set logging
 """
@@ -37,19 +37,27 @@
 formatter = logging.Formatter("%(asctime)s %(levelname)s %(name)s %(threadName)s : %(message)s",
                               "%Y-%m-%d %H:%M:%S")
 fileHandler.setFormatter(formatter)
 logging.basicConfig(handlers=[fileHandler])
 """
 
 #Get flask handle
-app = Flask(__name__)
+app_name = configure['AGENT_NAME'] \
+    if configure.get('AGENT_NAME') else __name__
+app = Flask(app_name)
 
 #enable CORS for all routes 
 CORS(app)
 
+# zipkin
+zipkin = None
+if configure.get('ZIPKIN_ADDRESS'):
+    zipkin = Zipkin(app, sample_rate=100)
+    app.config['ZIPKIN_ADDRESS']=configure['ZIPKIN_ADDRESS']
+
 #REST API
 api = Api(app, prefix="/api/v1")
 api.add_resource(Command, '/command')
 
 #local database
 if not configure.get('SQLALCHEMY_DATABASE_URI'):
     base_dir = os.path.abspath(os.path.dirname(__file__))
```

## miniagent/adapter.py

```diff
@@ -1,28 +1,23 @@
 import abc
 from importlib import import_module
 from datetime import datetime
-from .common import split_class_path
+from .common import split_class_path, get_class_object
 
 class AdapterFactory:
 
     @staticmethod
     def create_adapter(class_path: str):
 
-        package_name, class_name = split_class_path(class_path)
+        class_obj = get_class_object(class_path)
 
-        try:    
-            package_module = import_module(package_name)
-        except ImportError:
-            return None
-
-        class_obj = getattr(package_module, class_name)
-        
         if not issubclass(class_obj, Adapter):
-            return None
+            raise RuntimeError("Class [{}] must be a subclass of"
+                               " miniagent.adapter.Adapter"\
+                            .format(class_obj.__name__))
 
         class_instance = class_obj()
 
         class_instance.set_adapter_name(class_path)
 
         return class_instance
 
@@ -40,33 +35,31 @@
         return self.adapter_name
 
     def get_adaptee_name(self):
         return self.adaptee_name
 
     def set_adaptee(self, class_path: str):
         return self._create_adaptee(class_path)
+    
+    def get_adaptee(self):
+        if self._adaptee is None:
+            raise RuntimeError("Adapter [{}] has no adaptee."\
+                               .format(self.adapter_name))
+        else:
+            return self._adaptee
 
     def _create_adaptee(self, class_path: str):
 
         if not class_path:
             self.adaptee_name = ""
+            self._adaptee = None
             return 1, "No Adaptee"
         
-        package_name, class_name = split_class_path(class_path)
+        class_obj = get_class_object(class_path)
 
-        try:
-            package_module = import_module(package_name)
-        except ImportError:
-            return -1, "'{}' is not imported.".format(package_name)
-            
-        if not hasattr(package_module, class_name):
-            return -2, "module '{}' has no attribute '{}'"\
-                            .format(package_name, class_name)
-            
-        class_obj = getattr(package_module, class_name)
         self._adaptee = class_obj()
         self.adaptee_name = class_path
 
         return 1, "OK"
 
     @abc.abstractmethod
     def get_status(self) -> int:
```

## miniagent/command_reciever.py

```diff
@@ -18,32 +18,50 @@
         return response.status_code == 200
 
     def _polling(self, url):
 
         while True:
 
             if self.event.is_set():
-                print('[CommandsReciever is broken]')
                 break
 
             try:
                 result = poll(lambda: requests.get(url), 
                                 step=10, 
                                 poll_forever=True,
                                 check_success=self._get_response)
             except requests.exceptions.ConnectionError as e:
                 sleep(10)
                 continue
 
+            
             print('result : ',type(result.text), result.text)
             result_dict = json.loads(result.text)
 
-            #self.lock.locked()
-            rtn, message = ExecuterCaller.instance().execute_command(result_dict)
-            #self.lock.release()
+            from . import app, zipkin
+            with app.app_context():
+
+                if zipkin:
+
+                    header = result.headers
+                    trace_id = header.get('x-b3-traceid')
+                    parent_span_id = header.get('x-b3-spanid')
+
+                    zipkin.create_span('CommandsReciever.url='+ url,
+                                        trace_id = trace_id,
+                                        parent_span_id = parent_span_id,
+                                      )
+                    
+                rtn, comment = ExecuterCaller.instance().execute_command(result_dict)
+
+                if zipkin:
+                    zipkin.update_tags(
+                        param  = result_dict,
+                        result = comment,
+                        )
 
     def _start_polling(self, url):
 
         self.thread = threading.Thread(target=self._polling, args=(url,))
         self.thread.name = '_polling'
         self.thread.start()
         #self.thread.join()
```

## miniagent/common.py

```diff
@@ -1,29 +1,53 @@
 import json
 import sys
 import os
+from importlib import import_module
 
 def split_class_path(class_path: str) -> tuple[str, str]:
 
     package_name = '.'.join(class_path.split('.')[:-1])
     class_name = class_path.split('.')[-1]
 
     return package_name, class_name
 
 def jsonFile2Dict(jsonFile: str) -> tuple[int, dict]:
 
-  try:
-    f = open(jsonFile)
-    data = json.load(f)
-  except FileNotFoundError as e:
-    return -1, dict(error="JsonFile is not found : {}".format(jsonFile))
-  except json.decoder.JSONDecodeError as e:
-    return -2, dict(error="JSONDecodeError occured : {}".format(sys.exc_info()[1]))
-  
-  return 1, data
+    try:
+        f = open(jsonFile)
+        data = json.load(f)
+    except FileNotFoundError as e:
+        return -1, dict(error="JsonFile is not found : {}".format(jsonFile))
+    except json.decoder.JSONDecodeError as e:
+        return -2, dict(error="JSONDecodeError occured : {}".format(sys.exc_info()[1]))
+    
+    return 1, data
+
+def get_class_object(class_path: str) -> object:
+        
+    package_name, class_name = split_class_path(class_path)
+
+    if package_name is None:
+        raise RuntimeError("There is no package name in [{}].",format(class_path))
+
+    try:
+      package_module = sys.modules[package_name]\
+                    if package_name in sys.modules else import_module(package_name)
+
+    except ImportError:
+        raise RuntimeError("Package [{}] of class [{}] isn't able to be imported."\
+                        .format(package_name, class_path))
+
+    if not hasattr(package_module, class_name):
+        raise RuntimeError("Package [{}] has no attribute [{}]."\
+                        .format(package_name, class_name))
+
+    class_obj = getattr(package_module, class_name)
+
+    return class_obj
 
 class SingletonInstane:
   __instance = None
 
   @classmethod
   def __getInstance(cls):
     return cls.__instance
```

## miniagent/event_reciever.py

```diff
@@ -11,16 +11,14 @@
     parser.add_argument('executer', type=str)
     #parser.add_argument('items', type=list, location='json')
 
     def post(self):
 
         data = Command.parser.parse_args()
 
-        print('data : ',data)
-        
         rtn, message = ExecuterCaller.instance().execute_command(data)
 
         if rtn:
             status_code = status.HTTP_200_OK            
         else:
             status_code = status.HTTP_400_BAD_REQUEST
```

## miniagent/executer.py

```diff
@@ -1,14 +1,14 @@
 import sys
 import inspect
 import types
 import abc
 from importlib import import_module
 from typing import TypeVar
-from .common import SingletonInstane, split_class_path
+from .common import SingletonInstane, get_class_object
 from .adapter import AdapterFactory
 
 class ExecuterInterface(metaclass=abc.ABCMeta):
 
     @classmethod
     def __subclasshook__(cls, subclass):
         return (hasattr(subclass, 'execute_command') and 
@@ -25,83 +25,74 @@
         raise NotImplementedError
 
 class ExecuterFactory:
 
     @staticmethod
     def create_executer(class_path: str):
 
-        package_name, class_name = split_class_path(class_path)
-
-        print('create_executer {} {}'.format(package_name, class_name))
-
-        package_module = sys.modules[package_name]\
-                  if package_name in sys.modules else import_module(package_name)
-
-        """
-        try:    
-            
-            package_module = sys.modules[package_name]\
-                  if package_name in sys.modules else import_module(package_name)
-        
-        except ImportError:
-            return None
-        """
-        class_obj = getattr(package_module, class_name)
+        class_obj = get_class_object(class_path)
 
         if not issubclass(class_obj, ExecuterInterface):
-            return None
+            raise RuntimeError("Class [{}] must be a subclass of"
+                               " miniagent.executer.ExecuterInterface"\
+                            .format(class_obj.__name__))
 
         return class_obj()
 
 class ExecuterCaller(SingletonInstane):
   
     def __init__(self, configure=None):
-        if configure:
+        if configure and configure.get('DEFAULT_ADAPTEES'):
             self.default_adaptees = configure['DEFAULT_ADAPTEES']
+        else:
+            self.default_adaptees = {}
 
     def _create_adapter(self, adapter_name: str, adaptee_name: str) -> TypeVar('T'):
 
         padapter = AdapterFactory.create_adapter(adapter_name)
         rtn, msg = padapter.set_adaptee(adaptee_name)
 
         if not rtn:
             return None
         else:    
             return padapter
 
     def execute_command(self, message: dict) -> dict:
         """
+        sample message :
         {
-            "command_code":"01",
             "initial_param":{
                 "product_code":"00011",
                 "payment_amount":50000,
             },
             "executer":"addin.executer.purchase_card.PurchaseCard",
         }
         """
-        command_code = message['command_code'] if message.get('command_code') else ''
         initial_params = message['initial_param'] if message.get('initial_param') else {}
         executer_path = message['executer']
 
         executer = ExecuterFactory.create_executer(executer_path)
 
         sig = inspect.signature(executer.execute_command)
 
         adapters = dict()
 
         for param in sig.parameters.values():
 
             if param.name not in ['db', 'initial_param']:
                 dadapter = param.annotation.__module__ +'.'+param.annotation.__name__
                 dadaptee = self.default_adaptees[dadapter] if self.default_adaptees.get(dadapter) else ""
+                
+                #if dadaptee == "":
+                #    raise RuntimeError("Adapter [{}] doesn't have default adaptee."
+                #            " Please check the constant DEFAULT_ADAPTEES in config.py".format(dadapter))
+                
                 adapter_instance = self._create_adapter(dadapter, dadaptee)
                 adapters[param.name] = adapter_instance
 
-        print('execute_command adapters :',adapters)
-
-        from . import app
+        #from . import app
 
-        with app.app_context():
-            rtn, message = executer.execute_command(initial_params, **adapters)
+        #with app.app_context():
+        #    rtn, message = executer.execute_command(initial_params, **adapters)
+        rtn, message = executer.execute_command(initial_params, **adapters)
 
         return rtn, message
```

## miniagent/job_reciever.py

```diff
@@ -10,12 +10,30 @@
         for job in jobs:
             self._run_job(job)
 
     def _run_job(self, job: dict) -> int:
 
         executer = job.pop('executer')
         scheduler.add_job(
-            func=self.caller.execute_command,
-            args=[{'executer':executer}],
+            #func=self.caller.execute_command,
+            func=self._call_execute_command,
+            args=[job['id'], {'executer':executer}],
             **job
         )        
-        return 1
+        return 1
+    
+    def _call_execute_command(self, id: str, message: dict):
+
+        from . import app, zipkin
+        with app.app_context():
+
+            if zipkin:
+                zipkin.create_span('ScheduledJob.'+ id)
+                zipkin.update_tags(param=message)
+
+            rtn, comment = self.caller.execute_command(message)
+
+            if zipkin:
+                zipkin.update_tags(
+                    param  = message,
+                    result = comment,
+                )
```

## miniagent/message_reciever.py

```diff
@@ -49,34 +49,59 @@
                 sleep(10)
                 continue
 
             if not results:
                 sleep(5)
             
             for topic_partition, messages in results.items():
-                print('kafka message : ',type(messages), messages)
                 for message in messages:
                     result_dict = self.parse_message(topic_partition.topic, message.value)
 
-                    rtn, comment = ExecuterCaller.instance().execute_command(result_dict)
+                    from . import app, zipkin
+                    with app.app_context():
+
+                        if zipkin:
+
+                            header = result_dict['header']
+                            trace_id = header.get('trace_id')
+                            parent_span_id = header.get('span_id')
+
+                            zipkin.create_span('KafkaConsumer.topic='+ topic_partition.topic,
+                                               trace_id = trace_id,
+                                               parent_span_id = parent_span_id,
+                                               )
+                            zipkin.update_tags(param=message.value)
+
+                        rtn, comment = ExecuterCaller.instance().execute_command(result_dict)
+
+                        if zipkin:
+                            zipkin.update_tags(
+                                param  = message.value,
+                                result = comment,
+                                )
 
     def _start_polling(self):
 
         self.thread = threading.Thread(target=self._polling)
         self.thread.name = '_kafka_consumer'
         self.thread.start()
-        #self.thread.join()
 
     def parse_message(self, topic: str, message: dict):
         
+        header = message.pop('header') if message.get('header') else {}
+
         result_dict =\
             dict(
                 executer = self.executers[topic],
-                initial_param = message
+                initial_param = message,
+                header = header
             )
         
         return result_dict
     
     def __del__(self):
         #if self.consumer:
         #    self.consumer.close()
-        pass
+        try:
+            self.consumer.close()
+        except Exception as e:
+            pass
```

## Comparing `miniagent-0.0.6.dist-info/LICENSE` & `miniagent-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `miniagent-0.0.6.dist-info/METADATA` & `miniagent-0.0.7.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: miniagent
-Version: 0.0.6
+Version: 0.0.7
 Summary: Multi-adaptable and lightweight server framework based on Flask
 Home-page: https://github.com/tanminkwan/local-agent
 Author: tanminkwan
 Author-email: tanminkwan@gmail.com
 License: MIT
-Keywords: flask,sqlalchemy,scheduler
+Keywords: flask,sqlalchemy,scheduler,zipkin,kafka
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aniso8601 (>=9.0.1)
 Requires-Dist: APScheduler (>=3.10.1)
@@ -39,14 +39,15 @@
 Requires-Dist: SQLAlchemy (>=2.0.11)
 Requires-Dist: typing-extensions (>=4.5.0)
 Requires-Dist: tzdata (>=2023.3)
 Requires-Dist: tzlocal (>=4.3)
 Requires-Dist: urllib3 (>=1.26.15)
 Requires-Dist: Werkzeug (>=2.3.2)
 Requires-Dist: PyGithub (>=1.58.1)
+Requires-Dist: py-zipkin (>=1.2.8)
 
 # Miniagent
 
 Miniagent is a multi-adaptable and lightweight server framework based on **Flask**.
 
 ## Installing
 
@@ -102,21 +103,35 @@
 
 There must be two files config.py and run.py in the base directory.
 ```
 # this is a sample config.py
 import os
 from datetime import datetime, timedelta
 
+AGENT_NAME = 'BLUE_SKULL_NO13'
+
+ZIPKIN_ADDRESS = ('localhost',9411)
+
 COMMANDER_SERVER_URL = 'http://localhost:8809'
 
 base_dir = os.path.abspath(os.path.dirname(__file__))
 SQLALCHEMY_DATABASE_URI = 'sqlite:///' + os.path.join(base_dir, 'app.db')
 
 CUSTOM_MODELS_PATH = "myapp.model"
 
+KAFKA_BOOTSTRAP_SERVERS = ['localhost:9092']
+
+EXECUTERS_BY_TOPIC =\
+{
+    "TEST_TOPIC":
+    "example.executer.say_hello.PrintParam",
+    "TEST2_TOPIC":
+    "example.executer.say_hello.PrintParam",
+}
+
 DEFAULT_ADAPTEES =\
 {
     "myapp.adapter.printer_adapters.PrinterAdapter":
     "myapp.adaptee.tadaptees.CardPrinterAdaptee",
     "myapp.adapter.payment_adapters.PaymentAdapter":
     "myapp.adaptee.tadaptees.CreditCardPaymentAdaptee",
 }
```

