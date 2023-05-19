# Comparing `tmp/FCSAPIAccessSDK-1.0.1.tar.gz` & `tmp/FCSAPIAccessSDK-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FCSAPIAccessSDK-1.0.1.tar", last modified: Thu Apr 14 20:13:52 2022, max compression
+gzip compressed data, was "FCSAPIAccessSDK-1.1.0.tar", last modified: Fri May 19 20:59:01 2023, max compression
```

## Comparing `FCSAPIAccessSDK-1.0.1.tar` & `FCSAPIAccessSDK-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-04-14 20:13:52.346833 FCSAPIAccessSDK-1.0.1/
-drwxrwxrwx   0        0        0        0 2022-04-14 20:13:52.333862 FCSAPIAccessSDK-1.0.1/FCSAPIAccess/
--rw-rw-rw-   0        0        0      127 2022-03-16 06:17:23.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccess/__init__.py
--rw-rw-rw-   0        0        0     3740 2022-04-14 20:02:56.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccess/api_access.py
--rw-rw-rw-   0        0        0      102 2022-04-14 20:02:56.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccess/exceptions.py
--rw-rw-rw-   0        0        0     5725 2022-04-14 19:57:41.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccess/fcs_monitoring.py
--rw-rw-rw-   0        0        0     8620 2022-04-14 19:57:41.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccess/fcs_notification.py
--rw-rw-rw-   0        0        0    53853 2022-04-14 19:57:41.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccess/fcs_project.py
--rw-rw-rw-   0        0        0     2597 2022-04-14 20:11:14.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccess/scope.py
-drwxrwxrwx   0        0        0        0 2022-04-14 20:13:52.345835 FCSAPIAccessSDK-1.0.1/FCSAPIAccessSDK.egg-info/
--rw-rw-rw-   0        0        0     1757 2022-04-14 20:13:51.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccessSDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2022-04-14 20:13:52.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccessSDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-14 20:13:51.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccessSDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-04-14 20:13:52.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccessSDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-04-14 20:13:52.000000 FCSAPIAccessSDK-1.0.1/FCSAPIAccessSDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-03-16 05:36:31.000000 FCSAPIAccessSDK-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1757 2022-04-14 20:13:52.347829 FCSAPIAccessSDK-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      765 2022-04-14 20:12:51.000000 FCSAPIAccessSDK-1.0.1/README.md
--rw-rw-rw-   0        0        0       86 2022-04-14 20:13:52.349826 FCSAPIAccessSDK-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1303 2022-04-14 20:12:51.000000 FCSAPIAccessSDK-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:59:01.800546 FCSAPIAccessSDK-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-05-19 20:59:01.725288 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/
+-rw-rw-rw-   0        0        0      127 2022-03-16 06:17:23.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/__init__.py
+-rw-rw-rw-   0        0        0     3915 2022-04-26 02:36:49.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/api_access.py
+-rw-rw-rw-   0        0        0      102 2022-04-14 20:02:56.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/exceptions.py
+-rw-rw-rw-   0        0        0     6023 2023-05-19 20:53:50.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_monitoring.py
+-rw-rw-rw-   0        0        0     9389 2023-05-19 20:53:50.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_notification.py
+-rw-rw-rw-   0        0        0    66135 2023-05-19 20:53:50.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_project.py
+-rw-rw-rw-   0        0        0     5927 2023-05-19 20:53:50.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_translation.py
+-rw-rw-rw-   0        0        0     5071 2023-05-19 20:26:24.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/scope.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:59:01.745318 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/
+-rw-rw-rw-   0        0        0     1887 2023-05-19 20:59:01.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-05-19 20:59:01.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 20:59:01.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 20:59:01.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-19 20:59:01.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2022-03-16 05:36:31.000000 FCSAPIAccessSDK-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1887 2023-05-19 20:59:01.800546 FCSAPIAccessSDK-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2022-04-14 20:12:51.000000 FCSAPIAccessSDK-1.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-19 20:59:01.807529 FCSAPIAccessSDK-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-05-19 20:56:56.000000 FCSAPIAccessSDK-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:59:01.797551 FCSAPIAccessSDK-1.1.0/tests/
+-rw-rw-rw-   0        0        0     1203 2022-04-14 20:07:43.000000 FCSAPIAccessSDK-1.1.0/tests/test_auth.py
```

### Comparing `FCSAPIAccessSDK-1.0.1/FCSAPIAccess/api_access.py` & `FCSAPIAccessSDK-1.1.0/FCSAPIAccess/api_access.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import FCSAPIAccess.scope as scopes
 import FCSAPIAccess.exceptions as exceptions
 
 import FCSAPIAccess.fcs_monitoring as fcs_monitoring
 import FCSAPIAccess.fcs_notification as fcs_notification
 import FCSAPIAccess.fcs_project as fcs_project
