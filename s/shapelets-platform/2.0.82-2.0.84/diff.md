# Comparing `tmp/shapelets-platform-2.0.82.tar.gz` & `tmp/shapelets-platform-2.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapelets-platform-2.0.82.tar", last modified: Wed Apr 19 16:12:58 2023, max compression
+gzip compressed data, was "shapelets-platform-2.0.84.tar", last modified: Fri May 19 10:51:28 2023, max compression
```

## Comparing `shapelets-platform-2.0.82.tar` & `shapelets-platform-2.0.84.tar`

### file list

```diff
@@ -1,291 +1,291 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.846420 shapelets-platform-2.0.82/
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/COPYING.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-04-19 16:12:58.846420 shapelets-platform-2.0.82/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/noxfile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)     3007 2023-04-19 16:12:58.846420 shapelets-platform-2.0.82/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     4024 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.746419 shapelets-platform-2.0.82/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.750419 shapelets-platform-2.0.82/src/shapelets/
--rw-r--r--   0 vsts      (1001) docker     (123)      608 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6366 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18755 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/_cli.py
--rw-r--r--   0 vsts      (1001) docker     (123)    51826 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/_relations.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/_uom.py
--rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-04-19 16:12:54.000000 shapelets-platform-2.0.82/src/shapelets/_version.py
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/_version.pyi
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.754419 shapelets-platform-2.0.82/src/shapelets/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    62329 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/data_app.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/data_app_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.754419 shapelets-platform-2.0.82/src/shapelets/apps/widgets/
--rw-r--r--   0 vsts      (1001) docker     (123)      713 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2910 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/attribute_names.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.758419 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/
--rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/altair_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/bar_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/folium_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/heatmap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/histogram.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18963 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/line_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/pie_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/plotly_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/polar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/radar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/scatter_plot.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.762419 shapelets-platform-2.0.82/src/shapelets/apps/widgets/contexts/
--rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/contexts/filtering_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/contexts/metadata_field.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/contexts/metadata_filter.py
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/contexts/temporal_context.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.770419 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/
--rw-r--r--   0 vsts      (1001) docker     (123)     1177 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1483 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/button.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4400 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/checkbox.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/collection_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7465 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8049 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/datetime_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8263 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11087 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/number_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7362 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/progress.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9851 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/radio_group.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.770419 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/resources/
--rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
--rw-r--r--   0 vsts      (1001) docker     (123)    10639 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/sequence_list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14796 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/slider.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4389 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/text.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9070 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/text_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/timer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/datetime_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.770419 shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/
--rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/grid_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6028 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/horizontal_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/panel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4987 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/tabs_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5558 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/vertical_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1631 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    24070 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/apps/widgets/widget.py
--rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/iris.csv
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.778419 shapelets-platform-2.0.82/src/shapelets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/altair.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/capsule.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/collection.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/dataframe.py
--rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/function_description.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/function_parameter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/group.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/metadata_item.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/ndarray.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/permissions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/replicated_param.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/sequence.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/sequence_axis.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/user.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/model/view_match.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.778419 shapelets-platform-2.0.82/src/shapelets/svr/
--rw-r--r--   0 vsts      (1001) docker     (123)    10259 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/app.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.782419 shapelets-platform-2.0.82/src/shapelets/svr/authn/
--rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/authn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8713 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/authn/authhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8411 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/authn/authrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9640 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/authn/authservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/authn/gc_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2147 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/authn/iauthrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8961 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/authn/iauthservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.782419 shapelets-platform-2.0.82/src/shapelets/svr/data/
--rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.790419 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/
--rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/access_token_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/azure_gen1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/azure_gen2.py
--rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/driver.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/dynamic_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/fsspec_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/fsspec_vfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/local.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/protocols.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/smb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/vfs_sample_config.toml
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.794419 shapelets-platform-2.0.82/src/shapelets/svr/dataapps/
--rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/dataapps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3116 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/dataapps/dataapps_ws.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6025 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/dataapps/dataappshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9130 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/dataapps/dataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2226 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/dataapps/dataappsservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/dataapps/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1515 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/dataapps/idataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1260 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/dataapps/idataappsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.794419 shapelets-platform-2.0.82/src/shapelets/svr/db/
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.798419 shapelets-platform-2.0.82/src/shapelets/svr/db/native/
--rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/db/native/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/db/native/database.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/db/native/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/db/schema_builder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3858 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/db/schema_v1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/db/schema_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/db/schema_v3.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/db/setup.py
--rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/docs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.798419 shapelets-platform-2.0.82/src/shapelets/svr/execution/
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/execution/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1296 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/execution/executionhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/execution/executionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1033 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/execution/executionservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/execution/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/execution/iexecutionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      385 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/execution/iexecutionservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.802419 shapelets-platform-2.0.82/src/shapelets/svr/groups/
--rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/groups/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1596 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/groups/groupservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3770 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/groups/groupshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4753 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/groups/groupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/groups/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2094 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/groups/igroupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2626 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/groups/igroupsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.802419 shapelets-platform-2.0.82/src/shapelets/svr/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      631 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/model/dataapps.py
--rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/model/function.py
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/model/groups.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/model/principals.py
--rw-r--r--   0 vsts      (1001) docker     (123)      993 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/model/users.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.810419 shapelets-platform-2.0.82/src/shapelets/svr/mustang/
--rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/asttranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/conversions.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/core.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/decompiling.py
--rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/hashdict.py
--rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/identifier.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/ormtypes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.810419 shapelets-platform-2.0.82/src/shapelets/svr/mustang/prototypes/
--rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/prototypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/python_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/sqlbuilding.py
--rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/mustang/sqltranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4096 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/server.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.814420 shapelets-platform-2.0.82/src/shapelets/svr/settings/
--rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/defaults.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/http.py
--rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/reload.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/server.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/settings.toml
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/ssl.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/telemetry.py
--rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/settings/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.814420 shapelets-platform-2.0.82/src/shapelets/svr/telemetry/
--rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/telemetry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/telemetry/itelemetryservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/telemetry/sysinfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/telemetry/telemetryservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.818420 shapelets-platform-2.0.82/src/shapelets/svr/users/
--rw-r--r--   0 vsts      (1001) docker     (123)      732 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/users/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/users/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2248 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/users/iusersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1827 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/users/iusersservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3802 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/users/usershttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9016 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/users/usersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3233 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/users/usersservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.818420 shapelets-platform-2.0.82/src/shapelets/svr/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/utils/crypto.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/svr/utils/flexbytes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.822420 shapelets-platform-2.0.82/src/shapelets/svr/www/
--rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-04-19 16:12:52.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/altair.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/asset-manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/dataapp.json
--rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/favicon.ico
--rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/index.html
--rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/robots.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.746419 shapelets-platform-2.0.82/src/shapelets/svr/www/static/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.822420 shapelets-platform-2.0.82/src/shapelets/svr/www/static/css/
--rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
--rw-r--r--   0 vsts      (1001) docker     (123)    79553 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/css/main.8349d999.chunk.css
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.834420 shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/
--rw-r--r--   0 vsts      (1001) docker     (123)  6284390 2023-04-19 16:12:53.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   173518 2023-04-19 16:12:52.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/4.77242983.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/4.77242983.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   813635 2023-04-19 16:12:52.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.842420 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/
--rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/audit.cb539a06.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/bin.7e762965.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/clear.27b15301.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/download-image.87310709.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/filter.cec803b8.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
--rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/logout.57c593a5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/share.bc9a8370.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-04-19 16:12:52.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
--rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-04-19 16:12:51.000000 shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-04-19 15:54:19.000000 shapelets-platform-2.0.82/src/shapelets/systemd_template.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 16:12:58.842420 shapelets-platform-2.0.82/src/shapelets_platform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-04-19 16:12:54.000000 shapelets-platform-2.0.82/src/shapelets_platform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    11228 2023-04-19 16:12:58.000000 shapelets-platform-2.0.82/src/shapelets_platform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-19 16:12:54.000000 shapelets-platform-2.0.82/src/shapelets_platform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-04-19 16:12:54.000000 shapelets-platform-2.0.82/src/shapelets_platform.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)     1250 2023-04-19 16:12:54.000000 shapelets-platform-2.0.82/src/shapelets_platform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-19 16:12:54.000000 shapelets-platform-2.0.82/src/shapelets_platform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.194965 shapelets-platform-2.0.84/
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/COPYING.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-05-19 10:51:28.194965 shapelets-platform-2.0.84/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/noxfile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)     3007 2023-05-19 10:51:28.194965 shapelets-platform-2.0.84/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.102965 shapelets-platform-2.0.84/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.110965 shapelets-platform-2.0.84/src/shapelets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      608 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6366 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19249 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    51826 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/_relations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/_uom.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/_version.pyi
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.110965 shapelets-platform-2.0.84/src/shapelets/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    62329 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/data_app.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/data_app_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.114965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      713 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2910 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/attribute_names.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.118965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/altair_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/bar_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/folium_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/heatmap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18963 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/line_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/pie_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/plotly_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/polar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/radar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/scatter_plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.118965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/filtering_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/metadata_field.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/metadata_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/temporal_context.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.126965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1177 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1483 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/button.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4400 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/checkbox.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/collection_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7465 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8049 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/datetime_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8263 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11087 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/number_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7362 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9851 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/radio_group.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.126965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/resources/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
+-rw-r--r--   0 vsts      (1001) docker     (123)    10639 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/sequence_list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14796 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/slider.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4389 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/text.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9070 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/text_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/timer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/datetime_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.130965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/grid_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6028 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/horizontal_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/panel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4987 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/tabs_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5654 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/vertical_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1631 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    24282 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/widget.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/iris.csv
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.134965 shapelets-platform-2.0.84/src/shapelets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/altair.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/capsule.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/dataframe.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/function_description.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/function_parameter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/group.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/metadata_item.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/ndarray.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/permissions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/replicated_param.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/sequence.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/sequence_axis.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/user.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/view_match.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.138965 shapelets-platform-2.0.84/src/shapelets/svr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10259 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/app.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.138965 shapelets-platform-2.0.84/src/shapelets/svr/authn/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8713 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/authhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8411 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/authrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9640 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/authservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/gc_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2147 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/iauthrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8961 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/iauthservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.138965 shapelets-platform-2.0.84/src/shapelets/svr/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.146965 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/access_token_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/azure_gen1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/azure_gen2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/driver.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/dynamic_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/local.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/smb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/vfs_sample_config.toml
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.146965 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3116 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataapps_ws.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6025 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataappshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9130 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2226 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataappsservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1515 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/idataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1260 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/idataappsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.154965 shapelets-platform-2.0.84/src/shapelets/svr/db/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.154965 shapelets-platform-2.0.84/src/shapelets/svr/db/native/
+-rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/native/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/native/database.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/native/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/schema_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3858 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v3.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/docs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.158965 shapelets-platform-2.0.84/src/shapelets/svr/execution/
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1296 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/executionhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/executionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1033 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/executionservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/iexecutionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      385 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/iexecutionservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.162965 shapelets-platform-2.0.84/src/shapelets/svr/groups/
+-rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1596 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/groupservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3770 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/groupshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4753 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/groupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2094 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/igroupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2626 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/igroupsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.162965 shapelets-platform-2.0.84/src/shapelets/svr/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      631 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/dataapps.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/function.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/groups.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/principals.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      993 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/users.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.166965 shapelets-platform-2.0.84/src/shapelets/svr/mustang/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/asttranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/core.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/decompiling.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/hashdict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/identifier.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/ormtypes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.170965 shapelets-platform-2.0.84/src/shapelets/svr/mustang/prototypes/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/prototypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/python_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/sqlbuilding.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/sqltranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/server.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.174965 shapelets-platform-2.0.84/src/shapelets/svr/settings/
+-rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/http.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/reload.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/server.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/settings.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/ssl.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/telemetry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.174965 shapelets-platform-2.0.84/src/shapelets/svr/telemetry/
+-rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/telemetry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/telemetry/itelemetryservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/telemetry/sysinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/telemetry/telemetryservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.178965 shapelets-platform-2.0.84/src/shapelets/svr/users/
+-rw-r--r--   0 vsts      (1001) docker     (123)      732 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2248 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/iusersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1827 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/iusersservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3802 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/usershttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9016 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/usersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3233 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/usersservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.178965 shapelets-platform-2.0.84/src/shapelets/svr/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/utils/crypto.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/utils/flexbytes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.178965 shapelets-platform-2.0.84/src/shapelets/svr/www/
+-rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/altair.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/asset-manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/dataapp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/favicon.ico
+-rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/index.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/robots.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.102965 shapelets-platform-2.0.84/src/shapelets/svr/www/static/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.182965 shapelets-platform-2.0.84/src/shapelets/svr/www/static/css/
+-rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
+-rw-r--r--   0 vsts      (1001) docker     (123)    79553 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/css/main.8349d999.chunk.css
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.190965 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/
+-rw-r--r--   0 vsts      (1001) docker     (123)  6284390 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   173518 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/4.77242983.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/4.77242983.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   813635 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.194965 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/
+-rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/audit.cb539a06.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/bin.7e762965.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/clear.27b15301.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/download-image.87310709.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/filter.cec803b8.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logout.57c593a5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/share.bc9a8370.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/systemd_template.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.194965 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    11228 2023-05-19 10:51:28.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1250 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/top_level.txt
```

### Comparing `shapelets-platform-2.0.82/LICENSE.md` & `shapelets-platform-2.0.84/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/PKG-INFO` & `shapelets-platform-2.0.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.82
+Version: 2.0.84
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.82/README.md` & `shapelets-platform-2.0.84/README.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/noxfile.py` & `shapelets-platform-2.0.84/noxfile.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/pyproject.toml` & `shapelets-platform-2.0.84/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/setup.cfg` & `shapelets-platform-2.0.84/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 	psutil >= 5.9.2
 	pyarrow >=9.0.0
 	py-cpuinfo>=9.0.0
 	pydantic >= 1.10.2
 	pygeohash >= 1.2.0
 	PyNaCl >= 1.5.0
 	requests >= 2.28.1
