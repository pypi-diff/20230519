# Comparing `tmp/giant-plugins-1.0.8.tar.gz` & `tmp/giant-plugins-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant-plugins-1.0.8.tar", max compression
+gzip compressed data, was "giant-plugins-1.0.9.tar", max compression
```

## Comparing `giant-plugins-1.0.8.tar` & `giant-plugins-1.0.9.tar`

### file list

```diff
@@ -1,279 +1,280 @@
--rw-r--r--   0        0        0     1069 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/LICENSE
--rw-r--r--   0        0        0     4278 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/README.md
--rw-r--r--   0        0        0       22 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/__init__.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_image/__init__.py
--rw-r--r--   0        0        0      397 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_image/cms_plugins.py
--rw-r--r--   0        0        0     1314 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_image/migrations/0001_initial.py
--rw-r--r--   0        0        0      407 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_image/migrations/0002_contentwidthimage_credit.py
--rw-r--r--   0        0        0      620 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_image/migrations/0003_auto_20220621_1127.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_image/migrations/__init__.py
--rw-r--r--   0        0        0      699 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_image/models.py
--rw-r--r--   0        0        0      643 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_image/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:24:53.333255 giant-plugins-1.0.8/giant_plugins/content_width_video/__init__.py
--rw-r--r--   0        0        0      411 2022-08-04 13:24:53.353256 giant-plugins-1.0.8/giant_plugins/content_width_video/cms_plugins.py
--rw-r--r--   0        0        0     2067 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0001_initial.py
--rw-r--r--   0        0        0      408 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0002_contentwidthvideo_caption.py
--rw-r--r--   0        0        0     1073 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0003_auto_20220621_1127.py
--rw-r--r--   0        0        0      683 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0004_alter_contentwidthvideo_image.py
--rw-r--r--   0        0        0      895 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0004_alter_contentwidthvideo_youtube_url.py
--rw-r--r--   0        0        0      366 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0005_remove_contentwidthvideo_alt_title.py
--rw-r--r--   0        0        0      331 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0006_merge_20220729_0931.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/__init__.py
--rw-r--r--   0        0        0     1264 2022-08-04 13:24:53.366589 giant-plugins-1.0.8/giant_plugins/content_width_video/models.py
--rw-r--r--   0        0        0      643 2022-08-04 13:24:53.373256 giant-plugins-1.0.8/giant_plugins/content_width_video/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/donate/__init__.py
--rw-r--r--   0        0        0      323 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/donate/cms_plugins.py
--rw-r--r--   0        0        0      966 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/donate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.801786 giant-plugins-1.0.8/giant_plugins/donate/migrations/__init__.py
--rw-r--r--   0        0        0      613 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/donate/models.py
--rw-r--r--   0        0        0      625 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/donate/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/featured_cta/__init__.py
--rw-r--r--   0        0        0      360 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/featured_cta/cms_plugins.py
--rw-r--r--   0        0        0     1561 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/featured_cta/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/featured_cta/migrations/__init__.py
--rw-r--r--   0        0        0      841 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/featured_cta/models.py
--rw-r--r--   0        0        0      539 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/featured_cta/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/gallery/__init__.py
--rw-r--r--   0        0        0      740 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/gallery/cms_plugins.py
--rw-r--r--   0        0        0     1895 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/gallery/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/gallery/migrations/__init__.py
--rw-r--r--   0        0        0     1237 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/gallery/models.py
--rw-r--r--   0        0        0      660 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/gallery/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/hero_image/__init__.py
--rw-r--r--   0        0        0      378 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/hero_image/cms_plugins.py
--rw-r--r--   0        0        0     2166 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/hero_image/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/hero_image/migrations/__init__.py
--rw-r--r--   0        0        0     1180 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/hero_image/models.py
--rw-r--r--   0        0        0      568 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/hero_image/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/key_stats/__init__.py
--rw-r--r--   0        0        0      803 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/key_stats/cms_plugins.py
--rw-r--r--   0        0        0     1318 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/key_stats/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/key_stats/migrations/__init__.py
--rw-r--r--   0        0        0      605 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/key_stats/models.py
--rw-r--r--   0        0        0      628 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/key_stats/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/logo_grid/__init__.py
--rw-r--r--   0        0        0      748 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/logo_grid/cms_plugins.py
--rw-r--r--   0        0        0     2205 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/logo_grid/migrations/0001_initial.py
--rw-r--r--   0        0        0      579 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/logo_grid/migrations/0002_auto_20220530_0356.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/logo_grid/migrations/__init__.py
--rw-r--r--   0        0        0      807 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/logo_grid/models.py
--rw-r--r--   0        0        0     1252 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/logo_grid/tests.py
--rw-r--r--   0        0        0      922 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/mixins.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/multilink/__init__.py
--rw-r--r--   0        0        0     1084 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/multilink/cms_plugins.py
--rw-r--r--   0        0        0     2460 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/multilink/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/multilink/migrations/__init__.py
--rw-r--r--   0        0        0     1297 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/multilink/models.py
--rw-r--r--   0        0        0      629 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/multilink/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/page_card/__init__.py
--rw-r--r--   0        0        0      782 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/page_card/cms_plugins.py
--rw-r--r--   0        0        0     2888 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/page_card/migrations/0001_initial.py
--rw-r--r--   0        0        0      389 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/page_card/migrations/0002_auto_20220701_0220.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/page_card/migrations/__init__.py
--rw-r--r--   0        0        0     1790 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/page_card/models.py
--rw-r--r--   0        0        0      824 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/page_card/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/pullquote/__init__.py
--rw-r--r--   0        0        0      722 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/pullquote/cms_plugins.py
--rw-r--r--   0        0        0     1656 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/pullquote/migrations/0001_initial.py
--rw-r--r--   0        0        0      631 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/pullquote/migrations/0002_auto_20220407_0921.py
--rw-r--r--   0        0        0      631 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/pullquote/migrations/0003_auto_20220530_0356.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/pullquote/migrations/__init__.py
--rw-r--r--   0        0        0     1052 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/pullquote/models.py
--rw-r--r--   0        0        0      829 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/pullquote/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/rich_text/__init__.py
--rw-r--r--   0        0        0      354 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/rich_text/cms_plugins.py
--rw-r--r--   0        0        0      839 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/rich_text/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/rich_text/migrations/__init__.py
--rw-r--r--   0        0        0      745 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/rich_text/models.py
--rw-r--r--   0        0        0     1464 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/rich_text/tests.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/share_this_page/__init__.py
--rw-r--r--   0        0        0      371 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/share_this_page/cms_plugins.py
--rw-r--r--   0        0        0     1355 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/share_this_page/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/share_this_page/migrations/__init__.py
--rw-r--r--   0        0        0      903 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/share_this_page/models.py
--rw-r--r--   0        0        0      353 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/share_this_page/tests.py
--rw-r--r--   0        0        0    12072 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/font/summernote.eot
--rw-r--r--   0        0        0    11896 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/font/summernote.ttf
--rw-r--r--   0        0        0     7428 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/font/summernote.woff
--rw-r--r--   0        0        0     6156 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/font/summernote.woff2
--rw-r--r--   0        0        0      662 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/init.js
--rw-r--r--   0        0        0    10345 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ar-AR.js
--rw-r--r--   0        0        0     5834 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ar-AR.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ar-AR.min.js.LICENSE.txt
--rw-r--r--   0        0        0    10075 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-az-AZ.js
--rw-r--r--   0        0        0     5268 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-az-AZ.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-az-AZ.min.js.LICENSE.txt
--rw-r--r--   0        0        0    10113 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-bg-BG.js
--rw-r--r--   0        0        0     5595 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-bg-BG.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-bg-BG.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9499 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ca-ES.js
--rw-r--r--   0        0        0     4981 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ca-ES.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ca-ES.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9138 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-cs-CZ.js
--rw-r--r--   0        0        0     4680 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-cs-CZ.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-cs-CZ.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9283 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-da-DK.js
--rw-r--r--   0        0        0     4775 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-da-DK.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-da-DK.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9324 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-de-DE.js
--rw-r--r--   0        0        0     4813 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-de-DE.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-de-DE.min.js.LICENSE.txt
--rw-r--r--   0        0        0    11728 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-el-GR.js
--rw-r--r--   0        0        0     7150 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-el-GR.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-el-GR.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9862 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-es-ES.js
--rw-r--r--   0        0        0     5348 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-es-ES.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-es-ES.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9329 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-es-EU.js
--rw-r--r--   0        0        0     4831 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-es-EU.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-es-EU.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9936 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fa-IR.js
--rw-r--r--   0        0        0     5428 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fa-IR.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fa-IR.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9188 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fi-FI.js
--rw-r--r--   0        0        0     4707 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fi-FI.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fi-FI.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9742 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fr-FR.js
--rw-r--r--   0        0        0     5236 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fr-FR.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fr-FR.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9444 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-gl-ES.js
--rw-r--r--   0        0        0     4943 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-gl-ES.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-gl-ES.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9533 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-he-IL.js
--rw-r--r--   0        0        0     5025 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-he-IL.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-he-IL.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9226 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-hr-HR.js
--rw-r--r--   0        0        0     4718 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-hr-HR.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-hr-HR.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9497 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-hu-HU.js
--rw-r--r--   0        0        0     4996 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-hu-HU.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-hu-HU.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9345 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-id-ID.js
--rw-r--r--   0        0        0     4844 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-id-ID.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-id-ID.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9520 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-it-IT.js
--rw-r--r--   0        0        0     5008 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-it-IT.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-it-IT.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9135 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ja-JP.js
--rw-r--r--   0        0        0     4634 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ja-JP.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ja-JP.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9652 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ko-KR.js
--rw-r--r--   0        0        0     5131 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ko-KR.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ko-KR.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9554 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-lt-LT.js
--rw-r--r--   0        0        0     5046 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-lt-LT.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-lt-LT.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9476 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-lt-LV.js
--rw-r--r--   0        0        0     5027 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-lt-LV.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-lt-LV.min.js.LICENSE.txt
--rw-r--r--   0        0        0    10233 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-mn-MN.js
--rw-r--r--   0        0        0     5681 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-mn-MN.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-mn-MN.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9252 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-nb-NO.js
--rw-r--r--   0        0        0     4761 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-nb-NO.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-nb-NO.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9393 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-nl-NL.js
--rw-r--r--   0        0        0     4892 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-nl-NL.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-nl-NL.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9366 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pl-PL.js
--rw-r--r--   0        0        0     4865 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pl-PL.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pl-PL.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9417 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pt-BR.js
--rw-r--r--   0        0        0     4906 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pt-BR.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pt-BR.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9539 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pt-PT.js
--rw-r--r--   0        0        0     5038 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pt-PT.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pt-PT.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9586 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ro-RO.js
--rw-r--r--   0        0        0     5085 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ro-RO.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ro-RO.min.js.LICENSE.txt
--rw-r--r--   0        0        0    11350 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ru-RU.js
--rw-r--r--   0        0        0     6849 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ru-RU.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ru-RU.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9319 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sk-SK.js
--rw-r--r--   0        0        0     4831 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sk-SK.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sk-SK.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9350 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sl-SI.js
--rw-r--r--   0        0        0     4842 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sl-SI.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sl-SI.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9236 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS-Latin.js
--rw-r--r--   0        0        0     4734 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS-Latin.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS-Latin.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9964 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS.js
--rw-r--r--   0        0        0     5456 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9258 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sv-SE.js
--rw-r--r--   0        0        0     4750 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sv-SE.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sv-SE.min.js.LICENSE.txt
--rw-r--r--   0        0        0    10939 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ta-IN.js
--rw-r--r--   0        0        0     6431 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ta-IN.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ta-IN.min.js.LICENSE.txt
--rw-r--r--   0        0        0    11554 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-th-TH.js
--rw-r--r--   0        0        0     7052 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-th-TH.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-th-TH.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9609 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-tr-TR.js
--rw-r--r--   0        0        0     5108 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-tr-TR.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-tr-TR.min.js.LICENSE.txt
--rw-r--r--   0        0        0    10369 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-uk-UA.js
--rw-r--r--   0        0        0     5861 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-uk-UA.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-uk-UA.min.js.LICENSE.txt
--rw-r--r--   0        0        0     8423 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-uz-UZ.js
--rw-r--r--   0        0        0     4394 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-uz-UZ.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-uz-UZ.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9186 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-vi-VN.js
--rw-r--r--   0        0        0     4678 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-vi-VN.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-vi-VN.min.js.LICENSE.txt
--rw-r--r--   0        0        0     8843 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-zh-CN.js
--rw-r--r--   0        0        0     4394 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-zh-CN.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-zh-CN.min.js.LICENSE.txt
--rw-r--r--   0        0        0     9072 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-zh-TW.js
--rw-r--r--   0        0        0     4564 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-zh-TW.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-zh-TW.min.js.LICENSE.txt
--rw-r--r--   0        0        0      254 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/plugin/databasic/summernote-ext-databasic.css
--rw-r--r--   0        0        0     8229 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/plugin/databasic/summernote-ext-databasic.js
--rw-r--r--   0        0        0     2596 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/plugin/hello/summernote-ext-hello.js
--rw-r--r--   0        0        0    10449 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/plugin/specialchars/summernote-ext-specialchars.js
--rw-r--r--   0        0        0    19673 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.css
--rw-r--r--   0        0        0   333315 2022-08-04 13:04:45.808453 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.js
--rw-r--r--   0        0        0   549157 2022-08-04 13:04:45.811786 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.js.map
--rw-r--r--   0        0        0    19403 2022-08-04 13:04:45.811786 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.min.css
--rw-r--r--   0        0        0   151398 2022-08-04 13:04:45.811786 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.811786 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.min.js.LICENSE.txt
--rw-r--r--   0        0        0   427683 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.min.js.map
--rw-r--r--   0        0        0    36901 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.css
--rw-r--r--   0        0        0   355299 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.js
--rw-r--r--   0        0        0   586663 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.js.map
--rw-r--r--   0        0        0    36184 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.min.css
--rw-r--r--   0        0        0   163197 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.min.js.LICENSE.txt
--rw-r--r--   0        0        0   456334 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.min.js.map
--rw-r--r--   0        0        0    19552 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.css
--rw-r--r--   0        0        0   332911 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.js
--rw-r--r--   0        0        0   548548 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.js.map
--rw-r--r--   0        0        0    19266 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.min.css
--rw-r--r--   0        0        0   151092 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.min.js
--rw-r--r--   0        0        0       85 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.min.js.LICENSE.txt
--rw-r--r--   0        0        0   427187 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.min.js.map
--rw-r--r--   0        0        0      744 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/templates/plugins/content_width_image.html
--rw-r--r--   0        0        0      680 2022-08-04 13:04:45.815119 giant-plugins-1.0.8/giant_plugins/templates/plugins/content_width_video.html
--rw-r--r--   0        0        0     1931 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/donate.html
--rw-r--r--   0        0        0      622 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/featured_cta.html
--rw-r--r--   0        0        0     1368 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/gallery/container.html
--rw-r--r--   0        0        0      529 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/gallery/item.html
--rw-r--r--   0        0        0     1009 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/hero_image.html
--rw-r--r--   0        0        0      136 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/key_stats/card.html
--rw-r--r--   0        0        0      356 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/key_stats/container.html
--rw-r--r--   0        0        0      433 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/logo_grid/container.html
--rw-r--r--   0        0        0      655 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/logo_grid/item.html
--rw-r--r--   0        0        0      353 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/multilink/card.html
--rw-r--r--   0        0        0      399 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/multilink/container.html
--rw-r--r--   0        0        0      463 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/page_card/container.html
--rw-r--r--   0        0        0      782 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/page_card/item.html
--rw-r--r--   0        0        0      680 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/pullquote/container.html
--rw-r--r--   0        0        0      145 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/pullquote/item.html
--rw-r--r--   0        0        0      328 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/rich_text.html
--rw-r--r--   0        0        0     7756 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/templates/plugins/share_this_page.html
--rw-r--r--   0        0        0     2968 2022-08-04 13:04:45.818453 giant-plugins-1.0.8/giant_plugins/utils.py
--rw-r--r--   0        0        0     1368 2022-08-04 13:26:40.673729 giant-plugins-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     6728 2022-08-04 13:28:37.263213 giant-plugins-1.0.8/setup.py
--rw-r--r--   0        0        0     5307 2022-08-04 13:28:37.263552 giant-plugins-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/LICENSE
+-rw-r--r--   0        0        0     4278 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/README.md
+-rw-r--r--   0        0        0       22 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_image/__init__.py
+-rw-r--r--   0        0        0      397 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_image/cms_plugins.py
+-rw-r--r--   0        0        0     1314 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_image/migrations/0001_initial.py
+-rw-r--r--   0        0        0      407 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_image/migrations/0002_contentwidthimage_credit.py
+-rw-r--r--   0        0        0      620 2022-09-15 08:12:33.959265 giant-plugins-1.0.9/giant_plugins/content_width_image/migrations/0003_auto_20220621_1127.py
+-rw-r--r--   0        0        0      675 2022-09-15 08:15:15.520387 giant-plugins-1.0.9/giant_plugins/content_width_image/migrations/0004_auto_20220915.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_image/migrations/__init__.py
+-rw-r--r--   0        0        0      748 2022-09-15 08:03:59.188786 giant-plugins-1.0.9/giant_plugins/content_width_image/models.py
+-rw-r--r--   0        0        0      643 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_image/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:24:53.333255 giant-plugins-1.0.9/giant_plugins/content_width_video/__init__.py
+-rw-r--r--   0        0        0      411 2022-08-04 13:24:53.353256 giant-plugins-1.0.9/giant_plugins/content_width_video/cms_plugins.py
+-rw-r--r--   0        0        0     2067 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0001_initial.py
+-rw-r--r--   0        0        0      408 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0002_contentwidthvideo_caption.py
+-rw-r--r--   0        0        0     1073 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0003_auto_20220621_1127.py
+-rw-r--r--   0        0        0      683 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0004_alter_contentwidthvideo_image.py
+-rw-r--r--   0        0        0      895 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0004_alter_contentwidthvideo_youtube_url.py
+-rw-r--r--   0        0        0      366 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0005_remove_contentwidthvideo_alt_title.py
+-rw-r--r--   0        0        0      331 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0006_merge_20220729_0931.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/__init__.py
+-rw-r--r--   0        0        0     1264 2022-09-15 08:15:49.750023 giant-plugins-1.0.9/giant_plugins/content_width_video/models.py
+-rw-r--r--   0        0        0      643 2022-08-04 13:24:53.373256 giant-plugins-1.0.9/giant_plugins/content_width_video/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/donate/__init__.py
+-rw-r--r--   0        0        0      323 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/donate/cms_plugins.py
+-rw-r--r--   0        0        0      966 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/donate/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.801786 giant-plugins-1.0.9/giant_plugins/donate/migrations/__init__.py
+-rw-r--r--   0        0        0      613 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/donate/models.py
+-rw-r--r--   0        0        0      625 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/donate/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/featured_cta/__init__.py
+-rw-r--r--   0        0        0      360 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/featured_cta/cms_plugins.py
+-rw-r--r--   0        0        0     1561 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/featured_cta/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/featured_cta/migrations/__init__.py
+-rw-r--r--   0        0        0      841 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/featured_cta/models.py
+-rw-r--r--   0        0        0      539 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/featured_cta/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/gallery/__init__.py
+-rw-r--r--   0        0        0      740 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/gallery/cms_plugins.py
+-rw-r--r--   0        0        0     1895 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/gallery/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/gallery/migrations/__init__.py
+-rw-r--r--   0        0        0     1237 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/gallery/models.py
+-rw-r--r--   0        0        0      660 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/gallery/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/hero_image/__init__.py
+-rw-r--r--   0        0        0      378 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/hero_image/cms_plugins.py
+-rw-r--r--   0        0        0     2166 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/hero_image/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/hero_image/migrations/__init__.py
+-rw-r--r--   0        0        0     1180 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/hero_image/models.py
+-rw-r--r--   0        0        0      568 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/hero_image/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/key_stats/__init__.py
+-rw-r--r--   0        0        0      803 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/key_stats/cms_plugins.py
+-rw-r--r--   0        0        0     1318 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/key_stats/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/key_stats/migrations/__init__.py
+-rw-r--r--   0        0        0      605 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/key_stats/models.py
+-rw-r--r--   0        0        0      628 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/key_stats/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/logo_grid/__init__.py
+-rw-r--r--   0        0        0      748 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/logo_grid/cms_plugins.py
+-rw-r--r--   0        0        0     2205 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/logo_grid/migrations/0001_initial.py
+-rw-r--r--   0        0        0      579 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/logo_grid/migrations/0002_auto_20220530_0356.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/logo_grid/migrations/__init__.py
+-rw-r--r--   0        0        0      807 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/logo_grid/models.py
+-rw-r--r--   0        0        0     1252 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/logo_grid/tests.py
+-rw-r--r--   0        0        0      922 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/mixins.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/multilink/__init__.py
+-rw-r--r--   0        0        0     1084 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/multilink/cms_plugins.py
+-rw-r--r--   0        0        0     2460 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/multilink/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/multilink/migrations/__init__.py
+-rw-r--r--   0        0        0     1297 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/multilink/models.py
+-rw-r--r--   0        0        0      629 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/multilink/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/page_card/__init__.py
+-rw-r--r--   0        0        0      782 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/page_card/cms_plugins.py
+-rw-r--r--   0        0        0     2888 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/page_card/migrations/0001_initial.py
+-rw-r--r--   0        0        0      389 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/page_card/migrations/0002_auto_20220701_0220.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/page_card/migrations/__init__.py
+-rw-r--r--   0        0        0     1790 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/page_card/models.py
+-rw-r--r--   0        0        0      824 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/page_card/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/pullquote/__init__.py
+-rw-r--r--   0        0        0      722 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/pullquote/cms_plugins.py
+-rw-r--r--   0        0        0     1656 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/pullquote/migrations/0001_initial.py
+-rw-r--r--   0        0        0      631 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/pullquote/migrations/0002_auto_20220407_0921.py
+-rw-r--r--   0        0        0      631 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/pullquote/migrations/0003_auto_20220530_0356.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/pullquote/migrations/__init__.py
+-rw-r--r--   0        0        0     1052 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/pullquote/models.py
+-rw-r--r--   0        0        0      829 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/pullquote/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/rich_text/__init__.py
+-rw-r--r--   0        0        0      354 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/rich_text/cms_plugins.py
+-rw-r--r--   0        0        0      839 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/rich_text/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/rich_text/migrations/__init__.py
+-rw-r--r--   0        0        0      745 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/rich_text/models.py
+-rw-r--r--   0        0        0     1464 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/rich_text/tests.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/share_this_page/__init__.py
+-rw-r--r--   0        0        0      371 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/share_this_page/cms_plugins.py
+-rw-r--r--   0        0        0     1355 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/share_this_page/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/share_this_page/migrations/__init__.py
+-rw-r--r--   0        0        0      903 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/share_this_page/models.py
+-rw-r--r--   0        0        0      353 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/share_this_page/tests.py
+-rw-r--r--   0        0        0    12072 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/font/summernote.eot
+-rw-r--r--   0        0        0    11896 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/font/summernote.ttf
+-rw-r--r--   0        0        0     7428 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/font/summernote.woff
+-rw-r--r--   0        0        0     6156 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/font/summernote.woff2
+-rw-r--r--   0        0        0      662 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/init.js
+-rw-r--r--   0        0        0    10345 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ar-AR.js
+-rw-r--r--   0        0        0     5834 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ar-AR.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ar-AR.min.js.LICENSE.txt
+-rw-r--r--   0        0        0    10075 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-az-AZ.js
+-rw-r--r--   0        0        0     5268 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-az-AZ.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-az-AZ.min.js.LICENSE.txt
+-rw-r--r--   0        0        0    10113 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-bg-BG.js
+-rw-r--r--   0        0        0     5595 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-bg-BG.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-bg-BG.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9499 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ca-ES.js
+-rw-r--r--   0        0        0     4981 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ca-ES.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ca-ES.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9138 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-cs-CZ.js
+-rw-r--r--   0        0        0     4680 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-cs-CZ.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-cs-CZ.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9283 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-da-DK.js
+-rw-r--r--   0        0        0     4775 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-da-DK.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-da-DK.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9324 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-de-DE.js
+-rw-r--r--   0        0        0     4813 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-de-DE.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-de-DE.min.js.LICENSE.txt
+-rw-r--r--   0        0        0    11728 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-el-GR.js
+-rw-r--r--   0        0        0     7150 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-el-GR.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-el-GR.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9862 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-es-ES.js
+-rw-r--r--   0        0        0     5348 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-es-ES.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-es-ES.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9329 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-es-EU.js
+-rw-r--r--   0        0        0     4831 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-es-EU.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-es-EU.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9936 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fa-IR.js
+-rw-r--r--   0        0        0     5428 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fa-IR.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fa-IR.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9188 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fi-FI.js
+-rw-r--r--   0        0        0     4707 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fi-FI.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fi-FI.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9742 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fr-FR.js
+-rw-r--r--   0        0        0     5236 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fr-FR.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fr-FR.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9444 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-gl-ES.js
+-rw-r--r--   0        0        0     4943 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-gl-ES.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-gl-ES.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9533 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-he-IL.js
+-rw-r--r--   0        0        0     5025 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-he-IL.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-he-IL.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9226 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-hr-HR.js
+-rw-r--r--   0        0        0     4718 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-hr-HR.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-hr-HR.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9497 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-hu-HU.js
+-rw-r--r--   0        0        0     4996 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-hu-HU.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-hu-HU.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9345 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-id-ID.js
+-rw-r--r--   0        0        0     4844 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-id-ID.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-id-ID.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9520 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-it-IT.js
+-rw-r--r--   0        0        0     5008 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-it-IT.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-it-IT.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9135 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ja-JP.js
+-rw-r--r--   0        0        0     4634 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ja-JP.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.805119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ja-JP.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9652 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ko-KR.js
+-rw-r--r--   0        0        0     5131 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ko-KR.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ko-KR.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9554 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-lt-LT.js
+-rw-r--r--   0        0        0     5046 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-lt-LT.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-lt-LT.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9476 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-lt-LV.js
+-rw-r--r--   0        0        0     5027 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-lt-LV.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-lt-LV.min.js.LICENSE.txt
+-rw-r--r--   0        0        0    10233 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-mn-MN.js
+-rw-r--r--   0        0        0     5681 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-mn-MN.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-mn-MN.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9252 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-nb-NO.js
+-rw-r--r--   0        0        0     4761 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-nb-NO.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-nb-NO.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9393 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-nl-NL.js
+-rw-r--r--   0        0        0     4892 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-nl-NL.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-nl-NL.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9366 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pl-PL.js
+-rw-r--r--   0        0        0     4865 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pl-PL.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pl-PL.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9417 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pt-BR.js
+-rw-r--r--   0        0        0     4906 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pt-BR.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pt-BR.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9539 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pt-PT.js
+-rw-r--r--   0        0        0     5038 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pt-PT.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pt-PT.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9586 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ro-RO.js
+-rw-r--r--   0        0        0     5085 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ro-RO.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ro-RO.min.js.LICENSE.txt
+-rw-r--r--   0        0        0    11350 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ru-RU.js
+-rw-r--r--   0        0        0     6849 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ru-RU.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ru-RU.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9319 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sk-SK.js
+-rw-r--r--   0        0        0     4831 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sk-SK.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sk-SK.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9350 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sl-SI.js
+-rw-r--r--   0        0        0     4842 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sl-SI.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sl-SI.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9236 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS-Latin.js
+-rw-r--r--   0        0        0     4734 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS-Latin.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS-Latin.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9964 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS.js
+-rw-r--r--   0        0        0     5456 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9258 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sv-SE.js
+-rw-r--r--   0        0        0     4750 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sv-SE.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sv-SE.min.js.LICENSE.txt
+-rw-r--r--   0        0        0    10939 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ta-IN.js
+-rw-r--r--   0        0        0     6431 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ta-IN.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ta-IN.min.js.LICENSE.txt
+-rw-r--r--   0        0        0    11554 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-th-TH.js
+-rw-r--r--   0        0        0     7052 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-th-TH.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-th-TH.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9609 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-tr-TR.js
+-rw-r--r--   0        0        0     5108 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-tr-TR.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-tr-TR.min.js.LICENSE.txt
+-rw-r--r--   0        0        0    10369 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-uk-UA.js
+-rw-r--r--   0        0        0     5861 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-uk-UA.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-uk-UA.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     8423 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-uz-UZ.js
+-rw-r--r--   0        0        0     4394 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-uz-UZ.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-uz-UZ.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9186 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-vi-VN.js
+-rw-r--r--   0        0        0     4678 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-vi-VN.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-vi-VN.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     8843 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-zh-CN.js
+-rw-r--r--   0        0        0     4394 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-zh-CN.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-zh-CN.min.js.LICENSE.txt
+-rw-r--r--   0        0        0     9072 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-zh-TW.js
+-rw-r--r--   0        0        0     4564 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-zh-TW.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-zh-TW.min.js.LICENSE.txt
+-rw-r--r--   0        0        0      254 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/plugin/databasic/summernote-ext-databasic.css
+-rw-r--r--   0        0        0     8229 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/plugin/databasic/summernote-ext-databasic.js
+-rw-r--r--   0        0        0     2596 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/plugin/hello/summernote-ext-hello.js
+-rw-r--r--   0        0        0    10449 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/plugin/specialchars/summernote-ext-specialchars.js
+-rw-r--r--   0        0        0    19673 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.css
+-rw-r--r--   0        0        0   333315 2022-08-04 13:04:45.808453 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.js
+-rw-r--r--   0        0        0   549157 2022-08-04 13:04:45.811786 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.js.map
+-rw-r--r--   0        0        0    19403 2022-08-04 13:04:45.811786 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.min.css
+-rw-r--r--   0        0        0   151398 2022-08-04 13:04:45.811786 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.811786 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.min.js.LICENSE.txt
+-rw-r--r--   0        0        0   427683 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.min.js.map
+-rw-r--r--   0        0        0    36901 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.css
+-rw-r--r--   0        0        0   355299 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.js
+-rw-r--r--   0        0        0   586663 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.js.map
+-rw-r--r--   0        0        0    36184 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.min.css
+-rw-r--r--   0        0        0   163197 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.min.js.LICENSE.txt
+-rw-r--r--   0        0        0   456334 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.min.js.map
+-rw-r--r--   0        0        0    19552 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.css
+-rw-r--r--   0        0        0   332911 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.js
+-rw-r--r--   0        0        0   548548 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.js.map
+-rw-r--r--   0        0        0    19266 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.min.css
+-rw-r--r--   0        0        0   151092 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.min.js
+-rw-r--r--   0        0        0       85 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.min.js.LICENSE.txt
+-rw-r--r--   0        0        0   427187 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.min.js.map
+-rw-r--r--   0        0        0      744 2022-08-04 13:04:45.815119 giant-plugins-1.0.9/giant_plugins/templates/plugins/content_width_image.html
+-rw-r--r--   0        0        0      680 2022-09-05 15:06:13.006145 giant-plugins-1.0.9/giant_plugins/templates/plugins/content_width_video.html
+-rw-r--r--   0        0        0     1931 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/donate.html
+-rw-r--r--   0        0        0      622 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/featured_cta.html
+-rw-r--r--   0        0        0     1368 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/gallery/container.html
+-rw-r--r--   0        0        0      529 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/gallery/item.html
+-rw-r--r--   0        0        0     1009 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/hero_image.html
+-rw-r--r--   0        0        0      136 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/key_stats/card.html
+-rw-r--r--   0        0        0      356 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/key_stats/container.html
+-rw-r--r--   0        0        0      433 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/logo_grid/container.html
+-rw-r--r--   0        0        0      655 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/logo_grid/item.html
+-rw-r--r--   0        0        0      353 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/multilink/card.html
+-rw-r--r--   0        0        0      399 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/multilink/container.html
+-rw-r--r--   0        0        0      463 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/page_card/container.html
+-rw-r--r--   0        0        0      782 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/page_card/item.html
+-rw-r--r--   0        0        0      680 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/pullquote/container.html
+-rw-r--r--   0        0        0      145 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/pullquote/item.html
+-rw-r--r--   0        0        0      328 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/rich_text.html
+-rw-r--r--   0        0        0     7756 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/templates/plugins/share_this_page.html
+-rw-r--r--   0        0        0     2968 2022-08-04 13:04:45.818453 giant-plugins-1.0.9/giant_plugins/utils.py
+-rw-r--r--   0        0        0     1368 2022-09-15 08:18:08.425519 giant-plugins-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6732 1970-01-01 00:00:00.000000 giant-plugins-1.0.9/setup.py
+-rw-r--r--   0        0        0     5307 1970-01-01 00:00:00.000000 giant-plugins-1.0.9/PKG-INFO
```

### Comparing `giant-plugins-1.0.8/LICENSE` & `giant-plugins-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/README.md` & `giant-plugins-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/content_width_image/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/content_width_image/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/content_width_image/migrations/0003_auto_20220621_1127.py` & `giant-plugins-1.0.9/giant_plugins/content_width_image/migrations/0003_auto_20220621_1127.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/content_width_image/models.py` & `giant-plugins-1.0.9/giant_plugins/content_width_image/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from django.db import models
-
 from cms.models import CMSPlugin
