# Comparing `tmp/ezcord-0.1.5.tar.gz` & `tmp/ezcord-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.1.5.tar", last modified: Mon May  8 19:19:30 2023, max compression
+gzip compressed data, was "ezcord-0.2.0.tar", last modified: Thu May 18 20:04:09 2023, max compression
```

## Comparing `ezcord-0.1.5.tar` & `ezcord-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.608173 ezcord-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 19:19:18.000000 ezcord-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-08 19:19:30.608173 ezcord-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-08 19:19:18.000000 ezcord-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 19:19:18.000000 ezcord-0.1.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.604173 ezcord-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 19:19:18.000000 ezcord-0.1.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-08 19:19:18.000000 ezcord-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 19:19:18.000000 ezcord-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:19:30.608173 ezcord-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.604173 ezcord-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.604173 ezcord-0.1.5/src/ezcord/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.608173 ezcord-0.1.5/src/ezcord/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/embed_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/funcutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/ready_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/internal/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-08 19:19:18.000000 ezcord-0.1.5/src/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:19:30.604173 ezcord-0.1.5/src/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-08 19:19:30.000000 ezcord-0.1.5/src/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-08 19:19:30.000000 ezcord-0.1.5/src/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:19:30.000000 ezcord-0.1.5/src/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 19:19:30.000000 ezcord-0.1.5/src/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 19:19:30.000000 ezcord-0.1.5/src/ezcord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:04:09.130916 ezcord-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 20:03:54.000000 ezcord-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-18 20:04:09.130916 ezcord-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-18 20:03:54.000000 ezcord-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 20:03:54.000000 ezcord-0.2.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:04:09.126916 ezcord-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 20:03:54.000000 ezcord-0.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-18 20:03:54.000000 ezcord-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 20:03:54.000000 ezcord-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 20:04:09.130916 ezcord-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:04:09.126916 ezcord-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:04:09.126916 ezcord-0.2.0/src/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:04:09.130916 ezcord-0.2.0/src/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/internal/embed_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/internal/funcutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:04:09.130916 ezcord-0.2.0/src/ezcord/internal/language/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/internal/language/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/internal/ready_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-18 20:03:54.000000 ezcord-0.2.0/src/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:04:09.130916 ezcord-0.2.0/src/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-18 20:04:09.000000 ezcord-0.2.0/src/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-18 20:04:09.000000 ezcord-0.2.0/src/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 20:04:09.000000 ezcord-0.2.0/src/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 20:04:09.000000 ezcord-0.2.0/src/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 20:04:09.000000 ezcord-0.2.0/src/ezcord.egg-info/top_level.txt
```

### Comparing `ezcord-0.1.5/LICENSE` & `ezcord-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.5/PKG-INFO` & `ezcord-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.1.5
+Version: 0.2.0
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.1.5/README.md` & `ezcord-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.5/pyproject.toml` & `ezcord-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.5/src/ezcord/bot.py` & `ezcord-0.2.0/src/ezcord/bot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 from __future__ import annotations
 
 import logging
 import os
 import traceback
 import warnings
 from pathlib import Path
-from typing import Any, Literal
+from typing import Any
 
 import aiohttp
 import discord
-from discord.ext import commands
+from discord.ext import bridge, commands
 
 from .emb import error as error_emb
 from .enums import ReadyEvent
-from .internal import print_ready, set_lang, t
 from .logs import DEFAULT_LOG, custom_log, set_log
 from .times import dc_timestamp
 
