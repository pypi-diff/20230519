# Comparing `tmp/emmett-2.5.1.tar.gz` & `tmp/emmett-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett-2.5.1.tar", max compression
+gzip compressed data, was "emmett-2.5.2.tar", max compression
```

## Comparing `emmett-2.5.1.tar` & `emmett-2.5.2.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0    14193 2023-05-09 15:13:20.483174 emmett-2.5.1/CHANGES.md
--rw-r--r--   0        0        0     2074 2023-05-09 15:13:20.483174 emmett-2.5.1/LICENSE
--rw-r--r--   0        0        0     2922 2023-05-09 15:13:20.483174 emmett-2.5.1/README.md
--rw-r--r--   0        0        0     9917 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/app_and_modules.md
--rw-r--r--   0        0        0    15873 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/auth.md
--rw-r--r--   0        0        0    12150 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/caching.md
--rw-r--r--   0        0        0     2613 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/cli.md
--rw-r--r--   0        0        0     4481 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/debug_and_logging.md
--rw-r--r--   0        0        0     3056 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/deployment.md
--rw-r--r--   0        0        0     5295 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/extensions.md
--rw-r--r--   0        0        0     5174 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/foreword.md
--rw-r--r--   0        0        0     6493 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/forms.md
--rw-r--r--   0        0        0     2105 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/installation.md
--rw-r--r--   0        0        0     3596 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/languages.md
--rw-r--r--   0        0        0     3087 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/mailer.md
--rw-r--r--   0        0        0     9672 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/orm/advanced.md
--rw-r--r--   0        0        0    12917 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/orm/callbacks.md
--rw-r--r--   0        0        0     7060 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/orm/connecting.md
--rw-r--r--   0        0        0    20808 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/orm/migrations.md
--rw-r--r--   0        0        0    14034 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/orm/models.md
--rw-r--r--   0        0        0    29245 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/orm/operations.md
--rw-r--r--   0        0        0    27472 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/orm/relations.md
--rw-r--r--   0        0        0     5523 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/orm/scopes.md
--rw-r--r--   0        0        0     6732 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/orm/virtuals.md
--rw-r--r--   0        0        0     3172 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/orm.md
--rw-r--r--   0        0        0     4100 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/patterns.md
--rw-r--r--   0        0        0    14161 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/pipeline.md
--rw-r--r--   0        0        0    15916 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/quickstart.md
--rw-r--r--   0        0        0     6082 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/request.md
--rw-r--r--   0        0        0     3378 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/response.md
--rw-r--r--   0        0        0    11727 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/routing.md
--rw-r--r--   0        0        0     2424 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/services.md
--rw-r--r--   0        0        0     4535 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/sessions.md
--rw-r--r--   0        0        0     6405 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/templates.md
--rw-r--r--   0        0        0     6776 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/testing.md
--rw-r--r--   0        0        0      440 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/tree.yml
--rw-r--r--   0        0        0    14840 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/tutorial.md
--rw-r--r--   0        0        0    16597 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/upgrading.md
--rw-r--r--   0        0        0    15878 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/validations.md
--rw-r--r--   0        0        0     2307 2023-05-09 15:13:20.491174 emmett-2.5.1/docs/websocket.md
--rw-r--r--   0        0        0      386 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/__init__.py
--rw-r--r--   0        0        0      248 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/__main__.py
--rw-r--r--   0        0        0       22 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/__version__.py
--rw-r--r--   0        0        0    11242 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/_internal.py
--rw-r--r--   0        0        0     5633 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/_reloader.py
--rw-r--r--   0        0        0      771 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/_shortcuts.py
--rw-r--r--   0        0        0    27001 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/app.py
--rw-r--r--   0        0        0        0 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/asgi/__init__.py
--rw-r--r--   0        0        0    15183 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/asgi/handlers.py
--rw-r--r--   0        0        0      220 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/asgi/helpers.py
--rw-r--r--   0        0        0      533 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/asgi/typing.py
--rw-r--r--   0        0        0     3064 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/asgi/workers.py
--rw-r--r--   0        0        0     8029 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/asgi/wrappers.py
--rw-r--r--   0        0        0        0 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/debug/__init__.py
--rw-r--r--   0        0        0     2437 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/debug/shBrushPython.js
--rw-r--r--   0        0        0     6204 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/debug/shCore.css
--rw-r--r--   0        0        0    16175 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/debug/shCore.js
--rw-r--r--   0        0        0     2499 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/debug/shTheme.css
--rw-r--r--   0        0        0      647 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/debug/view.css
--rw-r--r--   0        0        0     4626 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/debug/view.html
--rw-r--r--   0        0        0     1630 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/helpers.js
--rw-r--r--   0        0        0    89476 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/jquery.min.js
--rw-r--r--   0        0        0   137986 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/assets/jquery.min.map
--rw-r--r--   0        0        0    18871 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/cache.py
--rw-r--r--   0        0        0    15186 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/cli.py
--rw-r--r--   0        0        0     2547 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/ctx.py
--rw-r--r--   0        0        0     8165 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/datastructures.py
--rw-r--r--   0        0        0     5076 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/debug.py
--rw-r--r--   0        0        0     3201 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/extensions.py
--rw-r--r--   0        0        0    25617 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/forms.py
--rw-r--r--   0        0        0     3095 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/helpers.py
--rw-r--r--   0        0        0     6435 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/html.py
--rw-r--r--   0        0        0     8726 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/http.py
--rw-r--r--   0        0        0        0 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/language/__init__.py
--rw-r--r--   0        0        0     1096 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/language/helpers.py
--rw-r--r--   0        0        0      933 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/language/translator.py
--rw-r--r--   0        0        0        0 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/libs/__init__.py
--rw-r--r--   0        0        0    25207 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/libs/contenttype.py
--rw-r--r--   0        0        0     3915 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/libs/portalocker.py
--rw-r--r--   0        0        0      925 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/locals.py
--rw-r--r--   0        0        0     3084 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/logger.py
--rw-r--r--   0        0        0      478 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/__init__.py
--rw-r--r--   0        0        0     2373 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/_patches.py
--rw-r--r--   0        0        0    13015 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/adapters.py
--rw-r--r--   0        0        0     3224 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/apis.py
--rw-r--r--   0        0        0     8857 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/base.py
--rw-r--r--   0        0        0    12058 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/connection.py
--rw-r--r--   0        0        0       80 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/engines/__init__.py
--rw-r--r--   0        0        0     5577 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/engines/postgres.py
--rw-r--r--   0        0        0     1191 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/engines/sqlite.py
--rw-r--r--   0        0        0      605 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/errors.py
--rw-r--r--   0        0        0     1677 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/geo.py
--rw-r--r--   0        0        0    18102 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/helpers.py
--rw-r--r--   0        0        0       62 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/migrations/__init__.py
--rw-r--r--   0        0        0     2892 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/migrations/base.py
--rw-r--r--   0        0        0    15289 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/migrations/commands.py
--rw-r--r--   0        0        0    14381 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/migrations/engine.py
--rw-r--r--   0        0        0     1058 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/migrations/exceptions.py
--rw-r--r--   0        0        0    21829 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/migrations/generation.py
--rw-r--r--   0        0        0     3636 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/migrations/helpers.py
--rw-r--r--   0        0        0      491 2023-05-09 15:13:20.491174 emmett-2.5.1/emmett/orm/migrations/migration.tmpl
--rw-r--r--   0        0        0    23246 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/orm/migrations/operations.py
--rw-r--r--   0        0        0    14902 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/orm/migrations/revisions.py
--rw-r--r--   0        0        0    12034 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/orm/migrations/scripts.py
--rw-r--r--   0        0        0     1150 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/orm/migrations/utils.py
--rw-r--r--   0        0        0    46716 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/orm/models.py
--rw-r--r--   0        0        0    57286 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/orm/objects.py
--rw-r--r--   0        0        0     4208 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/orm/transactions.py
--rw-r--r--   0        0        0      978 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/orm/wrappers.py
--rw-r--r--   0        0        0      917 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/parsers.py
--rw-r--r--   0        0        0    12040 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/pipeline.py
--rw-r--r--   0        0        0        0 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/routing/__init__.py
--rw-r--r--   0        0        0     5303 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/routing/dispatchers.py
--rw-r--r--   0        0        0     4112 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/routing/response.py
--rw-r--r--   0        0        0    11518 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/routing/router.py
--rw-r--r--   0        0        0     8479 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/routing/routes.py
--rw-r--r--   0        0        0     7026 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/routing/rules.py
--rw-r--r--   0        0        0     9704 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/routing/urls.py
--rw-r--r--   0        0        0        0 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/rsgi/__init__.py
--rw-r--r--   0        0        0     9783 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/rsgi/handlers.py
--rw-r--r--   0        0        0      878 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/rsgi/helpers.py
--rw-r--r--   0        0        0     4338 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/rsgi/wrappers.py
--rw-r--r--   0        0        0     5490 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/security.py
--rw-r--r--   0        0        0     2207 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/serializers.py
--rw-r--r--   0        0        0     1003 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/server.py
--rw-r--r--   0        0        0    11649 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/sessions.py
--rw-r--r--   0        0        0        0 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/templating/__init__.py
--rw-r--r--   0        0        0     1843 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/templating/lexers.py
--rw-r--r--   0        0        0     1957 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/templating/templater.py
--rw-r--r--   0        0        0       37 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/testing/__init__.py
--rw-r--r--   0        0        0    11877 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/testing/client.py
--rw-r--r--   0        0        0    10674 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/testing/env.py
--rw-r--r--   0        0        0    12272 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/testing/helpers.py
--rw-r--r--   0        0        0    15936 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/testing/urls.py
--rw-r--r--   0        0        0      125 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/tools/__init__.py
--rw-r--r--   0        0        0       52 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/tools/auth/__init__.py
--rw-r--r--   0        0        0     9035 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/tools/auth/apis.py
--rw-r--r--   0        0        0    19190 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/tools/auth/exposer.py
--rw-r--r--   0        0        0    13469 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/tools/auth/ext.py
--rw-r--r--   0        0        0     5270 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/tools/auth/forms.py
--rw-r--r--   0        0        0     7485 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/tools/auth/models.py
--rw-r--r--   0        0        0     1417 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/tools/decorators.py
--rw-r--r--   0        0        0    10953 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/tools/mailer.py
--rw-r--r--   0        0        0     1565 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/tools/service.py
--rw-r--r--   0        0        0      355 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/typing.py
--rw-r--r--   0        0        0     5357 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/utils.py
--rw-r--r--   0        0        0    11554 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/validators/__init__.py
--rw-r--r--   0        0        0     7636 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/validators/basic.py
--rw-r--r--   0        0        0    31120 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/validators/consist.py
--rw-r--r--   0        0        0    19038 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/validators/helpers.py
--rw-r--r--   0        0        0     7367 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/validators/inside.py
--rw-r--r--   0        0        0     4614 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/validators/process.py
--rw-r--r--   0        0        0     2190 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/wrappers/__init__.py
--rw-r--r--   0        0        0     2886 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/wrappers/helpers.py
--rw-r--r--   0        0        0     3984 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/wrappers/request.py
--rw-r--r--   0        0        0     1525 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/wrappers/response.py
--rw-r--r--   0        0        0     1062 2023-05-09 15:13:20.495175 emmett-2.5.1/emmett/wrappers/websocket.py
--rw-r--r--   0        0        0     2091 2023-05-09 15:13:20.495175 emmett-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     1524 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/helpers.py
--rw-r--r--   0        0        0       46 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/languages/de.json
--rw-r--r--   0        0        0       49 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/languages/it.json
--rw-r--r--   0        0        0       69 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/languages/ru.json
--rw-r--r--   0        0        0      134 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/templates/auth/auth.html
--rw-r--r--   0        0        0      479 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/templates/layout.html
--rw-r--r--   0        0        0      153 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/templates/test.html
--rw-r--r--   0        0        0     8027 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_auth.py
--rw-r--r--   0        0        0     4658 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_cache.py
--rw-r--r--   0        0        0     1415 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_http.py
--rw-r--r--   0        0        0      861 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_logger.py
--rw-r--r--   0        0        0    11854 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_mailer.py
--rw-r--r--   0        0        0     8618 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_migrations.py
--rw-r--r--   0        0        0    33038 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_orm.py
--rw-r--r--   0        0        0      853 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_orm_connections.py
--rw-r--r--   0        0        0    10074 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_orm_gis.py
--rw-r--r--   0        0        0    22722 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_orm_pks.py
--rw-r--r--   0        0        0     9863 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_orm_row.py
--rw-r--r--   0        0        0     2958 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_orm_transactions.py
--rw-r--r--   0        0        0    22478 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_pipeline.py
--rw-r--r--   0        0        0     8659 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_routing.py
--rw-r--r--   0        0        0     1475 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_session.py
--rw-r--r--   0        0        0     2705 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_templates.py
--rw-r--r--   0        0        0      622 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_translator.py
--rw-r--r--   0        0        0     2045 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_utils.py
--rw-r--r--   0        0        0    18633 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_validators.py
--rw-r--r--   0        0        0      822 2023-05-09 15:13:20.499174 emmett-2.5.1/tests/test_wrappers.py
--rw-r--r--   0        0        0     5026 1970-01-01 00:00:00.000000 emmett-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0    14193 2023-05-19 11:27:14.001857 emmett-2.5.2/CHANGES.md
+-rw-r--r--   0        0        0     2074 2023-05-19 11:27:14.001857 emmett-2.5.2/LICENSE
+-rw-r--r--   0        0        0     2922 2023-05-19 11:27:14.001857 emmett-2.5.2/README.md
+-rw-r--r--   0        0        0     9917 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/app_and_modules.md
+-rw-r--r--   0        0        0    15873 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/auth.md
+-rw-r--r--   0        0        0    12150 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/caching.md
+-rw-r--r--   0        0        0     2613 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/cli.md
+-rw-r--r--   0        0        0     4481 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/debug_and_logging.md
+-rw-r--r--   0        0        0     3056 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/deployment.md
+-rw-r--r--   0        0        0     5295 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/extensions.md
+-rw-r--r--   0        0        0     5174 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/foreword.md
+-rw-r--r--   0        0        0     6493 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/forms.md
+-rw-r--r--   0        0        0     2105 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/installation.md
+-rw-r--r--   0        0        0     3596 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/languages.md
+-rw-r--r--   0        0        0     3087 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/mailer.md
+-rw-r--r--   0        0        0     9672 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/advanced.md
+-rw-r--r--   0        0        0    12917 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/callbacks.md
+-rw-r--r--   0        0        0     7060 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/connecting.md
+-rw-r--r--   0        0        0    20808 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/migrations.md
+-rw-r--r--   0        0        0    14034 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/models.md
+-rw-r--r--   0        0        0    29245 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/operations.md
+-rw-r--r--   0        0        0    27472 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/relations.md
+-rw-r--r--   0        0        0     5523 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/scopes.md
+-rw-r--r--   0        0        0     6732 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm/virtuals.md
+-rw-r--r--   0        0        0     3172 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/orm.md
+-rw-r--r--   0        0        0     4100 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/patterns.md
+-rw-r--r--   0        0        0    14161 2023-05-19 11:27:14.001857 emmett-2.5.2/docs/pipeline.md
+-rw-r--r--   0        0        0    15916 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/quickstart.md
+-rw-r--r--   0        0        0     6082 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/request.md
+-rw-r--r--   0        0        0     3378 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/response.md
+-rw-r--r--   0        0        0    11727 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/routing.md
+-rw-r--r--   0        0        0     2424 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/services.md
+-rw-r--r--   0        0        0     4535 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/sessions.md
+-rw-r--r--   0        0        0     6405 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/templates.md
+-rw-r--r--   0        0        0     6776 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/testing.md
+-rw-r--r--   0        0        0      440 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/tree.yml
+-rw-r--r--   0        0        0    14840 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/tutorial.md
+-rw-r--r--   0        0        0    16597 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/upgrading.md
+-rw-r--r--   0        0        0    15878 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/validations.md
+-rw-r--r--   0        0        0     2307 2023-05-19 11:27:14.005857 emmett-2.5.2/docs/websocket.md
+-rw-r--r--   0        0        0      386 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/__init__.py
+-rw-r--r--   0        0        0      248 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/__main__.py
+-rw-r--r--   0        0        0       22 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/__version__.py
+-rw-r--r--   0        0        0    11242 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/_internal.py
+-rw-r--r--   0        0        0     5633 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/_reloader.py
+-rw-r--r--   0        0        0      771 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/_shortcuts.py
+-rw-r--r--   0        0        0    27001 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/app.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/__init__.py
+-rw-r--r--   0        0        0    15264 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/handlers.py
+-rw-r--r--   0        0        0      220 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/helpers.py
+-rw-r--r--   0        0        0      533 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/typing.py
+-rw-r--r--   0        0        0     3064 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/workers.py
+-rw-r--r--   0        0        0     8029 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/asgi/wrappers.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/__init__.py
+-rw-r--r--   0        0        0     2437 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/shBrushPython.js
+-rw-r--r--   0        0        0     6204 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/shCore.css
+-rw-r--r--   0        0        0    16175 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/shCore.js
+-rw-r--r--   0        0        0     2499 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/shTheme.css
+-rw-r--r--   0        0        0      647 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/view.css
+-rw-r--r--   0        0        0     4626 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/debug/view.html
+-rw-r--r--   0        0        0     1630 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/helpers.js
+-rw-r--r--   0        0        0    89476 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/jquery.min.js
+-rw-r--r--   0        0        0   137986 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/assets/jquery.min.map
+-rw-r--r--   0        0        0    18871 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/cache.py
+-rw-r--r--   0        0        0    15186 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/cli.py
+-rw-r--r--   0        0        0     2547 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/ctx.py
+-rw-r--r--   0        0        0     8165 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/datastructures.py
+-rw-r--r--   0        0        0     5076 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/debug.py
+-rw-r--r--   0        0        0     3201 2023-05-19 11:27:14.005857 emmett-2.5.2/emmett/extensions.py
+-rw-r--r--   0        0        0    25617 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/forms.py
+-rw-r--r--   0        0        0     3095 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/helpers.py
+-rw-r--r--   0        0        0     6435 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/html.py
+-rw-r--r--   0        0        0     8750 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/http.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/language/__init__.py
+-rw-r--r--   0        0        0     1096 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/language/helpers.py
+-rw-r--r--   0        0        0      933 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/language/translator.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/libs/__init__.py
+-rw-r--r--   0        0        0    25207 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/libs/contenttype.py
+-rw-r--r--   0        0        0     3915 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/libs/portalocker.py
+-rw-r--r--   0        0        0      925 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/locals.py
+-rw-r--r--   0        0        0     3084 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/logger.py
+-rw-r--r--   0        0        0      478 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/__init__.py
+-rw-r--r--   0        0        0     2373 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/_patches.py
+-rw-r--r--   0        0        0    13015 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/adapters.py
+-rw-r--r--   0        0        0     3224 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/apis.py
+-rw-r--r--   0        0        0     8857 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/base.py
+-rw-r--r--   0        0        0    12058 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/connection.py
+-rw-r--r--   0        0        0       80 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/engines/__init__.py
+-rw-r--r--   0        0        0     5577 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/engines/postgres.py
+-rw-r--r--   0        0        0     1191 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/engines/sqlite.py
+-rw-r--r--   0        0        0      605 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/errors.py
+-rw-r--r--   0        0        0     1677 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/geo.py
+-rw-r--r--   0        0        0    18102 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/helpers.py
+-rw-r--r--   0        0        0       62 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/__init__.py
+-rw-r--r--   0        0        0     2892 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/base.py
+-rw-r--r--   0        0        0    15289 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/commands.py
+-rw-r--r--   0        0        0    14381 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/engine.py
+-rw-r--r--   0        0        0     1058 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/exceptions.py
+-rw-r--r--   0        0        0    21829 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/generation.py
+-rw-r--r--   0        0        0     3636 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/helpers.py
+-rw-r--r--   0        0        0      491 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/migration.tmpl
+-rw-r--r--   0        0        0    23246 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/operations.py
+-rw-r--r--   0        0        0    14902 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/revisions.py
+-rw-r--r--   0        0        0    12034 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/scripts.py
+-rw-r--r--   0        0        0     1150 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/migrations/utils.py
+-rw-r--r--   0        0        0    46716 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/models.py
+-rw-r--r--   0        0        0    57286 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/objects.py
+-rw-r--r--   0        0        0     4208 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/transactions.py
+-rw-r--r--   0        0        0      978 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/orm/wrappers.py
+-rw-r--r--   0        0        0      917 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/parsers.py
+-rw-r--r--   0        0        0    12040 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/pipeline.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/__init__.py
+-rw-r--r--   0        0        0     5303 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/dispatchers.py
+-rw-r--r--   0        0        0     4112 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/response.py
+-rw-r--r--   0        0        0    11518 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/router.py
+-rw-r--r--   0        0        0     8479 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/routes.py
+-rw-r--r--   0        0        0     7026 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/rules.py
+-rw-r--r--   0        0        0     9704 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/routing/urls.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/rsgi/__init__.py
+-rw-r--r--   0        0        0     9938 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/rsgi/handlers.py
+-rw-r--r--   0        0        0      878 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/rsgi/helpers.py
+-rw-r--r--   0        0        0     4338 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/rsgi/wrappers.py
+-rw-r--r--   0        0        0     5490 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/security.py
+-rw-r--r--   0        0        0     2207 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/serializers.py
+-rw-r--r--   0        0        0     1003 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/server.py
+-rw-r--r--   0        0        0    11649 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/sessions.py
+-rw-r--r--   0        0        0        0 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/templating/__init__.py
+-rw-r--r--   0        0        0     1843 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/templating/lexers.py
+-rw-r--r--   0        0        0     1957 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/templating/templater.py
+-rw-r--r--   0        0        0       37 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/testing/__init__.py
+-rw-r--r--   0        0        0    11877 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/testing/client.py
+-rw-r--r--   0        0        0    10674 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/testing/env.py
+-rw-r--r--   0        0        0    12272 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/testing/helpers.py
+-rw-r--r--   0        0        0    15936 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/testing/urls.py
+-rw-r--r--   0        0        0      125 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/tools/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/tools/auth/__init__.py
+-rw-r--r--   0        0        0     9035 2023-05-19 11:27:14.009857 emmett-2.5.2/emmett/tools/auth/apis.py
+-rw-r--r--   0        0        0    19190 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/auth/exposer.py
+-rw-r--r--   0        0        0    13469 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/auth/ext.py
+-rw-r--r--   0        0        0     5270 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/auth/forms.py
+-rw-r--r--   0        0        0     7485 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/auth/models.py
+-rw-r--r--   0        0        0     1417 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/decorators.py
+-rw-r--r--   0        0        0    10953 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/mailer.py
+-rw-r--r--   0        0        0     1565 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/tools/service.py
+-rw-r--r--   0        0        0      355 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/typing.py
+-rw-r--r--   0        0        0     5357 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/utils.py
+-rw-r--r--   0        0        0    11554 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/__init__.py
+-rw-r--r--   0        0        0     7636 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/basic.py
+-rw-r--r--   0        0        0    31120 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/consist.py
+-rw-r--r--   0        0        0    19038 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/helpers.py
+-rw-r--r--   0        0        0     7367 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/inside.py
+-rw-r--r--   0        0        0     4614 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/validators/process.py
+-rw-r--r--   0        0        0     2190 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/wrappers/__init__.py
+-rw-r--r--   0        0        0     2886 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/wrappers/helpers.py
+-rw-r--r--   0        0        0     3984 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/wrappers/request.py
+-rw-r--r--   0        0        0     1525 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/wrappers/response.py
+-rw-r--r--   0        0        0     1062 2023-05-19 11:27:14.013857 emmett-2.5.2/emmett/wrappers/websocket.py
+-rw-r--r--   0        0        0     2091 2023-05-19 11:27:14.013857 emmett-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1524 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/helpers.py
+-rw-r--r--   0        0        0       46 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/languages/de.json
+-rw-r--r--   0        0        0       49 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/languages/it.json
+-rw-r--r--   0        0        0       69 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/languages/ru.json
+-rw-r--r--   0        0        0      134 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/templates/auth/auth.html
+-rw-r--r--   0        0        0      479 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/templates/layout.html
+-rw-r--r--   0        0        0      153 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/templates/test.html
+-rw-r--r--   0        0        0     8027 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_auth.py
+-rw-r--r--   0        0        0     4658 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_cache.py
+-rw-r--r--   0        0        0     1415 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_http.py
+-rw-r--r--   0        0        0      861 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_logger.py
+-rw-r--r--   0        0        0    11854 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_mailer.py
+-rw-r--r--   0        0        0     8618 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_migrations.py
+-rw-r--r--   0        0        0    33038 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm.py
+-rw-r--r--   0        0        0      853 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm_connections.py
+-rw-r--r--   0        0        0    10074 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm_gis.py
+-rw-r--r--   0        0        0    22722 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm_pks.py
+-rw-r--r--   0        0        0     9863 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm_row.py
+-rw-r--r--   0        0        0     2958 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_orm_transactions.py
+-rw-r--r--   0        0        0    22478 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_pipeline.py
+-rw-r--r--   0        0        0     8659 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_routing.py
+-rw-r--r--   0        0        0     1475 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_session.py
+-rw-r--r--   0        0        0     2705 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_templates.py
+-rw-r--r--   0        0        0      622 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_translator.py
+-rw-r--r--   0        0        0     2045 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_utils.py
+-rw-r--r--   0        0        0    18633 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_validators.py
+-rw-r--r--   0        0        0      822 2023-05-19 11:27:14.013857 emmett-2.5.2/tests/test_wrappers.py
+-rw-r--r--   0        0        0     5026 1970-01-01 00:00:00.000000 emmett-2.5.2/PKG-INFO
```

### Comparing `emmett-2.5.1/CHANGES.md` & `emmett-2.5.2/CHANGES.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/LICENSE` & `emmett-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/README.md` & `emmett-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/app_and_modules.md` & `emmett-2.5.2/docs/app_and_modules.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/auth.md` & `emmett-2.5.2/docs/auth.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/caching.md` & `emmett-2.5.2/docs/caching.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/cli.md` & `emmett-2.5.2/docs/cli.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/debug_and_logging.md` & `emmett-2.5.2/docs/debug_and_logging.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/deployment.md` & `emmett-2.5.2/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/extensions.md` & `emmett-2.5.2/docs/extensions.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/foreword.md` & `emmett-2.5.2/docs/foreword.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/forms.md` & `emmett-2.5.2/docs/forms.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/installation.md` & `emmett-2.5.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/languages.md` & `emmett-2.5.2/docs/languages.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/mailer.md` & `emmett-2.5.2/docs/mailer.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/orm/advanced.md` & `emmett-2.5.2/docs/orm/advanced.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/orm/callbacks.md` & `emmett-2.5.2/docs/orm/callbacks.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/orm/connecting.md` & `emmett-2.5.2/docs/orm/connecting.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/orm/migrations.md` & `emmett-2.5.2/docs/orm/migrations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/orm/models.md` & `emmett-2.5.2/docs/orm/models.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/orm/operations.md` & `emmett-2.5.2/docs/orm/operations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/orm/relations.md` & `emmett-2.5.2/docs/orm/relations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/orm/scopes.md` & `emmett-2.5.2/docs/orm/scopes.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/orm/virtuals.md` & `emmett-2.5.2/docs/orm/virtuals.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/orm.md` & `emmett-2.5.2/docs/orm.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/patterns.md` & `emmett-2.5.2/docs/patterns.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/pipeline.md` & `emmett-2.5.2/docs/pipeline.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/quickstart.md` & `emmett-2.5.2/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/request.md` & `emmett-2.5.2/docs/request.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/response.md` & `emmett-2.5.2/docs/response.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/routing.md` & `emmett-2.5.2/docs/routing.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/services.md` & `emmett-2.5.2/docs/services.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/sessions.md` & `emmett-2.5.2/docs/sessions.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/templates.md` & `emmett-2.5.2/docs/templates.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/testing.md` & `emmett-2.5.2/docs/testing.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/tutorial.md` & `emmett-2.5.2/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/upgrading.md` & `emmett-2.5.2/docs/upgrading.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/validations.md` & `emmett-2.5.2/docs/validations.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/docs/websocket.md` & `emmett-2.5.2/docs/websocket.md`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/_internal.py` & `emmett-2.5.2/emmett/_internal.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/_reloader.py` & `emmett-2.5.2/emmett/_reloader.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/_shortcuts.py` & `emmett-2.5.2/emmett/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/app.py` & `emmett-2.5.2/emmett/app.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/asgi/handlers.py` & `emmett-2.5.2/emmett/asgi/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,21 +246,23 @@
                     static_file = lang_file
             return static_file, version
         return None, None
 
     def _static_nolang_matcher(
         self, path: str
     ) -> Tuple[Optional[str], Optional[str]]:
-        if path.startswith('/static'):
+        if path.startswith('/static/'):
             mname, version, file_name = REGEX_STATIC.match(path).group('m', 'v', 'f')
             if mname:
                 mod = self.app._modules.get(mname[2:-3])
                 static_file = os.path.join(mod._static_path, file_name) if mod else None
-            else:
+            elif file_name:
                 static_file = os.path.join(self.app.static_path, file_name)
+            else:
+                static_file = None
             return static_file, version
         return None, None
 
     async def _static_response(self, file_path: str) -> HTTPFile:
         return HTTPFile(file_path)
 
     async def _static_content(self, content: bytes, content_type: str) -> HTTPBytes:
@@ -284,15 +286,15 @@
         receive: Receive,
         send: Send
     ) -> Awaitable[HTTPResponse]:
         path = scope['emt.path']
         #: handle internal assets
         if path.startswith('/__emmett__'):
             file_name = path[12:]
-            if file_name.endswith(".html"):
+            if not file_name or file_name.endswith(".html"):
                 return self._http_response(404)
             pkg = None
             if '/' in file_name:
                 pkg, file_name = file_name.split('/', 1)
             try:
                 file_contents = resources.read_binary(
                     f'emmett.assets.{pkg}' if pkg else 'emmett.assets',
```

