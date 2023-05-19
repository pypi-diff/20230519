# Comparing `tmp/cancelchain-1.3.2.tar.gz` & `tmp/cancelchain-1.4.0.tar.gz`

## Comparing `cancelchain-1.3.2.tar` & `cancelchain-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/__init__.py
--rw-r--r--   0        0        0    17905 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/api.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/api_client.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/application.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/block.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/browser.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/cache.py
--rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/chain.py
--rw-r--r--   0        0        0    29702 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/command.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/config.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/console.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/database.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/exceptions.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/miller.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/milling.py
--rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/models.py
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/node.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/payload.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/schema.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/signals.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/tasks.py
--rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/transaction.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/util.py
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/wallet.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/templates/base.html
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/templates/block.html
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/templates/chains.html
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/templates/index.html
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 cancelchain-1.3.2/src/cancelchain/templates/transaction.html
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cancelchain-1.3.2/.gitignore
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cancelchain-1.3.2/LICENSE
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 cancelchain-1.3.2/README.rst
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cancelchain-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 cancelchain-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/__init__.py
+-rw-r--r--   0        0        0    17905 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/api.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/api_client.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/application.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/block.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/browser.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/cache.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/chain.py
+-rw-r--r--   0        0        0    29702 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/command.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/config.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/console.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/database.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/exceptions.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/miller.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/milling.py
+-rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/models.py
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/node.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/payload.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/schema.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/signals.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/tasks.py
+-rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/transaction.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/util.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/wallet.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/templates/base.html
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/templates/block.html
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/templates/chains.html
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/templates/index.html
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/templates/transaction.html
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cancelchain-1.4.0/.gitignore
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cancelchain-1.4.0/LICENSE
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 cancelchain-1.4.0/README.rst
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cancelchain-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9823 2020-02-02 00:00:00.000000 cancelchain-1.4.0/PKG-INFO
```

### Comparing `cancelchain-1.3.2/src/cancelchain/__init__.py` & `cancelchain-1.4.0/src/cancelchain/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,41 +15,51 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import click
 from flask import Flask
 from flask.cli import FlaskGroup
 
-__version__ = "1.3.2"
+__version__ = "1.4.0"
 
 
-def create_app(app=None, register_browser=True, test_config=None):
+def create_app(app=None, config_map=None, register_browser=True):
     from .application import init_app
     from .cache import cache
     from .config import EnvAppSettings
     from .database import db
     from .tasks import init_tasks
 
     app = app or Flask(__name__)
+
     app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
+    app.config['CACHE_TYPE'] = 'NullCache'
 
-    if not test_config:
-        app.config.from_object(EnvAppSettings.from_env())
-        app.config.from_envvar('CANCELCHAIN_SETTINGS', silent=True)
-    else:
-        app.config.from_object(EnvAppSettings())
-        app.config.from_mapping(test_config)
+    app.config.from_prefixed_env()
+    app.config.from_object(EnvAppSettings.from_env())
+    app.config.from_envvar('CANCELCHAIN_SETTINGS', silent=True)
+    if config_map:
+        app.config.from_mapping(config_map)
 
     init_app(app, register_browser=register_browser)
+
     try:
         db.init_app(app)
     except RuntimeError as e:
         app.logger.error(e)
-    cache.init_app(app)
-    init_tasks(app)
+
+    try:
+        cache.init_app(app)
+    except Exception as e:
+        app.logger.error(e)
+
+    try:
+        init_tasks(app)
+    except Exception as e:
+        app.logger.error(e)
 
     @app.shell_context_processor
     def make_shell_context():
         return {'app': app, 'db': db}
 
     return app
```

### Comparing `cancelchain-1.3.2/src/cancelchain/api.py` & `cancelchain-1.4.0/src/cancelchain/api.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/api_client.py` & `cancelchain-1.4.0/src/cancelchain/api_client.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/application.py` & `cancelchain-1.4.0/src/cancelchain/application.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/block.py` & `cancelchain-1.4.0/src/cancelchain/block.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/browser.py` & `cancelchain-1.4.0/src/cancelchain/browser.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/chain.py` & `cancelchain-1.4.0/src/cancelchain/chain.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/command.py` & `cancelchain-1.4.0/src/cancelchain/command.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/config.py` & `cancelchain-1.4.0/src/cancelchain/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,18 +25,14 @@
         return c
 
 
 @dataclass
 class EnvAppSettings(EnvironSettings):
     _prefix: ClassVar[str] = 'CC_'
 
