# Comparing `tmp/mat_enm-0.0.10.tar.gz` & `tmp/mat_enm-0.0.11.tar.gz`

## Comparing `mat_enm-0.0.10.tar` & `mat_enm-0.0.11.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/ENMClient.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/__version__.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/enmscripting.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/enmsession.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/command/__init__.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/command/command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/common/__init__.py
--rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/common/element.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/common/file.py
--rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/common/output.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/private/__init__.py
--rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/private/executionhandler.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/private/logging_util.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/private/overrides.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/private/poller.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/private/retry.py
--rw-r--r--   0        0        0    11855 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/private/session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/security/__init__.py
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/security/authenticator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/terminal/__init__.py
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/terminal/terminal.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/__init__.py
--rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/element_iterator.py
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/json_generator.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/session_mock_utils.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_command.py
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_command_get_output.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_element.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_enmsession.py
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_executor.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_executor_get_url.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_open_external_session.py
--rw-r--r--   0        0        0    11091 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_open_internal_session.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_output.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_poller.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_result_groups_stress.py
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_retry.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_session.py
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_terminal.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/utils/cm_command_type.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/utils/constants.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mat_enm-0.0.10/src/mat_enm/utils/error_code.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mat_enm-0.0.10/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mat_enm-0.0.10/LICENSE
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 mat_enm-0.0.10/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 mat_enm-0.0.10/pyproject.toml
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 mat_enm-0.0.10/PKG-INFO
+-rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/ENMClient.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/__version__.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/enmscripting.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/enmsession.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/command/__init__.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/command/command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/common/__init__.py
+-rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/common/element.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/common/file.py
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/common/output.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/private/__init__.py
+-rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/private/executionhandler.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/private/logging_util.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/private/overrides.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/private/poller.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/private/retry.py
+-rw-r--r--   0        0        0    11855 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/private/session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/security/__init__.py
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/security/authenticator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/terminal/__init__.py
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/terminal/terminal.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/__init__.py
+-rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/element_iterator.py
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/json_generator.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/session_mock_utils.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_command.py
+-rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_command_get_output.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_element.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_enmsession.py
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_executor.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_executor_get_url.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_open_external_session.py
+-rw-r--r--   0        0        0    11091 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_open_internal_session.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_output.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_poller.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_result_groups_stress.py
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_retry.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_session.py
+-rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_terminal.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/utils/cm_command_type.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/utils/constants.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mat_enm-0.0.11/src/mat_enm/utils/error_code.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mat_enm-0.0.11/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mat_enm-0.0.11/LICENSE
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 mat_enm-0.0.11/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 mat_enm-0.0.11/pyproject.toml
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 mat_enm-0.0.11/PKG-INFO
```

### Comparing `mat_enm-0.0.10/src/mat_enm/ENMClient.py` & `mat_enm-0.0.11/src/mat_enm/ENMClient.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/enmscripting.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/enmscripting.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/enmsession.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/enmsession.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/exceptions.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/exceptions.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/command/command.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/command/command.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/common/element.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/common/element.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/common/file.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/common/file.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/common/output.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/common/output.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/private/executionhandler.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/private/executionhandler.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/private/logging_util.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/private/logging_util.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/private/overrides.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/private/overrides.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/private/poller.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/private/poller.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/private/retry.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/private/retry.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/private/session.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/private/session.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/security/authenticator.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/security/authenticator.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/terminal/terminal.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/element_iterator.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/element_iterator.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/json_generator.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/json_generator.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/session_mock_utils.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/session_mock_utils.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_command.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_command.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_command_get_output.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_command_get_output.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_element.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_element.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_executor.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_executor.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_executor_get_url.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_executor_get_url.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_open_external_session.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_open_external_session.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_open_internal_session.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_open_internal_session.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_output.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_output.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_poller.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_poller.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_result_groups_stress.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_result_groups_stress.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_retry.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_retry.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_session.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_session.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/enmscripting/test/test_terminal.py` & `mat_enm-0.0.11/src/mat_enm/enmscripting/test/test_terminal.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/src/mat_enm/utils/error_code.py` & `mat_enm-0.0.11/src/mat_enm/utils/error_code.py`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/LICENSE` & `mat_enm-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.10/README.md` & `mat_enm-0.0.11/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# mat-vertica
+# mat-enm
 
 [![PyPI version](https://img.shields.io/pypi/v/mat-vertica?color=brightgreen&label=PyPI%20package)](https://pypi.org/project/mat-enm/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vertica-python.svg)](https://www.python.org/downloads/)
 
 ## Lista de contenido
 
 * [Descripcion](#descripcion)
```

### Comparing `mat_enm-0.0.10/pyproject.toml` & `mat_enm-0.0.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mat_enm"
-version = "0.0.10"
+version = "0.0.11"
 authors = [
     { name="lucas", email="lucas.larroque@iquall.net" },
 ]
 description = "https://gitlab.com/lucas.larroque/mat-lib/-/blob/main/mat_enm/README.md"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `mat_enm-0.0.10/PKG-INFO` & `mat_enm-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat_enm
-Version: 0.0.10
+Version: 0.0.11
 Summary: https://gitlab.com/lucas.larroque/mat-lib/-/blob/main/mat_enm/README.md
 Project-URL: Homepage, https://gitlab.com/lucas.larroque/mat-lib/-/blob/main/mat_enm
 Project-URL: Bug Tracker, https://gitlab.com/lucas.larroque/mat-lib/-/issues
 Author-email: lucas <lucas.larroque@iquall.net>
 License: MIT License
         
         Copyright (c) 2023 lucas larroque
@@ -29,15 +29,15 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# mat-vertica
+# mat-enm
 
 [![PyPI version](https://img.shields.io/pypi/v/mat-vertica?color=brightgreen&label=PyPI%20package)](https://pypi.org/project/mat-enm/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vertica-python.svg)](https://www.python.org/downloads/)
 
 ## Lista de contenido
 
 * [Descripcion](#descripcion)
```

