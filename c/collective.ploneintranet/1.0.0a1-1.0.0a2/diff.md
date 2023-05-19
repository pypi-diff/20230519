# Comparing `tmp/collective.ploneintranet-1.0.0a1.tar.gz` & `tmp/collective.ploneintranet-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.ploneintranet-1.0.0a1.tar", last modified: Fri May 19 14:49:13 2023, max compression
+gzip compressed data, was "collective.ploneintranet-1.0.0a2.tar", last modified: Fri May 19 15:14:57 2023, max compression
```

## Comparing `collective.ploneintranet-1.0.0a1.tar` & `collective.ploneintranet-1.0.0a2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.327258 collective.ploneintranet-1.0.0a1/
--rw-r--r--   0 ericof     (501) staff       (20)       52 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/.coveragerc
--rw-r--r--   0 ericof     (501) staff       (20)      973 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/.editorconfig
--rw-r--r--   0 ericof     (501) staff       (20)      381 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/CHANGES.md
--rw-r--r--   0 ericof     (501) staff       (20)       52 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/CONTRIBUTORS.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/LICENSE.GPL
--rw-r--r--   0 ericof     (501) staff       (20)      672 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/LICENSE.md
--rw-r--r--   0 ericof     (501) staff       (20)      306 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     6816 2023-05-19 14:49:13.327135 collective.ploneintranet-1.0.0a1/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     5102 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/README.md
--rw-r--r--   0 ericof     (501) staff       (20)       61 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/constraints.txt
--rw-r--r--   0 ericof     (501) staff       (20)     2802 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/docker-compose.yml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.319051 collective.ploneintranet-1.0.0a1/docs/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/docs/.gitkeep
--rw-r--r--   0 ericof     (501) staff       (20)      309 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/docs/changelog_template.jinja
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.319208 collective.ploneintranet-1.0.0a1/news/
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/news/.gitkeep
--rw-r--r--   0 ericof     (501) staff       (20)     1072 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)       29 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/requirements-docker.txt
--rw-r--r--   0 ericof     (501) staff       (20)       32 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/requirements.txt
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-05-19 14:49:13.327291 collective.ploneintranet-1.0.0a1/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2446 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.315078 collective.ploneintranet-1.0.0a1/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.319364 collective.ploneintranet-1.0.0a1/src/collective/
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.321389 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/
--rw-r--r--   0 ericof     (501) staff       (20)      204 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      532 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)      320 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/dependencies.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.315290 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.321884 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.322275 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.315653 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/blobs/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.322407 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/blobs/a98774abf06e49078f3f206a8b055dc2-image/
--rw-r--r--   0 ericof     (501) staff       (20)    60300 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/blobs/a98774abf06e49078f3f206a8b055dc2-image/plone-foundation-logo.png
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.322573 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/blobs/c98f1f1eceab478097ed7d5ca13e0101-image/
--rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/blobs/c98f1f1eceab478097ed7d5ca13e0101-image/image.png
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.322827 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/blobs/f96cfb63b6284c49a49b9dd45e98394b-image/
--rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/blobs/f96cfb63b6284c49a49b9dd45e98394b-image/image.png
--rw-r--r--   0 ericof     (501) staff       (20)    26487 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/content.json
--rw-r--r--   0 ericof     (501) staff       (20)      593 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/ordering.json
--rw-r--r--   0 ericof     (501) staff       (20)     1605 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      226 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     3471 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/schema.json
--rw-r--r--   0 ericof     (501) staff       (20)      469 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     3278 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/handler.py
--rw-r--r--   0 ericof     (501) staff       (20)      239 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/interfaces.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.323293 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/locales/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/locales/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1867 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/locales/collective.ploneintranet.pot
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.315850 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/locales/en/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.323417 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/locales/en/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)     1758 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/locales/en/LC_MESSAGES/collective.ploneintranet.po
--rw-r--r--   0 ericof     (501) staff       (20)     1950 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/locales/update.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.316415 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.324158 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/
--rw-r--r--   0 ericof     (501) staff       (20)      181 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/browserlayer.xml
--rw-r--r--   0 ericof     (501) staff       (20)       81 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/catalog.xml
--rw-r--r--   0 ericof     (501) staff       (20)      195 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/metadata.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.324676 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/registry/
--rw-r--r--   0 ericof     (501) staff       (20)      810 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/registry/plone.app.discussion.interfaces.IDiscussionSettings.xml
--rw-r--r--   0 ericof     (501) staff       (20)      256 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/registry/plone.base.interfaces.controlpanel.IMailSchema.xml
--rw-r--r--   0 ericof     (501) staff       (20)      358 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/registry/plone.base.interfaces.controlpanel.INavigationSchema.xml
--rw-r--r--   0 ericof     (501) staff       (20)      251 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/registry/plone.base.interfaces.controlpanel.ISiteSchema.xml
--rw-r--r--   0 ericof     (501) staff       (20)      109 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/theme.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.324904 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/types/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/types/.gitkeep
--rw-r--r--   0 ericof     (501) staff       (20)      363 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/types/Glossary.xml
--rw-r--r--   0 ericof     (501) staff       (20)      192 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/types.xml
--rw-r--r--   0 ericof     (501) staff       (20)      951 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/userschema.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.325025 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/oauth/
--rw-r--r--   0 ericof     (501) staff       (20)      198 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/oauth/metadata.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.325154 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/oauth/registry/
--rw-r--r--   0 ericof     (501) staff       (20)      387 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/oauth/registry/pas.plugins.authomatic.interfaces.IPasPluginsAuthomaticSettings.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.325282 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/uninstall/
--rw-r--r--   0 ericof     (501) staff       (20)      127 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.325525 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/volto/
--rw-r--r--   0 ericof     (501) staff       (20)      187 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/volto/metadata.xml
--rw-r--r--   0 ericof     (501) staff       (20)      743 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/volto/workflows.xml
--rw-r--r--   0 ericof     (501) staff       (20)     1225 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.325651 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/setuphandlers/
--rw-r--r--   0 ericof     (501) staff       (20)      352 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/setuphandlers/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.325982 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/subscribers/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/subscribers/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      215 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/subscribers/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)      910 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/subscribers/post_login.py
--rw-r--r--   0 ericof     (501) staff       (20)     1354 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/testing.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.326202 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/upgrades/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/upgrades/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      475 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/upgrades/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.320414 collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     6816 2023-05-19 14:49:13.000000 collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     3847 2023-05-19 14:49:13.000000 collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-19 14:49:13.000000 collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)      134 2023-05-19 14:49:13.000000 collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)       11 2023-05-19 14:49:13.000000 collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-19 14:49:13.000000 collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/not-zip-safe
--rw-r--r--   0 ericof     (501) staff       (20)      223 2023-05-19 14:49:13.000000 collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)       11 2023-05-19 14:49:13.000000 collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/top_level.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.326411 collective.ploneintranet-1.0.0a1/tests/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/tests/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      487 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/tests/conftest.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.326734 collective.ploneintranet-1.0.0a1/tests/creation/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/tests/creation/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      167 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/tests/creation/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     5506 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/tests/creation/test_create_intranet_volto.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:13.326949 collective.ploneintranet-1.0.0a1/tests/registration/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/tests/registration/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     2500 2023-05-19 14:49:12.000000 collective.ploneintranet-1.0.0a1/tests/registration/test_distribution_volto.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.901843 collective.ploneintranet-1.0.0a2/
+-rw-r--r--   0 ericof     (501) staff       (20)       52 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/.coveragerc
+-rw-r--r--   0 ericof     (501) staff       (20)      973 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)      477 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/CHANGES.md
+-rw-r--r--   0 ericof     (501) staff       (20)       52 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/CONTRIBUTORS.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/LICENSE.GPL
+-rw-r--r--   0 ericof     (501) staff       (20)      672 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/LICENSE.md
+-rw-r--r--   0 ericof     (501) staff       (20)      306 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     6912 2023-05-19 15:14:57.901671 collective.ploneintranet-1.0.0a2/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     5102 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       61 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/constraints.txt
+-rw-r--r--   0 ericof     (501) staff       (20)     2802 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/docker-compose.yml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.893285 collective.ploneintranet-1.0.0a2/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/docs/.gitkeep
+-rw-r--r--   0 ericof     (501) staff       (20)      309 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/docs/changelog_template.jinja
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.893409 collective.ploneintranet-1.0.0a2/news/
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/news/.gitkeep
+-rw-r--r--   0 ericof     (501) staff       (20)     1072 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)       29 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/requirements-docker.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       32 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2023-05-19 15:14:57.901884 collective.ploneintranet-1.0.0a2/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2446 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.889462 collective.ploneintranet-1.0.0a2/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.893532 collective.ploneintranet-1.0.0a2/src/collective/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.895539 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/
+-rw-r--r--   0 ericof     (501) staff       (20)      204 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      532 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)      320 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/dependencies.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.889663 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.896038 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.896425 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.890018 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/blobs/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.896555 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/blobs/a98774abf06e49078f3f206a8b055dc2-image/
+-rw-r--r--   0 ericof     (501) staff       (20)    60300 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/blobs/a98774abf06e49078f3f206a8b055dc2-image/plone-foundation-logo.png
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.896720 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/blobs/c98f1f1eceab478097ed7d5ca13e0101-image/
+-rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/blobs/c98f1f1eceab478097ed7d5ca13e0101-image/image.png
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.896971 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/blobs/f96cfb63b6284c49a49b9dd45e98394b-image/
+-rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/blobs/f96cfb63b6284c49a49b9dd45e98394b-image/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)    26487 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/content.json
+-rw-r--r--   0 ericof     (501) staff       (20)      593 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/ordering.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1605 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      226 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     3471 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/schema.json
+-rw-r--r--   0 ericof     (501) staff       (20)      469 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     3278 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/handler.py
+-rw-r--r--   0 ericof     (501) staff       (20)      239 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/interfaces.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.897430 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/locales/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/locales/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1867 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/locales/collective.ploneintranet.pot
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.890224 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/locales/en/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.897554 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/locales/en/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)     1758 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/locales/en/LC_MESSAGES/collective.ploneintranet.po
+-rw-r--r--   0 ericof     (501) staff       (20)     1950 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/locales/update.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.890790 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.898306 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/
+-rw-r--r--   0 ericof     (501) staff       (20)      181 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/browserlayer.xml
+-rw-r--r--   0 ericof     (501) staff       (20)       81 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/catalog.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      195 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/metadata.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.898835 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/registry/
+-rw-r--r--   0 ericof     (501) staff       (20)      810 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/registry/plone.app.discussion.interfaces.IDiscussionSettings.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      256 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/registry/plone.base.interfaces.controlpanel.IMailSchema.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      358 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/registry/plone.base.interfaces.controlpanel.INavigationSchema.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      251 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/registry/plone.base.interfaces.controlpanel.ISiteSchema.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      109 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/theme.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.899064 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/types/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/types/.gitkeep
+-rw-r--r--   0 ericof     (501) staff       (20)      363 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/types/Glossary.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      192 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/types.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      951 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/userschema.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.899184 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/oauth/
+-rw-r--r--   0 ericof     (501) staff       (20)      198 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/oauth/metadata.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.899315 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/oauth/registry/
+-rw-r--r--   0 ericof     (501) staff       (20)      387 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/oauth/registry/pas.plugins.authomatic.interfaces.IPasPluginsAuthomaticSettings.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.899442 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/uninstall/
+-rw-r--r--   0 ericof     (501) staff       (20)      127 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.899693 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/volto/
+-rw-r--r--   0 ericof     (501) staff       (20)      187 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/volto/metadata.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      743 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/volto/workflows.xml
+-rw-r--r--   0 ericof     (501) staff       (20)     1225 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.899816 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/setuphandlers/
+-rw-r--r--   0 ericof     (501) staff       (20)      352 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/setuphandlers/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.900297 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/subscribers/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/subscribers/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      215 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/subscribers/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)      910 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/subscribers/post_login.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1354 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/testing.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.900579 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/upgrades/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/upgrades/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      475 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/upgrades/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.894545 collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)     6912 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     3847 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      134 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       11 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      223 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       11 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/top_level.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.900820 collective.ploneintranet-1.0.0a2/tests/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/tests/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      487 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.901172 collective.ploneintranet-1.0.0a2/tests/creation/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/tests/creation/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      167 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/tests/creation/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5506 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/tests/creation/test_create_intranet_volto.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.901409 collective.ploneintranet-1.0.0a2/tests/registration/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/tests/registration/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2500 2023-05-19 15:14:57.000000 collective.ploneintranet-1.0.0a2/tests/registration/test_distribution_volto.py
```

### Comparing `collective.ploneintranet-1.0.0a1/.editorconfig` & `collective.ploneintranet-1.0.0a2/.editorconfig`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/LICENSE.GPL` & `collective.ploneintranet-1.0.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/LICENSE.md` & `collective.ploneintranet-1.0.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/PKG-INFO` & `collective.ploneintranet-1.0.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.ploneintranet
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Plone Intranet configuration package.
 Home-page: https://github.com/collective/collective.ploneintranet
 Author: Plone Foundation
 Author-email: collective@plone.org
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.ploneintranet
 Project-URL: Source, https://github.com/collective/collective.ploneintranet
@@ -144,14 +144,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a2 (2023-05-19)
+
+
+### Bug fixes:
+
+- Fix GHA Docker image release process [@ericof] #2
+
+
 ## 1.0.0a1 (2023-05-19)
 
 
 ### New features:
 
 - Initial release. [ericof] #1
```

