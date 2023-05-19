# Comparing `tmp/NodeGraphQt-0.5.9.tar.gz` & `tmp/NodeGraphQt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NodeGraphQt-0.5.9.tar", last modified: Fri May  5 10:43:50 2023, max compression
+gzip compressed data, was "NodeGraphQt-0.6.0.tar", last modified: Fri May 19 08:55:01 2023, max compression
```

## Comparing `NodeGraphQt-0.5.9.tar` & `NodeGraphQt-0.6.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.868894 NodeGraphQt-0.5.9/
--rw-rw-rw-   0        0        0     1102 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.9/LICENSE.md
--rw-rw-rw-   0        0        0       49 2022-05-22 21:37:50.000000 NodeGraphQt-0.5.9/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.573658 NodeGraphQt-0.5.9/NodeGraphQt/
--rw-rw-rw-   0        0        0     2469 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.631841 NodeGraphQt-0.5.9/NodeGraphQt/base/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/__init__.py
--rw-rw-rw-   0        0        0    12642 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/commands.py
--rw-rw-rw-   0        0        0     2816 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/factory.py
--rw-rw-rw-   0        0        0    97819 2023-05-05 10:40:41.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/graph.py
--rw-rw-rw-   0        0        0     8273 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/menu.py
--rw-rw-rw-   0        0        0    14329 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/model.py
--rw-rw-rw-   0        0        0    15016 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/node.py
--rw-rw-rw-   0        0        0    12137 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/base/port.py
--rw-rw-rw-   0        0        0     7417 2023-05-03 04:38:45.000000 NodeGraphQt-0.5.9/NodeGraphQt/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.644844 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/
--rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0    11914 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-rw-rw-   0        0        0     4749 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/nodes_tree.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.699856 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/
--rw-rw-rw-   0        0        0        0 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-rw-rw-   0        0        0     3550 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-rw-rw-   0        0        0     2455 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-rw-rw-   0        0        0     4995 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-rw-rw-   0        0        0     6304 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-rw-rw-   0        0        0     2948 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-rw-rw-   0        0        0     2489 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-rw-rw-   0        0        0    20765 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-rw-rw-   0        0        0      761 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-rw-rw-   0        0        0     7267 2022-12-21 22:27:30.000000 NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-rw-rw-   0        0        0      406 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.729863 NodeGraphQt-0.5.9/NodeGraphQt/nodes/
--rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/__init__.py
--rw-rw-rw-   0        0        0     4465 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/backdrop_node.py
--rw-rw-rw-   0        0        0    23281 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/base_node.py
--rw-rw-rw-   0        0        0     1253 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/base_node_circle.py
--rw-rw-rw-   0        0        0     5817 2023-05-04 10:15:30.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/group_node.py
--rw-rw-rw-   0        0        0     4409 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/nodes/port_node.py
--rw-rw-rw-   0        0        0      239 2023-05-05 10:41:15.000000 NodeGraphQt-0.5.9/NodeGraphQt/pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.796878 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/
--rw-rw-rw-   0        0        0        0 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/__init__.py
--rw-rw-rw-   0        0        0     7060 2023-04-19 08:52:02.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_abstract.py
--rw-rw-rw-   0        0        0    10763 2023-05-03 01:54:07.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_backdrop.py
--rw-rw-rw-   0        0        0    36771 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_base.py
--rw-rw-rw-   0        0        0    21204 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_circle.py
--rw-rw-rw-   0        0        0    12346 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_group.py
--rw-rw-rw-   0        0        0     4273 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-rw-rw-   0        0        0     8159 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_port_in.py
--rw-rw-rw-   0        0        0     8158 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_port_out.py
--rw-rw-rw-   0        0        0     3749 2022-05-08 02:47:52.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_text_item.py
--rw-rw-rw-   0        0        0    21504 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/pipe.py
--rw-rw-rw-   0        0        0    10582 2023-04-30 08:29:15.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/port.py
--rw-rw-rw-   0        0        0     2885 2023-05-03 09:02:56.000000 NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/slicer.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.838887 NodeGraphQt-0.5.9/NodeGraphQt/widgets/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/__init__.py
--rw-rw-rw-   0        0        0     3709 2022-12-21 07:01:38.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/actions.py
--rw-rw-rw-   0        0        0     1873 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/dialogs.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.839889 NodeGraphQt-0.5.9/NodeGraphQt/widgets/icons/
--rw-rw-rw-   0        0        0    17542 2021-06-18 10:54:50.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/icons/node_base.png
--rw-rw-rw-   0        0        0     4550 2023-05-03 09:15:23.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/node_graph.py
--rw-rw-rw-   0        0        0    14045 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/node_widgets.py
--rw-rw-rw-   0        0        0     5681 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/scene.py
--rw-rw-rw-   0        0        0    11436 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/tab_search.py
--rw-rw-rw-   0        0        0    51135 2023-05-05 10:40:41.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/viewer.py
--rw-rw-rw-   0        0        0     6914 2023-05-04 05:49:13.000000 NodeGraphQt-0.5.9/NodeGraphQt/widgets/viewer_nav.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.593663 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/
--rw-rw-rw-   0        0        0     2738 2023-05-05 10:43:50.000000 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2023-05-05 10:43:50.000000 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 10:43:50.000000 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-05 10:43:50.000000 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-05 10:43:50.000000 NodeGraphQt-0.5.9/NodeGraphQt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2738 2023-05-05 10:43:50.868894 NodeGraphQt-0.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     2034 2023-05-03 10:36:51.000000 NodeGraphQt-0.5.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.546651 NodeGraphQt-0.5.9/examples/
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.845890 NodeGraphQt-0.5.9/examples/hotkeys/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/examples/hotkeys/__init__.py
--rw-rw-rw-   0        0        0     6199 2023-05-04 10:16:17.000000 NodeGraphQt-0.5.9/examples/hotkeys/hotkey_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:43:50.867894 NodeGraphQt-0.5.9/examples/nodes/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/examples/nodes/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-05-02 09:54:57.000000 NodeGraphQt-0.5.9/examples/nodes/basic_nodes.py
--rw-rw-rw-   0        0        0     3671 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/examples/nodes/custom_ports_node.py
--rw-rw-rw-   0        0        0      507 2022-10-18 20:17:59.000000 NodeGraphQt-0.5.9/examples/nodes/group_node.py
--rw-rw-rw-   0        0        0     1822 2023-05-02 10:58:55.000000 NodeGraphQt-0.5.9/examples/nodes/widget_nodes.py
--rw-rw-rw-   0        0        0     1070 2023-05-05 10:43:50.873911 NodeGraphQt-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0      123 2022-12-21 06:31:06.000000 NodeGraphQt-0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.458956 NodeGraphQt-0.6.0/
+-rw-rw-rw-   0        0        0     1102 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.0/LICENSE.md
+-rw-rw-rw-   0        0        0       49 2022-05-22 21:37:50.000000 NodeGraphQt-0.6.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.186585 NodeGraphQt-0.6.0/NodeGraphQt/
+-rw-rw-rw-   0        0        0     2469 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.237596 NodeGraphQt-0.6.0/NodeGraphQt/base/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/__init__.py
+-rw-rw-rw-   0        0        0    12642 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/commands.py
+-rw-rw-rw-   0        0        0     2816 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/factory.py
+-rw-rw-rw-   0        0        0   102277 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/graph.py
+-rw-rw-rw-   0        0        0     8273 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/menu.py
+-rw-rw-rw-   0        0        0    20817 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/model.py
+-rw-rw-rw-   0        0        0    15016 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/node.py
+-rw-rw-rw-   0        0        0    16292 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/port.py
+-rw-rw-rw-   0        0        0     7417 2023-05-09 09:46:08.000000 NodeGraphQt-0.6.0/NodeGraphQt/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.251600 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/
+-rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0    11914 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/nodes_palette.py
+-rw-rw-rw-   0        0        0     4749 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/nodes_tree.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.309614 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/
+-rw-rw-rw-   0        0        0        0 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-rw-rw-   0        0        0     3550 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-rw-rw-   0        0        0     2455 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-rw-rw-   0        0        0     4995 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-rw-rw-   0        0        0     6304 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-rw-rw-   0        0        0     2948 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-rw-rw-   0        0        0     2489 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-rw-rw-   0        0        0    20765 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-rw-rw-   0        0        0      761 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-rw-rw-   0        0        0     7267 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-rw-rw-   0        0        0      406 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.329616 NodeGraphQt-0.6.0/NodeGraphQt/nodes/
+-rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/__init__.py
+-rw-rw-rw-   0        0        0     4465 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/backdrop_node.py
+-rw-rw-rw-   0        0        0    27546 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/base_node.py
+-rw-rw-rw-   0        0        0     1253 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/base_node_circle.py
+-rw-rw-rw-   0        0        0     5817 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/group_node.py
+-rw-rw-rw-   0        0        0     4409 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/port_node.py
+-rw-rw-rw-   0        0        0      239 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.385630 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/
+-rw-rw-rw-   0        0        0        0 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/__init__.py
+-rw-rw-rw-   0        0        0     7060 2023-04-19 08:52:02.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_abstract.py
+-rw-rw-rw-   0        0        0    11022 2023-05-08 10:29:06.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_backdrop.py
+-rw-rw-rw-   0        0        0    37021 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_base.py
+-rw-rw-rw-   0        0        0    21204 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_circle.py
+-rw-rw-rw-   0        0        0    12346 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_group.py
+-rw-rw-rw-   0        0        0     4273 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_overlay_disabled.py
+-rw-rw-rw-   0        0        0     8159 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_port_in.py
+-rw-rw-rw-   0        0        0     8158 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_port_out.py
+-rw-rw-rw-   0        0        0     3749 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_text_item.py
+-rw-rw-rw-   0        0        0    23761 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/pipe.py
+-rw-rw-rw-   0        0        0    10582 2023-04-30 08:29:15.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/port.py
+-rw-rw-rw-   0        0        0     2885 2023-05-03 09:02:56.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/slicer.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.431950 NodeGraphQt-0.6.0/NodeGraphQt/widgets/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3709 2022-12-21 07:01:38.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/actions.py
+-rw-rw-rw-   0        0        0     1873 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/dialogs.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.432951 NodeGraphQt-0.6.0/NodeGraphQt/widgets/icons/
+-rw-rw-rw-   0        0        0    17542 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/icons/node_base.png
+-rw-rw-rw-   0        0        0     4550 2023-05-03 09:15:23.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/node_graph.py
+-rw-rw-rw-   0        0        0    14045 2023-05-07 22:11:12.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/node_widgets.py
+-rw-rw-rw-   0        0        0     5681 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/scene.py
+-rw-rw-rw-   0        0        0    11436 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/tab_search.py
+-rw-rw-rw-   0        0        0    55886 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/viewer.py
+-rw-rw-rw-   0        0        0     6914 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/viewer_nav.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.205588 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/
+-rw-rw-rw-   0        0        0     2746 2023-05-19 08:55:01.000000 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2543 2023-05-19 08:55:01.000000 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 08:55:01.000000 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-19 08:55:01.000000 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-19 08:55:01.000000 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2746 2023-05-19 08:55:01.458956 NodeGraphQt-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2042 2023-05-07 23:03:54.000000 NodeGraphQt-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.163579 NodeGraphQt-0.6.0/examples/
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.439952 NodeGraphQt-0.6.0/examples/hotkeys/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/examples/hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     6199 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.0/examples/hotkeys/hotkey_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.457956 NodeGraphQt-0.6.0/examples/nodes/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/examples/nodes/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-05-19 07:23:03.000000 NodeGraphQt-0.6.0/examples/nodes/basic_nodes.py
+-rw-rw-rw-   0        0        0     3671 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/examples/nodes/custom_ports_node.py
+-rw-rw-rw-   0        0        0      507 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/examples/nodes/group_node.py
+-rw-rw-rw-   0        0        0     1822 2023-05-02 10:58:55.000000 NodeGraphQt-0.6.0/examples/nodes/widget_nodes.py
+-rw-rw-rw-   0        0        0     1070 2023-05-19 08:55:01.464958 NodeGraphQt-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      123 2022-12-21 06:31:06.000000 NodeGraphQt-0.6.0/setup.py
```

### Comparing `NodeGraphQt-0.5.9/LICENSE.md` & `NodeGraphQt-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/__init__.py` & `NodeGraphQt-0.6.0/NodeGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/base/commands.py` & `NodeGraphQt-0.6.0/NodeGraphQt/base/commands.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/base/factory.py` & `NodeGraphQt-0.6.0/NodeGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/base/graph.py` & `NodeGraphQt-0.6.0/NodeGraphQt/base/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,19 @@
 
         self._sub_graphs = {}
 
         self._viewer = (
             kwargs.get('viewer') or NodeViewer(undo_stack=self._undo_stack))
         self._viewer.set_layout_direction(layout_direction)
 