-    SECRET_KEY: str = field(default=None)
-    SQLALCHEMY_DATABASE_URI: str = field(default=None)
-    CACHE_TYPE: str = field(default='NullCache')
-    CELERY_BROKER_URL: str = field(default=None)
     NODE_HOST: str = field(default=None)
     PEERS: list[str] = field(default_factory=list)
     API_CLIENT_TIMEOUT: int = field(default=10)
     API_ASYNC_PROCESSING: bool = field(default=False)
     DEFAULT_COMMAND_HOST: str = field(default=None)
     WALLET_DIR: str = field(default=None)
     ADMIN_ADDRESSES: list[str] = field(default_factory=list)
```

### Comparing `cancelchain-1.3.2/src/cancelchain/exceptions.py` & `cancelchain-1.4.0/src/cancelchain/exceptions.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/miller.py` & `cancelchain-1.4.0/src/cancelchain/miller.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/milling.py` & `cancelchain-1.4.0/src/cancelchain/milling.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/models.py` & `cancelchain-1.4.0/src/cancelchain/models.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/node.py` & `cancelchain-1.4.0/src/cancelchain/node.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/payload.py` & `cancelchain-1.4.0/src/cancelchain/payload.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/schema.py` & `cancelchain-1.4.0/src/cancelchain/schema.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/tasks.py` & `cancelchain-1.4.0/src/cancelchain/tasks.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/transaction.py` & `cancelchain-1.4.0/src/cancelchain/transaction.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/util.py` & `cancelchain-1.4.0/src/cancelchain/util.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/wallet.py` & `cancelchain-1.4.0/src/cancelchain/wallet.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/templates/base.html` & `cancelchain-1.4.0/src/cancelchain/templates/base.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/templates/block.html` & `cancelchain-1.4.0/src/cancelchain/templates/block.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/templates/chains.html` & `cancelchain-1.4.0/src/cancelchain/templates/chains.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/templates/index.html` & `cancelchain-1.4.0/src/cancelchain/templates/index.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/src/cancelchain/templates/transaction.html` & `cancelchain-1.4.0/src/cancelchain/templates/transaction.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/.gitignore` & `cancelchain-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/LICENSE` & `cancelchain-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/README.rst` & `cancelchain-1.4.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -12,78 +12,66 @@
 ===========
 
 Requirements
 ------------
 
 Python >= 3.9
 
-Installation
-------------
+Install
+-------
 
 Install CancelChain using pip:
 
 .. code-block:: console
 
   $ pip install cancelchain
 
 It is recommended that a `python virtual environment`_ is used for `all <https://realpython.com/python-virtual-environments-a-primer/#avoid-system-pollution>`__ `the <https://realpython.com/python-virtual-environments-a-primer/#sidestep-dependency-conflicts>`__ `usual <https://realpython.com/python-virtual-environments-a-primer/#minimize-reproducibility-issues>`__ `reasons <https://realpython.com/python-virtual-environments-a-primer/#dodge-installation-privilege-lockouts>`_.
 
 
-Configuration
--------------
+Configure
+---------
+
+Create a `python-dotenv`_ ``.env`` file. The ``cancelchain`` command loads a ``.env`` file in the current working directory by default.  See `dotenv documentation`_ to locate the file elsewhere. The following ``cancelchain`` command examples assume that the ``.env`` file is loaded by default.
 
-Create a `python-dotenv`_ ``.env`` file. Here is an example minimal configuration:
+A minimal ``.env`` configuration file:
 
 .. code-block:: console
 
   # Flask Settings
   FLASK_APP=cancelchain
   FLASK_RUN_HOST=0.0.0.0
+  FLASK_SECRET_KEY=0b6ceaa3b10d3e7a5dc53194
 
-  # CancelChain Settings
-  CC_SECRET_KEY=0b6ceaa3b10d3e7a5dc53194
-  CC_SQLALCHEMY_DATABASE_URI=sqlite:///cc.sqlite
+  # Flask-SQLAlchemy Settings
+  FLASK_SQLALCHEMY_DATABASE_URI=sqlite:///cc.sqlite
 
-The `CC_SECRET_KEY <https://docs.cancelchain.org/en/latest/usage.html#SECRET_KEY>`_ value should be a unique random string.
+The `FLASK_SECRET_KEY`_ value should be a unique random string.
 
 See the `Configuration Documentation`_ for more configuration settings.
 
