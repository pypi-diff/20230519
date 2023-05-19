# Comparing `tmp/pyaedt-0.6.75.tar.gz` & `tmp/pyaedt-0.6.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.75.tar", last modified: Fri May 12 16:29:05 2023, max compression
+gzip compressed data, was "pyaedt-0.6.76.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.6.75.tar` & `pyaedt-0.6.76.tar`

### file list

```diff
@@ -1,252 +1,252 @@
--rw-r--r--   0        0        0     1111 2023-03-24 16:10:16.742763 pyaedt-0.6.75/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-04 14:08:42.179957 pyaedt-0.6.75/README.md
--rw-r--r--   0        0        0     2634 2023-05-12 15:52:06.115764 pyaedt-0.6.75/pyaedt/__init__.py
--rw-r--r--   0        0        0    26253 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    89244 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    41260 2023-05-04 22:05:09.593531 pyaedt-0.6.75/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17009 2023-04-06 11:56:42.332868 pyaedt-0.6.75/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19795 2023-04-06 11:56:42.332868 pyaedt-0.6.75/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4374 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4539 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   127521 2023-04-27 08:03:43.579230 pyaedt-0.6.75/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75493 2023-04-27 13:10:02.023398 pyaedt-0.6.75/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12433 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    37014 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    57603 2023-05-11 09:46:53.726038 pyaedt-0.6.75/pyaedt/circuit.py
--rw-r--r--   0        0        0    10034 2023-03-24 16:10:18.758234 pyaedt-0.6.75/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    57391 2023-05-04 10:56:05.337017 pyaedt-0.6.75/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-04-27 07:01:19.524177 pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-04-27 07:01:19.524177 pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1092 2023-04-27 07:01:19.524177 pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-04-27 07:01:19.539803 pyaedt-0.6.75/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-04-27 07:01:19.539803 pyaedt-0.6.75/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-04-27 07:01:19.539803 pyaedt-0.6.75/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-04-27 07:01:19.539803 pyaedt-0.6.75/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-04-27 07:01:19.539803 pyaedt-0.6.75/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-04-27 07:01:19.555426 pyaedt-0.6.75/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-04-27 07:01:19.555426 pyaedt-0.6.75/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-04-27 07:01:19.555426 pyaedt-0.6.75/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-04-27 07:01:19.571050 pyaedt-0.6.75/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-04-27 07:01:19.571050 pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-04-27 07:01:19.571050 pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-04-27 07:01:19.586676 pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-04-27 07:01:19.602300 pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-04-27 07:01:19.602300 pyaedt-0.6.75/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-04-27 07:01:19.617927 pyaedt-0.6.75/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-04-27 07:01:19.617927 pyaedt-0.6.75/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-04-27 07:01:19.617927 pyaedt-0.6.75/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    23386 2023-04-18 21:46:42.426459 pyaedt-0.6.75/pyaedt/downloads.py
--rw-r--r--   0        0        0   134259 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-04-06 16:51:57.478550 pyaedt-0.6.75/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    92731 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.820698 pyaedt-0.6.75/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    32856 2023-04-06 17:43:43.595268 pyaedt-0.6.75/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0    40043 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0      937 2023-03-24 16:10:18.820698 pyaedt-0.6.75/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      324 2023-03-24 16:10:18.820698 pyaedt-0.6.75/pyaedt/edb_core/edb_data/edb_builder.py
--rw-r--r--   0        0        0     1166 2023-03-24 16:10:18.820698 pyaedt-0.6.75/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12141 2023-04-28 15:10:16.972093 pyaedt-0.6.75/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65580 2023-04-13 10:23:17.415379 pyaedt-0.6.75/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20305 2023-04-06 16:51:57.478550 pyaedt-0.6.75/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     4724 2023-04-17 09:21:51.433903 pyaedt-0.6.75/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61111 2023-04-27 17:41:51.680530 pyaedt-0.6.75/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32298 2023-04-06 16:51:57.478550 pyaedt-0.6.75/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0    99826 2023-04-25 22:05:43.936271 pyaedt-0.6.75/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36282 2023-04-25 22:05:43.936271 pyaedt-0.6.75/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    33728 2023-05-09 13:57:21.715124 pyaedt-0.6.75/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     4147 2023-03-24 16:10:18.820698 pyaedt-0.6.75/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2425 2023-03-27 19:28:28.383108 pyaedt-0.6.75/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-04-25 22:05:43.936271 pyaedt-0.6.75/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    60863 2023-04-25 22:05:43.936271 pyaedt-0.6.75/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2844 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7706 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4646 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11333 2023-05-02 12:13:55.192015 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21750 2023-04-03 14:45:49.232236 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-03-24 16:10:18.867622 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    49064 2023-05-02 12:59:04.166088 pyaedt-0.6.75/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33242 2023-04-07 10:17:20.946469 pyaedt-0.6.75/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    43680 2023-04-06 17:49:40.538145 pyaedt-0.6.75/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    46611 2023-05-09 09:08:50.766572 pyaedt-0.6.75/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    57133 2023-04-06 16:51:57.478550 pyaedt-0.6.75/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   108893 2023-04-28 11:15:40.689926 pyaedt-0.6.75/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11275 2023-04-26 16:24:45.451996 pyaedt-0.6.75/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-03-24 16:10:18.867622 pyaedt-0.6.75/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3291 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/emit_core/EmitConstants.py
--rw-r--r--   0        0        0     1074 2023-05-03 22:08:50.820887 pyaedt-0.6.75/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0        2 2023-03-24 16:10:18.867622 pyaedt-0.6.75/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-05-03 22:08:50.820887 pyaedt-0.6.75/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    12191 2023-05-12 15:07:06.269545 pyaedt-0.6.75/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-03-27 12:10:05.425190 pyaedt-0.6.75/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    11758 2023-03-24 16:10:18.867622 pyaedt-0.6.75/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.867622 pyaedt-0.6.75/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-04-28 11:15:40.689926 pyaedt-0.6.75/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83387 2023-04-26 10:50:39.177934 pyaedt-0.6.75/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-04-07 12:58:03.133395 pyaedt-0.6.75/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    21891 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3416 2023-03-30 13:11:17.942263 pyaedt-0.6.75/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    67958 2023-05-10 08:50:46.369435 pyaedt-0.6.75/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-03-24 16:10:18.883250 pyaedt-0.6.75/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-03-24 16:10:18.883250 pyaedt-0.6.75/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-04-28 11:15:40.689926 pyaedt-0.6.75/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62296 2023-04-07 12:58:03.133395 pyaedt-0.6.75/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11301 2023-03-24 16:10:18.883250 pyaedt-0.6.75/pyaedt/generic/process.py
--rw-r--r--   0        0        0    20326 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3466 2023-03-24 16:10:18.883250 pyaedt-0.6.75/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60355 2023-03-24 16:10:18.898857 pyaedt-0.6.75/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-03-24 16:10:18.898857 pyaedt-0.6.75/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   252855 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/hfss.py
--rw-r--r--   0        0        0    82916 2023-04-06 11:56:42.332868 pyaedt-0.6.75/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   154940 2023-05-04 12:30:42.836343 pyaedt-0.6.75/pyaedt/icepak.py
--rw-r--r--   0        0        0   118454 2023-05-10 06:31:48.338096 pyaedt-0.6.75/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24259 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-04-03 09:31:32.851623 pyaedt-0.6.75/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-03-24 16:10:18.907751 pyaedt-0.6.75/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-04-03 09:31:32.851623 pyaedt-0.6.75/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-03-30 19:37:04.658681 pyaedt-0.6.75/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-03-30 19:37:04.658681 pyaedt-0.6.75/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-03-24 16:10:18.907751 pyaedt-0.6.75/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-04-18 21:46:42.442098 pyaedt-0.6.75/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-03-24 16:10:18.907751 pyaedt-0.6.75/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3829 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14076 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    19994 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-04-18 21:46:42.442098 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16809 2023-04-07 12:58:03.149048 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120831 2023-04-05 05:51:09.186354 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   194513 2023-04-28 15:10:16.972093 pyaedt-0.6.75/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   115362 2023-05-10 15:44:48.349712 pyaedt-0.6.75/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11332 2023-03-24 16:10:18.945688 pyaedt-0.6.75/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   127894 2023-05-10 08:50:46.369435 pyaedt-0.6.75/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.945688 pyaedt-0.6.75/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    31549 2023-05-05 11:21:23.857681 pyaedt-0.6.75/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49002 2023-04-06 10:00:10.649919 pyaedt-0.6.75/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59516 2023-05-04 12:57:11.212325 pyaedt-0.6.75/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53100 2023-04-28 15:10:16.972093 pyaedt-0.6.75/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12588 2023-04-13 16:03:19.110009 pyaedt-0.6.75/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42270 2023-04-25 22:05:43.967519 pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32723 2023-05-08 20:33:32.647460 pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8157 2023-03-24 16:10:18.945688 pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63043 2023-04-13 10:51:44.555559 pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15094 2023-03-24 16:10:18.945688 pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.945688 pyaedt-0.6.75/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    31983 2023-04-13 10:51:44.555559 pyaedt-0.6.75/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68020 2023-04-28 15:10:16.972093 pyaedt-0.6.75/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6897 2023-04-25 22:05:43.967519 pyaedt-0.6.75/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    52442 2023-05-12 11:17:44.639145 pyaedt-0.6.75/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    31270 2023-04-13 15:33:56.717485 pyaedt-0.6.75/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49837 2023-04-25 22:05:43.967519 pyaedt-0.6.75/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.961334 pyaedt-0.6.75/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65608 2023-04-25 22:05:43.967519 pyaedt-0.6.75/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    21640 2023-04-25 22:05:43.983120 pyaedt-0.6.75/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30094 2023-04-27 07:01:19.617927 pyaedt-0.6.75/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   114236 2023-05-04 09:41:18.539853 pyaedt-0.6.75/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71549 2023-03-24 16:10:18.961334 pyaedt-0.6.75/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-05-11 09:46:53.726038 pyaedt-0.6.75/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51910 2023-03-24 16:10:18.961334 pyaedt-0.6.75/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40297 2023-04-25 22:05:43.983120 pyaedt-0.6.75/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82846 2023-03-24 16:10:18.961334 pyaedt-0.6.75/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28306 2023-03-24 16:43:00.406402 pyaedt-0.6.75/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53168 2023-04-07 14:18:16.263614 pyaedt-0.6.75/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11919 2023-03-24 16:10:18.961334 pyaedt-0.6.75/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    26048 2023-03-31 15:10:27.419349 pyaedt-0.6.75/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   172944 2023-05-10 12:27:31.281987 pyaedt-0.6.75/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64104 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   119693 2023-05-10 15:44:48.349712 pyaedt-0.6.75/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33226 2023-04-07 14:18:16.263614 pyaedt-0.6.75/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    28652 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103276 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   125048 2023-05-04 22:05:09.593531 pyaedt-0.6.75/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95851 2023-05-10 17:22:00.121611 pyaedt-0.6.75/pyaedt/q3d.py
--rw-r--r--   0        0        0    10556 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-04-18 21:46:42.457739 pyaedt-0.6.75/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7601 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10373 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4134 2023-05-09 19:48:15.535200 pyaedt-0.6.75/pyproject.toml
--rw-r--r--   0        0        0    15129 1970-01-01 00:00:00.000000 pyaedt-0.6.75/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-18 13:27:42.185924 pyaedt-0.6.76/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-18 13:27:42.185924 pyaedt-0.6.76/README.md
+-rw-r--r--   0        0        0     2634 2023-05-19 13:13:55.389500 pyaedt-0.6.76/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26596 2023-05-18 14:05:55.328452 pyaedt-0.6.76/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    86515 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    41260 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17009 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19795 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4374 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4539 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   128111 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75493 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12433 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    37014 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    62746 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10034 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    61908 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1092 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-05-18 13:27:43.920373 pyaedt-0.6.76/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-05-18 13:27:43.920373 pyaedt-0.6.76/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-05-18 13:27:43.920373 pyaedt-0.6.76/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-05-18 13:27:43.935986 pyaedt-0.6.76/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-05-18 13:27:43.935986 pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-05-18 13:27:43.935986 pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-05-18 13:27:43.951639 pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-05-18 13:27:43.967239 pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-05-18 13:27:43.967239 pyaedt-0.6.76/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    23386 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/downloads.py
+-rw-r--r--   0        0        0   142256 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    92731 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    32856 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    40043 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      324 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/edb_builder.py
+-rw-r--r--   0        0        0     1166 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12141 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65580 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20305 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     4724 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61111 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32298 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0    99826 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36282 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    33728 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     4147 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2425 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    64993 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2844 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7706 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4646 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11333 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21750 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    49064 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33242 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    43680 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    46611 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    57133 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   108971 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11275 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit.py
+-rw-r--r--   0        0        0     3555 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3291 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit_core/EmitConstants.py
+-rw-r--r--   0        0        0     1074 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0        2 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-05-19 05:07:06.470308 pyaedt-0.6.76/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    12191 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    11758 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83387 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3395 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    68697 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    25808 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     6989 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62296 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11301 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3466 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60355 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   252855 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/hfss.py
+-rw-r--r--   0        0        0    82916 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   166996 2023-05-19 06:55:34.512608 pyaedt-0.6.76/pyaedt/icepak.py
+-rw-r--r--   0        0        0   118454 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24259 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3695 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     2380 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     3731 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     3818 2023-05-19 06:53:58.810568 pyaedt-0.6.76/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14076 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    19994 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16809 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120831 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   194513 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   115362 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11332 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   127894 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    31549 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49002 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59516 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53100 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12588 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42270 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    32723 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8157 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63043 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15094 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    31982 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68135 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6897 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    52442 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    31270 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49837 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65608 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    21640 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    30094 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   114658 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71549 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51910 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40297 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82846 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28306 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53168 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11919 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    26048 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   172950 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64104 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   119149 2023-05-19 05:07:06.470308 pyaedt-0.6.76/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33226 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    28652 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103276 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   125048 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95851 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10556 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7601 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10373 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4134 2023-05-19 13:13:55.389500 pyaedt-0.6.76/pyproject.toml
+-rw-r--r--   0        0        0    15129 1970-01-01 00:00:00.000000 pyaedt-0.6.76/PKG-INFO
```