+import FCSAPIAccess.fcs_translation as fcs_translation
 
 
 class FCSAPIAccess:
     url_base = "https://fangcloudservices.pythonanywhere.com/api/v1"
 
     def __init__(
             self, client_id: str, client_secret: str, scope: typing.Union[typing.List[scopes.Scope], scopes.Scope]
@@ -24,19 +25,21 @@
             self._scope = [self._scope]
 
         self._access_token, self._refresh_token = self.client_credentials()
 
         self.monitoring = fcs_monitoring.FangMonitoringServices(self._access_token)
         self.notification = fcs_notification.FangNotificationServices(self._access_token)
         self.project = fcs_project.FangCloudServicesAPI(self._access_token)
+        self.translation = fcs_translation.FangTranslationServices(self._access_token)
 
         self._composite_objects = [
             self.monitoring,
             self.notification,
-            self.project
+            self.project,
+            self.translation
         ]
 
         for o in self._composite_objects:
             o._status_check = self._check_status
 
     def client_credentials(self) -> typing.Tuple[str, str]:
         r = requests.post(self.url_base + "/project/oauth2", json={
```

### Comparing `FCSAPIAccessSDK-1.0.1/FCSAPIAccess/fcs_monitoring.py` & `FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_monitoring.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         
     def _url_encode(self, text: str) -> str:
         return urllib.parse.quote_plus(str(text))
     
     def get_urls(self) -> dict:
         """
         This endpoint retrieves the URLs you are monitoring
+        
+        **Requires Scope**: `monitor:view:url`
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
             "GET", 
@@ -52,14 +54,16 @@
         return self._check_status(r, lambda: self.get_urls(**local_vars))
         
     def create_url(self, name, url, interval, notification_channel) -> dict:
         """
         Adds a new URL to your list of URLs being monitored
         
         `notification_channel` is the ID of the channel where change notifications will automatically be sent. This is part of Notification services.
+        
+        **Requires Scope**: `monitor:update:url`
         :param name:
         :param url:
         :param interval:
         :param notification_channel:
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
@@ -81,14 +85,16 @@
         return self._check_status(r, lambda: self.create_url(**local_vars))
         
     def update_url(self, id, name, url, interval, notification_channel) -> dict:
         """
         Updates the data related to the specified URL
         
         `notification_channel` is the ID of the channel where change notifications will automatically be sent. This is part of Notification services.
+        
+        **Requires Scope**: `monitor:update:url`
         :param id: 
         :param name:
         :param url:
         :param interval:
         :param notification_channel:
         """
         local_vars = locals()
@@ -111,14 +117,16 @@
         return self._check_status(r, lambda: self.update_url(**local_vars))
         
     def delete_url(self, id) -> dict:
         """
         Deletes the specified URL and wipes all of its history.
         
         **WARNING**: This **CAN NOT** be undone!
+        
+        **Requires Scope**: `monitor:update:url`
         :param id: 
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
@@ -132,14 +140,16 @@
     def get_url_history(self, id) -> dict:
         """
         Pulls all the history of either all or one of the monitored endpoints.
         
         Note that the response only contains state changes in chronological order.
         
         It is assumed that each state carries over to the next record. For example, if a state starts at `00:25:26` and the next state begins at `10:25:26`, it is assumed that the URL was in that state for the full 10 hour interval.
+        
+        **Requires Scope**: `monitor:view:state`
         :param id: Optional URL ID to pull the history of a single tracked URL
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
```

### Comparing `FCSAPIAccessSDK-1.0.1/FCSAPIAccess/fcs_notification.py` & `FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_notification.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         
     def _url_encode(self, text: str) -> str:
         return urllib.parse.quote_plus(str(text))
     
     def get_channels(self) -> dict:
         """
         Retrieves a list of existing channels
+        
+        **Requires Scope**: `notification:view:channel`
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
             "GET", 
@@ -48,14 +50,16 @@
         )
         
         return self._check_status(r, lambda: self.get_channels(**local_vars))
         
     def create_channel(self, name) -> dict:
         """
         Creates a new channel
+        
+        **Requires Scope**: `notification:update:channel`
         :param name:
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         headers["Content-Type"] = "application/json"
@@ -69,14 +73,16 @@
         )
         
         return self._check_status(r, lambda: self.create_channel(**local_vars))
         
     def update_channel(self, id, name) -> dict:
         """
         Updates the channel information
+        
+        **Requires Scope**: `notification:update:channel`
         :param id: 
         :param name:
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
@@ -91,14 +97,16 @@
         )
         
         return self._check_status(r, lambda: self.update_channel(**local_vars))
         
     def remove_channel(self, id) -> dict:
         """
         Deletes a channel and all of its history
+        
+        **Requires Scope**: `notification:update:channel`
         :param id: 
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
@@ -108,14 +116,16 @@
         )
         
         return self._check_status(r, lambda: self.remove_channel(**local_vars))
         
     def get_recipients(self, channel) -> dict:
         """
         Returns all of the recipients which have been added to a channel
+        
+        **Requires Scope**: `notification:view:channel_recipient`
         :param channel: 
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
@@ -125,14 +135,16 @@
         )
         
         return self._check_status(r, lambda: self.get_recipients(**local_vars))
         
     def add_recipient(self, channel, recipient) -> dict:
         """
         Adds the specified recipient to the specified channel
+        
+        **Requires Scope**: `notification:update:channel_recipient`
         :param channel: 
         :param recipient:
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
@@ -147,14 +159,16 @@
         )
         
         return self._check_status(r, lambda: self.add_recipient(**local_vars))
         
     def remove_recipient(self, channel, recipient) -> dict:
         """
         Removes the specified recipient from the specified channel
+        
+        **Requires Scope**: `notification:update:channel_recipient`
         :param channel: 
         :param recipient: 
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
@@ -167,14 +181,16 @@
         return self._check_status(r, lambda: self.remove_recipient(**local_vars))
         
     def pull_message(self, channel) -> dict:
         """
         Pulls the queued messages. Note that once a message is pulled, you will not be able to pull it again from this endpoint.
         
         Services authenticated using the same `client_id` and `client_secret` are considered the same application, and so pulling a message from one instance of an app will prevent other apps authenticated with the same credentials from being able to pull that message.