+from .internal import (  # isort: skip
+    READY_TITLE,
+    load_lang,
+    print_custom_ready,
+    print_ready,
+    set_lang,
+    t,
+)
+
 
 class Bot(discord.Bot):
     """The EzCord bot class. This is a subclass of :class:`discord.Bot`.
 
     .. hint::
 
         As this class extends from :class:`discord.Bot`, only slash commands are supported.
         If you want to use prefix commands, use :class:`PrefixBot` instead.
 
     Parameters
     ----------
     intents:
         The intents to use for the bot. Defaults to :meth:`discord.Intents.default()`.
     debug:
-        Enable debug logs. Defaults to ``True``.
+        Enable log messages. Defaults to ``True``.
     error_handler:
         Enable the error handler. Defaults to ``True``.
     error_webhook_url:
         The webhook URL to send error messages to. Defaults to ``None``.
 
         .. note::
             You need to enable the error handler for the webhook to work.
     ignored_errors:
         A list of error types to ignore. Defaults to ``None``.
     full_error_traceback:
         Whether to send the full error traceback. If this is ``False``,
         only the most recent traceback will be sent. Defaults to ``False``.
     language:
-        The language to use for the bot. Defaults to ``en``.
+        The language to use for user output.
+
+        The default languages are ``en`` and ``de``. If you add your own language file as
+        described in :doc:`the language example </examples/languages>`, you can use that language as well.
     ready_event:
         The style for :meth:`on_ready_event`. Defaults to :attr:`.ReadyEvent.default`.
         If this is ``None``, the event will be disabled.
     **kwargs:
         Additional keyword arguments for :class:`discord.Bot`.
     """
 
@@ -58,99 +69,140 @@
         intents: discord.Intents = discord.Intents.default(),
         *,
         debug: bool = True,
         error_handler: bool = True,
         error_webhook_url: str | None = None,
         ignored_errors: list[Any] | None = None,
         full_error_traceback: bool = False,
-        language: Literal["en", "de"] = "en",
+        language: str = "en",
         ready_event: ReadyEvent | None = ReadyEvent.default,
         **kwargs,
     ):
         super().__init__(intents=intents, **kwargs)
 
+        if error_handler and error_webhook_url:
+            os.environ.setdefault("ERROR_WEBHOOK_URL", error_webhook_url)
+
         if debug:
             self.logger = set_log(DEFAULT_LOG)
         else:
             self.logger = logging.getLogger(DEFAULT_LOG)
             self.logger.addHandler(logging.NullHandler())
 
         self.error_webhook_url = error_webhook_url
         self.ignored_errors = ignored_errors or []
         self.full_error_traceback = full_error_traceback
-        set_lang(language)
+        load_lang(language)
+        set_lang(language) if language != {} else set_lang("en")
 
         if error_handler:
             self.add_listener(self._error_event, "on_application_command_error")
         elif error_webhook_url:
             warnings.warn("You need to enable the error handler for the webhook to work.")
 
         self.ready_event = ready_event
         if ready_event:
-            self.add_listener(self.on_ready_event, "on_ready")
+            self.add_listener(self._ready_event, "on_ready")
+
+    def _cog_log(self, name: str, custom_logs: bool | str):
+        """Sends a log message for a loaded cog."""
+        if custom_logs:
+            custom_log("COG", f"Loaded {name}", color=custom_logs, level=logging.INFO)
+        else:
+            self.logger.info(f"Loaded {name}")
 
     def load_cogs(
         self,
         *directories: str,
         subdirectories: bool = False,
         ignored_cogs: list[str] | None = None,
+        log: bool = True,
         custom_logs: bool | str = True,
+        log_directories: bool = False,
     ):
         """Load all cogs in the given directories.
 
         Parameters
         ----------
         *directories:
             Names of the directories to load cogs from.
             Defaults to ``"cogs"``.
         subdirectories:
             Whether to load cogs from subdirectories.
             Defaults to ``False``.
         ignored_cogs:
             A list of cogs to ignore. Defaults to ``None``.
+        log:
+            Whether to log the loaded cogs. Defaults to ``True``.
         custom_logs:
             Whether to use a custom log format for cogs. Defaults to ``True``.
             You can also pass in a custom color.
+        log_directories:
+            Whether to include the directory name in log messages. Defaults to ``False``.
         """
         ignored_cogs = ignored_cogs or []
         if not directories:
             directories = ("cogs",)
 
         for directory in directories:
             path = Path(directory)
 
             for filename in os.listdir(directory):
                 name = filename[:-3]
                 if filename.endswith(".py") and name not in ignored_cogs:
                     self.load_extension(f"{'.'.join(path.parts)}.{name}")