+        # viewer needs a reference to the model port connection constrains
+        # for the user interaction with the live pipe.
+        self._viewer.accept_connection_types = self._model.accept_connection_types
+        self._viewer.reject_connection_types = self._model.reject_connection_types
+
         self._context_menu = {}
 
         self._register_context_menu()
         self._register_builtin_nodes()
         self._wire_signals()
 
     def __repr__(self):
@@ -870,17 +875,17 @@
             :meth:`NodeGraph.set_acyclic`
 
         Returns:
             bool: true if acyclic (default: ``True``).
         """
         return self._model.acyclic
 
-    def set_acyclic(self, mode=False):
+    def set_acyclic(self, mode=True):
         """
-        Enable the node graph to be a acyclic graph. (default: ``False``)
+        Enable the node graph to be a acyclic graph. (default: ``True``)
 
         See Also:
             :meth:`NodeGraph.acyclic`
 
         Args:
             mode (bool): true to enable acyclic.
         """
@@ -1139,14 +1144,47 @@
                 node_attrs = {node.type_: {
                     n: {'widget_type': wt} for n, wt in wid_types.items()
                 }}
                 for pname, pattrs in prop_attrs.items():
                     node_attrs[node.type_][pname].update(pattrs)
                 self.model.set_node_common_properties(node_attrs)
 
+            accept_types = node.model.__dict__.pop(
+                '_TEMP_accept_connection_types'
+            )
+            for ptype, pdata in accept_types.get(node.type_, {}).items():
+                for pname, accept_data in pdata.items():
+                    for accept_ntype, accept_ndata in accept_data.items():
+                        for accept_ptype, accept_pnames in accept_ndata.items():
+                            for accept_pname in accept_pnames:
+                                self._model.add_port_accept_connection_type(
+                                    port_name=pname,
+                                    port_type=ptype,
+                                    node_type=node.type_,
+                                    accept_pname=accept_pname,
+                                    accept_ptype=accept_ptype,
+                                    accept_ntype=accept_ntype
+                                )
+            reject_types = node.model.__dict__.pop(
+                '_TEMP_reject_connection_types'
+            )
+            for ptype, pdata in reject_types.get(node.type_, {}).items():
+                for pname, reject_data in pdata.items():
+                    for reject_ntype, reject_ndata in reject_data.items():
+                        for reject_ptype, reject_pnames in reject_ndata.items():
+                            for reject_pname in reject_pnames:
+                                self._model.add_port_reject_connection_type(
+                                    port_name=pname,
+                                    port_type=ptype,
+                                    node_type=node.type_,
+                                    reject_pname=reject_pname,
+                                    reject_ptype=reject_ptype,
+                                    reject_ntype=reject_ntype
+                                )
+
             node.NODE_NAME = self.get_unique_name(name or node.NODE_NAME)
             node.model.name = node.NODE_NAME
             node.model.selected = selected
 
             def format_color(clr):
                 if isinstance(clr, str):
                     clr = clr.strip('#')
@@ -1203,14 +1241,47 @@
             node_attrs = {node.type_: {
                 n: {'widget_type': wt} for n, wt in wid_types.items()
             }}
             for pname, pattrs in prop_attrs.items():
                 node_attrs[node.type_][pname].update(pattrs)
             self.model.set_node_common_properties(node_attrs)
 
+        accept_types = node.model.__dict__.pop(
+            '_TEMP_accept_connection_types'
+        )
+        for ptype, pdata in accept_types.get(node.type_, {}).items():
+            for pname, accept_data in pdata.items():
+                for accept_ntype, accept_ndata in accept_data.items():
+                    for accept_ptype, accept_pnames in accept_ndata.items():
+                        for accept_pname in accept_pnames:
+                            self._model.add_port_accept_connection_type(
+                                port_name=pname,
+                                port_type=ptype,
+                                node_type=node.type_,
+                                accept_pname=accept_pname,
+                                accept_ptype=accept_ptype,
+                                accept_ntype=accept_ntype
+                            )
+        reject_types = node.model.__dict__.pop(
+            '_TEMP_reject_connection_types'
+        )
+        for ptype, pdata in reject_types.get(node.type_, {}).items():
+            for pname, reject_data in pdata.items():
+                for reject_ntype, reject_ndata in reject_data.items():
+                    for reject_ptype, reject_pnames in reject_ndata.items():
+                        for reject_pname in reject_pnames:
+                            self._model.add_port_reject_connection_type(
+                                port_name=pname,
+                                port_type=ptype,
+                                node_type=node.type_,
+                                reject_pname=reject_pname,
+                                reject_ptype=reject_ptype,
+                                reject_ntype=reject_ntype
+                            )
+
         node._graph = self
         node.NODE_NAME = self.get_unique_name(node.NODE_NAME)
         node.model._graph_model = self.model
         node.model.name = node.NODE_NAME
 
         # initial node direction layout.
         node.model.layout_direction = self.layout_direction()
@@ -1550,14 +1621,18 @@
 
         # serialize graph session.
         serial_data['graph']['layout_direction'] = self.layout_direction()
         serial_data['graph']['acyclic'] = self.acyclic()
         serial_data['graph']['pipe_collision'] = self.pipe_collision()
         serial_data['graph']['pipe_slicing'] = self.pipe_slicing()
 
+        # connection constrains.
+        serial_data['graph']['accept_connection_types'] = self.model.accept_connection_types
+        serial_data['graph']['reject_connection_types'] = self.model.reject_connection_types
+
         # serialize nodes.
         for n in nodes:
             # update the node model.
             n.update_model()
 
             node_dict = n.model.to_dict
             nodes_data.update(node_dict)
@@ -1614,14 +1689,20 @@
             elif attr_name == 'acyclic':
                 self.set_acyclic(attr_value)
             elif attr_name == 'pipe_collision':
                 self.set_pipe_collision(attr_value)
             elif attr_name == 'pipe_slicing':
                 self.set_pipe_slicing(attr_value)
 
+            # connection constrains.
+            elif attr_name == 'accept_connection_types':
+                self.model.accept_connection_types = attr_value
+            elif attr_name == 'reject_connection_types':
+                self.model.reject_connection_types = attr_value
+
         # build the nodes.
         nodes = {}
         for n_id, n_data in data.get('nodes', {}).items():
             identifier = n_data['type_']
             node = self._node_factory.create_node_instance(identifier)
             if node:
                 node.NODE_NAME = n_data.get('name', node.NODE_NAME)
```

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/base/menu.py` & `NodeGraphQt-0.6.0/NodeGraphQt/base/menu.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/base/model.py` & `NodeGraphQt-0.6.0/NodeGraphQt/widgets/node_widgets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,439 +1,447 @@
 #!/usr/bin/python
-import json
-from collections import defaultdict
+from Qt import QtCore, QtWidgets
 
-from NodeGraphQt.constants import LayoutDirectionEnum, NodePropWidgetEnum
-from NodeGraphQt.errors import NodePropertyError
+from NodeGraphQt.constants import ViewerEnum, Z_VAL_NODE_WIDGET
+from NodeGraphQt.errors import NodeWidgetError
 
 
-class PortModel(object):
-    """
-    Data dump for a port object.
-    """
+class _NodeGroupBox(QtWidgets.QGroupBox):
 
-    def __init__(self, node):
-        self.node = node
-        self.type_ = ''
-        self.name = 'port'
-        self.display_name = True
-        self.multi_connection = False
-        self.visible = True
-        self.locked = False
-        self.connected_ports = defaultdict(list)
-
-    def __repr__(self):
-        return '<{}(\'{}\') object at {}>'.format(
-            self.__class__.__name__, self.name, hex(id(self)))
+    def __init__(self, label, parent=None):
+        super(_NodeGroupBox, self).__init__(parent)
+        layout = QtWidgets.QVBoxLayout(self)
+        layout.setSpacing(1)
+        self.setTitle(label)
+
+    def setTitle(self, text):
+        margin = (0, 2, 0, 0) if text else (0, 0, 0, 0)
+        self.layout().setContentsMargins(*margin)
+        super(_NodeGroupBox, self).setTitle(text)
+
+    def setTitleAlign(self, align='center'):
+        text_color = tuple(map(lambda i, j: i - j, (255, 255, 255),
+                               ViewerEnum.BACKGROUND_COLOR.value))
+        style_dict = {
+            'QGroupBox': {
+                'background-color': 'rgba(0, 0, 0, 0)',
+                'border': '0px solid rgba(0, 0, 0, 0)',
+                'margin-top': '1px',
+                'padding-bottom': '2px',
+                'padding-left': '1px',
+                'padding-right': '1px',
+                'font-size': '8pt',
+            },
+            'QGroupBox::title': {
+                'subcontrol-origin': 'margin',
+                'subcontrol-position': 'top center',
+                'color': 'rgba({0}, {1}, {2}, 100)'.format(*text_color),
+                'padding': '0px',
+            }
+        }
+        if self.title():
+            style_dict['QGroupBox']['padding-top'] = '14px'
+        else:
+            style_dict['QGroupBox']['padding-top'] = '2px'
 
-    @property
-    def to_dict(self):
-        """
-        serialize model information to a dictionary.
+        if align == 'center':
+            style_dict['QGroupBox::title']['subcontrol-position'] = 'top center'
+        elif align == 'left':
+            style_dict['QGroupBox::title']['subcontrol-position'] += 'top left'
+            style_dict['QGroupBox::title']['margin-left'] = '4px'
+        elif align == 'right':
+            style_dict['QGroupBox::title']['subcontrol-position'] += 'top right'
+            style_dict['QGroupBox::title']['margin-right'] = '4px'
+        stylesheet = ''
+        for css_class, css in style_dict.items():
+            style = '{} {{\n'.format(css_class)
+            for elm_name, elm_val in css.items():
+                style += '  {}:{};\n'.format(elm_name, elm_val)
+            style += '}\n'
+            stylesheet += style
+        self.setStyleSheet(stylesheet)
 
