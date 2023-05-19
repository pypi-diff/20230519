# Comparing `tmp/py_auth_amqp_wrapper-0.0.6.tar.gz` & `tmp/py_auth_amqp_wrapper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_amqp_wrapper-0.0.6.tar", last modified: Mon May  8 12:52:44 2023, max compression
+gzip compressed data, was "py_auth_amqp_wrapper-0.0.7.tar", last modified: Fri May 19 12:03:21 2023, max compression
```

## Comparing `py_auth_amqp_wrapper-0.0.6.tar` & `py_auth_amqp_wrapper-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:44.271793 py_auth_amqp_wrapper-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 12:52:44.271793 py_auth_amqp_wrapper-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:44.271793 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_getlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:52:44.271793 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 12:52:44.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 12:52:44.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:52:44.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 12:52:44.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 12:52:44.000000 py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 12:52:07.000000 py_auth_amqp_wrapper-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-08 12:52:44.271793 py_auth_amqp_wrapper-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:03:21.775524 py_auth_amqp_wrapper-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-19 12:03:21.775524 py_auth_amqp_wrapper-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:03:21.775524 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_getlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:03:21.775524 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-19 12:03:21.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-19 12:03:21.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:03:21.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 12:03:21.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 12:03:21.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-19 12:03:21.775524 py_auth_amqp_wrapper-0.0.7/setup.cfg
```

### Comparing `py_auth_amqp_wrapper-0.0.6/LICENSE` & `py_auth_amqp_wrapper-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.6/PKG-INFO` & `py_auth_amqp_wrapper-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_auth_amqp_wrapper
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_amqp_wrapper
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: AMQP
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/__main__.py` & `py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,52 +12,76 @@
 
 def cli() -> Optional[str]:
     parser = argparse.ArgumentParser(
         prog="py_auth_amqp_wrapper",
         description="This will start an auth server based on py_auth_micro and connect it to an AMQP message Broker",
     )
     parser.add_argument(
-        "--config", "-c", help="path to the configuration file", default="./config.json", type=str)
+        "--config",
+        "-c",
+        help="path to the configuration file",
+        default="./config.json",
+        type=str,
+    )
+    parser.add_argument(
+        "--version",
+        "-v",
+        help="displays the package version and quits",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--disable_existing_loggers",
+        "-d",
+        help="disables existing loggers",
+        action="store_true",
+    )
     parser.add_argument(
-        "--version", "-v", help="displays the package version and quits", action="store_true")
-    parser.add_argument("--disable_existing_loggers", "-d",
-                        help="disables existing loggers", action="store_true")
+        "--generate_db", "-g", help="generate database schema", action="store_true"
+    )
 
     inputvars = parser.parse_args()
 
     if inputvars.version:
         print(f"py_auth_micro=={__version__}")
         return None
 
-    return inputvars.config, inputvars.disable_existing_loggers
+    return inputvars.config, inputvars.disable_existing_loggers, inputvars.generate_db
 
 
 if __name__ == "__main__":
-    config, disable_existing_loggers = cli()
+    config, disable_existing_loggers, generate_db = cli()
 
     if config is None:
         sys.exit(0)
 
         # configure DB
-    print(f"""                             _   _     
+    print(
+        f"""                             _   _     
                             | | | |    
   _ __  _   _     __ _ _   _| |_| |__  
  | '_ \| | | |   / _` | | | | __| '_ \ 
  | |_) | |_| |  | (_| | |_| | |_| | | |
  | .__/ \__, |   \__,_|\__,_|\__|_| |_|
  | |     __/ |_____                    
  |_|    |___/______|
        py_auth_micro: {py_auth_micro.__version__}
 py_auth_amqp_wrapper: {__version__}
  
-Starting Up!""")
+Starting Up!"""
+    )
 
     print(f"loading config file: '{config}'")
     try:
         config = load_config(config)
     except Exception as exc:
         print(exc)
         print("could not load config")
         sys.exit(78)
     print("loaded config")
     print("\n\nstarting up")
-    asyncio.run(run(**config, disable_existing_loggers=disable_existing_loggers))
+    asyncio.run(
+        run(
+            **config,
+            disable_existing_loggers=disable_existing_loggers,
+            generate_schema=generate_db,
+        )
+    )
```

### Comparing `py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_getlogger.py` & `py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_getlogger.py`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_load_config.py` & `py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_load_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         "user_workflow_change_user": "user_change",
         "user_workflow_get_all": "user_all",
         "user_workflow_get_user": "user_get",
         "group_workflow_add_user_to_group": "group_add_user",
         "group_workflow_remove_user_from_group": "group_remove_user",
         "group_workflow_create_group": "group_create",
         "group_workflow_delete_group": "group_delete",
+        "group_workflow_get_groups": "group_all",
+        "group_workflow_group_users": "group_user",
     }
 
     if jwt_validation is not None:
         jwt_validator = JWTValidator()
 
         for issuer in jwt_validation:
             # translate sign methods
@@ -82,15 +84,14 @@
             secret = SECRET_METHODS[key_type](secret_value)
 
             jwt_validator.add_issuer(Issuer(issuer["name"], secret, methods))
 
         config_dict["jwt_validator"] = jwt_validator
 
     if jwt_creation is not None:
-
         # get secret for signing
         key_type = jwt_creation["secret"]["type"]
         secret_value = jwt_creation["secret"]["value"]
         key_secret = jwt_creation["secret"].get("secret", None)
 
         if not (
             key_type == "keyfile"
@@ -126,15 +127,14 @@
         config_dict["amqp_config"] = AMQPConfig(**amqp_settings)
 
     if queue_settings is not None:
         for key, value in queue_settings.items():
             default_queue_names[key] = value
 
     if log_settings is not None:
-
         LEVELMAP = {
             "NOTSET": logging.NOTSET,
             "DEBUG": logging.DEBUG,
             "INFO": logging.INFO,
             "WARNING": logging.WARNING,
             "ERROR": logging.ERROR,
             "CRITICAL": logging.CRITICAL,
@@ -152,12 +152,15 @@
         handler_settings = log_settings.get("handler_settings", {})
 
         if handler_settings.get("amqp", None) is not None:
             amqp_settings = AMQPConfig(**handler_settings["amqp"])
             handler_settings = {"amqp_config": amqp_settings}
 
         config_dict["log_config"] = {
-            "log_level": level, "handler": handler, "handler_config": handler_settings}
+            "log_level": level,
+            "handler": handler,
+            "handler_config": handler_settings,
+        }
 
     config_dict["queue_settings"] = default_queue_names
 
     return config_dict
```