-                    if custom_logs:
-                        custom_log("COG", f"Loaded {name}", color=custom_logs, level=logging.DEBUG)
-                    else:
-                        self.logger.debug(f"Loaded {name}")
+                    if not log:
+                        continue
+                    self._cog_log(f"{name}", custom_logs)
 
             if subdirectories:
                 for element in os.scandir(directory):
                     if not element.is_dir():
                         continue
 
                     for sub_file in os.scandir(element.path):
                         name = sub_file.name[:-3]
                         if sub_file.name.endswith(".py") and name not in ignored_cogs:
                             self.load_extension(f"{'.'.join(path.parts)}.{element.name}.{name}")
-                            if custom_logs:
-                                custom_log(
-                                    "COG",
-                                    f"Loaded {element.name}.{name}",
-                                    color=custom_logs,
-                                    level=logging.DEBUG,
-                                )
-                            else:
-                                self.logger.debug(f"Loaded {element.name}.{name}")
+                            dirname = f"{element.name}." if log_directories else ""
+                            if not log:
+                                continue
+                            self._cog_log(f"{dirname}{name}", custom_logs)
 
-    async def on_ready_event(self):
+    def ready(
+        self,
+        *,
+        title: str = READY_TITLE,
+        style: ReadyEvent = ReadyEvent.default,
+        default_info: bool = True,
+        new_info: dict | None = None,
+        colors: list[str] | None = None,
+    ):
+        """Print a custom ready message.
+
+        Parameters
+        ----------
+        title:
+            The title of the ready message.
+        style:
+            The style of the ready message. Defaults to :attr:`.ReadyEvent.default`.
+        default_info:
+            Whether to include the default information. Defaults to ``True``.
+        new_info:
+            A dictionary of information to include in the ready message.
+            Defaults to ``None``.
+        colors:
+            A list of colors to use for the ready message. If no colors are given,
+            default colors will be used.
+
+            Colors can only be used with :attr:`.ReadyEvent.box_colorful` and all table styles.
+        """
+        print_custom_ready(self, title, style, default_info, new_info, colors)
+
+    async def _ready_event(self):
         """Prints the bot's information when it's ready."""
         print_ready(self, self.ready_event)
 
     async def _error_event(self, ctx: discord.ApplicationContext, error: discord.DiscordException):
         """The event that handles application command errors."""
         if type(error) in self.ignored_errors:
             return
@@ -169,65 +221,94 @@
             if "original" in error.__dict__ and not self.full_error_traceback:
                 original_error = error.__dict__["original"]
                 error_msg = f"{original_error.__class__.__name__}: {error.__cause__}"
                 error = original_error
             else:
                 error_msg = f"{error}"
 
-            error_txt = f"{t('error')}: ```{error_msg}```"
+            error_txt = f"{t('error', f'```{error_msg}```')}"
             try:
                 await error_emb(ctx, error_txt, title="Error")
             except discord.HTTPException:
                 pass
 
             webhook_sent = False
             if self.error_webhook_url:
-                async with aiohttp.ClientSession() as session:
-                    webhook = discord.Webhook.from_url(
-                        self.error_webhook_url, session=session, bot_token=self.http.token
-                    )
-                    error_txt = "".join(
-                        traceback.format_exception(type(error), error, error.__traceback__)
-                    )
-                    guild_txt = (
-                        f"\n- **Guild:** {ctx.guild.name} - `{ctx.guild.id}`" if ctx.guild else ""
-                    )
-                    user_txt = (
-                        f"\n- **User:** {ctx.author} - `{ctx.author.id}`" if ctx.author else ""
-                    )
-
-                    embed = discord.Embed(
-                        title="Error Report",
-                        description=f"- **Command:** /{ctx.command.qualified_name}"
-                        f"{guild_txt}{user_txt}"
-                        f"\n```py\n{error_txt[:3500]}```",
-                        color=discord.Color.red(),
-                    )
-                    try:
-                        await webhook.send(
-                            embed=embed,
-                            username=f"{self.user.name} Error Report",
-                            avatar_url=self.user.display_avatar.url,
-                        )
-                    except discord.HTTPException:
-                        self.logger.error(
-                            "Error while sending error report to webhook. "
-                            "Please check if the URL is correct."
-                        )
-                    else:
-                        webhook_sent = True
+                description = self.get_error_text(ctx, error)
+                webhook_sent = await self._send_error_webhook(description)
 
             self.logger.exception(
                 f"Error while executing **/{ctx.command.qualified_name}** ```{error_msg}```",
                 exc_info=error,
                 extra={"webhook_sent": webhook_sent},
             )
 