+        
+        **Requires Scope**: `notification:pull:message`
         :param channel: 
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
@@ -183,15 +199,17 @@
             headers=headers
         )
         
         return self._check_status(r, lambda: self.pull_message(**local_vars))
         
     def push_message(self, channel, name, body) -> dict:
         """
-        Pushes a new message to the queue. In the JSON you may specify `name`, `body` or `code`. All 3 are optional.
+        Pushes a new message to the queue. In the JSON you may specify `name`, `body` or `code`. All 3 are optional. This does, however, mean that you can push empty messages.
+        
+        **Requires Scope**: `notification:push:message`
         :param channel: 
         :param name:
         :param body:
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
@@ -212,14 +230,16 @@
     def get_history(self, channel) -> dict:
         """
         Pulls the message history of the specified channel.
         
         Messages can only be seen for up to 24 hours.
         
         Note that if the `sender` is `null`, the message was either system generated, or sent through the message sender.
+        
+        **Requires Scope**: `notification:view:history`
         :param channel: The ID of the channel to pull message history from
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
```

### Comparing `FCSAPIAccessSDK-1.0.1/FCSAPIAccess/fcs_project.py` & `FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_project.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,98 @@
         check = self._status_check(r, retry)
         
         return r.json() if check is None else check
         
     def _url_encode(self, text: str) -> str:
         return urllib.parse.quote_plus(str(text))
     