### Comparing `emmett-2.5.1/emmett/asgi/typing.py` & `emmett-2.5.2/emmett/asgi/typing.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/asgi/workers.py` & `emmett-2.5.2/emmett/asgi/workers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/asgi/wrappers.py` & `emmett-2.5.2/emmett/asgi/wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/assets/debug/shBrushPython.js` & `emmett-2.5.2/emmett/assets/debug/shBrushPython.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/assets/debug/shCore.css` & `emmett-2.5.2/emmett/assets/debug/shCore.css`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/assets/debug/shCore.js` & `emmett-2.5.2/emmett/assets/debug/shCore.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/assets/debug/shTheme.css` & `emmett-2.5.2/emmett/assets/debug/shTheme.css`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/assets/debug/view.css` & `emmett-2.5.2/emmett/assets/debug/view.css`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/assets/debug/view.html` & `emmett-2.5.2/emmett/assets/debug/view.html`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/assets/helpers.js` & `emmett-2.5.2/emmett/assets/helpers.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/assets/jquery.min.js` & `emmett-2.5.2/emmett/assets/jquery.min.js`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/assets/jquery.min.map` & `emmett-2.5.2/emmett/assets/jquery.min.map`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/cache.py` & `emmett-2.5.2/emmett/cache.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/cli.py` & `emmett-2.5.2/emmett/cli.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/ctx.py` & `emmett-2.5.2/emmett/ctx.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/datastructures.py` & `emmett-2.5.2/emmett/datastructures.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/debug.py` & `emmett-2.5.2/emmett/debug.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/extensions.py` & `emmett-2.5.2/emmett/extensions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/forms.py` & `emmett-2.5.2/emmett/forms.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/helpers.py` & `emmett-2.5.2/emmett/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/html.py` & `emmett-2.5.2/emmett/html.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/http.py` & `emmett-2.5.2/emmett/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,20 +240,20 @@
                     'more_body': more_body,
                 })
 
     def rsgi(self, protocol: HTTPProtocol):
         try:
             stat_data = os.stat(self.file_path)
             if not stat.S_ISREG(stat_data.st_mode):
