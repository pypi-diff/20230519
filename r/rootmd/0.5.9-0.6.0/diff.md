# Comparing `tmp/rootmd-0.5.9.tar.gz` & `tmp/rootmd-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootmd-0.5.9.tar", max compression
+gzip compressed data, was "rootmd-0.6.0.tar", max compression
```

## Comparing `rootmd-0.5.9.tar` & `rootmd-0.6.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1075 2023-02-06 15:24:37.795290 rootmd-0.5.9/LICENSE
--rw-r--r--   0        0        0     7097 2023-05-04 21:09:52.165241 rootmd-0.5.9/README.md
--rw-r--r--   0        0        0      757 2023-05-04 21:10:05.709372 rootmd-0.5.9/pyproject.toml
--rw-r--r--   0        0        0     3676 2023-05-04 21:10:01.814479 rootmd-0.5.9/rootmd/Executor.py
--rw-r--r--   0        0        0     4796 2023-02-06 15:24:37.988540 rootmd-0.5.9/rootmd/Md2MacroRenderer.py
--rw-r--r--   0        0        0     2866 2023-02-06 15:24:38.045297 rootmd-0.5.9/rootmd/RootBaseRenderer.py
--rw-r--r--   0        0        0    20986 2023-02-06 15:24:37.997268 rootmd-0.5.9/rootmd/RootHtmlRenderer.py
--rw-r--r--   0        0        0     4077 2023-04-29 21:16:18.592024 rootmd-0.5.9/rootmd/RootMdRenderer.py
--rw-r--r--   0        0        0     6549 2023-02-06 15:24:37.989078 rootmd-0.5.9/rootmd/YamlBlock.py
--rw-r--r--   0        0        0      531 2023-02-06 15:24:37.989478 rootmd-0.5.9/rootmd/__init__.py
--rwxr-xr-x   0        0        0     8821 2023-05-04 21:05:23.511213 rootmd-0.5.9/rootmd/__main__.py
--rw-r--r--   0        0        0     1130 2023-02-06 15:24:38.019160 rootmd-0.5.9/rootmd/data/css/core.css
--rw-r--r--   0        0        0     2438 2023-02-06 15:24:38.000040 rootmd-0.5.9/rootmd/data/css/prismjs/prism-a11y-dark.css
--rw-r--r--   0        0        0     1945 2023-02-06 15:24:38.011657 rootmd-0.5.9/rootmd/data/css/prismjs/prism-atom-dark.css
--rw-r--r--   0        0        0     3332 2023-02-06 15:24:38.013757 rootmd-0.5.9/rootmd/data/css/prismjs/prism-base16-ateliersulphurpool.light.css
--rw-r--r--   0        0        0     2618 2023-02-06 15:24:38.015816 rootmd-0.5.9/rootmd/data/css/prismjs/prism-cb.css
--rw-r--r--   0        0        0     6782 2023-02-06 15:24:38.018137 rootmd-0.5.9/rootmd/data/css/prismjs/prism-coldark-cold.css
--rw-r--r--   0        0        0     6776 2023-02-06 15:24:38.002562 rootmd-0.5.9/rootmd/data/css/prismjs/prism-coldark-dark.css
--rw-r--r--   0        0        0     2306 2023-02-06 15:24:38.006485 rootmd-0.5.9/rootmd/data/css/prismjs/prism-coy-without-shadows.css
--rw-r--r--   0        0        0     4031 2023-02-06 15:24:38.006001 rootmd-0.5.9/rootmd/data/css/prismjs/prism-coy.css
--rw-r--r--   0        0        0     3062 2023-02-06 15:24:38.012747 rootmd-0.5.9/rootmd/data/css/prismjs/prism-coy.min.css
--rw-r--r--   0        0        0     2680 2023-02-06 15:24:38.012408 rootmd-0.5.9/rootmd/data/css/prismjs/prism-darcula.css
--rw-r--r--   0        0        0     2070 2023-02-06 15:24:38.009811 rootmd-0.5.9/rootmd/data/css/prismjs/prism-dark.css
--rw-r--r--   0        0        0     1533 2023-02-06 15:24:38.002247 rootmd-0.5.9/rootmd/data/css/prismjs/prism-dark.min.css
--rw-r--r--   0        0        0     1795 2023-02-06 15:24:38.006828 rootmd-0.5.9/rootmd/data/css/prismjs/prism-dracula.css
--rw-r--r--   0        0        0     3389 2023-02-06 15:24:38.016149 rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-dark.css
--rw-r--r--   0        0        0     3390 2023-02-06 15:24:38.018512 rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-earth.css
--rw-r--r--   0        0        0     3395 2023-02-06 15:24:38.005334 rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-forest.css
--rw-r--r--   0        0        0     3380 2023-02-06 15:24:37.999330 rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-light.css
--rw-r--r--   0        0        0     3398 2023-02-06 15:24:38.015165 rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-sea.css
--rw-r--r--   0        0        0     3388 2023-02-06 15:24:38.013409 rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-space.css
--rw-r--r--   0        0        0     2495 2023-02-06 15:24:38.018836 rootmd-0.5.9/rootmd/data/css/prismjs/prism-funky.css
--rw-r--r--   0        0        0     1990 2023-02-06 15:24:38.001000 rootmd-0.5.9/rootmd/data/css/prismjs/prism-funky.min.css
--rw-r--r--   0        0        0     2109 2023-02-06 15:24:38.001639 rootmd-0.5.9/rootmd/data/css/prismjs/prism-ghcolors.css
--rw-r--r--   0        0        0     2417 2023-02-06 15:24:38.004131 rootmd-0.5.9/rootmd/data/css/prismjs/prism-gruvbox-dark.css
--rw-r--r--   0        0        0     2529 2023-02-06 15:24:37.999681 rootmd-0.5.9/rootmd/data/css/prismjs/prism-gruvbox-light.css
--rw-r--r--   0        0        0     2011 2023-02-06 15:24:38.011256 rootmd-0.5.9/rootmd/data/css/prismjs/prism-holi-theme.css
--rw-r--r--   0        0        0     1897 2023-02-06 15:24:38.001937 rootmd-0.5.9/rootmd/data/css/prismjs/prism-hopscotch.css
--rw-r--r--   0        0        0     1823 2023-02-06 15:24:38.010752 rootmd-0.5.9/rootmd/data/css/prismjs/prism-lucario.css
--rw-r--r--   0        0        0     2497 2023-02-06 15:24:38.000362 rootmd-0.5.9/rootmd/data/css/prismjs/prism-material-dark.css
--rw-r--r--   0        0        0     2534 2023-02-06 15:24:38.000684 rootmd-0.5.9/rootmd/data/css/prismjs/prism-material-light.css
--rw-r--r--   0        0        0     2556 2023-02-06 15:24:38.012028 rootmd-0.5.9/rootmd/data/css/prismjs/prism-material-oceanic.css
--rw-r--r--   0        0        0     2589 2023-02-06 15:24:38.016816 rootmd-0.5.9/rootmd/data/css/prismjs/prism-night-owl.css
--rw-r--r--   0        0        0     1814 2023-02-06 15:24:38.016491 rootmd-0.5.9/rootmd/data/css/prismjs/prism-nord.css
--rw-r--r--   0        0        0     1812 2023-02-06 15:24:38.001312 rootmd-0.5.9/rootmd/data/css/prismjs/prism-okaidia.css
--rw-r--r--   0        0        0     1380 2023-02-06 15:24:38.014831 rootmd-0.5.9/rootmd/data/css/prismjs/prism-okaidia.min.css
--rw-r--r--   0        0        0    12132 2023-02-06 15:24:38.014101 rootmd-0.5.9/rootmd/data/css/prismjs/prism-one-dark.css
--rw-r--r--   0        0        0    11915 2023-02-06 15:24:38.017810 rootmd-0.5.9/rootmd/data/css/prismjs/prism-one-light.css
--rw-r--r--   0        0        0     3839 2023-02-06 15:24:38.017152 rootmd-0.5.9/rootmd/data/css/prismjs/prism-pojoaque.css
--rw-r--r--   0        0        0     3246 2023-02-06 15:24:38.008435 rootmd-0.5.9/rootmd/data/css/prismjs/prism-shades-of-purple.css
--rw-r--r--   0        0        0     1968 2023-02-06 15:24:38.003224 rootmd-0.5.9/rootmd/data/css/prismjs/prism-solarized-dark-atom.css
--rw-r--r--   0        0        0     2606 2023-02-06 15:24:38.014446 rootmd-0.5.9/rootmd/data/css/prismjs/prism-solarizedlight.css
--rw-r--r--   0        0        0     1589 2023-02-06 15:24:38.009417 rootmd-0.5.9/rootmd/data/css/prismjs/prism-solarizedlight.min.css
--rw-r--r--   0        0        0     2456 2023-02-06 15:24:38.009005 rootmd-0.5.9/rootmd/data/css/prismjs/prism-synthwave84.css
--rw-r--r--   0        0        0     1766 2023-02-06 15:24:38.003588 rootmd-0.5.9/rootmd/data/css/prismjs/prism-tomorrow.css
--rw-r--r--   0        0        0     1313 2023-02-06 15:24:38.010322 rootmd-0.5.9/rootmd/data/css/prismjs/prism-tomorrow.min.css
--rw-r--r--   0        0        0     3620 2023-02-06 15:24:38.017485 rootmd-0.5.9/rootmd/data/css/prismjs/prism-twilight.css
--rw-r--r--   0        0        0     2440 2023-02-06 15:24:38.005672 rootmd-0.5.9/rootmd/data/css/prismjs/prism-twilight.min.css
--rw-r--r--   0        0        0     3070 2023-02-06 15:24:38.013066 rootmd-0.5.9/rootmd/data/css/prismjs/prism-vs.css
--rw-r--r--   0        0        0     4178 2023-02-06 15:24:38.002892 rootmd-0.5.9/rootmd/data/css/prismjs/prism-vsc-dark-plus.css
--rw-r--r--   0        0        0     2703 2023-02-06 15:24:38.007145 rootmd-0.5.9/rootmd/data/css/prismjs/prism-xonokai.css
--rw-r--r--   0        0        0     2520 2023-02-06 15:24:38.008097 rootmd-0.5.9/rootmd/data/css/prismjs/prism-z-touch.css
--rw-r--r--   0        0        0     2335 2023-02-06 15:24:38.015488 rootmd-0.5.9/rootmd/data/css/prismjs/prism.css
--rw-r--r--   0        0        0     1789 2023-02-06 15:24:38.007670 rootmd-0.5.9/rootmd/data/css/prismjs/prism.min.css
--rw-r--r--   0        0        0     5472 2023-02-06 15:24:38.042782 rootmd-0.5.9/rootmd/data/js/prism-1.26.0-autoloader.min.js
--rw-r--r--   0        0        0    18650 2023-02-06 15:24:38.042093 rootmd-0.5.9/rootmd/data/js/prism-1.26.0.min.js
--rw-r--r--   0        0        0     3272 2023-02-06 15:24:38.043544 rootmd-0.5.9/rootmd/data/template.html
--rw-r--r--   0        0        0     8093 1970-01-01 00:00:00.000000 rootmd-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-02-06 15:24:37.795290 rootmd-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7641 2023-05-19 00:27:29.352561 rootmd-0.6.0/README.md
+-rw-r--r--   0        0        0      757 2023-05-19 12:31:46.568931 rootmd-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3726 2023-05-05 00:24:29.186108 rootmd-0.6.0/rootmd/Executor.py
+-rw-r--r--   0        0        0     4796 2023-02-06 15:24:37.988540 rootmd-0.6.0/rootmd/Md2MacroRenderer.py
+-rw-r--r--   0        0        0     2866 2023-02-06 15:24:38.045297 rootmd-0.6.0/rootmd/RootBaseRenderer.py
+-rw-r--r--   0        0        0    20986 2023-05-19 00:28:09.186988 rootmd-0.6.0/rootmd/RootHtmlRenderer.py
+-rw-r--r--   0        0        0     5489 2023-05-19 00:24:13.575011 rootmd-0.6.0/rootmd/RootMdRenderer.py
+-rw-r--r--   0        0        0     6549 2023-02-06 15:24:37.989078 rootmd-0.6.0/rootmd/YamlBlock.py
+-rw-r--r--   0        0        0      531 2023-02-06 15:24:37.989478 rootmd-0.6.0/rootmd/__init__.py
+-rwxr-xr-x   0        0        0     8821 2023-05-05 16:06:03.073989 rootmd-0.6.0/rootmd/__main__.py
+-rw-r--r--   0        0        0     1130 2023-02-06 15:24:38.019160 rootmd-0.6.0/rootmd/data/css/core.css
+-rw-r--r--   0        0        0     2438 2023-02-06 15:24:38.000040 rootmd-0.6.0/rootmd/data/css/prismjs/prism-a11y-dark.css
+-rw-r--r--   0        0        0     1945 2023-02-06 15:24:38.011657 rootmd-0.6.0/rootmd/data/css/prismjs/prism-atom-dark.css
+-rw-r--r--   0        0        0     3332 2023-02-06 15:24:38.013757 rootmd-0.6.0/rootmd/data/css/prismjs/prism-base16-ateliersulphurpool.light.css
+-rw-r--r--   0        0        0     2618 2023-02-06 15:24:38.015816 rootmd-0.6.0/rootmd/data/css/prismjs/prism-cb.css
+-rw-r--r--   0        0        0     6782 2023-02-06 15:24:38.018137 rootmd-0.6.0/rootmd/data/css/prismjs/prism-coldark-cold.css
+-rw-r--r--   0        0        0     6776 2023-02-06 15:24:38.002562 rootmd-0.6.0/rootmd/data/css/prismjs/prism-coldark-dark.css
+-rw-r--r--   0        0        0     2306 2023-02-06 15:24:38.006485 rootmd-0.6.0/rootmd/data/css/prismjs/prism-coy-without-shadows.css
+-rw-r--r--   0        0        0     4031 2023-02-06 15:24:38.006001 rootmd-0.6.0/rootmd/data/css/prismjs/prism-coy.css
+-rw-r--r--   0        0        0     3062 2023-02-06 15:24:38.012747 rootmd-0.6.0/rootmd/data/css/prismjs/prism-coy.min.css
+-rw-r--r--   0        0        0     2680 2023-02-06 15:24:38.012408 rootmd-0.6.0/rootmd/data/css/prismjs/prism-darcula.css
+-rw-r--r--   0        0        0     2070 2023-02-06 15:24:38.009811 rootmd-0.6.0/rootmd/data/css/prismjs/prism-dark.css
+-rw-r--r--   0        0        0     1533 2023-02-06 15:24:38.002247 rootmd-0.6.0/rootmd/data/css/prismjs/prism-dark.min.css
+-rw-r--r--   0        0        0     1795 2023-02-06 15:24:38.006828 rootmd-0.6.0/rootmd/data/css/prismjs/prism-dracula.css
+-rw-r--r--   0        0        0     3389 2023-02-06 15:24:38.016149 rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-dark.css
+-rw-r--r--   0        0        0     3390 2023-02-06 15:24:38.018512 rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-earth.css
+-rw-r--r--   0        0        0     3395 2023-02-06 15:24:38.005334 rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-forest.css
+-rw-r--r--   0        0        0     3380 2023-02-06 15:24:37.999330 rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-light.css
+-rw-r--r--   0        0        0     3398 2023-02-06 15:24:38.015165 rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-sea.css
+-rw-r--r--   0        0        0     3388 2023-02-06 15:24:38.013409 rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-space.css
+-rw-r--r--   0        0        0     2495 2023-02-06 15:24:38.018836 rootmd-0.6.0/rootmd/data/css/prismjs/prism-funky.css
+-rw-r--r--   0        0        0     1990 2023-02-06 15:24:38.001000 rootmd-0.6.0/rootmd/data/css/prismjs/prism-funky.min.css
+-rw-r--r--   0        0        0     2109 2023-02-06 15:24:38.001639 rootmd-0.6.0/rootmd/data/css/prismjs/prism-ghcolors.css
+-rw-r--r--   0        0        0     2417 2023-02-06 15:24:38.004131 rootmd-0.6.0/rootmd/data/css/prismjs/prism-gruvbox-dark.css
+-rw-r--r--   0        0        0     2529 2023-02-06 15:24:37.999681 rootmd-0.6.0/rootmd/data/css/prismjs/prism-gruvbox-light.css
+-rw-r--r--   0        0        0     2011 2023-02-06 15:24:38.011256 rootmd-0.6.0/rootmd/data/css/prismjs/prism-holi-theme.css
+-rw-r--r--   0        0        0     1897 2023-02-06 15:24:38.001937 rootmd-0.6.0/rootmd/data/css/prismjs/prism-hopscotch.css
+-rw-r--r--   0        0        0     1823 2023-02-06 15:24:38.010752 rootmd-0.6.0/rootmd/data/css/prismjs/prism-lucario.css
+-rw-r--r--   0        0        0     2497 2023-02-06 15:24:38.000362 rootmd-0.6.0/rootmd/data/css/prismjs/prism-material-dark.css
+-rw-r--r--   0        0        0     2534 2023-02-06 15:24:38.000684 rootmd-0.6.0/rootmd/data/css/prismjs/prism-material-light.css
+-rw-r--r--   0        0        0     2556 2023-02-06 15:24:38.012028 rootmd-0.6.0/rootmd/data/css/prismjs/prism-material-oceanic.css
+-rw-r--r--   0        0        0     2589 2023-02-06 15:24:38.016816 rootmd-0.6.0/rootmd/data/css/prismjs/prism-night-owl.css
+-rw-r--r--   0        0        0     1814 2023-02-06 15:24:38.016491 rootmd-0.6.0/rootmd/data/css/prismjs/prism-nord.css
+-rw-r--r--   0        0        0     1812 2023-02-06 15:24:38.001312 rootmd-0.6.0/rootmd/data/css/prismjs/prism-okaidia.css
+-rw-r--r--   0        0        0     1380 2023-02-06 15:24:38.014831 rootmd-0.6.0/rootmd/data/css/prismjs/prism-okaidia.min.css
+-rw-r--r--   0        0        0    12132 2023-02-06 15:24:38.014101 rootmd-0.6.0/rootmd/data/css/prismjs/prism-one-dark.css
+-rw-r--r--   0        0        0    11915 2023-02-06 15:24:38.017810 rootmd-0.6.0/rootmd/data/css/prismjs/prism-one-light.css
+-rw-r--r--   0        0        0     3839 2023-02-06 15:24:38.017152 rootmd-0.6.0/rootmd/data/css/prismjs/prism-pojoaque.css
+-rw-r--r--   0        0        0     3246 2023-02-06 15:24:38.008435 rootmd-0.6.0/rootmd/data/css/prismjs/prism-shades-of-purple.css
+-rw-r--r--   0        0        0     1968 2023-02-06 15:24:38.003224 rootmd-0.6.0/rootmd/data/css/prismjs/prism-solarized-dark-atom.css
+-rw-r--r--   0        0        0     2606 2023-02-06 15:24:38.014446 rootmd-0.6.0/rootmd/data/css/prismjs/prism-solarizedlight.css
+-rw-r--r--   0        0        0     1589 2023-02-06 15:24:38.009417 rootmd-0.6.0/rootmd/data/css/prismjs/prism-solarizedlight.min.css
+-rw-r--r--   0        0        0     2456 2023-02-06 15:24:38.009005 rootmd-0.6.0/rootmd/data/css/prismjs/prism-synthwave84.css
+-rw-r--r--   0        0        0     1766 2023-02-06 15:24:38.003588 rootmd-0.6.0/rootmd/data/css/prismjs/prism-tomorrow.css
+-rw-r--r--   0        0        0     1313 2023-02-06 15:24:38.010322 rootmd-0.6.0/rootmd/data/css/prismjs/prism-tomorrow.min.css
+-rw-r--r--   0        0        0     3620 2023-02-06 15:24:38.017485 rootmd-0.6.0/rootmd/data/css/prismjs/prism-twilight.css
+-rw-r--r--   0        0        0     2440 2023-02-06 15:24:38.005672 rootmd-0.6.0/rootmd/data/css/prismjs/prism-twilight.min.css
+-rw-r--r--   0        0        0     3070 2023-02-06 15:24:38.013066 rootmd-0.6.0/rootmd/data/css/prismjs/prism-vs.css
+-rw-r--r--   0        0        0     4178 2023-02-06 15:24:38.002892 rootmd-0.6.0/rootmd/data/css/prismjs/prism-vsc-dark-plus.css
+-rw-r--r--   0        0        0     2703 2023-02-06 15:24:38.007145 rootmd-0.6.0/rootmd/data/css/prismjs/prism-xonokai.css
+-rw-r--r--   0        0        0     2520 2023-02-06 15:24:38.008097 rootmd-0.6.0/rootmd/data/css/prismjs/prism-z-touch.css
+-rw-r--r--   0        0        0     2335 2023-02-06 15:24:38.015488 rootmd-0.6.0/rootmd/data/css/prismjs/prism.css
+-rw-r--r--   0        0        0     1789 2023-02-06 15:24:38.007670 rootmd-0.6.0/rootmd/data/css/prismjs/prism.min.css
+-rw-r--r--   0        0        0     5472 2023-02-06 15:24:38.042782 rootmd-0.6.0/rootmd/data/js/prism-1.26.0-autoloader.min.js
+-rw-r--r--   0        0        0    18650 2023-02-06 15:24:38.042093 rootmd-0.6.0/rootmd/data/js/prism-1.26.0.min.js
+-rw-r--r--   0        0        0     3272 2023-02-06 15:24:38.043544 rootmd-0.6.0/rootmd/data/template.html
+-rw-r--r--   0        0        0     8637 1970-01-01 00:00:00.000000 rootmd-0.6.0/PKG-INFO
```

### Comparing `rootmd-0.5.9/LICENSE` & `rootmd-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/README.md` & `rootmd-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -118,16 +118,21 @@
 }
 
 void world() 
 {
   // this DOES NOT work
 }
 ```
-
-
+## Code Block Options
+- `stdout` or `out`: Default `true`.  Set to `false` to hide stdout block. Set to <filename> to write output to the given file.
+- `stderr` or `err`: Default `true`. Set to `false` to hide stderr block. Set to <filename> to write output to the given file.
+- `silent` or `quiet`: Default `false`. Set to `true` to hide both stderr and stdout
+- HTML only
+  - `.image`: css class to use for produced images.
+  - `raw`: output raw result from `stdout` as html
 
 ## Dependencies
 RootMD itself is a pure python package which uses:
 - [mistletoe](https://github.com/miyuchina/mistletoe) : python markdown parser and processor
 - [rich](https://github.com/Textualize/rich) : Rich for pretty terminal output
 - pyyaml : for parsing yaml front matter
 - Dependencies for HTML output
@@ -173,14 +178,16 @@
 
 ```
 
 ![h1.svg](h1.svg)
 
 ## Changelog
 
