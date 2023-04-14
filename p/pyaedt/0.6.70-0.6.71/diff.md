# Comparing `tmp/pyaedt-0.6.70.tar.gz` & `tmp/pyaedt-0.6.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.70.tar", last modified: Fri Apr  7 18:42:41 2023, max compression
+gzip compressed data, was "pyaedt-0.6.71.tar", last modified: Fri Apr 14 08:21:39 2023, max compression
```

## Comparing `pyaedt-0.6.70.tar` & `pyaedt-0.6.71.tar`

### file list

```diff
@@ -1,248 +1,249 @@
--rw-r--r--   0        0        0     1111 2023-03-24 16:10:16.742763 pyaedt-0.6.70/LICENSE
--rw-r--r--   0        0        0     9857 2023-04-07 10:17:20.915272 pyaedt-0.6.70/README.rst
--rw-r--r--   0        0        0     2503 2023-04-07 18:23:53.677004 pyaedt-0.6.70/pyaedt/__init__.py
--rw-r--r--   0        0        0    26253 2023-03-24 16:10:18.742581 pyaedt-0.6.70/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-03-24 16:10:18.742581 pyaedt-0.6.70/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88655 2023-04-07 18:23:53.677004 pyaedt-0.6.70/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    41260 2023-04-06 11:56:42.332868 pyaedt-0.6.70/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17009 2023-04-06 11:56:42.332868 pyaedt-0.6.70/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-03-24 16:10:18.742581 pyaedt-0.6.70/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19795 2023-04-06 11:56:42.332868 pyaedt-0.6.70/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4374 2023-03-24 16:10:18.742581 pyaedt-0.6.70/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4539 2023-03-24 16:10:18.742581 pyaedt-0.6.70/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   126722 2023-03-30 14:12:42.537578 pyaedt-0.6.70/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-03-24 16:10:18.742581 pyaedt-0.6.70/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    72583 2023-04-03 12:18:59.459114 pyaedt-0.6.70/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.742581 pyaedt-0.6.70/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12433 2023-03-24 16:10:18.742581 pyaedt-0.6.70/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    37014 2023-03-24 16:10:18.742581 pyaedt-0.6.70/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    57605 2023-03-24 16:10:18.758234 pyaedt-0.6.70/pyaedt/circuit.py
--rw-r--r--   0        0        0    10034 2023-03-24 16:10:18.758234 pyaedt-0.6.70/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    56983 2023-04-07 12:39:52.648098 pyaedt-0.6.70/pyaedt/desktop.py
--rw-r--r--   0        0        0    23552 2023-03-24 16:10:18.758234 pyaedt-0.6.70/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1092 2023-03-24 16:10:18.758234 pyaedt-0.6.70/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0    23996 2023-03-24 16:10:18.758234 pyaedt-0.6.70/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   249856 2023-03-24 16:10:18.758234 pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.dll
--rw-r--r--   0        0        0   481931 2023-03-24 16:10:18.773842 pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.xml
--rw-r--r--   0        0        0   131072 2023-03-24 16:10:18.773842 pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.dll
--rw-r--r--   0        0        0    85860 2023-03-24 16:10:18.773842 pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.xml
--rw-r--r--   0        0        0    86016 2023-03-24 16:10:18.773842 pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.RtfRendering-gdi.dll
--rw-r--r--   0        0        0    51586 2023-03-24 16:10:18.773842 pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.RtfRendering-gdi.xml
--rw-r--r--   0        0        0   700336 2023-03-24 16:10:18.773842 pyaedt-0.6.70/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   707721 2023-03-24 16:10:18.789780 pyaedt-0.6.70/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0   585728 2023-03-24 16:10:18.789780 pyaedt-0.6.70/pyaedt/dlls/PDFReport/PdfSharp-gdi.dll
--rw-r--r--   0        0        0  1164073 2023-03-24 16:10:18.789780 pyaedt-0.6.70/pyaedt/dlls/PDFReport/PdfSharp-gdi.xml
--rw-r--r--   0        0        0    94208 2023-03-24 16:10:18.805116 pyaedt-0.6.70/pyaedt/dlls/PDFReport/PdfSharp.Charting-gdi.dll
--rw-r--r--   0        0        0   129427 2023-03-24 16:10:18.805116 pyaedt-0.6.70/pyaedt/dlls/PDFReport/PdfSharp.Charting-gdi.xml
--rw-r--r--   0        0        0     9728 2023-03-24 16:10:18.805116 pyaedt-0.6.70/pyaedt/dlls/PDFReport/de/MigraDoc.DocumentObjectModel-gdi.resources.dll
--rw-r--r--   0        0        0     7168 2023-03-24 16:10:18.805116 pyaedt-0.6.70/pyaedt/dlls/PDFReport/de/MigraDoc.Rendering-gdi.resources.dll
--rw-r--r--   0        0        0     7168 2023-03-24 16:10:18.805116 pyaedt-0.6.70/pyaedt/dlls/PDFReport/de/MigraDoc.RtfRendering-gdi.resources.dll
--rw-r--r--   0        0        0     5120 2023-03-24 16:10:18.805116 pyaedt-0.6.70/pyaedt/dlls/PDFReport/de/PdfSharp-gdi.resources.dll
--rw-r--r--   0        0        0     4608 2023-03-24 16:10:18.805116 pyaedt-0.6.70/pyaedt/dlls/PDFReport/de/PdfSharp.Charting-gdi.resources.dll
--rw-r--r--   0        0        0    23488 2023-03-24 16:43:00.390747 pyaedt-0.6.70/pyaedt/downloads.py
--rw-r--r--   0        0        0   130774 2023-04-07 14:18:16.247983 pyaedt-0.6.70/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-04-06 16:51:57.478550 pyaedt-0.6.70/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    88171 2023-04-06 17:43:43.595268 pyaedt-0.6.70/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.820698 pyaedt-0.6.70/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    32856 2023-04-06 17:43:43.595268 pyaedt-0.6.70/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0      937 2023-03-24 16:10:18.820698 pyaedt-0.6.70/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      324 2023-03-24 16:10:18.820698 pyaedt-0.6.70/pyaedt/edb_core/edb_data/edb_builder.py
--rw-r--r--   0        0        0     1166 2023-03-24 16:10:18.820698 pyaedt-0.6.70/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    65819 2023-03-24 16:10:18.820698 pyaedt-0.6.70/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20305 2023-04-06 16:51:57.478550 pyaedt-0.6.70/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     4724 2023-04-03 14:45:49.216597 pyaedt-0.6.70/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    58397 2023-04-03 14:45:49.216597 pyaedt-0.6.70/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32298 2023-04-06 16:51:57.478550 pyaedt-0.6.70/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0    96893 2023-03-30 14:49:31.546231 pyaedt-0.6.70/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36296 2023-03-24 16:43:00.390747 pyaedt-0.6.70/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    31276 2023-04-06 16:51:57.478550 pyaedt-0.6.70/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     4147 2023-03-24 16:10:18.820698 pyaedt-0.6.70/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2425 2023-03-27 19:28:28.383108 pyaedt-0.6.70/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     2657 2023-03-24 16:10:18.820698 pyaedt-0.6.70/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    60090 2023-04-03 14:45:49.216597 pyaedt-0.6.70/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2844 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-03-24 16:10:18.836323 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7706 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4646 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11163 2023-04-03 14:45:49.232236 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-03-24 16:10:18.851970 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21750 2023-04-03 14:45:49.232236 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-03-24 16:10:18.867622 pyaedt-0.6.70/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    48211 2023-04-03 14:45:49.232236 pyaedt-0.6.70/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33242 2023-04-07 10:17:20.946469 pyaedt-0.6.70/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    43680 2023-04-06 17:49:40.538145 pyaedt-0.6.70/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    46506 2023-04-06 09:50:14.101200 pyaedt-0.6.70/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    57133 2023-04-06 16:51:57.478550 pyaedt-0.6.70/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   101238 2023-04-07 14:18:16.247983 pyaedt-0.6.70/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    10889 2023-04-01 08:45:04.717291 pyaedt-0.6.70/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-03-24 16:10:18.867622 pyaedt-0.6.70/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3256 2023-04-01 08:45:04.717291 pyaedt-0.6.70/pyaedt/emit_core/EmitConstants.py
--rw-r--r--   0        0        0      448 2023-03-24 16:10:18.867622 pyaedt-0.6.70/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0        2 2023-03-24 16:10:18.867622 pyaedt-0.6.70/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     6825 2023-04-06 11:17:50.336000 pyaedt-0.6.70/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    11615 2023-04-06 11:17:50.351622 pyaedt-0.6.70/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-03-27 12:10:05.425190 pyaedt-0.6.70/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    11758 2023-03-24 16:10:18.867622 pyaedt-0.6.70/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.867622 pyaedt-0.6.70/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3021 2023-03-24 16:10:18.883250 pyaedt-0.6.70/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83375 2023-03-24 16:10:18.883250 pyaedt-0.6.70/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-04-07 12:58:03.133395 pyaedt-0.6.70/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    19616 2023-03-24 16:10:18.883250 pyaedt-0.6.70/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3416 2023-03-30 13:11:17.942263 pyaedt-0.6.70/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    62967 2023-04-07 12:39:52.648098 pyaedt-0.6.70/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-03-24 16:10:18.883250 pyaedt-0.6.70/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-03-24 16:10:18.883250 pyaedt-0.6.70/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0    62296 2023-04-07 12:58:03.133395 pyaedt-0.6.70/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11301 2023-03-24 16:10:18.883250 pyaedt-0.6.70/pyaedt/generic/process.py
--rw-r--r--   0        0        0    19736 2023-03-24 16:10:18.883250 pyaedt-0.6.70/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3466 2023-03-24 16:10:18.883250 pyaedt-0.6.70/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60355 2023-03-24 16:10:18.898857 pyaedt-0.6.70/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17088 2023-04-07 12:58:03.149048 pyaedt-0.6.70/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-03-24 16:10:18.898857 pyaedt-0.6.70/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   253030 2023-04-06 12:36:53.912898 pyaedt-0.6.70/pyaedt/hfss.py
--rw-r--r--   0        0        0    82916 2023-04-06 11:56:42.332868 pyaedt-0.6.70/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   151079 2023-03-24 16:10:18.898857 pyaedt-0.6.70/pyaedt/icepak.py
--rw-r--r--   0        0        0   113532 2023-04-06 10:00:10.649919 pyaedt-0.6.70/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7816 2023-03-24 16:10:18.907751 pyaedt-0.6.70/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    23989 2023-03-24 16:10:18.907751 pyaedt-0.6.70/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-04-03 09:31:32.851623 pyaedt-0.6.70/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-03-24 16:10:18.907751 pyaedt-0.6.70/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-04-03 09:31:32.851623 pyaedt-0.6.70/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-03-30 19:37:04.658681 pyaedt-0.6.70/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-03-30 19:37:04.658681 pyaedt-0.6.70/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-03-24 16:10:18.907751 pyaedt-0.6.70/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0     8973 2023-03-24 16:10:18.907751 pyaedt-0.6.70/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-03-24 16:10:18.907751 pyaedt-0.6.70/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-03-24 16:10:18.914516 pyaedt-0.6.70/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-03-24 16:10:18.914516 pyaedt-0.6.70/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-03-24 16:10:18.914516 pyaedt-0.6.70/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-03-24 16:10:18.914516 pyaedt-0.6.70/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3507 2023-03-30 19:37:04.658681 pyaedt-0.6.70/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-03-24 16:10:18.914516 pyaedt-0.6.70/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-03-24 16:10:18.914516 pyaedt-0.6.70/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-03-24 16:10:18.914516 pyaedt-0.6.70/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-03-24 16:10:18.914516 pyaedt-0.6.70/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14076 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    19994 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18540 2023-03-24 16:10:18.930163 pyaedt-0.6.70/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16809 2023-04-07 12:58:03.149048 pyaedt-0.6.70/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120831 2023-04-05 05:51:09.186354 pyaedt-0.6.70/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   194519 2023-04-06 11:56:42.332868 pyaedt-0.6.70/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   114949 2023-04-06 10:00:10.649919 pyaedt-0.6.70/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11332 2023-03-24 16:10:18.945688 pyaedt-0.6.70/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   119547 2023-04-06 10:00:10.649919 pyaedt-0.6.70/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.945688 pyaedt-0.6.70/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    29079 2023-04-06 11:56:42.332868 pyaedt-0.6.70/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49002 2023-04-06 10:00:10.649919 pyaedt-0.6.70/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59259 2023-04-06 11:56:42.332868 pyaedt-0.6.70/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53056 2023-04-06 10:00:10.665549 pyaedt-0.6.70/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    42008 2023-04-07 12:45:00.476659 pyaedt-0.6.70/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32231 2023-03-24 16:10:18.945688 pyaedt-0.6.70/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8157 2023-03-24 16:10:18.945688 pyaedt-0.6.70/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63322 2023-04-06 11:56:42.348489 pyaedt-0.6.70/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15094 2023-03-24 16:10:18.945688 pyaedt-0.6.70/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.945688 pyaedt-0.6.70/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    31901 2023-04-06 10:00:10.665549 pyaedt-0.6.70/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    67799 2023-03-24 16:10:18.945688 pyaedt-0.6.70/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6902 2023-03-24 16:10:18.945688 pyaedt-0.6.70/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    48446 2023-04-06 11:56:42.348489 pyaedt-0.6.70/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    30435 2023-03-24 16:10:18.961334 pyaedt-0.6.70/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49786 2023-03-28 09:04:51.922409 pyaedt-0.6.70/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.961334 pyaedt-0.6.70/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    58183 2023-04-06 10:00:10.665549 pyaedt-0.6.70/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    21513 2023-03-24 16:10:18.961334 pyaedt-0.6.70/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30108 2023-03-31 15:10:27.403749 pyaedt-0.6.70/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   113864 2023-04-06 09:22:50.539831 pyaedt-0.6.70/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71549 2023-03-24 16:10:18.961334 pyaedt-0.6.70/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-03-24 16:10:18.961334 pyaedt-0.6.70/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51910 2023-03-24 16:10:18.961334 pyaedt-0.6.70/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    37371 2023-03-31 10:06:49.073815 pyaedt-0.6.70/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82846 2023-03-24 16:10:18.961334 pyaedt-0.6.70/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28306 2023-03-24 16:43:00.406402 pyaedt-0.6.70/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53168 2023-04-07 14:18:16.263614 pyaedt-0.6.70/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11919 2023-03-24 16:10:18.961334 pyaedt-0.6.70/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    26048 2023-03-31 15:10:27.419349 pyaedt-0.6.70/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-03-24 16:10:18.976973 pyaedt-0.6.70/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   172123 2023-04-06 11:56:42.348489 pyaedt-0.6.70/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64104 2023-03-24 16:10:18.976973 pyaedt-0.6.70/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   116130 2023-04-06 10:00:10.665549 pyaedt-0.6.70/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33226 2023-04-07 14:18:16.263614 pyaedt-0.6.70/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.976973 pyaedt-0.6.70/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    28652 2023-03-24 16:10:18.976973 pyaedt-0.6.70/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103276 2023-03-24 16:10:18.976973 pyaedt-0.6.70/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   124676 2023-04-07 09:15:24.184408 pyaedt-0.6.70/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    92404 2023-03-28 20:31:48.903203 pyaedt-0.6.70/pyaedt/q3d.py
--rw-r--r--   0        0        0    10556 2023-03-24 16:10:18.976973 pyaedt-0.6.70/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.976973 pyaedt-0.6.70/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-03-24 16:10:18.976973 pyaedt-0.6.70/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-03-24 16:10:18.976973 pyaedt-0.6.70/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-03-24 16:10:18.976973 pyaedt-0.6.70/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-04-03 16:00:03.137655 pyaedt-0.6.70/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-03-24 16:10:18.992592 pyaedt-0.6.70/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-03-24 16:10:18.992592 pyaedt-0.6.70/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-03-24 16:10:18.992592 pyaedt-0.6.70/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-03-28 22:11:07.622485 pyaedt-0.6.70/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-03-28 22:11:07.622485 pyaedt-0.6.70/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-03-28 22:11:07.622485 pyaedt-0.6.70/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-03-24 16:10:18.992592 pyaedt-0.6.70/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-03-28 22:11:07.622485 pyaedt-0.6.70/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-03-28 22:11:07.622485 pyaedt-0.6.70/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-03-28 22:11:07.622485 pyaedt-0.6.70/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-03-28 22:11:07.622485 pyaedt-0.6.70/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-03-28 22:11:07.622485 pyaedt-0.6.70/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-03-28 22:11:07.622485 pyaedt-0.6.70/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-03-24 16:10:18.992592 pyaedt-0.6.70/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-03-28 22:11:07.622485 pyaedt-0.6.70/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7601 2023-03-24 16:10:18.992592 pyaedt-0.6.70/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10373 2023-03-24 16:10:18.992592 pyaedt-0.6.70/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-03-24 16:10:18.992592 pyaedt-0.6.70/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4090 2023-04-06 12:42:41.798409 pyaedt-0.6.70/pyproject.toml
--rw-r--r--   0        0        0    14895 1970-01-01 00:00:00.000000 pyaedt-0.6.70/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-03-24 16:12:59.270687 pyaedt-0.6.71/LICENSE
+-rw-r--r--   0        0        0     9857 2023-04-07 12:13:26.641029 pyaedt-0.6.71/README.rst
+-rw-r--r--   0        0        0     2503 2023-04-14 08:04:16.194632 pyaedt-0.6.71/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26253 2023-03-24 16:13:01.176952 pyaedt-0.6.71/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-03-24 16:13:01.176952 pyaedt-0.6.71/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88739 2023-04-07 18:09:06.609599 pyaedt-0.6.71/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    41260 2023-04-06 10:12:59.809616 pyaedt-0.6.71/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17009 2023-04-06 10:12:59.809616 pyaedt-0.6.71/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19795 2023-04-06 10:12:59.809616 pyaedt-0.6.71/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4374 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4539 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   126722 2023-03-27 07:03:01.756479 pyaedt-0.6.71/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    72583 2023-04-03 13:04:44.954527 pyaedt-0.6.71/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12433 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    37014 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    57605 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10034 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    57176 2023-04-13 13:45:42.136087 pyaedt-0.6.71/pyaedt/desktop.py
+-rw-r--r--   0        0        0    23552 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1092 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0    23996 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   249856 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.dll
+-rw-r--r--   0        0        0   481931 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.xml
+-rw-r--r--   0        0        0   131072 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.dll
+-rw-r--r--   0        0        0    85860 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.xml
+-rw-r--r--   0        0        0    86016 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.RtfRendering-gdi.dll
+-rw-r--r--   0        0        0    51586 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.RtfRendering-gdi.xml
+-rw-r--r--   0        0        0   700336 2023-03-24 16:13:01.223835 pyaedt-0.6.71/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   707721 2023-03-24 16:13:01.223835 pyaedt-0.6.71/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0   585728 2023-03-24 16:13:01.223835 pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp-gdi.dll
+-rw-r--r--   0        0        0  1164073 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp-gdi.xml
+-rw-r--r--   0        0        0    94208 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp.Charting-gdi.dll
+-rw-r--r--   0        0        0   129427 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp.Charting-gdi.xml
+-rw-r--r--   0        0        0     9728 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/MigraDoc.DocumentObjectModel-gdi.resources.dll
+-rw-r--r--   0        0        0     7168 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/MigraDoc.Rendering-gdi.resources.dll
+-rw-r--r--   0        0        0     7168 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/MigraDoc.RtfRendering-gdi.resources.dll
+-rw-r--r--   0        0        0     5120 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/PdfSharp-gdi.resources.dll
+-rw-r--r--   0        0        0     4608 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/PdfSharp.Charting-gdi.resources.dll
+-rw-r--r--   0        0        0    23488 2023-03-24 16:43:09.200130 pyaedt-0.6.71/pyaedt/downloads.py
+-rw-r--r--   0        0        0   130992 2023-04-13 18:44:13.853500 pyaedt-0.6.71/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-04-06 16:52:05.688099 pyaedt-0.6.71/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    88157 2023-04-12 15:16:57.734625 pyaedt-0.6.71/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    32856 2023-04-06 16:52:05.688099 pyaedt-0.6.71/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0      937 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      324 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/edb_core/edb_data/edb_builder.py
+-rw-r--r--   0        0        0     1166 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    65580 2023-04-13 08:40:21.234448 pyaedt-0.6.71/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20305 2023-04-06 16:52:05.703674 pyaedt-0.6.71/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     4724 2023-04-03 15:08:34.103504 pyaedt-0.6.71/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    58397 2023-04-03 15:08:34.103504 pyaedt-0.6.71/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32298 2023-04-06 16:52:05.703674 pyaedt-0.6.71/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0    96895 2023-04-13 10:24:29.982183 pyaedt-0.6.71/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36296 2023-03-24 16:43:09.200130 pyaedt-0.6.71/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    31276 2023-04-06 16:52:05.703674 pyaedt-0.6.71/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     4147 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2425 2023-03-27 19:21:09.792652 pyaedt-0.6.71/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     2657 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    60230 2023-04-13 08:40:21.234448 pyaedt-0.6.71/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2844 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7706 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4646 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11163 2023-04-03 15:08:34.103504 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21750 2023-04-03 15:08:34.103504 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    48211 2023-04-03 15:08:34.103504 pyaedt-0.6.71/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33242 2023-04-07 12:13:26.672217 pyaedt-0.6.71/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    43680 2023-04-07 07:07:57.602451 pyaedt-0.6.71/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    46506 2023-04-06 10:00:43.540000 pyaedt-0.6.71/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    57133 2023-04-06 16:52:05.703674 pyaedt-0.6.71/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   108085 2023-04-13 08:40:21.234448 pyaedt-0.6.71/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    10889 2023-03-31 19:32:16.029670 pyaedt-0.6.71/pyaedt/emit.py
+-rw-r--r--   0        0        0     3555 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3256 2023-03-31 19:32:16.029670 pyaedt-0.6.71/pyaedt/emit_core/EmitConstants.py
+-rw-r--r--   0        0        0      448 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0        2 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     6796 2023-04-10 16:06:04.843675 pyaedt-0.6.71/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    11153 2023-04-10 16:06:04.843675 pyaedt-0.6.71/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-03-27 11:43:10.713537 pyaedt-0.6.71/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    11758 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3021 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83375 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-04-07 12:58:12.911113 pyaedt-0.6.71/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    19616 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3416 2023-03-30 13:17:30.662219 pyaedt-0.6.71/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    62967 2023-04-07 13:54:16.226712 pyaedt-0.6.71/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    25808 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     6989 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0    62296 2023-04-07 12:58:12.911113 pyaedt-0.6.71/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11301 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    19736 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3466 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60355 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17088 2023-04-07 12:58:12.911113 pyaedt-0.6.71/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   252857 2023-04-13 10:51:58.724974 pyaedt-0.6.71/pyaedt/hfss.py
+-rw-r--r--   0        0        0    82916 2023-04-06 10:12:59.840928 pyaedt-0.6.71/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   157774 2023-04-13 16:06:58.693317 pyaedt-0.6.71/pyaedt/icepak.py
+-rw-r--r--   0        0        0   118317 2023-04-14 08:04:16.194632 pyaedt-0.6.71/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7816 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    23989 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-04-03 09:42:52.307879 pyaedt-0.6.71/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-04-03 09:42:52.307879 pyaedt-0.6.71/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3695 2023-03-30 18:43:32.942201 pyaedt-0.6.71/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     2380 2023-03-30 18:43:32.942201 pyaedt-0.6.71/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0     8973 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     3731 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     3507 2023-03-30 18:43:32.942201 pyaedt-0.6.71/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-03-24 16:13:01.317589 pyaedt-0.6.71/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-03-24 16:13:01.317589 pyaedt-0.6.71/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14076 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    19994 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18540 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16809 2023-04-07 12:58:12.911113 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120831 2023-04-05 05:51:01.697466 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   194519 2023-04-06 10:24:56.942325 pyaedt-0.6.71/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   115251 2023-04-13 15:34:05.970087 pyaedt-0.6.71/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11332 2023-03-24 16:13:01.348840 pyaedt-0.6.71/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   119547 2023-04-06 09:42:17.714071 pyaedt-0.6.71/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.348840 pyaedt-0.6.71/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    29079 2023-04-06 10:24:56.942325 pyaedt-0.6.71/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49002 2023-04-06 09:42:17.714071 pyaedt-0.6.71/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59392 2023-04-11 17:32:37.677113 pyaedt-0.6.71/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53056 2023-04-06 09:42:17.714071 pyaedt-0.6.71/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12588 2023-04-13 16:06:58.693317 pyaedt-0.6.71/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42008 2023-04-07 13:54:16.226712 pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    32175 2023-04-13 10:24:29.982183 pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8157 2023-03-24 16:13:01.348840 pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63043 2023-04-13 10:24:29.982183 pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15094 2023-03-24 16:13:01.348840 pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.348840 pyaedt-0.6.71/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    31983 2023-04-13 10:24:29.982183 pyaedt-0.6.71/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    67799 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6902 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    48446 2023-04-06 10:24:56.942325 pyaedt-0.6.71/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    31270 2023-04-13 15:34:05.970087 pyaedt-0.6.71/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49786 2023-03-28 09:14:52.645654 pyaedt-0.6.71/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65526 2023-04-13 15:34:05.985626 pyaedt-0.6.71/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    21619 2023-04-13 15:34:05.985626 pyaedt-0.6.71/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    30108 2023-03-31 13:49:23.220683 pyaedt-0.6.71/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   113864 2023-04-06 09:22:52.765550 pyaedt-0.6.71/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71549 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51910 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    39609 2023-04-13 15:34:05.985626 pyaedt-0.6.71/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82846 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28306 2023-03-24 16:43:09.215755 pyaedt-0.6.71/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53168 2023-04-07 13:54:16.226712 pyaedt-0.6.71/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11919 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    26048 2023-03-31 13:49:23.236244 pyaedt-0.6.71/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   172107 2023-04-13 10:24:29.997810 pyaedt-0.6.71/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64104 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   116130 2023-04-06 09:42:17.729701 pyaedt-0.6.71/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33226 2023-04-07 13:54:16.226712 pyaedt-0.6.71/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    28652 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103276 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   124676 2023-04-07 09:25:28.374503 pyaedt-0.6.71/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95492 2023-04-13 10:24:29.997810 pyaedt-0.6.71/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10556 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-04-03 14:30:32.207324 pyaedt-0.6.71/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-03-24 16:13:01.395712 pyaedt-0.6.71/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7601 2023-03-24 16:13:01.395712 pyaedt-0.6.71/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10373 2023-03-24 16:13:01.395712 pyaedt-0.6.71/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-03-24 16:13:01.395712 pyaedt-0.6.71/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4066 2023-04-12 13:46:49.217739 pyaedt-0.6.71/pyproject.toml
+-rw-r--r--   0        0        0    14845 1970-01-01 00:00:00.000000 pyaedt-0.6.71/PKG-INFO
```

### Comparing `pyaedt-0.6.70/LICENSE` & `pyaedt-0.6.71/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/README.rst` & `pyaedt-0.6.71/README.rst`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/__init__.py` & `pyaedt-0.6.71/pyaedt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 os.environ["ANSYSEM_FEATURE_SF6694_NON_GRAPHICAL_COMMAND_EXECUTION_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.70"
+__version__ = "0.6.71"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
 from pyaedt.generic.general_methods import _pythonver
```