### Comparing `pyaedt-0.6.75/LICENSE` & `pyaedt-0.6.76/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/README.md` & `pyaedt-0.6.76/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/__init__.py` & `pyaedt-0.6.76/pyaedt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.75"
+__version__ = "0.6.76"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
 from pyaedt.generic.general_methods import _pythonver
```

### Comparing `pyaedt-0.6.75/pyaedt/aedt_logger.py` & `pyaedt-0.6.76/pyaedt/aedt_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,14 +313,18 @@
             List of messages for the specified project and design.
 
         """
         project_name = project_name or self._project_name
         design_name = design_name or self._design_name
         if self._log_on_desktop or aedt_messages:
             global_message_data = self._desktop.GetMessages("", "", level)
+            # if a 3d component is open, GetMessages without the project name argument returns messages with
+            # "(3D Component)" appended to project name
+            if not any(msg in global_message_data for msg in self._desktop.GetMessages(project_name, "", 0)):
+                project_name = project_name + " (3D Component)"
             return MessageList(global_message_data, project_name, design_name)
         return MessageList([], project_name, design_name)
 
     def add_error_message(self, message_text, level=None):
         """
         Add a type 2 "Error" message to the message manager tree.
```

### Comparing `pyaedt-0.6.75/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.76/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/application/Analysis.py` & `pyaedt-0.6.76/pyaedt/application/Analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1888,15 +1888,15 @@
             while not os.path.exists(queue_file_completed):
                 time.sleep(0.5)
         return True
 
     @pyaedt_function_handler()
     def submit_job(
         self, clustername, aedt_full_exe_path=None, numnodes=1, numcores=32, wait_for_license=True, setting_file=None
-    ):
+    ):  # pragma: no cover
         """Submit a job to be solved on a cluster.
 
         Parameters
         ----------
         clustername : str
             Name of the cluster to submit the job to.
         aedt_full_exe_path : str, optional
@@ -1917,72 +1917,17 @@
             ID of the job.
 
         References
         ----------
 
         >>> oDesktop.SubmitJob
         """
-        project_file = self.project_file
-        project_path = self.project_path
-        if not aedt_full_exe_path:
-            version = self.odesktop.GetVersion()[2:6]
-            if version >= "22.2":
-                version_name = "v" + version.replace(".", "")
-            else:
-                version_name = "AnsysEM" + version
-            if os.path.exists(r"\\" + clustername + r"\AnsysEM\{}\Win64\ansysedt.exe".format(version_name)):
-                aedt_full_exe_path = (
-                    r"\\\\\\\\" + clustername + r"\\\\AnsysEM\\\\{}\\\\Win64\\\\ansysedt.exe".format(version_name)
-                )
-            elif os.path.exists(r"\\" + clustername + r"\AnsysEM\{}\Linux64\ansysedt".format(version_name)):
-                aedt_full_exe_path = (
-                    r"\\\\\\\\" + clustername + r"\\\\AnsysEM\\\\{}\\\\Linux64\\\\ansysedt".format(version_name)
-                )
-            else:
-                self.logger.error("AEDT shared path does not exist. Please provide a full path.")
-                return False
-        else:
-            if not os.path.exists(aedt_full_exe_path):
-                self.logger.error("AEDT shared path does not exist. Provide a full path.")
-                return False
-            aedt_full_exe_path.replace("\\", "\\\\")
-
-        self.close_project()
-        path_file = os.path.dirname(__file__)
-        destination_reg = os.path.join(project_path, "Job_settings.areg")
-        if not setting_file:
-            setting_file = os.path.join(path_file, "..", "misc", "Job_Settings.areg")
-        shutil.copy(setting_file, destination_reg)
-
-        f1 = open_file(destination_reg, "w")
-        with open_file(setting_file) as f:
-            lines = f.readlines()
-            for line in lines:
-                if "\\	$begin" == line[:8]:
-                    lin = "\\	$begin \\'{}\\'\\\n".format(clustername)
-                    f1.write(lin)
-                elif "\\	$end" == line[:6]:
-                    lin = "\\	$end \\'{}\\'\\\n".format(clustername)
-                    f1.write(lin)
-                elif "NumCores" in line:
-                    lin = "\\	\\	\\	\\	NumCores={}\\\n".format(numcores)
-                    f1.write(lin)
-                elif "NumNodes=1" in line:
-                    lin = "\\	\\	\\	\\	NumNodes={}\\\n".format(numnodes)
-                    f1.write(lin)
-                elif "ProductPath" in line:
-                    lin = "\\	\\	ProductPath =\\'{}\\'\\\n".format(aedt_full_exe_path)
-                    f1.write(lin)
-                elif "WaitForLicense" in line:
-                    lin = "\\	\\	WaitForLicense={}\\\n".format(str(wait_for_license).lower())
-                    f1.write(lin)
-                else:
-                    f1.write(line)
-        f1.close()
-        return self.odesktop.SubmitJob(os.path.join(project_path, "Job_settings.areg"), project_file)
+        return self.desktop_class.submit_job(
+            self.project_file, clustername, aedt_full_exe_path, numnodes, numcores, wait_for_license, setting_file
+        )
 
     @pyaedt_function_handler()
     def _export_touchstone(
         self, solution_name=None, sweep_name=None, file_name=None, variations=None, variations_value=None
     ):
         """Export the Touchstone file to a local folder.
```

### Comparing `pyaedt-0.6.75/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.76/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.76/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.76/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.76/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.76/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.76/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/application/Design.py` & `pyaedt-0.6.76/pyaedt/application/Design.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,28 +185,38 @@
         self._boundaries = []
         self._project_datasets = {}
         self._design_datasets = {}
         main_module = sys.modules["__main__"]
         self.close_on_exit = close_on_exit
         self._global_logger = pyaedt_logger
         self._logger = pyaedt_logger
-
+        self._desktop_class = None
         if "pyaedt_initialized" not in dir(main_module):
-            desktop = Desktop(
+            self._desktop_class = Desktop(
                 specified_version,
                 non_graphical,
                 new_desktop_session,
                 close_on_exit,
                 student_version,
                 machine,
                 port,
                 aedt_process_id,
             )
             self.release_on_exit = True
         else:
+            self._desktop_class = Desktop(
+                settings.aedt_version,
+                settings.non_graphical,
+                False,
+                close_on_exit,
+                student_version,
+                settings.machine,
+                settings.port,
+                settings.aedt_process_id,
+            )
             self.release_on_exit = False
 
         self.student_version = main_module.student_version
         if self.student_version:
             settings.disable_bounding_box_sat = True
         self._mttime = None
         self._design_type = design_type
@@ -239,16 +249,26 @@
         self._variable_manager = VariableManager(self)
         self._project_datasets = []
         self._design_datasets = []
         # _mtime = self.project_time_stamp
         self.logger.info("Variable Manager initialized")
 
     @property
+    def desktop_class(self):
+        """``Desktop`` class.
+
+        Returns
+        -------
+        :class:`pyaedt.desktop.Desktop`
+        """
+        return self._desktop_class
+
+    @property
     def project_datasets(self):
-        """Dictionary of Project Datasets.
+        """Dictionary of project datasets.
 
         Returns
         -------
         Dict[str, :class:`pyaedt.application.Variables.DataSet`]
         """
         if not self._project_datasets:
             self._project_datasets = self._get_project_datasets()