+### v0.6
+- Add control of output blocks to MdRenderer, update README
 ### v0.5.9
 - Add additional executor catch
   - Catch "_sigtramp"  
   - Catch "(no debug info)"
 
 ### v0.5.8
 - Allow log level to be set from command line arguments.
```

### Comparing `rootmd-0.5.9/pyproject.toml` & `rootmd-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rootmd"
-version = "0.5.9"
+version = "0.6.0"
 description = "RootMD is a markdown processor for markdown with ROOT-flavored c++ code. RootMD can execute c++ code and inject the output (from stdout, stderr) and link or embed image outputs"
 authors = ["Daniel Brandenburg <hello@jdbburg.com>"]
 include = ["rootmd/data"]
 readme = "README.md"
 repository = "https://github.com/jdbrice/RootMD"
 keywords = ["root", "markdown", "physics"]
```

### Comparing `rootmd-0.5.9/rootmd/Executor.py` & `rootmd-0.6.0/rootmd/Executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         output = ""
         while True:
             poll_result = select.select([s], [], [], time_limit)[0]
             if len(poll_result) > 0 :
                 l = s.readline()
                 log.debug( l )
                 if ( "ROOTEOF" in l or ("root [" in l and "]" in l) or "*** Break *** segmentation violation" in l or "Root >" in l or "_sigtramp" in l or "(no debug info)" in l ):