-        Returns:
-            dict: node port dictionary eg.
-                {
-                    'type': 'in',
-                    'name': 'port',
-                    'display_name': True,
-                    'multi_connection': False,
-                    'visible': True,
-                    'locked': False,
-                    'connected_ports': {<node_id>: [<port_name>, <port_name>]}
-                }
-        """
-        props = self.__dict__.copy()
-        props.pop('node')
-        props['connected_ports'] = dict(props.pop('connected_ports'))
-        return props
+    def add_node_widget(self, widget):
+        self.layout().addWidget(widget)
+
+    def get_node_widget(self):
+        return self.layout().itemAt(0).widget()
 
 
-class NodeModel(object):
+class NodeBaseWidget(QtWidgets.QGraphicsProxyWidget):
     """
-    Data dump for a node object.
+    This is the main wrapper class that allows a ``QtWidgets.QWidget`` to be
+    added in a :class:`NodeGraphQt.BaseNode` object.
+
+    .. inheritance-diagram:: NodeGraphQt.NodeBaseWidget
+        :parts: 1
+
+    Args:
+        parent (NodeGraphQt.BaseNode.view): parent node view.
+        name (str): property name for the parent node.
+        label (str): label text above the embedded widget.
     """
 
-    def __init__(self):
-        self.type_ = None
-        self.id = hex(id(self))
-        self.icon = None
-        self.name = 'node'
-        self.color = (13, 18, 23, 255)
-        self.border_color = (74, 84, 85, 255)
-        self.text_color = (255, 255, 255, 180)
-        self.disabled = False
-        self.selected = False
-        self.visible = True
-        self.width = 100.0
-        self.height = 80.0
-        self.pos = [0.0, 0.0]
-        self.layout_direction = LayoutDirectionEnum.HORIZONTAL.value
-
-        # BaseNode attrs.
-        self.inputs = {}
-        self.outputs = {}
-        self.port_deletion_allowed = False
-
-        # GroupNode attrs.
-        self.subgraph_session = {}
-
-        # Custom
-        self._custom_prop = {}
-
-        # node graph model set at node added time.
-        self._graph_model = None
-
-        # store the property attributes.
-        # (deleted when node is added to the graph)
-        self._TEMP_property_attrs = {}
-
-        # temp store the property widget types.
-        # (deleted when node is added to the graph)
-        self._TEMP_property_widget_types = {
-            'type_': NodePropWidgetEnum.QLABEL.value,
-            'id': NodePropWidgetEnum.QLABEL.value,
-            'icon': NodePropWidgetEnum.HIDDEN.value,
-            'name': NodePropWidgetEnum.QLINE_EDIT.value,
-            'color': NodePropWidgetEnum.COLOR_PICKER.value,
-            'border_color': NodePropWidgetEnum.HIDDEN.value,
-            'text_color': NodePropWidgetEnum.COLOR_PICKER.value,
-            'disabled': NodePropWidgetEnum.QCHECK_BOX.value,
-            'selected': NodePropWidgetEnum.HIDDEN.value,
-            'width': NodePropWidgetEnum.HIDDEN.value,
-            'height': NodePropWidgetEnum.HIDDEN.value,
-            'pos': NodePropWidgetEnum.HIDDEN.value,
-            'layout_direction': NodePropWidgetEnum.HIDDEN.value,
-            'inputs': NodePropWidgetEnum.HIDDEN.value,
-            'outputs': NodePropWidgetEnum.HIDDEN.value,
-        }
+    value_changed = QtCore.Signal(str, object)
+    """
+    Signal triggered when the ``value`` attribute has changed.
+    
+    (This is connected to the :meth: `BaseNode.set_property` function when the 
+    widget is added into the node.)
 
-    def __repr__(self):
-        return '<{}(\'{}\') object at {}>'.format(
-            self.__class__.__name__, self.name, self.id)
+    :parameters: str, object
+    :emits: property name, propety value
+    """
 
-    def add_property(self, name, value, items=None, range=None,
-                     widget_type=None, tab=None):
-        """
-        add custom property or raises an error if the property name is already
-        taken.
+    def __init__(self, parent=None, name=None, label=''):
+        super(NodeBaseWidget, self).__init__(parent)
+        self.setZValue(Z_VAL_NODE_WIDGET)
+        self._name = name
+        self._label = label
+        self._node = None
+
+    def setToolTip(self, tooltip):
+        tooltip = tooltip.replace('\n', '<br/>')
+        tooltip = '<b>{}</b><br/>{}'.format(self.name, tooltip)
+        super(NodeBaseWidget, self).setToolTip(tooltip)
+
+    def on_value_changed(self, *args, **kwargs):
+        """
+        This is the slot function that
+        Emits the widgets current :meth:`NodeBaseWidget.value` with the
+        :attr:`NodeBaseWidget.value_changed` signal.
 
         Args:
-            name (str): name of the property.
-            value (object): data.
-            items (list[str]): items used by widget type NODE_PROP_QCOMBO.
-            range (tuple): min, max values used by NODE_PROP_SLIDER.
-            widget_type (int): widget type flag.
-            tab (str): widget tab name.
-        """
-        widget_type = widget_type or NodePropWidgetEnum.HIDDEN.value
-        tab = tab or 'Properties'
-
-        if name in self.properties.keys():
-            raise NodePropertyError(
-                '"{}" reserved for default property.'.format(name))
-        if name in self._custom_prop.keys():
-            raise NodePropertyError(
-                '"{}" property already exists.'.format(name))
-
-        self._custom_prop[name] = value
-
-        if self._graph_model is None:
-            self._TEMP_property_widget_types[name] = widget_type
-            self._TEMP_property_attrs[name] = {'tab': tab}
-            if items:
-                self._TEMP_property_attrs[name]['items'] = items
-            if range:
-                self._TEMP_property_attrs[name]['range'] = range
-        else:
-            attrs = {
-                self.type_: {
-                    name: {
-                        'widget_type': widget_type,
-                        'tab': tab
-                    }
-                }
-            }
-            if items:
-                attrs[self.type_][name]['items'] = items
-            if range:
-                attrs[self.type_][name]['range'] = range
-            self._graph_model.set_node_common_properties(attrs)
+            args: not used.
+            kwargs: not used.
 