-	shapelets_native == 2.0.82
+	shapelets_native == 2.0.84
 	tabulate>=0.8.10
 	tomlkit >= 0.11.4
 	tqdm >= 4.64.1
 	uvicorn >= 0.18.3
 	vega-datasets >= 0.9
 	websocket >= 0.2.1
 	websockets >= 10.3
```

### Comparing `shapelets-platform-2.0.82/setup.py` & `shapelets-platform-2.0.84/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,19 +93,19 @@
     #     webbrowser.open(f"https://shapelets.io/enroll?cid={id}&lang={user_language()}")
 
 
 def stop_local_server():
     import psutil
     
     shapelets_dir = os.path.expanduser('~/.shapelets')
-    system_pid = os.path.join(shapelets_dir, 'server.pid')
+    system_pid = os.path.join(shapelets_dir, 'shapelets.pid')
     
     #
     # Stop current server, if any. If the server is running,
-    # its PID is storedin ~/.shapelets/server.pid
+    # its PID is storedin ~/.shapelets/shapelets.pid
     #
     
     if os.path.exists( system_pid ):
         
         with open(system_pid, 'rt') as f:
             
             try:
```

### Comparing `shapelets-platform-2.0.82/src/shapelets/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/_api.py` & `shapelets-platform-2.0.84/src/shapelets/_api.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/_cli.py` & `shapelets-platform-2.0.84/src/shapelets/_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import traceback
 import uuid
 import pydantic
 import tomlkit
 import json
 import shutil
 import socket