+                    log.debug("Executor::return")
                     return output
                 output += l
             elif time_limit != None:
                 break
         return output
     
     def run_cmd( self, code ):
```

### Comparing `rootmd-0.5.9/rootmd/Md2MacroRenderer.py` & `rootmd-0.6.0/rootmd/Md2MacroRenderer.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/RootBaseRenderer.py` & `rootmd-0.6.0/rootmd/RootBaseRenderer.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/RootHtmlRenderer.py` & `rootmd-0.6.0/rootmd/RootHtmlRenderer.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/YamlBlock.py` & `rootmd-0.6.0/rootmd/YamlBlock.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/__init__.py` & `rootmd-0.6.0/rootmd/__init__.py`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/__main__.py` & `rootmd-0.6.0/rootmd/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env conda run -n py38 python
+#!/usr/bin/env conda run -n base python
 
 import json
 import requests
 import os
 from xmlrpc.client import boolean
 import mistletoe as md
 from mistletoe.ast_renderer import ASTRenderer
```

### Comparing `rootmd-0.5.9/rootmd/data/css/core.css` & `rootmd-0.6.0/rootmd/data/css/core.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-a11y-dark.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-a11y-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-atom-dark.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-atom-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-base16-ateliersulphurpool.light.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-base16-ateliersulphurpool.light.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-cb.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-cb.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-coldark-cold.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-coldark-cold.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-coldark-dark.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-coldark-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-coy-without-shadows.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-coy-without-shadows.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-coy.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-coy.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-coy.min.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-coy.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-darcula.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-darcula.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-dark.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-dark.min.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-dark.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-dracula.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-dracula.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-dark.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-earth.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-earth.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-forest.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-forest.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-light.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-light.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-sea.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-sea.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-duotone-space.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-duotone-space.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-funky.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-funky.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-funky.min.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-funky.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-ghcolors.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-ghcolors.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-gruvbox-dark.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-gruvbox-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-gruvbox-light.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-gruvbox-light.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-holi-theme.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-holi-theme.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-hopscotch.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-hopscotch.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-lucario.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-lucario.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-material-dark.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-material-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-material-light.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-material-light.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-material-oceanic.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-material-oceanic.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-night-owl.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-night-owl.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-nord.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-nord.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-okaidia.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-okaidia.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-okaidia.min.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-okaidia.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-one-dark.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-one-dark.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-one-light.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-one-light.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-pojoaque.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-pojoaque.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-shades-of-purple.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-shades-of-purple.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-solarized-dark-atom.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-solarized-dark-atom.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-solarizedlight.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-solarizedlight.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-solarizedlight.min.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-solarizedlight.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-synthwave84.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-synthwave84.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-tomorrow.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-tomorrow.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-tomorrow.min.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-tomorrow.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-twilight.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-twilight.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-twilight.min.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-twilight.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-vs.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-vs.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-vsc-dark-plus.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-vsc-dark-plus.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-xonokai.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-xonokai.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism-z-touch.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism-z-touch.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/css/prismjs/prism.min.css` & `rootmd-0.6.0/rootmd/data/css/prismjs/prism.min.css`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/js/prism-1.26.0-autoloader.min.js` & `rootmd-0.6.0/rootmd/data/js/prism-1.26.0-autoloader.min.js`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/js/prism-1.26.0.min.js` & `rootmd-0.6.0/rootmd/data/js/prism-1.26.0.min.js`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/rootmd/data/template.html` & `rootmd-0.6.0/rootmd/data/template.html`

 * *Files identical despite different names*