-    def set_property(self, name, value):
+        Emits:
+            str, object: <node_property_name>, <node_property_value>
         """
-        Args:
-            name (str): property name.
-            value (object): property value.
+        self.value_changed.emit(self.get_name(), self.get_value())
+
+    @property
+    def type_(self):
         """
-        if name in self.properties.keys():
-            setattr(self, name, value)
-        elif name in self._custom_prop.keys():
-            self._custom_prop[name] = value
-        else:
-            raise NodePropertyError('No property "{}"'.format(name))
+        Returns the node widget type.
 
-    def get_property(self, name):
+        Returns:
+            str: widget type.
         """
-        Args:
-            name (str): property name.
+        return str(self.__class__.__name__)
+
+    @property
+    def node(self):
+        """
+        Returns the node object this widget is embedded in.
+        (This will return ``None`` if the widget has not been added to
+        the node yet.)
 
         Returns:
-            object: property value.
+            NodeGraphQt.BaseNode: parent node.
         """
-        if name in self.properties.keys():
-            return self.properties[name]
-        return self._custom_prop.get(name)
+        return self._node
 
-    def is_custom_property(self, name):
+    def get_icon(self, name):
         """
-        Args:
-            name (str): property name.
+        Returns the default icon from the Qt framework.
 
         Returns:
-            bool: true if custom property.
+            str: icon name.
         """
-        return name in self._custom_prop
+        return self.style().standardIcon(QtWidgets.QStyle.StandardPixmap(name))
 
-    def get_widget_type(self, name):
+    def get_name(self):
         """
-        Args:
-            name (str): property name.
+        Returns the parent node property name.
 
         Returns:
-            int: node property widget type.
+            str: property name.
         """
-        model = self._graph_model
-        if model is None:
-            return self._TEMP_property_widget_types.get(name)
-        return model.get_node_common_properties(self.type_)[name]['widget_type']
+        return self._name
 
-    def get_tab_name(self, name):
+    def set_name(self, name):
         """
+        Set the property name for the parent node.
+
+        Important:
+            The property name must be set before the widget is added to
+            the node.
+
         Args:
             name (str): property name.
-
-        Returns:
-            str: name of the tab for the properties bin.
         """
-        model = self._graph_model
-        if model is None:
-            attrs = self._TEMP_property_attrs.get(name)
-            if attrs:
-                return attrs[name].get('tab')
+        if not name:
             return
-        return model.get_node_common_properties(self.type_)[name]['tab']
+        if self.node:
+            raise NodeWidgetError(
+                'Can\'t set property name widget already added to a Node'
+            )
+        self._name = name
 
-    @property
-    def properties(self):
+    def get_value(self):
         """
-        return all default node properties.
+        Returns the widgets current value.
+
+        You must re-implement this property to if you're using a custom widget.
 
         Returns:
-            dict: default node properties.
+            str: current property value.
         """
-        props = self.__dict__.copy()
-        exclude = ['_custom_prop',
-                   '_graph_model',
-                   '_TEMP_property_attrs',
-                   '_TEMP_property_widget_types']
-        [props.pop(i) for i in exclude if i in props.keys()]
-        return props
+        raise NotImplementedError
 
-    @property
-    def custom_properties(self):
+    def set_value(self, text):
+        """
+        Sets the widgets current value.
+
+        You must re-implement this property to if you're using a custom widget.
+
+        Args:
+            text (str): new text value.
+        """
+        raise NotImplementedError
+
+    def get_custom_widget(self):
         """
-        return all custom properties specified by the user.
+        Returns the embedded QWidget used in the node.
 
         Returns:
-            dict: user defined properties.
+            QtWidgets.QWidget: nested QWidget
         """
-        return self._custom_prop
+        widget = self.widget()
+        return widget.get_node_widget()
 
-    @property
-    def to_dict(self):
+    def set_custom_widget(self, widget):
+        """
+        Set the custom QWidget used in the node.
+
+        Args:
+            widget (QtWidgets.QWidget): custom.
         """
-        serialize model information to a dictionary.
+        if self.widget():
+            raise NodeWidgetError('Custom node widget already set.')
+        group = _NodeGroupBox(self._label)
+        group.add_node_widget(widget)
+        self.setWidget(group)
+
+    def get_label(self):
+        """
+        Returns the label text displayed above the embedded node widget.
 
         Returns:
-            dict: node id as the key and properties as the values eg.
-                {'0x106cf75a8': {
-                    'name': 'foo node',
-                    'color': (48, 58, 69, 255),
-                    'border_color': (85, 100, 100, 255),
-                    'text_color': (255, 255, 255, 180),
-                    'type_': 'io.github.jchanvfx.FooNode',
-                    'selected': False,
-                    'disabled': False,
-                    'visible': True,
-                    'width': 0.0,
-                    'height: 0.0,
-                    'pos': (0.0, 0.0),
-                    'layout_direction': 0,
-                    'custom': {},
-                    'inputs': {
-                        <port_name>: {<node_id>: [<port_name>, <port_name>]}
-                    },
-                    'outputs': {
-                        <port_name>: {<node_id>: [<port_name>, <port_name>]}
-                    },
-                    'input_ports': [<port_name>, <port_name>],
-                    'output_ports': [<port_name>, <port_name>],
-                    },
-                    subgraph_session: <sub graph session data>
-                }
-        """
-        node_dict = self.__dict__.copy()
-        node_id = node_dict.pop('id')
-
-        inputs = {}
-        outputs = {}
-        input_ports = []
-        output_ports = []
-        for name, model in node_dict.pop('inputs').items():
-            if self.port_deletion_allowed:
-                input_ports.append({
-                    'name': name,
-                    'multi_connection': model.multi_connection,
-                    'display_name': model.display_name,
-                })
-            connected_ports = model.to_dict['connected_ports']
-            if connected_ports:
-                inputs[name] = connected_ports
-        for name, model in node_dict.pop('outputs').items():
-            if self.port_deletion_allowed:
-                output_ports.append({
-                    'name': name,
-                    'multi_connection': model.multi_connection,
-                    'display_name': model.display_name,
-                })
-            connected_ports = model.to_dict['connected_ports']
-            if connected_ports:
-                outputs[name] = connected_ports
-        if inputs:
-            node_dict['inputs'] = inputs
-        if outputs:
-            node_dict['outputs'] = outputs
-
-        if self.port_deletion_allowed:
-            node_dict['input_ports'] = input_ports
-            node_dict['output_ports'] = output_ports
-
-        if self.subgraph_session:
-            node_dict['subgraph_session'] = self.subgraph_session
-
-        custom_props = node_dict.pop('_custom_prop', {})
-        if custom_props:
-            node_dict['custom'] = custom_props
-
-        exclude = ['_graph_model',
-                   '_TEMP_property_attrs',
-                   '_TEMP_property_widget_types']
-        [node_dict.pop(i) for i in exclude if i in node_dict.keys()]
+            str: label text.
+        """
+        return self._label
+
+    def set_label(self, label=''):
+        """
+        Sets the label text above the embedded widget.
+
+        Args:
+            label (str): new label ext.
+        """
+        if self.widget():
+            self.widget().setTitle(label)
+        self._label = label
+
 
-        return {node_id: node_dict}
+class NodeComboBox(NodeBaseWidget):
+    """
+    Displays as a ``QComboBox`` in a node.
+
+    .. inheritance-diagram:: NodeGraphQt.widgets.node_widgets.NodeComboBox
+        :parts: 1
+
+    .. note::
+        `To embed a` ``QComboBox`` `in a node see func:`
+        :meth:`NodeGraphQt.BaseNode.add_combo_menu`
+    """
+
+    def __init__(self, parent=None, name='', label='', items=None):
+        super(NodeComboBox, self).__init__(parent, name, label)
+        self.setZValue(Z_VAL_NODE_WIDGET + 1)
+        combo = QtWidgets.QComboBox()
+        combo.setMinimumHeight(24)
+        combo.addItems(items or [])
+        combo.currentIndexChanged.connect(self.on_value_changed)
+        combo.clearFocus()
+        self.set_custom_widget(combo)
 
     @property
-    def serial(self):
+    def type_(self):
+        return 'ComboNodeWidget'
+
+    def get_value(self):
         """
-        Serialize model information to a string.
+        Returns the widget current text.
 
         Returns:
-            str: serialized JSON string.
+            str: current text.
         """
-        model_dict = self.to_dict
-        return json.dumps(model_dict)
+        combo_widget = self.get_custom_widget()
+        return str(combo_widget.currentText())
+
+    def set_value(self, text=''):
+        combo_widget = self.get_custom_widget()
+        if type(text) is list:
+            combo_widget.clear()
+            combo_widget.addItems(text)
+            return
+        if text != self.get_value():
+            index = combo_widget.findText(text, QtCore.Qt.MatchExactly)
+            combo_widget.setCurrentIndex(index)
+
+    def add_item(self, item):
+        combo_widget = self.get_custom_widget()
+        combo_widget.addItem(item)
+
+    def add_items(self, items=None):
+        if items:
+            combo_widget = self.get_custom_widget()
+            combo_widget.addItems(items)
+
+    def all_items(self):
+        combo_widget = self.get_custom_widget()
+        return [combo_widget.itemText(i) for i in range(combo_widget.count())]
+
+    def sort_items(self, reversed=False):
+        items = sorted(self.all_items(), reverse=reversed)
+        combo_widget = self.get_custom_widget()
+        combo_widget.clear()
+        combo_widget.addItems(items)
+
+    def clear(self):
+        combo_widget = self.get_custom_widget()
+        combo_widget.clear()
 
 
-class NodeGraphModel(object):
+class NodeLineEdit(NodeBaseWidget):
     """
-    Data dump for a node graph.
+    Displays as a ``QLineEdit`` in a node.
+
+    .. inheritance-diagram:: NodeGraphQt.widgets.node_widgets.NodeLineEdit
+        :parts: 1
+
+    .. note::
+        `To embed a` ``QLineEdit`` `in a node see func:`
+        :meth:`NodeGraphQt.BaseNode.add_text_input`
     """
 