+    def get_all_email_addresses(self, user) -> dict:
+        """
+        Retrieves the email addresses linked to a specified user.
+        :param user: The ID of the user
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "GET", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email?user={}".format(self._url_encode(user)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.get_all_email_addresses(**local_vars))
+        
+    def create_email_address(self, user, email) -> dict:
+        """
+        Links the specified email address to the specified user.
+        
+        This will cause the confirmation email to be sent to the new email address.
+        :param user:
+        :param email:
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        headers["Content-Type"] = "application/json"
+        r = requests.request(
+            "POST", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email", 
+            headers=headers,
+            json={
+                "email": email,
+                "user": user
+            }
+        )
+        
+        return self._check_status(r, lambda: self.create_email_address(**local_vars))
+        
+    def update_email_address(self, id, user, email) -> dict:
+        """
+        Updates a user's existing email address
+        :param id: The ID of the email address
+        :param user:
+        :param email:
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        headers["Content-Type"] = "application/json"
+        r = requests.request(
+            "PUT", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email?id={}".format(self._url_encode(id)), 
+            headers=headers,
+            json={
+                "email": email,
+                "user": user
+            }
+        )
+        
+        return self._check_status(r, lambda: self.update_email_address(**local_vars))
+        
+    def remove_email_address(self, id, user) -> dict:
+        """
+        
+        :param id: The ID of the email address to remove
+        :param user: The ID of the user ascociated with the email address
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "DELETE", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email?id={}&user={}".format(self._url_encode(id), self._url_encode(user)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.remove_email_address(**local_vars))
+        
     def validate_token(self, token, minified) -> dict:
         """
         Takes the specified access token which is provided by your API client, and returns the data related to the user's account.
         
         This endpoint will also detect expired and invalid tokens.
         :param token: The token you wish to validate
         :param minified: If a minified response should be created
@@ -193,14 +277,55 @@
             "GET", 
             "https://fangcloudservices.pythonanywhere.com/api/v1/project/user?id={}".format(self._url_encode(id)), 
             headers=headers
         )
         
         return self._check_status(r, lambda: self.get_user(**local_vars))
         
+    def create_user(self, data, username, email, user_role, password, mailing_lists, dob, favourite_color) -> dict:
+        """
+        StartFragment
+        
+        Sets the properties of a new user.
+        
+        If the requested `user_role` or `mailing_list` IDs do not correspond to an existing user role or mailing list, you will receive a 404 error and the update will not be made.
+        
+        Note that `dob` and `favorite_color` are cusom user fields specific to this project. Use your own fields in their place if you have specified any.
+        :param data:
+        :param username:
+        :param email:
+        :param user_role:
+        :param password:
+        :param mailing_lists:
+        :param dob:
+        :param favourite_color:
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        headers["Content-Type"] = "application/json"
+        r = requests.request(
+            "POST", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/user", 
+            headers=headers,
+            json={
+                "data": data,
+                "dob": dob,
+                "email": email,
+                "favourite_color": favourite_color,
+                "mailing_lists": mailing_lists,
+                "password": password,
+                "user_role": user_role,
+                "username": username
+            }
+        )
+        
+        return self._check_status(r, lambda: self.create_user(**local_vars))
+        
     def update_user(self, id, data, username, primary_email, user_role, active) -> dict:
         """
         Updates the properties of the specified user. Note that sending up the `data` JSON blob will overwrite the existing data so be sure to merge the data before sending.
         
         **Note** that this action can not be undone.
         
         If the requested `user_role` or `primary_email` IDs do not correspond to an existing user role or email address, you will receive a 404 error and the update will not be made.
@@ -229,97 +354,193 @@
                 "user_role": user_role,
                 "username": username
             }
         )
         
         return self._check_status(r, lambda: self.update_user(**local_vars))
         
-    def get_all_email_addresses(self, user) -> dict:
+    def get_all_email_categories(self) -> dict:
         """