-The ``cancelchain`` command loads a ``.env`` file by default if it is located either in the current working directory or in the ``cancelchain`` `instance folder`_. Use the ``--env-file`` parameter to specify an alternate file path.
-
-You can find the location of the `instance folder`_ by running the ``cancelchain`` `shell command`_:
-
-.. code-block:: console
-
-  $ cancelchain --env-file path/to/.env shell
-  Python 3.10.11 (main, Apr  8 2023, 14:38:50) [GCC 11.3.0] on linux
-  App: cancelchain
-  Instance: /home/arlo/.pyenv/versions/3.10.11/envs/my-cancelchain/var/cancelchain-instance
-
-By default, it is the directory ``$PREFIX/var/cancelchain-instance`` where ``$PREFIX`` is the prefix of the Python installation.
-
-The following ``cancelchain`` command examples assume that the ``.env`` file is loaded by default.
 
 Initialize
 ----------
 
 Create a local database by running the `init command`_:
 
 .. code-block:: console
 
   $ cancelchain init
 
-The `CC_SQLALCHEMY_DATABASE_URI`_ value in the example configuration above specifies a `SQLite`_ database called ``cc.sqlite`` with a file path relative to the ``cancelchain`` `instance folder`_.
+The `FLASK_SQLALCHEMY_DATABASE_URI`_ value in the example configuration above specifies a `SQLite`_ database called ``cc.sqlite`` with a file path relative to the ``cancelchain`` `instance folder`_.
 
 
 Import
 ------
 
 Download the most recent export of `CancelChain data`_. This `JSON Lines`_ file is updated at every blockchain epoch (2016 blocks or approximately every two weeks).
 
-Next, run the `import command`_, passing it the location of the downloaded file:
+Run the `import command`_, passing it the location of the downloaded file:
 
 .. code-block:: console
 
   $ cancelchain import path/to/cancelchain.jsonl
 
 This command could take a while to run depending on your computer and the number of blocks imported. A progress bar will display with estimated time remaining. You can run the ``import`` command multiple times and it will only import new blocks that are not yet in the database.
 
@@ -127,21 +115,21 @@
 
 The CancelChain is run by a permissioned network of nodes. A CancelChain instance requires `miller`_ or `transactor`_ role `API access`_ to a node in the network in order to have locally milled blocks or submitted transactions propagate to the official CancelChain.
 
 `The Cancel Button`_ allows `reader`_ role `API access`_ to any account that completes at least one transaction on the blockchain:
 
 1) `Register for an account`_.
 2) Submit a successful transaction for any subject. Access won't be granted until the sentiment transaction successfully completes.
-3) Click `Download Account Key`_ on the `Account`_ page to download the account's key (`PEM`_) file.
+3) Click `Download Account Key`_ on the `account page`_ to download the account's key (`PEM`_) file.
 4) Create a directory called ``wallets`` and copy the downloaded key file into it.
-5) Add the following settings to the ``.env`` configuration file. Replace ``CCTheCancelButtonAddressCC`` with the address on the `Account`_ page and ``/path/to/wallet`` with the path to the ``wallets`` directory created above:
+5) Add the following settings to the ``.env`` configuration file. Replace ``CCTheCancelButtonAddressCC`` with the address on the `account page`_ and ``/path/to/wallet`` with the path to the ``wallets`` directory created above:
 
   .. code-block:: console
 
-    # Network Settings
+    # CancelChain Settings
     CC_NODE_HOST=http://CCTheCancelButtonAddressCC@localhost:5000
     CC_PEERS=["https://CCTheCancelButtonAddressCC@thecancelbutton.com"]
     CC_DEFAULT_COMMAND_HOST=https://CCTheCancelButtonAddressCC@thecancelbutton.com
     CC_WALLET_DIR=/path/to/wallets
 
 6) Restart to load the new configuration.
 
@@ -158,37 +146,35 @@
 Reader access also allows querying data (i.e. subject counts and balances) using the CLI. See `Command Line Interface Documentation`_ for more information.
 
 If you would like to be granted other `API access`_ to a node in the CancelChain network, send an email to contact@cancelchain.org including what kind of role you'd like (e.g. `reader`_, `transactor`_, or `miller`_) and how you intend to use it (e.g. research, business, non-profit, hobby).
 
 See the `documentation`_ for some potential development ideas.
 
 