+    @staticmethod
+    def get_error_text(
+        ctx: discord.ApplicationContext | discord.Interaction,
+        error: Exception,
+        item: discord.ui.Item | discord.ui.Modal | None = None,
+    ):
+        if item:
+            if isinstance(item, discord.ui.Button) and item.label:
+                location = f"- **Button:** {item.label}"
+            elif ctx.type == discord.InteractionType.modal_submit:
+                location = f"- **Modal:** {type(item).__name__}"
+            else:
+                location = f"- **Select Menu:** {type(item.view).__name__}"
+        else:
+            location = f"- **Command:** /{ctx.command.qualified_name}"
+
+        error_txt = "".join(traceback.format_exception(type(error), error, error.__traceback__))
+        guild_txt = f"\n- **Guild:** {ctx.guild.name} - `{ctx.guild.id}`" if ctx.guild else ""
+        user_txt = f"\n- **User:** {ctx.user} - `{ctx.user.id}`" if ctx.user else ""
+
+        description = location + guild_txt + user_txt + f"\n```py\n{error_txt[:3500]}```"
+        return description
+
+    async def _send_error_webhook(self, description):
+        webhook_sent = False
+        async with aiohttp.ClientSession() as session:
+            webhook = discord.Webhook.from_url(
+                self.error_webhook_url, session=session, bot_token=self.http.token
+            )
+
+            embed = discord.Embed(
+                title="Error Report",
+                description=description,
+                color=discord.Color.red(),
+            )
+            try:
+                await webhook.send(
+                    embed=embed,
+                    username=f"{self.user.name} Error Report",
+                    avatar_url=self.user.display_avatar.url,
+                )
+            except discord.HTTPException:
+                self.logger.error(
+                    "Error while sending error report to webhook. "
+                    "Please check if the URL is correct."
+                )
+            else:
+                webhook_sent = True
+
+        return webhook_sent
+
 
 class PrefixBot(Bot, commands.Bot):
     """A subclass of :class:`discord.ext.commands.Bot` that implements the :class:`Bot` class.
 
     This class can be used if you want to use EzCord with prefix commands.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+
+
+class BridgeBot(Bot, bridge.Bot):
+    """A subclass of :class:`discord.ext.bridge.Bot` that implements the :class:`Bot` class.
+
+    This class can be used if you want to use EzCord with bridge commands.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
```

### Comparing `ezcord-0.1.5/src/ezcord/emb.py` & `ezcord-0.2.0/src/ezcord/emb.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.5/src/ezcord/enums.py` & `ezcord-0.2.0/src/ezcord/enums.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,17 +22,18 @@
         return self.value
 
 
 class ReadyEvent(Enum):
     """Styles for the ready event."""
 
     box = 0
-    box_bold = 1
-    logs = 2
-    table = 3
-    table_bold = 4
-    table_vertical = 5
-    table_vertical_bold = 6
+    box_colorful = 1
+    box_bold = 2
+    logs = 3
+    table = 4
+    table_bold = 5
+    table_vertical = 6
+    table_vertical_bold = 7
     default = table
 
     def __str__(self):
         return self.name