+import subprocess
 
 from ipaddress import IPv4Address, IPv6Address
 from string import Template
 from urllib.parse import urlparse
 
 from .svr import Settings, crypto, FlexBytes, UserAttributes, initialize_svr
 from . import _api
@@ -23,15 +24,15 @@
 try:
     import pwd
     import lockfile
     import daemon
 
     _on_windows = False
 except:
-    _on_windows = True 
+    _on_windows = True
 
 
 def build_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(prog='shapelets', description='Shapelets Platform Tools')
     subparsers = parser.add_subparsers(dest='command')
 
     server_parser = subparsers.add_parser('server', help='Server tools')
@@ -112,14 +113,20 @@
 
     # server run
     server_run_options = server_options.add_parser(
         'run',
         help='Runs the server',
         description="Runs the server using the current Python interpreter.")
 
+    # server stop
+    server_options.add_parser(
+        'stop',
+        help='Stops the server',
+        description="Stops the server.")
+
     # if we are running on windows, disable the tools for daemons and systemd
     if not _on_windows:
         server_run_options.add_argument('--daemon', action='store_true', help='Run as a traditional *nix daemon')
         server_run_options.add_argument('--lock', type=str,
                                         help='Only used if daemon is used, it sets the location of the lock file',
                                         default='./shapelets.lock')
         server_run_options.add_argument('--log', type=str,
@@ -180,47 +187,48 @@
                                     help='User running the server')
 
         daemon_options.add_argument('-g', '--grp', type=str,
                                     help='Group to run the server')
 
         daemon_options.add_argument('-d', '--dst', type=str,
                                     default='/etc/systemd/system/',
-                                    help='Folder to store the service template (/etc/systemd/system/).',)
+                                    help='Folder to store the service template (/etc/systemd/system/).', )
 
     client_parser = subparsers.add_parser('client', help='Client Defaults')
     which_server = client_parser.add_mutually_exclusive_group(required=True)
     which_server.add_argument("--local", action="store_true", help='Use Local server')
     which_server.add_argument("--url", type=str, help='URL of the server to connect to')
 
     client_parser.add_argument("-u", "--usr", type=str, help='User Name')
     client_parser.add_argument("-p", "--pwd", type=str, help='User Password')
     client_parser.add_argument("--create", action="store_true", help='Create user if not exists')
     client_parser.add_argument("--remember-me", action="store_true", help='Logon and remember credentials')
     client_parser.add_argument("--enable-telemetry", action="store_true", help='Enable telemetry')
     client_parser.add_argument("--disable-telemetry", action="store_true", help='Disable telemetry')
     return parser
 