-.. _Account: https://thecancelbutton.com/account
+.. _account page: https://thecancelbutton.com/account
 .. _API access: https://docs.cancelchain.org/en/latest/api.html#api-roles
 .. _API Documentation: https://docs.cancelchain.org/en/latest/api.html
 .. _Blog: https://blog.cancelchain.org
 .. _CancelChain data: https://storage.googleapis.com/blocks.cancelchain.org/cancelchain.jsonl
-.. _CC_SECRET_KEY: https://docs.cancelchain.org/en/latest/usage.html#SECRET_KEY
-.. _CC_SQLALCHEMY_DATABASE_URI: https://docs.cancelchain.org/en/latest/usage.html#SQLALCHEMY_DATABASE_URI
+.. _FLASK_SECRET_KEY: https://docs.cancelchain.org/en/latest/usage.html#SECRET_KEY
+.. _FLASK_SQLALCHEMY_DATABASE_URI: https://docs.cancelchain.org/en/latest/usage.html#SQLALCHEMY_DATABASE_URI
 .. _Command Line Interface Documentation: https://docs.cancelchain.org/en/latest/usage.html#command-line-interface
 .. _Configuration Documentation: https://docs.cancelchain.org/en/latest/usage.html#configuration
 .. _documentation: https://docs.cancelchain.org
 .. _Documentation: https://docs.cancelchain.org
+.. _dotenv documentation: https://docs.cancelchain.org/en/latest/usage.html#dotenv
 .. _Download Account Key: https://thecancelbutton.com/pem
 .. _import command: https://docs.cancelchain.org/en/latest/usage.html#import
 .. _init command: https://docs.cancelchain.org/en/latest/usage.html#init
 .. _instance folder: https://flask.palletsprojects.com/en/2.2.x/config/#instance-folders
 .. _JSON Lines: https://jsonlines.org/
 .. _miller: https://docs.cancelchain.org/en/latest/api.html#miller
 .. _PEM: https://en.wikipedia.org/wiki/Privacy-Enhanced_Mail
 .. _Project Home Page: https://cancelchain.org
 .. _python virtual environment: https://docs.python.org/3/library/venv.html
 .. _python-dotenv: https://pypi.org/project/python-dotenv/
 .. _reader: https://docs.cancelchain.org/en/latest/api.html#reader
 .. _Register for an account: https://thecancelbutton.com/register
-.. _running milling processes: https://docs.cancelchain.org/en/latest/usage.html#mill
-.. _shell command: https://flask.palletsprojects.com/en/2.2.x/cli/#open-a-shell
-.. _sock puppet accounts: https://en.wikipedia.org/wiki/Sock_puppet_account
 .. _SQLite: https://sqlite.org/index.html
 .. _sync command: https://docs.cancelchain.org/en/latest/usage.html#sync
 .. _The Cancel Button: https://thecancelbutton.com
 .. _transactor: https://docs.cancelchain.org/en/latest/api.html#transactor
```

### Comparing `cancelchain-1.3.2/pyproject.toml` & `cancelchain-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cancelchain-1.3.2/PKG-INFO` & `cancelchain-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cancelchain
-Version: 1.3.2
+Version: 1.4.0
 Summary: A Blockchain of Accountability, Forgiveness, and Support
 Project-URL: Homepage, https://cancelchain.org
 Project-URL: Documentation, https://docs.cancelchain.org
 Project-URL: Source, https://github.com/cancelchain/cancelchain
 Project-URL: Tracker, https://github.com/cancelchain/cancelchain/issues
 Author-email: Thomas Bohmbach Jr <tom@cancelchain.org>
 License-Expression: MIT
@@ -55,78 +55,66 @@
 ===========
 
 Requirements
 ------------
 
 Python >= 3.9
 
-Installation
-------------
+Install
+-------
 
 Install CancelChain using pip:
 
 .. code-block:: console
 
   $ pip install cancelchain
 
 It is recommended that a `python virtual environment`_ is used for `all <https://realpython.com/python-virtual-environments-a-primer/#avoid-system-pollution>`__ `the <https://realpython.com/python-virtual-environments-a-primer/#sidestep-dependency-conflicts>`__ `usual <https://realpython.com/python-virtual-environments-a-primer/#minimize-reproducibility-issues>`__ `reasons <https://realpython.com/python-virtual-environments-a-primer/#dodge-installation-privilege-lockouts>`_.
 
 