-    def __init__(self):
-        self.__common_node_props = {}
+    def __init__(self, parent=None, name='', label='', text=''):
+        super(NodeLineEdit, self).__init__(parent, name, label)
+        bg_color = ViewerEnum.BACKGROUND_COLOR.value
+        text_color = tuple(map(lambda i, j: i - j, (255, 255, 255),
+                               bg_color))
+        text_sel_color = text_color
+        style_dict = {
+            'QLineEdit': {
+                'background': 'rgba({0},{1},{2},20)'.format(*bg_color),
+                'border': '1px solid rgb({0},{1},{2})'
+                          .format(*ViewerEnum.GRID_COLOR.value),
+                'border-radius': '3px',
+                'color': 'rgba({0},{1},{2},150)'.format(*text_color),
+                'selection-background-color': 'rgba({0},{1},{2},100)'
+                                              .format(*text_sel_color),
+            }
+        }
+        stylesheet = ''
+        for css_class, css in style_dict.items():
+            style = '{} {{\n'.format(css_class)
+            for elm_name, elm_val in css.items():
+                style += '  {}:{};\n'.format(elm_name, elm_val)
+            style += '}\n'
+            stylesheet += style
+        ledit = QtWidgets.QLineEdit()
+        ledit.setText(text)
+        ledit.setStyleSheet(stylesheet)
+        ledit.setAlignment(QtCore.Qt.AlignCenter)
+        ledit.editingFinished.connect(self.on_value_changed)
+        ledit.clearFocus()
+        self.set_custom_widget(ledit)
+        self.widget().setMaximumWidth(140)
 
-        self.nodes = {}
-        self.session = ''
-        self.acyclic = True
-        self.pipe_collision = False
-        self.pipe_slicing = True
-        self.layout_direction = LayoutDirectionEnum.HORIZONTAL.value
+    @property
+    def type_(self):
+        return 'LineEditNodeWidget'
 
-    def common_properties(self):
+    def get_value(self):
         """
-        Return all common node properties.
+        Returns the widgets current text.
 
         Returns:
-            dict: common node properties.
-                eg.
-                    {'nodeGraphQt.nodes.FooNode': {
-                        'my_property': {
-                            'widget_type': 0,
-                            'tab': 'Properties',
-                            'items': ['foo', 'bar', 'test'],
-                            'range': (0, 100)
-                            }
-                        }
-                    }
+            str: current text.
         """
-        return self.__common_node_props
+        return str(self.get_custom_widget().text())
 
-    def set_node_common_properties(self, attrs):
+    def set_value(self, text=''):
         """
-        Store common node properties.
+        Sets the widgets current text.
 
         Args:
-            attrs (dict): common node properties.
-                eg.
-                    {'nodeGraphQt.nodes.FooNode': {
-                        'my_property': {
-                            'widget_type': 0,
-                            'tab': 'Properties',
-                            'items': ['foo', 'bar', 'test'],
-                            'range': (0, 100)
-                            }
-                        }
-                    }
-        """
-        for node_type in attrs.keys():
-            node_props = attrs[node_type]
-
-            if node_type not in self.__common_node_props.keys():
-                self.__common_node_props[node_type] = node_props
-                continue
-
-            for prop_name, prop_attrs in node_props.items():
-                common_props = self.__common_node_props[node_type]
-                if prop_name not in common_props.keys():
-                    common_props[prop_name] = prop_attrs
-                    continue
-                common_props[prop_name].update(prop_attrs)
-
-    def get_node_common_properties(self, node_type):
+            text (str): new text.
         """
-        Return all the common properties for a registered node.
+        if text != self.get_value():
+            self.get_custom_widget().setText(text)
+            self.on_value_changed()
 
-        Args:
-            node_type (str): node type.
+
+class NodeCheckBox(NodeBaseWidget):
+    """
+    Displays as a ``QCheckBox`` in a node.
+
+    .. inheritance-diagram:: NodeGraphQt.widgets.node_widgets.NodeCheckBox
+        :parts: 1
+
+    .. note::
+        `To embed a` ``QCheckBox`` `in a node see func:`
+        :meth:`NodeGraphQt.BaseNode.add_checkbox`
+    """
+
+    def __init__(self, parent=None, name='', label='', text='', state=False):
+        super(NodeCheckBox, self).__init__(parent, name, label)
+        _cbox = QtWidgets.QCheckBox(text)
+        text_color = tuple(map(lambda i, j: i - j, (255, 255, 255),
+                               ViewerEnum.BACKGROUND_COLOR.value))
+        style_dict = {
+            'QCheckBox': {
+                'color': 'rgba({0},{1},{2},150)'.format(*text_color),
+            }
+        }
+        stylesheet = ''
+        for css_class, css in style_dict.items():
+            style = '{} {{\n'.format(css_class)
+            for elm_name, elm_val in css.items():
+                style += '  {}:{};\n'.format(elm_name, elm_val)
+            style += '}\n'
+            stylesheet += style
+        _cbox.setStyleSheet(stylesheet)
+        _cbox.setChecked(state)
+        _cbox.setMinimumWidth(80)
+        font = _cbox.font()
+        font.setPointSize(11)
+        _cbox.setFont(font)
+        _cbox.stateChanged.connect(self.on_value_changed)
+        self.set_custom_widget(_cbox)
+        self.widget().setMaximumWidth(140)
+
+    @property
+    def type_(self):
+        return 'CheckboxNodeWidget'
+
+    def get_value(self):
+        """
+        Returns the widget checked state.
 
         Returns:
-            dict: node common properties.
+            bool: checked state.
         """
-        return self.__common_node_props.get(node_type)
+        return self.get_custom_widget().isChecked()
 
+    def set_value(self, state=False):
+        """
+        Sets the widget checked state.
 
-if __name__ == '__main__':
-    p = PortModel(None)
-    # print(p.to_dict)
-
-    n = NodeModel()
-    n.inputs[p.name] = p
-    n.add_property('foo', 'bar')
-
-    print('-'*100)
-    print('property keys\n')
-    print(list(n.properties.keys()))
-    print('-'*100)
-    print('to_dict\n')
-    for k, v in n.to_dict[n.id].items():
-        print(k, v)
+        Args:
+            state (bool): check state.
+        """
+        if state != self.get_value():
+            self.get_custom_widget().setChecked(state)
```

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/base/node.py` & `NodeGraphQt-0.6.0/NodeGraphQt/base/node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/constants.py` & `NodeGraphQt-0.6.0/NodeGraphQt/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     :py:mod:`NodeGraphQt.constants.PipeEnum`
     """
     #: default width.
     WIDTH = 1.2
     #: default color.
     COLOR = (175, 95, 30, 255)
     #: pipe color to a node when it's disabled.
-    DISABLED_COLOR = (190, 20, 20, 255)
+    DISABLED_COLOR = (200, 60, 60, 255)
     #: pipe color when selected or mouse over.
     ACTIVE_COLOR = (70, 255, 220, 255)
     #: pipe color to a node when it's selected.
     HIGHLIGHT_COLOR = (232, 184, 13, 255)
     #: draw connection as a line.
     DRAW_TYPE_DEFAULT = 0
     #: draw connection as dashed lines.