+
 def resolve_host(expression: str) -> Optional[str]:
     try:
         return str(IPv4Address(expression))
     except:
-        pass 
+        pass
 
     try:
         return str(IPv6Address(expression))
     except:
-        pass 
+        pass
 
     try:
         return socket.gethostbyname(expression)
     except:
         return None
 
-def process_client(data: argparse.Namespace):
 
+def process_client(data: argparse.Namespace):
     # change the current directory to user's home
     home_dir = os.path.expanduser('~/.shapelets')
     os.makedirs(home_dir, exist_ok=True)
     os.chdir(home_dir)
 
     # and load from here the settings
     current_settings = Settings()
@@ -269,17 +277,17 @@
             host, port = netloc.split(':')
         else:
             host = netloc
             port = 443 if protocol == 'https' else 80
 
     ip = resolve_host(host)
     if ip is None:
-        raise ValueError(f'Unable to resolve host {host}')        
+        raise ValueError(f'Unable to resolve host {host}')
     if ip != host:
-        print(f"{host} resolved to {ip}")   
+        print(f"{host} resolved to {ip}")
 
     client_doc['server_mode'] = 'out-of-process'
     client_doc['host'] = ip
     client_doc['port'] = int(port)
     client_doc['protocol'] = protocol
 
     # save the new settings