### Comparing `py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper/_runner.py` & `py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,41 +17,46 @@
     jwt_encoder: JWTEncoder = None,
     jwt_validator: JWTValidator = None,
     db_config: DBConfig = DBConfig,
     app_config: AppConfig = AppConfig,
     ldap_config: LDAPConfig = None,
     amqp_config: AMQPConfig = AMQPConfig,
     log_config: logging.Logger = None,
-    disable_existing_loggers=False,
+    disable_existing_loggers: bool = False,
+    generate_schema: bool = False,
 ):
     """This Function will run the auth_service
 
     Args:
         queue_settings (dict): Settings for the QUEUE-Names to use
         jwt_encoder (JWTEncoder, optional): JWT Encoder used for creating JWTs. Defaults to None.
         jwt_validator (JWTValidator, optional): JWTValidator used to verify JWTS. Defaults to None.
         db_config (DBConfig, optional): Database Configuration. Defaults to DBConfig.
         app_config (AppConfig, optional): General App Settings. Defaults to AppConfig.
         ldap_config (LDAPConfig, optional): Configuration for LDAP Interactions. Defaults to None.
         amqp_config (AMQPConfig, optional): Configuration for the AMQP Protocoll. Defaults to AMQPConfig.
         log_config (logging.Logger, optional): If given will configure the root logger. Defaults to None.
         disable_existing_loggers (bool, optional): Disables existing loggers. Defaults to False.
+        generate_schema (bool, optional): Generate the database Schema. Defaults to False.
     """
     await Tortoise.init(
         config={
             "connections": db_config.to_dict("default"),
             "apps": {
                 "models": {
                     "models": ["py_auth_micro.Models"],
                     "default_connection": "default",
                 }
             },
         }
     )
 
+    if generate_schema:
+        await Tortoise.generate_schemas()
+
     logger = logging.getLogger("py_auth_amqp_wrapper")
     if log_config is not None:
         logger = getlogger(
             **log_config, disable_existing_loggers=disable_existing_loggers
         )
         logger.info("setup logger")
 
@@ -96,14 +101,20 @@
     )
     group_workflow_create_group = new_amqp_func(
         queue_settings["group_workflow_create_group"], groupwf.create_group
     )
     group_workflow_delete_group = new_amqp_func(
         queue_settings["group_workflow_delete_group"], groupwf.delete_group
     )
+    group_workflow_get_groups = new_amqp_func(
+        queue_settings["group_workflow_get_groups"], groupwf.get_groups
+    )
+    group_workflow_group_users = new_amqp_func(
+        queue_settings["group_workflow_group_users"], groupwf.group_members
+    )
 
     @session_workflow_logout.exception_handler(TypeError)
     @session_workflow_login.exception_handler(TypeError)
     @session_workflow_get_access_token.exception_handler(TypeError)
     async def handle_exception(*args, exc: Exception, **kwargs):
         logger.exception(exc, kwargs)
         return {"resp_code": 400, "resp_data": {"msg": "Invalid Data"}}
@@ -119,14 +130,16 @@
     @user_workflow_change_user.exception_handler(Exception)
     @user_workflow_get_all.exception_handler(Exception)
     @user_workflow_get_user.exception_handler(Exception)
     @group_workflow_add_user_to_group.exception_handler(Exception)
     @group_workflow_remove_user_from_group.exception_handler(Exception)
     @group_workflow_create_group.exception_handler(Exception)
     @group_workflow_delete_group.exception_handler(Exception)
+    @group_workflow_get_groups.exception_handler(Exception)
+    @group_workflow_group_users.exception_handler(Exception)
     @session_workflow_logout.exception_handler(Exception)
     @session_workflow_login.exception_handler(Exception)
     @session_workflow_get_access_token.exception_handler(Exception)
     async def handle_exception(*args, exc: Exception, **kwargs):
         logger.exception(exc, kwargs)
         return {"resp_code": 500, "resp_data": {"msg": f"something went wrong! {exc}"}}
```

### Comparing `py_auth_amqp_wrapper-0.0.6/py_auth_amqp_wrapper.egg-info/PKG-INFO` & `py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-auth-amqp-wrapper
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_amqp_wrapper
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: AMQP
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_amqp_wrapper-0.0.6/setup.cfg` & `py_auth_amqp_wrapper-0.0.7/setup.cfg`

 * *Files identical despite different names*