### Comparing `pyaedt-0.6.70/pyaedt/aedt_logger.py` & `pyaedt-0.6.71/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.71/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/Analysis.py` & `pyaedt-0.6.71/pyaedt/application/Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1860,23 +1860,25 @@
             self.logger.info("Batch job launched.")
 
         else:
             subprocess.Popen(batch_run)
             self.logger.info("Batch job finished.")
 
         if machine == "localhost":
-            while not os.path.exists(queue_file_completed):
+            while not os.path.exists(queue_file):
                 time.sleep(0.5)
             with open(queue_file, "r") as f:
                 lines = f.readlines()
                 for line in lines:
                     if "JobID" in line:
                         ls = line.split("=")[1].strip().strip("'")
                         self.last_run_job = ls
                         self.last_run_log = os.path.join(filename + ".batchinfo", project_name + "-" + ls + ".log")
+            while not os.path.exists(queue_file_completed):
+                time.sleep(0.5)
         return True
 
     @pyaedt_function_handler()
     def submit_job(
         self, clustername, aedt_full_exe_path=None, numnodes=1, numcores=32, wait_for_license=True, setting_file=None
     ):
         """Submit a job to be solved on a cluster.
```

### Comparing `pyaedt-0.6.70/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.71/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.71/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.71/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.71/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.71/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.71/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/Design.py` & `pyaedt-0.6.71/pyaedt/application/Design.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/JobManager.py` & `pyaedt-0.6.71/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/Variables.py` & `pyaedt-0.6.71/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.71/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/application/design_solutions.py` & `pyaedt-0.6.71/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/circuit.py` & `pyaedt-0.6.71/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/common_rpc.py` & `pyaedt-0.6.71/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/desktop.py` & `pyaedt-0.6.71/pyaedt/desktop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1513,14 +1513,17 @@
 
             commands = []
             if package_path.startswith("git") and package_name:
                 commands.append([executable, "-m", "pip", "uninstall", "--yes", package_name])
 
             commands.append([executable, "-m", "pip", "install", "--upgrade", package_path])
 
+            if self.aedt_version_id == "2023.1" and is_windows and "AnsysEM" in sys.base_prefix:
+                commands.append([executable, "-m", "pip", "uninstall", "--yes", "pywin32"])
+
             for command in commands:
                 if is_linux:
                     p = subprocess.Popen(command)
                 else:
                     p = subprocess.Popen(" ".join(command))
                 p.wait()
```

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.xml` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.xml` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.RtfRendering-gdi.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.RtfRendering-gdi.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/MigraDoc.RtfRendering-gdi.xml` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.RtfRendering-gdi.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/PdfSharp-gdi.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp-gdi.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/PdfSharp-gdi.xml` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp-gdi.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/PdfSharp.Charting-gdi.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp.Charting-gdi.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/PdfSharp.Charting-gdi.xml` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp.Charting-gdi.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/de/MigraDoc.DocumentObjectModel-gdi.resources.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/MigraDoc.DocumentObjectModel-gdi.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/de/MigraDoc.Rendering-gdi.resources.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/MigraDoc.Rendering-gdi.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/de/MigraDoc.RtfRendering-gdi.resources.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/MigraDoc.RtfRendering-gdi.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/de/PdfSharp-gdi.resources.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/PdfSharp-gdi.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/dlls/PDFReport/de/PdfSharp.Charting-gdi.resources.dll` & `pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/PdfSharp.Charting-gdi.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/downloads.py` & `pyaedt-0.6.71/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb.py` & `pyaedt-0.6.71/pyaedt/edb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module contains the ``Edb`` class.
 
 This module is implicitily loaded in HFSS 3D Layout when launched.
 
 """
-import gc
 import os
 import re
 import shutil
 import sys
 import time
 import traceback
 import warnings
@@ -284,15 +283,14 @@
         self._layout_instance = None
         self._variables = None
         # time.sleep(2)
         # gc.collect()
 
     @pyaedt_function_handler()
     def _init_objects(self):
-        time.sleep(1)
         self._components = Components(self)
         self._stackup = Stackup(self)
         self._padstack = EdbPadstacks(self)
         self._siwave = EdbSiwave(self)
         self._hfss = EdbHfss(self)
         self._nets = EdbNets(self)
         self._core_primitives = EdbLayout(self)
@@ -1167,38 +1165,36 @@
             ``True`` when successful, ``False`` when failed.
 
         """
         self._db.Close()
         if self.log_name and settings.enable_local_log_file:
             self._global_logger.remove_file_logger(os.path.splitext(os.path.split(self.log_name)[-1])[0])
             self._logger = self._global_logger
-        time.sleep(2)
         start_time = time.time()
         self._wait_for_file_release()
         elapsed_time = time.time() - start_time
         self.logger.info("EDB file release time: {0:.2f}ms".format(elapsed_time * 1000.0))
         self._clean_variables()
-        timeout = 4
-        time.sleep(2)
-        while gc.collect() != 0 and timeout > 0:
-            time.sleep(1)
-            timeout -= 1
         return True
 
     @pyaedt_function_handler()
     def save_edb(self):
         """Save the EDB file.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
         self._db.Save()
+        start_time = time.time()
+        self._wait_for_file_release()
+        elapsed_time = time.time() - start_time
+        self.logger.info("EDB file save time: {0:.2f}ms".format(elapsed_time * 1000.0))
         return True
 
     @pyaedt_function_handler()
     def save_edb_as(self, fname):
         """Save the EDB file as another file.
 
         Parameters
@@ -1209,14 +1205,18 @@
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
         self._db.SaveAs(fname)
+        start_time = time.time()
+        self._wait_for_file_release()
+        elapsed_time = time.time() - start_time
+        self.logger.info("EDB file save time: {0:.2f}ms".format(elapsed_time * 1000.0))
         self.edbpath = self._db.GetDirectory()
         if self.log_name:
             self._global_logger.remove_file_logger(os.path.splitext(os.path.split(self.log_name)[-1])[0])
             self._logger = self._global_logger
 
         self.log_name = os.path.join(
             os.path.dirname(fname), "pyaedt_" + os.path.splitext(os.path.split(fname)[-1])[0] + ".log"
```

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/components.py` & `pyaedt-0.6.71/pyaedt/edb_core/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,15 +306,15 @@
         --------
 
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder")
         >>> edbapp.components.resistors
         """
         self._res = {}
-        for el, val in self.components.items():
+        for el, val in self.instances.items():
             if val.type == "Resistor":
                 self._res[el] = val
         return self._res
 
     @property
     def capacitors(self):
         """Capacitors.
@@ -328,15 +328,15 @@
         --------
 
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder")
         >>> edbapp.components.capacitors
         """
         self._cap = {}
-        for el, val in self.components.items():
+        for el, val in self.instances.items():
             if val.type == "Capacitor":
                 self._cap[el] = val
         return self._cap
 
     @property
     def inductors(self):
         """Inductors.
@@ -351,15 +351,15 @@
 
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder")
         >>> edbapp.components.inductors
 
         """
         self._ind = {}
-        for el, val in self.components.items():
+        for el, val in self.instances.items():
             if val.type == "Inductor":
                 self._ind[el] = val
         return self._ind
 
     @property
     def ICs(self):
         """Integrated circuits.
@@ -374,15 +374,15 @@
 
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder")
         >>> edbapp.components.ICs
 
         """
         self._ics = {}
-        for el, val in self.components.items():
+        for el, val in self.instances.items():
             if val.type == "IC":
                 self._ics[el] = val
         return self._ics
 
     @property
     def IOs(self):
         """Circuit inupts and outputs.
@@ -397,15 +397,15 @@
 
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder")
         >>> edbapp.components.IOs
 
         """
         self._ios = {}
-        for el, val in self.components.items():
+        for el, val in self.instances.items():
             if val.type == "IO":
                 self._ios[el] = val
         return self._ios
 
     @property
     def Others(self):
         """Other core components.
@@ -420,15 +420,15 @@
 
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder")
         >>> edbapp.components.others
 
         """
         self._others = {}
-        for el, val in self.components.items():
+        for el, val in self.instances.items():
             if val.type == "Other":
                 self._others[el] = val
         return self._others
 
     @property
     def components_by_partname(self):
         """Components by part name.
@@ -443,15 +443,15 @@
 
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder")
         >>> edbapp.components.components_by_partname
 
         """
         self._comps_by_part = {}
-        for el, val in self.components.items():
+        for el, val in self.instances.items():
             if val.partname in self._comps_by_part.keys():
                 self._comps_by_part[val.partname].append(val)
             else:
                 self._comps_by_part[val.partname] = [val]
         return self._comps_by_part
 
     @pyaedt_function_handler()
@@ -505,15 +505,15 @@
         list
             List of components that belong to the signal nets.
 
         """
         cmp_list = []
         if isinstance(netlist, str):
             netlist = [netlist]
-        components = list(self.components.keys())
+        components = list(self.instances.keys())
         for refdes in components:
             cmpnets = self._cmp[refdes].nets
             if set(cmpnets).intersection(set(netlist)):
                 cmp_list.append(refdes)
         return cmp_list
 
     @pyaedt_function_handler()
@@ -1444,15 +1444,15 @@
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder")
         >>> list_of_deleted_rlcs = edbapp.components.delete_single_pin_rlc()
         >>> print(list_of_deleted_rlcs)
 
         """
         deleted_comps = []
-        for comp, val in self.components.items():
+        for comp, val in self.instances.items():
             if val.numpins < 2 and val.type in ["Resistor", "Capacitor", "Inductor"]:
                 val.edbcomponent.Delete()
                 deleted_comps.append(comp)
         self.refresh_components()
         self._pedb._logger.info("Deleted {} components".format(len(deleted_comps)))
 
         return deleted_comps
@@ -1506,15 +1506,15 @@
         >>> edbapp = Edb("myaedbfolder")
         >>> edbapp.components.delete("A1")
 
         """
         edb_cmp = self.get_component_by_name(component_name)
         if edb_cmp is not None:
             edb_cmp.Delete()
-            if edb_cmp in list(self.components.keys()):
+            if edb_cmp in list(self.instances.keys()):
                 del self.components[edb_cmp]
             return True
         return False
 
     @pyaedt_function_handler()
     def disable_rlc_component(self, component_name):
         """Disable a RLC component.
@@ -1767,15 +1767,15 @@
         """
         with open(bom_file, "r") as f:
             Lines = f.readlines()
             found = False
             refdescolumn = None
             comptypecolumn = None
             valuecolumn = None
-            unmount_comp_list = list(self.components.keys())
+            unmount_comp_list = list(self.instances.keys())
             for line in Lines:
                 content_line = [i.strip() for i in line.split(delimiter)]
                 if valuefield in content_line:
                     valuecolumn = content_line.index(valuefield)
                 if comptype in content_line:
                     comptypecolumn = content_line.index(comptype)
                 if refdes in content_line:
@@ -1828,15 +1828,15 @@
             if the column does not exist.
         Returns
         -------
         bool
         """
         with open(bom_file, "r") as f:
             lines = f.readlines()
-            unmount_comp_list = list(self.components.keys())
+            unmount_comp_list = list(self.instances.keys())
             for l in lines[1:]:
                 l = l.replace(" ", "").replace("\n", "")
                 if not l:
                     continue
                 l = l.split(delimiter)
 
                 refdes = l[refdes_col]
