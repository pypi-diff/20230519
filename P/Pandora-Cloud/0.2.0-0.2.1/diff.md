# Comparing `tmp/Pandora-Cloud-0.2.0.tar.gz` & `tmp/Pandora-Cloud-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora-cloud/pandora-cloud/dist/.tmp-9jl96syb/Pandora-Cloud-0.2.0.tar", last modified: Mon May 15 06:56:06 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora-cloud/pandora-cloud/dist/.tmp-j3pghfbo/Pandora-Cloud-0.2.1.tar", last modified: Fri May 19 04:28:07 2023, max compression
```

## Comparing `Pandora-Cloud-0.2.0.tar` & `Pandora-Cloud-0.2.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/Pandora_Cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/Pandora_Cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/Pandora_Cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/Pandora_Cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/Pandora_Cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/35uzIQibpwv56FyPcgmGz/
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/35uzIQibpwv56FyPcgmGz/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/35uzIQibpwv56FyPcgmGz/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    69737 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
--rw-r--r--   0 runner    (1001) docker     (123)   262802 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    18732 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/259-3a89909da92e8e07.js
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/2802bd5f-8ff236fd4fe2a08c.js
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/58-f9da11f48bf979b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js
--rw-r--r--   0 runner    (1001) docker     (123)   305313 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/734-d34f3efd388e555d.js
--rw-r--r--   0 runner    (1001) docker     (123)  1258458 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/791-87c69e21acb5fd01.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141071 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
--rw-r--r--   0 runner    (1001) docker     (123)   115058 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)   832615 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/_app-ab949dad0ea9d6e3.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/_error-433a1bbdb23dd341.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-3f284519581cedab.js
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/manage-6ac6d4f0510ced68.js
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-67c7e2815007721d.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-73c3d3d7a4970449.js
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-78bcf9600a6bd4b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-338530f42d5b2105.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-2337d8baa604475c.js
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-a51bd7ac61420e8d.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/
--rw-r--r--   0 runner    (1001) docker     (123)    27863 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-31ac023eeccf1f5b.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-b9488b953c4653c2.js
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/status-6557d60655b68492.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/webpack-febc072ffb3fcfd3.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   118969 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/css/b389cdeaa663d62e.css
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/
--rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/
--rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/signifier/
--rw-r--r--   0 runner    (1001) docker     (123)    56682 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    56456 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    53009 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    40456 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    38746 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35690 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/ulp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/ulp/react-components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
--rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:56:06.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/templates/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/flask/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-15 06:55:53.000000 Pandora-Cloud-0.2.0/src/pandora_cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/Pandora_Cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/Pandora_Cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/Pandora_Cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/Pandora_Cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/Pandora_Cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/35uzIQibpwv56FyPcgmGz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/35uzIQibpwv56FyPcgmGz/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/35uzIQibpwv56FyPcgmGz/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    69737 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
+-rw-r--r--   0 runner    (1001) docker     (123)   262802 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18732 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/259-3a89909da92e8e07.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/2802bd5f-8ff236fd4fe2a08c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/58-f9da11f48bf979b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js
+-rw-r--r--   0 runner    (1001) docker     (123)   305403 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/734-d34f3efd388e555d.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1258458 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/791-87c69e21acb5fd01.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141071 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   115058 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   832615 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/_app-ab949dad0ea9d6e3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/_error-433a1bbdb23dd341.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-3f284519581cedab.js
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/manage-6ac6d4f0510ced68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-67c7e2815007721d.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-73c3d3d7a4970449.js
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-78bcf9600a6bd4b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-338530f42d5b2105.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-2337d8baa604475c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-a51bd7ac61420e8d.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)    27863 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-31ac023eeccf1f5b.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-b9488b953c4653c2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/status-6557d60655b68492.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/webpack-febc072ffb3fcfd3.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   118969 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/css/b389cdeaa663d62e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/
+-rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/
+-rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/signifier/
+-rw-r--r--   0 runner    (1001) docker     (123)    56682 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    56456 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    53009 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    40456 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    38746 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35690 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/ulp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/ulp/react-components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:28:07.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/templates/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/flask/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-05-19 04:27:55.000000 Pandora-Cloud-0.2.1/src/pandora_cloud/server.py
```

### Comparing `Pandora-Cloud-0.2.0/LICENSE` & `Pandora-Cloud-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/PKG-INFO` & `Pandora-Cloud-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-Cloud
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/pengzhile/pandora-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora-cloud
 Project-URL: Tracker, https://github.com/pengzhile/pandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `Pandora-Cloud-0.2.0/Pandora_Cloud.egg-info/PKG-INFO` & `Pandora-Cloud-0.2.1/Pandora_Cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-Cloud
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/pengzhile/pandora-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora-cloud
 Project-URL: Tracker, https://github.com/pengzhile/pandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `Pandora-Cloud-0.2.0/Pandora_Cloud.egg-info/SOURCES.txt` & `Pandora-Cloud-0.2.1/Pandora_Cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/README.md` & `Pandora-Cloud-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/setup.py` & `Pandora-Cloud-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/35uzIQibpwv56FyPcgmGz/_buildManifest.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/35uzIQibpwv56FyPcgmGz/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/259-3a89909da92e8e07.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/259-3a89909da92e8e07.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/2802bd5f-8ff236fd4fe2a08c.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/2802bd5f-8ff236fd4fe2a08c.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/58-f9da11f48bf979b2.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/58-f9da11f48bf979b2.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/734-d34f3efd388e555d.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/734-d34f3efd388e555d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3732,15 +3732,16 @@
 
             function tn(e) {
                 var n, t;
                 if (e.author.role === n5.uU.Assistant) {
                     if ("bing_search" === e.recipient) return u.SimpleBrowsing;
                     if ("browser" === e.recipient || "restricted_browser" === e.recipient) return u.Browsing;
                     if ("code" === e.content.content_type || "python" === e.recipient && "text" === e.content.content_type) return u.Code;
-                    if (null === (n = e.recipient) || void 0 === n ? void 0 : n.includes(".")) return u.Plugin
+                    if (null === (n = e.recipient) || void 0 === n ? void 0 : n.includes(".")) return u.Plugin;
+                    if ("text" === e.content.content_type) return u.Text
                 } else if (e.author.role === n5.uU.Tool) {
                     if ("bing_search" === e.author.name || "browser" === e.author.name || "restricted_browser" === e.author.name) return u.BrowseTool;
                     if ("execution_output" === e.content.content_type) return u.CodeExecutionOutput;
                     if ((null === (t = e.author.name) || void 0 === t ? void 0 : t.includes(".")) || "plugin_service" === e.author.name) return u.PluginTool
                 } else if ("text" === e.content.content_type) return u.Text;
                 return u.Unknown
             }(a = u || (u = {}))[a.Text = 0] = "Text", a[a.SimpleBrowsing = 1] = "SimpleBrowsing", a[a.Browsing = 2] = "Browsing", a[a.BrowseTool = 3] = "BrowseTool", a[a.Code = 4] = "Code", a[a.CodeExecutionOutput = 5] = "CodeExecutionOutput", a[a.Plugin = 6] = "Plugin", a[a.PluginTool = 7] = "PluginTool", a[a.Unknown = 8] = "Unknown";