-Configuration
--------------
+Configure
+---------
+
+Create a `python-dotenv`_ ``.env`` file. The ``cancelchain`` command loads a ``.env`` file in the current working directory by default.  See `dotenv documentation`_ to locate the file elsewhere. The following ``cancelchain`` command examples assume that the ``.env`` file is loaded by default.
 
-Create a `python-dotenv`_ ``.env`` file. Here is an example minimal configuration:
+A minimal ``.env`` configuration file:
 
 .. code-block:: console
 
   # Flask Settings
   FLASK_APP=cancelchain
   FLASK_RUN_HOST=0.0.0.0
+  FLASK_SECRET_KEY=0b6ceaa3b10d3e7a5dc53194
 
-  # CancelChain Settings
-  CC_SECRET_KEY=0b6ceaa3b10d3e7a5dc53194
-  CC_SQLALCHEMY_DATABASE_URI=sqlite:///cc.sqlite
+  # Flask-SQLAlchemy Settings
+  FLASK_SQLALCHEMY_DATABASE_URI=sqlite:///cc.sqlite
 
-The `CC_SECRET_KEY <https://docs.cancelchain.org/en/latest/usage.html#SECRET_KEY>`_ value should be a unique random string.
+The `FLASK_SECRET_KEY`_ value should be a unique random string.
 
 See the `Configuration Documentation`_ for more configuration settings.
 
-The ``cancelchain`` command loads a ``.env`` file by default if it is located either in the current working directory or in the ``cancelchain`` `instance folder`_. Use the ``--env-file`` parameter to specify an alternate file path.
-
-You can find the location of the `instance folder`_ by running the ``cancelchain`` `shell command`_:
-
-.. code-block:: console
-
-  $ cancelchain --env-file path/to/.env shell
-  Python 3.10.11 (main, Apr  8 2023, 14:38:50) [GCC 11.3.0] on linux
-  App: cancelchain
-  Instance: /home/arlo/.pyenv/versions/3.10.11/envs/my-cancelchain/var/cancelchain-instance
-
-By default, it is the directory ``$PREFIX/var/cancelchain-instance`` where ``$PREFIX`` is the prefix of the Python installation.
-
-The following ``cancelchain`` command examples assume that the ``.env`` file is loaded by default.
 
 Initialize
 ----------
 
 Create a local database by running the `init command`_:
 
 .. code-block:: console
 
   $ cancelchain init
 
-The `CC_SQLALCHEMY_DATABASE_URI`_ value in the example configuration above specifies a `SQLite`_ database called ``cc.sqlite`` with a file path relative to the ``cancelchain`` `instance folder`_.
+The `FLASK_SQLALCHEMY_DATABASE_URI`_ value in the example configuration above specifies a `SQLite`_ database called ``cc.sqlite`` with a file path relative to the ``cancelchain`` `instance folder`_.
 
 
 Import
 ------
 
 Download the most recent export of `CancelChain data`_. This `JSON Lines`_ file is updated at every blockchain epoch (2016 blocks or approximately every two weeks).
 
-Next, run the `import command`_, passing it the location of the downloaded file:
+Run the `import command`_, passing it the location of the downloaded file:
 
 .. code-block:: console
 
   $ cancelchain import path/to/cancelchain.jsonl
 
 This command could take a while to run depending on your computer and the number of blocks imported. A progress bar will display with estimated time remaining. You can run the ``import`` command multiple times and it will only import new blocks that are not yet in the database.
 
@@ -170,21 +158,21 @@
 
 The CancelChain is run by a permissioned network of nodes. A CancelChain instance requires `miller`_ or `transactor`_ role `API access`_ to a node in the network in order to have locally milled blocks or submitted transactions propagate to the official CancelChain.
 
 `The Cancel Button`_ allows `reader`_ role `API access`_ to any account that completes at least one transaction on the blockchain:
 
 1) `Register for an account`_.
 2) Submit a successful transaction for any subject. Access won't be granted until the sentiment transaction successfully completes.
-3) Click `Download Account Key`_ on the `Account`_ page to download the account's key (`PEM`_) file.
+3) Click `Download Account Key`_ on the `account page`_ to download the account's key (`PEM`_) file.
 4) Create a directory called ``wallets`` and copy the downloaded key file into it.