@@ -1897,15 +1897,15 @@
         bom_file : str
             Full path to the BOM file, which is a delimited text file.
         delimiter : str, optional
             Value to use for the delimiter. The default is ``","``.
         """
         with open(bom_file, "w") as f:
             f.writelines([delimiter.join(["RefDes", "Part name", "Type", "Value\n"])])
-            for refdes, comp in self.components.items():
+            for refdes, comp in self.instances.items():
                 if not comp.is_enabled and comp.type in ["Resistor", "Capacitor", "Inductor"]:
                     continue
                 part_name = comp.partname
                 comp_type = comp.type
                 if comp_type == "Resistor":
                     value = comp.res_value
                 elif comp_type == "Capacitor":
@@ -2153,15 +2153,15 @@
 
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder", "project name", "release version")
         >>> edbapp.components.get_rats()
 
         """
         df_list = []
-        for refdes in self.components.keys():
+        for refdes in self.instances.keys():
             df = self.get_component_net_connection_info(refdes)
             df_list.append(df)
         return df_list
 
     def get_through_resistor_list(self, threshold=1):
         """Retrieve through resistors.
```

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,14 +472,15 @@
                 temp.extend(list(self._edb_sweep_data.SetFrequencies(i[1], i[2], i[3])))
             elif i[0] == "linear scale":
                 temp.extend(list(self._edb_sweep_data.SetFrequencies(i[1], i[2], i[3])))
             elif i[0] == "log scale":
                 temp.extend(list(self._edb_sweep_data.SetLogFrequencies(i[1], i[2], i[3])))
             else:
                 return False
+        self._edb_sweep_data.Frequencies.Clear()
         for i in temp:
             self._edb_sweep_data.Frequencies.Add(i)
         return self._update_sweep()
 
 
 class MeshOperation(object):
     """Mesh Operation Class."""
@@ -1180,20 +1181,16 @@
         bool
             ``True`` if method is successful, ``False`` otherwise.
         """
         low_freq_adapt_data = self._parent._edb.simsetupdata.AdaptiveFrequencyData()
         low_freq_adapt_data.MaxDelta = self._parent._edb.edb_value(max_delta_s).ToString()
         low_freq_adapt_data.MaxPasses = max_num_passes
         low_freq_adapt_data.AdaptiveFrequency = self._parent._edb.edb_value(frequency).ToString()
-        high_freq_adapt_data = self._parent._edb.simsetupdata.AdaptiveFrequencyData()
-        high_freq_adapt_data.MaxDelta = self._parent._edb.edb_value(max_delta_s).ToString()
-        high_freq_adapt_data.MaxPasses = max_num_passes
-        high_freq_adapt_data.AdaptiveFrequency = self._parent._edb.edb_value(frequency).ToString()
+        self.adaptive_settings.AdaptiveFrequencyDataList.Clear()
         self.adaptive_settings.AdaptiveFrequencyDataList.Add(low_freq_adapt_data)
-        self.adaptive_settings.AdaptiveFrequencyDataList.Add(high_freq_adapt_data)
         return self._parent._update_setup()
 
     @pyaedt_function_handler()
     def add_broadband_adaptive_frequency_data(
         self, low_frequency=0, high_frequency=10e9, max_num_passes=10, max_delta_s=0.02
     ):
         """Add a setup for frequency data.
@@ -1218,14 +1215,15 @@
         low_freq_adapt_data.MaxDelta = self._parent._edb.edb_value(max_delta_s).ToString()
         low_freq_adapt_data.MaxPasses = max_num_passes
         low_freq_adapt_data.AdaptiveFrequency = self._parent._edb.edb_value(low_frequency).ToString()
         high_freq_adapt_data = self._parent._edb.simsetupdata.AdaptiveFrequencyData()
         high_freq_adapt_data.MaxDelta = self._parent._edb.edb_value(max_delta_s).ToString()
         high_freq_adapt_data.MaxPasses = max_num_passes
         high_freq_adapt_data.AdaptiveFrequency = self._parent._edb.edb_value(high_frequency).ToString()
+        self.adaptive_settings.AdaptiveFrequencyDataList.Clear()
         self.adaptive_settings.AdaptiveFrequencyDataList.Add(low_freq_adapt_data)
         self.adaptive_settings.AdaptiveFrequencyDataList.Add(high_freq_adapt_data)
         return self._parent._update_setup()
 
 
 class DefeatureSettings(object):
     """Manages EDB methods for defeature settings."""
```

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -2006,15 +2006,15 @@
     Import DC thermal data when `True``
 
     >>> sim_setup.dc_per_pin_res_path = r"C:\temp\dc_pin_res_file"
     Provides the resistance per pin file path.
 
     >>> sim_setup.dc_per_pin_use_pin_format = True
 
-    When ``True activate the pin format.
+    When ``True`` activate the pin format.
 
     >>> sim_setup.dc_use_loop_res_for_per_pin = True
 
     Activate the loop resistance usage per pin when ``True``
 
     >>> sim_setup.dc_via_report_path = 'C:\\temp\\via_report_file'
```

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/sources.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.71/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/general.py` & `pyaedt-0.6.71/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.71/pyaedt/edb_core/hfss.py`

 * *Files 1% similar despite different names*

```diff
@@ -701,27 +701,33 @@
         edge = self._edb.Cell.Terminal.PrimitiveEdge.Create(polygon, terminal_point)
         edges = convert_py_list_to_net_list(edge, self._edb.Cell.Terminal.Edge)
         edge_term = self._edb.Cell.Terminal.EdgeTerminal.Create(
             polygon.GetLayout(), polygon.GetNet(), port_name, edges, isRef=False
         )
         if force_circuit_port:
             edge_term.SetIsCircuitPort(True)
+        else:
+            edge_term.SetIsCircuitPort(False)
+
         if port_impedance:
             edge_term.SetImpedance(self._pedb.edb_value(port_impedance))
         edge_term.SetName(port_name)
         if reference_polygon and reference_point:
             ref_edge = self._edb.Cell.Terminal.PrimitiveEdge.Create(reference_polygon, reference_point)
             ref_edges = convert_py_list_to_net_list(ref_edge, self._edb.Cell.Terminal.Edge)
             ref_edge_term = self._edb.Cell.Terminal.EdgeTerminal.Create(
                 reference_polygon.GetLayout(), reference_polygon.GetNet(), port_name + "_ref", ref_edges, isRef=True
             )
             if reference_layer:
                 ref_edge_term.SetReferenceLayer(reference_layer)
             if force_circuit_port:
                 ref_edge_term.SetIsCircuitPort(True)
+            else:
+                ref_edge_term.SetIsCircuitPort(False)
+
             if port_impedance:
                 ref_edge_term.SetImpedance(self._pedb.edb_value(port_impedance))
             edge_term.SetReferenceTerminal(ref_edge_term)
         return True
 
     @pyaedt_function_handler()
     def create_wave_port(
```

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/layout.py` & `pyaedt-0.6.71/pyaedt/edb_core/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/materials.py` & `pyaedt-0.6.71/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/nets.py` & `pyaedt-0.6.71/pyaedt/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.71/pyaedt/edb_core/padstack.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.71/pyaedt/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.71/pyaedt/edb_core/stackup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 class Stackup(object):
     """Manages EDB methods for stackup accessible from `Edb.stackup` property."""
 
     def __getitem__(self, item):
         return self.layers[item]
 
     def __init__(self, pedb):
+        # parent caller class
         self._pedb = pedb
         self._lc = None
 
     @property
     def _logger(self):
         return self._pedb.logger
 
@@ -1299,14 +1300,160 @@
             self._edb_value(math.cos(_angle)), self._edb_value(-1 * math.sin(_angle)), zero_data
         )
         cell_inst2.Set3DTransformation(point_loc, point_from, point_to, rotation, point3d_t)
         self.refresh_layer_collection()
         return True
 
     @pyaedt_function_handler()
+    def place_instance(
+        self,
+        component_edb,
+        angle=0.0,
+        offset_x=0.0,
+        offset_y=0.0,
+        flipped_stackup=True,
+        place_on_top=True,
+        solder_height=0,
+    ):
+        """Place current Cell into another cell using 3d placement method.
+        Flip the current layer stackup of a layout if requested. Transform parameters currently not supported.
+
+        Parameters
+        ----------
+        component_edb : Edb
+            Cell to place in the current layout.
+        angle : double, optional
+            The rotation angle applied on the design.
+        offset_x : double, optional
+            The x offset value.
+        offset_y : double, optional
+            The y offset value.
+        flipped_stackup : bool, optional
+            Either if the current layout is inverted.
+            If `True` and place_on_top is `True` the stackup will be flipped before the merge.
+        place_on_top : bool, optional
+            Either if place the component_edb layout on Top or Bottom of destination Layout.
+        solder_height : float, optional
+            Solder Ball or Bumps eight.
+            This value will be added to the elevation to align the two layouts.
+
+        Returns
+        -------
+        bool
+            ``True`` when succeed ``False`` if not.
+
+        Examples
+        --------
+        >>> edb1 = Edb(edbpath=targetfile1,  edbversion="2021.2")
+        >>> edb2 = Edb(edbpath=targetfile2, edbversion="2021.2")
+        >>> hosting_cmp = edb1.components.get_component_by_name("U100")
+        >>> mounted_cmp = edb2.components.get_component_by_name("BGA")
+        >>> edb1.stackup.place_instance(edb2, angle=0.0, offset_x="1mm",
+        ...                                   offset_y="2mm", flipped_stackup=False, place_on_top=True,
+        ...                                   )
+        """
+        _angle = angle * math.pi / 180.0
+
+        if solder_height <= 0:
+            if flipped_stackup and not place_on_top or (place_on_top and not flipped_stackup):
+                minimum_elevation = None
+                layers_from_the_bottom = sorted(
+                    component_edb.stackup.signal_layers.values(), key=lambda lay: lay.upper_elevation
+                )
+                for lay in layers_from_the_bottom:
+                    if minimum_elevation is None:
+                        minimum_elevation = lay.lower_elevation
+                    elif lay.lower_elevation > minimum_elevation:
+                        break
+                    lay_solder_height = component_edb.stackup._get_solder_height(lay.name)
+                    solder_height = max(lay_solder_height, solder_height)
+                    component_edb.stackup._remove_solder_pec(lay.name)
+            else:
+                maximum_elevation = None
+                layers_from_the_top = sorted(
+                    component_edb.stackup.signal_layers.values(), key=lambda lay: -lay.upper_elevation
+                )
+                for lay in layers_from_the_top:
+                    if maximum_elevation is None:
+                        maximum_elevation = lay.upper_elevation
+                    elif lay.upper_elevation < maximum_elevation:
+                        break
+                    lay_solder_height = component_edb.stackup._get_solder_height(lay.name)
+                    solder_height = max(lay_solder_height, solder_height)
+                    component_edb.stackup._remove_solder_pec(lay.name)
+        edb_cell = component_edb.active_cell
+        _offset_x = self._edb_value(offset_x)
+        _offset_y = self._edb_value(offset_y)
+
+        if edb_cell.GetName() not in self._pedb.cell_names:
+            _dbCell = convert_py_list_to_net_list([edb_cell])
+            list_cells = self._pedb.db.CopyCells(_dbCell)
+            edb_cell = list_cells[0]
+        for cell in list(self._pedb.db.TopCircuitCells):
+            if cell.GetName() == edb_cell.GetName():
+                edb_cell = cell
+        # Keep Cell Independent
+        edb_cell.SetBlackBox(True)
+        rotation = self._edb_value(0.0)
+        if flipped_stackup:
+            rotation = self._edb_value(math.pi)
+
+        _offset_x = self._edb_value(offset_x)
+        _offset_y = self._edb_value(offset_y)
+
+        cell_inst2 = self._pedb.edb.Cell.Hierarchy.CellInstance.Create(
+            self._pedb.active_layout, edb_cell.GetName(), edb_cell.GetLayout()
+        )
+
+        stackup_source = self._pedb.edb.Cell.LayerCollection(edb_cell.GetLayout().GetLayerCollection())
+        stackup_target = self._pedb.edb.Cell.LayerCollection(self._pedb.active_layout.GetLayerCollection())
+
+        if place_on_top:
+            cell_inst2.SetPlacementLayer(
+                list(stackup_target.Layers(self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet))[0]
+            )
+        else:
+            cell_inst2.SetPlacementLayer(
+                list(stackup_target.Layers(self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet))[-1]
+            )
+        cell_inst2.SetIs3DPlacement(True)
+        sig_set = self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet
+        res = stackup_target.GetTopBottomStackupLayers(sig_set)
+        target_top_elevation = res[2]
+        target_bottom_elevation = res[4]
+        res_s = stackup_source.GetTopBottomStackupLayers(sig_set)
+        source_stack_top_elevation = res_s[2]
+        source_stack_bot_elevation = res_s[4]
+
+        if place_on_top and flipped_stackup:
+            elevation = target_top_elevation + source_stack_top_elevation
+        elif place_on_top:
+            elevation = target_top_elevation - source_stack_bot_elevation
+        elif flipped_stackup:
+            elevation = target_bottom_elevation + source_stack_bot_elevation
+            solder_height = -solder_height
+        else:
+            elevation = target_bottom_elevation - source_stack_top_elevation
+            solder_height = -solder_height
+
+        h_stackup = self._edb_value(elevation + solder_height)
+
+        zero_data = self._edb_value(0.0)
+        one_data = self._edb_value(1.0)
+        point3d_t = self._pedb.edb.Geometry.Point3DData(_offset_x, _offset_y, h_stackup)
+        point_loc = self._pedb.edb.Geometry.Point3DData(zero_data, zero_data, zero_data)
+        point_from = self._pedb.edb.Geometry.Point3DData(one_data, zero_data, zero_data)
+        point_to = self._pedb.edb.Geometry.Point3DData(
+            self._edb_value(math.cos(_angle)), self._edb_value(-1 * math.sin(_angle)), zero_data
+        )
+        cell_inst2.Set3DTransformation(point_loc, point_from, point_to, rotation, point3d_t)
+        self.refresh_layer_collection()
+        return True
+
+    @pyaedt_function_handler()
     def place_a3dcomp_3d_placement(self, a3dcomp_path, angle=0.0, offset_x=0.0, offset_y=0.0, place_on_top=True):
         """Place a 3D Component into current layout.
          3D Component ports are not visible via EDB. They will be visible after the EDB has been opened in Ansys
          Electronics Desktop as a project.
 
         Parameters
         ----------
@@ -2278,16 +2425,16 @@
                     if stackup_mode == "Laminate":
                         x = [
                             x_start - pad_size / 2 * scaling_f_pad,
                             x_start - pad_size / 2 * scaling_f_pad,
                             x_start + pad_size / 2 * scaling_f_pad,
                             x_start + pad_size / 2 * scaling_f_pad,
                         ]
-                        le = [e[1] for e in layers_data if e[0].name == layer][0]
-                        ue = [e[2] for e in layers_data if e[0].name == layer][0]
+                        le = [e[1] for e in layers_data if e[0].name == layer or layer == "Default"][0]
+                        ue = [e[2] for e in layers_data if e[0].name == layer or layer == "Default"][0]
                         y = [le, ue, ue, le]
                         # create the patch for that signal layer
                         plot_data.append([x, y, color_keys[color_index], None, 1.0, "fill"])
                     elif stackup_mode == "Overlapping":
                         # here evaluate the x based on the column evaluated before and the pad size
                         pass
```

### Comparing `pyaedt-0.6.70/pyaedt/emit.py` & `pyaedt-0.6.71/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.71/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/emit_core/EmitConstants.py` & `pyaedt-0.6.71/pyaedt/emit_core/EmitConstants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.71/pyaedt/emit_core/results/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,16 +144,16 @@
     def get_revision(self, revision_name=None):
         """
         Load the specified revision.
 
         Parameters
         ----------
         revision_name : str
-            Revision to load. If revision_name = None, the
-            latest revision will be returned.
+            Revision to load. The default is  ``None`` in which
+            case the latest revision will be returned.
 
         Returns
         -------
         rev:class:`pyaedt.modules.Revision`
             Specified ``Revision`` object that was loaded.
 
         Examples
@@ -182,18 +182,15 @@
                 warnings.warn("{} not found.".format(revision_name))
         return self.current_revision
 
     @pyaedt_function_handler()
     def analyze(self):
         """
         Analyze the current revision or create a new revision if
-         the design has changed.
-
-        Parameters
-        ----------
+        the design has changed.
 
         Returns
         -------
         rev:class:`pyaedt.modules.Revision`
             Specified ``Revision`` object that was generated.
 
         Examples
```

### Comparing `pyaedt-0.6.70/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.71/pyaedt/emit_core/results/revision.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,50 +305,26 @@
         if self.revision_loaded:
             freqs = self.emit_project._emit_api.get_active_frequencies(radio_name, band_name, tx_rx_mode, units)
         else:
             freqs = None
             self.result_mode_error()
         return freqs
 
-    @pyaedt_function_handler
-    def set_notes(self, notes):
+    @property
+    def notes(self):
         """
         Add notes to the revision.
 
-        Parameters
-        ----------
-        notes : str
-            Notes to add to the revision.
-
-        Returns
-        -------
-        None
-
         Examples
         ----------
-        >>> notes = "Added a filter to the WiFi Radio."
-        >>> freqs = aedtapp.results.current_revision.set_notes(notes)
+        >>> aedtapp.results.current_revision.notes = "Added a filter to the WiFi Radio."
+        >>> aedtapp.results.current_revision.notes
+        'Added a filter to the WiFi Radio.'
         """
         design = self.emit_project.odesktop.GetActiveProject().GetActiveDesign()
-        design.SetResultNotes(self.name, notes)
-        self.emit_project._emit_api.save_project()
-
-    @pyaedt_function_handler
-    def get_notes(self):
-        """
-        Get the current revision's notes.
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        notes : str
-            Notes to add to the revision.
+        return design.GetResultNotes(self.name)
 
-        Examples
-        ----------
-        >>> notes = aedtapp.results.current_revision.get_notes()
-        """
+    @notes.setter
+    def notes(self, notes):
         design = self.emit_project.odesktop.GetActiveProject().GetActiveDesign()
-        return design.GetResultNotes(self.name)
+        design.SetResultNotes(self.name, notes)
+        self.emit_project._emit_api.save_project()
```

### Comparing `pyaedt-0.6.70/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.71/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.71/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/clr_module.py` & `pyaedt-0.6.71/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/configurations.py` & `pyaedt-0.6.71/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/constants.py` & `pyaedt-0.6.71/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/design_types.py` & `pyaedt-0.6.71/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/filesystem.py` & `pyaedt-0.6.71/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/general_methods.py` & `pyaedt-0.6.71/pyaedt/generic/general_methods.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.71/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.71/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/plot.py` & `pyaedt-0.6.71/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/process.py` & `pyaedt-0.6.71/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.71/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.71/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/toolkit.py` & `pyaedt-0.6.71/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.71/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/hfss.py` & `pyaedt-0.6.71/pyaedt/hfss.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,23 @@
         props["ShowReporterFilter"] = False
         props["ReporterFilter"] = [True]
         props["Impedance"] = str(impedance) + "ohm"
         return self._create_boundary(portname, props, "Lumped Port")
 
     @pyaedt_function_handler()
     def _create_port_terminal(
-        self, objectname, int_line_stop, portname, renorm=True, deembed=None, iswaveport=False, impedance=None
+        self,
+        objectname,
+        int_line_stop,
+        portname,
+        renorm=True,
+        deembed=None,
+        iswaveport=False,
+        impedance=None,
+        terminals_rename=True,
     ):
         ref_conductors = self.modeler.convert_to_selections(int_line_stop, True)
         props = OrderedDict()
         props["Faces"] = int(objectname)
         props["IsWavePort"] = iswaveport
         props["ReferenceConductors"] = ref_conductors
         props["RenormalizeModes"] = True