### Comparing `rootmd-0.5.9/PKG-INFO` & `rootmd-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootmd
-Version: 0.5.9
+Version: 0.6.0
 Summary: RootMD is a markdown processor for markdown with ROOT-flavored c++ code. RootMD can execute c++ code and inject the output (from stdout, stderr) and link or embed image outputs
 Home-page: https://github.com/jdbrice/RootMD
 Keywords: root,markdown,physics
 Author: Daniel Brandenburg
 Author-email: hello@jdbburg.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -141,16 +141,21 @@
 }
 
 void world() 
 {
   // this DOES NOT work
 }
 ```
-
-
+## Code Block Options
+- `stdout` or `out`: Default `true`.  Set to `false` to hide stdout block. Set to <filename> to write output to the given file.
+- `stderr` or `err`: Default `true`. Set to `false` to hide stderr block. Set to <filename> to write output to the given file.
+- `silent` or `quiet`: Default `false`. Set to `true` to hide both stderr and stdout
+- HTML only
+  - `.image`: css class to use for produced images.
+  - `raw`: output raw result from `stdout` as html
 
 ## Dependencies
 RootMD itself is a pure python package which uses:
 - [mistletoe](https://github.com/miyuchina/mistletoe) : python markdown parser and processor
 - [rich](https://github.com/Textualize/rich) : Rich for pretty terminal output
 - pyyaml : for parsing yaml front matter
 - Dependencies for HTML output
@@ -196,14 +201,16 @@
 
 ```
 
 ![h1.svg](h1.svg)
 
 ## Changelog
 
+### v0.6
+- Add control of output blocks to MdRenderer, update README
 ### v0.5.9
 - Add additional executor catch
   - Catch "_sigtramp"  
   - Catch "(no debug info)"
 
 ### v0.5.8
 - Allow log level to be set from command line arguments.
```