```

### Comparing `ezcord-0.1.5/src/ezcord/internal/colors.py` & `ezcord-0.2.0/src/ezcord/internal/colors.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     if color_string.startswith("\x1b["):
         return color_string
 
     try:
         return getattr(Fore, color_string.upper())
     except AttributeError:
         raise ValueError(
-            f"{color_string} is not a valid color string. Use either the colorama library or a string like 'red'."
+            f"'{color_string}' is not a valid color string. Use either the colorama library or a string like 'red'."
         )
 
 
 def replace_second(string: str, substring: str, color: str) -> str:
     """Replaces custom formatters with ansi colors.
 
     Example
@@ -51,10 +51,11 @@
 
 def replace_dc_format(string: str, color: str | None = None) -> str:
     """Replaces Discord markdown with ansi colors."""
     if color is None:
         color = DEFAULT_COLOR
     color = get_escape_code(color)
 
+    string = replace_second(string, "***", color)  # color text that contains multiple other colors
     string = replace_second(string, "**", color)
     string = re.sub("```.*?```", "", string)  # remove codeblocks
     return string
```

### Comparing `ezcord-0.1.5/src/ezcord/internal/embed_templates.py` & `ezcord-0.2.0/src/ezcord/internal/embed_templates.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.5/src/ezcord/internal/ready_style.py` & `ezcord-0.2.0/src/ezcord/internal/ready_style.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Utility functions for the ready event."""
 
+from itertools import cycle, islice
+
 import discord
 from colorama import Fore
 
+from .. import __version__
 from ..enums import ReadyEvent
 from ..logs import log
+from .colors import get_escape_code
 
 
 class Style:
     TL = "╭"  # top left
     TR = "╮"  # top right
     BL = "╰"  # bottom left
     BR = "╯"  # bottom right
@@ -21,78 +25,136 @@
     B = "┴"  # bottom
 
 
 class Bold(Style):
     TL, TR, BL, BR, H, V, M, L, R, T, B = "╔", "╗", "╚", "╝", "═", "║", "╬", "╠", "╣", "╦", "╩"
 
 
-COLORS = [Fore.CYAN, Fore.MAGENTA, Fore.YELLOW, Fore.GREEN, Fore.BLUE, Fore.RED]
+READY_TITLE: str = f"Bot is online with EzCord {__version__}"
+DEFAULT_COLORS: list[str] = [Fore.CYAN, Fore.MAGENTA, Fore.YELLOW, Fore.GREEN, Fore.BLUE, Fore.RED]
 
 
-def print_ready(bot: discord.Bot, style: ReadyEvent):
+def get_default_info(bot: discord.Bot):
     cmds = [
         cmd for cmd in bot.walk_application_commands() if type(cmd) != discord.SlashCommandGroup
     ]
 
     infos = {
         "Bot": f"{bot.user}",
         "ID": f"{bot.user.id}",
         "Pycord": discord.__version__,
         "Commands": f"{len(cmds):,}",
         "Guilds": f"{len(bot.guilds):,}",
         "Latency": f"{round(bot.latency * 1000):,}ms",
     }
 
-    txt = f"Bot is online!"
+    return infos
+
+
+def print_custom_ready(
+    bot: discord.Bot,
+    title: str,
+    style: ReadyEvent = ReadyEvent.default,
+    default_info: bool = True,
+    new_info: dict | None = None,
+    colors: list[str] | None = None,
+):
+    infos = get_default_info(bot) if default_info else {}
+    colors = list(map(get_escape_code, colors or DEFAULT_COLORS))
+
+    if new_info:
+        for key, value in new_info.items():
+            infos[key] = value
+
+    print_ready(bot, style, infos, title, colors)
+
+
+def print_ready(
+    bot: discord.Bot,
+    style: ReadyEvent,
+    infos: dict[str, str] | None = None,
+    title: str = READY_TITLE,
+    colors: list[str] | None = None,
+):
+    infos = infos or get_default_info(bot)
+    colors = colors or DEFAULT_COLORS
+
+    info_count = len(infos.items())
+    colors = list(islice(cycle(colors), info_count))
+
     colon_infos = {key + ":": value for key, value in infos.items()}
 
     style_cls = Style()
     if "bold" in style.name:
         style_cls = Bold()
 