```

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/nodes_palette.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/nodes_tree.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/nodes/backdrop_node.py` & `NodeGraphQt-0.6.0/NodeGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/nodes/base_node.py` & `NodeGraphQt-0.6.0/NodeGraphQt/nodes/base_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,19 +82,24 @@
         if self.get_property(name) == value:
             return
 
         if name == 'visible':
             if self.graph:
                 undo_cmd = NodeVisibleCmd(self, value)
                 if push_undo:
-                    undo_stack = self.graph.undo_stack()
-                    undo_stack.push(undo_cmd)
+                    self.graph.undo_stack().push(undo_cmd)
                 else:
                     undo_cmd.redo()
                 return
+        elif name == 'disabled':
+            # redraw the connected pipes in the scene.
+            ports = self.view.inputs + self.view.outputs
+            for port in ports:
+                for pipe in port.connected_pipes:
+                    pipe.update()
         super(BaseNode, self).set_property(name, value, push_undo)
 
     def set_layout_direction(self, value=0):
         """
         Sets the node layout direction to either horizontal or vertical on
         the current node only.
 
@@ -648,14 +653,132 @@
             dict: {<output_port>: <node_list>}
         """
         nodes = OrderedDict()
         for p in self.output_ports():
             nodes[p] = [cp.node() for cp in p.connected_ports()]
         return nodes
 
+    def add_accept_port_type(self, port, port_type_data):
+        """
+        Add a accept constrain to a specified node port.
+
+        Once a constrain has been added only ports of that type specified will
+        be allowed a pipe connection.
+
+        port type data example
+
+        .. highlight:: python
+        .. code-block:: python
+            {
+                'port_name': 'foo'
+                'port_type': PortTypeEnum.IN.value
+                'node_type': 'io.github.jchanvfx.NodeClass'
+            }
+
+        See Also:
+            :meth:`NodeGraphQt.BaseNode.accepted_port_types`
+
+        Args:
+            port (NodeGraphQt.Port): port to assign constrain to.
+            port_type_data (dict): port type data to accept a connection
+        """
+        node_ports = self._inputs + self._outputs
+        if port not in node_ports:
+            raise PortError('Node does not contain port: "{}"'.format(port))
+
+        self._model.add_port_accept_connection_type(
+            port_name=port.name(),
+            port_type=port.type_(),
+            node_type=self.type_,
+            accept_pname=port_type_data['port_name'],
+            accept_ptype=port_type_data['port_type'],
+            accept_ntype=port_type_data['node_type']
+        )
+
+    def accepted_port_types(self, port):
+        """
+        Returns a dictionary of connection constrains of the port types
+        that allow for a pipe connection to this node.
+
+        Args:
+            port (NodeGraphQt.Port): port object.
+
+        Returns:
+            dict: {<node_type>: {<port_type>: [<port_name>]}}
+        """
+        ports = self._inputs + self._outputs
+        if port not in ports:
+            raise PortError('Node does not contain port "{}"'.format(port))
+
+        accepted_types = self.graph.model.port_accept_connection_types(
+            node_type=self.type_,
+            port_type=port.type_(),
+            port_name=port.name()
+        )
+        return accepted_types
+
+    def add_reject_port_type(self, port, port_type_data):
+        """
+        Add a reject constrain to a specified node port.
+
+        Once a constrain has been added only ports of that type specified will
+        NOT be allowed a pipe connection.
+
+        port type data example
+
+        .. highlight:: python
+        .. code-block:: python
+            {
+                'port_name': 'foo'
+                'port_type': PortTypeEnum.IN.value
+                'node_type': 'io.github.jchanvfx.NodeClass'
+            }
+
+        See Also:
+            :meth:`NodeGraphQt.Port.rejected_port_types`
+
+        Args:
+            port (NodeGraphQt.Port): port to assign constrain to.
+            port_type_data (dict): port type data to reject a connection
+        """
+        node_ports = self._inputs + self._outputs
+        if port not in node_ports:
+            raise PortError('Node does not contain port: "{}"'.format(port))
+
+        self._model.add_port_reject_connection_type(
+            port_name=port.name(),
+            port_type=port.type_(),
+            node_type=self.type_,
+            reject_pname=port_type_data['port_name'],
+            reject_ptype=port_type_data['port_type'],
+            reject_ntype=port_type_data['node_type']
+        )
+
+    def rejected_port_types(self, port):
+        """
+        Returns a dictionary of connection constrains of the port types
+        that are NOT allowed for a pipe connection to this node.
+
+        Args:
+            port (NodeGraphQt.Port): port object.
+
+        Returns:
+            dict: {<node_type>: {<port_type>: [<port_name>]}}
+        """
+        ports = self._inputs + self._outputs
+        if port not in ports:
+            raise PortError('Node does not contain port "{}"'.format(port))
+
+        rejected_types = self.graph.model.port_reject_connection_types(
+            node_type=self.type_,
+            port_type=port.type_(),
+            port_name=port.name()
+        )
+        return rejected_types
+
     def on_input_connected(self, in_port, out_port):
         """
         Callback triggered when a new pipe connection is made.
 
         *The default of this function does nothing re-implement if you require
         logic to run for this event.*
```

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/nodes/base_node_circle.py` & `NodeGraphQt-0.6.0/NodeGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/nodes/group_node.py` & `NodeGraphQt-0.6.0/NodeGraphQt/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/nodes/port_node.py` & `NodeGraphQt-0.6.0/NodeGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_abstract.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_backdrop.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_backdrop.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,16 +254,24 @@
                     continue
                 if isinstance(item, AbstractNodeItem):
                     nodes.append(item)
         return nodes
 
     def calc_backdrop_size(self, nodes=None):
         nodes = nodes or self.get_nodes(True)
+        if nodes:
+            nodes_rect = self._combined_rect(nodes)
+        else:
+            center = self.mapToScene(self.boundingRect().center())
+            nodes_rect = QtCore.QRectF(
+                center.x(), center.y(),
+                self._min_size[0], self._min_size[1]
+            )
+
         padding = 40
-        nodes_rect = self._combined_rect(nodes)
         return {
             'pos': [
                 nodes_rect.x() - padding, nodes_rect.y() - padding
             ],
             'width': nodes_rect.width() + (padding * 2),
             'height': nodes_rect.height() + (padding * 2)
         }
```

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_base.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -757,23 +757,31 @@
         # disable overlay item.
         self._x_item.proxy_mode = self._proxy_mode
 
         # node widget visibility.
         for w in self._widgets.values():
             w.widget().setVisible(visible)
 
+        # port text is not visible in vertical layout.
+        if self.layout_direction is LayoutDirectionEnum.VERTICAL.value:
+            port_text_visible = False
+        else:
+            port_text_visible = visible
+
         # input port text visibility.
         for port, text in self._input_items.items():
             if port.display_name:
-                text.setVisible(visible)
+                text.setVisible(port_text_visible)
 
         # output port text visibility.
         for port, text in self._output_items.items():
             if port.display_name:
-                text.setVisible(visible)
+                text.setVisible(port_text_visible)
+
+
 
         self._text_item.setVisible(visible)
         self._icon_item.setVisible(visible)
 
     @property
     def icon(self):
         return self._properties['icon']
```

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_circle.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_group.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_overlay_disabled.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_port_in.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_port_out.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/node_text_item.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/port.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/qgraphics/slicer.py` & `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/widgets/actions.py` & `NodeGraphQt-0.6.0/NodeGraphQt/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/widgets/dialogs.py` & `NodeGraphQt-0.6.0/NodeGraphQt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/widgets/icons/node_base.png` & `NodeGraphQt-0.6.0/NodeGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/widgets/node_graph.py` & `NodeGraphQt-0.6.0/NodeGraphQt/widgets/node_graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/widgets/scene.py` & `NodeGraphQt-0.6.0/NodeGraphQt/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/widgets/tab_search.py` & `NodeGraphQt-0.6.0/NodeGraphQt/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/widgets/viewer.py` & `NodeGraphQt-0.6.0/NodeGraphQt/widgets/viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 from Qt import QtGui, QtCore, QtWidgets
 
 from NodeGraphQt.base.menu import BaseMenu
 from NodeGraphQt.constants import (
     LayoutDirectionEnum,
     PortTypeEnum,
+    PipeEnum,
     PipeLayoutEnum,
     ViewerEnum,
-    Z_VAL_NODE_WIDGET
+    Z_VAL_PIPE,
 )
 from NodeGraphQt.qgraphics.node_abstract import AbstractNodeItem
 from NodeGraphQt.qgraphics.node_backdrop import BackdropNodeItem
 from NodeGraphQt.qgraphics.pipe import PipeItem, LivePipeItem
 from NodeGraphQt.qgraphics.port import PortItem
 from NodeGraphQt.qgraphics.slicer import SlicerPipeItem
 from NodeGraphQt.widgets.dialogs import BaseDialog, FileDialog
@@ -84,27 +85,29 @@
         self._start_port = None
         self._origin_pos = None
         self._previous_pos = QtCore.QPoint(int(self.width() / 2),
                                            int(self.height() / 2))
         self._prev_selection_nodes = []
         self._prev_selection_pipes = []
         self._node_positions = {}
+
         self._rubber_band = QtWidgets.QRubberBand(
             QtWidgets.QRubberBand.Rectangle, self
         )
         self._rubber_band.isActive = False
 
         text_color = QtGui.QColor(*tuple(map(
             lambda i, j: i - j, (255, 255, 255),
             ViewerEnum.BACKGROUND_COLOR.value
         )))
         text_color.setAlpha(50)
         self._cusor_text = QtWidgets.QGraphicsTextItem()
+        self._cusor_text.setFlag(self._cusor_text.ItemIsSelectable, False)
         self._cusor_text.setDefaultTextColor(text_color)
-        self._cusor_text.setZValue(Z_VAL_NODE_WIDGET + 1)
+        self._cusor_text.setZValue(Z_VAL_PIPE - 1)
         font = self._cusor_text.font()
         font.setPointSize(7)
         self._cusor_text.setFont(font)
         self.scene().addItem(self._cusor_text)
 
         self._LIVE_PIPE = LivePipeItem()
         self._LIVE_PIPE.setVisible(False)
@@ -145,14 +148,19 @@
         self.RMB_state = False
         self.MMB_state = False
         self.ALT_state = False
         self.CTRL_state = False
         self.SHIFT_state = False
         self.COLLIDING_state = False
 