-        Retrieves the email addresses linked to a specified user.
-        :param user: The ID of the user
+        
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
             "GET", 
-            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email?user={}".format(self._url_encode(user)), 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email_category", 
             headers=headers
         )
         
-        return self._check_status(r, lambda: self.get_all_email_addresses(**local_vars))
+        return self._check_status(r, lambda: self.get_all_email_categories(**local_vars))
         
-    def create_email_address(self, user, email) -> dict:
+    def create_email_category(self, name) -> dict:
         """
-        Links the specified email address to the specified user.
         
-        This will cause the confirmation email to be sent to the new email address.
-        :param user:
-        :param email:
+        :param name:
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         headers["Content-Type"] = "application/json"
         r = requests.request(
             "POST", 
-            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email_category", 
             headers=headers,
             json={
-                "email": email,
-                "user": user
+                "name": name
             }
         )
         
-        return self._check_status(r, lambda: self.create_email_address(**local_vars))
+        return self._check_status(r, lambda: self.create_email_category(**local_vars))
         
-    def update_email_address(self, id, user, email) -> dict:
+    def update_email_category(self, id, name) -> dict:
         """
-        Updates a user's existing email address
-        :param id: The ID of the email address
-        :param user:
-        :param email:
+        
+        :param id: 
+        :param name:
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         headers["Content-Type"] = "application/json"
         r = requests.request(
             "PUT", 
-            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email?id={}".format(self._url_encode(id)), 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email_category?id={}".format(self._url_encode(id)), 
             headers=headers,
             json={
-                "email": email,
-                "user": user
+                "name": name
             }
         )
         
-        return self._check_status(r, lambda: self.update_email_address(**local_vars))
+        return self._check_status(r, lambda: self.update_email_category(**local_vars))
         
-    def remove_email_address(self, id, user) -> dict:
+    def remove_email_category(self, id) -> dict:
         """
         
-        :param id: The ID of the email address to remove
-        :param user: The ID of the user ascociated with the email address
+        :param id: 
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
             "DELETE", 
-            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email?id={}&user={}".format(self._url_encode(id), self._url_encode(user)), 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/email_category?id={}".format(self._url_encode(id)), 
             headers=headers
         )
         
-        return self._check_status(r, lambda: self.remove_email_address(**local_vars))
+        return self._check_status(r, lambda: self.remove_email_category(**local_vars))
+        
+    def get_email_addresses_subscribed_to_a_category(self, category) -> dict:
+        """
+        
+        :param category: 
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "GET", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/mailing_list?category={}".format(self._url_encode(category)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.get_email_addresses_subscribed_to_a_category(**local_vars))
+        
+    def get_categories_subscribed_to_by_an_email_address(self, email) -> dict:
+        """
+        
+        :param email: 
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "GET", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/mailing_list?email={}".format(self._url_encode(email)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.get_categories_subscribed_to_by_an_email_address(**local_vars))
+        
+    def subscribe_to_category(self, email, category) -> dict:
+        """
+        
+        :param email: 
+        :param category: 
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "POST", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/mailing_list?email={}&category={}".format(self._url_encode(email), self._url_encode(category)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.subscribe_to_category(**local_vars))
+        
+    def subscribe_to_all_categories(self, email) -> dict:
+        """
+        
+        :param email: 
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "POST", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/mailing_list?email={}".format(self._url_encode(email)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.subscribe_to_all_categories(**local_vars))
+        
+    def remove_subscription_from_category(self, email, category) -> dict:
+        """
+        
+        :param email: 
+        :param category: 
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "DELETE", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/mailing_list?email={}&category={}".format(self._url_encode(email), self._url_encode(category)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.remove_subscription_from_category(**local_vars))
+        
+    def remove_subscription_from_all_categories(self, email) -> dict:
+        """
+        
+        :param email: 
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "DELETE", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/mailing_list?email={}".format(self._url_encode(email)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.remove_subscription_from_all_categories(**local_vars))
         
     def get_external_accounts(self) -> dict:
         """
         This endpoint lists the external accounts your project allows users to log in with
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
@@ -456,39 +677,45 @@
             "GET", 
             "https://fangcloudservices.pythonanywhere.com/api/v1/project", 
             headers=headers
         )
         
         return self._check_status(r, lambda: self.get_settings(**local_vars))
         