-    if style == ReadyEvent.box or style == ReadyEvent.box_bold:
-        txt += box(colon_infos, style_cls)
+    txt = title
+    if style in [ReadyEvent.box, ReadyEvent.box_bold, ReadyEvent.box_colorful]:
+        txt += box(colon_infos, colors, style, style_cls)
         log.info(txt)
     elif style == ReadyEvent.logs:
         log.info(txt)
         logs(colon_infos)
     else:
         color_table = {
-            key: COLORS[i] + value + Fore.RESET for i, (key, value) in enumerate(infos.items())
+            key: colors[i] + value + Fore.RESET for i, (key, value) in enumerate(infos.items())
         }
         if style == ReadyEvent.table or style == ReadyEvent.table_bold:
             info_list = [list(infos.keys()), list(infos.values())]
             color_list = [list(color_table.keys()), list(color_table.values())]
         else:
             info_list = [list(item) for item in infos.items()]
             color_list = [list(item) for item in color_table.items()]
 
         txt += f"\n{Fore.RESET}" + tables(info_list, color_list, style_cls)
         log.info(txt)
 
 
-def box(infos: dict[str, str], s: Style = Style()):
+def box(infos: dict[str, str], colors: list[str], box_style: ReadyEvent, s: Style = Style()):
     longest = max([str(i) for i in infos.values()], key=len)
     formatter = f"<{len(longest)}"
     longest_key = max([len(i) for i in infos.keys()]) + 1
 
-    txt = f"\n{s.TL}{(len(longest) + 2 + longest_key) * s.H}{s.TR}\n"
-    for key, info in infos.items():
+    if box_style == ReadyEvent.box_colorful:
+        txt = f"\n{Fore.RESET}"
+    else:
+        txt = "\n"
+
+    txt += f"{s.TL}{(len(longest) + 2 + longest_key) * s.H}{s.TR}\n"
+    for index, (key, info) in enumerate(infos.items()):
         key = f"{key:<{longest_key}}"
-        txt += f"{s.V} {key}{info:{formatter}} {s.V}\n"
+        if box_style == ReadyEvent.box_colorful:
+            txt += f"{s.V} {key}{colors[index]}{info:{formatter}}{Fore.RESET} {s.V}\n"
+        else:
+            txt += f"{s.V} {key}{info:{formatter}} {s.V}\n"
     txt += f"{s.BL}{(len(longest) + 2 + longest_key) * s.H}{s.BR}"
     return txt
 
 
 def logs(infos: dict[str, str]):
     for key, info in infos.items():
         log.info(f"{key} **{info}**")
 
 
-def tables(rows: list[list[str]], color_rows: list[list[str]], s: Style = Style()):
+def tables(rows: list[list[str]], color_rows: list[list[str]] | None = None, s: Style = Style()):
+    """Create a table from a list of rows.
+
+    Parameters
+    ----------
+    rows:
+        The rows of the table. This is used to calculate the length of each column.
+    color_rows:
+        The rows of the table with color. This is used as the actual content of the table.
+        If this is None, the content of the table will be taken from ``rows``.
+    s:
+        The style of the table.
+    """
+    if color_rows is None:
+        color_rows = rows
+
     length = [max([len(value) for value in column]) for column in zip(*rows)]
     table = ""
     for index, (row, color_row) in enumerate(zip(rows, color_rows)):
         table += s.V
 
         middle_row = ""
         for max_length, content, color_content in zip(length, row, color_row):
```

### Comparing `ezcord-0.1.5/src/ezcord/internal/translation.py` & `ezcord-0.2.0/src/ezcord/internal/translation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Internal language utilities for the library."""
 
 import inspect
 import os
 from configparser import ConfigParser
 from functools import cache
 from pathlib import Path
-from typing import Literal
 
-from .languages import *
+from ..logs import log
+from .language.languages import load_lang
 
 
 def plural_de(amount: int, word: str, relative: bool = True) -> str:
     """Pluralize a given word (German).
 
     Parameters
     ----------
@@ -99,31 +99,34 @@
 
     while origin_file == Path(__file__).stem:
         n += 1
         origin_file = Path(inspect.stack()[n].filename).stem
 
     lang = get_lang()
 