-                return HTTP(403).rsgi()
+                return HTTP(403).rsgi(protocol)
             self._headers.update(self._get_stat_headers(stat_data))
         except IOError as e:
             if e.errno == errno.EACCES:
-                return HTTP(403).rsgi()
-            return HTTP(404).rsgi()
+                return HTTP(403).rsgi(protocol)
+            return HTTP(404).rsgi(protocol)
 
         protocol.response_file(
             self.status_code,
             list(self.rsgi_headers),
             self.file_path
         )
```

### Comparing `emmett-2.5.1/emmett/language/helpers.py` & `emmett-2.5.2/emmett/language/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/language/translator.py` & `emmett-2.5.2/emmett/language/translator.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/libs/contenttype.py` & `emmett-2.5.2/emmett/libs/contenttype.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/libs/portalocker.py` & `emmett-2.5.2/emmett/libs/portalocker.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/locals.py` & `emmett-2.5.2/emmett/locals.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/logger.py` & `emmett-2.5.2/emmett/logger.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/_patches.py` & `emmett-2.5.2/emmett/orm/_patches.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/adapters.py` & `emmett-2.5.2/emmett/orm/adapters.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/apis.py` & `emmett-2.5.2/emmett/orm/apis.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/base.py` & `emmett-2.5.2/emmett/orm/base.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/connection.py` & `emmett-2.5.2/emmett/orm/connection.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/engines/postgres.py` & `emmett-2.5.2/emmett/orm/engines/postgres.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/engines/sqlite.py` & `emmett-2.5.2/emmett/orm/engines/sqlite.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/errors.py` & `emmett-2.5.2/emmett/orm/errors.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/geo.py` & `emmett-2.5.2/emmett/orm/geo.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/helpers.py` & `emmett-2.5.2/emmett/orm/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/migrations/base.py` & `emmett-2.5.2/emmett/orm/migrations/base.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/migrations/commands.py` & `emmett-2.5.2/emmett/orm/migrations/commands.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/migrations/engine.py` & `emmett-2.5.2/emmett/orm/migrations/engine.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/migrations/exceptions.py` & `emmett-2.5.2/emmett/orm/migrations/exceptions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/migrations/generation.py` & `emmett-2.5.2/emmett/orm/migrations/generation.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/migrations/helpers.py` & `emmett-2.5.2/emmett/orm/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/migrations/operations.py` & `emmett-2.5.2/emmett/orm/migrations/operations.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/migrations/revisions.py` & `emmett-2.5.2/emmett/orm/migrations/revisions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/migrations/scripts.py` & `emmett-2.5.2/emmett/orm/migrations/scripts.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/migrations/utils.py` & `emmett-2.5.2/emmett/orm/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/models.py` & `emmett-2.5.2/emmett/orm/models.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/objects.py` & `emmett-2.5.2/emmett/orm/objects.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/transactions.py` & `emmett-2.5.2/emmett/orm/transactions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/orm/wrappers.py` & `emmett-2.5.2/emmett/orm/wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/parsers.py` & `emmett-2.5.2/emmett/parsers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/pipeline.py` & `emmett-2.5.2/emmett/pipeline.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/routing/dispatchers.py` & `emmett-2.5.2/emmett/routing/dispatchers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/routing/response.py` & `emmett-2.5.2/emmett/routing/response.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/routing/router.py` & `emmett-2.5.2/emmett/routing/router.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/routing/routes.py` & `emmett-2.5.2/emmett/routing/routes.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/routing/rules.py` & `emmett-2.5.2/emmett/routing/rules.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/routing/urls.py` & `emmett-2.5.2/emmett/routing/urls.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/rsgi/handlers.py` & `emmett-2.5.2/emmett/rsgi/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,21 +140,23 @@
                     static_file = lang_file
             return static_file, version
         return None, None
 
     def _static_nolang_matcher(
         self, path: str
     ) -> Tuple[Optional[str], Optional[str]]:
-        if path.startswith('/static'):
+        if path.startswith('/static/'):
             mname, version, file_name = REGEX_STATIC.match(path).group('m', 'v', 'f')
             if mname:
                 mod = self.app._modules.get(mname[2:-3])
                 static_file = os.path.join(mod._static_path, file_name) if mod else None
-            else:
+            elif file_name:
                 static_file = os.path.join(self.app.static_path, file_name)
+            else:
+                static_file = None
             return static_file, version
         return None, None
 
     async def _static_response(self, file_path: str) -> HTTPFile:
         return HTTPFile(file_path)
 
     def _static_handler(
@@ -162,16 +164,19 @@
         scope: Scope,
         protocol: HTTPProtocol,
         path: str
     ) -> Awaitable[HTTPResponse]:
         #: handle internal assets
         if path.startswith('/__emmett__'):
             file_name = path[12:]
+            if not file_name:
+                return self._http_response(404)
             static_file = os.path.join(
-                os.path.dirname(__file__), '..', 'assets', file_name)
+                os.path.dirname(__file__), '..', 'assets', file_name
+            )
             if os.path.splitext(static_file)[1] == 'html':
                 return self._http_response(404)
             return self._static_response(static_file)
         #: handle app assets
         static_file, _ = self.static_matcher(path)
         if static_file:
             return self._static_response(static_file)