@@ -375,15 +383,15 @@
 
     with open(settings_file, "wt", encoding="utf-8") as handle:
         handle.truncate()
         tomlkit.dump(new_cfg, handle)
 
 
 def process_server_run(data: argparse.Namespace):
-    run_classic_daemon = ('daemon' in data and data.daemon) or False 
+    run_classic_daemon = ('daemon' in data and data.daemon) or False
     if _on_windows or not run_classic_daemon:
         initialize_svr('standalone')
     else:
         pid_path = os.path.realpath(os.path.expanduser(data.pid))
         lock_path = os.path.realpath(os.path.expanduser(data.lock))
         log_path = os.path.realpath(os.path.expanduser(data.log))
 
@@ -397,14 +405,23 @@
         print()
         print('To stop it:')
         print(f'\tcat {pid_path} | xargs kill')
 
         with daemon.DaemonContext(pidfile=lock, stderr=log):
             initialize_svr('standalone', pid_file=pid_path)
 
+
+def process_server_stop():
+    pid_path = os.path.join(os.path.expanduser('~/.shapelets'), 'shapelets.pid')
+    cmd_str = f'cat {pid_path} | xargs kill'
+    result = subprocess.run(cmd_str, shell=True)
+    if result.returncode == 0:
+        print('Shapelets Server stopped.')
+
+
 def get_current_user_and_group():
     data = pwd.getpwuid(os.getuid())
     return data[0], data[3]
 
 
 def get_current_user():
     data = pwd.getpwuid(os.getuid())
@@ -449,14 +466,16 @@
 def process_server(data: argparse.Namespace):
     if data.server_command == 'show':
         process_server_show(data)
     elif data.server_command == 'config':
         process_server_config(data)
     elif data.server_command == 'run':
         process_server_run(data)
+    elif data.server_command == 'stop':
+        process_server_stop()
     else:
         process_server_systemd(data)
 
 
 def cli() -> None:
     parser = build_parser()
     # argcomplete.autocomplete(parser)
