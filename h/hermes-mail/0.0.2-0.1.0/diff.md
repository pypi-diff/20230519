# Comparing `tmp/hermes_mail-0.0.2.tar.gz` & `tmp/hermes_mail-0.1.0.tar.gz`

## Comparing `hermes_mail-0.0.2.tar` & `hermes_mail-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/hermes_mail/__about__.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/hermes_mail/__init__.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/hermes_mail/_src/hermes_mail.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/LICENSE
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hermes_mail-0.1.0/hermes_mail/__about__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 hermes_mail-0.1.0/hermes_mail/__init__.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 hermes_mail-0.1.0/hermes_mail/_src/hermes_mail.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hermes_mail-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hermes_mail-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 hermes_mail-0.1.0/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 hermes_mail-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 hermes_mail-0.1.0/PKG-INFO
```

### Comparing `hermes_mail-0.0.2/hermes_mail/_src/hermes_mail.py` & `hermes_mail-0.1.0/hermes_mail/_src/hermes_mail.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import smtplib
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
-from typing import List
+from typing import List, Union
 
 # Set up logging with metadata
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(name)s: %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
@@ -23,55 +23,55 @@
     """
     import re
 
     pattern = re.compile(r"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$")
     return True if pattern.match(email) else False
 
 
-class Client:
+class EmailClient:
     """
     A class for sending emails via Gmail.
 
     Args:
         sender_email (str): The sender's email address.
-        password (str): The password for the sender's email account.
+        sender_password (str): The password for the sender's email account.
 
     Attributes:
         sender_email (str): The sender's email address.
-        password (str): The password for the sender's email account.
+        sender_password (str): The password for the sender's email account.
 
     """
 
-    def __init__(self, sender_email: str, password: str):
+    def __init__(self, sender_email: str, sender_password: str):
         self.logger = logging.getLogger(__name__)
         self.sender_email = sender_email
         if not self.sender_email:
             raise ValueError("No sender email provided during initialization.")
 
         if not validate_email(self.sender_email):
             raise ValueError("Invalid sender email provided. Must be a valid email address.")
 
-        self.password = password
-        if not self.password:
+        self.sender_password = sender_password
+        if not self.sender_password:
             raise ValueError("No password provided during initialization.")
 
-    def send_email(self, receiver_emails: List[str], subject: str = "Empty subject", body: str = "Empty body"):
+    def send_email(self, receiver_emails: Union[List[str], str], subject: str = "Empty subject", body: str = "Empty body"):
         """Send an email via Gmail.
 
         Args:
-            receiver_email (List[str]): A list of receiver's email addresses.
+            receiver_emails (Union[List[str], str]): A list or a single string of receiver's email addresses.
             subject (str): The subject line of the email.
             body (str): The body text of the email.
 
         Returns:
             None.
         """
         # Validate inputs
-        if not type(receiver_emails) == list:
-            raise ValueError("receiver_emails must be a list of receiver emails.")
+        if isinstance(receiver_emails, str):
+            receiver_emails = [receiver_emails]
 
         if not receiver_emails:
             raise ValueError("No receiver emails provided.")
 
         for receiver_email in receiver_emails:
             if not validate_email(receiver_email):
                 raise ValueError("Invalid receiver email provided. Must be valid email addresses.")
@@ -84,12 +84,12 @@
         message.attach(MIMEText(body, "plain"))
 
         text = message.as_string()
 
         try:
             with smtplib.SMTP(host="smtp.gmail.com", port=587) as server:
                 server.starttls()
-                server.login(self.sender_email, self.password)
+                server.login(self.sender_email, self.sender_password)
                 server.sendmail(self.sender_email, receiver_emails, text)
                 self.logger.info("\033[32mEmail sent successfully to {}\033[0m".format(", ".join(receiver_emails)))
         except Exception as e:
             self.logger.error("\033[31mFailed to send email. Error: {}\033[0m".format(str(e)))
```

### Comparing `hermes_mail-0.0.2/LICENSE` & `hermes_mail-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hermes_mail-0.0.2/README.md` & `hermes_mail-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Hermes Mail
 Send Python job alerts via email.
 
 ```python
-from hermes_mail import Client
+from hermes_mail import EmailClient
+import os
 
-hermes = Client(sender_email="mlguy@gmail.com", password=os.getenv("GMAIL_PASSWORD"))
+hermes = EmailClient(sender_email="mlguy@gmail.com", sender_password=os.getenv("GMAIL_PASSWORD"))
 hermes.send_email(
     receiver_emails=["foo@gmail.com", "bar@gmail.com"], 
     subject="cuda:0 is free", 
-    body="I finished training my models on cuda:0 so feel free to use it.")
+    body="I finished training my models on cuda:0 so feel free to use it."
+)
 ```
 `hermes_mail` works seamlessly within Python code to send emails. It is designed for sending job alerts upon completion of long-running jobs. This currently only works when the sender is a Gmail account.
 
 ## Installation
 ```bash
 pip install hermes-mail
 ```
```

### Comparing `hermes_mail-0.0.2/pyproject.toml` & `hermes_mail-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hermes_mail-0.0.2/PKG-INFO` & `hermes_mail-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermes-mail
-Version: 0.0.2
+Version: 0.1.0
 Summary: Send Python job alerts via email
 Project-URL: Homepage, https://github.com/ishan0102/hermes-mail
 Project-URL: Bug Tracker, https://github.com/ishan0102/hermes-mail/issues
 Author-email: Ishan Shah <ishan0102@utexas.edu>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -13,21 +13,23 @@
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # Hermes Mail
 Send Python job alerts via email.
 
 ```python
-from hermes_mail import Client
+from hermes_mail import EmailClient
+import os
 
-hermes = Client(sender_email="mlguy@gmail.com", password=os.getenv("GMAIL_PASSWORD"))
+hermes = EmailClient(sender_email="mlguy@gmail.com", sender_password=os.getenv("GMAIL_PASSWORD"))
 hermes.send_email(
     receiver_emails=["foo@gmail.com", "bar@gmail.com"], 
     subject="cuda:0 is free", 
-    body="I finished training my models on cuda:0 so feel free to use it.")
+    body="I finished training my models on cuda:0 so feel free to use it."
+)
 ```
 `hermes_mail` works seamlessly within Python code to send emails. It is designed for sending job alerts upon completion of long-running jobs. This currently only works when the sender is a Gmail account.
 
 ## Installation
 ```bash
 pip install hermes-mail
 ```
```