+        # connection constrains.
+        # TODO: maybe this should be a reference to the graph model instead?
+        self.accept_connection_types = None
+        self.reject_connection_types = None
+
     def __repr__(self):
         return '<{}() object at {}>'.format(
             self.__class__.__name__, hex(id(self)))
 
     def focusInEvent(self, event):
         """
         Args:
@@ -464,15 +472,32 @@
             rect = QtCore.QRect(self._previous_pos, QtCore.QSize())
             rect = rect.normalized()
             map_rect = self.mapToScene(rect).boundingRect()
             self.scene().update(map_rect)
             self._rubber_band.setGeometry(rect)
             self._rubber_band.isActive = True
 
-        if self.LMB_state and (self.SHIFT_state or self.CTRL_state):
+        # stop here so we don't select a node.
+        # (ctrl modifier can be used for something else in future.)
+        if self.CTRL_state:
+            return
+
+        # allow new live pipe with the shift modifier on port that allow
+        # for multi connection.
+        if self.SHIFT_state:
+            if pipes:
+                pipes[0].reset()
+                port = pipes[0].port_from_pos(map_pos, reverse=True)
+                if not port.locked and port.multi_connection:
+                    self._cusor_text.setPlainText('')
+                    self._cusor_text.setVisible(False)
+                    self.start_live_connection(port)
+
+            # return here as the default behaviour unselects nodes with
+            # the shift modifier.
             return
 
         if not self._LIVE_PIPE.isVisible():
             super(NodeViewer, self).mousePressEvent(event)
 
     def mouseReleaseEvent(self, event):
         if event.button() == QtCore.Qt.LeftButton:
@@ -563,15 +588,16 @@
             previous_pos = self.mapToScene(self._previous_pos)
             current_pos = self.mapToScene(event.pos())
             delta = previous_pos - current_pos
             self._set_viewer_pan(delta.x(), delta.y())
 
         if not self.ALT_state:
             if self.SHIFT_state or self.CTRL_state:
-                self._cusor_text.setPos(self.mapToScene(event.pos()))
+                if not self._LIVE_PIPE.isVisible():
+                    self._cusor_text.setPos(self.mapToScene(event.pos()))
 
         if self.LMB_state and self._rubber_band.isActive:
             rect = QtCore.QRect(self._origin_pos, event.pos()).normalized()
             # if the rubber band is too small, do not show it.
             if max(rect.width(), rect.height()) > 5:
                 if not self._rubber_band.isVisible():
                     self._rubber_band.show()
@@ -669,14 +695,18 @@
         self.SHIFT_state = event.modifiers() == QtCore.Qt.ShiftModifier
 
         # Todo: find a better solution to catch modifier keys.
         if event.modifiers() == (QtCore.Qt.AltModifier | QtCore.Qt.ShiftModifier):
             self.ALT_state = True
             self.SHIFT_state = True
 
+        if self._LIVE_PIPE.isVisible():
+            super(NodeViewer, self).keyPressEvent(event)
+            return
+
         # show cursor text
         overlay_text = None
         self._cusor_text.setVisible(False)
         if not self.ALT_state:
             if self.SHIFT_state:
                 overlay_text = '\n    SHIFT:\n    Toggle/Extend Selection'
             elif self.CTRL_state:
@@ -723,34 +753,45 @@
         """
         if not self._LIVE_PIPE.isVisible():
             return
         if not self._start_port:
             return
 
         pos = event.scenePos()
-        color_mode = None
+        pointer_color = None
         for item in self.scene().items(pos):
-            if isinstance(item, PortItem):
-                x = item.boundingRect().width() / 2
-                y = item.boundingRect().height() / 2
-                pos = item.scenePos()
-                pos.setX(pos.x() + x)
-                pos.setY(pos.y() + y)
-                if item == self._start_port:
-                    break
-                color_mode = 'accept'
-                if self.acyclic:
-                    if item.node == self._start_port.node:
-                        color_mode = 'reject'
-                    elif item.port_type == self._start_port.port_type:
-                        color_mode = 'reject'
+            if not isinstance(item, PortItem):
+                continue
+
+            x = item.boundingRect().width() / 2
+            y = item.boundingRect().height() / 2
+            pos = item.scenePos()
+            pos.setX(pos.x() + x)
+            pos.setY(pos.y() + y)
+            if item == self._start_port:
+                break
+            pointer_color = PipeEnum.HIGHLIGHT_COLOR.value
+            accept = self._validate_accept_connection(self._start_port, item)
+            if not accept:
+                pointer_color = [150, 60, 255]
+                break
+            reject = self._validate_reject_connection(self._start_port, item)
+            if reject:
+                pointer_color = [150, 60, 255]
                 break
 
+            if self.acyclic:
+                if item.node == self._start_port.node:
+                    pointer_color = PipeEnum.DISABLED_COLOR.value
+                elif item.port_type == self._start_port.port_type:
+                    pointer_color = PipeEnum.DISABLED_COLOR.value
+            break
+
         self._LIVE_PIPE.draw_path(
-            self._start_port, cursor_pos=pos, color_mode=color_mode
+            self._start_port, cursor_pos=pos, color=pointer_color
         )
 
     def sceneMousePressEvent(self, event):
         """
         triggered mouse press event for the scene (takes priority over viewer event).
          - detect selected pipe and start connection.
          - remap Shift and Ctrl modifier.
@@ -846,14 +887,86 @@
                 The event handler from the QtWidgets.QGraphicsScene
         """
         if event.button() != QtCore.Qt.MiddleButton:
             self.apply_live_connection(event)
 
     # --- port connections ---
 