### Comparing `collective.ploneintranet-1.0.0a1/README.md` & `collective.ploneintranet-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/docker-compose.yml` & `collective.ploneintranet-1.0.0a2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/pyproject.toml` & `collective.ploneintranet-1.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/setup.py` & `collective.ploneintranet-1.0.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 {Path("CONTRIBUTORS.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 
 setup(
     name="collective.ploneintranet",
-    version="1.0.0a1",
+    version="1.0.0a2",
     description="Plone Intranet configuration package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/configure.zcml` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/blobs/a98774abf06e49078f3f206a8b055dc2-image/plone-foundation-logo.png` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/blobs/a98774abf06e49078f3f206a8b055dc2-image/plone-foundation-logo.png`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/blobs/c98f1f1eceab478097ed7d5ca13e0101-image/image.png` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/blobs/c98f1f1eceab478097ed7d5ca13e0101-image/image.png`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/blobs/f96cfb63b6284c49a49b9dd45e98394b-image/image.png` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/blobs/f96cfb63b6284c49a49b9dd45e98394b-image/image.png`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/content.json` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/content.json`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/ordering.json` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/ordering.json`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/content/portal.json` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/content/portal.json`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/image.png` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/image.png`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/distributions/volto/schema.json` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/distributions/volto/schema.json`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/handler.py` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/handler.py`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/locales/collective.ploneintranet.pot` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/locales/collective.ploneintranet.pot`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/locales/en/LC_MESSAGES/collective.ploneintranet.po` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/locales/en/LC_MESSAGES/collective.ploneintranet.po`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/locales/update.py` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/registry/plone.app.discussion.interfaces.IDiscussionSettings.xml` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/registry/plone.app.discussion.interfaces.IDiscussionSettings.xml`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/default/userschema.xml` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/default/userschema.xml`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles/volto/workflows.xml` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles/volto/workflows.xml`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/profiles.zcml` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/subscribers/post_login.py` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/subscribers/post_login.py`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective/ploneintranet/testing.py` & `collective.ploneintranet-1.0.0a2/src/collective/ploneintranet/testing.py`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/PKG-INFO` & `collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.ploneintranet
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Plone Intranet configuration package.
 Home-page: https://github.com/collective/collective.ploneintranet
 Author: Plone Foundation
 Author-email: collective@plone.org
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.ploneintranet
 Project-URL: Source, https://github.com/collective/collective.ploneintranet
@@ -144,14 +144,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a2 (2023-05-19)
+
+
+### Bug fixes:
+
+- Fix GHA Docker image release process [@ericof] #2
+
+
 ## 1.0.0a1 (2023-05-19)
 
 
 ### New features:
 
 - Initial release. [ericof] #1
```

### Comparing `collective.ploneintranet-1.0.0a1/src/collective.ploneintranet.egg-info/SOURCES.txt` & `collective.ploneintranet-1.0.0a2/src/collective.ploneintranet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/tests/creation/test_create_intranet_volto.py` & `collective.ploneintranet-1.0.0a2/tests/creation/test_create_intranet_volto.py`

 * *Files identical despite different names*

### Comparing `collective.ploneintranet-1.0.0a1/tests/registration/test_distribution_volto.py` & `collective.ploneintranet-1.0.0a2/tests/registration/test_distribution_volto.py`

 * *Files identical despite different names*