@@ -410,28 +418,28 @@
                             ],
                         ],
                     ]
                     try:
                         self.odesign.ChangeProperty(properties)
                     except:  # pragma: no cover
                         self.logger.warning("Failed to change normalization.")
-
-                new_name = portname + "_T" + str(count)
-                properties = [
-                    "NAME:AllTabs",
-                    [
-                        "NAME:HfssTab",
-                        ["NAME:PropServers", "BoundarySetup:" + terminal],
-                        ["NAME:ChangedProps", ["NAME:Name", "Value:=", new_name]],
-                    ],
-                ]
-                try:
-                    self.odesign.ChangeProperty(properties)
-                except:  # pragma: no cover
-                    self.logger.warning("Failed to rename terminal {}.".format(terminal))
+                if terminals_rename:
+                    new_name = portname + "_T" + str(count)
+                    properties = [
+                        "NAME:AllTabs",
+                        [
+                            "NAME:HfssTab",
+                            ["NAME:PropServers", "BoundarySetup:" + terminal],
+                            ["NAME:ChangedProps", ["NAME:Name", "Value:=", new_name]],
+                        ],
+                    ]
+                    try:
+                        self.odesign.ChangeProperty(properties)
+                    except:  # pragma: no cover
+                        self.logger.warning("Failed to rename terminal {}.".format(terminal))
 
             if iswaveport:
                 boundary.type = "Wave Port"
             else:
                 boundary.type = "Lumped Port"
             props["Faces"] = [objectname]
             if iswaveport:
@@ -1556,14 +1564,17 @@
 
     @pyaedt_function_handler()
     def create_circuit_port_between_objects(
         self, startobj, endobject, axisdir=0, impedance=50, portname=None, renorm=True, renorm_impedance=50, deemb=False
     ):
         """Create a circuit port taking the closest edges of two objects.
 
+        .. deprecated:: 0.6.70
+        Use :func:`circuit_port` method instead.
+
         Parameters
         ----------
         startobj :
             Starting object for the integration line.
         endobject :
             Ending object for the integration line.
         axisdir : int or :class:`pyaedt.application.Analysis.Analysis.AxisDir`, optional
@@ -1602,32 +1613,35 @@
         ...                                "BoxCircuit2", "copper")
         >>> hfss.create_circuit_port_between_objects("BoxCircuit1", "BoxCircuit2",
         ...                                          hfss.AxisDir.XNeg, 50,
         ...                                          "CircuitExample", True, 50, False)
         'CircuitExample'
 
         """
-
-        if not self.modeler.does_object_exists(startobj) or not self.modeler.does_object_exists(endobject):
-            self.logger.error("One or both objects do not exist. Check and retry.")
-            return False
-        if self.solution_type in ["Modal", "Terminal", "Transient Network"]:
-            out, parallel = self.modeler.find_closest_edges(startobj, endobject, axisdir)
-            port_edges = []
-            portname = self._get_unique_source_name(portname, "Port")
-
-            return self._create_circuit_port(out, impedance, portname, renorm, deemb, renorm_impedance=renorm_impedance)
-        return False  # pragma: no cover
+        warnings.warn("Use :func:`circuit_port` method instead.", DeprecationWarning)
+        return self.circuit_port(
+            signal=startobj,
+            reference=endobject,
+            port_location=axisdir,
+            impedance=impedance,
+            name=portname,
+            renormalize=renorm,
+            renorm_impedance=renorm_impedance,
+            deembed=deemb,
+        )
 
     @pyaedt_function_handler()
     def create_lumped_port_between_objects(
         self, startobj, endobject, axisdir=0, impedance=50, portname=None, renorm=True, deemb=False, port_on_plane=True
     ):
         """Create a lumped port taking the closest edges of two objects.
 
+        .. deprecated:: 0.6.70
+        Use :func:`lumped_port` method instead.
+
         Parameters
         ----------
         startobj :
             Starting object for the integration line.
         endobject :
             Ending object for the integration line.
         axisdir : int or :class:`pyaedt.application.Analysis.Analysis.AxisDir`, optional
@@ -1669,45 +1683,26 @@
         >>> hfss.create_lumped_port_between_objects("BoxLumped1", "BoxLumped2",
         ...                                         hfss.AxisDir.XNeg, 50,
         ...                                         "LumpedPort", True, False)
         pyaedt INFO: Connection Correctly created
         'LumpedPort'
 
         """
-        startobj = self.modeler.convert_to_selections(startobj)
-        endobject = self.modeler.convert_to_selections(endobject)
-        if not self.modeler.does_object_exists(startobj) or not self.modeler.does_object_exists(endobject):
-            self.logger.error("One or both objects do not exist. Check and retry.")
-            return False
-
-        if self.solution_type in ["Modal", "Terminal", "Transient Network"]:
-            sheet_name, point0, point1 = self.modeler._create_sheet_from_object_closest_edge(
-                startobj, endobject, axisdir, port_on_plane
-            )
-
-            portname = self._get_unique_source_name(portname, "Port")
-
-            if "Modal" in self.solution_type:
-                return self._create_lumped_driven(sheet_name, point0, point1, impedance, portname, renorm, deemb)
-            else:
-                faces = self.modeler.get_object_faces(sheet_name)
-                if deemb:
-                    deembed = 0
-                else:
-                    deembed = None
-                return self._create_port_terminal(
-                    faces[0],
-                    endobject,
-                    portname,
-                    renorm=renorm,
-                    deembed=deembed,
-                    iswaveport=False,
-                    impedance=impedance,
-                )
-        return False  # pragma: no cover
+        warnings.warn("Use :func:`lumped_port` method instead.", DeprecationWarning)
+        return self.lumped_port(
+            signal=startobj,
+            reference=endobject,
+            create_port_sheet=True,
+            port_on_plane=port_on_plane,
+            integration_line=axisdir,
+            impedance=impedance,
+            name=portname,
+            renormalize=renorm,
+            deembed=deemb,
+        )
 
     @pyaedt_function_handler()
     def create_spiral_lumped_port(self, start_object, end_object, port_width=None):
         """Create a spiral lumped port between two adjacent objects.
 
         The two objects must have two adjacent, parallel, and identical faces.
         The faces must be a polygon (not a circle).
@@ -3626,17 +3621,19 @@
         port_name="",
         port_impedance="50",
         renormalize=False,
         renorm_impedance="50",
         deembed=False,
     ):
         """Create a circuit port from two edges.
-
         The integration line is from edge 2 to edge 1.
 
+        .. deprecated:: 0.6.70
+        Use :func:`circuit_port` method instead.
+
         Parameters
         ----------
         edge_signal : int
             Edge ID of the signal.
         edge_gnd : int
             Edge ID of the ground.
         port_name : str, optional
@@ -3682,20 +3679,24 @@
         >>> hfss.solution_type = "Modal"
         >>> hfss.create_circuit_port_from_edges(first_edge, second_edge, port_name="PortExample",
         ...                                     port_impedance=50.1, renormalize=False,
         ...                                     renorm_impedance="50")
         'PortExample'
 
         """
-
-        edge_list = [edge_signal, edge_gnd]
-        port_name = self._get_unique_source_name(port_name, "Port")
-
-        return self._create_circuit_port(
-            edge_list, port_impedance, port_name, renormalize, deembed, renorm_impedance=renorm_impedance
+        warnings.warn("Use :func:`circuit_port` method instead.", DeprecationWarning)
+        return self.circuit_port(
+            signal=edge_signal,
+            reference=edge_gnd,
+            port_location=0,
+            impedance=port_impedance,
+            name=port_name,
+            renormalize=renormalize,
+            renorm_impedance=renorm_impedance,
+            deembed=deembed,
         )
 
     @pyaedt_function_handler()
     def edit_sources(
         self, excitations, include_port_post_processing=True, max_available_power=None, use_incident_voltage=False
     ):
         """Set up the power loaded for HFSS postprocessing in multiple sources simultaneously.
@@ -5951,14 +5952,15 @@
         create_port_sheet=False,
         port_on_plane=True,
         integration_line=0,
         impedance=50,
         name=None,
         renormalize=True,
         deembed=False,
+        terminals_rename=True,
     ):
         """Create a waveport taking the closest edges of two objects.
 
         Parameters
         ----------
         signal : str, int, list or :class:`pyaedt.modeler.object3d.Object3d` or
          :class:`pyaedt.modeler.elements3d.FacePrimitive`
@@ -5980,14 +5982,16 @@
         name : str, optional
             name of the port. The default is ``None``.
         renormalize : bool, optional
             Whether to renormalize the mode. The default is ``True``.
         deembed : float, optional
             Deembed distance in millimeters. The default is ``0``,
             in which case deembed is disabled.
+        terminals_rename : bool, optional
+            Modify terminals name with the port name plus the terminal number. The default value is ``True``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Port object.
 
         Examples
@@ -6051,14 +6055,15 @@
                     faces[0],
                     reference,
                     name,
                     renorm=renormalize,
                     deembed=deembed,
                     iswaveport=False,
                     impedance=impedance,
+                    terminals_rename=terminals_rename,
                 )
         return False
 
     @pyaedt_function_handler()
     def wave_port(
         self,
         signal,
@@ -6071,14 +6076,15 @@
         impedance=50,
         name=None,
         renormalize=True,
         deembed=0,
         is_microstrip=False,
         vfactor=3,
         hfactor=5,
+        terminals_rename=True,
     ):
         """Create a waveport from a sheet (``start_object``) or taking the closest edges of two objects.
 
         Parameters
         ----------
         signal : int, str, :class:`pyaedt.modeler.object3d.Object3d` or
          :class:`pyaedt.modeler.elements3d.FacePrimitive`
@@ -6111,14 +6117,16 @@
         is_microstrip : bool, optional
             Whether if the wave port will be created and is a microstrip port.
             The default is ``False``.
         vfactor : int, optional
             Port vertical factor. Only valid if ``is_microstrip`` is enabled. The default is ``3``.
         hfactor : int, optional
             Port horizontal factor. Only valid if ``is_microstrip`` is enabled. The default is ``5``.
+        terminals_rename : bool, optional
+            Modify terminals name with the port name plus the terminal number. The default value is ``True``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Port object.
 
         References
@@ -6222,12 +6230,13 @@
                     faces[0],
                     reference,
                     name,
                     renorm=renormalize,
                     deembed=deembed,
                     iswaveport=True,
                     impedance=impedance,
+                    terminals_rename=terminals_rename,
                 )
             else:
                 self.logger.error("Reference conductors are missing.")
                 return False
         return False
```

### Comparing `pyaedt-0.6.70/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.71/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/icepak.py` & `pyaedt-0.6.71/pyaedt/icepak.py`

 * *Files 2% similar despite different names*

```diff
@@ -626,14 +626,17 @@
         surface_heat="0irrad_W_per_m2",
         temperature="AmbientTemp",
         radiate=False,
         source_name=None,
     ):
         """Create a source power for a face.
 
+        .. deprecated:: 0.6.71
+            This method is replaced by `assign_source`.
+
         Parameters
         ----------
         face_id : int or str
             If int, Face ID. If str, object name.
         thermal_dependent_dataset : str, optional
             Name of the dataset if a thermal dependent power source is to be assigned. The default is ``None``.
         input_power : str, float, or int, optional
@@ -3719,7 +3722,136 @@
         setup.auto_update = False
         for arg_name, arg_value in kwargs.items():
             if setup[arg_name] is not None:
                 setup[arg_name] = arg_value
         setup.auto_update = True
         setup.update()
         return setup
+
+    @pyaedt_function_handler()
+    def _parse_variation_data(self, quantity, variation_type, variation_value, function):
+        if variation_type == "Transient" and self.solution_type == "SteadyState":
+            self.logger.error("A transient boundary condition cannot be assigned for a non-transient simulation.")
+            return None
+        if variation_type == "Temp Dep" and function != "Piecewise Linear":
+            self.logger.error("Temperature dependent assignment support only piecewise linear function.")
+            return None
+        out_dict = {"Variation Type": variation_type, "Variation Function": function}
+        if function == "Piecewise Linear":
+            if not isinstance(variation_value, list):
+                variation_value = ["1", "pwl({},Temp)".format(variation_value)]
+            else:
+                variation_value = [variation_value[0], "pwl({},Temp)".format(variation_value[1])]
+            out_dict["Variation Value"] = "[{}]".format(", ".join(['"' + str(i) + '"' for i in variation_value]))
+        else:
+            out_dict["Variation Value"] = "[{}]".format(", ".join([str(i) for i in variation_value]))
+        return {"{} Variation Data".format(quantity): out_dict}
+
+    @pyaedt_function_handler()
+    def assign_source(
+        self,
+        assignment,
+        thermal_condition,
+        assignment_value,
+        boundary_name=None,
+        radiate=False,
+        voltage_current_choice=False,
+        voltage_current_value=None,
+    ):
+        """Create a source power for a face.
+
+        Parameters
+        ----------
+        assignment : int or str
+            If int, Face ID. If str, object name.
+        thermal_condition : str
+            Thermal condition. Accepted values are ``"Total Power"``, ``"Surface Heat"``,
+            ``"Temperature"``.
+        assignment_value : str or dict
+            Value and units of the input power, surface heat or temperature (depending on
+            ``thermal_condition``). A dictionary can be used for temperature dependent or transient
+             assignment. The dictionary should contain three keys: ``"Type"``, ``"Function"`` and
+             ``"Values"``. Accepted ``"Type"`` values are: ``"Temp Dep"`` and ``"Transient"``.
+             Accepted ``"Function"`` are: ``"Linear"``, ``"Power Law"``, ``"Exponential"``,
+             ``"Sinusoidal"``, ``"Square Wave"`` and ``"Piecewise Linear"``. ``"Temp Dep"`` only
+             support the latter. ``"Values"`` contains a list of strings containing the parameters
+            required by the ``"Function"`` selection (e.g. ``"Linear"`` requires two parameters:
+            the value of the variable at t=0 and the slope of the line). The parameters required by
+            each ``Function`` option is in Icepak documentation. The parameters must contain the
+            units where needed.
+        boundary_name : str, optional
+            Name of the source boundary. The default is ``None`` and the boundary name will be
+            generated automatically.
+        radiate : bool, optional
+            Whether to enable radiation. The default is ``False``.
+        voltage_current_choice : str or bool, optional
+            Whether to assign ``"Voltage"`` or ``"Current"`` or none of them. The default is
+            ``False`` (none of them is assigned).
+        voltage_current_value : str or dict, optional
+            Value and units of current or voltage assignment. A dictionary can be used for
+            transient assignment. The dictionary must be structured as described for the
+            ``assignment_value`` argument. The default is ``None``.
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Boundary object when successful or ``None`` when failed.
+
+        References
+        ----------
+
+        >>> oModule.AssignSourceBoundary
+
+        """
+        default_values = {"Total Power": "0W", "Surface Heat": "0irrad_W_per_m2", "Temperature": "AmbientTemp"}
+        if not boundary_name:
+            boundary_name = generate_unique_name("Source")
+        props = {}
+        if isinstance(assignment, int):
+            props["Faces"] = [assignment]
+        elif isinstance(assignment, str):
+            props["Objects"] = [assignment]
+        props["Thermal Condition"] = thermal_condition
+        for quantity, value in default_values.items():
+            if quantity == thermal_condition:
+                if isinstance(assignment_value, dict):
+                    assignment_value = self._parse_variation_data(
+                        quantity,
+                        assignment_value["Type"],
+                        variation_value=assignment_value["Values"],
+                        function=assignment_value["Function"],
+                    )
+                    if assignment_value is None:
+                        return None
+                    props.update(assignment_value)
+                else:
+                    props[quantity] = assignment_value
+            else:
+                props[quantity] = value
+        props["Radiation"] = OrderedDict({"Radiate": radiate})
+        props["Voltage/Current - Enabled"] = bool(voltage_current_choice)
+        default_values = {"Current": "0A", "Voltage": "0V"}
+        props["Voltage/Current Option"] = voltage_current_choice
+        for quantity, value in default_values.items():
+            if voltage_current_choice == quantity:
+                if isinstance(voltage_current_value, dict):
+                    if voltage_current_value["Type"] == "Temp Dep":
+                        self.logger.error("Voltage or Current assignment does not support temperature dependence.")
+                        return None
+                    voltage_current_value = self._parse_variation_data(
+                        quantity,
+                        voltage_current_value["Type"],
+                        variation_value=voltage_current_value["Values"],
+                        function=voltage_current_value["Function"],
+                    )
+                    if voltage_current_value == None:
+                        return None
+                    props.update(voltage_current_value)
+                else:
+                    props[quantity] = voltage_current_value
+            else:
+                props[quantity] = value
+
+        bound = BoundaryObject(self, boundary_name, props, "SourceIcepak")
+        if bound.create():
+            self.boundaries.append(bound)
+            return bound
```

### Comparing `pyaedt-0.6.70/pyaedt/maxwell.py` & `pyaedt-0.6.71/pyaedt/maxwell.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,24 +53,31 @@
     def design_file(self):
         """Design file."""
         design_file = os.path.join(self.working_directory, "design_data.json")
         return design_file
 
     @pyaedt_function_handler()
     def change_symmetry_multiplier(self, value=1):
-        """Set the Design Symmetry Multiplier to a specified value.
+        """Set the design symmetry multiplier to a specified value.
+        The symmetry multiplier is automatically applied to all input quantities.
 
         Parameters
         ----------
         value : int, optional
             Value to use as the Design Symmetry Multiplier coefficient. The default value is ``1``.
 
         Returns
         -------
         bool
+            ``True`` when successful, ``False`` when failed.
+
+        References
+        ----------
+
+        >>> oDesign.SetDesignSettings
         """
         return self.change_design_settings({"Multiplier": value})
 
     @pyaedt_function_handler()
     def change_inductance_computation(self, compute_transient_inductance=True, incremental_matrix=False):
         """Enable the inductance computation for the transient analysis and set the incremental matrix.
 
@@ -97,15 +104,17 @@
             {"ComputeTransientInductance": compute_transient_inductance, "ComputeIncrementalMatrix": incremental_matrix}
         )
 
     @pyaedt_function_handler()
     def set_core_losses(self, objects, value=True):
         """Whether to enable core losses for a set of objects.
 
-        This method works only on ``EddyCurrent`` and ``Transient`` solutions.
+        For``EddyCurrent`` and ``Transient`` solver design, core losses calulcations
+        may be included in the simulation on any object that has a corresponding
+        core loss definition (with core loss coefficient settings) in the material library.
 
         Parameters
         ----------
         objects : list, str
             List of object to apply core losses to.
         value : bool, optional
             Whether to enable core losses for the given list. The default is
@@ -146,14 +155,19 @@
         turns=None,
         return_path=None,
         group_sources=None,
         branches=None,
     ):
         """Assign a matrix to the selection.
 
+        Matrix assignment can be calculated based upon the solver type.
+        For 2D/3D solvers the available solution types are: ``Magnetostatic``,
+        ``Electrostatic``, ``Eddy Current``, ``DC Conduction`` and ``AC Conduction``.
+
+
         Parameters
         ----------
         sources : list, str
             List of sources to assign a matrix to.
         matrix_name : str, optional
             Name of the matrix. The default is ``None``.
         turns : list, int, optional
@@ -317,98 +331,102 @@
             return False
 
     @pyaedt_function_handler()
     def setup_ctrlprog(
         self, setupname, file_str=None, keep_modifications=False, python_interpreter=None, aedt_lib_dir=None
     ):
         """Configure the transient design setup to run a specific control program.