@@ -4950,15 +4951,15 @@
                         }, [o]),
                         eE = (0, y.useMemo)(function() {
                             var e = [];
                             return A.forEach(function(n, t) {
                                 var r = tn(n.message),
                                     a = null == A ? void 0 : A[t - 1],
                                     i = a && (n4.Cv.getIsIncompleteFromMessage(a.message) || n4.Cv.getIsContinuedFromMessage(a.message)),
-                                    o = n4.Cv.getIsContinuedFromMessage(n.message),
+                                    o = n4.Cv.getIsContinuedFromMessage(n.message) || n.message.author.role === n5.uU.Assistant,
                                     s = r === u.Text && n4.Cv.getTextFromMessage(n.message);
                                 if (i && o && s) {
                                     var l = e.pop();
                                     (null == l ? void 0 : l.type) === c.MultiText ? (l.messages.push(n), e.push(l)) : (null == l ? void 0 : l.type) === c.Text && e.push({
                                         type: c.MultiText,
                                         messages: [l.message, n]
                                     })
```

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/791-87c69e21acb5fd01.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/791-87c69e21acb5fd01.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/_app-ab949dad0ea9d6e3.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/_app-ab949dad0ea9d6e3.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-67c7e2815007721d.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-67c7e2815007721d.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-73c3d3d7a4970449.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-73c3d3d7a4970449.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-78bcf9600a6bd4b9.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-78bcf9600a6bd4b9.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-2337d8baa604475c.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-2337d8baa604475c.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-a51bd7ac61420e8d.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-a51bd7ac61420e8d.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-31ac023eeccf1f5b.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-31ac023eeccf1f5b.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-b9488b953c4653c2.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-b9488b953c4653c2.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/chunks/webpack-febc072ffb3fcfd3.js` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/chunks/webpack-febc072ffb3fcfd3.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/_next/static/css/b389cdeaa663d62e.css` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/_next/static/css/b389cdeaa663d62e.css`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/apple-touch-icon.png` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/favicon-16x16.png` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/favicon-32x32.png` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/templates/chat.html` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/templates/detail.html` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/templates/detail.html`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/flask/templates/login.html` & `Pandora-Cloud-0.2.1/src/pandora_cloud/flask/templates/login.html`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.2.0/src/pandora_cloud/server.py` & `Pandora-Cloud-0.2.1/src/pandora_cloud/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,14 @@
                 'data_export_enabled',
                 'show_existing_user_age_confirmation_modal',
                 'bucketed_history',
                 'priority_driven_models_list',
                 'message_style_202305',
                 'layout_may_2023',
                 'plugins_available',
-                'new_model_switcher_20230512',
                 'beta_features',
                 'infinite_scroll_history',
                 'browsing_available',
                 'browsing_inner_monologue',
                 'tools3_dev',
                 'tools3_admin',
                 'tools2',
```