-    if lang == "de":
-        return de[origin_file][key].format(*args)
-    else:
-        return en[origin_file][key].format(*args)
+    try:
+        return load_lang(lang)[origin_file][key].format(*args)
+    except KeyError:
+        # fallback to english if the key is not in the custom language file
+        # provided by the user
+        log.warn(f"Key '{key}' not found in language file '{lang}'. Falling back to 'en'.")
+        return load_lang("en")[origin_file][key].format(*args)
 
 
 @cache
 def get_lang():
     """Get the language from the config file."""
     parent = Path(__file__).parent.absolute()
     config = ConfigParser()
     config.read(os.path.join(parent, "config.ini"))
 
     return config["DEFAULT"]["lang"]
 
 
-def set_lang(lang: Literal["en", "de"]):
+def set_lang(lang: str):
     """Set the language in the config file.
 
     Parameters
     ----------
     lang:
         The language to set.
     """
```

### Comparing `ezcord-0.1.5/src/ezcord/logs.py` & `ezcord-0.2.0/src/ezcord/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         new_record = logging.makeLogRecord(record.__dict__)
 
         # color new lines
         if isinstance(log_format, str) and log_format.endswith("//"):
             log_format = log_format.replace("//", "")
             split = new_record.msg.split("\n", 1)
             if len(split) > 1:
-                new_record.msg = split[0] + "\n**" + split[1] + "**"
+                new_record.msg = split[0] + "\n***" + split[1] + "***"
 
         new_record.msg = replace_dc_format(new_record.msg, current_level_color)
 
         formatter = logging.Formatter(log_format, self.TIME_FORMAT)
         return formatter.format(new_record)
 
 
@@ -214,15 +214,15 @@
     if "webhook_sent" in record.__dict__:
         return not record.__dict__["webhook_sent"]
     return True
 
 
 def set_log(
     name: str = DEFAULT_LOG,
-    log_level: int = logging.DEBUG,
+    log_level: int = logging.INFO,
     *,
     file: bool = False,
     log_format: str | LogFormat = LogFormat.default,
     time_format: str = "%Y-%m-%d %H:%M:%S",
     discord_log_level: int = logging.WARNING,
     webhook_url: str | None = None,
     dc_codeblocks: bool = True,
@@ -231,15 +231,15 @@
     """Creates a logger. If this logger already exists, it will return the existing logger.
 
     Parameters
     ----------
     name:
         The name of the logger.
     log_level:
-        The log level for default log messages ``logging.DEBUG``.
+        The log level for default log messages ``logging.INFO``.
     file:
         Whether to log to a file. Defaults to ``False``.
     log_format:
         The log format. Defaults to :attr:`.LogFormat.default`.
     time_format:
         The time format. Defaults to ``%Y-%m-%d %H:%M:%S``.
     discord_log_level:
@@ -271,17 +271,17 @@
             ezcord.set_log(colors=colors)
 
     Returns
     -------
     :class:`logging.Logger`
     """
     logger = logging.getLogger(name)
-    logger.setLevel(log_level)
     if logger.handlers:
         return logger
+    logger.setLevel(log_level)
 
     handler: logging.FileHandler | logging.StreamHandler
     if file:
         if not os.path.exists("logs"):
             os.mkdir("logs")
         filename = name.split(".")[-1]
         handler = logging.FileHandler(f"logs/{filename}.log", mode="w", encoding="utf-8")
```

### Comparing `ezcord-0.1.5/src/ezcord/times.py` & `ezcord-0.2.0/src/ezcord/times.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.5/src/ezcord/utils.py` & `ezcord-0.2.0/src/ezcord/utils.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.5/src/ezcord.egg-info/PKG-INFO` & `ezcord-0.2.0/src/ezcord.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.1.5
+Version: 0.2.0
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.1.5/src/ezcord.egg-info/SOURCES.txt` & `ezcord-0.2.0/src/ezcord.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 src/ezcord.egg-info/dependency_links.txt
 src/ezcord.egg-info/requires.txt
 src/ezcord.egg-info/top_level.txt
 src/ezcord/internal/__init__.py
 src/ezcord/internal/colors.py
 src/ezcord/internal/embed_templates.py
 src/ezcord/internal/funcutils.py
-src/ezcord/internal/languages.py
 src/ezcord/internal/ready_style.py
-src/ezcord/internal/translation.py
+src/ezcord/internal/translation.py
+src/ezcord/internal/language/languages.py
```

