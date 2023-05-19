# Comparing `tmp/hermes_mail-0.0.1.tar.gz` & `tmp/hermes_mail-0.0.2.tar.gz`

## Comparing `hermes_mail-0.0.1.tar` & `hermes_mail-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hermes_mail-0.0.1/hermes/__about__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hermes_mail-0.0.1/hermes/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 hermes_mail-0.0.1/hermes/_src/hermes.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hermes_mail-0.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hermes_mail-0.0.1/LICENSE
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hermes_mail-0.0.1/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 hermes_mail-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 hermes_mail-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/hermes_mail/__about__.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/hermes_mail/__init__.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/hermes_mail/_src/hermes_mail.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 hermes_mail-0.0.2/PKG-INFO
```

### Comparing `hermes_mail-0.0.1/hermes/_src/hermes.py` & `hermes_mail-0.0.2/hermes_mail/_src/hermes_mail.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,43 +8,88 @@
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s %(name)s: %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
+def validate_email(email: str) -> bool:
+    """Validate an email address.
+
+    Args:
+        email (str): An email address.
+
+    Returns:
+        bool: True if the email address is valid, False otherwise.
+    """
+    import re
+
+    pattern = re.compile(r"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$")
+    return True if pattern.match(email) else False
+
+
 class Client:
-    def __init__(self, password: str):
+    """
+    A class for sending emails via Gmail.
+
+    Args:
+        sender_email (str): The sender's email address.
+        password (str): The password for the sender's email account.
+
+    Attributes:
+        sender_email (str): The sender's email address.
+        password (str): The password for the sender's email account.
+
+    """
+
+    def __init__(self, sender_email: str, password: str):
         self.logger = logging.getLogger(__name__)
+        self.sender_email = sender_email
+        if not self.sender_email:
+            raise ValueError("No sender email provided during initialization.")
+
+        if not validate_email(self.sender_email):
+            raise ValueError("Invalid sender email provided. Must be a valid email address.")
+
         self.password = password
         if not self.password:
-            self.logger.error("No email password provided. Set EMAIL_PASSWORD environment variable.")
+            raise ValueError("No password provided during initialization.")
 
-    def send_email(self, sender_email: str, receiver_email: List[str], subject: str, body: str):
+    def send_email(self, receiver_emails: List[str], subject: str = "Empty subject", body: str = "Empty body"):
         """Send an email via Gmail.
 
         Args:
-            sender_email: The sender's email address.
-            receiver_email: A list of receiver's email addresses.
-            subject: The subject line of the email.
-            body: The body text of the email.
+            receiver_email (List[str]): A list of receiver's email addresses.
+            subject (str): The subject line of the email.
+            body (str): The body text of the email.
 
         Returns:
             None.
         """
+        # Validate inputs
+        if not type(receiver_emails) == list:
+            raise ValueError("receiver_emails must be a list of receiver emails.")
+
+        if not receiver_emails:
+            raise ValueError("No receiver emails provided.")
+
+        for receiver_email in receiver_emails:
+            if not validate_email(receiver_email):
+                raise ValueError("Invalid receiver email provided. Must be valid email addresses.")
+
         # Create email
         message = MIMEMultipart()
-        message["From"] = sender_email
-        message["To"] = ", ".join(receiver_email)
+        message["From"] = self.sender_email
+        message["To"] = ", ".join(receiver_emails)
         message["Subject"] = subject
         message.attach(MIMEText(body, "plain"))
 
         text = message.as_string()
 
         try:
             with smtplib.SMTP(host="smtp.gmail.com", port=587) as server:
                 server.starttls()
-                server.login(sender_email, self.password)
-                server.sendmail(sender_email, receiver_email, text)
-                self.logger.info("\033[32mEmail sent successfully to {}\033[0m".format(", ".join(receiver_email)))
+                server.login(self.sender_email, self.password)
+                server.sendmail(self.sender_email, receiver_emails, text)
+                self.logger.info("\033[32mEmail sent successfully to {}\033[0m".format(", ".join(receiver_emails)))
         except Exception as e:
             self.logger.error("\033[31mFailed to send email. Error: {}\033[0m".format(str(e)))
```

### Comparing `hermes_mail-0.0.1/LICENSE` & `hermes_mail-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hermes_mail-0.0.1/pyproject.toml` & `hermes_mail-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "hermes-mail"
 authors = [
   { name="Ishan Shah", email="ishan0102@utexas.edu" },
 ]
-description = "Python job alerts via email"
+description = "Send Python job alerts via email"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3"
+license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/ishan0102/hermes-mail"
 "Bug Tracker" = "https://github.com/ishan0102/hermes-mail/issues"
 
 [tool.hatch.version]
-path = "hermes/__about__.py"
+path = "hermes_mail/__about__.py"
```

