# Comparing `tmp/yeref-0.1.62.tar.gz` & `tmp/yeref-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.62.tar", last modified: Tue May 16 16:19:26 2023, max compression
+gzip compressed data, was "yeref-0.1.63.tar", last modified: Fri May 19 10:28:48 2023, max compression
```

## Comparing `yeref-0.1.62.tar` & `yeref-0.1.63.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-16 16:19:26.409659 yeref-0.1.62/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-16 16:19:26.410076 yeref-0.1.62/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-16 16:19:26.410873 yeref-0.1.62/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-16 16:19:11.000000 yeref-0.1.62/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-16 16:19:26.400857 yeref-0.1.62/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.62/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   511251 2023-05-09 14:24:53.000000 yeref-0.1.62/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   200404 2023-05-16 13:39:01.000000 yeref-0.1.62/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-16 16:19:26.409029 yeref-0.1.62/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-16 16:19:26.000000 yeref-0.1.62/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-16 16:19:26.000000 yeref-0.1.62/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-16 16:19:26.000000 yeref-0.1.62/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-16 16:19:26.000000 yeref-0.1.62/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-19 10:28:48.622886 yeref-0.1.63/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-19 10:28:48.623379 yeref-0.1.63/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-19 10:28:48.624108 yeref-0.1.63/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-19 10:28:37.000000 yeref-0.1.63/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-19 10:28:48.614916 yeref-0.1.63/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.63/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   511251 2023-05-09 14:24:53.000000 yeref-0.1.63/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   204234 2023-05-19 10:27:02.000000 yeref-0.1.63/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-19 10:28:48.621580 yeref-0.1.63/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-19 10:28:48.000000 yeref-0.1.63/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-19 10:28:48.000000 yeref-0.1.63/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-19 10:28:48.000000 yeref-0.1.63/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-19 10:28:48.000000 yeref-0.1.63/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.62/setup.py` & `yeref-0.1.63/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.62',
+      version='0.1.63',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,15 +39,15 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.62-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.63-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.62/yeref/l_.py` & `yeref-0.1.63/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.62/yeref/yeref.py` & `yeref-0.1.63/yeref/yeref.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,18 @@
 🇬🇧🇨🇳🇦🇪🇪🇸🇷🇸🇫🇷
 """
 
 markupAdmin = types.ReplyKeyboardMarkup(keyboard=[
     [types.KeyboardButton(text='⬅️ Prev'), types.KeyboardButton(text='↩️ Menu'),
      types.KeyboardButton(text='➡️️ Next')]], resize_keyboard=True, selective=True, row_width=3)
 
-
+BOT_VARS_ = '{"DATE_TIME": 0, "BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": 0}'
+BOT_LSTS_ = '{"ADMIN_USERS": [], "PREMIUM_USERS": [], "CHANNEL_USERS": [], "GROUP_USERS": [], "PROMO_USERS": [], "UTM_USERS": []}'
+USER_VARS_ = '{"USER_TEXT": "", "USER_PHONE": "", "USER_GEO": "", "USER_PROMO": "", "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "USER_UTM": "", "USER_ID": 0, "USER_TZ": 0, "USER_LZ": "", "USER_DT": "", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "DATE_TIME": 0}'
+USER_LSTS_ = '{"USER_UTMREF": []}'
 # endregion
 
 
 # region db
 def sqlite_lower(value_):
     return value_.lower() if value_ else None
 
@@ -210,14 +213,106 @@
         except Exception as e:
             await log(e)
             await asyncio.sleep(round(random.uniform(1, 2), 2))
             retry -= 1
     return 0
 
 
+async def db_bot_create(db):
+    con = sqlite3.connect(db, timeout=10)
+    try:
+        cur = con.cursor()
+
+        # USER
+        cur.execute(f'''CREATE TABLE IF NOT EXISTS USER ( 
+            USER_ID         INTEGER     PRIMARY KEY AUTOINCREMENT
+                                        UNIQUE
+                                        NOT NULL,
+            USER_TID        BIGINT      UNIQUE
+                                        NOT NULL,
+            USER_USERNAME   VARCHAR,
+            USER_FULLNAME   VARCHAR,
+
+            USER_VARS       VARCHAR     DEFAULT '{USER_VARS_}',
+            USER_LSTS       VARCHAR     DEFAULT '{USER_LSTS_}'
+        )''')
+
+        # USERBAN
+        cur.execute('''CREATE TABLE IF NOT EXISTS USERBAN ( 
+            USERBAN_ID          INTEGER     PRIMARY KEY AUTOINCREMENT
+                                            UNIQUE
+                                            NOT NULL,
+            USERBAN_TID         BIGINT      UNIQUE,
+            USERBAN_USERNAME    VARCHAR     UNIQUE,
+            USERBAN_FULLNAME    VARCHAR,
+            USERBAN_BAN         VARCHAR, 
+            USERBAN_DT          VARCHAR
+        )''')
+
+        # TRG
+        cur.execute('''CREATE TABLE IF NOT EXISTS TRG ( 
+            TRG_ID          INTEGER     PRIMARY KEY AUTOINCREMENT
+                                        UNIQUE
+                                        NOT NULL,
+            TRG_VID         VARCHAR     UNIQUE NOT NULL,
+            TRG_TYPE        VARCHAR,
+            TRG_CONTENT     VARCHAR,
+
+            TRG_RIGHTID     VARCHAR,
+            TRG_RIGHTTYPE   VARCHAR,
+            TRG_LEFTID      VARCHAR,
+            TRG_LEFTTYPE    VARCHAR,
+            TRG_USERS       VARCHAR
+        )''')
+
+        # ACT
+        cur.execute('''CREATE TABLE IF NOT EXISTS ACT ( 
+            ACT_ID          INTEGER     PRIMARY KEY AUTOINCREMENT
+                                        UNIQUE
+                                        NOT NULL,
+            ACT_VID         VARCHAR     UNIQUE NOT NULL,
+            ACT_TYPE        VARCHAR,
+            ACT_CONTENT     VARCHAR,
+
+            ACT_NEXTID      VARCHAR,
+            ACT_NEXTTYPE    VARCHAR,
+            ACT_USERS       VARCHAR
+        )''')
+
+        # MSG
+        cur.execute('''CREATE TABLE IF NOT EXISTS MSG ( 
+            MSG_ID          INTEGER     PRIMARY KEY AUTOINCREMENT
+                                        UNIQUE
+                                        NOT NULL,
+            MSG_VID         VARCHAR     UNIQUE NOT NULL,
+            MSG_TYPE        VARCHAR,
+            MSG_TEXT        VARCHAR,
+            MSG_MEDIA       VARCHAR,
+            MSG_BUTTONS     VARCHAR,
+            MSG_CHKBOX      VARCHAR,
+            MSG_TEXTF       VARCHAR,
+            MSG_BUTTONSF    VARCHAR,
+            MSG_FILENAME    VARCHAR,
+
+            MSG_STATUS      VARCHAR,
+            MSG_LZ          VARCHAR,
+            MSG_DT          VARCHAR,
+
+            MSG_NEXTID      VARCHAR,
+            MSG_NEXTTYPE    VARCHAR,
+            MSG_USERS       VARCHAR
+        )''')
+
+        con.commit()
+        cur.close()
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+    finally:
+        con.close()
 # endregion
 
 
 # region menu
 async def post_offer(bot, data, BASE_D):
     try:
         for item in data:
```