+        The control program is executed from a temporary directory that Maxwell creates for every setup run.
 
         Parameters
         ----------
         setupname : str
             Name of the setup.
+            It will become the name of the Python file.
         file_str : str, optional
             Name of the file. The default value is ``None``.
         keep_modifications : bool, optional
             Whether to save the changes. The default value is ``False``.
         python_interpreter : str, optional
              Python interpreter to use. The default value is ``None``.
         aedt_lib_dir : str, optional
              Full path to the ``pyaedt`` directory. The default value is ``None``.
 
         Returns
         -------
         bool
             ``True`` when successful and ``False`` when failed.
         """
+        if self.solution_type not in ["Transient"]:
+            self.logger.error("Control Program is only available in Maxwell 2D and 3D Transient solutions.")
+            return False
 
         self._py_file = setupname + ".py"
-        ctl_path = self.working_directory
-        ctl_file_compute = os.path.join(ctl_path, self._py_file)
-        ctl_file = os.path.join(self.working_directory, self._py_file)
+        ctl_file_path = os.path.join(self.working_directory, self._py_file)
 
         if aedt_lib_dir:
             source_dir = aedt_lib_dir
         else:
             source_dir = self.pyaedt_dir
 
-        if os.path.exists(ctl_file) and keep_modifications:
-            with open(ctl_file, "r") as fi:
+        if os.path.exists(ctl_file_path) and keep_modifications:
+            with open(ctl_file_path, "r") as fi:
                 existing_data = fi.readlines()
-            with open(ctl_file, "w") as fo:
+            with open(ctl_file_path, "w") as fo:
                 first_line = True
                 for line in existing_data:
                     if first_line:
                         first_line = False
                         if python_interpreter:
                             fo.write("#!{0}\n".format(python_interpreter))
                     if line.startswith("work_dir"):
-                        fo.write("work_dir = r'{0}'\n".format(ctl_path))
+                        fo.write("work_dir = r'{0}'\n".format(self.working_directory))
                     elif line.startswith("lib_dir"):
                         fo.write("lib_dir = r'{0}'\n".format(source_dir))
                     else:
                         fo.write(line)
         else:
             if file_str is not None:
-                with io.open(ctl_file, "w", newline="\n") as fo:
+                with io.open(ctl_file_path, "w", newline="\n") as fo:
                     fo.write(file_str)
-                assert os.path.exists(ctl_file), "Control program file could not be created."
+                assert os.path.exists(ctl_file_path), "Control program file could not be created."
 
         self.oanalysis.EditSetup(
             setupname,
             [
                 "NAME:" + setupname,
                 "Enabled:=",
                 True,
                 "UseControlProgram:=",
                 True,
                 "ControlProgramName:=",
-                ctl_file_compute,
+                ctl_file_path,
                 "ControlProgramArg:=",
                 "",
                 "CallCtrlProgAfterLastStep:=",
                 True,
             ],
         )
-
         return True
 
-    # Set eddy effects
     @pyaedt_function_handler()
     def eddy_effects_on(self, object_list, activate_eddy_effects=True, activate_displacement_current=True):
-        """Assign eddy effects on objects.
+        """Assign eddy effects on a list of objects.
+
+        For Eddy Current solvers only, you must specify the displacement current on the model objects.
 
         Parameters
         ----------
         object_list : list
             List of objects.
         activate_eddy_effects : bool, optional
             Whether to activate eddy effects. The default is ``True``.
         activate_displacement_current : bool, optional
             Whether to activate the displacement current. The default is ``True``.
+            Valid only for Eddy Current solvers.
 
         Returns
         -------
         bool
             ``True`` when successful and ``False`` when failed.
 
         References
@@ -487,25 +505,24 @@
                             "NAME:Data",
                             "Object Name:=",
                             obj,
                             "Eddy Effect:=",
                             bool(self.oboundary.GetEddyEffect(obj)),
                         ]
                     )
-
         self.oboundary.SetEddyEffect(["NAME:Eddy Effect Setting", EddyVector])
         return True
 
     @pyaedt_function_handler()
     def setup_y_connection(self, windings_name=None):
         """Setup the Y connection.
 
         Parameters
         ----------
-        winding_name : list, optional
+        windings_name : list, optional
             List of windings. For example, ``["PhaseA", "PhaseB", "PhaseC"]``.
             The default value is ``None``, in which case the design has no Y connection.
 
         Returns
         -------
         bool
             ``True`` when successful and ``False`` when failed.
@@ -522,20 +539,21 @@
 
         >>> from pyaedt import Maxwell2d
         >>> aedtapp = Maxwell2d("Motor_EM_R2019R3.aedt")
         >>> aedtapp.set_active_design("Basis_Model_For_Test")
         >>> aedtapp.setup_y_connection(["PhaseA", "PhaseB", "PhaseC"])
         """
 
+        if self.solution_type not in ["Transient"]:
+            self.logger.error("Y connections only available for Transient solutions.")
+            return False
+
         if windings_name:
-            connection = ["NAME:YConnection"]
-            connection.append("Windings:=")
-            connection.append(",".join(windings_name))
-            windings = ["NAME:YConnection"]
-            windings.append(connection)
+            connection = ["NAME:YConnection", "Windings:=", ",".join(windings_name)]
+            windings = ["NAME:YConnection", connection]
             self.oboundary.SetupYConnection(windings)
         else:
             self.oboundary.SetupYConnection()
         return True
 
     @pyaedt_function_handler()
     def assign_current(self, object_list, amplitude=1, phase="0deg", solid=True, swap_direction=False, name=None):
@@ -544,21 +562,26 @@
         Parameters
         ----------
         object_list : list
             List of objects to assign the current source to.
         amplitude : float or str, optional
             Current amplitude. The default is ``1A``.
         phase : str, optional
+            Current phase.
             The default is ``"0deg"``.
         solid : bool, optional
-            The default is ``True``.
+            Specifies the type of conductor, which can be solid or stranded.
+            The default is ``True``, which means the conductor is solid``.
+            When ``False``, it means the conductor is stranded.
         swap_direction : bool, optional
-            The default is ``False``.
+            Reference direction.
+            The default is ``False`` which means that current is flowing inside the object.
         name : str, optional
-            The default is ``None``.
+            Name of the current excitation.
+            The default is ``None`` in which case a generic name will be given.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object.
 
         References
@@ -636,14 +659,16 @@
         mass=1,
         damping=0,
         load_force=0,
         motion_name=None,
     ):
         """Assign a translation motion to an object container.
 
+        For both rotational and translational problems, the band objects must always enclose all the moving objects.
+
         Parameters
         ----------
         band_object : str
             Object container.
         coordinate_system : str, optional
             Coordinate system name. The default is ``"Global"``.
         axis : str or int, optional
@@ -659,26 +684,27 @@
         negative_limit : float or str, optional
             Negative limit of the movement. The default is ``0``. If a float
             value is used, the default modeler units are applied.
         positive_limit : float or str, optional
             Positive limit of the movement. The default is ``0``. If a float
             value is used, the default modeler units are applied.
         velocity : float or str, optional
-            Movement velocity. The default is ``0``. If a float value
-            is used, "m_per_sec" units are applied.
+            Initial velocity.
+            The default is ``0``. If a float value is used, "m_per_sec" units are applied.
         mechanical_transient : bool, optional
             Whether to consider the mechanical movement. The default is ``False``.
         mass : float or str, optional
             Mechanical mass. The default is ``1``. If a float value is used, "Kg" units
             are applied.
         damping : float, optional
             Damping factor. The default is ``0``.
         load_force : float or str, optional
-            Load force. The default is ``0``. If a float value is used, "newton"
-            units are applied.
+            Load force is positive if it's applied in the same direction as the moving vector and negative
+            in the opposite direction.
+            The default is ``0``. If a float value is used, "newton" units are applied.
         motion_name : str, optional
             Motion name. The default is ``None``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object.
@@ -733,14 +759,16 @@
         angular_velocity="0rpm",
         inertia="1",
         damping=0,
         load_torque="0newton",
     ):
         """Assign a rotation motion to an object container.
 
+        For both rotational and translational problems, the band objects must always enclose all the moving objects.
+
         Parameters
         ----------
         band_object : str,
             Object container.
         coordinate_system : str, optional
             Coordinate system name. The default is ``"Global"``.
         axis : str or int, optional
@@ -767,16 +795,16 @@
         mechanical_transient : bool, optional
             Whether to consider mechanical movement. The default is ``False``.
         inertia : float, optional
             Mechanical inertia. The default is ``1``.
         damping : float, optional
             Damping factor. The default is ``0``.
         load_torque : float or str, optional
-            Load force. The default is ``"0newton"``. If a float value is used,
-            "NewtonMeter" units are applied.
+            Load torque sign is determined based on the moving vector, using the right-hand rule.
+            The default is ``"0NewtonMeter"``. If a float value is used "NewtonMeter" units are applied.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object.
 
         References
@@ -826,42 +854,43 @@
         name : str, optional
             Name of the boundary. The default is ``None``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object.
+            ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.AssignVoltage
         """
         if isinstance(amplitude, (int, float)):
             amplitude = str(amplitude) + "mV"
 
         if not name:
             name = generate_unique_name("Voltage")
         face_list = self.modeler.convert_to_selections(face_list, True)
 
-        # if type(face_list) is not list and type(face_list) is not tuple:
-        #     face_list = [face_list]
         if self.design_type == "Maxwell 2D":
             props = OrderedDict({"Objects": face_list, "Value": amplitude})
         else:
             props = OrderedDict({"Faces": face_list, "Voltage": amplitude})
         bound = BoundaryObject(self, name, props, "Voltage")
         if bound.create():
             self.boundaries.append(bound)
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_voltage_drop(self, face_list, amplitude=1, swap_direction=False, name=None):
-        """Assign a voltage drop to a list of faces.
+        """Assign a voltage drop across a list of faces to a specific value.
+
+        The voltage drop applies only to sheet objects.
 
         Parameters
         ----------
         face_list : list
             List of faces to assign a voltage drop to.
         amplitude : float, optional
             Voltage amplitude in mV. The default is ``1``.
@@ -870,14 +899,15 @@
         name : str, optional
             Name of the boundary. The default is ``None``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object.
+            ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.AssignVoltageDrop
         """
         if isinstance(amplitude, (int, float)):
@@ -933,14 +963,15 @@
         name : str, optional
             Name of the boundary. The default is ``None``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Bounding object for the winding, otherwise only the bounding object.
+            ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.AssignWindingGroup
         """
 
@@ -1017,16 +1048,17 @@
         polarity : str, optional
             Type of the polarity. The default is ``"Positive"``.
         name : str, optional
             The default is ``None``.
 
         Returns
         -------
-        CoilObject
-            Coil object.
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Bounding object for the winding, otherwise only the bounding object.
+            ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.AssignCoil
         """
         if polarity.lower() == "positive":
@@ -1069,14 +1101,20 @@
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_force(self, input_object, reference_cs="Global", is_virtual=True, force_name=None):
         """Assign a force to one or more objects.
 
+        Force assignment can be calculated based upon the solver type.
+        For 3D solvers the available solution types are: ``Magnetostatic``,
+        ``Electrostatic``, ``Eddy Current``, ``Transient`` and ``Electric Transient``.
+        For 2D solvers the available solution types are: ``Magnetostatic``,
+        ``Electrostatic``, ``Eddy Current`` and ``Transient``.
+
         Parameters
         ----------
         input_object : str, list
             One or more objects to assign the force to.
         reference_cs : str, optional
             Name of the reference coordinate system. The default is ``"Global"``.
         is_virtual : bool, optional
@@ -1127,14 +1165,20 @@
 
     @pyaedt_function_handler()
     def assign_torque(
         self, input_object, reference_cs="Global", is_positive=True, is_virtual=True, axis="Z", torque_name=None
     ):
         """Assign a torque to one or more objects.
 
+        Torque assignment can be calculated based upon the solver type.
+        For 3D solvers the available solution types are: ``Magnetostatic``,
+        ``Electrostatic``, ``Eddy Current``, ``Transient`` and ``Electric Transient``.
+        For 2D solvers the available solution types are: ``Magnetostatic``,
+        ``Electrostatic``, ``Eddy Current`` and ``Transient``.
+
         Parameters
         ----------
         input_object : str or list
            One or more objects to assign the torque to.
         reference_cs : str, optional
             Name of the reference coordinate system. The default is ``"Global"``.
         is_positive : bool, optional
@@ -1190,19 +1234,22 @@
                 return bound
         else:
             self.logger.error("Solution Type has not Matrix Parameter")
             return False
 
     @pyaedt_function_handler()
     def solve_inside(self, name, activate=True):
-        """Solve inside.
+        """Solve inside to generate a solution inside an object.
+
+        With this method, Maxwell will create a mesh inside the object and generate the solution from the mesh.
 
         Parameters
         ----------
         name : str
+            Name of the object to generate the solution into.
 
         activate : bool, optional
             The default value is ``True``.
 
         Returns
         -------
         bool
@@ -1214,26 +1261,31 @@
         >>> oEditor.ChangeProperty
         """
         self.modeler[name].solve_inside = activate
         return True
 
     @pyaedt_function_handler()
     def analyze_from_zero(self):
-        """Analyze from zero.
+        """Force the next solve to start from time 0 for a given setup.
+
+        This method applies only to the Transient solution type.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.ResetSetupToTimeZero
         """
+        if self.solution_type != "Transient":
+            self.logger.error("This methods work only with Maxwell Transient Analysis.")
+            return False
         self.oanalysis.ResetSetupToTimeZero(self._setup)
         self.analyze()
         return True
 
     @pyaedt_function_handler()
     def set_initial_angle(self, motion_setup, val):
         """Set the initial angle.
@@ -1267,14 +1319,17 @@
         )
         return True
 
     @pyaedt_function_handler()
     def assign_symmetry(self, entity_list, symmetry_name=None, is_odd=True):
         """Assign symmetry boundary.
 
+        This boundary condition defines a plane of geometric or magnetic symmetry in a structure.
+        Assign it only to the outer surfaces of the problem region.
+
         Parameters
         ----------
         entity_list : list
             List IDs or :class:`pyaedt.modeler.Object3d.EdgePrimitive` or
             :class:`pyaedt.modeler.Object3d.FacePrimitive`.
         symmetry_name : str, optional
             Name of the symmetry.
@@ -1327,14 +1382,16 @@
         current_density_z="0",
         current_density_2d="0",
         coordinate_system_name="Global",
         coordinate_system_cartesian="Cartesian",
     ):
         """Assign current density to a single or list of entities.
 
+        This method specifies the x-, y-, and z-components of the current density in a conduction path.
+
         Parameters
         ----------
         entities : list
             Objects to assign the current to.
         current_density_name : str, optional
             Current density name.
             If no name is provided a random name is generated.
@@ -1461,28 +1518,34 @@
         calculate_force="Harmonic",
     ):
         """Set the Harmonic Force for Transient Analysis.
 
         Parameters
         ----------
         objects : list
-            Object list to enable force computation.
+            List of object names for force calculations.
         force_type : int, optional
-            Force Type. `0` for Objects, `1` for Surface, `2` for volumetric.
+            Force Type. ``0`` for Objects, ``1`` for Surface, ``2`` for volumetric.
         window_function : str, optional
-            Windowing function. Default is `"Rectangular"`.
+            Windowing function. Default is ``"Rectangular"``.
+            Available options are: ``"Rectangular"``, ``"Tri"``, ``"Van Hann"``, ``"Hamming"``,
+            ``"Blackman"``, ``"Lanczos"``, ``"Welch"``.
         use_number_of_last_cycles : bool, optional
-            Either to use or not the last cycle. Default is `True`.
+            Use number Of last cycles for force calculations. Default is ``True``.
         last_cycles_number : int, optional
-            Defines the number of cycles to compute if `use_number_of_last_cycle` is `True`.
+            Defines the number of cycles to compute if `use_number_of_last_cycle` is ``True``.
         calculate_force : sr, optional
-            Either `"Harmonic"` or `"Transient"`. Default is `"Harmonic"`.
+            How to calculate force. The default is ``"Harmonic"``.
+            Options are ``"Harmonic"`` and ``"Transient"``.
+
 
         Returns
         -------
+        bool
+            ``True`` when successful, ``False`` when failed.
 
         """
         if self.solution_type != "Transient":
             self.logger.error("This methods work only with Maxwell Transient Analysis.")
             return False
         objects = self.modeler.convert_to_selections(objects, True)
         self.odesign.EnableHarmonicForceCalculation(
@@ -1518,26 +1581,26 @@
         self,
         output_directory=None,
         setup_name=None,
         start_frequency=None,
         stop_frequency=None,
         number_of_frequency=None,
     ):
-        """Export Element Based Harmonic Forces csv to file.
+        """Export an element-based harmonic force data to a .csv file.
 
         Parameters
         ----------
         output_directory : str, optional
-            Path to export. If ``None`` pyaedt working dir will be used.
+            The path for the output directory. If ``None`` pyaedt working dir will be used.
         setup_name : str, optional
-            Setup name. If ``None`` pyaedt will use nominal setup.
+            Name of the solution setup. If ``None``, the nominal setup is used.
         start_frequency : float, optional
             When a float is entered the Start-Stop Frequency approach is used.
         stop_frequency : float, optional
-            A float must be entered when the Start-Stop Frequency approach is used.
+            When a float is entered, the Start-Stop Frequency approach is used.
         number_of_frequency : int, optional
             When a number is entered, the number of frequencies approach is used.
 
         Returns
         -------
         str
             Path to the export directory.
@@ -1590,15 +1653,15 @@
         remove_blends=True,
         hole_radius_tolerance=1,
         chamfer_width_tolerance=1,
         blend_radius_tolerance=1,
         allowable_surface_area_change=5,
         allowable_volume_change=5,
     ):
-        """Analyze healing objects options.
+        """Repair invalid geometry entities for the selected objects within the specified tolerance settings.
 
         Parameters
         ----------
         input_objects_list : str
             List of object names to analyze.
         auto_heal : bool, optional
             Auto heal option. Default value is ``True``.
@@ -1747,20 +1810,16 @@
             "BlendRadiusTol:=",
             blend_radius_tolerance,
             "AllowableSurfaceAreaChange:=",
             allowable_surface_area_change,
             "AllowableVolumeChange:=",
             allowable_volume_change,
         ]
-        try:
-            self.oeditor.HealObject(selections_args, healing_parameters)
-            return True
-        except:
-            self.logger.error("Heal objects failed.")
-            return False
+        self.oeditor.HealObject(selections_args, healing_parameters)
+        return True
 
     @pyaedt_function_handler()
     def simplify_objects(
         self,
         input_objects_list,
         simplify_type="Polygon Fit",
         extrusion_axis="Auto",
@@ -1769,15 +1828,15 @@
         separate_bodies=True,
         clone_body=True,
         generate_primitive_history=False,
         interior_points_on_arc=5,
         length_threshold_percentage=25,
         create_group_for_new_objects=False,
     ):