```

### Comparing `pyaedt-0.6.75/pyaedt/application/JobManager.py` & `pyaedt-0.6.76/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/application/Variables.py` & `pyaedt-0.6.76/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.76/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/application/design_solutions.py` & `pyaedt-0.6.76/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/circuit.py` & `pyaedt-0.6.76/pyaedt/circuit.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import glob
 import io
 import math
 import os
 import re
 import shutil
 
+from pyaedt import Hfss3dLayout
 from pyaedt.application.AnalysisNexxim import FieldAnalysisCircuit
 from pyaedt.generic import ibis_reader
 from pyaedt.generic.DataHandlers import from_rkm_to_aedt
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Boundary import CurrentSinSource
@@ -1547,7 +1548,118 @@
         else:
             self.logger.error("Design not solved")
             return None
 
         shutil.copy(latest_file, filepath)
         filename = os.path.basename(latest_file)
         return os.path.join(filepath, filename)
+
+    @pyaedt_function_handler()
+    def connect_circuit_models_from_multi_zone_cutout(
+        self, project_connections, edb_zones_dict, ports=None, schematic_units="mm", model_inc=50
+    ):
+        """Connect circuit model from a multizone clipped project.
+
+        Parameters
+        ----------
+        project_connections : dic[str][str]
+            Dictionary of project connections returned from the
+            ``edb.get_connected_ports_from_multizone_cutout()`` method.
+        edb_zones_dict : dict[str][EDB PolygonData]
+            Dictionary of zones returned by the ``edb.copy_zones()`` method.
+        ports : dict[str][str]
+            dictionary return from command edb.cutout_multizone_layout(). These ports are the ones created before
+            processing the multizone clipping. Like for instance ports created on components resulting from previous
+            automated workflow execution.
+        schematic_units : str, optional
+            Units for the schematic, such as ``"mm"`` or ``"in"``. The
+            default is ``"mm"``.
+        model_inc : float, optional
+            Distance increment for adding models. The default is ``50``.
+
+        Returns
+        -------
+        bool
+            ``True`` when succeessful, ``False`` when failed.
+
+        Examples
+        --------
+        These commands show how to get input arguments described in this method:
+        - project_connections
+        - edb_zone_dict
+        -
+        >>> edb = Edb(edb_file)
+        >>> edb_zones = edb.copy_zones(r"C:\Temp\test")
+        >>> defined_ports, project_connections = edb.cutout_multizone_layout(edb_zones, common_reference_net)
+        >>> circ = Circuit()
+        >>> circ.connect_circuit_models_from_multi_zone_cutout(project_connexions, edb_zones, defined_ports)
+        """
+        if project_connections and edb_zones_dict:
+            self.modeler.schematic_units = schematic_units
+            inc = model_inc
+            ind = 1
+            for edb_file in list(edb_zones_dict.keys()):
+                hfss3d_layout_model = self.import_edb_in_circuit(edb_path=edb_file)
+                model_position = [ind * inc, 0]
+                hfss3d_layout_model.location = model_position
+                ind += 1
+            for connection in project_connections:
+                pin1 = None
+                pin2 = None
+                model1 = next(
+                    cmp for cmp in list(self.modeler.schematic.components.values()) if connection[0][0] in cmp.name
+                )
+                if model1:
+                    try:
+                        pin1 = next(pin for pin in model1.pins if pin.name == connection[0][1])
+                    except:
+                        print("failed to get pin1")
+                model2 = next(
+                    cmp for cmp in list(self.modeler.schematic.components.values()) if connection[1][0] in cmp.name
+                )
+                if model2:
+                    try:
+                        pin2 = next(pin for pin in model2.pins if pin.name == connection[1][1])
+                    except:
+                        print("failed to get pin2")
+                if pin1 and pin2:
+                    pin1.connect_to_component(component_pin=pin2, use_wire=False)
+            for model_name, ports in ports.items():
+                if any(cmp for cmp in list(self.modeler.schematic.components.values()) if model_name in cmp.name):
+                    model = next(
+                        cmp for cmp in list(self.modeler.schematic.components.values()) if model_name in cmp.name
+                    )
+                    if model:
+                        for port_name in ports:
+                            model_pin = next(pin for pin in model.pins if pin.name == port_name)
+                            if model_pin:
+                                self.modeler.components.create_interface_port(port_name, model_pin.location)
+            self.save_project()
+            return True
+        return False
+
+    @pyaedt_function_handler()
+    def import_edb_in_circuit(self, edb_path):
+        """Import an EDB design inside a Circuit project.
+
+        Parameters
+        ----------
+        edb_path : str
+            Path of the EDB file to copy.
+
+        Returns
+        -------
+            ``Hfss3DLayout`` component instance.
+        """
+        hfss = Hfss3dLayout(edb_path)
+        hfss.edit_cosim_options(
+            simulate_missing_solution=True,
+            setup_override_name=hfss.setup_names[0],
+            sweep_override_name=hfss.existing_analysis_sweeps[0].split(":")[1].strip(" "),
+        )
+        active_project = hfss.odesktop.SetActiveProject(hfss.project_name)
+        active_project.CopyDesign(hfss.design_name)
+        active_project = self.odesktop.SetActiveProject(self.project_name)
+        active_project.Paste()
+        hfss_3d_layout_model = self.modeler.schematic.add_subcircuit_3dlayout(hfss.design_name)
+        hfss.close_project(save_project=False)
+        return hfss_3d_layout_model
```

### Comparing `pyaedt-0.6.75/pyaedt/common_rpc.py` & `pyaedt-0.6.76/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/desktop.py` & `pyaedt-0.6.76/pyaedt/desktop.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import datetime
 import gc
 import logging
 import os
 import pkgutil
 import re
+import shutil
 import socket
 import sys
 import tempfile
 import threading
 import time
 import traceback
 import warnings
@@ -41,14 +42,15 @@
 from pyaedt import settings
 from pyaedt.generic.general_methods import _pythonver
 from pyaedt.generic.general_methods import active_sessions
 from pyaedt.generic.general_methods import com_active_sessions
 from pyaedt.generic.general_methods import grpc_active_sessions
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import is_ironpython
+from pyaedt.generic.general_methods import open_file
 from pyaedt.misc import list_installed_ansysem
 
 pathname = os.path.dirname(__file__)
 
 pyaedtversion = __version__
 
 modules = [tup[1] for tup in pkgutil.iter_modules()]
@@ -569,14 +571,16 @@
         if not settings.remote_api:
             self._logger.info("Python version %s", sys.version)
         self.odesktop = self._main.oDesktop
         settings.aedt_version = self.odesktop.GetVersion()[0:6]
         settings.machine = self.machine
         settings.port = self.port
         self.aedt_process_id = self.odesktop.GetProcessID()  # bit of cleanup for consistency if used in future
+        settings.aedt_process_id = self.aedt_process_id
+        settings.is_student = student_version
         self._logger.info("AEDT %s Build Date %s", self.odesktop.GetVersion(), self.odesktop.GetBuildDateTimeString())
 
         if _com == "ironpython":
             sys.path.append(
                 os.path.join(self._main.sDesktopinstallDirectory, "common", "commonfiles", "IronPython", "DLLs")
             )
 