```

### Comparing `shapelets-platform-2.0.82/src/shapelets/_relations.py` & `shapelets-platform-2.0.84/src/shapelets/_relations.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/_uom.py` & `shapelets-platform-2.0.84/src/shapelets/_uom.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/data_app.py` & `shapelets-platform-2.0.84/src/shapelets/apps/data_app.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/data_app_utils.py` & `shapelets-platform-2.0.84/src/shapelets/apps/data_app_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/attribute_names.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/attribute_names.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/altair_chart.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/altair_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/bar_chart.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/folium_chart.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/folium_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/heatmap.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/heatmap.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/histogram.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/histogram.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/line_chart.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/pie_chart.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/plotly_chart.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/polar_area.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/polar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/radar_area.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/radar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/charts/scatter_plot.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/contexts/filtering_context.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/filtering_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/contexts/metadata_field.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/metadata_field.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/contexts/metadata_filter.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/metadata_filter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/contexts/temporal_context.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/temporal_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/button.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/button.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/checkbox.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/checkbox.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/collection_selector.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/collection_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/datetime_range_selector.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/datetime_range_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/datetime_selector.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/datetime_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/image.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/list.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/number_input.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/number_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/progress.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/progress.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/radio_group.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/radio_group.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/selector.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/sequence_list.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/sequence_list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/sequence_selector.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/slider.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/slider.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/table.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/table.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/text.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/text.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/text_input.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/text_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/controllers/timer.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/timer.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/datetime_utils.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/grid_layout.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/grid_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/horizontal_layout.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/horizontal_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/panel.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/panel.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/tabs_layout.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/tabs_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/layouts/vertical_layout.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/vertical_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,18 @@
                 AttributeNames.WIDTH.value: width,
                 AttributeNames.OFFSET.value: offset
             } for key, (width, offset) in self.placements.items()]
         })
         panel_dict[AttributeNames.PROPERTIES.value].update({
             AttributeNames.VERTICAL_ALIGN.value: self.vertical_align
         })
-        panel_dict[AttributeNames.PROPERTIES.value].update({
-            AttributeNames.COL_SPAN.value: self.span
-        })
-        panel_dict[AttributeNames.PROPERTIES.value].update({
-            AttributeNames.COL_OFFSET.value: self.offset
-        })
+
+        if self.span is not None:
+            panel_dict[AttributeNames.PROPERTIES.value].update({
+                AttributeNames.COL_SPAN.value: self.span
+            })
+
+        if self.offset is not None:
+            panel_dict[AttributeNames.PROPERTIES.value].update({
+                AttributeNames.COL_OFFSET.value: self.offset
+            })
         return panel_dict
```

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/util.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/util.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/apps/widgets/widget.py` & `shapelets-platform-2.0.84/src/shapelets/apps/widgets/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,17 +315,22 @@
         """
         Find the parameters use in a function.
         param fn: Function to extract parameters from.
         return List with all the parameters.
         """
         parameters = []
         for param in inspect.signature(fn).parameters.values():
+            try:
+                input_type = param.annotation.__name__
+            except AttributeError:
+                # When using typing, type name is included in _name
+                input_type = param.annotation._name
             parameters.append({
                 "name": param.name,
-                "type": param.annotation.__name__,
+                "type": input_type,
                 "default": None if param.default is param.empty else param.default
             })
         return parameters
 
     @staticmethod
     def _find_triggers(kwargs: Dict) -> List:
         """
```