-    def change_settings(self, id, default_data, default_user_role, name, privacy_policy, terms_of_service, ignore_expired_tokens, access_token_prefix) -> dict:
+    def change_settings(self, id, default_data, default_user_role, name, privacy_policy, terms_of_service, ignore_expired_tokens, access_token_prefix, enable_password_login, alert_channel, allow_registration) -> dict:
         """
         Changes your project settings
         :param id: 
         :param default_data:
         :param default_user_role:
         :param name:
         :param privacy_policy:
         :param terms_of_service:
         :param ignore_expired_tokens:
         :param access_token_prefix:
+        :param enable_password_login:
+        :param alert_channel:
+        :param allow_registration:
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         headers["Content-Type"] = "application/json"
         r = requests.request(
             "PUT", 
             "https://fangcloudservices.pythonanywhere.com/api/v1/project?id={}".format(self._url_encode(id)), 
             headers=headers,
             json={
                 "access_token_prefix": access_token_prefix,
+                "alert_channel": alert_channel,
+                "allow_registration": allow_registration,
                 "default_data": default_data,
                 "default_user_role": default_user_role,
+                "enable_password_login": enable_password_login,
                 "ignore_expired_tokens": ignore_expired_tokens,
                 "name": name,
                 "privacy_policy": privacy_policy,
                 "terms_of_service": terms_of_service
             }
         )
         
@@ -1099,14 +1326,112 @@
             "DELETE", 
             "https://fangcloudservices.pythonanywhere.com/api/v1/project/api/scope?id={}&scope={}".format(self._url_encode(id), self._url_encode(scope)), 
             headers=headers
         )
         
         return self._check_status(r, lambda: self.remove_scope(**local_vars))
         
+    def get_sessions(self, id) -> dict:
+        """
+        Retrieves a list of active sessions for a specified application
+        :param id: The ID of the application
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "GET", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/api/session?id={}".format(self._url_encode(id)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.get_sessions(**local_vars))
+        
+    def expire_session(self, id, session) -> dict:
+        """
+        Expires the specified session. It can be refreshed via the refresh token flow.
+        
+        Note that it is possible to expire the session you are currently using for API Access. Doing so will cause the token to expire, but it can be refreshed.
+        :param id: The ID of the application
+        :param session: The ID of the session to expire
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "PUT", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/api/session?id={}&session={}".format(self._url_encode(id), self._url_encode(session)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.expire_session(**local_vars))
+        
+    def refresh_token(self, id, session) -> dict:
+        """
+        Refreshes the specified session and returns the new access and refresh tokens.
+        :param id: The ID of the application
+        :param session: The ID of the session to refresh
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "PATCH", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/api/session?id={}&session={}".format(self._url_encode(id), self._url_encode(session)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.refresh_token(**local_vars))
+        
+    def remove_session(self, id, session) -> dict:
+        """
+        Revokes an active sessions for a specified application.
+        
+        Note that it is possible to revoke the session you are currently using for API Access. Doing so will cause the token to expire and it can not be refreshed.
+        
+        This action can not be undone.
+        :param id: The ID of the application
+        :param session: The ID of the session to revoke
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "DELETE", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/api/session?id={}&session={}".format(self._url_encode(id), self._url_encode(session)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.remove_session(**local_vars))
+        
+    def remove_all_sessions(self, id) -> dict:
+        """
+        Revokes an active sessions for a specified application.
+        
+        Note that it is possible to revoke the session you are currently using for API Access. Doing so will cause the token to expire and it can not be refreshed.
+        
+        This action can not be undone.
+        :param id: The ID of the application
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "DELETE", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/api/session?id={}".format(self._url_encode(id)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.remove_all_sessions(**local_vars))
+        
     def get_tokens(self) -> dict:
         """
         Retrieves a list of your API applications which can be used to access FangCloudServices API
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
```

### Comparing `FCSAPIAccessSDK-1.0.1/FCSAPIAccessSDK.egg-info/PKG-INFO` & `FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: FCSAPIAccessSDK
-Version: 1.0.1
+Version: 1.1.0
 Summary: The SDK for project-level access to your FangCloudServices account
 Home-page: https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK
 Author: CPSuperstore
 Author-email: cpsuperstoreinc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK/issues
 Keywords: FANG,CLOUD,SERVICES,FCS,SDK,USER,MANAGEMENT,OAUTH2,SECURITY
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apple Public Source License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FangCloudServicesAPIAccessSDK
 The SDK for accessing FangCloudServices with API Access Credentials
 
@@ -43,9 +45,7 @@
 
 Or if you only require a single scope:
 ```python
 from FCSAPIAccess import FCSAPIAccess, Scope
 
 FCSAPIAccess(client_id, client_secret, Scope.FULL_ACCESS)
 ```
-
-
```

### Comparing `FCSAPIAccessSDK-1.0.1/LICENSE` & `FCSAPIAccessSDK-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.0.1/PKG-INFO` & `FCSAPIAccessSDK-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: FCSAPIAccessSDK
-Version: 1.0.1
+Version: 1.1.0
 Summary: The SDK for project-level access to your FangCloudServices account
 Home-page: https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK
 Author: CPSuperstore
 Author-email: cpsuperstoreinc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK/issues
 Keywords: FANG,CLOUD,SERVICES,FCS,SDK,USER,MANAGEMENT,OAUTH2,SECURITY
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apple Public Source License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FangCloudServicesAPIAccessSDK
 The SDK for accessing FangCloudServices with API Access Credentials
 
@@ -43,9 +45,7 @@
 
 Or if you only require a single scope:
 ```python
 from FCSAPIAccess import FCSAPIAccess, Scope
 
 FCSAPIAccess(client_id, client_secret, Scope.FULL_ACCESS)
 ```
-
-
```

### Comparing `FCSAPIAccessSDK-1.0.1/README.md` & `FCSAPIAccessSDK-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.0.1/setup.py` & `FCSAPIAccessSDK-1.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='FCSAPIAccessSDK',
-    version='1.0.1',
+    version='1.1.0',
     packages=['FCSAPIAccess'],
     url='https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK',
     license='Apache License 2.0',
     author='CPSuperstore',
     author_email='cpsuperstoreinc@gmail.com',
     description='The SDK for project-level access to your FangCloudServices account',
     long_description=long_description,
@@ -26,10 +26,13 @@
         'Intended Audience :: Developers',
         'Topic :: Security',
         'License :: OSI Approved :: Apple Public Source License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Natural Language :: English'
     ]
 )
```