-        """Analyze healing objects options.
+        """Simplify command to converts complex objects into simpler primitives which are easy to mesh and solve.
 
         Parameters
         ----------
         input_objects_list : str
             List of object names to simplify.
         simplify_type : str, optional
             Simplify type. Default value is ``Polygon Fit``.
@@ -1908,19 +1967,16 @@
                 source_type = comp_instance.GetPropHost().GetText("Type")
                 if source_type == "TIME":
                     sources_type_array.append(1)
                 elif source_type == "POS":
                     sources_type_array.append(2)
                 elif source_type == "SPEED":
                     sources_type_array.append(3)
-        try:
-            self.oboundary.EditExternalCircuit(netlist_file_path, sources_array, sources_type_array, [], [])
-            return True
-        except:
-            return False
+        self.oboundary.EditExternalCircuit(netlist_file_path, sources_array, sources_type_array, [], [])
+        return True
 
     @pyaedt_function_handler()
     def create_setup(self, setupname="MySetupAuto", setuptype=None, **kwargs):
         """Create an analysis setup for Maxwell 3D or 2D.
         Optional arguments are passed along with ``setuptype`` and ``setupname``.  Keyword
         names correspond to the ``setuptype``
         corresponding to the native AEDT API.  The list of
@@ -2093,14 +2149,17 @@
         )
         Maxwell.__init__(self)
 
     @pyaedt_function_handler()
     def assign_insulating(self, geometry_selection, insulation_name=None):
         """Create an insulating boundary condition.
 
+        This boundary condition is used to model very thin sheets of perfectly insulating material between
+        touching conductors. Current cannot cross an insulating boundary.
+
         Parameters
         ----------
         geometry_selection : str or int
             Objects or faces to apply the insulating boundary to.
         insulation_name : str, optional
             Name of the insulation. The default is ``None`` in which case a unique name is chosen.
 
@@ -2153,15 +2212,18 @@
         geometry_selection,
         material_name=None,
         permeability=0.0,
         conductivity=None,
         non_linear_permeability=False,
         impedance_name=None,
     ):
-        """Create an impedance boundary condition.
+        """Create an impedance boundary condition for Transient or Eddy Current solvers.
+
+        This boundary condition is used to simulate the effect of induced currents in a conductor without
+        explicitly computing them.
 
         Parameters
         ----------
         geometry_selection : str
             Objects to apply the impedance boundary to.
         material_name : str, optional
             If it is different from ``None``, then material properties values will be extracted from
@@ -2222,15 +2284,15 @@
                 props["Conductivity"] = conductivity
 
             return self._create_boundary(impedance_name, props, "Impedance")
         return False
 
     @pyaedt_function_handler()
     def assign_current_density_terminal(self, entities, current_density_name=None):
-        """Assign current density terminal to a single or list of entities.
+        """Assign current density terminal to a single or list of entities for an Eddy Current or Magnetostatic solver.
 
         Parameters
         ----------
         entities : list
             Objects to assign the current to.
         current_density_name : str, optional
             Current density name.
@@ -2335,15 +2397,15 @@
         u_vector_origin_coordinates_slave,
         u_vector_pos_coordinates_slave,
         reverse_master=False,
         reverse_slave=False,
         same_as_master=True,
         bound_name=None,
     ):
-        """Assign master and slave boundary conditions to two faces of the same object.
+        """Assign dependent and independent boundary conditions to two faces of the same object.
 
         Parameters
         ----------
         master_entity : int
             ID of the master entity.
         slave_entity : int
             ID of the slave entity.
@@ -2364,15 +2426,15 @@
         bound_name : str, optional
             Name of the master boundary. The default is ``None``, in which case the default name
             is used. The name of the slave boundary has a ``_dep`` suffix.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`, :class:`pyaedt.modules.Boundary.BoundaryObject`
-            Master and slave objects.
+            Master and slave objects. If the method fails to execute it returns ``False``.
 
         References
         ----------
 
         >>> oModule.AssignIndependent
         >>> oModule.AssignDependent
         """
@@ -2684,15 +2746,15 @@
         bound_name : str, optional
             Name of the boundary. The default is ``None``, in which
             case the default name is used.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
-            Boundary object.
+            Boundary object. If the method fails to execute it returns ``False``.
 
         References
         ----------
 
         >>> oModule.AssignBalloon
         """
         edge_list = self.modeler.convert_to_selections(edge_list, True)
@@ -2706,30 +2768,32 @@
         if bound.create():
             self.boundaries.append(bound)
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_vector_potential(self, input_edge, vectorvalue=0, bound_name=None):
-        """Assign a vector to a list of edges.
+        """Assign a vector potential boundary condition to specified edges.
+
+        This method is valid for Maxwell 2D Eddy Current, Magnetostatic, and Transient solvers.
 
         Parameters
         ----------
         input_edge : list
             List of edge names or edge IDs to assign a vector to.
         vectorvalue : float, optional
             Value of the vector. The default is ``0``.
         bound_name : str, optional
             Name of the boundary. The default is ``None``, in which
             case the default name is used.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
-            Vector Potential Object.
+            Vector Potential Object. ``False`` if it fails.
 
         References
         ----------
 
         >>> oModule.AssignVectorPotential
         """
         input_edge = self.modeler.convert_to_selections(input_edge, True)
@@ -2747,15 +2811,15 @@
             return bound
         return False
 
     @pyaedt_function_handler()
     def assign_master_slave(
         self, master_edge, slave_edge, reverse_master=False, reverse_slave=False, same_as_master=True, bound_name=None
     ):
-        """Assign master and slave boundary conditions to two edges of the same object.
+        """Assign dependent and independent boundary conditions to two edges of the same object.
 
         Parameters
         ----------
         master_edge : int
             ID of the master edge.
         slave_edge : int
             ID of the slave edge.
@@ -2768,15 +2832,15 @@
         bound_name : str, optional
             Name of the master boundary. The default is ``None``, in which case the default name
             is used. The name of the slave boundary has a ``_dep`` suffix.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`, :class:`pyaedt.modules.Boundary.BoundaryObject`
-            Master and slave objects.
+            Master and slave objects. If the method fails to execute it returns ``False``.
 
         References
         ----------
         >>> oModule.AssignIndependent
         >>> oModule.AssignDependent
         """
         master_edge = self.modeler.convert_to_selections(master_edge, True)
@@ -2825,15 +2889,15 @@
         bound_name : str, optional
             Name of the end connection boundary. The default is ``None``, in which case the
             default name is used.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
-            New created object.
+            Newly created object. ``False`` if it fails.
 
         References
         ----------
 
         >>> oModule.AssignEndConnection
         """
         if self.solution_type not in ["EddyCurrent", "Transient"]:
```

### Comparing `pyaedt-0.6.70/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.71/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/mechanical.py` & `pyaedt-0.6.71/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/Console.py_build` & `pyaedt-0.6.71/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.71/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.71/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.71/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.71/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.71/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/amat.xml` & `pyaedt-0.6.71/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/console_setup.py` & `pyaedt-0.6.71/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.71/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.71/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.71/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.71/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/misc.py` & `pyaedt-0.6.71/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.71/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.71/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.71/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.71/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.71/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.71/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/misc/template.acf` & `pyaedt-0.6.71/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.71/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.71/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.71/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.71/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.71/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.71/pyaedt/modeler/cad/Modeler.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.71/pyaedt/modeler/cad/Primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1454,14 +1454,18 @@
             if obj_name not in self._object_names_to_ids:
                 self._create_object(obj_name)
                 added_objects.append(obj_name)
         for obj_name in self.unclassified_names:
             if obj_name not in self._object_names_to_ids:
                 self._create_object(obj_name)
                 added_objects.append(obj_name)
+        for obj_name in self.point_names:
+            if obj_name not in self.points.keys():
+                self._create_object(obj_name)
+                added_objects.append(obj_name)
         return added_objects
 
     @pyaedt_function_handler()
     def add_new_user_defined_component(self):
         """Add 3D components and user-defined models that have been created in the modeler by
         previous operations.
 
@@ -3049,21 +3053,24 @@
         arg_str += ["XSectionNumSegments:=", "{}".format(num_seg)]
         arg_str += ["XSectionBendType:=", section_bend]
 
         return arg_str
 
     @pyaedt_function_handler()
     def _arg_with_dim(self, value, units=None):
-        if isinstance(value, str):
-            val = value
+        if units is None:
+            units = self.model_units
+        if type(value) is str:
+            try:
+                float(value)
+                val = "{0}{1}".format(value, units)
+            except:
+                val = value
         else:
-            if units is None:
-                units = self.model_units
             val = "{0}{1}".format(value, units)
-
         return val
 
     @pyaedt_function_handler()
     def _pos_with_arg(self, pos, units=None):
         xpos = self._arg_with_dim(pos[0], units)
         if len(pos) < 2:
             ypos = self._arg_with_dim(0, units)
```

### Comparing `pyaedt-0.6.70/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.71/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.71/pyaedt/modeler/cad/Primitives3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.71/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.71/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.71/pyaedt/modeler/cad/object3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,16 @@
         ----------
 
         >>> oEditor.GetModelBoundingBox
 
         """
         if self.object_type == "Unclassified":
             return [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
+        if settings.aedt_version >= "2023.2":
+            return [float(i) for i in self._oeditor.GetObjectBoundingBox(self.name)]
         if not settings.disable_bounding_box_sat:
             bounding = self._bounding_box_sat()
             if bounding:
                 return bounding
             else:
                 return self._bounding_box_unmodel()
         else:
```

### Comparing `pyaedt-0.6.70/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.71/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     @property
     def model_units(self):
         """Model units."""
         return self.modeler.model_units
 
     @property
     def o_model_manager(self):
-        """Aedt Model Manager"""
+        """Aedt Model Manager."""
         return self.modeler.o_model_manager
 
     @property
     def o_definition_manager(self):
         """Aedt Definition Manager.
 
         References
@@ -208,22 +208,18 @@
         # Connect the radio and antenna.
         if rad_update and ant_update:
             ant_update.move_and_connect_to(rad_update)
         return rad_update, ant_update
 
     @pyaedt_function_handler()
     def get_radios(self):
-        """Return a dict of all the radios in the design.
+        """Get all radios in the design.
 
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
+        Returns
+        -------
         Dict : radio_name : EmitRadioComponents
             Dict of all the radio_name and EmitRadioComponents in the
             design.
         """
         return {k: v for k, v in self.components.items() if v.get_type() == "RadioNode"}
 
     @pyaedt_function_handler()
@@ -235,15 +231,15 @@
                 o = EmitComponent.create(self, comp_name)
                 o_update = self.update_object_properties(o)
                 self.components[comp_name] = o_update
         return len(self.components)
 
     @pyaedt_function_handler()
     def get_obj_id(self, object_name):
-        """
+        """Get object ID.
 
         Parameters
         ----------
         object_name : str
             Name of the object.
 
         Returns
```

### Comparing `pyaedt-0.6.70/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1751,27 +1751,21 @@
         arg.append(arg1)
 
         self._app._oproject.ChangeProperty(arg)
         return True
 
     @pyaedt_function_handler()
     def refresh_dynamic_link(self, component_name):
-        """Refresh a dynamic link component.  This method is adapted from the native API.
-        ```
-            oDefinitionManager = oProject.GetDefinitionManager()
-            oComponentManager = oDefinitionManager.GetManager("Component")
-            oComponentManager.UpdateDynamicLink("TeeModel_L1")
-        ```
+        """Refresh a dynamic link component.
 
         Parameters
         ----------
         component_name : str
             Name of the dynamic link component.
 
-
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
```

### Comparing `pyaedt-0.6.70/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.71/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,14 +305,16 @@
         if ret1 and ret2:
             return True
         else:
             return False
 
 
 class ComponentParameters(dict):
+    """Manages component parameters."""
+
     def __setitem__(self, key, value):
         try:
             self._component._oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
                         "NAME:" + self._tab,
@@ -328,14 +330,16 @@
     def __init__(self, component, tab, *args, **kw):
         dict.__init__(self, *args, **kw)
         self._component = component
         self._tab = tab
 
 
 class ModelParameters(object):
+    """Manages model parameters."""
+
     def update(self):
         """Update the model properties.
 
         Returns
         -------
         bool
         """
```

### Comparing `pyaedt-0.6.70/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.71/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.71/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.71/pyaedt/modeler/modeler3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.71/pyaedt/modeler/modelerpcb.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,24 @@
         Primitives3DLayout.__init__(self, app)
         self._primitives = self
         self.logger.info("Primitives loaded.")
         self.o_def_manager = self._app.odefinition_manager
         self.rigid_flex = None
 
     @property
+    def stackup(self):
+        """Get the Stackup class and its methods.
+
+        Returns
+        -------
+        :class:`pyaedt.modules.LayerStackup.Layers`
+        """
+        return self.layers
+
+    @property
     def oeditor(self):
         """Oeditor Module.
 
         References
         ----------
 
         >>> oEditor = oDesign.SetActiveEditor("Layout")"""
@@ -179,21 +189,24 @@
 
         >>> oEditor.GetModelBoundingBox
         """
         return self.oeditor.GetModelBoundingBox()
 
     @pyaedt_function_handler()
     def _arg_with_dim(self, value, units=None):
-        if isinstance(value, str):
-            val = value
+        if units is None:
+            units = self.model_units
+        if type(value) is str:
+            try:
+                float(value)
+                val = "{0}{1}".format(value, units)
+            except:
+                val = value
         else:
-            if units is None:
-                units = self.model_units
             val = "{0}{1}".format(value, units)
-
         return val
 
     def _pos_with_arg(self, pos, units=None):
         xpos = self._arg_with_dim(pos[0], units)
         if len(pos) < 2:
             ypos = self._arg_with_dim(0, units)
         else:
@@ -252,26 +265,37 @@
                     [
                         "NAME:" + property_tab,
                         ["NAME:PropServers", property_object],
                         ["NAME:ChangedProps", ["NAME:" + property_name, "Value:=", property_value]],
                     ],
                 ]
             )
-        elif isinstance(property_value, (str, float, int)):
+        elif isinstance(property_value, (float, int)):
             xpos = self._arg_with_dim(property_value, self.model_units)
             self.oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
                         "NAME:" + property_tab,
                         ["NAME:PropServers", property_object],
                         ["NAME:ChangedProps", ["NAME:" + property_name, "Value:=", xpos]],
                     ],
                 ]
             )
+        elif isinstance(property_value, str):
+            self.oeditor.ChangeProperty(
+                [
+                    "NAME:AllTabs",
+                    [
+                        "NAME:" + property_tab,
+                        ["NAME:PropServers", property_object],
+                        ["NAME:ChangedProps", ["NAME:" + property_name, "Value:=", property_value]],
+                    ],
+                ]
+            )
         else:
             self.logger.error("Wrong Property Value")
             return False
         self.logger.info("Property {} Changed correctly.".format(property_name))
         return True
 
     @pyaedt_function_handler()
@@ -308,22 +332,22 @@
                     break
             except:
                 continue
         if not comp_name:
             return False
         comp = ComponentsSubCircuit3DLayout(self, comp_name)
         self.components_3d[comp_name] = comp
-        self.change_property(property_object=comp_name, property_name="3D Placement", property_value=True)
-        self.change_property(property_object=comp_name, property_name="Local Origin", property_value=[0.0, 0.0, 0.0])
+        comp.is_3d_placement = True
+        comp.local_origin = [0.0, 0.0, 0.0]
         pos_x = self._arg_with_dim(pos_x)
         pos_y = self._arg_with_dim(pos_y)
         pos_z = self._arg_with_dim(pos_z)
         rotation = self._arg_with_dim(rotation, "deg")
-        self.change_property(property_object=comp_name, property_name="Location", property_value=[pos_x, pos_y, pos_z])
-        self.change_property(property_object=comp_name, property_name="Rotation Angle", property_value=rotation)
+        comp.angle = rotation
+        comp.location = [pos_x, pos_y, pos_z]
         return comp
 
     @pyaedt_function_handler()
     def change_clip_plane_position(self, clip_name, position):
         """Change the clip plane position.
 
         Parameters
@@ -907,26 +931,34 @@
         ]
         args = ["NAME:ModelChanges", ["NAME:UpdateModel0", ["NAME:ComponentNames", component_name], "Prop:=", args2]]
         self.oeditor.UpdateModels(args)
         self.logger.info("Spice Model Correctly assigned to {}.".format(component_name))
         return True
 
     @pyaedt_function_handler()
-    def clip_plane(self, name=None):
-        """Create a clip plane in Layout.
+    def clip_plane(self):
+        """Create a clip plane in the layout.
 
         .. note::
-            It works only in AEDT from 2022R2.
-
-        Parameters
-        ----------
-        name : str, optional
-            Name of the clip plane.
+            This method works only in AEDT 2022 R2 and later.
 
         Returns
         -------
+        str
+            Name of newly created clip plane.
+        """
+        names = self.clip_planes[::]
+        new_name = generate_unique_name("VCP", n=3)
+        self.oeditor.ClipPlane(new_name)
+        new_cp = [i for i in self.clip_planes if i not in names]
+        return new_cp[0]
 
+    @property
+    def clip_planes(self):
+        """All available clip planes. To be considered a clip plane, the name must follow this
+        naming convention: "VCP_xxx".
+
+        Returns
+        -------
+        list
         """
-        if not name:
-            name = generate_unique_name("CS")
-        self.oeditor.ClipPlane(name)
-        return name
+        return [i for i in self.oeditor.FindObjects("Name", "VCP*")]
```

### Comparing `pyaedt-0.6.70/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.71/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.71/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files 3% similar despite different names*

```diff
@@ -839,16 +839,32 @@
 
 
 class Geometries3DLayout(Objec3DLayout, object):
     """Contains geometries in HFSS 3D Layout."""
 
     def __init__(self, primitives, name, prim_type="poly", is_void=False):
         Objec3DLayout.__init__(self, primitives, prim_type)
-        self.name = name
         self.is_void = is_void
+        self._name = name
+
+    @property
+    def name(self):
+        """Name of Primitive."""
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        try:
+            del self._primitives._lines[self.name]
+            vMaterial = ["NAME:Name", "Value:=", value]
+            self.change_property(vMaterial)
+            self._name = value
+            self._primitives._lines[self._name] = self
+        except:
+            pass
 
     @property
     def is_closed(self):
         """Either if the Geometry is closed or not.
 
         Returns
         -------
@@ -1457,14 +1473,114 @@
     def center_line(self, points):
         u = self._primitives.model_units
         for point_name, value in points.items():
             vpoint = ["NAME:{}".format(point_name), "X:=", _dim_arg(value[0], u), "Y:=", _dim_arg(value[1], u)]
             self.change_property(vpoint)
         self._center_line = {}
 