### Comparing `shapelets-platform-2.0.82/src/shapelets/functions.py` & `shapelets-platform-2.0.84/src/shapelets/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/iris.csv` & `shapelets-platform-2.0.84/src/shapelets/iris.csv`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/model/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/altair.py` & `shapelets-platform-2.0.84/src/shapelets/model/altair.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/capsule.py` & `shapelets-platform-2.0.84/src/shapelets/model/capsule.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/collection.py` & `shapelets-platform-2.0.84/src/shapelets/model/collection.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/dataframe.py` & `shapelets-platform-2.0.84/src/shapelets/model/dataframe.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/function_description.py` & `shapelets-platform-2.0.84/src/shapelets/model/function_description.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/function_parameter.py` & `shapelets-platform-2.0.84/src/shapelets/model/function_parameter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/group.py` & `shapelets-platform-2.0.84/src/shapelets/model/group.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/image.py` & `shapelets-platform-2.0.84/src/shapelets/model/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/metadata_item.py` & `shapelets-platform-2.0.84/src/shapelets/model/metadata_item.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/model.py` & `shapelets-platform-2.0.84/src/shapelets/model/model.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/ndarray.py` & `shapelets-platform-2.0.84/src/shapelets/model/ndarray.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/permissions.py` & `shapelets-platform-2.0.84/src/shapelets/model/permissions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/replicated_param.py` & `shapelets-platform-2.0.84/src/shapelets/model/replicated_param.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/sequence.py` & `shapelets-platform-2.0.84/src/shapelets/model/sequence.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/sequence_axis.py` & `shapelets-platform-2.0.84/src/shapelets/model/sequence_axis.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/user.py` & `shapelets-platform-2.0.84/src/shapelets/model/user.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/model/view_match.py` & `shapelets-platform-2.0.84/src/shapelets/model/view_match.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/app.py` & `shapelets-platform-2.0.84/src/shapelets/svr/app.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/authn/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/authn/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/authn/authhttp.py` & `shapelets-platform-2.0.84/src/shapelets/svr/authn/authhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/authn/authrepo.py` & `shapelets-platform-2.0.84/src/shapelets/svr/authn/authrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/authn/authservice.py` & `shapelets-platform-2.0.84/src/shapelets/svr/authn/authservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/authn/gc_client.py` & `shapelets-platform-2.0.84/src/shapelets/svr/authn/gc_client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/authn/iauthrepo.py` & `shapelets-platform-2.0.84/src/shapelets/svr/authn/iauthrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/authn/iauthservice.py` & `shapelets-platform-2.0.84/src/shapelets/svr/authn/iauthservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/access_token_credentials.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/access_token_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/azure_gen1.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/azure_gen1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/azure_gen2.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/azure_gen2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/driver.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/driver.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/dynamic_credentials.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/dynamic_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/fsspec_config.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_config.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/fsspec_vfs.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/fsspec_vfs_file.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs_file.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/ftp.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/ftp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/local.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/local.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/protocols.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/protocols.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/smb.py` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/smb.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/data/vfs/vfs_sample_config.toml` & `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/vfs_sample_config.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/dataapps/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/dataapps/dataapps_ws.py` & `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataapps_ws.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/dataapps/dataappshttp.py` & `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataappshttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/dataapps/dataappsrepo.py` & `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/dataapps/dataappsservice.py` & `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataappsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/dataapps/http_docs.py` & `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/dataapps/idataappsrepo.py` & `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/idataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/dataapps/idataappsservice.py` & `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/idataappsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/db/native/database.py` & `shapelets-platform-2.0.84/src/shapelets/svr/db/native/database.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/db/native/settings.py` & `shapelets-platform-2.0.84/src/shapelets/svr/db/native/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/db/schema_builder.py` & `shapelets-platform-2.0.84/src/shapelets/svr/db/schema_builder.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/db/schema_v1.py` & `shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/db/schema_v2.py` & `shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/db/schema_v3.py` & `shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v3.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/db/setup.py` & `shapelets-platform-2.0.84/src/shapelets/svr/db/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/execution/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/execution/executionhttp.py` & `shapelets-platform-2.0.84/src/shapelets/svr/execution/executionhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/execution/executionservice.py` & `shapelets-platform-2.0.84/src/shapelets/svr/execution/executionservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/execution/http_docs.py` & `shapelets-platform-2.0.84/src/shapelets/svr/execution/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/groups/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/groups/groupservice.py` & `shapelets-platform-2.0.84/src/shapelets/svr/groups/groupservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/groups/groupshttp.py` & `shapelets-platform-2.0.84/src/shapelets/svr/groups/groupshttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/groups/groupsrepo.py` & `shapelets-platform-2.0.84/src/shapelets/svr/groups/groupsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/groups/igroupsrepo.py` & `shapelets-platform-2.0.84/src/shapelets/svr/groups/igroupsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/groups/igroupsservice.py` & `shapelets-platform-2.0.84/src/shapelets/svr/groups/igroupsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/model/dataapps.py` & `shapelets-platform-2.0.84/src/shapelets/svr/model/dataapps.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/model/principals.py` & `shapelets-platform-2.0.84/src/shapelets/svr/model/principals.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/model/users.py` & `shapelets-platform-2.0.84/src/shapelets/svr/model/users.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/asttranslation.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/asttranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/conversions.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/conversions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/core.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/core.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/decompiling.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/decompiling.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/exceptions.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/exceptions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/hashdict.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/hashdict.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/ormtypes.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/ormtypes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/prototypes/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/prototypes/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/serialization.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/serialization.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/sqlbuilding.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/sqlbuilding.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/mustang/sqltranslation.py` & `shapelets-platform-2.0.84/src/shapelets/svr/mustang/sqltranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/server.py` & `shapelets-platform-2.0.84/src/shapelets/svr/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,19 +123,19 @@
     if pid_file :
         
         with open(pid_file, 'wt') as f:
             f.truncate()
             f.write(svr_pid)
            
     #