@@ -1569,7 +1573,108 @@
                         .replace("##PYTHON_SCRIPT##", full_path)
                     )
                     build_file_data = build_file_data.replace(" % version", "")
                     out_file.write(build_file_data)
         if aedt_version >= "2023.2":
             write_toolkit_config(os.path.join(toolkit_dir, product), lib_dir, toolkit_name, toolkit=toolkit)
         self.logger.info("{} toolkit installed.".format(toolkit_name))
+
+    @pyaedt_function_handler()
+    def submit_job(
+        self,
+        project_file,
+        clustername,
+        aedt_full_exe_path=None,
+        numnodes=1,
+        numcores=32,
+        wait_for_license=True,
+        setting_file=None,
+    ):  # pragma: no cover
+        """Submit a job to be solved on a cluster.
+
+        Parameters
+        ----------
+        project : str
+            Full path to the project.
+        clustername : str
+            Name of the cluster to submit the job to.
+        aedt_full_exe_path : str, optional
+            Full path to the AEDT executable file. The default is ``None``, in which
+            case ``"/clustername/AnsysEM/AnsysEM2x.x/Win64/ansysedt.exe"`` is used.
+        numnodes : int, optional
+            Number of nodes. The default is ``1``.
+        numcores : int, optional
+            Number of cores. The default is ``32``.
+        wait_for_license : bool, optional
+             Whether to wait for the license to be validated. The default is ``True``.
+        setting_file : str, optional
+            Name of the file to use as a template. The default value is ``None``.
+
+        Returns
+        -------
+        int
+            ID of the job.
+
+        References
+        ----------
+
+        >>> oDesktop.SubmitJob
+        """
+
+        project_path = os.path.dirname(project_file)
+        project_name = os.path.basename(project_file).split(".")[0]
+        if not aedt_full_exe_path:
+            version = self.odesktop.GetVersion()[2:6]
+            if version >= "22.2":
+                version_name = "v" + version.replace(".", "")
+            else:
+                version_name = "AnsysEM" + version
+            if os.path.exists(r"\\" + clustername + r"\AnsysEM\{}\Win64\ansysedt.exe".format(version_name)):
+                aedt_full_exe_path = (
+                    r"\\\\\\\\" + clustername + r"\\\\AnsysEM\\\\{}\\\\Win64\\\\ansysedt.exe".format(version_name)
+                )
+            elif os.path.exists(r"\\" + clustername + r"\AnsysEM\{}\Linux64\ansysedt".format(version_name)):
+                aedt_full_exe_path = (
+                    r"\\\\\\\\" + clustername + r"\\\\AnsysEM\\\\{}\\\\Linux64\\\\ansysedt".format(version_name)
+                )
+            else:
+                self.logger.error("AEDT shared path does not exist. Provide a full path.")
+                return False
+        else:
+            if not os.path.exists(aedt_full_exe_path):
+                self.logger.error("AEDT shared path does not exist. Provide a full path.")
+                return False
+            aedt_full_exe_path.replace("\\", "\\\\")
+        if project_name in self.project_list:
+            self.odesktop.CloseProject(project_name)
+        path_file = os.path.dirname(__file__)
+        destination_reg = os.path.join(project_path, "Job_settings.areg")
+        if not setting_file:
+            setting_file = os.path.join(path_file, "misc", "Job_Settings.areg")
+        shutil.copy(setting_file, destination_reg)
+
+        f1 = open_file(destination_reg, "w")
+        with open_file(setting_file) as f:
+            lines = f.readlines()
+            for line in lines:
+                if "\\	$begin" == line[:8]:
+                    lin = "\\	$begin \\'{}\\'\\\n".format(clustername)
+                    f1.write(lin)
+                elif "\\	$end" == line[:6]:
+                    lin = "\\	$end \\'{}\\'\\\n".format(clustername)
+                    f1.write(lin)
+                elif "NumCores" in line:
+                    lin = "\\	\\	\\	\\	NumCores={}\\\n".format(numcores)
+                    f1.write(lin)
+                elif "NumNodes=1" in line:
+                    lin = "\\	\\	\\	\\	NumNodes={}\\\n".format(numnodes)
+                    f1.write(lin)
+                elif "ProductPath" in line:
+                    lin = "\\	\\	ProductPath =\\'{}\\'\\\n".format(aedt_full_exe_path)
+                    f1.write(lin)
+                elif "WaitForLicense" in line:
+                    lin = "\\	\\	WaitForLicense={}\\\n".format(str(wait_for_license).lower())
+                    f1.write(lin)
+                else:
+                    f1.write(line)
+        f1.close()
+        return self.odesktop.SubmitJob(os.path.join(project_path, "Job_settings.areg"), project_file)
```

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.76/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/downloads.py` & `pyaedt-0.6.76/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb.py` & `pyaedt-0.6.76/pyaedt/edb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains the ``Edb`` class.
 
 This module is implicitily loaded in HFSS 3D Layout when launched.
 
 """
+from itertools import combinations
 import os
 import re
 import shutil
 import sys
 import tempfile
 import time
 import traceback
@@ -56,14 +57,15 @@
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
 from pyaedt.generic.general_methods import is_windows
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.process import SiwaveSolve
 from pyaedt.misc.misc import list_installed_ansysem
+from pyaedt.modeler.geometry_operators import GeometryOperators
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
 else:
     import subprocess
 
 
@@ -141,18 +143,18 @@
         isaedtowned=False,
         oproject=None,
         student_version=False,
         use_ppe=False,
         technology_file=None,
     ):
         self._clean_variables()
-        if inside_desktop:
-            self.standalone = False
-        else:
-            self.standalone = True
+        # if inside_desktop:
+        #    self.standalone = False
+        # else:
+        self.standalone = True
         if edb_initialized:
             self.oproject = oproject
             self._main = sys.modules["__main__"]
             self._global_logger = pyaedt_logger
             self._logger = pyaedt_logger
             self.student_version = student_version
             self.logger.info("Logger is initialized in EDB.")
@@ -3333,14 +3335,18 @@
         """Compute a float representing the larger number between the dielectric thickness or trace width
         multiplied by the nW factor. The trace width search is limited to nets with ports attached.
 
         Parameters
         ----------
         expansion_factor : float
             Value for the width multiplier (nW factor).
+
+        Returns
+        -------
+        float
         """
         nets = []
         for port in self.excitations.values():
             nets.append(port.net_name)
         for port in self.sources.values():
             nets.append(port.net_name)
         nets = list(set(nets))
@@ -3352,7 +3358,151 @@
 
         for layer in list(self.stackup.dielectric_layers.values()):
             max_width = max(max_width, layer.thickness)
 
         max_width = max_width * expansion_factor
         self.logger.info("The W factor is {}, The initial extent = {:e}".format(expansion_factor, max_width))
         return max_width
+
+    @pyaedt_function_handler()
+    def copy_zones(self, working_directory=None):
+        """Copy multizone EDB project to one new edb per zone.
+
+        Parameters
+        ----------
+        working_directory : str
+            Directory path where all EDB project are copied, if empty will use the current EDB project.
+
+        Returns
+        -------
+           dict[str](EDB PolygonData)
+           Return a dictionary with edb path as key and EDB polygon Data defining the region.
+
+        """
+        if working_directory:
+            if not os.path.isdir(working_directory):
+                os.mkdir(working_directory)
+            else:
+                shutil.rmtree(working_directory)
+                os.mkdir(working_directory)
+        else:
+            working_directory = os.path.dirname(self.edbpath)
+        zone_primitives = list(self.active_layout.GetZonePrimitives())
+        edb_zones = {}
+        if not self.setups:
+            self.siwave.add_siwave_syz_analysis()
+            self.save_edb()
+        for zone in zone_primitives:
+            edb_zone_path = os.path.join(
+                working_directory, "{}_{}".format(zone.GetId(), os.path.basename(self.edbpath))
+            )
+            shutil.copytree(self.edbpath, edb_zone_path)
+            poly_data = zone.GetPolygonData()
+            edb_zones[edb_zone_path] = poly_data
+        return edb_zones
+
+    @pyaedt_function_handler()
+    def cutout_multizone_layout(self, zone_dict, common_reference_net):
+        """Create multizone project cutout.
+
+        Parameters
+        ----------
+        zone_dict : dict[str](EDB PolygonData)
+            Dictionary with EDB path as key and EDB PolygonData as value defining the zone region.
+            This dictionary is returned from the command copy_zones():
+            >>> edb = Edb(edb_file)
+            >>> zone_dict = edb.copy_zones(r"C:\Temp\test")
+
+        common_reference_net : str
+            the common reference net name. This net name must be provided to provide a valid project.
+
+        Returns
+        -------
+        dict[str][str] , list of str
+        first dictionary defined_ports with edb name as key and existing port name list as value. Those ports are the
+        ones defined before processing the multizone clipping.
+        second is the list of connected port.
+
+        """
+        terminals = {}
+        defined_ports = {}
+        for edb_path, zone_polygon in zone_dict.items():
+            edb = Edb(edbversion=self.edbversion, edbpath=edb_path)
+            edb.stackup.stackup_mode = "Laminate"
+            signal_nets = list(self.nets.signal.keys())
+            edb.cutout(use_pyaedt_cutout=True, custom_extent=zone_polygon, open_cutout_at_end=True)
+            edb.active_cell.SetName(os.path.splitext(os.path.basename(edb_path))[0])
+            defined_ports[os.path.splitext(os.path.basename(edb_path))[0]] = list(edb.excitations.keys())
+            edb_terminals_info = edb.hfss.create_vertical_circuit_port_on_clipped_traces(
+                nets=signal_nets, reference_net=common_reference_net, user_defined_extent=zone_polygon
+            )
+            if edb_terminals_info:
+                terminals[os.path.splitext(os.path.basename(edb_path))[0]] = edb_terminals_info
+            edb.save_edb()
+            edb.close_edb()
+        project_connexions = self._get_connected_ports_from_multizone_cutout(terminals)
+        return defined_ports, project_connexions
+
+    @pyaedt_function_handler()
+    def _get_connected_ports_from_multizone_cutout(self, terminal_info_dict):
+        """Return connected port list from clipped multizone layout.
+
+        Parameters
+            terminal_info_dict : dict[str][str]
+                dictionary terminals with edb name as key and created ports name on clipped signal nets.
+                Dictionary is generated by the command cutout_multizone_layout:
+                >>> edb = Edb(edb_file)
+                >>> edb_zones = edb.copy_zones(r"C:\Temp\test")
+                >>> defined_ports, terminals_info = edb.cutout_multizone_layout(edb_zones, common_reference_net)
+                >>> project_connexions = get_connected_ports(terminals_info)
+
+        Returns
+        -------
+        list[str]
+            list of connected ports.
+        """
+        if terminal_info_dict:
+            tolerance = 1e-8
+            connected_ports_list = []
+            project_list = list(terminal_info_dict.keys())
+            project_combinations = list(combinations(range(0, len(project_list)), 2))
+            for comb in project_combinations:
+                terminal_set1 = terminal_info_dict[project_list[comb[0]]]
+                terminal_set2 = terminal_info_dict[project_list[comb[1]]]
+                project1_nets = [t[0] for t in terminal_set1]
+                project2_nets = [t[0] for t in terminal_set2]
+                net_with_connected_ports = list(set(project1_nets).intersection(project2_nets))
+                if net_with_connected_ports:
+                    for net_name in net_with_connected_ports:
+                        project1_port_info = [term_info for term_info in terminal_set1 if term_info[0] == net_name]
+                        project2_port_info = [term_info for term_info in terminal_set2 if term_info[0] == net_name]
+                        port_list = [p[3] for p in project1_port_info] + [p[3] for p in project2_port_info]
+                        port_combinations = list(combinations(port_list, 2))
+                        for port_combination in port_combinations:
+                            if not port_combination[0] == port_combination[1]:
+                                port1 = [port for port in terminal_set1 if port[3] == port_combination[0]]
+                                if not port1:
+                                    port1 = [port for port in terminal_set2 if port[3] == port_combination[0]]
+                                port2 = [port for port in terminal_set2 if port[3] == port_combination[1]]
+                                if not port2:
+                                    port2 = [port for port in terminal_set1 if port[3] == port_combination[1]]
+                                port1 = port1[0]
+                                port2 = port2[0]
+                                if not port1[3] == port2[3]:
+                                    port_distance = GeometryOperators.points_distance(port1[1:3], port2[1:3])
+                                    if port_distance < tolerance:
+                                        port1_connexion = None
+                                        port2_connexion = None
+                                        for project_path, port_info in terminal_info_dict.items():
+                                            port1_map = [port for port in port_info if port[3] == port1[3]]
+                                            if port1_map:
+                                                port1_connexion = (project_path, port1[3])
+                                            port2_map = [port for port in port_info if port[3] == port2[3]]
+                                            if port2_map:
+                                                port2_connexion = (project_path, port2[3])
+                                        if port1_connexion and port2_connexion:
+                                            if (
+                                                not port1_connexion[0] == port2_connexion[0]
+                                                or not port1_connexion[1] == port2_connexion[1]
+                                            ):
+                                                connected_ports_list.append((port1_connexion, port2_connexion))
+            return connected_ports_list
```

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/components.py` & `pyaedt-0.6.76/pyaedt/edb_core/components.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/control_file.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/control_file.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/sources.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.76/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/general.py` & `pyaedt-0.6.76/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.76/pyaedt/edb_core/hfss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1021,14 +1021,92 @@
                                 term.SetReferenceLayer(reference_layer)
 
             if return_points_only:
                 return edges_pts
         return True
 
     @pyaedt_function_handler()