+from django.db import models
 from filer.fields.image import FilerImageField
 
 
 class ContentWidthImage(CMSPlugin):
     """
     Represents an image object
     """
 
     image = FilerImageField(
-        related_name="+", verbose_name="Content Width Image", on_delete=models.SET_NULL, null=True,
+        related_name="+",
+        verbose_name="Content Width Image",
+        on_delete=models.SET_NULL,
+        null=True,
+    )
+    caption = models.CharField(
+        max_length=255, help_text="Add a caption to the image", blank=True, default=""
     )
-    alt_text = models.CharField(max_length=64, help_text="Image name", blank=True, default="")
-    caption = models.CharField(max_length=255, help_text="Add a caption to the image")
+    alt_text = models.CharField(max_length=64, help_text="Image name", default="")
     credit = models.CharField(max_length=255)
 
     def __str__(self):
         """
         String representation of the object
         """
         return f"Content Width Image {self.pk}"
```

### Comparing `giant-plugins-1.0.8/giant_plugins/content_width_image/tests.py` & `giant-plugins-1.0.9/giant_plugins/content_width_image/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0003_auto_20220621_1127.py` & `giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0003_auto_20220621_1127.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0004_alter_contentwidthvideo_image.py` & `giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0004_alter_contentwidthvideo_image.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/content_width_video/migrations/0004_alter_contentwidthvideo_youtube_url.py` & `giant-plugins-1.0.9/giant_plugins/content_width_video/migrations/0004_alter_contentwidthvideo_youtube_url.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/content_width_video/models.py` & `giant-plugins-1.0.9/giant_plugins/content_width_video/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/content_width_video/tests.py` & `giant-plugins-1.0.9/giant_plugins/content_width_video/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/donate/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/donate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/donate/models.py` & `giant-plugins-1.0.9/giant_plugins/donate/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/donate/tests.py` & `giant-plugins-1.0.9/giant_plugins/donate/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/featured_cta/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/featured_cta/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/featured_cta/models.py` & `giant-plugins-1.0.9/giant_plugins/featured_cta/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/featured_cta/tests.py` & `giant-plugins-1.0.9/giant_plugins/featured_cta/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/gallery/cms_plugins.py` & `giant-plugins-1.0.9/giant_plugins/gallery/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/gallery/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/gallery/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/gallery/models.py` & `giant-plugins-1.0.9/giant_plugins/gallery/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/gallery/tests.py` & `giant-plugins-1.0.9/giant_plugins/gallery/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/hero_image/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/hero_image/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/hero_image/models.py` & `giant-plugins-1.0.9/giant_plugins/hero_image/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/hero_image/tests.py` & `giant-plugins-1.0.9/giant_plugins/hero_image/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/key_stats/cms_plugins.py` & `giant-plugins-1.0.9/giant_plugins/key_stats/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/key_stats/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/key_stats/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/key_stats/models.py` & `giant-plugins-1.0.9/giant_plugins/key_stats/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/key_stats/tests.py` & `giant-plugins-1.0.9/giant_plugins/key_stats/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/logo_grid/cms_plugins.py` & `giant-plugins-1.0.9/giant_plugins/logo_grid/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/logo_grid/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/logo_grid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/logo_grid/migrations/0002_auto_20220530_0356.py` & `giant-plugins-1.0.9/giant_plugins/logo_grid/migrations/0002_auto_20220530_0356.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/logo_grid/models.py` & `giant-plugins-1.0.9/giant_plugins/logo_grid/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/logo_grid/tests.py` & `giant-plugins-1.0.9/giant_plugins/logo_grid/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/mixins.py` & `giant-plugins-1.0.9/giant_plugins/mixins.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/multilink/cms_plugins.py` & `giant-plugins-1.0.9/giant_plugins/multilink/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/multilink/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/multilink/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/multilink/models.py` & `giant-plugins-1.0.9/giant_plugins/multilink/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/multilink/tests.py` & `giant-plugins-1.0.9/giant_plugins/multilink/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/page_card/cms_plugins.py` & `giant-plugins-1.0.9/giant_plugins/page_card/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/page_card/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/page_card/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/page_card/models.py` & `giant-plugins-1.0.9/giant_plugins/page_card/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/page_card/tests.py` & `giant-plugins-1.0.9/giant_plugins/page_card/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/pullquote/cms_plugins.py` & `giant-plugins-1.0.9/giant_plugins/pullquote/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/pullquote/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/pullquote/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/pullquote/migrations/0002_auto_20220407_0921.py` & `giant-plugins-1.0.9/giant_plugins/pullquote/migrations/0002_auto_20220407_0921.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/pullquote/migrations/0003_auto_20220530_0356.py` & `giant-plugins-1.0.9/giant_plugins/pullquote/migrations/0003_auto_20220530_0356.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/pullquote/models.py` & `giant-plugins-1.0.9/giant_plugins/pullquote/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/pullquote/tests.py` & `giant-plugins-1.0.9/giant_plugins/pullquote/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/rich_text/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/rich_text/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/rich_text/models.py` & `giant-plugins-1.0.9/giant_plugins/rich_text/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/rich_text/tests.py` & `giant-plugins-1.0.9/giant_plugins/rich_text/tests.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/share_this_page/migrations/0001_initial.py` & `giant-plugins-1.0.9/giant_plugins/share_this_page/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/share_this_page/models.py` & `giant-plugins-1.0.9/giant_plugins/share_this_page/models.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/font/summernote.eot` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/font/summernote.eot`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/font/summernote.ttf` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/font/summernote.ttf`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/font/summernote.woff` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/font/summernote.woff`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/font/summernote.woff2` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/font/summernote.woff2`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/init.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/init.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ar-AR.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ar-AR.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ar-AR.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ar-AR.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-az-AZ.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-az-AZ.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-az-AZ.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-az-AZ.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-bg-BG.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-bg-BG.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-bg-BG.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-bg-BG.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ca-ES.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ca-ES.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ca-ES.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ca-ES.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-cs-CZ.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-cs-CZ.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-cs-CZ.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-cs-CZ.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-da-DK.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-da-DK.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-da-DK.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-da-DK.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-de-DE.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-de-DE.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-de-DE.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-de-DE.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-el-GR.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-el-GR.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-el-GR.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-el-GR.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-es-ES.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-es-ES.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-es-ES.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-es-ES.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-es-EU.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-es-EU.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-es-EU.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-es-EU.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fa-IR.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fa-IR.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fa-IR.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fa-IR.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fi-FI.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fi-FI.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fi-FI.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fi-FI.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fr-FR.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fr-FR.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-fr-FR.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-fr-FR.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-gl-ES.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-gl-ES.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-gl-ES.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-gl-ES.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-he-IL.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-he-IL.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-he-IL.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-he-IL.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-hr-HR.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-hr-HR.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-hr-HR.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-hr-HR.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-hu-HU.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-hu-HU.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-hu-HU.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-hu-HU.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-id-ID.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-id-ID.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-id-ID.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-id-ID.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-it-IT.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-it-IT.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-it-IT.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-it-IT.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ja-JP.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ja-JP.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ja-JP.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ja-JP.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ko-KR.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ko-KR.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ko-KR.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ko-KR.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-lt-LT.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-lt-LT.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-lt-LT.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-lt-LT.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-lt-LV.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-lt-LV.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-lt-LV.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-lt-LV.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-mn-MN.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-mn-MN.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-mn-MN.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-mn-MN.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-nb-NO.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-nb-NO.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-nb-NO.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-nb-NO.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-nl-NL.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-nl-NL.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-nl-NL.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-nl-NL.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pl-PL.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pl-PL.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pl-PL.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pl-PL.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pt-BR.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pt-BR.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pt-BR.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pt-BR.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pt-PT.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pt-PT.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-pt-PT.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-pt-PT.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ro-RO.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ro-RO.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ro-RO.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ro-RO.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ru-RU.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ru-RU.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ru-RU.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ru-RU.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sk-SK.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sk-SK.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sk-SK.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sk-SK.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sl-SI.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sl-SI.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sl-SI.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sl-SI.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS-Latin.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS-Latin.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS-Latin.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS-Latin.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sr-RS.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sv-SE.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sv-SE.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-sv-SE.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-sv-SE.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ta-IN.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ta-IN.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-ta-IN.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-ta-IN.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-th-TH.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-th-TH.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-th-TH.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-th-TH.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-tr-TR.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-tr-TR.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-tr-TR.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-tr-TR.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-uk-UA.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-uk-UA.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-uk-UA.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-uk-UA.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-uz-UZ.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-uz-UZ.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-uz-UZ.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-uz-UZ.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-vi-VN.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-vi-VN.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-vi-VN.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-vi-VN.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-zh-CN.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-zh-CN.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-zh-CN.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-zh-CN.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-zh-TW.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-zh-TW.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/lang/summernote-zh-TW.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/lang/summernote-zh-TW.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/plugin/databasic/summernote-ext-databasic.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/plugin/databasic/summernote-ext-databasic.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/plugin/hello/summernote-ext-hello.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/plugin/hello/summernote-ext-hello.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/plugin/specialchars/summernote-ext-specialchars.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/plugin/specialchars/summernote-ext-specialchars.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.css` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.css`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.js.map` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.js.map`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.min.css` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.min.css`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-bs4.min.js.map` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-bs4.min.js.map`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.css` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.css`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.js.map` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.js.map`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.min.css` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.min.css`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote-lite.min.js.map` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote-lite.min.js.map`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.css` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.css`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.js.map` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.js.map`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.min.css` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.min.css`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.min.js` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.min.js`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/static/vendor/summernote/summernote.min.js.map` & `giant-plugins-1.0.9/giant_plugins/static/vendor/summernote/summernote.min.js.map`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/content_width_image.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/content_width_image.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/content_width_video.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/content_width_video.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/donate.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/donate.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/featured_cta.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/featured_cta.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/gallery/container.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/gallery/container.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/gallery/item.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/gallery/item.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/hero_image.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/hero_image.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/logo_grid/item.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/logo_grid/item.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/page_card/item.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/page_card/item.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/pullquote/container.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/pullquote/container.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/templates/plugins/share_this_page.html` & `giant-plugins-1.0.9/giant_plugins/templates/plugins/share_this_page.html`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/giant_plugins/utils.py` & `giant-plugins-1.0.9/giant_plugins/utils.py`

 * *Files identical despite different names*

### Comparing `giant-plugins-1.0.8/pyproject.toml` & `giant-plugins-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-plugins"
-version = "1.0.8"
+version = "1.0.9"
 description = "Adds a generic list of plugins for use within projects"
 authors = ["Will-Hoey <will.hoey@giantdigital.co.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-plugins"
 repository = "https://github.com/giantmade/giant-plugins"
 keywords = ["plugins", "app"]
```

### Comparing `giant-plugins-1.0.8/setup.py` & `giant-plugins-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,21 @@
                    'templates/plugins/pullquote/*']}
 
 install_requires = \
 ['django-filer', 'giant-mixins']
 
 setup_kwargs = {
     'name': 'giant-plugins',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'Adds a generic list of plugins for use within projects',
     'long_description': '# Giant Plugins\n\nA re-usable package which can be used in any project that requires a base set of plugins. \n\nThis will include a small set of plugins that are used in a large number of projects, but will not necessarily cover the full requirements. It will also provide a RichText field which can be used in other areas of the project\nThe RichText field uses ![summernote](https://github.com/summernote/summernote/) for styling the WYSIWYG widget.\n\n\nSupported Django versions:\n\n- Django 2.2, 3.2\n\nSupported django CMS versions:\n\n- django CMS 3.8, 3.9\n\n> &#x26a0;&#xfe0f; Release 1.0.0 and above are NOT compatible with\n> versions < 1 due to model name changes and a migration reset. Only upgrade to\n> this version if you are aware of what changes need to be made\n\n## Installation\n\nTo install with the package manager, run:\n\n    $ poetry add giant-plugins\n\nYou should then add `"giant_plugins"` to the `INSTALLED_APPS` in `base.py`. Move to "C \n\nThe structure of these files is slightly different than the norm, allowing for more control\nover which plugins are added to the Django project. In order to add the plugins it is\nadvised to create a `PLUGINS` variable in your settings file which will be appended to the\n`INSTALLED_APPS`. The following snippet will install all of the currently available plugins (note that this should be tweaked to suit your needs):\n\n```\nPLUGINS = [\n    "giant_plugins.content_width_image",\n    "giant_plugins.content_width_video",\n    "giant_plugins.donate",\n    "giant_plugins.featured_cta",\n    "giant_plugins.hero_image",\n    "giant_plugins.logo_grid",\n    "giant_plugins.page_card",\n    "giant_plugins.pullquote",\n    "giant_plugins.rich_text",\n    "giant_plugins.share_this_page",\n    "giant_plugins.gallery",\n    "giant_plugins.key_stats",\n    "giant_plugins.multilink",\n]\n\nINSTALLED_APPS = [...] + PLUGINS\n```\nOnce these have been added as such you can now run the `migrate` command and create the tables for the\ninstalled plugins.\n\n## Configuration\n\nIf you do not have a default WYSIWYG config then you can use the following settings:\n\n```\nSUMMERNOTE_CONFIG = (\n    {\n        "iframe": True,\n        "summernote": {\n            "airMode": False,\n            # Change editor size\n            "width": "100%",\n            "height": "480",\n            "lang": None,\n            "toolbar": [\n                ["style", ["style"]],\n                ["font", ["bold", "underline", "clear"]],\n                ["fontname", ["fontname"]],\n                ["color", ["color"]],\n                ["para", ["ul", "ol", "paragraph"]],\n                ["table", ["table"]],\n                ["insert", ["link", "picture", "video"]],\n                ["view", ["fullscreen", "codeview", "help"]],\n            ],\n        },\n    },\n)\n\n```\n\nIn order to specify a form to use for a specific plugin you should add something like this to your settings file:\n\n```\n<PLUGIN_NAME>_FORM = "<path.to.form.FormClass>"\n```\n\nWhere PLUGIN_NAME is the capitalised name of the plugin (e.g `TEXTWITHIMAGEPLUGIN_FORM`) and the path to the form class as a string so it can be imported.\n\n## Local development\n\nIn order to run `django-admin` commands you will need to set the `DJANGO_SETTINGS_MODULE` variable by running\n\n    $ export DJANGO_SETTINGS_MODULE=settings\n\nWhen adding a plugin you should add the new plugin to the `PLUGINS` variable in your settings file\nand to this README.\n\n\n\n ## Preparing for release\n \n In order to prep the package for a new release on TestPyPi and PyPi there is one key thing that you need to do. You need to update the version number in the `pyproject.toml`.\n This is so that the package can be published without running into version number conflicts. The version numbering must also follow the Semantic Version rules which can be found here https://semver.org/.\n \n \n ## Publishing\n \n Publishing a package with poetry is incredibly easy. Once you have checked that the version number has been updated (not the same as a previous version) then you only need to run two commands.\n \n    $ `poetry build` \n\nwill package the project up for you into a way that can be published.\n \n    $ `poetry publish`\n\nwill publish the package to PyPi. You will need to enter the username and password for the account which can be found in the company password manager\n',
     'author': 'Will-Hoey',
     'author_email': 'will.hoey@giantdigital.co.uk',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/giantmade/giant-plugins',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `giant-plugins-1.0.8/PKG-INFO` & `giant-plugins-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: giant-plugins
-Version: 1.0.8
+Version: 1.0.9
 Summary: Adds a generic list of plugins for use within projects
 Home-page: https://github.com/giantmade/giant-plugins
 License: MIT
 Keywords: plugins,app
 Author: Will-Hoey
 Author-email: will.hoey@giantdigital.co.uk
 Requires-Python: >=3.6,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django-filer
 Requires-Dist: giant-mixins
 Project-URL: Repository, https://github.com/giantmade/giant-plugins
 Description-Content-Type: text/markdown
```