+    def _validate_accept_connection(self, from_port, to_port):
+        """
+        Check if a pipe connection is allowed if there are a constrains set
+        on the ports.
+
+        Args:
+            from_port (PortItem):
+            to_port (PortItem):
+
+        Returns:
+            bool: true to allow connection.
+        """
+        to_ptype = to_port.port_type
+        from_ptype = from_port.port_type
+
+        to_data = self.accept_connection_types.get(to_port.node.type_) or {}
+        constraints = to_data.get(to_ptype, {}).get(to_port.name, {})
+        accept_data = constraints.get(from_port.node.type_, {})
+
+        accepted_pnames = accept_data.get(from_ptype)
+        if accepted_pnames:
+            if from_port.name in accepted_pnames:
+                return True
+            return False
+
+        from_data = self.accept_connection_types.get(from_port.node.type_) or {}
+        constraints = from_data.get(from_ptype, {}).get(from_port.name, {})
+        accept_data = constraints.get(to_port.node.type_, {})
+
+        accepted_pnames = accept_data.get(to_ptype)
+        if accepted_pnames:
+            if from_port.name in accepted_pnames:
+                return True
+            return False
+        return True
+
+    def _validate_reject_connection(self, from_port, to_port):
+        """
+        Check if a pipe connection is NOT allowed if there are a constrains set
+        on the ports.
+
+        Args:
+            from_port (PortItem):
+            to_port (PortItem):
+
+        Returns:
+            bool: true to reject connection.
+        """
+        to_ptype = to_port.port_type
+        from_ptype = from_port.port_type
+
+        to_data = self.reject_connection_types.get(to_port.node.type_) or {}
+        constraints = to_data.get(to_ptype, {}).get(to_port.name, {})
+        reject_data = constraints.get(from_port.node.type_, {})
+
+        rejected_pnames = reject_data.get(from_ptype)
+        if rejected_pnames:
+            if from_port.name in rejected_pnames:
+                return True
+            return False
+
+        from_data = self.reject_connection_types.get(from_port.node.type_) or {}
+        constraints = from_data.get(from_ptype, {}).get(from_port.name, {})
+        reject_data = constraints.get(to_port.node.type_, {})
+
+        rejected_pnames = reject_data.get(to_ptype)
+        if rejected_pnames:
+            if to_port.name in rejected_pnames:
+                return True
+            return False
+        return False
+
     def apply_live_connection(self, event):
         """
         triggered mouse press/release event for the scene.
         - verifies the live connection pipe.
         - makes a connection pipe if valid.
         - emits the "connection changed" signal.
 
@@ -893,26 +1006,44 @@
             self.end_live_connection()
             return
 
         else:
             if self._start_port is end_port:
                 return
 
+        # if connection to itself
+        same_node_connection = end_port.node == self._start_port.node
+        if not self.acyclic:
+            # allow a node cycle connection.
+            same_node_connection = False
+
+        # constrain check
+        accept_connection = self._validate_accept_connection(
+            self._start_port, end_port
+        )
+        reject_connection = self._validate_reject_connection(
+            self._start_port, end_port
+        )
+
         # restore connection check.
         restore_connection = any([
             # if the end port is locked.
             end_port.locked,
             # if same port type.
             end_port.port_type == self._start_port.port_type,
             # if connection to itself.
-            end_port.node == self._start_port.node,
+            same_node_connection,
             # if end port is the start port.
             end_port == self._start_port,
             # if detached port is the end port.
-            self._detached_port == end_port
+            self._detached_port == end_port,
+            # if a port has a accept port type constrain.
+            not accept_connection,
+            # if a port has a reject port type constrain.
+            reject_connection
         ])
         if restore_connection:
             if self._detached_port:
                 to_port = self._detached_port or end_port
                 self.establish_connection(self._start_port, to_port)
                 self._detached_port = None
             self.end_live_connection()
```

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt/widgets/viewer_nav.py` & `NodeGraphQt-0.6.0/NodeGraphQt/widgets/viewer_nav.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt.egg-info/PKG-INFO` & `NodeGraphQt-0.6.0/NodeGraphQt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.5.9
+Version: 0.6.0
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
@@ -21,36 +21,34 @@
 
 <p align="center">
     <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">
     <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/logo.png" title="logo">
     </a>
 </p>
 
-``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
+NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
 applications.
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
 
 ## Install
 
-NodeGraphQt is avaliable on The Python Package Index (PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
+NodeGraphQt is avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/NodeGraphQt) so it can be installed with:
 ```
 pip install NodeGraphQt
 ```
 or you can download previous versions from the [releases](https://github.com/jchanvfx/NodeGraphQt/releases) page.
 
 
 ## Documentation
 
 <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">https://jchanvfx.github.io/NodeGraphQt</a>
 
-See the [basic_example.py](/examples/basic_example.py) python script from this repo.
-
-More examples can be found in the API documentation:<br>
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_overview.html#simple-example
+See the [basic_example.py](/examples/basic_example.py) script to get started or check out the API example overview 
+<a href="https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_overview.html#simple-example" target="_blank">here.</a>
 
 ## Vertical Layout
 
 https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png" width="800" title="Vertical Layout">
 
@@ -61,8 +59,9 @@
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif" width="600" title="Pipe Layout">
 
 ## Custom Widgets
 
 https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png" width="600" title="Properties Bin">
-<img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="600" title="Node Palette">
+
+<img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="450" title="Node Palette">
```

#### html2text {}

```diff
@@ -1,33 +1,31 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.5.9 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.0 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: PySide2 License-File:
 LICENSE.md # NodeGraphQt
   [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
                                    logo.png]
-``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be
-implemented and re-purposed into applications. [https://
+NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented
+and re-purposed into applications. [https://raw.githubusercontent.com/jchanvfx/
+NodeGraphQt/main/docs/_images/screenshot.png] ## Install NodeGraphQt is
+avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/
+NodeGraphQt) so it can be installed with: ``` pip install NodeGraphQt ``` or
+you can download previous versions from the [releases](https://github.com/
+jchanvfx/NodeGraphQt/releases) page. ## Documentation https://
+jchanvfx.github.io/NodeGraphQt See the [basic_example.py](/examples/
+basic_example.py) script to get started or check out the API example overview
+here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/html/
+examples/ex_pipe.html#layout-direction [https://raw.githubusercontent.com/
+jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png] ## Pipe Layout
+https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-
+styles [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/
+_images/pipe_layout_types.gif] ## Custom Widgets https://jchanvfx.github.io/
+NodeGraphQt/api/html/custom_widgets.html [https://raw.githubusercontent.com/
+jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png] [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
-screenshot.png] ## Install NodeGraphQt is avaliable on The Python Package Index
-(PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
-``` pip install NodeGraphQt ``` or you can download previous versions from the
-[releases](https://github.com/jchanvfx/NodeGraphQt/releases) page. ##
-Documentation https://jchanvfx.github.io/NodeGraphQt See the [basic_example.py]
-(/examples/basic_example.py) python script from this repo. More examples can be
-found in the API documentation:
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/
-ex_overview.html#simple-example ## Vertical Layout https://jchanvfx.github.io/
-NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction [https://
-raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
-vertical_layout.png] ## Pipe Layout https://jchanvfx.github.io/NodeGraphQt/api/
-html/examples/ex_pipe.html#layout-styles [https://raw.githubusercontent.com/
-jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif] ## Custom Widgets
-https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html [https://
-raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png]
-[https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
 nodes_palette.png]
```

### Comparing `NodeGraphQt-0.5.9/NodeGraphQt.egg-info/SOURCES.txt` & `NodeGraphQt-0.6.0/NodeGraphQt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/PKG-INFO` & `NodeGraphQt-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.5.9
+Version: 0.6.0
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
@@ -21,36 +21,34 @@
 
 <p align="center">
     <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">
     <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/logo.png" title="logo">
     </a>
 </p>
 
-``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
+NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
 applications.
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
 
 ## Install
 
-NodeGraphQt is avaliable on The Python Package Index (PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
+NodeGraphQt is avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/NodeGraphQt) so it can be installed with:
 ```
 pip install NodeGraphQt
 ```
 or you can download previous versions from the [releases](https://github.com/jchanvfx/NodeGraphQt/releases) page.
 
 
 ## Documentation
 
 <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">https://jchanvfx.github.io/NodeGraphQt</a>
 
-See the [basic_example.py](/examples/basic_example.py) python script from this repo.
-
-More examples can be found in the API documentation:<br>
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_overview.html#simple-example
+See the [basic_example.py](/examples/basic_example.py) script to get started or check out the API example overview 
+<a href="https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_overview.html#simple-example" target="_blank">here.</a>
 
 ## Vertical Layout
 
 https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png" width="800" title="Vertical Layout">
 
@@ -61,8 +59,9 @@
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif" width="600" title="Pipe Layout">
 
 ## Custom Widgets
 
 https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png" width="600" title="Properties Bin">
-<img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="600" title="Node Palette">
+
+<img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="450" title="Node Palette">
```

#### html2text {}

```diff
@@ -1,33 +1,31 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.5.9 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.0 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: PySide2 License-File:
 LICENSE.md # NodeGraphQt
   [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
                                    logo.png]
-``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be
-implemented and re-purposed into applications. [https://
+NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented
+and re-purposed into applications. [https://raw.githubusercontent.com/jchanvfx/
+NodeGraphQt/main/docs/_images/screenshot.png] ## Install NodeGraphQt is
+avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/
+NodeGraphQt) so it can be installed with: ``` pip install NodeGraphQt ``` or
+you can download previous versions from the [releases](https://github.com/
+jchanvfx/NodeGraphQt/releases) page. ## Documentation https://
+jchanvfx.github.io/NodeGraphQt See the [basic_example.py](/examples/
+basic_example.py) script to get started or check out the API example overview
+here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/html/
+examples/ex_pipe.html#layout-direction [https://raw.githubusercontent.com/
+jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png] ## Pipe Layout
+https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-
+styles [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/
+_images/pipe_layout_types.gif] ## Custom Widgets https://jchanvfx.github.io/
+NodeGraphQt/api/html/custom_widgets.html [https://raw.githubusercontent.com/
+jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png] [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
-screenshot.png] ## Install NodeGraphQt is avaliable on The Python Package Index
-(PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
-``` pip install NodeGraphQt ``` or you can download previous versions from the
-[releases](https://github.com/jchanvfx/NodeGraphQt/releases) page. ##
-Documentation https://jchanvfx.github.io/NodeGraphQt See the [basic_example.py]
-(/examples/basic_example.py) python script from this repo. More examples can be
-found in the API documentation:
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/
-ex_overview.html#simple-example ## Vertical Layout https://jchanvfx.github.io/
-NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction [https://
-raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
-vertical_layout.png] ## Pipe Layout https://jchanvfx.github.io/NodeGraphQt/api/
-html/examples/ex_pipe.html#layout-styles [https://raw.githubusercontent.com/
-jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif] ## Custom Widgets
-https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html [https://
-raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png]
-[https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
 nodes_palette.png]
```

### Comparing `NodeGraphQt-0.5.9/README.md` & `NodeGraphQt-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,36 +3,34 @@
 
 <p align="center">
     <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">
     <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/logo.png" title="logo">
     </a>
 </p>
 
-``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
+NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
 applications.
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
 
 ## Install
 
-NodeGraphQt is avaliable on The Python Package Index (PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
+NodeGraphQt is avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/NodeGraphQt) so it can be installed with:
 ```
 pip install NodeGraphQt
 ```
 or you can download previous versions from the [releases](https://github.com/jchanvfx/NodeGraphQt/releases) page.
 
 
 ## Documentation
 
 <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">https://jchanvfx.github.io/NodeGraphQt</a>
 
-See the [basic_example.py](/examples/basic_example.py) python script from this repo.
-
-More examples can be found in the API documentation:<br>
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_overview.html#simple-example
+See the [basic_example.py](/examples/basic_example.py) script to get started or check out the API example overview 
+<a href="https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_overview.html#simple-example" target="_blank">here.</a>
 
 ## Vertical Layout
 
 https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png" width="800" title="Vertical Layout">
 
@@ -43,8 +41,9 @@
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif" width="600" title="Pipe Layout">
 
 ## Custom Widgets
 
 https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png" width="600" title="Properties Bin">
-<img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="600" title="Node Palette">
+
+<img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="450" title="Node Palette">
```

#### html2text {}

```diff
@@ -1,24 +1,22 @@
  # NodeGraphQt
   [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
                                    logo.png]
-``NodeGraphQt`` is a node graph UI framework for `PySide2` that can be
-implemented and re-purposed into applications. [https://
+NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented
+and re-purposed into applications. [https://raw.githubusercontent.com/jchanvfx/
+NodeGraphQt/main/docs/_images/screenshot.png] ## Install NodeGraphQt is
+avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/
+NodeGraphQt) so it can be installed with: ``` pip install NodeGraphQt ``` or
+you can download previous versions from the [releases](https://github.com/
+jchanvfx/NodeGraphQt/releases) page. ## Documentation https://
+jchanvfx.github.io/NodeGraphQt See the [basic_example.py](/examples/
+basic_example.py) script to get started or check out the API example overview
+here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/html/
+examples/ex_pipe.html#layout-direction [https://raw.githubusercontent.com/
+jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png] ## Pipe Layout
+https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-
+styles [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/
+_images/pipe_layout_types.gif] ## Custom Widgets https://jchanvfx.github.io/
+NodeGraphQt/api/html/custom_widgets.html [https://raw.githubusercontent.com/
+jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png] [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
-screenshot.png] ## Install NodeGraphQt is avaliable on The Python Package Index
-(PyPI) here https://pypi.org/project/NodeGraphQt so it can be installed with:
-``` pip install NodeGraphQt ``` or you can download previous versions from the
-[releases](https://github.com/jchanvfx/NodeGraphQt/releases) page. ##
-Documentation https://jchanvfx.github.io/NodeGraphQt See the [basic_example.py]
-(/examples/basic_example.py) python script from this repo. More examples can be
-found in the API documentation:
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/
-ex_overview.html#simple-example ## Vertical Layout https://jchanvfx.github.io/
-NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction [https://
-raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
-vertical_layout.png] ## Pipe Layout https://jchanvfx.github.io/NodeGraphQt/api/
-html/examples/ex_pipe.html#layout-styles [https://raw.githubusercontent.com/
-jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif] ## Custom Widgets
-https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html [https://
-raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png]
-[https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
 nodes_palette.png]
```

### Comparing `NodeGraphQt-0.5.9/examples/hotkeys/hotkey_functions.py` & `NodeGraphQt-0.6.0/examples/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/examples/nodes/basic_nodes.py` & `NodeGraphQt-0.6.0/examples/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/examples/nodes/custom_ports_node.py` & `NodeGraphQt-0.6.0/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/examples/nodes/widget_nodes.py` & `NodeGraphQt-0.6.0/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.5.9/setup.cfg` & `NodeGraphQt-0.6.0/setup.cfg`

 * *Files identical despite different names*