+    def create_vertical_circuit_port_on_clipped_traces(self, nets=None, reference_net=None, user_defined_extent=None):
+        """Create an edge port on clipped signal traces.
+
+        Parameters
+        ----------
+        nets : list, optional
+            String of one net or EDB net or a list of multiple nets or EDB nets.
+
+        reference_net : str, Edb net.
+             Name or EDB reference net.
+
+        user_defined_extent : [x, y], EDB PolygonData
+            Use this point list or PolygonData object to check if ports are at this polygon border.
+
+        Returns
+        -------
+        [[str]]
+            Nested list of str, with net name as first value, X value for point at border, Y value for point at border,
+            and terminal name.
+        """
+        if not isinstance(nets, list):
+            if isinstance(nets, str):
+                nets = list(self._pedb.nets.signal.values())
+        else:
+            nets = [self._pedb.nets.signal[net] for net in nets]
+        if nets:
+            if isinstance(reference_net, str):
+                reference_net = self._pedb.nets[reference_net]
+            if not reference_net:
+                self._logger.error("No reference net provided for creating port")
+                return False
+            if user_defined_extent:
+                if isinstance(user_defined_extent, self._edb.Geometry.PolygonData):
+                    _points = [pt for pt in list(user_defined_extent.Points)]
+                    _x = []
+                    _y = []
+                    for pt in _points:
+                        if pt.X.ToDouble() < 1e100 and pt.Y.ToDouble() < 1e100:
+                            _x.append(pt.X.ToDouble())
+                            _y.append(pt.Y.ToDouble())
+                    user_defined_extent = [_x, _y]
+            terminal_info = []
+            for net in nets:
+                net_polygons = [
+                    pp
+                    for pp in net.primitives
+                    if pp.GetPrimitiveType() == self._edb.Cell.Primitive.PrimitiveType.Polygon
+                ]
+                for poly in net_polygons:
+                    mid_points = [[arc.mid_point.X.ToDouble(), arc.mid_point.Y.ToDouble()] for arc in poly.arcs]
+                    for mid_point in mid_points:
+                        if GeometryOperators.point_in_polygon(mid_point, user_defined_extent) == 0:
+                            port_name = generate_unique_name("{}_{}".format(poly.GetNet().GetName(), poly.GetId()))
+                            term = self._create_edge_terminal(poly.GetId(), mid_point, port_name)  # pragma no cover
+                            if not term.IsNull():
+                                self._logger.info("Terminal {} created".format(term.GetName()))
+                                term.SetIsCircuitPort(True)
+                                terminal_info.append(
+                                    [poly.GetNet().GetName(), mid_point[0], mid_point[1], term.GetName()]
+                                )
+                                mid_pt_data = self._edb.Geometry.PointData(
+                                    self._edb.Utility.Value(mid_point[0]), self._edb.Utility.Value(mid_point[1])
+                                )
+                                ref_prim = [
+                                    prim
+                                    for prim in reference_net.primitives
+                                    if prim.polygon_data.PointInPolygon(mid_pt_data)
+                                ]
+                                if not ref_prim:
+                                    self._logger.warning("No reference primitive found in port vicinity")
+                                else:
+                                    reference_layer = ref_prim[0].layer
+                                    if term.SetReferenceLayer(reference_layer):  # pragma no cover
+                                        self._logger.info("Port {} created".format(port_name))
+            return terminal_info
+        return False
+
+    @pyaedt_function_handler()
     def get_layout_bounding_box(self, layout=None, digit_resolution=6):
         """Evaluate the layout bounding box.
 
         Parameters
         ----------
         layout :
             Edb layout.
```

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/layout.py` & `pyaedt-0.6.76/pyaedt/edb_core/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/materials.py` & `pyaedt-0.6.76/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/nets.py` & `pyaedt-0.6.76/pyaedt/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.76/pyaedt/edb_core/padstack.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.76/pyaedt/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.76/pyaedt/edb_core/stackup.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,14 +344,15 @@
         mode = self._pedb.edb.Cell.LayerCollectionMode
         if value == 0 or value == mode.Laminate or value == "Laminate":
             self._layer_collection.SetMode(mode.Laminate)
         elif value == 1 or value == mode.Overlapping or value == "Overlapping":
             self._layer_collection.SetMode(mode.Overlapping)
         elif value == 2 or value == mode.MultiZone or value == "MultiZone":
             self._layer_collection.SetMode(mode.MultiZone)
+        self._pedb._active_layout.SetLayerCollection(self._layer_collection)
 
     @property
     def _edb_layer_list(self):
         return list(self._layer_collection.Layers(self._pedb.edb.Cell.LayerTypeSet.AllLayerSet))
 
     @property
     def _edb_layer_list_nonstackup(self):
```

### Comparing `pyaedt-0.6.75/pyaedt/emit.py` & `pyaedt-0.6.76/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.76/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/emit_core/EmitConstants.py` & `pyaedt-0.6.76/pyaedt/emit_core/EmitConstants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.76/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.76/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.76/pyaedt/emit_core/results/revision.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.76/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.76/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/clr_module.py` & `pyaedt-0.6.76/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/configurations.py` & `pyaedt-0.6.76/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/constants.py` & `pyaedt-0.6.76/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/design_types.py` & `pyaedt-0.6.76/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/filesystem.py` & `pyaedt-0.6.76/pyaedt/generic/filesystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         if os.path.exists(dst_file):
             try:
                 os.unlink(dst_file)
             except OSError:  # pragma: no cover
                 pass
         try:
             shutil.copy2(src_file, dst_file)
-        except shutil.SameFileError:  # pragma: no cover
+        except:  # pragma: no cover
             pass
 
         return dst_file
 
     def copyfolder(self, src_folder, destfolder):
         """