-    # Store the process PID on 'server.pid', so it can be easily
+    # Store the process PID on 'shapelets.pid', so it can be easily
     # retrieved (for instance, if the process needs to be shut down)
     #
     shapelets_dir = os.path.expanduser('~/.shapelets')
-    system_pid = os.path.join(shapelets_dir, 'server.pid')
+    system_pid = os.path.join(shapelets_dir, 'shapelets.pid')
     
     with open(system_pid, 'wt') as f:
         f.truncate()
         f.write(svr_pid)
         
     server = UviServer(update_uvicorn_settings(cfg.server, UviConfig(app)))
     server.run()
```

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/client.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/defaults.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/functions.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/http.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/http.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/reload.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/reload.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/server.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/settings.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/settings.toml` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/settings.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/ssl.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/ssl.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/telemetry.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/telemetry.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/settings/websocket.py` & `shapelets-platform-2.0.84/src/shapelets/svr/settings/websocket.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/telemetry/sysinfo.py` & `shapelets-platform-2.0.84/src/shapelets/svr/telemetry/sysinfo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/telemetry/telemetryservice.py` & `shapelets-platform-2.0.84/src/shapelets/svr/telemetry/telemetryservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/users/__init__.py` & `shapelets-platform-2.0.84/src/shapelets/svr/users/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/users/http_docs.py` & `shapelets-platform-2.0.84/src/shapelets/svr/users/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/users/iusersrepo.py` & `shapelets-platform-2.0.84/src/shapelets/svr/users/iusersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/users/iusersservice.py` & `shapelets-platform-2.0.84/src/shapelets/svr/users/iusersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/users/usershttp.py` & `shapelets-platform-2.0.84/src/shapelets/svr/users/usershttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/users/usersrepo.py` & `shapelets-platform-2.0.84/src/shapelets/svr/users/usersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/users/usersservice.py` & `shapelets-platform-2.0.84/src/shapelets/svr/users/usersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/utils/crypto.py` & `shapelets-platform-2.0.84/src/shapelets/svr/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/utils/flexbytes.py` & `shapelets-platform-2.0.84/src/shapelets/svr/utils/flexbytes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/altair.json` & `shapelets-platform-2.0.84/src/shapelets/svr/www/altair.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/asset-manifest.json` & `shapelets-platform-2.0.84/src/shapelets/svr/www/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/dataapp.json` & `shapelets-platform-2.0.84/src/shapelets/svr/www/dataapp.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/favicon.ico` & `shapelets-platform-2.0.84/src/shapelets/svr/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/index.html` & `shapelets-platform-2.0.84/src/shapelets/svr/www/index.html`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/css/main.8349d999.chunk.css` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/css/main.8349d999.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/4.77242983.chunk.js` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/4.77242983.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/audit.cb539a06.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/audit.cb539a06.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/bin.7e762965.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/bin.7e762965.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/clear.27b15301.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/clear.27b15301.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/collections.06fdf54a.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/collections.06fdf54a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/date-time.a1e86419.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/date-time.a1e86419.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/download-image.87310709.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/download-image.87310709.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/filter.cec803b8.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/filter.cec803b8.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/logout.57c593a5.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logout.57c593a5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/pdf.5d189efa.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/pdf.5d189efa.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/share.bc9a8370.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/share.bc9a8370.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/single-plot.864a583b.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/single-plot.864a583b.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets/svr/www/static/media/wave-top.6d51781b.png` & `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/wave-top.6d51781b.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets_platform.egg-info/PKG-INFO` & `shapelets-platform-2.0.84/src/shapelets_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.82
+Version: 2.0.84
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.82/src/shapelets_platform.egg-info/SOURCES.txt` & `shapelets-platform-2.0.84/src/shapelets_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.82/src/shapelets_platform.egg-info/requires.txt` & `shapelets-platform-2.0.84/src/shapelets_platform.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 psutil>=5.9.2
 pyarrow>=9.0.0
 py-cpuinfo>=9.0.0
 pydantic>=1.10.2
 pygeohash>=1.2.0
 PyNaCl>=1.5.0
 requests>=2.28.1
-shapelets_native==2.0.82
+shapelets_native==2.0.84
 tabulate>=0.8.10
 tomlkit>=0.11.4
 tqdm>=4.64.1
 uvicorn>=0.18.3
 vega-datasets>=0.9
 websocket>=0.2.1
 websockets>=10.3
```