-5) Add the following settings to the ``.env`` configuration file. Replace ``CCTheCancelButtonAddressCC`` with the address on the `Account`_ page and ``/path/to/wallet`` with the path to the ``wallets`` directory created above:
+5) Add the following settings to the ``.env`` configuration file. Replace ``CCTheCancelButtonAddressCC`` with the address on the `account page`_ and ``/path/to/wallet`` with the path to the ``wallets`` directory created above:
 
   .. code-block:: console
 
-    # Network Settings
+    # CancelChain Settings
     CC_NODE_HOST=http://CCTheCancelButtonAddressCC@localhost:5000
     CC_PEERS=["https://CCTheCancelButtonAddressCC@thecancelbutton.com"]
     CC_DEFAULT_COMMAND_HOST=https://CCTheCancelButtonAddressCC@thecancelbutton.com
     CC_WALLET_DIR=/path/to/wallets
 
 6) Restart to load the new configuration.
 
@@ -201,37 +189,35 @@
 Reader access also allows querying data (i.e. subject counts and balances) using the CLI. See `Command Line Interface Documentation`_ for more information.
 
 If you would like to be granted other `API access`_ to a node in the CancelChain network, send an email to contact@cancelchain.org including what kind of role you'd like (e.g. `reader`_, `transactor`_, or `miller`_) and how you intend to use it (e.g. research, business, non-profit, hobby).
 
 See the `documentation`_ for some potential development ideas.
 
 
-.. _Account: https://thecancelbutton.com/account
+.. _account page: https://thecancelbutton.com/account
 .. _API access: https://docs.cancelchain.org/en/latest/api.html#api-roles
 .. _API Documentation: https://docs.cancelchain.org/en/latest/api.html
 .. _Blog: https://blog.cancelchain.org
 .. _CancelChain data: https://storage.googleapis.com/blocks.cancelchain.org/cancelchain.jsonl
-.. _CC_SECRET_KEY: https://docs.cancelchain.org/en/latest/usage.html#SECRET_KEY
-.. _CC_SQLALCHEMY_DATABASE_URI: https://docs.cancelchain.org/en/latest/usage.html#SQLALCHEMY_DATABASE_URI
+.. _FLASK_SECRET_KEY: https://docs.cancelchain.org/en/latest/usage.html#SECRET_KEY
+.. _FLASK_SQLALCHEMY_DATABASE_URI: https://docs.cancelchain.org/en/latest/usage.html#SQLALCHEMY_DATABASE_URI
 .. _Command Line Interface Documentation: https://docs.cancelchain.org/en/latest/usage.html#command-line-interface
 .. _Configuration Documentation: https://docs.cancelchain.org/en/latest/usage.html#configuration
 .. _documentation: https://docs.cancelchain.org
 .. _Documentation: https://docs.cancelchain.org
+.. _dotenv documentation: https://docs.cancelchain.org/en/latest/usage.html#dotenv
 .. _Download Account Key: https://thecancelbutton.com/pem
 .. _import command: https://docs.cancelchain.org/en/latest/usage.html#import
 .. _init command: https://docs.cancelchain.org/en/latest/usage.html#init
 .. _instance folder: https://flask.palletsprojects.com/en/2.2.x/config/#instance-folders
 .. _JSON Lines: https://jsonlines.org/
 .. _miller: https://docs.cancelchain.org/en/latest/api.html#miller
 .. _PEM: https://en.wikipedia.org/wiki/Privacy-Enhanced_Mail
 .. _Project Home Page: https://cancelchain.org
 .. _python virtual environment: https://docs.python.org/3/library/venv.html
 .. _python-dotenv: https://pypi.org/project/python-dotenv/
 .. _reader: https://docs.cancelchain.org/en/latest/api.html#reader
 .. _Register for an account: https://thecancelbutton.com/register
-.. _running milling processes: https://docs.cancelchain.org/en/latest/usage.html#mill
-.. _shell command: https://flask.palletsprojects.com/en/2.2.x/cli/#open-a-shell
-.. _sock puppet accounts: https://en.wikipedia.org/wiki/Sock_puppet_account
 .. _SQLite: https://sqlite.org/index.html
 .. _sync command: https://docs.cancelchain.org/en/latest/usage.html#sync
 .. _The Cancel Button: https://thecancelbutton.com
 .. _transactor: https://docs.cancelchain.org/en/latest/api.html#transactor
```