+    @pyaedt_function_handler()
+    def add(self, point, position=0):
+        """Add a new point to the center line.
+
+        Parameters
+        ----------
+        point : list
+            [x,y] coordinate point to add.
+        position : int, optional
+            Position of the new point.
+
+        Returns
+        -------
+        :class:`pyaedt.modeler.pcb.object3dlayout.Line3dLayout`
+        """
+        points = [
+            [self._primitives.number_with_units(j, self.object_units) for j in i] for i in (self.center_line.values())
+        ]
+        points.insert(position, [self._primitives.number_with_units(j, self.object_units) for j in point])
+        line = self._primitives.create_line(
+            self.placement_layer,
+            points,
+            lw=self.width,
+            start_style=self.start_cap_type,
+            end_style=self.end_cap_type,
+            net_name=self.net_name,
+        )
+        line_name = self.name
+        self._primitives.oeditor.Delete([self.name])
+        line.name = line_name
+        self._primitives._lines[self.name] = line
+        return line
+
+    @pyaedt_function_handler()
+    def remove(self, point):
+        """Remove one or more points from the center line.
+
+        Parameters
+        ----------
+        point : list, str
+            Name of points to remove in the form of ``"Ptx"``.
+
+
+        Returns
+        -------
+        :class:`pyaedt.modeler.pcb.object3dlayout.Line3dLayout`
+        """
+        if isinstance(point, str):
+            point = [point]
+        points = [
+            [self._primitives.number_with_units(j, self.object_units) for j in v]
+            for i, v in self.center_line.items()
+            if i not in point
+        ]
+        line = self._primitives.create_line(
+            self.placement_layer,
+            points,
+            lw=self.width,
+            start_style=self.start_cap_type,
+            end_style=self.end_cap_type,
+            net_name=self.net_name,
+        )
+        line_name = self.name
+        self._primitives.oeditor.Delete([self.name])
+        line.name = line_name
+        self._primitives._lines[self.name] = line
+        return line
+
+    @pyaedt_function_handler()
+    def _edit(self, points):
+        name = self.name
+        arg = ["NAME:Contents", "lineGeometry:="]
+        arg2 = [
+            "Name:=",
+            name,
+            "LayerName:=",
+            self.placement_layer,
+            "lw:=",
+            self._primitives.number_with_units(self.width),
+            "endstyle:=",
+            self.end_cap_type,
+            "StartCap:=",
+            self.start_cap_type,
+            "n:=",
+            len(points),
+            "U:=",
+            self.object_units,
+        ]
+        i = 0
+        for a in points:
+            arg2.append("x{}:=".format(i))
+            arg2.append(a[0])
+            arg2.append("y{}:=".format(i))
+            arg2.append(a[1])
+            i += 1
+        arg.append(arg2)
+        arg_edit = ["NAME:items", ["NAME:item", "name:" + self.name]]
+        arg_edit[1].append(arg)
+        self._oeditor.Edit(arg_edit)
+
 
 class Points3dLayout(object):
     """Manages HFSS 3D Layout points."""
 
     def __init__(self, primitives, point):
         self._primitives = primitives
         self.point = point
@@ -1576,14 +1692,124 @@
     def is_3d_placement(self):
         """Retrieve if the component has 3d placement."""
         if self._oeditor.GetPropertyValue("BaseElementTab", self.name, "3D Placement") in ["true", "True"]:
             return True
         else:
             return False
 
+    @is_3d_placement.setter
+    def is_3d_placement(self, value):
+        props = ["NAME:3D Placement", "Value:=", value]
+        self.change_property(props)
+
+    @property
+    def is_flipped(self):
+        """Retrieve if the component is flipped or not."""
+        if self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Flipped").lower() == "true":
+            return True
+        else:
+            return False
+
+    @is_flipped.setter
+    def is_flipped(self, value):
+        props = ["NAME:Flipped", "Value:=", value]
+        self.change_property(props)
+
+    @property
+    def rotation_axis(self):
+        """Rotation axis around which the component is rotated."""
+        if self.is_3d_placement:
+            return self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Rotation Axis")
+        return False
+
+    @rotation_axis.setter
+    def rotation_axis(self, value):
+        if self.is_3d_placement and value in ["X", "Y", "Z"]:
+            props = ["NAME:Rotation Axis", "Value:=", value]
+            self.change_property(props)
+
+    @property
+    def rotation_axis_direction(self):
+        """Axis direction of the rotation."""
+        if self.is_3d_placement:
+            return [
+                float(i)
+                for i in self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Rotation Axis Direction").split(
+                    ","
+                )
+            ]
+        return [0, 0, 1]
+
+    @rotation_axis_direction.setter
+    def rotation_axis_direction(self, value):
+        if self.is_3d_placement:
+            props = ["NAME:Rotation Axis Direction", "X:=", str(value[0]), "Y:=", str(value[1]), "Z:=", str(value[2])]
+            self.change_property(props)
+
+    @property
+    def local_origin(self):
+        """Retrieve if the component has 3d placement, the local origin.
+
+        Returns
+        -------
+        list
+            [x, y, z] position.
+        """
+        if self.is_3d_placement:
+            return [i for i in self._oeditor.GetPropertyValue("BaseElementTab", self.name, "Local Origin").split(",")]
+        return [0, 0, 0]
+
+    @local_origin.setter
+    def local_origin(self, value):
+        if self.is_3d_placement:
+            value = [self._primitives._arg_with_dim(i) for i in value]
+            props = ["NAME:Local Origin", "X:=", value[0], "Y:=", value[1], "Z:=", value[2]]
+            self.change_property(props)
+
+    @property
+    def location(self):
+        """Retrieve/Set the absolute location in model units.
+        Location is computed with combination of 3d Layout location and model center.
+
+        Returns
+        -------
+        list
+           List of ``(x, y)`` coordinates for the component location.
+
+        References
+        ----------
+
+        >>> oEditor.GetPropertyValue
+        """
+        location = _retry_ntimes(
+            self._n, self._oeditor.GetPropertyValue, "BaseElementTab", self.name, "Location"
+        ).split(",")
+        locs = []
+        for i in location:
+            try:
+                locs.append(float(i))
+            except ValueError:  # pragma: no cover
+                locs.append(i)
+        return locs
+
+    @location.setter
+    def location(self, position):
+        props = [
+            "NAME:Location",
+            "X:=",
+            self._primitives.number_with_units(position[0]),
+            "Y:=",
+            self._primitives.number_with_units(position[1]),
+            "Z:=",
+            self._primitives.number_with_units(self.location[2])
+            if len(position) < 3
+            else self._primitives.number_with_units(position[2]),
+        ]
+        self.change_property(props)
+
 
 class Padstack(object):
     """Manages properties of a padstack.
 
     Parameters
     ----------
     name : str, optional
```

### Comparing `pyaedt-0.6.70/pyaedt/modeler/schematic.py` & `pyaedt-0.6.71/pyaedt/modeler/schematic.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,19 +401,22 @@
             return ", ".join(sels)
         return sels
 
     @pyaedt_function_handler()
     def _arg_with_dim(self, value, units=None):
         if units is None:
             units = self.schematic_units
-        if isinstance(value, str):
-            val = value
+        if type(value) is str:
+            try:
+                float(value)
+                val = "{0}{1}".format(value, units)
+            except:
+                val = value
         else:
             val = "{0}{1}".format(value, units)
-
         return val
 
 
 class ModelerNexxim(ModelerCircuit):
     """ModelerNexxim class.
 
     Parameters
@@ -529,16 +532,15 @@
         Parameters
         ----------
         selections : list
             List of the selections.
         pos : list
             Offset for the ``[x, y]`` axis.
         units : str
-            Units of the movement. The default is ``"meter"``. If ``None``,
-            ``schematic_units` are used.
+            Units of the movement. The default is ``meter``. If ``None``, ``schematic_units`` are used.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
```

### Comparing `pyaedt-0.6.70/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.71/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/Boundary.py` & `pyaedt-0.6.71/pyaedt/modules/Boundary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.71/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.71/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.71/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.71/pyaedt/modules/LayerStackup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 This module provides all layer stackup functionalities for the Circuit and HFSS 3D Layout tools.
 """
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
 
+from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 @pyaedt_function_handler()
 def _str2bool(str0):
     """Convert a string to a Boolean value.
 
@@ -123,50 +124,51 @@
         self.LengthUnitRough = app.LengthUnit
         self._layers = app
         self.name = None
         self.type = layertype
         self.id = 0
         self._color = [255, 0, 0]
         self._transparency = 60
-        self.IsVisible = True
-        self.IsVisibleShape = True
-        self.IsVisiblePath = True
-        self.IsVisiblePad = True
-        self.IsVisibleHole = True
-        self.IsVisibleComponent = True
-        self.IsMeshBackgroundMaterial = True
-        self.IsMeshOverlay = True
+        self._is_visible = True
+        self._is_visible_shape = True
+        self._is_visible_path = True
+        self._is_visible_pad = True
+        self._is_visible_hole = True
+        self._is_visible_component = True
+        self._is_mesh_background = True
+        self._is_mesh_overlay = True
         self._locked = False
         self._topbottom = "neither"
         self._pattern = 1
         self._drawoverride = 0
         self._thickness = 0
         self._lower_elevation = 0
         self._roughness = 0
         self._botroughness = 0
         self._toprounghenss = 0
         self._sideroughness = 0
         self._material = "copper"
         self._fillmaterial = "FR4_epoxy"
         self._index = 1
-        self.IsNegative = negative
+        self._is_negative = negative
+        self._thickness_units = ""
         # Etch option
         self._useetch = False
         self._etch = 0
         # Rough option
         self._user = False
-        self.RMdl = "Huray"
-        self.NR = 0.5
-        self.HRatio = 2.9
-        self.BRMdl = "Huray"
-        self.BNR = 0.5
-        self.BHRatio = 2.9
-        self.SRMdl = "Huray"
-        self.SNR = 0.5
-        self.SHRatio = 2.9
+        self._RMdl = "Huray"
+        self._NR = 0.5
+        self._HRatio = 2.9
+        self._BRMdl = "Huray"
+        self._BNR = 0.5
+        self._BHRatio = 2.9
+        self._SRMdl = "Huray"
+        self._SNR = 0.5
+        self._SHRatio = 2.9
         # Solver option
         self._usp = False
         self.hfssSp = {"si": True, "dt": 0, "dtv": 0.1}
         self.planaremSp = {"ifg": False, "vly": False}
         self._zones = None
 
     @property
@@ -210,124 +212,124 @@
     def is_visible(self):
         """Get/Set the active layer visibility.
 
         Returns
         -------
         bool
         """
-        return self.IsVisible
+        return self._is_visible
 
     @is_visible.setter
     def is_visible(self, val):
-        self.IsVisible = val
+        self._is_visible = val
         self.update_stackup_layer()
 
     @property
     def is_visible_shape(self):
         """Get/Set the active layer shape visibility.
 
         Returns
         -------
         bool
         """
-        return self.IsVisibleShape
+        return self._is_visible_shape
 
     @is_visible_shape.setter
     def is_visible_shape(self, val):
-        self.IsVisibleShape = val
+        self._is_visible_shape = val
         self.update_stackup_layer()
 
     @property
     def is_visible_path(self):
         """Get/Set the active layer paths visibility.
 
         Returns
         -------
         bool
         """
-        return self.IsVisiblePath
+        return self._is_visible_path
 
     @is_visible_path.setter
     def is_visible_path(self, val):
-        self.IsVisiblePath = val
+        self._is_visible_path = val
         self.update_stackup_layer()
 
     @property
     def is_visible_pad(self):
         """Get/Set the active layer pad visibility.
 
         Returns
         -------
         bool
         """
-        return self.IsVisiblePad
+        return self._is_visible_pad
 
     @is_visible_pad.setter
     def is_visible_pad(self, val):
-        self.IsVisiblePad = val
+        self._is_visible_pad = val
         self.update_stackup_layer()
 
     @property
     def is_visible_hole(self):
         """Get/Set the active layer hole visibility.
 
         Returns
         -------
         bool
         """
-        return self.IsVisibleHole
+        return self._is_visible_hole
 
     @is_visible_hole.setter
     def is_visible_hole(self, val):
-        self.IsVisibleHole = val
+        self._is_visible_hole = val
         self.update_stackup_layer()
 
     @property
     def is_visible_component(self):
         """Get/Set the active layer component visibility.
 
         Returns
         -------
         bool
         """
-        return self.IsVisibleComponent
+        return self._is_visible_component
 
     @is_visible_component.setter
     def is_visible_component(self, val):
-        self.IsVisibleComponent = val
+        self._is_visible_component = val
         self.update_stackup_layer()
 
     @property
     def is_mesh_background(self):
         """Get/Set the active layer mesh backgraound.
 
         Returns
         -------
         bool
         """
-        return self.IsMeshBackgroundMaterial
+        return self._is_mesh_background
 
     @is_mesh_background.setter
     def is_mesh_background(self, val):
-        self.IsMeshBackgroundMaterial = val
+        self._is_mesh_background = val
         self.update_stackup_layer()
 
     @property
     def is_mesh_overlay(self):
         """Get/Set the active layer mesh overlay.
 
         Returns
         -------
         bool
         """
-        return self.IsMeshOverlay
+        return self._is_mesh_overlay
 
     @is_mesh_overlay.setter
     def is_mesh_overlay(self, val):
-        self.IsMeshOverlay = val
+        self._is_mesh_overlay = val
         self.update_stackup_layer()
 
     @property
     def locked(self):
         """Get/Set the active layer lock flag.
 
         Returns
@@ -394,16 +396,29 @@
         -------
         float
         """
         return self._thickness
 
     @thickness.setter
     def thickness(self, val):
-        self._thickness = val
+        self._thickness = self._arg_with_dim(val, self.thickness_units)
         self.update_stackup_layer()
+        tck = decompose_variable_value(self._thickness)
+        self._thickness = tck[0]
+        self._thickness_units = tck[1]
+
+    @property
+    def thickness_units(self):
+        """Get the active layer thickness units value.
+
+        Returns
+        -------
+        str
+        """
+        return self._thickness_units
 
     @property
     def lower_elevation(self):
         """Get/Set the active layer lower elevation.
 
         Returns
         -------
@@ -525,19 +540,19 @@
     def is_negative(self):
         """Get/Set the active layer negative flag. When `True` the layer will be negative.
 
         Returns
         -------
         bool
         """
-        return self.IsNegative
+        return self._is_negative
 
     @is_negative.setter
     def is_negative(self, val):
-        self.IsNegative = val
+        self._is_negative = val
         self.update_stackup_layer()
 
     @property
     def use_etch(self):
         """Get/Set the active layer etiching flag. When `True` the layer will use etch.
 
         Returns
@@ -585,139 +600,139 @@
     def top_roughness_model(self):
         """Get/Set the active layer top roughness model.
 
         Returns
         -------
         str
         """
-        return self.RMdl
+        return self._RMdl
 
     @top_roughness_model.setter
     def top_roughness_model(self, val):
-        self.RMdl = val
+        self._RMdl = val
         self.update_stackup_layer()
 
     @property
     def top_nodule_radius(self):
         """Get/Set the active layer top roughness radius.
 
         Returns
         -------
         float
         """
-        return self.NR
+        return self._NR
 
     @top_nodule_radius.setter
     def top_nodule_radius(self, val):
-        self.NR = val
+        self._NR = val
         self.update_stackup_layer()
 
     @property
     def top_huray_ratio(self):
         """Get/Set the active layer top roughness ratio.
 
         Returns
         -------
         float
         """
-        return self.HRatio
+        return self._HRatio
 
     @top_huray_ratio.setter
     def top_huray_ratio(self, val):
-        self.HRatio = val
+        self._HRatio = val
         self.update_stackup_layer()
 
     @property
     def bottom_roughness_model(self):
         """Get/Set the active layer bottom roughness model.
 
         Returns
         -------
         str
         """
-        return self.BRMdl
+        return self._BRMdl
 
     @bottom_roughness_model.setter
     def bottom_roughness_model(self, val):
-        self.BRMdl = val
+        self._BRMdl = val
         self.update_stackup_layer()
 
     @property
     def bottom_nodule_radius(self):
         """Get/Set the active layer bottom roughness radius.
 
         Returns
         -------
         float
         """
-        return self.BNR
+        return self._BNR
 
     @bottom_nodule_radius.setter
     def bottom_nodule_radius(self, val):
-        self.BNR = val
+        self._BNR = val
         self.update_stackup_layer()
 
     @property
     def bottom_huray_ratio(self):
         """Get/Set the active layer bottom roughness ratio.
 
         Returns
         -------
         float
         """
-        return self.BHRatio
+        return self._BHRatio
 
     @bottom_huray_ratio.setter
     def bottom_huray_ratio(self, val):
-        self.BHRatio = val
+        self._BHRatio = val
         self.update_stackup_layer()
 
     @property
     def side_model(self):
         """Get/Set the active layer side roughness model.
 
         Returns
         -------
         str
         """
-        return self.SRMdl
+        return self._SRMdl
 
     @side_model.setter
     def side_model(self, val):
-        self.SRMdl = val
+        self._SRMdl = val
         self.update_stackup_layer()
 
     @property
     def side_nodule_radius(self):
         """Get/Set the active layer side roughness radius.
 
         Returns
         -------
         float
         """
-        return self.SNR
+        return self._SNR
 
     @side_nodule_radius.setter
     def side_nodule_radius(self, val):
-        self.SNR = val
+        self._SNR = val
         self.update_stackup_layer()
 
     @property
     def side_huray_ratio(self):
         """Get/Set the active layer bottom roughness ratio.
 
         Returns
         -------
         float
         """
-        return self.SHRatio
+        return self._SHRatio
 
     @side_huray_ratio.setter
     def side_huray_ratio(self, val):
-        self.SHRatio = val
+        self._SHRatio = val
         self.update_stackup_layer()
 
     @property
     def usp(self):
         """Get/Set the active layer usp flag.
 
         Returns
@@ -783,30 +798,30 @@
         """Oeditor Module."""
         return self._layers.oeditor
 
     @property
     def visflag(self):
         """Visibility flag for objects on the layer."""
         visflag = 0
-        if not self.IsVisible:
+        if not self._is_visible:
             visflag = 0
         else:
-            if self.IsMeshBackgroundMaterial:
+            if self._is_mesh_background:
                 visflag += 64
-            if self.IsMeshOverlay:
+            if self._is_mesh_overlay:
                 visflag += 32
-            if self.IsVisibleShape:
+            if self._is_visible_shape:
                 visflag += 1
-            if self.IsVisiblePath:
+            if self._is_visible_path:
                 visflag += 2
-            if self.IsVisiblePad:
+            if self.is_visible_pad:
                 visflag += 4
-            if self.IsVisibleHole:
+            if self._is_visible_hole:
                 visflag += 8
-            if self.IsVisibleComponent:
+            if self._is_visible_component:
                 visflag += 16
         return visflag
 
     @pyaedt_function_handler()
     def set_layer_color(self, r, g, b):
         """Update the color of the layer.
 