```

### Comparing `emmett-2.5.1/emmett/rsgi/helpers.py` & `emmett-2.5.2/emmett/rsgi/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/rsgi/wrappers.py` & `emmett-2.5.2/emmett/rsgi/wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/security.py` & `emmett-2.5.2/emmett/security.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/serializers.py` & `emmett-2.5.2/emmett/serializers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/server.py` & `emmett-2.5.2/emmett/server.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/sessions.py` & `emmett-2.5.2/emmett/sessions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/templating/lexers.py` & `emmett-2.5.2/emmett/templating/lexers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/templating/templater.py` & `emmett-2.5.2/emmett/templating/templater.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/testing/client.py` & `emmett-2.5.2/emmett/testing/client.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/testing/env.py` & `emmett-2.5.2/emmett/testing/env.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/testing/helpers.py` & `emmett-2.5.2/emmett/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/testing/urls.py` & `emmett-2.5.2/emmett/testing/urls.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/tools/auth/apis.py` & `emmett-2.5.2/emmett/tools/auth/apis.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/tools/auth/exposer.py` & `emmett-2.5.2/emmett/tools/auth/exposer.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/tools/auth/ext.py` & `emmett-2.5.2/emmett/tools/auth/ext.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/tools/auth/forms.py` & `emmett-2.5.2/emmett/tools/auth/forms.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/tools/auth/models.py` & `emmett-2.5.2/emmett/tools/auth/models.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/tools/decorators.py` & `emmett-2.5.2/emmett/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/tools/mailer.py` & `emmett-2.5.2/emmett/tools/mailer.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/tools/service.py` & `emmett-2.5.2/emmett/tools/service.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/utils.py` & `emmett-2.5.2/emmett/utils.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/validators/__init__.py` & `emmett-2.5.2/emmett/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/validators/basic.py` & `emmett-2.5.2/emmett/validators/basic.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/validators/consist.py` & `emmett-2.5.2/emmett/validators/consist.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/validators/helpers.py` & `emmett-2.5.2/emmett/validators/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/validators/inside.py` & `emmett-2.5.2/emmett/validators/inside.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/validators/process.py` & `emmett-2.5.2/emmett/validators/process.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/wrappers/__init__.py` & `emmett-2.5.2/emmett/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/wrappers/helpers.py` & `emmett-2.5.2/emmett/wrappers/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/wrappers/request.py` & `emmett-2.5.2/emmett/wrappers/request.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/wrappers/response.py` & `emmett-2.5.2/emmett/wrappers/response.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/emmett/wrappers/websocket.py` & `emmett-2.5.2/emmett/wrappers/websocket.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/pyproject.toml` & `emmett-2.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett"
-version = "2.5.1"
+version = "2.5.2"
 description = "The web framework for inventors"
 authors = ["Giovanni Barillari <gi0baro@d4net.org>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://emmett.sh"
 repository = "https://github.com/emmett-framework/emmett"
@@ -39,15 +39,15 @@
 
 [tool.poetry.scripts]
 emmett = "emmett.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = ">=6.0"
-granian = "~0.4.0"
+granian = "~0.4.2"
 emmett-crypto = "~0.3"
 pendulum = "~2.1.2"
 pyDAL = "17.3"
 python-rapidjson = "^1.0"
 pyyaml = "^6.0"
 renoir = "^1.6"
 severus = "^1.1"
```

### Comparing `emmett-2.5.1/tests/helpers.py` & `emmett-2.5.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_auth.py` & `emmett-2.5.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_cache.py` & `emmett-2.5.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_http.py` & `emmett-2.5.2/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_logger.py` & `emmett-2.5.2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_mailer.py` & `emmett-2.5.2/tests/test_mailer.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_migrations.py` & `emmett-2.5.2/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_orm.py` & `emmett-2.5.2/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_orm_connections.py` & `emmett-2.5.2/tests/test_orm_connections.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_orm_gis.py` & `emmett-2.5.2/tests/test_orm_gis.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_orm_pks.py` & `emmett-2.5.2/tests/test_orm_pks.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_orm_row.py` & `emmett-2.5.2/tests/test_orm_row.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_orm_transactions.py` & `emmett-2.5.2/tests/test_orm_transactions.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_pipeline.py` & `emmett-2.5.2/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_routing.py` & `emmett-2.5.2/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_session.py` & `emmett-2.5.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_templates.py` & `emmett-2.5.2/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_translator.py` & `emmett-2.5.2/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_utils.py` & `emmett-2.5.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_validators.py` & `emmett-2.5.2/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/tests/test_wrappers.py` & `emmett-2.5.2/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett-2.5.1/PKG-INFO` & `emmett-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett
-Version: 2.5.1
+Version: 2.5.2
 Summary: The web framework for inventors
 Home-page: https://emmett.sh
 License: BSD-3-Clause
 Keywords: web,asyncio
 Author: Giovanni Barillari
 Author-email: gi0baro@d4net.org
 Requires-Python: >=3.8,<4.0
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: orjson
 Provides-Extra: uvicorn
 Requires-Dist: click (>=6.0)
 Requires-Dist: emmett-crypto (>=0.3,<0.4)
-Requires-Dist: granian (>=0.4.0,<0.5.0)
+Requires-Dist: granian (>=0.4.2,<0.5.0)
 Requires-Dist: h11 (>=0.12.0) ; extra == "uvicorn"
 Requires-Dist: httptools (>=0.5.0,<0.6.0) ; (sys_platform != "win32") and (extra == "uvicorn")
 Requires-Dist: orjson (>=3.8,<3.9) ; extra == "orjson"
 Requires-Dist: pendulum (>=2.1.2,<2.2.0)
 Requires-Dist: pyDAL (==17.3)
 Requires-Dist: python-rapidjson (>=1.0,<2.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
```