```

### Comparing `pyaedt-0.6.75/pyaedt/generic/general_methods.py` & `pyaedt-0.6.76/pyaedt/generic/general_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1766,14 +1766,45 @@
             "ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE": "1",
             "ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE": "1",
             "ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE": "1",
         }
         if is_linux:
             self._aedt_environment_variables["ANS_NODEPCHECK"] = "1"
         self._desktop_launch_timeout = 90
+        self._aedt_process_id = None
+        self._is_student = False
+
+    @property
+    def aedt_process_id(self):
+        """ID of the desktop process. The default is ``None``.
+
+        Returns
+        -------
+        int
+        """
+        return self._aedt_process_id
+
+    @aedt_process_id.setter
+    def aedt_process_id(self, value):
+        self._aedt_process_id = int(value)
+
+    @property
+    def is_student(self):
+        """Whether the desktop process is set to the student version. The
+        default is ``False``.
+
+        Returns
+        -------
+        bool
+        """
+        return self._is_student
+
+    @is_student.setter
+    def is_student(self, value):
+        self._is_student = value
 
     @property
     def desktop_launch_timeout(self):
         """Set the desktop launcher max timeout. Default is ``90`` seconds.
 
         Returns
         -------
```

### Comparing `pyaedt-0.6.75/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.76/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.76/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/pdf.py` & `pyaedt-0.6.76/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/plot.py` & `pyaedt-0.6.76/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/process.py` & `pyaedt-0.6.76/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.76/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.76/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/toolkit.py` & `pyaedt-0.6.76/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.76/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/hfss.py` & `pyaedt-0.6.76/pyaedt/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.76/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/icepak.py` & `pyaedt-0.6.76/pyaedt/icepak.py`

 * *Files 3% similar despite different names*

```diff
@@ -447,14 +447,17 @@
 
     @pyaedt_function_handler()
     def create_source_block(
         self, object_name, input_power, assign_material=True, material_name="Ceramic_material", use_object_for_name=True
     ):
         """Create a source block for an object.
 
+        .. deprecated:: 0.6.75
+            This method is deprecated. Use the ``assign_solid_block()`` method instead.
+
         Parameters
         ----------
         object_name : str, list
             Name of the object.
         input_power : str or var
             Input power.
         assign_material : bool, optional
@@ -3645,15 +3648,16 @@
         if function == "Piecewise Linear":
             if not isinstance(variation_value, list):
                 variation_value = ["1", "pwl({},Temp)".format(variation_value)]
             else:
                 variation_value = [variation_value[0], "pwl({},Temp)".format(variation_value[1])]
             out_dict["Variation Value"] = "[{}]".format(", ".join(['"' + str(i) + '"' for i in variation_value]))
         else:
-            out_dict["Variation Value"] = "[{}]".format(", ".join([str(i) for i in variation_value]))
+            if variation_value is not None:
+                out_dict["Variation Value"] = "[{}]".format(", ".join([str(i) for i in variation_value]))
         return {"{} Variation Data".format(quantity): out_dict}
 
     @pyaedt_function_handler()
     def assign_source(
         self,
         assignment,
         thermal_condition,
@@ -3768,7 +3772,244 @@
             else:
                 props[quantity] = value
 
         bound = BoundaryObject(self, boundary_name, props, "SourceIcepak")
         if bound.create():
             self.boundaries.append(bound)
             return bound
+
+    @pyaedt_function_handler
+    def assign_solid_block(
+        self, object_name, power_assignment, boundary_name=None, htc=None, ext_temperature="AmbientTemp"
+    ):
+        """
+        Assign block boundary for solid objects.
+
+        Parameters
+        ----------
+        object_name : str
+            Name of the object.
+        power_assignment : str or dict
+            String with value and units of the power assignment or with ``"Joule Heating"``.
+            Also, a dictionary can be used for temperature dependent or transient assignment.
+            The dictionary should contain three keys: ``"Type"``, ``"Function"`` and
+            ``"Values"``. Accepted ``"Type"`` values are: ``"Temp Dep"`` and ``"Transient"``.
+            Accepted ``"Function"`` are: ``"Linear"``, ``"Power Law"``, ``"Exponential"``,
+            ``"Sinusoidal"``, ``"Square Wave"`` and ``"Piecewise Linear"``. ``"Temp Dep"`` only
+            support the latter. ``"Values"`` contains a list of strings containing the parameters
+            required by the ``"Function"`` selection (e.g. ``"Linear"`` requires two parameters:
+            the value of the variable at t=0 and the slope of the line). The parameters required by
+            each ``Function`` option is in Icepak documentation. The parameters must contain the
+            units where needed.
+        boundary_name : str, optional
+            Name of the source boundary. The default is ``None`` and the boundary name will be
+            generated automatically.
+        htc : float, str or dict, optional
+            String with value and units of heat transfer coefficient for the external conditions.
+            Also, a dictionary can be used for temperature dependent or transient assignment as
+            described in ``power_assignment``. The default is ``None``
+        ext_temperature : float, str or dict, optional
+            String with value and units of temperature for the external conditions.
+            Also, a dictionary can be used for transient assignment as described in ``power_assignment``.
+            The default is ``"AmbientTemp"`` and will have effect if ``htc`` is not ``None``
+
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Boundary object when successful or ``None`` when failed.
+
+        References
+        ----------
+
+        >>> oModule.AssignBlockBoundary
+
+        Examples
+        --------
+        >>> from pyaedt import Icepak
+        >>> ipk = Icepak()
+        >>> ipk.solution_type = "Transient"
+        >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox3", "copper")
+        >>> power_dict = {"Type": "Transient", "Function": "Sinusoidal", "Values": ["0W", 1, 1, "1s"]}
+        >>> block = ipk.assign_solid_block("BlockBox3", power_dict)
+        """
+        if not self.modeler.get_object_from_name(object_name).solve_inside:
+            self.logger.add_error_message(
+                "Please use ``assign_hollow_block`` function with this object as" "``solve_inside`` is ``False``."
+            )
+            return None
+        if ext_temperature != "AmbientTemp" and ext_temperature is not None and not htc:
+            self.logger.add_error_message("Please set an argument for ``htc`` or remove ``ext_temperature`` argument.")
+            return None
+        if isinstance(ext_temperature, dict) and ext_temperature["Type"] == "Temp Dep":
+            self.logger.add_error_message(
+                'It is not possible to use a "Temp Dep" assignment for ' "temperature assignment."
+            )
+            return None
+        props = {"Block Type": "Solid", "Objects": [object_name]}
+        if isinstance(power_assignment, dict):
+            assignment_value = self._parse_variation_data(
+                "Total Power",
+                power_assignment["Type"],
+                variation_value=power_assignment["Values"],
+                function=power_assignment["Function"],
+            )
+            props.update(assignment_value)
+        elif power_assignment == "Joule Heating":
+            assignment_value = self._parse_variation_data(
+                "Total Power", "Joule Heating", variation_value=None, function="None"
+            )
+            props.update(assignment_value)
+        elif isinstance(power_assignment, (float, int)):
+            props["Total Power"] = str(power_assignment) + "W"
+        else:
+            props["Total Power"] = power_assignment
+
+        if htc:
+            props["Use External Conditions"] = True
+            for quantity, assignment in [("Temperature", ext_temperature), ("Heat Transfer Coefficient", htc)]:
+                if isinstance(assignment, dict):
+                    assignment_value = self._parse_variation_data(
+                        quantity,
+                        assignment["Type"],
+                        variation_value=assignment["Values"],
+                        function=assignment["Function"],
+                    )
+                    props.update(assignment_value)
+                else:
+                    if isinstance(assignment, (float, int)):
+                        assignment = str(assignment) + ["w_per_m2kel", "cel"][int(quantity == "Temperature")]
+                    props[quantity] = assignment
+        else:
+            props["Use External Conditions"] = False
+
+        if not boundary_name:
+            boundary_name = generate_unique_name(object_name + "_Block")
+
+        bound = BoundaryObject(self, boundary_name, props, "Block")
+        if bound.create():
+            self.boundaries.append(bound)
+            return bound
+
+    @pyaedt_function_handler
+    def assign_hollow_block(
+        self, object_name, assignment_type, assignment_value, boundary_name=None, external_temperature="AmbientTemp"
+    ):
+        """
+        Assign block boundary for hollow objects.
+
+        Parameters
+        ----------
+        object_name : str
+            Name of the object.
+        assignment_type : str
+            Type of the boundary assignment. The accepted types are: "Total Power", "Heat Flux",
+            "Temperature" or "Heat Transfer Coefficient".
+        assignment_value : str or dict
+            String with value and units of the assignment. If ``"Total Power"`` is assignment_type,
+            ``"Joule Heating"`` can be used.
+            Also, a dictionary can be used for temperature dependent or transient assignment.
+            The dictionary should contain three keys: ``"Type"``, ``"Function"`` and
+            ``"Values"``. Accepted ``"Type"`` values are: ``"Temp Dep"`` and ``"Transient"``.
+            Accepted ``"Function"`` are: ``"Linear"``, ``"Power Law"``, ``"Exponential"``,
+            ``"Sinusoidal"``, ``"Square Wave"`` and ``"Piecewise Linear"``. ``"Temp Dep"`` only
+            support the latter. ``"Values"`` contains a list of strings containing the parameters
+            required by the ``"Function"`` selection (e.g. ``"Linear"`` requires two parameters:
+            the value of the variable at t=0 and the slope of the line). The parameters required by
+            each ``Function`` option is in Icepak documentation. The parameters must contain the
+            units where needed.
+        boundary_name : str, optional
+            Name of the source boundary. The default is ``None`` and the boundary name will be
+            generated automatically.
+        external_temperature : str, dict or float, optional
+            String with value and unit of temperature for the Heat Transfer Coefficient. If float,
+            ``"cel"`` unit will be added automatically. The default is ``"AmbientTemp"``.
+
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Boundary object when successful or ``None`` when failed.
+
+        References
+        ----------
+
+        >>> oModule.AssignBlockBoundary
+
+        Examples
+        --------
+        >>> from pyaedt import Icepak
+        >>> ipk = Icepak()
+        >>> ipk.solution_type = "Transient"
+        >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox5", "copper")
+        >>> box.solve_inside = False
+        >>> temp_dict = {"Type": "Transient", "Function": "Square Wave", "Values": ["1cel", "0s", "1s", "0.5s", "0cel"]}
+        >>> block = ipk.assign_hollow_block("BlockBox5", "Heat Transfer Coefficient", "1w_per_m2kel", "Test", temp_dict)
+        """
+        if self.modeler.get_object_from_name(object_name).solve_inside:
+            self.logger.add_error_message(
+                "Please use ``assign_solid_block`` function with this object as" "``solve_inside`` is ``True``."
+            )
+            return None
+        if assignment_value == "Joule Heating" and assignment_type != "Total Power":
+            self.logger.add_error_message(
+                '``"Joule Heating"`` assignment is supported only if ``assignment_type``' 'is ``"Total Power"``.'
+            )
+            return None
+
+        assignment_dict = {
+            "Total Power": ["Fixed Heat", "Total Power"],
+            "Heat Flux": ["Fixed Heat", "Heat Flux"],
+            "Temperature": ["Fixed Temperature", "Fixed Temperature"],
+            "Heat Transfer Coefficient": ["Internal Conditions", "Heat Transfer Coefficient"],
+        }
+        thermal_condition = assignment_dict.get(assignment_type, None)
+        if thermal_condition is None:
+            self.logger.add_error_message(
+                'Available assignment_type are "Total Power", "Heat Flux",'
+                '"Temperature" and "Heat Transfer Coefficient".'
+                "{} not recognized.".format(assignment_type)
+            )
+            return None
+
+        props = {"Block Type": "Hollow", "Objects": [object_name], "Thermal Condition": thermal_condition[0]}
+        if thermal_condition[0] == "Fixed Heat":
+            props["Use Total Power"] = thermal_condition[1] == "Total Power"
+        if isinstance(assignment_value, dict):
+            assignment_value_dict = self._parse_variation_data(
+                thermal_condition[1],
+                assignment_value["Type"],
+                variation_value=assignment_value["Values"],
+                function=assignment_value["Function"],
+            )
+            props.update(assignment_value_dict)
+        elif assignment_value == "Joule Heating":
+            assignment_value_dict = self._parse_variation_data(
+                thermal_condition[1], "Joule Heating", variation_value=None, function="None"
+            )
+            props.update(assignment_value_dict)
+        else:
+            props[thermal_condition[1]] = assignment_value
+        if thermal_condition[0] == "Internal Conditions":
+            if isinstance(external_temperature, dict):
+                if external_temperature["Type"] == "Temp Dep":
+                    self.logger.add_error_message(
+                        'It is not possible to use a "Temp Dep" assignment for a' "temperature assignment."
+                    )
+                    return None
+                assignment_value_dict = self._parse_variation_data(
+                    "Temperature",
+                    external_temperature["Type"],
+                    variation_value=external_temperature["Values"],
+                    function=external_temperature["Function"],
+                )
+                props.update(assignment_value_dict)
+            else:
+                props["Temperature"] = external_temperature
+
+        if not boundary_name:
+            boundary_name = generate_unique_name(object_name + "_Block")
+
+        bound = BoundaryObject(self, boundary_name, props, "Block")
+        if bound.create():
+            self.boundaries.append(bound)
+            return bound
```

### Comparing `pyaedt-0.6.75/pyaedt/maxwell.py` & `pyaedt-0.6.76/pyaedt/maxwell.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.76/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/mechanical.py` & `pyaedt-0.6.76/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/Console.py_build` & `pyaedt-0.6.76/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.76/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.76/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.76/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.76/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.76/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/amat.xml` & `pyaedt-0.6.76/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/console_setup.py` & `pyaedt-0.6.76/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.76/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.76/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.76/pyaedt/misc/install_extra_toolkits.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 from xml.etree.ElementTree import ParseError
 
 from pyaedt.misc.aedtlib_personalib_install import current_dir
 from pyaedt.misc.aedtlib_personalib_install import write_pretty_xml
 
 available_toolkits = {
     "AntennaWizard": {
-        "pip": "git+https://github.com/pyansys/pyaedt-antenna-toolkit.git",
+        "pip": "git+https://github.com/ansys/pyaedt-antenna-toolkit.git",
         "image": "pyansys.png",
         "toolkit_script": "ansys/aedt/toolkits/antennas/antenna_toolkit.py",
         "installation_path": "HFSS",
         "package_name": "ansys.aedt.toolkits.antennas",
     },
     "ChokeWizard": {
-        "pip": "git+https://github.com/pyansys/pyaedt-choke-toolkit.git",
+        "pip": "git+https://github.com/ansys/pyaedt-choke-toolkit.git",
         "image": "pyansys.png",
         "toolkit_script": "ansys/aedt/toolkits/choke/choke_toolkit.py",
         "installation_path": "Project",
         "package_name": "ansys.aedt.toolkits.choke",
     },
     "TemplateToolkit": {
-        "pip": "git+https://github.com/pyansys/pyaedt-toolkit-template.git",
+        "pip": "git+https://github.com/ansys/pyaedt-toolkit-template.git",
         "image": "pyansys.png",
-        "toolkit_script": "ansys/aedt/toolkits/template/template_toolkit.py",
+        "toolkit_script": "ansys/aedt/toolkits/template/run_toolkit.py",
         "installation_path": "Project",
         "package_name": "ansys.aedt.toolkits.template",
     },
 }
 
 
 def write_toolkit_config(product_toolkit_dir, pyaedt_lib_dir, toolkitname, toolkit, force_write=False):
```

### Comparing `pyaedt-0.6.75/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.76/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/misc.py` & `pyaedt-0.6.76/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.76/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.76/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.76/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.76/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.76/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.76/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/misc/template.acf` & `pyaedt-0.6.76/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.76/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.76/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.76/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.76/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.76/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.76/pyaedt/modeler/cad/Modeler.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.76/pyaedt/modeler/cad/Primitives.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.76/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.76/pyaedt/modeler/cad/Primitives3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.76/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.76/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.76/pyaedt/modeler/cad/object3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.76/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/calculators.py` & `pyaedt-0.6.76/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.76/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         ret1 = self._circuit_comp._circuit_components.create_page_port(page_name, self.location, angle=angle)
         for cmp in component_pin:
             try:
                 x_loc = AEDT_UNITS["Length"][decompose_variable_value(cmp._circuit_comp.location[0])[1]] * float(
                     decompose_variable_value(cmp._circuit_comp.location[0])[0]
                 )
             except:
-                x_loc = float(self._circuit_comp.location[0])
+                x_loc = float(cmp._circuit_comp.location[0])
             comp_pin_angle = cmp._circuit_comp.angle * math.pi / 180
             if len(cmp._circuit_comp.pins) == 2:
                 comp_pin_angle += math.pi / 2
             if cmp.location[0] < x_loc:
                 angle = comp_pin_angle
             else:
                 angle = math.pi + comp_pin_angle
```

### Comparing `pyaedt-0.6.75/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.76/pyaedt/modeler/geometry_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1547,35 +1547,37 @@
         if right_handed:
             return math.atan2(c, GeometryOperators.v_dot(va, vb))
         else:
             return math.atan2(-c, GeometryOperators.v_dot(va, vb))
 
     @staticmethod
     @pyaedt_function_handler()
-    def point_in_polygon(point, polygon):
-        """Determine if a point is inside or outside a polygon, both located on the same plane.
+    def point_in_polygon(point, polygon, tolerance=1e-8):
+        """Determine if a point is inside, outside the polygon or at exactly at the border.
 
         The method implements the radial algorithm (https://es.wikipedia.org/wiki/Algoritmo_radial)
 
         point : List
             List of ``[x, y]`` coordinates.
         polygon : List
             [[x1, x2, ..., xn],[y1, y2, ..., yn]]
+        tolerance : float
+            tolerance used for the algorithm. Default value is 1e-8.
 
         Returns
         -------
         int
             - ``-1`` When the point is outside the polygon.
             - ``0`` When the point is exactly on one of the sides of the polygon.
             - ``1`` When the point is inside the polygon.
         """
         # fmt: off
-        tol = 1e-8
+        tol = tolerance
         if len(point) != 2:  # pragma: no cover
-            raise ValueError("point must be a list in the form [x, y]")
+            raise ValueError("Point must be a list in the form [x, y].")
         pl = len(polygon[0])
         if len(polygon[1]) != pl:  # pragma: no cover
             raise ValueError("Polygon x and y lists must be the same length")
         asum = 0
         for i in range(pl):
             vj = [polygon[0][i-1], polygon[1][i-1]]
             vi = [polygon[0][i], polygon[1][i]]
```

### Comparing `pyaedt-0.6.75/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.76/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.76/pyaedt/modeler/modeler3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.76/pyaedt/modeler/modelerpcb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.76/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.76/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modeler/schematic.py` & `pyaedt-0.6.76/pyaedt/modeler/schematic.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.76/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/Boundary.py` & `pyaedt-0.6.76/pyaedt/modules/Boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,19 +313,37 @@
     """
 
     def __init__(self, app, name, props, boundarytype):
         self.auto_update = False
         self._app = app
         self._name = name
         self.props = BoundaryProps(self, OrderedDict(props))
-        self.type = boundarytype
+        self._type = boundarytype
         self._boundary_name = self.name
         self.auto_update = True
 
     @property
+    def type(self):
+        """Boundary type.
+
+        Returns
+        -------
+        str
+            Returns Type of the boundary
+        """
+        if self._app.design_type == "Icepak" and self._type == "Source":
+            return "SourceIcepak"
+        else:
+            return self._type
+
+    @type.setter
+    def type(self, value):
+        self._type = value
+
+    @property
     def name(self):
         """Boundary Name."""
         return self._name
 
     @name.setter
     def name(self, value):
         self._name = value
@@ -595,15 +613,15 @@
         elif self.type == "Opening":
             self._app.oboundary.EditOpeningBoundary(self._boundary_name, self._get_args())
         elif self.type == "EMLoss":
             self._app.oboundary.EditEMLoss(self._boundary_name, self._get_args())  # pragma: no cover
         elif self.type == "Block":
             self._app.oboundary.EditBlockBoundary(self._boundary_name, self._get_args())
         elif self.type == "SourceIcepak":
-            self._app.oboundary.EditSourceBoundary(self._get_args())
+            self._app.oboundary.EditSourceBoundary(self._boundary_name, self._get_args())
         elif self.type == "HeatFlux":
             self._app.oboundary.EditHeatFlux(self._boundary_name, self._get_args())
         elif self.type == "HeatGeneration":
             self._app.oboundary.EditHeatGeneration(self._boundary_name, self._get_args())
         elif self.type == "Voltage":
             self._app.oboundary.EditVoltage(self._boundary_name, self._get_args())
         elif self.type == "VoltageDrop":
```

### Comparing `pyaedt-0.6.75/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.76/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.76/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.76/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.76/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/Material.py` & `pyaedt-0.6.76/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.76/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/Mesh.py` & `pyaedt-0.6.76/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.76/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.76/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.76/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.76/pyaedt/modules/PostProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3433,15 +3433,15 @@
                 else:
                     power_value, exp = extract_dataset_info(bc_obj, units_input=units, boundary="Power")
                     mult = multiplier_from_dataset(exp, temperature)
 
                 power_dict[bc_obj.name] = power_value * n * mult
                 self.logger.info("The power of {} is {} {}".format(bc_obj.name, str(power_dict[bc_obj.name]), units))
 
-            elif bc_obj.type == "Source":
+            elif bc_obj.type == "SourceIcepak":
                 if bc_obj.props["Thermal Condition"] == "Total Power":
                     n = 0
                     if "Faces" in bc_obj.props:
                         n += len(bc_obj.props["Faces"])
                     if "Objects" in bc_obj.props:
                         n += len(bc_obj.props["Objects"])
```

### Comparing `pyaedt-0.6.75/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.76/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.76/pyaedt/modules/SolveSetup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 This module provides all functionalities for creating and editing setups in AEDT.
 It is based on templates to allow for easy creation and modification of setup properties.
 
 """
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
-import copy
 import logging
 import os.path
 from random import randrange
 import time
 import warnings
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import pyaedt_function_handler
-from pyaedt.modules.SetupTemplates import MaxwellTransient
 from pyaedt.modules.SetupTemplates import SetupKeys
 from pyaedt.modules.SolveSweeps import SetupProps
 from pyaedt.modules.SolveSweeps import SweepHFSS
 from pyaedt.modules.SolveSweeps import SweepHFSS3DLayout
 from pyaedt.modules.SolveSweeps import SweepMatrix
 from pyaedt.modules.SolveSweeps import identify_setup
 
@@ -2629,36 +2627,22 @@
             self._app.logger.error("Control Program file does not exist.")
             return False
 
         if not isinstance(control_program_args, str):
             self._app.logger.error("Control Program arguments have to be a string.")
             return False
 
-        self.props = copy.deepcopy(MaxwellTransient)
+        self.auto_update = False
         self.props["UseControlProgram"] = True
         self.props["ControlProgramName"] = control_program_path
         self.props["ControlProgramArg"] = control_program_args
         self.props["CallCtrlProgAfterLastStep"] = call_after_last_step
+        self.auto_update = True
+        self.update()
 
-        self.p_app.oanalysis.EditSetup(
-            self.name,
-            [
-                "NAME:" + self.name,
-                "Enabled:=",
-                True,
-                "UseControlProgram:=",
-                True,
-                "ControlProgramName:=",
-                control_program_path,
-                "ControlProgramArg:=",
-                control_program_args,
-                "CallCtrlProgAfterLastStep:=",
-                call_after_last_step,
-            ],
-        )
         return True
 
 
 class SetupQ3D(Setup, object):
     """Initializes, creates, and updates an Q3D setup.
 
     Parameters
```

### Comparing `pyaedt-0.6.75/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.76/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.76/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/report_templates.py` & `pyaedt-0.6.76/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/modules/solutions.py` & `pyaedt-0.6.76/pyaedt/modules/solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/q3d.py` & `pyaedt-0.6.76/pyaedt/q3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/rmxprt.py` & `pyaedt-0.6.76/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.76/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.76/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.76/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.76/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.76/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/siwave.py` & `pyaedt-0.6.76/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyaedt/twinbuilder.py` & `pyaedt-0.6.76/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.75/pyproject.toml` & `pyaedt-0.6.76/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -44,41 +44,41 @@
     "numpy==1.24.3; python_version > '3.7'",
     "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "pytest==7.3.1",
     "pytest-cov==4.0.0",
-    "pytest-xdist==3.2.1",
-    "pyvista==0.38.6",
+    "pytest-xdist==3.3.0",
+    "pyvista==0.39.1",
     "scikit-learn==1.2.2",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
     "ansys-sphinx-theme==0.9.9",
     "imageio==2.28.0",
     "imageio-ffmpeg==0.4.8",
     "ipython==8.13.0",
     "ipywidgets==8.0.6",
     "joblib==1.2.0",
-    "jupyterlab==3.6.3",
+    "jupyterlab==4.0.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "nbsphinx==0.9.1",
     "numpydoc==1.5.0",
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
-    "pyvista==0.38.6",
+    "pyvista==0.39.1",
     "recommonmark==0.7.1",
     "scikit-learn==1.2.2",
-    "Sphinx==7.0.0",
+    "Sphinx==7.0.1",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.23.0",
     "sphinx-copybutton==0.5.2",
     "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
     "SRTM.py",
@@ -91,30 +91,30 @@
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.38.6",
+    "pyvista==0.39.1",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 all = [
     "imageio==2.28.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.38.6",
+    "pyvista==0.39.1",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 
 [tool.flit.module]
```

### Comparing `pyaedt-0.6.75/PKG-INFO` & `pyaedt-0.6.76/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.75
+Version: 0.6.76
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -25,37 +25,37 @@
 Requires-Dist: matplotlib==3.5.3 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
-Requires-Dist: pyvista==0.38.6 ; extra == "all"
+Requires-Dist: pyvista==0.39.1 ; extra == "all"
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: imageio==2.28.0 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
 Requires-Dist: ipython==8.13.0 ; extra == "doc"
 Requires-Dist: ipywidgets==8.0.6 ; extra == "doc"
 Requires-Dist: joblib==1.2.0 ; extra == "doc"
-Requires-Dist: jupyterlab==3.6.3 ; extra == "doc"
+Requires-Dist: jupyterlab==4.0.0 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: nbsphinx==0.9.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
-Requires-Dist: pyvista==0.38.6 ; extra == "doc"
+Requires-Dist: pyvista==0.39.1 ; extra == "doc"
 Requires-Dist: recommonmark==0.7.1 ; extra == "doc"
 Requires-Dist: scikit-learn==1.2.2 ; extra == "doc"
-Requires-Dist: Sphinx==7.0.0 ; extra == "doc"
+Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
@@ -66,15 +66,15 @@
 Requires-Dist: matplotlib==3.5.3 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
-Requires-Dist: pyvista==0.38.6 ; extra == "full"
+Requires-Dist: pyvista==0.39.1 ; extra == "full"
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.1.2 ; extra == "full"
 Requires-Dist: ipython==8.13.0 ; extra == "tests"
 Requires-Dist: imageio==2.28.0 ; extra == "tests"
 Requires-Dist: joblib==1.2.0 ; extra == "tests"
@@ -84,16 +84,16 @@
 Requires-Dist: numpy==1.24.3 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
-Requires-Dist: pytest-xdist==3.2.1 ; extra == "tests"
-Requires-Dist: pyvista==0.38.6 ; extra == "tests"
+Requires-Dist: pytest-xdist==3.3.0 ; extra == "tests"
+Requires-Dist: pyvista==0.39.1 ; extra == "tests"
 Requires-Dist: scikit-learn==1.2.2 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: scikit-rf ; extra == "tests"
 Project-URL: Bug Tracker, https://github.com/pyansys/pyaedt/issues
 Project-URL: Documentation, https://aedt.docs.pyansys.com
 Project-URL: Source Code, https://github.com/pyansys/pyaedt
```