@@ -867,21 +882,24 @@
         units :
              The default is ``None``.
 
         Returns
         -------
 
         """
-        if isinstance(value, str):
-            val = value
+        if units is None:
+            units = self.LengthUnit
+        if type(value) is str:
+            try:
+                float(value)
+                val = "{0}{1}".format(value, units)
+            except:
+                val = value
         else:
-            if units is None:
-                units = self.LengthUnit
             val = "{0}{1}".format(value, units)
-
         return val
 
     @property
     def _get_layer_arg(self):
         if self.type in ["signal", "via", "dielectric"]:
             args = [
                 "NAME:stackup layer",
@@ -918,30 +936,30 @@
                     "DrawOverride:=",
                     self.draw_override,
                     "Zones:=",
                     self.zones,
                     [
                         "NAME:Sublayer",
                         "Thickness:=",
-                        self.thickness,
+                        self._arg_with_dim(self.thickness, self.thickness_units),
                         "LowerElevation:=",
                         self._arg_with_dim(self.lower_elevation, self.LengthUnit),
                         "Roughness:=",
                         self._arg_with_dim(self.roughness, self.LengthUnitRough),
                         "BotRoughness:=",
                         self._arg_with_dim(self.bottom_roughness, self.LengthUnitRough),
                         "SideRoughness:=",
                         self._arg_with_dim(self.top_roughness, self.LengthUnitRough),
                         "Material:=",
                         self.material.lower(),
                         "FillMaterial:=",
                         self.fill_material.lower(),
                     ],
                     "Neg:=",
-                    self.IsNegative,
+                    self._is_negative,
                     "Usp:=",
                     self.usp,
                     [
                         "NAME:Sp",
                         "Sn:=",
                         "HFSS",
                         "Sv:=",
@@ -967,31 +985,31 @@
                     "Etch:=",
                     str(self.etch),
                     "UseEtch:=",
                     self.use_etch,
                     "UseR:=",
                     self.user,
                     "RMdl:=",
-                    self.RMdl,
+                    self._RMdl,
                     "NR:=",
-                    self._arg_with_dim(self.NR, self.LengthUnitRough),
+                    self._arg_with_dim(self._NR, self.LengthUnitRough),
                     "HRatio:=",
-                    str(self.HRatio),
+                    str(self._HRatio),
                     "BRMdl:=",
-                    self.BRMdl,
+                    self._BRMdl,
                     "BNR:=",
-                    self._arg_with_dim(self.BNR, self.LengthUnitRough),
+                    self._arg_with_dim(self._BNR, self.LengthUnitRough),
                     "BHRatio:=",
-                    str(self.BHRatio),
+                    str(self._BHRatio),
                     "SRMdl:=",
-                    self.SRMdl,
+                    self._SRMdl,
                     "SNR:=",
-                    self._arg_with_dim(self.SNR, self.LengthUnitRough),
+                    self._arg_with_dim(self._SNR, self.LengthUnitRough),
                     "SHRatio:=",
-                    str(self.SHRatio),
+                    str(self._SHRatio),
                 ]
             )
         elif self.type == "dielectric":
             args.extend(
                 [
                     "Type:=",
                     self.type,
@@ -1010,17 +1028,17 @@
                     "DrawOverride:=",
                     self.draw_override,
                     "Zones:=",
                     self.zones,
                     [
                         "NAME:Sublayer",
                         "Thickness:=",
-                        self.thickness,
+                        self._arg_with_dim(self.thickness, self.thickness_units),
                         "LowerElevation:=",
-                        self.lower_elevation,
+                        self._arg_with_dim(self.lower_elevation, self.LengthUnit),
                         "Roughness:=",
                         0,
                         "BotRoughness:=",
                         0,
                         "SideRoughness:=",
                         0,
                         "Material:=",
@@ -1203,14 +1221,63 @@
         List of :class:`pyaedt.modules.LayerStackup.Layer`
             List of signal layers.
         """
 
         return [v for k, v in self.layers.items() if v.type == "signal"]
 
     @property
+    def signals(self):
+        """All signal layers.
+
+        Returns
+        -------
+        Dict[str, :class:`pyaedt.modules.LayerStackup.Layer`]
+           Conductor layers.
+
+        References
+        ----------
+
+        >>> oEditor.GetAllLayerNames()
+        """
+        return {k: v for k, v in self.layers.items() if v.type == "signal"}
+
+    @property
+    def dielectrics(self):
+        """All dielectric layers.
+
+        Returns
+        -------
+        Dict[str, :class:`pyaedt.modules.LayerStackup.Layer`]
+           Dielectric layers.
+
+        References
+        ----------
+
+        >>> oEditor.GetAllLayerNames()
+        """
+        return {k: v for k, v in self.layers.items() if v.type == "dielectric"}
+
+    @property
+    def drawings(self):
+        """All stackup layers.
+
+        Returns
+        -------
+        Dict[str, :class:`pyaedt.modules.LayerStackup.Layer`]
+           Drawing layers.
+
+        References
+        ----------
+
+        >>> oEditor.GetAllLayerNames()
+        """
+
+        return {k: v for k, v in self.layers.items() if v.type in ["signal", "via", "dielectric"]}
+
+    @property
     def all_diel_layers(self):
         """All dielectric layers.
 
         Returns
         -------
         List of :class:`pyaedt.modules.LayerStackup.Layer`
             List of dielectric layers.
@@ -1251,52 +1318,54 @@
             o.name = el
             infos = self.oeditor.GetLayerInfo(el)
             infos = [i.split(": ") for i in infos]
             infosdict = {i[0].strip(): i[1].strip() for i in infos}
             o.id = int(infosdict["LayerId"])
             if infosdict["Type"] == "metalizedsignal":
                 o.type = "signal"
-                o.IsNegative = True
+                o._is_negative = True
             else:
                 o.type = infosdict["Type"]
-                o.IsNegative = False
+                o._is_negative = False
             o._locked = _str2bool(infosdict["IsLocked"])
             o._top_bottom = infosdict["TopBottomAssociation"].lower()
-            o.IsVisible = infosdict["IsVisible"]
+            o._is_visible = _str2bool(infosdict["IsVisible"])
             if "IsVisiblePath" in infosdict:
-                o.IsVisiblePath = infosdict["IsVisiblePath"]
-                o.IsVisiblePad = infosdict["IsVisiblePad"]
-                o.IsVisibleComponent = infosdict["IsVisibleComponent"]
-                o.IsVisibleShape = infosdict["IsVisibleShape"]
-                o.IsVisibleHole = infosdict["IsVisibleHole"]
+                o._is_visible_path = _str2bool(infosdict["IsVisiblePath"])
+                o._is_visible_pad = _str2bool(infosdict["IsVisiblePad"])
+                o._is_visible_component = _str2bool(infosdict["IsVisibleComponent"])
+                o._is_visible_shape = _str2bool(infosdict["IsVisibleShape"])
+                o._is_visible_hole = _str2bool(infosdict["IsVisibleHole"])
             o._color = _getRGBfromI(int(infosdict["Color"][:-1]))
             if o.type in ["signal", "dielectric", "via"]:
                 o._index = int(infosdict["Index"])
-                o._thickness = _conv_number(infosdict["LayerThickness"])
-                o._lower_elevation = _conv_number(infosdict["LowerElevation0"])
+                tck = decompose_variable_value(infosdict["LayerThickness"])
+                o._thickness = tck[0]
+                o._thickness_units = tck[1]
+                o._lower_elevation = decompose_variable_value(infosdict["LowerElevation0"])[0]
                 o._fillmaterial = infosdict["FillMaterial0"]
                 o._material = infosdict["Material0"]
                 if "EtchFactor" in infosdict:
                     o._useetch = True
-                    o._etch = _conv_number(infosdict["EtchFactor"])
+                    o._etch = decompose_variable_value(infosdict["EtchFactor"])[0]
                 if "Roughness0 Type" in infosdict:
                     o._user = True
-                    o.RMdl = infosdict["Roughness0 Type"]
-                    o.NR = infosdict["Roughness0"].split(", ")[0]
-                    o.HRatio = _conv_number(infosdict["Roughness0"].split(", ")[1])
+                    o._RMdl = infosdict["Roughness0 Type"]
+                    o._NR = infosdict["Roughness0"].split(", ")[0]
+                    o._HRatio = decompose_variable_value(infosdict["Roughness0"].split(", ")[1])[0]
                 if "BottomRoughness0 Type" in infosdict:
                     o._user = True
-                    o.BRMdl = infosdict["BottomRoughness0 Type"]
-                    o.BNR = infosdict["BottomRoughness0"].split(", ")[0]
-                    o.BHRatio = _conv_number(infosdict["BottomRoughness0"].split(", ")[1])
+                    o._BRMdl = infosdict["BottomRoughness0 Type"]
+                    o._BNR = infosdict["BottomRoughness0"].split(", ")[0]
+                    o._BHRatio = decompose_variable_value(infosdict["BottomRoughness0"].split(", ")[1])[0]
                 if "SideRoughness0 Type" in infosdict:
                     o._user = True
-                    o.SRMdl = infosdict["SideRoughness0 Type"]
-                    o.SNR = infosdict["SideRoughness0"].split(", ")[0]
-                    o.SHRatio = _conv_number(infosdict["SideRoughness0"].split(", ")[1])
+                    o._SRMdl = infosdict["SideRoughness0 Type"]
+                    o._SNR = infosdict["SideRoughness0"].split(", ")[0]
+                    o._SHRatio = decompose_variable_value(infosdict["SideRoughness0"].split(", ")[1])[0]
             layers[o.id] = o
         return layers
 
     @pyaedt_function_handler()
     def add_layer(
         self, layername, layertype="signal", thickness="0mm", elevation="0mm", material="copper", isnegative=False
     ):
```

### Comparing `pyaedt-0.6.70/pyaedt/modules/Material.py` & `pyaedt-0.6.71/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.71/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/Mesh.py` & `pyaedt-0.6.71/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.71/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.71/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.71/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.71/pyaedt/modules/PostProcessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3799,37 +3799,37 @@
     ):
         """Create an SBR Point Source Visual Ray Tracing and return the class object.
 
         Parameters
         ----------
 
         max_frequency : str, optional
-            Maximum Frequency. Default is ``"1GHz"``.
+            Maximum Frequency. Default is ``1GHz``.
         ray_density : int, optional
             Ray Density. Default is ``2``.
         number_of_bounces : int, optional
             Maximum number of bounces. Default is ``5``.
         multi_bounce : bool, optional
             Whether if enable or not Multi-Bounce ray density control. Default is ``False``.
         mbrd_max_sub_division : int, optional
             Maximum number of MBRD subdivisions. Default is ``2``.
         shoot_utd : bool, optional
             Whether if enable or UTD Rays shooting or not. Default is ``False``.
         custom_location : list, optional
             List of x, y,z position of point source. Default is ``None`.
         shoot_filter_type : str, optional
-            Shooter Type. Default is ``"All Rays"``. Options are  ``"Rays by index"``,  ``"Rays in box"``.
+            Shooter Type. Default is ``"All Rays"``. Options are ``Rays by index``, ``Rays in box``.
         ray_index_start : int, optional
-            Ray index start. Valid only if ``"Rays by index"`` is chosen.  Default is ``0``.
+            Ray index start. Valid only if ``Rays by index`` is chosen.  Default is ``0``.
         ray_index_stop : int, optional
-            Ray index stop. Valid only if ``"Rays by index"`` is chosen.  Default is ``1``.
+            Ray index stop. Valid only if ``Rays by index`` is chosen.  Default is ``1``.
         ray_index_step : int, optional
-            Ray index step. Valid only if ``"Rays by index"`` is chosen.  Default is ``1``.
+            Ray index step. Valid only if ``Rays by index`` is chosen.  Default is ``1``.
         ray_box : int or str optional
-            Ray box name or id. Valid only if ``"Rays by box"`` is chosen.  Default is ``None``.
+            Ray box name or id. Valid only if ``Rays by box`` is chosen.  Default is ``None``.
 
         Returns
         -------
         :class:` pyaedt.modules.solutions.VRTFieldPlot`
         """
         if custom_location is None:
             custom_location = [0, 0, 0]
```

### Comparing `pyaedt-0.6.70/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.71/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.71/pyaedt/modules/SolveSetup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.71/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.71/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/report_templates.py` & `pyaedt-0.6.71/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/modules/solutions.py` & `pyaedt-0.6.71/pyaedt/modules/solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/q3d.py` & `pyaedt-0.6.71/pyaedt/q3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1490,17 +1490,122 @@
         bound = BoundaryObject(self, net_name, props, type_bound)
         if bound.create():
             self.boundaries.append(bound)
             return bound
         return False
 
     @pyaedt_function_handler()
+    def source(self, objects=None, axisdir=0, name=None, net_name=None, terminal_type="voltage"):
+        """Generate a source on a face of an object or a group of faces or face ids.
+        The face ID is selected based on the axis direction. It is the face that
+        has the maximum/minimum in this axis direction.
+
+        Parameters
+        ----------
+        objects : str, int or list or :class:`pyaedt.modeler.object3d.Object3d`
+            Name of the object or face ID or face ID list.
+        axisdir : int, optional
+            Initial axis direction. Options are ``0`` to ``5``. The default is ``0``.
+        name : str, optional
+            Name of the source. The default is ``None``.
+        net_name : str, optional
+            Name of the net. The default is ``None``, in which case the ``object_name`` is considered.
+        terminal_type : str
+            Type of the terminal. Options are ``voltage`` and ``current``. The default is ``voltage``.
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Source object.
+
+        References
+        ----------
+
+        >>> oModule.AssignSource
+        """
+        return self._assign_source_or_sink(objects, axisdir, name, net_name, terminal_type, "Source")
+
+    @pyaedt_function_handler()
+    def sink(self, objects=None, axisdir=0, name=None, net_name=None, terminal_type="voltage"):
+        """Generate a sink on a face of an object or a group of faces or face ids.
+
+        The face ID is selected based on the axis direction. It is the face that
+        has the maximum/minimum in this axis direction.
+
+        Parameters
+        ----------
+        objects : str, int or list or :class:`pyaedt.modeler.object3d.Object3d`
+            Name of the object or face ID or face ID list.
+        axisdir : int, optional
+            Initial axis direction. Options are ``0`` to ``5``. The default is ``0``.
+        name : str, optional
+            Name of the source. The default is ``None``.
+        net_name : str, optional
+            Name of the net. The default is ``None``, in which case the ``object_name`` is considered.
+        terminal_type : str
+            Type of the terminal. Options are ``voltage`` and ``current``. The default is ``voltage``.
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Sink object.
+
+        References
+        ----------
+
+        >>> oModule.AssignSource
+        """
+        return self._assign_source_or_sink(objects, axisdir, name, net_name, terminal_type, "Sink")
+
+    @pyaedt_function_handler()
+    def _assign_source_or_sink(self, objects, axisdir, name, net_name, terminal_type, exc_type):
+        if not name:
+            name = generate_unique_name(exc_type)
+        objects = self.modeler.convert_to_selections(objects, True)
+        sheets = []
+        is_face = True
+        for object_name in objects:
+            if isinstance(object_name, str) and object_name in self.modeler.solid_names:
+                sheets.append(self.modeler._get_faceid_on_axis(object_name, axisdir))
+                if not net_name:
+                    for net in self.nets:
+                        if object_name in self.objects_from_nets(net):
+                            net_name = net
+            elif isinstance(object_name, str):
+                is_face = False
+                sheets.append(object_name)
+            else:
+                sheets.append(object_name)
+
+        if is_face:
+            props = OrderedDict({"Faces": sheets})
+        else:
+            props = OrderedDict({"Objects": sheets})
+
+        if terminal_type == "current":
+            terminal_str = "UniformCurrent"
+        else:
+            terminal_str = "ConstantVoltage"
+
+        props["TerminalType"] = terminal_str
+        if net_name:
+            props["Net"] = net_name
+        bound = BoundaryObject(self, name, props, exc_type)
+        if bound.create():
+            self.boundaries.append(bound)
+            return bound
+        return False
+
+    @pyaedt_function_handler()
     def assign_source_to_objectface(self, object_name, axisdir=0, source_name=None, net_name=None):
         """Generate a source on a face of an object.
 
+        .. deprecated:: 0.6.70
+           Use :func:`source` method instead.
+
         The face ID is selected based on the axis direction. It is the face that
         has the maximum/minimum in this axis direction.
 
         Parameters
         ----------
         object_name : str, int
             Name of the object or face ID.
@@ -1517,43 +1622,30 @@
             Source object.
 
         References
         ----------
 
         >>> oModule.AssignSource
         """
-        object_name = self.modeler.convert_to_selections(object_name, True)[0]
-        if isinstance(object_name, int):
-            a = object_name
-        else:
-            a = self.modeler._get_faceid_on_axis(object_name, axisdir)
-        if not source_name:
-            source_name = generate_unique_name("Source")
-        if not net_name:
-            net_name = object_name
-        if a:
-            props = OrderedDict(
-                {"Faces": [a], "ParentBndID": object_name, "TerminalType": "ConstantVoltage", "Net": net_name}
-            )
-            bound = BoundaryObject(self, source_name, props, "Source")
-            if bound.create():
-                self.boundaries.append(bound)
-                return bound
-        return False
+        warnings.warn("Use :func:`source` method instead.", DeprecationWarning)
+        return self.source(objects=object_name, axisdir=0, name=source_name, net_name=net_name)
 
     @pyaedt_function_handler()
     def assign_source_to_sheet(
         self, sheetname, objectname=None, netname=None, sourcename=None, terminal_type="voltage"
     ):
         """Generate a source on a sheet.
 
+        .. deprecated:: 0.6.70
+           Use :func:`source` method instead.
+
         Parameters
         ----------
-        sheetname : str, int
-            Name of the sheet to create the source on.
+        sheetname : str, int or list
+            Name of the sheets to create the source on.
         objectname :  str, optional
             Name of the parent object. The default is ``None``.
         netname : str, optional
             Name of the net. The default is ``None``.
         sourcename : str,  optional
             Name of the source. The default is ``None``.
         terminal_type : str
@@ -1565,38 +1657,16 @@
             Source object.
 
         References
         ----------
 
         >>> oModule.AssignSource
         """
-        if not sourcename:
-            sourcename = generate_unique_name("Source")
-        sheetname = self.modeler.convert_to_selections(sheetname, True)[0]
-        if isinstance(sheetname, int):
-            props = OrderedDict({"Faces": [sheetname]})
-        else:
-            props = OrderedDict({"Objects": [sheetname]})
-
-        if objectname:
-            props["ParentBndID"] = objectname
-
-        if terminal_type == "current":
-            terminal_str = "UniformCurrent"
-        else:
-            terminal_str = "ConstantVoltage"
-
-        props["TerminalType"] = terminal_str
-        if netname:
-            props["Net"] = netname
-        bound = BoundaryObject(self, sourcename, props, "Source")
-        if bound.create():
-            self.boundaries.append(bound)
-            return bound
-        return False
+        warnings.warn("Use :func:`source` method instead.", DeprecationWarning)
+        return self.source(objects=sheetname, name=sourcename, net_name=netname, terminal_type=terminal_type)
 
     @pyaedt_function_handler()
     def assign_sink_to_objectface(self, object_name, axisdir=0, sink_name=None, net_name=None):
         """Generate a sink on a face of an object.
 
         The face ID is selected based on the axis direction. It is the face that has
         the maximum or minimum in this axis direction.
```

### Comparing `pyaedt-0.6.70/pyaedt/rmxprt.py` & `pyaedt-0.6.71/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.71/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.71/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.71/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.71/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.71/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/siwave.py` & `pyaedt-0.6.71/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyaedt/twinbuilder.py` & `pyaedt-0.6.71/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.70/pyproject.toml` & `pyaedt-0.6.71/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     "rpyc==5.3.0",
     "psutil",
     "dotnetcore2 ==3.1.23;platform_system=='Linux'",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "codecov==2.1.12",
     "ipython==8.8.0",
     "joblib==1.2.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.1; python_version > '3.7'",
     "openpyxl==3.0.10",
```

### Comparing `pyaedt-0.6.70/PKG-INFO` & `pyaedt-0.6.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.70
+Version: 0.6.71
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -69,15 +69,14 @@
 Requires-Dist: pandas==1.5.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
 Requires-Dist: pyvista==0.37.0 ; extra == "full"
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.0.10 ; extra == "full"
-Requires-Dist: codecov==2.1.12 ; extra == "tests"
 Requires-Dist: ipython==8.8.0 ; extra == "tests"
 Requires-Dist: joblib==1.2.0 ; extra == "tests"
 Requires-Dist: matplotlib==3.5.3 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: openpyxl==3.0.10 ; extra == "tests"
```

