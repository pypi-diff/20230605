# Comparing `tmp/pyaedt-0.6.78.tar.gz` & `tmp/pyaedt-0.6.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.78.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.6.79.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.6.78.tar` & `pyaedt-0.6.79.tar`

### file list

```diff
@@ -1,252 +1,255 @@
--rw-r--r--   0        0        0     1111 2023-05-16 06:59:23.102429 pyaedt-0.6.78/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-16 06:59:23.102429 pyaedt-0.6.78/README.md
--rw-r--r--   0        0        0     2691 2023-05-29 08:06:46.309364 pyaedt-0.6.78/pyaedt/__init__.py
--rw-r--r--   0        0        0    26683 2023-05-24 15:53:22.079958 pyaedt-0.6.78/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-05-16 06:59:25.180542 pyaedt-0.6.78/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88300 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    41317 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17066 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19852 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4431 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4596 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   128778 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75524 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12464 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    36749 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    62954 2023-05-23 13:08:30.544249 pyaedt-0.6.78/pyaedt/circuit.py
--rw-r--r--   0        0        0    10034 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    64534 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1092 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-05-16 06:59:25.227417 pyaedt-0.6.78/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-05-16 06:59:25.227417 pyaedt-0.6.78/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-05-16 06:59:25.227417 pyaedt-0.6.78/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-05-16 06:59:25.243041 pyaedt-0.6.78/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-05-16 06:59:25.243041 pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-05-16 06:59:25.243041 pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-05-16 06:59:25.258665 pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-05-16 06:59:25.274293 pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-05-16 06:59:25.289918 pyaedt-0.6.78/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-05-16 06:59:25.289918 pyaedt-0.6.78/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-05-16 06:59:25.289918 pyaedt-0.6.78/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-05-16 06:59:25.305543 pyaedt-0.6.78/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    23386 2023-05-25 10:01:32.202746 pyaedt-0.6.78/pyaedt/downloads.py
--rw-r--r--   0        0        0   143749 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-05-16 06:59:25.305543 pyaedt-0.6.78/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    92788 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.305543 pyaedt-0.6.78/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    32911 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0    40100 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0      937 2023-05-16 06:59:25.305543 pyaedt-0.6.78/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      324 2023-05-16 06:59:25.305543 pyaedt-0.6.78/pyaedt/edb_core/edb_data/edb_builder.py
--rw-r--r--   0        0        0      867 2023-05-25 15:57:26.266409 pyaedt-0.6.78/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12198 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65637 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20336 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     4781 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61168 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32355 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0    99883 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36339 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    33759 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     4147 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2425 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    66640 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2844 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7763 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4703 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11390 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21750 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    49121 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33299 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    43737 2023-05-29 06:50:09.631460 pyaedt-0.6.78/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    46668 2023-05-29 06:50:09.631460 pyaedt-0.6.78/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    57190 2023-05-29 06:50:09.631460 pyaedt-0.6.78/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   109028 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11363 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3291 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/emit_core/EmitConstants.py
--rw-r--r--   0        0        0     1091 2023-05-20 16:14:01.011451 pyaedt-0.6.78/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0        2 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-05-19 04:27:23.959058 pyaedt-0.6.78/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    12248 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    11758 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-05-26 11:30:36.599404 pyaedt-0.6.78/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83444 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    21891 2023-05-24 15:53:22.126810 pyaedt-0.6.78/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3395 2023-05-19 12:41:48.802021 pyaedt-0.6.78/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    69591 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62327 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11301 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/process.py
--rw-r--r--   0        0        0    20326 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3466 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60412 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   252848 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/hfss.py
--rw-r--r--   0        0        0    82916 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   168417 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/icepak.py
--rw-r--r--   0        0        0   118479 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24316 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3818 2023-05-19 12:41:48.802021 pyaedt-0.6.78/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14107 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    20051 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16840 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120888 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   194593 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   116607 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11387 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   127894 2023-05-24 13:33:05.690067 pyaedt-0.6.78/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    31589 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49057 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59078 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53131 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12645 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42629 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32780 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8212 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63100 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15149 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.446165 pyaedt-0.6.78/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    32013 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68135 2023-05-19 10:14:06.395089 pyaedt-0.6.78/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6952 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    52600 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    31327 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49892 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.446165 pyaedt-0.6.78/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65639 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23689 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30094 2023-05-16 06:59:25.461791 pyaedt-0.6.78/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   114715 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71549 2023-05-16 06:59:25.461791 pyaedt-0.6.78/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-05-16 06:59:25.461791 pyaedt-0.6.78/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51967 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40465 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82903 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28363 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53226 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11976 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    26105 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-05-16 06:59:25.461791 pyaedt-0.6.78/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   173007 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64104 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   119432 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33257 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    28709 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103333 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   125079 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95908 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/q3d.py
--rw-r--r--   0        0        0    10581 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7632 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10430 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4426 2023-05-29 07:58:53.347931 pyaedt-0.6.78/pyproject.toml
--rw-r--r--   0        0        0    15568 1970-01-01 00:00:00.000000 pyaedt-0.6.78/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-30 06:59:37.486926 pyaedt-0.6.79/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-30 06:59:37.486926 pyaedt-0.6.79/README.md
+-rw-r--r--   0        0        0     2691 2023-06-05 18:57:16.886587 pyaedt-0.6.79/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26683 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88300 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    41317 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17066 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19852 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4431 2023-05-30 06:59:39.408947 pyaedt-0.6.79/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4596 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   129320 2023-06-05 14:54:59.781956 pyaedt-0.6.79/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75524 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12464 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    36749 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    62954 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10247 2023-06-05 09:04:16.749339 pyaedt-0.6.79/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    64951 2023-06-05 14:54:59.781956 pyaedt-0.6.79/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1092 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-05-30 06:59:39.424579 pyaedt-0.6.79/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-05-30 06:59:39.440208 pyaedt-0.6.79/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-05-30 06:59:39.440208 pyaedt-0.6.79/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-05-30 06:59:39.440208 pyaedt-0.6.79/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-05-30 06:59:39.440208 pyaedt-0.6.79/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-05-30 06:59:39.455836 pyaedt-0.6.79/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-05-30 06:59:39.455836 pyaedt-0.6.79/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-05-30 06:59:39.455836 pyaedt-0.6.79/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-05-30 06:59:39.471459 pyaedt-0.6.79/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-05-30 06:59:39.471459 pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-05-30 06:59:39.471459 pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-05-30 06:59:39.487088 pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-05-30 06:59:39.502713 pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-05-30 06:59:39.502713 pyaedt-0.6.79/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-05-30 06:59:39.518353 pyaedt-0.6.79/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-05-30 06:59:39.518353 pyaedt-0.6.79/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    23386 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/downloads.py
+-rw-r--r--   0        0        0   136802 2023-06-05 14:54:59.781956 pyaedt-0.6.79/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    92242 2023-06-05 09:36:43.922575 pyaedt-0.6.79/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:36:43.922575 pyaedt-0.6.79/pyaedt/edb_core/dotnet/__init__.py
+-rw-r--r--   0        0        0    31497 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/dotnet/database.py
+-rw-r--r--   0        0        0     7909 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/dotnet/layout.py
+-rw-r--r--   0        0        0    48210 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/dotnet/primitive.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    32946 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    40100 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      867 2023-05-30 06:59:39.533962 pyaedt-0.6.79/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12243 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65661 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20386 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     4025 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61171 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    33851 2023-06-05 15:29:29.398358 pyaedt-0.6.79/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0   101786 2023-06-05 14:54:59.781956 pyaedt-0.6.79/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36324 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    33847 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     3923 2023-06-05 14:54:59.781956 pyaedt-0.6.79/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2432 2023-06-05 09:36:43.938202 pyaedt-0.6.79/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    66975 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-05-30 06:59:39.549589 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2850 2023-06-05 09:36:43.953828 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7763 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4703 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11390 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-05-30 06:59:39.565215 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21800 2023-06-05 09:36:43.953828 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    47125 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33310 2023-06-05 09:36:43.953828 pyaedt-0.6.79/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    44030 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    47600 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    57553 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   109207 2023-06-05 09:36:43.953828 pyaedt-0.6.79/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11363 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit.py
+-rw-r--r--   0        0        0     3555 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3291 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit_core/EmitConstants.py
+-rw-r--r--   0        0        0     1091 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0        2 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    13338 2023-06-05 14:54:59.797581 pyaedt-0.6.79/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    11758 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-30 06:59:39.580847 pyaedt-0.6.79/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83444 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3395 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    69591 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    25808 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     6989 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62327 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11301 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3466 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60412 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   253082 2023-06-05 09:04:16.749339 pyaedt-0.6.79/pyaedt/hfss.py
+-rw-r--r--   0        0        0    82916 2023-05-30 06:59:39.596468 pyaedt-0.6.79/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   168417 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/icepak.py
+-rw-r--r--   0        0        0   118479 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24316 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3695 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     2380 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     3731 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     3818 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-05-30 06:59:39.612097 pyaedt-0.6.79/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14107 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20051 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-05-30 06:59:39.627726 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16840 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120888 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   194639 2023-05-30 14:16:58.540805 pyaedt-0.6.79/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   116607 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11387 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   127894 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    31589 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49057 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59078 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53131 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12645 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42629 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    32780 2023-05-30 06:59:39.643351 pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8212 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63100 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15149 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    32013 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68135 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6952 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    59936 2023-05-30 14:16:58.540805 pyaedt-0.6.79/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    31327 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49892 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65639 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23689 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    30094 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   114715 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71549 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51967 2023-05-30 06:59:39.658979 pyaedt-0.6.79/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40465 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82903 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28363 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53226 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11976 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    26105 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   173007 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64104 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   119432 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33257 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    28709 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103333 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   125079 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95908 2023-05-30 06:59:39.674599 pyaedt-0.6.79/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10581 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7632 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10410 2023-06-05 09:36:43.953828 pyaedt-0.6.79/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-05-30 06:59:39.690227 pyaedt-0.6.79/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4426 2023-06-01 13:49:54.137333 pyaedt-0.6.79/pyproject.toml
+-rw-r--r--   0        0        0    15568 1970-01-01 00:00:00.000000 pyaedt-0.6.79/PKG-INFO
```

### Comparing `pyaedt-0.6.78/LICENSE` & `pyaedt-0.6.79/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/README.md` & `pyaedt-0.6.79/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/__init__.py` & `pyaedt-0.6.79/pyaedt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.78"
+__version__ = "0.6.79"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
```

### Comparing `pyaedt-0.6.78/pyaedt/aedt_logger.py` & `pyaedt-0.6.79/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.79/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/Analysis.py` & `pyaedt-0.6.79/pyaedt/application/Analysis.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.79/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.79/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.79/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.79/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.79/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.79/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/Design.py` & `pyaedt-0.6.79/pyaedt/application/Design.py`

 * *Files 0% similar despite different names*

```diff
@@ -2197,18 +2197,32 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
+        self.desktop_class.release_desktop(close_projects, close_desktop)
         release_desktop(close_projects, close_desktop)
         props = [a for a in dir(self) if not a.startswith("__")]
         for a in props:
             self.__dict__.pop(a, None)
+
+        dicts = [self, sys.modules["__main__"]]
+        for dict_to_clean in dicts:
+            props = [
+                a
+                for a in dir(dict_to_clean)
+                if "win32com" in str(type(dict_to_clean.__dict__.get(a, None)))
+                or "pyaedt" in str(type(dict_to_clean.__dict__.get(a, None)))
+            ]
+            for a in props:
+                dict_to_clean.__dict__[a] = None
+
+        self._desktop_class = None
         gc.collect()
         return True
 
     @pyaedt_function_handler()
     def generate_temp_project_directory(self, subdir_name):
         """Generate a unique directory string to save a project to.
```

### Comparing `pyaedt-0.6.78/pyaedt/application/JobManager.py` & `pyaedt-0.6.79/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/Variables.py` & `pyaedt-0.6.79/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.79/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/application/design_solutions.py` & `pyaedt-0.6.79/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/circuit.py` & `pyaedt-0.6.79/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/common_rpc.py` & `pyaedt-0.6.79/pyaedt/common_rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,33 +137,35 @@
     --------
     >>> from pyaedt.common_rpc import pyaedt_service_manager
     >>> pyaedt_service_manager()
 
     """
     port1 = check_port(port)
     if port == 0:
-        print("Error. No ports are available.")
+        logger.error("Error. No ports are available.")
         return False
     if port1 != port:
-        print("Port {} is already in use. Starting the server on port {}.".format(port, port1))
+        logger.info("Port {} is already in use. Starting the server on port {}.".format(port, port1))
     aa = list_installed_ansysem()
     if aedt_version:
         if student_version:
             v = "ANSYSEMSV_ROOT{}".format(aedt_version[-4:].replace(".", ""))
         else:
             v = "ANSYSEM_ROOT{}".format(aedt_version[-4:].replace(".", ""))
 
         valid_version = v
     else:
         if aa:
             valid_version = aa[0]
         else:
-            raise Exception("no ANSYSEM_ROOTXXX environment variable defined.")
+            raise Exception("No ANSYSEM_ROOTXXX environment variable defined.")
 
-    os.environ["PYAEDT_SERVER_AEDT_PATH"] = os.environ[valid_version]
+    ansysem_path = os.environ[valid_version]
+    logger.info("AEDT located at {} will be used.".format(ansysem_path))
+    os.environ["PYAEDT_SERVER_AEDT_PATH"] = ansysem_path
     os.environ["PYAEDT_SERVER_AEDT_NG"] = "True"
     os.environ["ANS_NODEPCHECK"] = str(1)
 
     hostname = socket.gethostname()
     t = ThreadedServer(
         ServiceManager,
         hostname=hostname,
@@ -204,24 +206,25 @@
     --------
     >>> from pyaedt.common_rpc import launch_server
     >>> launch_server()
 
     """
     port1 = check_port(port)
     if port == 0:
-        print("Error. No ports are available.")
+        logger.error("Error. No ports are available.")
         return False
     if port1 != port:
-        print("Port {} is already in use. Starting the server on port {}.".format(port, port1))
+        logger.info("Port {} is already in use. Starting the server on port {}.".format(port, port1))
     if not ansysem_path:
         aa = list_installed_ansysem()
         if aa:
             ansysem_path = os.environ[aa[0]]
         else:
-            raise Exception("no ANSYSEM_ROOTXXX environment variable defined.")
+            raise Exception("No ANSYSEM_ROOTXXX environment variable defined.")
+    logger.info("AEDT located at {} will be used.".format(ansysem_path))
     os.environ["PYAEDT_SERVER_AEDT_PATH"] = ansysem_path
     os.environ["PYAEDT_SERVER_AEDT_NG"] = str(non_graphical)
     os.environ["ANS_NO_MONO_CLEANUP"] = str(1)
     os.environ["ANS_NODEPCHECK"] = str(1)
 
     hostname = socket.gethostname()
     if threaded:
@@ -237,15 +240,15 @@
             "allow_public_attrs": True,
             "allow_setattr": True,
             "safe_attrs": safe_attrs,
             "allow_delattr": True,
             "logger": logger,
         },
     )
-    print("Starting the server on port {} on {}.".format(port, hostname))
+    logger.info("Starting the server on port {} on {}.".format(port, hostname))
     signal.signal(signal.SIGINT, lambda signum, frame: t.close())
     signal.signal(signal.SIGTERM, lambda signum, frame: t.close())
 
     t.start()
 
 
 def create_session(server_name, client_port=None, launch_aedt_on_server=False, aedt_port=None, non_graphical=True):
```

### Comparing `pyaedt-0.6.78/pyaedt/desktop.py` & `pyaedt-0.6.79/pyaedt/desktop.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 pyaedtversion = __version__
 
 modules = [tup[1] for tup in pkgutil.iter_modules()]
 
 if is_ironpython:
     _com = "ironpython"
-elif is_windows and "pythonnet" in modules:  # pragma: no cover
+elif is_windows and "pythonnet" in modules:
     _com = "pythonnet_v3"
 else:
     _com = "gprc_v3"
     settings.use_grpc_api = True
 
 
 @pyaedt_function_handler()
@@ -1319,14 +1319,24 @@
         >>> desktop = pyaedt.Desktop("2021.2")
         PyAEDT INFO: pyaedt v...
         PyAEDT INFO: Python version ...
         >>> desktop.release_desktop(close_projects=False, close_on_exit=False) # doctest: +SKIP
 
         """
         result = release_desktop(close_projects, close_on_exit)
+        props = [a for a in dir(self) if not a.startswith("__")]
+        for a in props:
+            self.__dict__.pop(a, None)
+        dicts = [self, sys.modules["__main__"]]
+        for dict_to_clean in dicts:
+            props = [a for a in dir(dict_to_clean) if "win32com" in str(type(dict_to_clean.__dict__.get(a, None)))]
+            for a in props:
+                dict_to_clean.__dict__[a] = None
+
+        gc.collect()
         self.odesktop = None
         return result
 
     def close_desktop(self):
         """Close all projects and shut down AEDT.
 
         Returns
```

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.79/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/downloads.py` & `pyaedt-0.6.79/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb.py` & `pyaedt-0.6.79/pyaedt/edb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """This module contains the ``Edb`` class.
 
 This module is implicitily loaded in HFSS 3D Layout when launched.
 
 """
 from itertools import combinations
 import os
-import re
 import shutil
 import sys
 import tempfile
 import time
 import traceback
 import warnings
 
-from pyaedt import __version__
-from pyaedt import pyaedt_logger
 from pyaedt import settings
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.edb_core import Components
 from pyaedt.edb_core import EdbHfss
 from pyaedt.edb_core import EdbLayout
 from pyaedt.edb_core import EdbNets
 from pyaedt.edb_core import EdbSiwave
+from pyaedt.edb_core.dotnet.database import Database
+from pyaedt.edb_core.dotnet.layout import LayoutDotNet
 from pyaedt.edb_core.edb_data.control_file import ControlFile
 from pyaedt.edb_core.edb_data.control_file import convert_technology_file
 from pyaedt.edb_core.edb_data.design_options import EdbDesignOptions
-from pyaedt.edb_core.edb_data.edb_builder import EdbBuilder
 from pyaedt.edb_core.edb_data.edbvalue import EdbValue
 from pyaedt.edb_core.edb_data.hfss_simulation_setup_data import HfssSimulationSetup
 from pyaedt.edb_core.edb_data.simulation_configuration import SimulationConfiguration
 from pyaedt.edb_core.edb_data.siwave_simulation_setup_data import SiwaveDCSimulationSetup
 from pyaedt.edb_core.edb_data.siwave_simulation_setup_data import SiwaveSYZSimulationSetup
 from pyaedt.edb_core.edb_data.sources import ExcitationDifferential
 from pyaedt.edb_core.edb_data.sources import ExcitationPorts
@@ -39,43 +37,35 @@
 from pyaedt.edb_core.edb_data.variables import Variable
 import pyaedt.edb_core.general
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.edb_core.ipc2581.ipc2581 import Ipc2581
 from pyaedt.edb_core.materials import Materials
 from pyaedt.edb_core.padstack import EdbPadstacks
 from pyaedt.edb_core.stackup import Stackup
-from pyaedt.generic.clr_module import Convert
-from pyaedt.generic.clr_module import List
-from pyaedt.generic.clr_module import Tuple
-from pyaedt.generic.clr_module import _clr
-from pyaedt.generic.clr_module import edb_initialized
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import SolverType
-
-# from pyaedt.generic.general_methods import property
-from pyaedt.generic.general_methods import env_path
-from pyaedt.generic.general_methods import env_path_student
-from pyaedt.generic.general_methods import env_value
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
 from pyaedt.generic.general_methods import is_windows
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.process import SiwaveSolve
-from pyaedt.misc.misc import list_installed_ansysem
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
+# from pyaedt.generic.general_methods import property
+
+
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
 else:
     import subprocess
 
 
-class Edb(object):
+class Edb(Database):
     """Provides the EDB application interface.
 
     This module inherits all objects that belong to EDB.
 
     Parameters
     ----------
     edbpath : str, optional
@@ -145,98 +135,76 @@
         isaedtowned=False,
         oproject=None,
         student_version=False,
         use_ppe=False,
         technology_file=None,
     ):
         self._clean_variables()
-        # if inside_desktop:
-        #    self.standalone = False
-        # else:
+
+        Database.__init__(self, edbversion, student_version)
         self.standalone = True
-        if edb_initialized:
-            self.oproject = oproject
-            self._main = sys.modules["__main__"]
-            self._global_logger = pyaedt_logger
-            self._logger = pyaedt_logger
-            self.student_version = student_version
-            if settings.enable_screen_logs:
-                self.logger.enable_stdout_log()
-            else:
-                self.logger.disable_stdout_log()
-            self.logger.info("Logger is initialized in EDB.")
-            self.logger.info("pyaedt v%s", __version__)
-            self.logger.info("Python version %s", sys.version)
-            if not edbversion:
-                try:
-                    edbversion = "20{}.{}".format(list_installed_ansysem()[0][-3:-1], list_installed_ansysem()[0][-1:])
-                    self._logger.info("Edb version " + edbversion)
-                except IndexError:
-                    raise Exception("No ANSYSEM_ROOTxxx is found.")
-            self.edbversion = edbversion
-            self.isaedtowned = isaedtowned
-            self._init_dlls()
-            self._db = None
-            self.isreadonly = isreadonly
-            self.cellname = cellname
-            if not edbpath:
-                if is_windows:
-                    edbpath = os.getenv("USERPROFILE")
-                    if not edbpath:
-                        edbpath = os.path.expanduser("~")
-                    edbpath = os.path.join(edbpath, "Documents", generate_unique_name("layout") + ".aedb")
+        self.oproject = oproject
+        self._main = sys.modules["__main__"]
+        self.edbversion = edbversion
+        self.isaedtowned = isaedtowned
+        self.isreadonly = isreadonly
+        self.cellname = cellname
+        if not edbpath:
+            if is_windows:
+                edbpath = os.getenv("USERPROFILE")
+                if not edbpath:
+                    edbpath = os.path.expanduser("~")
+                edbpath = os.path.join(edbpath, "Documents", generate_unique_name("layout") + ".aedb")
+            else:
+                edbpath = os.getenv("HOME")
+                if not edbpath:
+                    edbpath = os.path.expanduser("~")
+                edbpath = os.path.join(edbpath, generate_unique_name("layout") + ".aedb")
+            self.logger.info("No EDB is provided. Creating a new EDB {}.".format(edbpath))
+        self.edbpath = edbpath
+        self.log_name = None
+        if edbpath:
+            self.log_name = os.path.join(
+                os.path.dirname(edbpath), "pyaedt_" + os.path.splitext(os.path.split(edbpath)[-1])[0] + ".log"
+            )
+
+        if isaedtowned and (inside_desktop or settings.remote_api):
+            self.open_edb_inside_aedt()
+        elif edbpath[-3:] in ["brd", "gds", "xml", "dxf", "tgz"]:
+            self.edbpath = edbpath[:-4] + ".aedb"
+            working_dir = os.path.dirname(edbpath)
+            control_file = None
+            if technology_file:
+                if os.path.splitext(technology_file)[1] == ".xml":
+                    control_file = technology_file
                 else:
-                    edbpath = os.getenv("HOME")
-                    if not edbpath:
-                        edbpath = os.path.expanduser("~")
-                    edbpath = os.path.join(edbpath, generate_unique_name("layout") + ".aedb")
-                self.logger.info("No EDB is provided. Creating a new EDB {}.".format(edbpath))
+                    control_file = convert_technology_file(technology_file, edbversion=edbversion)
+            self.import_layout_pcb(edbpath, working_dir, use_ppe=use_ppe, control_file=control_file)
+            if settings.enable_local_log_file and self.log_name:
+                self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
+            self.logger.info("EDB %s was created correctly from %s file.", self.edbpath, edbpath[-2:])
+        elif edbpath.endswith("edb.def"):
+            self.edbpath = os.path.dirname(edbpath)
+            if settings.enable_local_log_file and self.log_name:
+                self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
+            self.open_edb()
+        elif not os.path.exists(os.path.join(self.edbpath, "edb.def")):
+            self.create_edb()
+            if settings.enable_local_log_file and self.log_name:
+                self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
+            self.logger.info("EDB %s was created correctly.", self.edbpath)
+        elif ".aedb" in edbpath:
             self.edbpath = edbpath
-            self.log_name = None
-            if edbpath:
-                self.log_name = os.path.join(
-                    os.path.dirname(edbpath), "pyaedt_" + os.path.splitext(os.path.split(edbpath)[-1])[0] + ".log"
-                )
-
-            if isaedtowned and (inside_desktop or settings.remote_api):
-                self.open_edb_inside_aedt()
-            elif edbpath[-3:] in ["brd", "gds", "xml", "dxf", "tgz"]:
-                self.edbpath = edbpath[:-4] + ".aedb"
-                working_dir = os.path.dirname(edbpath)
-                control_file = None
-                if technology_file:
-                    if os.path.splitext(technology_file)[1] == ".xml":
-                        control_file = technology_file
-                    else:
-                        control_file = convert_technology_file(technology_file, edbversion=edbversion)
-                self.import_layout_pcb(edbpath, working_dir, use_ppe=use_ppe, control_file=control_file)
-                if settings.enable_local_log_file and self.log_name:
-                    self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
-                self.logger.info("EDB %s was created correctly from %s file.", self.edbpath, edbpath[-2:])
-            elif edbpath.endswith("edb.def"):
-                self.edbpath = os.path.dirname(edbpath)
-                if settings.enable_local_log_file and self.log_name:
-                    self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
-                self.open_edb()
-            elif not os.path.exists(os.path.join(self.edbpath, "edb.def")):
-                self.create_edb()
-                if settings.enable_local_log_file and self.log_name:
-                    self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
-                self.logger.info("EDB %s was created correctly.", self.edbpath)
-            elif ".aedb" in edbpath:
-                self.edbpath = edbpath
-                if settings.enable_local_log_file and self.log_name:
-                    self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
-                self.open_edb()
-            if self.builder:
-                self.logger.info("EDB was initialized.")
-            else:
-                self.logger.info("Failed to initialize DLLs.")
+            if settings.enable_local_log_file and self.log_name:
+                self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
+            self.open_edb()
+        if self.active_cell:
+            self.logger.info("EDB was initialized.")
         else:
-            warnings.warn("Failed to initialize DLLs.")
+            self.logger.info("Failed to initialize DLLs.")
 
     def __enter__(self):
         return self
 
     def __exit__(self, ex_type, ex_value, ex_traceback):
         if ex_type:
             self.edb_exception(ex_value, ex_traceback)
@@ -280,31 +248,28 @@
         else:
             self.add_design_variable(variable_name, val)
         if description:  # Add the variable description if a two-item list is passed for variable_value.
             self.__getitem__(variable_name).description = description
 
     def _clean_variables(self):
         """Initialize internal variables and perform garbage collection."""
-
+        self._materials = None
         self._components = None
         self._core_primitives = None
         self._stackup = None
+        self._stackup2 = None
         self._padstack = None
         self._siwave = None
         self._hfss = None
         self._nets = None
-        self._db = None
-        self._edb = None
-        self.builder = None
-        self.edbutils = None
-        self.simSetup = None
-        self.simsetupdata = None
         self._setups = {}
         self._layout_instance = None
         self._variables = None
+        self._active_cell = None
+        self._layout = None
         # time.sleep(2)
         # gc.collect()
 
     @pyaedt_function_handler()
     def _init_objects(self):
         self._components = Components(self)
         self._stackup = Stackup(self)
@@ -315,87 +280,25 @@
         self._core_primitives = EdbLayout(self)
         self._stackup2 = self._stackup
         self._materials = Materials(self)
 
         self.logger.info("Objects Initialized")
 
     @property
-    def logger(self):
-        """Logger for EDB.
-
-        Returns
-        -------
-        :class:`pyaedt.aedt_logger.AedtLogger`
-        """
-        return self._logger
-
-    @property
     def cell_names(self):
         """Cell name container.
         Returns
         -------
         list of str, cell names.
         """
         names = []
-        for cell in list(self._db.CircuitCells):
+        for cell in self.circuit_cells:
             names.append(cell.GetName())
         return names
 
-    @pyaedt_function_handler()
-    def _init_dlls(self):
-        """Initialize DLLs."""
-        if is_linux:
-            if env_value(self.edbversion) in os.environ or settings.edb_dll_path:
-                if settings.edb_dll_path:
-                    self.base_path = settings.edb_dll_path
-                else:
-                    self.base_path = env_path(self.edbversion)
-                sys.path.append(self.base_path)
-            else:
-                main = sys.modules["__main__"]
-                if "oDesktop" in dir(main):
-                    self.base_path = main.oDesktop.GetExeDir()
-                    sys.path.append(main.oDesktop.GetExeDir())
-                    os.environ[env_value(self.edbversion)] = self.base_path
-                else:
-                    edb_path = os.getenv("PYAEDT_SERVER_AEDT_PATH")
-                    if edb_path:
-                        self.base_path = edb_path
-                        sys.path.append(edb_path)
-                        os.environ[env_value(self.edbversion)] = self.base_path
-            if is_ironpython:
-                _clr.AddReferenceToFile("Ansys.Ansoft.Edb.dll")
-                _clr.AddReferenceToFile("Ansys.Ansoft.EdbBuilderUtils.dll")
-                _clr.AddReferenceToFileAndPath(os.path.join(self.base_path, "Ansys.Ansoft.SimSetupData.dll"))
-            else:
-                _clr.AddReference("Ansys.Ansoft.Edb")
-                _clr.AddReference("Ansys.Ansoft.EdbBuilderUtils")
-                _clr.AddReference("Ansys.Ansoft.SimSetupData")
-        else:
-            if settings.edb_dll_path:
-                self.base_path = settings.edb_dll_path
-            elif self.student_version:
-                self.base_path = env_path_student(self.edbversion)
-            else:
-                self.base_path = env_path(self.edbversion)
-            sys.path.append(self.base_path)
-            _clr.AddReference("Ansys.Ansoft.Edb")
-            _clr.AddReference("Ansys.Ansoft.EdbBuilderUtils")
-            _clr.AddReference("Ansys.Ansoft.SimSetupData")
-        os.environ["ECAD_TRANSLATORS_INSTALL_DIR"] = self.base_path
-        oaDirectory = os.path.join(self.base_path, "common", "oa")
-        os.environ["ANSYS_OADIR"] = oaDirectory
-        os.environ["PATH"] = "{};{}".format(os.environ["PATH"], self.base_path)
-        edb = __import__("Ansys.Ansoft.Edb")
-        self.edb = edb.Ansoft.Edb
-        edbbuilder = __import__("Ansys.Ansoft.EdbBuilderUtils")
-        self.edbutils = edbbuilder.Ansoft.EdbBuilderUtils
-        self.simSetup = __import__("Ansys.Ansoft.SimSetupData")
-        self.simsetupdata = self.simSetup.Ansoft.SimSetupData.Data
-
     @property
     def design_variables(self):
         """Get all edb design variables.
 
         Returns
         -------
         Dict[str, :class:`pyaedt.edb_core.edb_data.variables.Variable`]
@@ -411,15 +314,15 @@
 
         Returns
         -------
         Dict[str, :class:`pyaedt.edb_core.edb_data.variables.Variable`]
 
         """
         p_var = dict()
-        for i in self.db.GetVariableServer().GetAllVariableNames():
+        for i in self.active_db.GetVariableServer().GetAllVariableNames():
             p_var[i] = Variable(self, i)
         return p_var
 
     @property
     def variables(self):
         """Get all Edb variables.
 
@@ -434,196 +337,151 @@
         for i, j in self.design_variables.items():
             all_vars[i] = j
         return all_vars
 
     @property
     def excitations(self):
         """Get all layout excitations."""
-        terms = [term for term in list(self._active_layout.Terminals) if int(term.GetBoundaryType()) == 0]
+        terms = [term for term in self.layout.terminals if int(term.GetBoundaryType()) == 0]
         terms = [i for i in terms if not i.IsReferenceTerminal()]
         temp = {}
         for ter in terms:
             if "BundleTerminal" in ter.GetType().ToString():
                 temp[ter.GetName()] = ExcitationDifferential(self, ter)
             else:
                 temp[ter.GetName()] = ExcitationPorts(self, ter)
         return temp
 
     @property
     def excitations_nets(self):
         """Get all excitations net names."""
-        return list(set([i.GetNet().GetName() for i in list(self._active_layout.Terminals)]))
+        return list(set([i.GetNet().GetName() for i in self.layout.terminals]))
 
     @property
     def sources(self):
         """Get all layout sources."""
-        terms = [term for term in list(self._active_layout.Terminals) if int(term.GetBoundaryType()) in [3, 4, 7]]
+        terms = [term for term in self.layout.terminals if int(term.GetBoundaryType()) in [3, 4, 7]]
         return {ter.GetName(): ExcitationSources(self, ter) for ter in terms}
 
     @property
     def probes(self):
         """Get all layout sources."""
-        terms = [term for term in list(self._active_layout.Terminals) if int(term.GetBoundaryType()) in [8]]
+        terms = [term for term in self.layout.terminals if int(term.GetBoundaryType()) in [8]]
         return {ter.GetName(): ExcitationProbes(self, ter) for ter in terms}
 
     @pyaedt_function_handler()
-    def open_edb(self, init_dlls=False):
+    def open_edb(self):
         """Open EDB.
 
-        Parameters
-        ----------
-        init_dlls : bool, optional
-            Whether to initialize DLLs. The default is ``False``.
-
         Returns
         -------
 
         """
-        if init_dlls:
-            self._init_dlls()
         # self.logger.info("EDB Path is %s", self.edbpath)
         # self.logger.info("EDB Version is %s", self.edbversion)
         # if self.edbversion > "2023.1":
         #     self.standalone = False
 
-        self.edb.Database.SetRunAsStandAlone(self.standalone)
+        self.run_as_standalone(self.standalone)
 
         # self.logger.info("EDB Standalone %s", self.standalone)
         try:
-            db = self.edb.Database.Open(self.edbpath, self.isreadonly)
+            self.open(self.edbpath, self.isreadonly)
         except Exception as e:
-            db = None
             self.logger.error("Builder is not Initialized.")
-        if not db:
+        if not self.active_db:
             self.logger.warning("Error Opening db")
-            self._db = None
             self._active_cell = None
-            self.builder = None
             return None
-        self._db = db
         self.logger.info("Database {} Opened in {}".format(os.path.split(self.edbpath)[-1], self.edbversion))
 
         self._active_cell = None
         if self.cellname:
-            for cell in list(self._db.TopCircuitCells):
+            for cell in list(self.top_circuit_cells):
                 if cell.GetName() == self.cellname:
                     self._active_cell = cell
         # if self._active_cell is still None, set it to default cell
         if self._active_cell is None:
-            self._active_cell = list(self._db.TopCircuitCells)[0]
+            self._active_cell = list(self.top_circuit_cells)[0]
         self.logger.info("Cell %s Opened", self._active_cell.GetName())
-        if self._db and self._active_cell:
-            self.builder = EdbBuilder(self.edbutils, self._db, self._active_cell)
+        if self._active_cell:
             self._init_objects()
             self.logger.info("Builder was initialized.")
         else:
-            self.builder = None
             self.logger.error("Builder was not initialized.")
 
-        return self.builder
+        return True
 
     @pyaedt_function_handler()
-    def open_edb_inside_aedt(self, init_dlls=False):
+    def open_edb_inside_aedt(self):
         """Open EDB inside of AEDT.
 
-        Parameters
-        ----------
-        init_dlls : bool, optional
-            Whether to initialize DLLs. The default is ``False``.
-
         Returns
         -------
 
         """
-        if init_dlls:
-            self._init_dlls()
         self.logger.info("Opening EDB from HDL")
-        self.edb.Database.SetRunAsStandAlone(False)
+        self.run_as_standalone(False)
         if self.oproject.GetEDBHandle():
-            hdl = Convert.ToUInt64(self.oproject.GetEDBHandle())
-            db = self.edb.Database.Attach(hdl)
-            if not db:
+            self.attach(self.oproject.GetEDBHandle())
+            if not self.active_db:
                 self.logger.warning("Error getting the database.")
-                self._db = None
                 self._active_cell = None
-                self.builder = None
                 return None
-            self._db = db
-            self._active_cell = self.edb.Cell.Cell.FindByName(
-                self.db, self.edb.Cell.CellType.CircuitCell, self.cellname
+            self._active_cell = self.edb_api.cell.cell.FindByName(
+                self.active_db, self.edb_api.cell._cell.CellType.CircuitCell, self.cellname
             )
             if self._active_cell is None:
-                self._active_cell = list(self._db.TopCircuitCells)[0]
-            if self._db and self._active_cell:
+                self._active_cell = list(self.top_circuit_cells)[0]
+            if self._active_cell:
                 if not os.path.exists(self.edbpath):
                     os.makedirs(self.edbpath)
-                time.sleep(3)
-                self.builder = EdbBuilder(self.edbutils, self._db, self._active_cell)
                 self._init_objects()
-                return self.builder
+                return True
             else:
-                self.builder = None
                 return None
         else:
-            self._db = None
             self._active_cell = None
-            self.builder = None
             return None
 
     @pyaedt_function_handler()
-    def create_edb(self, init_dlls=False):
-        """Create EDB.
-
-        Parameters
-        ----------
-        init_dlls : bool, optional
-            Whether to initialize DLLs. The default is ``False``.
-
-        """
-        if init_dlls:
-            self._init_dlls()
+    def create_edb(self):
+        """Create EDB."""
         # if self.edbversion > "2023.1":
         #     self.standalone = False
 
-        self.edb.Database.SetRunAsStandAlone(self.standalone)
-        db = self.edb.Database.Create(self.edbpath)
-        if not db:
+        self.run_as_standalone(self.standalone)
+        self.create(self.edbpath)
+        if not self.active_db:
             self.logger.warning("Error creating the database.")
-            self._db = None
             self._active_cell = None
-            self.builder = None
             return None
-        self._db = db
         if not self.cellname:
             self.cellname = generate_unique_name("Cell")
-        self._active_cell = self.edb.Cell.Cell.Create(self._db, self.edb.Cell.CellType.CircuitCell, self.cellname)
-        if self._db and self._active_cell:
-            self.builder = EdbBuilder(self.edbutils, self._db, self._active_cell)
+        self._active_cell = self.edb_api.cell.create(
+            self.active_db, self.edb_api.cell.CellType.CircuitCell, self.cellname
+        )
+        if self._active_cell:
             self._init_objects()
-            return self.builder
-        self.builder = None
+            return True
         return None
 
     @pyaedt_function_handler()
-    def import_layout_pcb(
-        self, input_file, working_dir, init_dlls=False, anstranslator_full_path="", use_ppe=False, control_file=None
-    ):
+    def import_layout_pcb(self, input_file, working_dir, anstranslator_full_path="", use_ppe=False, control_file=None):
         """Import a board file and generate an ``edb.def`` file in the working directory.
 
         This function supports all AEDT formats, including DXF, GDS, SML (IPC2581), BRD, and TGZ.
 
         Parameters
         ----------
         input_file : str
             Full path to the board file.
         working_dir : str
             Directory in which to create the ``aedb`` folder. The name given to the AEDB file
             is the same as the name of the board file.
-        init_dlls : bool
-            Whether to initialize DLLs. The default is ``False``.
         anstranslator_full_path : str, optional
             Full path to the Ansys translator. The default is ``""``.
         use_ppe : bool
             Whether to use the PPE License. The default is ``False``.
         control_file : str, optional
             Path to the XML file. The default is ``None``, in which case an attempt is made to find
             the XML file in the same directory as the board file. To succeed, the XML file and board file
@@ -637,17 +495,14 @@
         self._components = None
         self._core_primitives = None
         self._stackup = None
         self._padstack = None
         self._siwave = None
         self._hfss = None
         self._nets = None
-        self._db = None
-        if init_dlls:
-            self._init_dlls()
         aedb_name = os.path.splitext(os.path.basename(input_file))[0] + ".aedb"
         if anstranslator_full_path and os.path.exists(anstranslator_full_path):
             command = anstranslator_full_path
         else:
             command = os.path.join(self.base_path, "anstranslator")
             if is_windows:
                 command += ".exe"
@@ -746,17 +601,17 @@
         tb_trace = traceback.format_tb(tb_data)
         tblist = tb_trace[0].split("\n")
         self.logger.error(str(ex_value))
         for el in tblist:
             self.logger.error(el)
 
     @property
-    def db(self):
+    def active_db(self):
         """Database object."""
-        return self._db
+        return self.db
 
     @property
     def active_cell(self):
         """Active cell."""
         return self._active_cell
 
     @property
@@ -787,30 +642,30 @@
         :class:`pyaedt.edb_core.Components.Components`
 
         Examples
         --------
         >>> edbapp = pyaedt.Edb("myproject.aedb")
         >>> comp = self.edbapp.components.get_component_by_name("J1")
         """
-        if not self._components and self.builder:
+        if not self._components and self.active_db:
             self._components = Components(self)
         return self._components
 
     @property
     def core_stackup(self):
         """Core stackup.
 
         .. deprecated:: 0.6.5
             There is no need to use the ``core_stackup`` property anymore.
             You can instantiate a new ``stackup`` class directly from the ``Edb`` class.
         """
         mess = "`core_stackup` is deprecated.\n"
         mess += " Use `app.stackup` directly to instantiate new stackup methods."
         warnings.warn(mess, DeprecationWarning)
-        if not self._stackup and self.builder:
+        if not self._stackup and self.active_db:
             self._stackup = Stackup(self)
         return self._stackup
 
     @property
     def design_options(self):
         """Edb Design Settings and Options.
 
@@ -831,15 +686,15 @@
         Examples
         --------
         >>> edbapp = pyaedt.Edb("myproject.aedb")
         >>> edbapp.stackup.layers["TOP"].thickness = 4e-5
         >>> edbapp.stackup.layers["TOP"].thickness == 4e-05
         >>> edbapp.stackup.add_layer("Diel", "GND", layer_type="dielectric", thickness="0.1mm", material="FR4_epoxy")
         """
-        if not self._stackup2 and self.builder:
+        if not self._stackup2 and self.active_db:
             self._stackup2 = Stackup(self)
         return self._stackup2
 
     @property
     def materials(self):
         """Material Database.
 
@@ -851,15 +706,15 @@
         --------
         >>> edbapp = pyaedt.Edb("myproject.aedb")
         >>> edbapp.materials["FR4_epoxy"].conductivity = 1
         >>> edbapp.materials.add_debye_material("My_Debye2", 5, 3, 0.02, 0.05, 1e5, 1e9)
         >>> edbapp.materials.add_djordjevicsarkar_material("MyDjord2", 3.3, 0.02, 3.3)
         """
 
-        if not self._materials and self.builder:
+        if not self._materials and self.active_db:
             self._materials = Materials(self)
         return self._materials
 
     @property
     def core_padstack(self):  # pragma: no cover
         """Core padstack.
 
@@ -897,15 +752,15 @@
         >>> edbapp = pyaedt.Edb("myproject.aedb")
         >>> p = edbapp.padstacks.create(padstackname="myVia_bullet", antipad_shape="Bullet")
         >>> edbapp.padstacks.get_pad_parameters(
         >>> ... p, "TOP", self.edbapp.padstacks.pad_type.RegularPad
         >>> ... )
         """
 
-        if not self._padstack and self.builder:
+        if not self._padstack and self.active_db:
             self._padstack = EdbPadstacks(self)
         return self._padstack
 
     @property
     def core_siwave(self):  # pragma: no cover
         """Core SIWave methods and properties.
 
@@ -933,15 +788,15 @@
         Instance of :class: `pyaedt.edb_core.siwave.EdbSiwave`
 
         Examples
         --------
         >>> edbapp = pyaedt.Edb("myproject.aedb")
         >>> p2 = edbapp.siwave.create_circuit_port_on_net("U2A5", "V3P3_S0", "U2A5", "GND", 50, "test")
         """
-        if not self._siwave and self.builder:
+        if not self._siwave and self.active_db:
             self._siwave = EdbSiwave(self)
         return self._siwave
 
     @property
     def core_hfss(self):  # pragma: no cover
         """Core HFSS methods and properties.
 
@@ -969,15 +824,15 @@
         :class:`pyaedt.edb_core.hfss.EdbHfss`
 
         Examples
         --------
         >>> edbapp = pyaedt.Edb("myproject.aedb")
         >>> edbapp.hfss.configure_hfss_analysis_setup(sim_config)
         """
-        if not self._hfss and self.builder:
+        if not self._hfss and self.active_db:
             self._hfss = EdbHfss(self)
         return self._hfss
 
     @property
     def core_nets(self):  # pragma: no cover
         """Core nets.
 
@@ -1008,15 +863,15 @@
         Examples
         --------
         >>> edbapp = pyaedt.Edb("myproject.aedb")
         >>> edbapp.nets.find_or_create_net("GND")
         >>> edbapp.nets.find_and_fix_disjoint_nets("GND", keep_only_main_net=True)
         """
 
-        if not self._nets and self.builder:
+        if not self._nets and self.active_db:
             self._nets = EdbNets(self)
         return self._nets
 
     @property
     def core_primitives(self):  # pragma: no cover
         """Core primitives.
 
@@ -1045,37 +900,42 @@
         Instance of :class: `pyaedt.edb_core.layout.EdbLayout`
 
         Examples
         --------
         >>> edbapp = pyaedt.Edb("myproject.aedb")
         >>> top_prims = edbapp.modeler.primitives_by_layer["TOP"]
         """
-        if not self._core_primitives and self.builder:
+        if not self._core_primitives and self.active_db:
             self._core_primitives = EdbLayout(self)
         return self._core_primitives
 
     @property
+    def layout(self):
+        """Layout object.
+
+        Returns
+        -------
+        :class:`pyaedt.edb_core.dotnet.layout.Layout`
+        """
+        return LayoutDotNet(self)
+
+    @property
     def active_layout(self):
         """Active layout.
 
         Returns
         -------
-        Instance of :class: `pyaedt.`
+        Instance of EDB API Layout Class.
         """
-        self._active_layout = None
-        if self._active_cell:
-            self._active_layout = self.active_cell.GetLayout()
-        return self._active_layout
+        return self.layout._layout
 
     @property
     def layout_instance(self):
         """Edb Layout Instance."""
-        if not self._layout_instance:
-            self._layout_instance = self.active_layout.GetLayoutInstance()
-        return self._layout_instance
+        return self.layout.layout_instance
 
     @property
     def pins(self):
         """EDBPadstackInstance of Component.
 
         .. deprecated:: 0.6.62
            Use new method :func:`edb.padstacks.pins` instead.
@@ -1114,32 +974,15 @@
 
 
         Returns
         -------
         Instance of `Edb.Utility.Value`
 
         """
-        if isinstance(val, self.edb.Utility.Value):
-            return val
-        if isinstance(val, (int, float)):
-            return self.edb.Utility.Value(val)
-        m1 = re.findall(r"(?<=[/+-/*//^/(/[])([a-z_A-Z/$]\w*)", str(val).replace(" ", ""))
-        m2 = re.findall(r"^([a-z_A-Z/$]\w*)", str(val).replace(" ", ""))
-        val_decomposed = list(set(m1).union(m2))
-        if not val_decomposed:
-            return self.edb.Utility.Value(val)
-        var_server_db = self.db.GetVariableServer()
-        var_names = var_server_db.GetAllVariableNames()
-        var_server_cell = self.active_cell.GetVariableServer()
-        var_names_cell = var_server_cell.GetAllVariableNames()
-        if set(val_decomposed).intersection(var_names_cell):
-            return self.edb.Utility.Value(val, var_server_cell)
-        if set(val_decomposed).intersection(var_names):
-            return self.edb.Utility.Value(val, var_server_db)
-        return self.edb.Utility.Value(val)
+        return self.edb_api.utility.value(val)
 
     @pyaedt_function_handler()
     def point_3d(self, x, y, z=0.0):
         """Compute the Edb 3d Point Data.
 
         Parameters
         ----------
@@ -1150,15 +993,15 @@
         z : float, int or str, optional
             Z value.
 
         Returns
         -------
         ``Geometry.Point3DData``.
         """
-        return self.edb.Geometry.Point3DData(self.edb_value(x), self.edb_value(y), self.edb_value(z))
+        return self.edb_api.geometry.point3d_data(x, y, z)
 
     @pyaedt_function_handler()
     def point_data(self, x, y=None):
         """Compute the Edb Point Data.
 
         Parameters
         ----------
@@ -1169,17 +1012,17 @@
 
 
         Returns
         -------
         ``Geometry.PointData``.
         """
         if y is None:
-            return self.edb.Geometry.PointData(self.edb_value(x))
+            return self.edb_api.geometry.point_data(x)
         else:
-            return self.edb.Geometry.PointData(self.edb_value(x), self.edb_value(y))
+            return self.edb_api.geometry.point_data(x, y)
 
     @pyaedt_function_handler()
     def _is_file_existing_and_released(self, filename):
         if os.path.exists(filename):
             try:
                 os.rename(filename, filename + "_")
                 os.rename(filename + "_", filename)
@@ -1234,15 +1077,15 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        self._db.Close()
+        self.close()
         if self.log_name and settings.enable_local_log_file:
             self._global_logger.remove_file_logger(os.path.splitext(os.path.split(self.log_name)[-1])[0])
             self._logger = self._global_logger
         start_time = time.time()
         self._wait_for_file_release()
         elapsed_time = time.time() - start_time
         self.logger.info("EDB file release time: {0:.2f}ms".format(elapsed_time * 1000.0))
@@ -1255,15 +1098,15 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        self._db.Save()
+        self.save()
         start_time = time.time()
         self._wait_for_file_release()
         elapsed_time = time.time() - start_time
         self.logger.info("EDB file save time: {0:.2f}ms".format(elapsed_time * 1000.0))
         return True
 
     @pyaedt_function_handler()
@@ -1277,20 +1120,20 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        self._db.SaveAs(fname)
+        self.save_as(fname)
         start_time = time.time()
         self._wait_for_file_release()
         elapsed_time = time.time() - start_time
         self.logger.info("EDB file save time: {0:.2f}ms".format(elapsed_time * 1000.0))
-        self.edbpath = self._db.GetDirectory()
+        self.edbpath = self.directory
         if self.log_name:
             self._global_logger.remove_file_logger(os.path.splitext(os.path.split(self.log_name)[-1])[0])
             self._logger = self._global_logger
 
         self.log_name = os.path.join(
             os.path.dirname(fname), "pyaedt_" + os.path.splitext(os.path.split(fname)[-1])[0] + ".log"
         )
@@ -1310,15 +1153,15 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        return self.edb.Utility.Command.Execute(func)
+        return self.edb_api.utility.utility.Command.Execute(func)
 
     @pyaedt_function_handler()
     def import_cadence_file(self, inputBrd, WorkDir=None, anstranslator_full_path="", use_ppe=False):
         """Import a board file and generate an ``edb.def`` file in the working directory.
 
         Parameters
         ----------
@@ -1416,52 +1259,62 @@
         expansion_size,
         use_round_corner,
         use_pyaedt_extent=False,
         smart_cut=False,
         reference_list=[],
         include_pingroups=True,
     ):
-        if extent_type in ["Conforming", self.edb.Geometry.ExtentType.Conforming, 1]:
+        if extent_type in ["Conforming", self.edb_api.geometry.extent_type.Conforming, 1]:
             if use_pyaedt_extent:
                 _poly = self._create_conformal(
                     net_signals,
                     expansion_size,
                     1e-12,
                     use_round_corner,
                     expansion_size,
                     smart_cut,
                     reference_list,
                     include_pingroups,
                 )
             else:
-                _poly = self.active_layout.GetExpandedExtentFromNets(
-                    net_signals, self.edb.Geometry.ExtentType.Conforming, expansion_size, False, use_round_corner, 1
+                _poly = self.layout.expanded_extent(
+                    net_signals,
+                    self.edb_api.geometry.extent_type.Conforming,
+                    expansion_size,
+                    False,
+                    use_round_corner,
+                    1,
                 )
-        elif extent_type in ["Bounding", self.edb.Geometry.ExtentType.BoundingBox, 0]:
-            _poly = self.active_layout.GetExpandedExtentFromNets(
-                net_signals, self.edb.Geometry.ExtentType.BoundingBox, expansion_size, False, use_round_corner, 1
+        elif extent_type in ["Bounding", self.edb_api.geometry.extent_type.BoundingBox, 0]:
+            _poly = self.layout.expanded_extent(
+                net_signals, self.edb_api.geometry.extent_type.BoundingBox, expansion_size, False, use_round_corner, 1
             )
         else:
             if use_pyaedt_extent:
                 _poly = self._create_convex_hull(
                     net_signals,
                     expansion_size,
                     1e-12,
                     use_round_corner,
                     expansion_size,
                     smart_cut,
                     reference_list,
                     include_pingroups,
                 )
             else:
-                _poly = self.active_layout.GetExpandedExtentFromNets(
-                    net_signals, self.edb.Geometry.ExtentType.Conforming, expansion_size, False, use_round_corner, 1
+                _poly = self.layout.expanded_extent(
+                    net_signals,
+                    self.edb_api.geometry.extent_type.Conforming,
+                    expansion_size,
+                    False,
+                    use_round_corner,
+                    1,
                 )
                 _poly_list = convert_py_list_to_net_list([_poly])
-                _poly = self.edb.Geometry.PolygonData.GetConvexHullOfPolygons(_poly_list)
+                _poly = self.edb_api.geometry.polygon_data.get_convex_hull_of_polygons(_poly_list)
         return _poly
 
     @pyaedt_function_handler()
     def _create_conformal(
         self,
         net_signals,
         expansion_size,
@@ -1481,43 +1334,50 @@
                 obj_data = prim.primitive_object.GetPolygonData().Expand(
                     expansion_size, tolerance, round_corner, round_extension
                 )
                 if obj_data:
                     _polys.extend(list(obj_data))
         if smart_cutout:
             _polys.extend(self._smart_cut(net_signals, reference_list, include_pingroups))
-        _poly_unite = list(self.edb.Geometry.PolygonData.Unite(convert_py_list_to_net_list(_polys)))
+        _poly_unite = self.edb_api.geometry.polygon_data.unite(_polys)
         if len(_poly_unite) == 1:
             return _poly_unite[0]
         else:
             areas = [i.Area() for i in _poly_unite]
             return _poly_unite[areas.index(max(areas))]
 
     @pyaedt_function_handler()
     def _smart_cut(self, net_signals, reference_list=[], include_pingroups=True):
         _polys = []
-        terms = [term for term in list(self.active_layout.Terminals) if int(term.GetBoundaryType()) in [0, 3, 4, 7, 8]]
+        terms = [term for term in self.layout.terminals if int(term.GetBoundaryType()) in [0, 3, 4, 7, 8]]
         locations = []
         for term in terms:
             if term.GetTerminalType().ToString() == "PadstackInstanceTerminal":
                 if term.GetParameters()[1].GetNet().GetName() in reference_list:
                     locations.append(self.padstacks.instances[term.GetParameters()[1].GetId()].position)
             elif term.GetTerminalType().ToString() == "PointTerminal" and term.GetNet().GetName() in reference_list:
                 pd = term.GetParameters()[1]
                 locations.append([pd.X.ToDouble(), pd.Y.ToDouble()])
         if include_pingroups:
             for reference in reference_list:
                 for pin in self.nets.nets[reference].padstack_instances:
                     if pin.pingroups:
                         locations.append(pin.position)
         for point in locations:
-            pointA = self.edb.Geometry.PointData(self.edb_value(point[0] - 1e-12), self.edb_value(point[1] - 1e-12))
-            pointB = self.edb.Geometry.PointData(self.edb_value(point[0] + 1e-12), self.edb_value(point[1] + 1e-12))
-            points = Tuple[self.edb.Geometry.PointData, self.edb.Geometry.PointData](pointA, pointB)
-            _polys.append(self.edb.Geometry.PolygonData.CreateFromBBox(points))
+            pointA = self.edb_api.geometry.point_data(
+                self.edb_value(point[0] - 1e-12), self.edb_value(point[1] - 1e-12)
+            )
+            pointB = self.edb_api.geometry.point_data(
+                self.edb_value(point[0] + 1e-12), self.edb_value(point[1] + 1e-12)
+            )
+
+            points = Tuple[self.edb_api.geometry.geometry.PointData, self.edb_api.geometry.geometry.PointData](
+                pointA, pointB
+            )
+            _polys.append(self.edb_api.geometry.polygon_data.create_from_bbox(points))
         for cname, c in self.components.instances.items():
             if (
                 set(net_signals).intersection(c.nets)
                 and c.is_enabled
                 and c.model_type in ["SParameterModel", "SpiceModel", "NetlistModel"]
             ):
                 for pin in c.pins:
@@ -1541,15 +1401,15 @@
         for net in net_signals:
             names.append(net.GetName())
         for prim in self.modeler.primitives:
             if prim.net_name in names:
                 _polys.append(prim.primitive_object.GetPolygonData())
         if smart_cut:
             _polys.extend(self._smart_cut(net_signals, reference_list, include_pingroups))
-        _poly = self.edb.Geometry.PolygonData.GetConvexHullOfPolygons(convert_py_list_to_net_list(_polys))
+        _poly = self.edb_api.geometry.polygon_data.get_convex_hull_of_polygons(convert_py_list_to_net_list(_polys))
         _poly = _poly.Expand(expansion_size, tolerance, round_corner, round_extension)[0]
         return _poly
 
     @pyaedt_function_handler()
     def cutout(
         self,
         signal_list=None,
@@ -1728,15 +1588,15 @@
                             self.save_edb_as(output_aedb_path)
                         else:
                             self.save_edb_as(legacy_path)
                         working_cutout = True
                         break
                     self.close_edb()
                     self.edbpath = legacy_path
-                    self.open_edb(True)
+                    self.open_edb()
                     i += 1
                     expansion = expansion_size * i
                 if working_cutout:
                     msg = "Cutout completed in {} iterations with expansion size of {}mm".format(i, expansion * 1e3)
                     self.logger.info_timer(msg, start)
                 else:
                     msg = "Cutout failed after {} iterations and expansion size of {}mm".format(i, expansion * 1e3)
@@ -1759,15 +1619,15 @@
                     check_terminals=check_terminals,
                     include_pingroups=include_pingroups,
                 )
             if result and not open_cutout_at_end and self.edbpath != legacy_path:
                 self.save_edb()
                 self.close_edb()
                 self.edbpath = legacy_path
-                self.open_edb(init_dlls=True)
+                self.open_edb()
             return result
 
     @pyaedt_function_handler()
     def _create_cutout_legacy(
         self,
         signal_list=[],
         reference_list=["GND"],
@@ -1780,20 +1640,19 @@
         remove_single_pin_components=False,
         check_terminals=False,
         include_pingroups=True,
     ):
         expansion_size = self.edb_value(expansion_size).ToDouble()
 
         # validate nets in layout
-        net_signals = convert_py_list_to_net_list(
-            [net for net in list(self.active_layout.Nets) if net.GetName() in signal_list]
-        )
+        net_signals = [net.api_object for net in self.layout.nets if net.name in signal_list]
+
         # validate references in layout
         _netsClip = convert_py_list_to_net_list(
-            [net for net in list(self.active_layout.Nets) if net.GetName() in reference_list]
+            [net.api_object for net in self.layout.nets if net.name in reference_list]
         )
 
         _poly = self._create_extent(
             net_signals,
             extent_type,
             expansion_size,
             use_round_corner,
@@ -1802,15 +1661,15 @@
             reference_list=reference_list,
             include_pingroups=include_pingroups,
         )
 
         # Create new cutout cell/design
         included_nets_list = signal_list + reference_list
         included_nets = convert_py_list_to_net_list(
-            [net for net in list(self.active_layout.Nets) if net.GetName() in included_nets_list]
+            [net.api_object for net in self.layout.nets if net.name in included_nets_list]
         )
         _cutout = self.active_cell.CutOut(included_nets, _netsClip, _poly, True)
         # Analysis setups do not come over with the clipped design copy,
         # so add the analysis setups from the original here.
         id = 1
         for _setup in self.active_cell.SimulationSetups:
             # Empty string '' if coming from setup copy and don't set explicitly.
@@ -1825,32 +1684,31 @@
                 id += 1
             else:
                 _cutout.AddSimulationSetup(_setup)  # Add simulation setup to the cutout design
 
         _dbCells = [_cutout]
 
         if output_aedb_path:
-            db2 = self.edb.Database.Create(output_aedb_path)
+            db2 = self.create(output_aedb_path)
             _success = db2.Save()
             _dbCells = convert_py_list_to_net_list(_dbCells)
             db2.CopyCells(_dbCells)  # Copies cutout cell/design to db2 project
             if len(list(db2.CircuitCells)) > 0:
                 for net in list(list(db2.CircuitCells)[0].GetLayout().Nets):
                     if not net.GetName() in included_nets_list:
                         net.Delete()
                 _success = db2.Save()
-            for c in list(self.db.TopCircuitCells):
+            for c in list(self.active_db.TopCircuitCells):
                 if c.GetName() == _cutout.GetName():
                     c.Delete()
             if open_cutout_at_end:  # pragma: no cover
                 self._db = db2
                 self.edbpath = output_aedb_path
-                self._active_cell = list(self._db.TopCircuitCells)[0]
-                self.builder = EdbBuilder(self.edbutils, self._db, self._active_cell)
-                self.edbpath = self._db.GetDirectory()
+                self._active_cell = list(self.top_circuit_cells)[0]
+                self.edbpath = self.directory
                 self._init_objects()
                 if remove_single_pin_components:
                     self.components.delete_single_pin_rlc()
                     self.logger.info_timer("Single Pins components deleted")
                     self.components.refresh_components()
             else:
                 if remove_single_pin_components:
@@ -2011,70 +1869,65 @@
                 for i in custom_extent
             ]
             plane = self.modeler.Shape("polygon", points=custom_extent)
             _poly = self.modeler.shape_to_polygon_data(plane)
         elif custom_extent:
             _poly = custom_extent
         else:
-            net_signals = convert_py_list_to_net_list(
-                [net for net in list(self.active_layout.Nets) if net.GetName() in signal_list]
-            )
+            net_signals = [net.api_object for net in self.layout.nets if net.name in signal_list]
             _poly = self._create_extent(
                 net_signals,
                 extent_type,
                 expansion_size,
                 use_round_corner,
                 use_pyaedt_extent_computing,
                 smart_cut=check_terminals,
                 reference_list=reference_list,
                 include_pingroups=include_pingroups,
             )
-            if extent_type in ["Conforming", self.edb.Geometry.ExtentType.Conforming, 1] and extent_defeature > 0:
+            if extent_type in ["Conforming", self.edb_api.geometry.extent_type.Conforming, 1] and extent_defeature > 0:
                 _poly = _poly.Defeature(extent_defeature)
 
         if not _poly or _poly.IsNull():
             self._logger.error("Failed to create Extent.")
             return False
         self.logger.info_timer("Expanded Net Polygon Creation")
         self.logger.reset_timer()
         _poly_list = convert_py_list_to_net_list([_poly])
         prims_to_delete = []
         poly_to_create = []
         pins_to_delete = []
 
-        def get_polygon_data(prim):
-            return prim.primitive_object.GetPolygonData()
-
         def intersect(poly1, poly2):
             if not isinstance(poly2, list):
                 poly2 = [poly2]
             return list(poly1.Intersect(convert_py_list_to_net_list(poly1), convert_py_list_to_net_list(poly2)))
 
         def subtract(poly, voids):
             return poly.Subtract(convert_py_list_to_net_list(poly), convert_py_list_to_net_list(voids))
 
         def clean_prim(prim_1):  # pragma: no cover
-            pdata = get_polygon_data(prim_1)
+            pdata = prim_1.polygon_data
             int_data = _poly.GetIntersectionType(pdata)
             if int_data == 2:
                 return
             elif int_data == 0:
                 prims_to_delete.append(prim_1)
             else:
                 list_poly = intersect(_poly, pdata)
                 if list_poly:
                     net = prim_1.net_name
                     voids = prim_1.voids
                     for p in list_poly:
                         if p.IsNull():
                             continue
-                        points = list(p.Points)
+                        # points = list(p.Points)
                         list_void = []
                         if voids:
-                            voids_data = [get_polygon_data(void) for void in voids]
+                            voids_data = [void.polygon_data for void in voids]
                             list_prims = subtract(p, voids_data)
                             for prim in list_prims:
                                 if not prim.IsNull():
                                     poly_to_create.append([prim, prim_1.layer_name, net, list_void])
                             #
                             # list_voids = intersect(p, voids_data)
                             # for void_intersected in list_voids:
@@ -2115,21 +1968,23 @@
         self.logger.reset_timer()
 
         i = 0
         for _, val in self.components.components.items():
             if val.numpins == 0:
                 val.edbcomponent.Delete()
                 i += 1
+                i += 1
         self.logger.info("Deleted {} additional components".format(i))
         if remove_single_pin_components:
             self.components.delete_single_pin_rlc()
             self.logger.info_timer("Single Pins components deleted")
 
         self.components.refresh_components()
-
+        if output_aedb_path:
+            self.save_edb()
         self.logger.info_timer("Cutout completed.", timer_start)
         self.logger.reset_timer()
         return True
 
     @pyaedt_function_handler()
     def create_cutout_multithread(
         self,
@@ -2243,26 +2098,22 @@
         """
         temp_edb_path = self.edbpath[:-5] + "_temp_aedb.aedb"
         shutil.copytree(self.edbpath, temp_edb_path)
         temp_edb = Edb(temp_edb_path)
         for via in list(temp_edb.padstacks.instances.values()):
             via.pin.Delete()
         if netlist:
-            nets = convert_py_list_to_net_list(
-                [net for net in list(self.active_layout.Nets) if net.GetName() in netlist]
-            )
-            _poly = temp_edb.active_layout.GetExpandedExtentFromNets(
-                nets, self.edb.Geometry.ExtentType.Conforming, 0.0, True, True, 1
+            nets = [net for net in temp_edb.layout.nets if net.name in netlist]
+            _poly = temp_edb.layout.expanded_extent(
+                nets, self.edb_api.geometry.extent_type.Conforming, 0.0, True, True, 1
             )
         else:
-            nets = convert_py_list_to_net_list(
-                [net for net in list(temp_edb.active_layout.Nets) if "gnd" in net.GetName().lower()]
-            )
-            _poly = temp_edb.active_layout.GetExpandedExtentFromNets(
-                nets, self.edb.Geometry.ExtentType.Conforming, 0.0, True, True, 1
+            nets = [net.api_object for net in temp_edb.layout.nets if "gnd" in net.name.lower()]
+            _poly = temp_edb.layout.expanded_extent(
+                nets, self.edb_api.geometry.extent_type.Conforming, 0.0, True, True, 1
             )
             temp_edb.close_edb()
         if _poly:
             return _poly
         else:
             return False
 
@@ -2367,28 +2218,31 @@
             voids = []
         voids_to_add = []
         for circle in voids:
             if polygonData.GetIntersectionType(circle.primitive_object.GetPolygonData()) >= 3:
                 voids_to_add.append(circle)
 
         _netsClip = convert_py_list_to_net_list(_ref_nets)
-        net_signals = List[type(_ref_nets[0])]()  # pragma: no cover
+        net_signals = convert_py_list_to_net_list([], type(_ref_nets[0]))
+
         # Create new cutout cell/design
         _cutout = self.active_cell.CutOut(net_signals, _netsClip, polygonData)
         layout = _cutout.GetLayout()
         cutout_obj_coll = list(layout.PadstackInstances)
         ids = []
         for lobj in cutout_obj_coll:
             ids.append(lobj.GetId())
 
         if include_partial_instances:
             p_missing = [i for i in pinstance_to_add if i.id not in ids]
             self.logger.info("Added {} padstack instances after cutout".format(len(p_missing)))
             for p in p_missing:
-                position = self.edb.Geometry.PointData(self.edb_value(p.position[0]), self.edb_value(p.position[1]))
+                position = self.edb_api.geometry.point_data(
+                    self.edb_value(p.position[0]), self.edb_value(p.position[1])
+                )
                 net = self.nets.find_or_create_net(p.net_name)
                 rotation = self.edb_value(p.rotation)
                 sign_layers = list(self.stackup.signal_layers.keys())
                 if not p.start_layer:  # pragma: no cover
                     fromlayer = self.stackup.signal_layers[sign_layers[0]]._edb_layer
                 else:
                     fromlayer = self.stackup.signal_layers[p.start_layer]._edb_layer
@@ -2397,15 +2251,15 @@
                     tolayer = self.stackup.signal_layers[sign_layers[-1]]._edb_layer
                 else:
                     tolayer = self.stackup.signal_layers[p.stop_layer]._edb_layer
                 padstack = None
                 for pad in list(self.padstacks.definitions.keys()):
                     if pad == p.padstack_definition:
                         padstack = self.padstacks.definitions[pad].edb_padstack
-                        padstack_instance = self.edb.Cell.Primitive.PadstackInstance.Create(
+                        padstack_instance = self.edb_api.cell.primitive.padstack_instance.create(
                             _cutout.GetLayout(),
                             net,
                             p.name,
                             padstack,
                             position,
                             rotation,
                             fromlayer,
@@ -2418,25 +2272,25 @@
 
         for void_circle in voids_to_add:
             if void_circle.type == "Circle":
                 if is_ironpython:  # pragma: no cover
                     res, center_x, center_y, radius = void_circle.primitive_object.GetParameters()
                 else:
                     res, center_x, center_y, radius = void_circle.primitive_object.GetParameters(0.0, 0.0, 0.0)
-                cloned_circle = self.edb.Cell.Primitive.Circle.Create(
+                cloned_circle = self.edb_api.cell.primitive.circle.create(
                     layout,
                     void_circle.layer_name,
                     void_circle.net,
                     self.edb_value(center_x),
                     self.edb_value(center_y),
                     self.edb_value(radius),
                 )
                 cloned_circle.SetIsNegative(True)
             elif void_circle.type == "Polygon":
-                cloned_polygon = self.edb.Cell.Primitive.Polygon.Create(
+                cloned_polygon = self.edb_api.cell.primitive.polygon.create(
                     layout, void_circle.layer_name, void_circle.net, void_circle.primitive_object.GetPolygonData()
                 )
                 cloned_polygon.SetIsNegative(True)
         layers = [i for i in list(self.stackup.signal_layers.keys())]
         for layer in layers:
             layer_primitves = self.modeler.get_primitives(layer_name=layer)
             if len(layer_primitves) == 0:
@@ -2455,33 +2309,32 @@
                 _cutout.AddSimulationSetup(_setup)  # Add simulation setup to the cutout design
                 id += 1
             else:
                 _cutout.AddSimulationSetup(_setup)  # Add simulation setup to the cutout design
 
         _dbCells = [_cutout]
         if output_aedb_path:
-            db2 = self.edb.Database.Create(output_aedb_path)
+            db2 = self.create(output_aedb_path)
             if not db2.Save():
                 self.logger.error("Failed to create new Edb. Check if the path already exists and remove it.")
                 return False
             _dbCells = convert_py_list_to_net_list(_dbCells)
             cell_copied = db2.CopyCells(_dbCells)  # Copies cutout cell/design to db2 project
             cell = list(cell_copied)[0]
             cell.SetName(os.path.basename(output_aedb_path[:-5]))
             db2.Save()
-            for c in list(self.db.TopCircuitCells):
+            for c in list(self.active_db.TopCircuitCells):
                 if c.GetName() == _cutout.GetName():
                     c.Delete()
             if open_cutout_at_end:  # pragma: no cover
                 _success = db2.Save()
                 self._db = db2
                 self.edbpath = output_aedb_path
                 self._active_cell = cell
-                self.builder = EdbBuilder(self.edbutils, self._db, self._active_cell)
-                self.edbpath = self._db.GetDirectory()
+                self.edbpath = self.directory
                 self._init_objects()
             else:
                 db2.Close()
                 source = os.path.join(output_aedb_path, "edb.def.tmp")
                 target = os.path.join(output_aedb_path, "edb.def")
                 self._wait_for_file_release(file_to_release=output_aedb_path)
                 if os.path.exists(source) and not os.path.exists(target):
@@ -2721,15 +2574,15 @@
         Returns
         -------
         str
             Siwave project path.
         """
         process = SiwaveSolve(self.edbpath, aedt_version=self.edbversion)
         try:
-            self._db.Close()
+            self.close()
         except:
             pass
         process.solve()
         return self.edbpath[:-5] + ".siw"
 
     @pyaedt_function_handler()
     def export_siwave_dc_results(
@@ -2773,15 +2626,15 @@
         Returns
         -------
         list
             List of files generated.
         """
         process = SiwaveSolve(self.edbpath, aedt_version=self.edbversion)
         try:
-            self._db.Close()
+            self.close()
         except:
             pass
         return process.export_dc_report(
             siwave_project,
             solution_name,
             output_folder,
             html_report,
@@ -2802,15 +2655,15 @@
         -------
         tuple of bool and VaribleServer
             It returns a booleand to check if the variable exists and the variable
             server that should contain the variable.
         """
         if "$" in variable_name:
             if variable_name.index("$") == 0:
-                var_server = self.db.GetVariableServer()
+                var_server = self.active_db.GetVariableServer()
 
             else:
                 var_server = self.active_cell.GetVariableServer()
 
         else:
             var_server = self.active_cell.GetVariableServer()
 
@@ -3013,15 +2866,15 @@
                         use_round_corner=simulation_setup.cutout_subdesign_round_corner,
                         extent_type=simulation_setup.cutout_subdesign_type,
                         use_pyaedt_cutout=False,
                         use_pyaedt_extent_computing=False,
                     ):
                         self.logger.info("Cutout processed.")
                         old_cell = self.active_cell.FindByName(
-                            self._db, self.edb.Cell.CellType.CircuitCell, old_cell_name
+                            self.db, self.edb_api.cell.CellType.CircuitCell, old_cell_name
                         )
                         if old_cell:
                             old_cell.Delete()
                     else:  # pragma: no cover
                         self.logger.error("Cutout failed.")
                 else:
                     self.logger.info("Cutting out using method: {0}".format(simulation_setup.cutout_subdesign_type))
@@ -3032,64 +2885,74 @@
                         use_round_corner=simulation_setup.cutout_subdesign_round_corner,
                         extent_type=simulation_setup.cutout_subdesign_type,
                         use_pyaedt_cutout=True,
                         use_pyaedt_extent_computing=True,
                         remove_single_pin_components=True,
                     )
                     self.logger.info("Cutout processed.")
+            else:
+                if simulation_setup.include_only_selected_nets:
+                    included_nets = simulation_setup.signal_nets + simulation_setup.power_nets
+                    nets_to_remove = [
+                        net.name for net in list(self.nets.nets.values()) if not net.name in included_nets
+                    ]
+                    self.nets.delete(nets_to_remove)
             self.logger.info("Deleting existing ports.")
-            map(lambda port: port.Delete(), list(self.active_layout.Terminals))
-            map(lambda pg: pg.Delete(), list(self.active_layout.PinGroups))
+            map(lambda port: port.Delete(), self.layout.terminals)
+            map(lambda pg: pg.Delete(), self.layout.pin_groups)
             if simulation_setup.solver_type == SolverType.Hfss3dLayout:
-                self.logger.info("Creating HFSS ports for signal nets.")
-                for cmp in simulation_setup.components:
-                    self.components.create_port_on_component(
-                        cmp,
-                        net_list=simulation_setup.signal_nets,
-                        do_pingroup=False,
-                        reference_net=simulation_setup.power_nets,
-                        port_type=SourceType.CoaxPort,
-                    )
-                if not self.hfss.set_coax_port_attributes(simulation_setup):  # pragma: no cover
-                    self.logger.error("Failed to configure coaxial port attributes.")
-                self.logger.info("Number of ports: {}".format(self.hfss.get_ports_number()))
-                self.logger.info("Configure HFSS extents.")
-                if simulation_setup.trim_reference_size:  # pragma: no cover
-                    self.logger.info(
-                        "Trimming the reference plane for coaxial ports: {0}".format(
-                            bool(simulation_setup.trim_reference_size)
+                if simulation_setup.generate_excitations:
+                    self.logger.info("Creating HFSS ports for signal nets.")
+                    for cmp in simulation_setup.components:
+                        self.components.create_port_on_component(
+                            cmp,
+                            net_list=simulation_setup.signal_nets,
+                            do_pingroup=False,
+                            reference_net=simulation_setup.power_nets,
+                            port_type=SourceType.CoaxPort,
                         )
-                    )
-                    self.hfss.trim_component_reference_size(simulation_setup)  # pragma: no cover
+                    if not self.hfss.set_coax_port_attributes(simulation_setup):  # pragma: no cover
+                        self.logger.error("Failed to configure coaxial port attributes.")
+                    self.logger.info("Number of ports: {}".format(self.hfss.get_ports_number()))
+                    self.logger.info("Configure HFSS extents.")
+                    if simulation_setup.trim_reference_size:  # pragma: no cover
+                        self.logger.info(
+                            "Trimming the reference plane for coaxial ports: {0}".format(
+                                bool(simulation_setup.trim_reference_size)
+                            )
+                        )
+                        self.hfss.trim_component_reference_size(simulation_setup)  # pragma: no cover
                 self.hfss.configure_hfss_extents(simulation_setup)
                 if not self.hfss.configure_hfss_analysis_setup(simulation_setup):
                     self.logger.error("Failed to configure HFSS simulation setup.")
             if simulation_setup.solver_type == SolverType.SiwaveSYZ:
-                for cmp in simulation_setup.components:
-                    self.components.create_port_on_component(
-                        cmp,
-                        net_list=simulation_setup.signal_nets,
-                        do_pingroup=simulation_setup.do_pingroup,
-                        reference_net=simulation_setup.power_nets,
-                        port_type=SourceType.CircPort,
-                    )
+                if simulation_setup.generate_excitations:
+                    for cmp in simulation_setup.components:
+                        self.components.create_port_on_component(
+                            cmp,
+                            net_list=simulation_setup.signal_nets,
+                            do_pingroup=simulation_setup.do_pingroup,
+                            reference_net=simulation_setup.power_nets,
+                            port_type=SourceType.CircPort,
+                        )
                 self.logger.info("Configuring analysis setup.")
                 if not self.siwave.configure_siw_analysis_setup(simulation_setup):  # pragma: no cover
                     self.logger.error("Failed to configure Siwave simulation setup.")
 
             if simulation_setup.solver_type == SolverType.SiwaveDC:
-                self.components.create_source_on_component(simulation_setup.sources)
+                if simulation_setup.generate_excitations:
+                    self.components.create_source_on_component(simulation_setup.sources)
                 if not self.siwave.configure_siw_analysis_setup(simulation_setup):  # pragma: no cover
                     self.logger.error("Failed to configure Siwave simulation setup.")
             self.padstacks.check_and_fix_via_plating()
             self.save_edb()
             if not simulation_setup.open_edb_after_build and simulation_setup.output_aedb:
                 self.close_edb()
                 self.edbpath = legacy_name
-                self.open_edb(True)
+                self.open_edb()
             return True
         except:  # pragma: no cover
             return False
 
     @pyaedt_function_handler()
     def get_statistics(self, compute_area=False):
         """Get the EDBStatistics object.
@@ -3213,19 +3076,19 @@
         Dict[str, :class:`pyaedt.edb_core.edb_data.hfss_simulation_setup_data.HfssSimulationSetup`] or
         Dict[str, :class:`pyaedt.edb_core.edb_data.siwave_simulation_setup_data.SiwaveDCSimulationSetup`] or
         Dict[str, :class:`pyaedt.edb_core.edb_data.siwave_simulation_setup_data.SiwaveSYZSimulationSetup`]
 
         """
         for i in list(self.active_cell.SimulationSetups):
             if i.GetName() not in self._setups:
-                if i.GetType() == self.edb.Utility.SimulationSetupType.kHFSS:
+                if i.GetType() == self.edb_api.utility.utility.SimulationSetupType.kHFSS:
                     self._setups[i.GetName()] = HfssSimulationSetup(self, i.GetName(), i)
-                elif i.GetType() == self.edb.Utility.SimulationSetupType.kSIWave:
+                elif i.GetType() == self.edb_api.utility.utility.SimulationSetupType.kSIWave:
                     self._setups[i.GetName()] = SiwaveSYZSimulationSetup(self, i.GetName(), i)
-                elif i.GetType() == self.edb.Utility.SimulationSetupType.kSIWaveDCIR:
+                elif i.GetType() == self.edb_api.utility.utility.SimulationSetupType.kSIWaveDCIR:
                     self._setups[i.GetName()] = SiwaveDCSimulationSetup(self, i.GetName(), i)
         return self._setups
 
     @property
     def hfss_setups(self):
         """Active HFSS setup in EDB.
 
@@ -3389,15 +3252,15 @@
             if not os.path.isdir(working_directory):
                 os.mkdir(working_directory)
             else:
                 shutil.rmtree(working_directory)
                 os.mkdir(working_directory)
         else:
             working_directory = os.path.dirname(self.edbpath)
-        zone_primitives = list(self.active_layout.GetZonePrimitives())
+        zone_primitives = list(self.layout.zone_primitives)
         zone_ids = list(self.stackup._layer_collection.GetZoneIds())
         edb_zones = {}
         if not self.setups:
             self.siwave.add_siwave_syz_analysis()
             self.save_edb()
         if not len(zone_primitives) == len(zone_ids):
             self.logger.info("Number of zone primitives not equal to zone number, zone information will be lost")
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/components.py` & `pyaedt-0.6.79/pyaedt/edb_core/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,49 +102,49 @@
     @property
     def _logger(self):
         """Logger."""
         return self._pedb.logger
 
     @property
     def _edb(self):
-        return self._pedb.edb
+        return self._pedb.edb_api
 
     @pyaedt_function_handler()
     def _init_parts(self):
         a = self.components
         a = self.resistors
         a = self.ICs
         a = self.Others
         a = self.inductors
         a = self.IOs
         a = self.components_by_partname
         return True
 
-    @property
-    def _builder(self):
-        return self._pedb.builder
-
     def _get_edb_value(self, value):
         return self._pedb.edb_value(value)
 
     @property
     def _edbutils(self):
         return self._pedb.edbutils
 
     @property
     def _active_layout(self):
         return self._pedb.active_layout
 
     @property
+    def _layout(self):
+        return self._pedb.layout
+
+    @property
     def _cell(self):
         return self._pedb.cell
 
     @property
     def _db(self):
-        return self._pedb.db
+        return self._pedb.active_db
 
     @property
     def components(self):
         """Component setup information.
 
         .. deprecated:: 0.6.62
            Use new property :func:`instances` instead.
@@ -189,15 +189,15 @@
     @property
     def definitions(self):
         """Retrieve component definition list.
 
         Returns
         -------
         dict of :class:`pyaedt.edb_core.edb_data.components_data.EDBComponentDef`"""
-        return {l.GetName(): EDBComponentDef(self, l) for l in list(self._db.ComponentDefs)}
+        return {l.GetName(): EDBComponentDef(self, l) for l in list(self._pedb.component_defs)}
 
     @property
     def nport_comp_definition(self):
         """Retrieve Nport component definition list."""
         m = "Ansys.Ansoft.Edb.Definition.NPortComponentModel"
         return {name: l for name, l in self.definitions.items() if m in [i.ToString() for i in l._comp_model]}
 
@@ -286,15 +286,15 @@
 
     @pyaedt_function_handler()
     def refresh_components(self):
         """Refresh the component dictionary."""
         # self._logger.info("Refreshing the Components dictionary.")
         self._cmp = {
             l.GetName(): EDBComponent(self, l)
-            for l in self._active_layout.Groups
+            for l in self._layout.groups
             if l.ToString() == "Ansys.Ansoft.Edb.Cell.Hierarchy.Component"
         }
         return True
 
     @property
     def resistors(self):
         """Resistors.
@@ -453,45 +453,29 @@
             if val.partname in self._comps_by_part.keys():
                 self._comps_by_part[val.partname].append(val)
             else:
                 self._comps_by_part[val.partname] = [val]
         return self._comps_by_part
 
     @pyaedt_function_handler()
-    def get_component_list(self):
-        """Retrieve conponent setup information.
-
-        Returns
-        -------
-        list
-            List of component setup information.
-
-        """
-        cmp_setup_info_list = self._edbutils.ComponentSetupInfo.GetFromLayout(self._active_layout)
-        cmp_list = []
-        for comp in cmp_setup_info_list:
-            cmp_list.append(comp)
-        return cmp_list
-
-    @pyaedt_function_handler()
     def get_component_by_name(self, name):
         """Retrieve a component by name.
 
         Parameters
         ----------
         name : str
             Name of the component.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        edbcmp = self._edb.Cell.Hierarchy.Component.FindByName(self._active_layout, name)
+        edbcmp = self._pedb.edb_api.cell.hierarchy.component.FindByName(self._active_layout, name)
         if edbcmp is not None:
             return edbcmp
         else:
             pass
 
     @pyaedt_function_handler()
     def get_components_from_nets(self, netlist=None):
@@ -516,15 +500,15 @@
             cmpnets = self._cmp[refdes].nets
             if set(cmpnets).intersection(set(netlist)):
                 cmp_list.append(refdes)
         return cmp_list
 
     @pyaedt_function_handler()
     def _get_edb_pin_from_pin_name(self, cmp, pin):
-        if not isinstance(cmp, self._edb.Cell.Hierarchy.Component):
+        if not isinstance(cmp, self._pedb.edb_api.cell.hierarchy.component):
             return False
         if not isinstance(pin, str):
             pin = pin.GetName()
         pins = self.get_pin_from_component(component=cmp, pinName=pin)
         if pins:
             return pins[0]
         return False
@@ -540,17 +524,17 @@
         hosting_component_pin2,
         flipped=False,
     ):
         """Get the placement vector between 2 components.
 
         Parameters
         ----------
-        mounted_component : `edb.Cell.Hierarchy.Component`
+        mounted_component : `edb.cell.hierarchy._hierarchy.Component`
             Mounted component name.
-        hosting_component : `edb.Cell.Hierarchy.Component`
+        hosting_component : `edb.cell.hierarchy._hierarchy.Component`
             Hosting component name.
         mounted_component_pin1 : str
             Mounted component Pin 1 name.
         mounted_component_pin2 : str
             Mounted component Pin 2 name.
         hosting_component_pin1 : str
             Hosted component Pin 1 name.
@@ -577,17 +561,17 @@
         ...                                             hosting_component_pin1="A12",
         ...                                             hosting_component_pin2="A14")
         """
         m_pin1_pos = [0.0, 0.0]
         m_pin2_pos = [0.0, 0.0]
         h_pin1_pos = [0.0, 0.0]
         h_pin2_pos = [0.0, 0.0]
-        if not isinstance(mounted_component, self._edb.Cell.Hierarchy.Component):
+        if not isinstance(mounted_component, self._pedb.edb_api.cell.hierarchy.component):
             return False
-        if not isinstance(hosting_component, self._edb.Cell.Hierarchy.Component):
+        if not isinstance(hosting_component, self._pedb.edb_api.cell.hierarchy.component):
             return False
 
         if mounted_component_pin1:
             m_pin1 = self._get_edb_pin_from_pin_name(mounted_component, mounted_component_pin1)
             m_pin1_pos = self.get_pin_position(m_pin1)
         if mounted_component_pin2:
             m_pin2 = self._get_edb_pin_from_pin_name(mounted_component, mounted_component_pin2)
@@ -629,25 +613,25 @@
 
     @pyaedt_function_handler()
     def get_solder_ball_height(self, cmp):
         """Get component solder ball height.
 
         Parameters
         ----------
-        cmp : str or self._edb.Cell.Hierarchy.Component
+        cmp : str or  self._pedb.component
             EDB component or str component name.
 
         Returns
         -------
         double, bool
             Salder ball height vale, ``False`` when failed.
 
         """
         if cmp is not None:
-            if not (isinstance(cmp, self._edb.Cell.Hierarchy.Component)):
+            if not (isinstance(cmp, self._pedb.edb_api.cell.hierarchy.component)):
                 cmp = self.get_component_by_name(cmp)
             cmp_prop = cmp.GetComponentProperty().Clone()
             return cmp_prop.GetSolderBallProperty().GetHeight()
         return False
 
     @pyaedt_function_handler()
     def create_source_on_component(self, sources=None):
@@ -686,16 +670,16 @@
             if source.source_type == SourceType.Vsource:  # pragma: no cover
                 positive_pin_group_term = self._create_pin_group_terminal(
                     positive_pin_group, source.positive_node.component
                 )
                 negative_pin_group_term = self._create_pin_group_terminal(
                     negative_pin_group, source.negative_node.component, isref=True
                 )
-                positive_pin_group_term.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kVoltageSource)
-                negative_pin_group_term.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kVoltageSource)
+                positive_pin_group_term.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kVoltageSource)
+                negative_pin_group_term.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kVoltageSource)
                 term_name = source.name
                 positive_pin_group_term.SetName(term_name)
                 negative_pin_group_term.SetName("{}_ref".format(term_name))
                 positive_pin_group_term.SetSourceAmplitude(self._get_edb_value(source.amplitude))
                 negative_pin_group_term.SetSourceAmplitude(self._get_edb_value(source.amplitude))
                 positive_pin_group_term.SetSourcePhase(self._get_edb_value(source.phase))
                 negative_pin_group_term.SetSourcePhase(self._get_edb_value(source.phase))
@@ -705,16 +689,16 @@
             elif source.source_type == SourceType.Isource:  # pragma: no cover
                 positive_pin_group_term = self._create_pin_group_terminal(
                     positive_pin_group, source.positive_node.component
                 )
                 negative_pin_group_term = self._create_pin_group_terminal(
                     negative_pin_group, source.negative_node.component, isref=True
                 )
-                positive_pin_group_term.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kCurrentSource)
-                negative_pin_group_term.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kCurrentSource)
+                positive_pin_group_term.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kCurrentSource)
+                negative_pin_group_term.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kCurrentSource)
                 term_name = source.name
                 positive_pin_group_term.SetName(term_name)
                 negative_pin_group_term.SetName("{}_ref".format(term_name))
                 positive_pin_group_term.SetSourceAmplitude(self._get_edb_value(source.amplitude))
                 negative_pin_group_term.SetSourceAmplitude(self._get_edb_value(source.amplitude))
                 positive_pin_group_term.SetSourcePhase(self._get_edb_value(source.phase))
                 negative_pin_group_term.SetSourcePhase(self._get_edb_value(source.phase))
@@ -802,15 +786,15 @@
         ref_group_name = "group_{}_{}_ref".format(pins[0].net_name, pins[0].name)
         pin_group = self.create_pingroup_from_pins(pins, group_name)
         ref_pin_group = self.create_pingroup_from_pins(reference_pins, ref_group_name)
         term = self._create_pin_group_terminal(pingroup=pin_group, component=refdes.refdes)
         term.SetIsCircuitPort(True)
         ref_term = self._create_pin_group_terminal(pingroup=ref_pin_group, component=refdes.refdes)
         ref_term.SetIsCircuitPort(True)
-        term.SetImpedance(self._edb.Utility.Value(impedance))
+        term.SetImpedance(self._edb.utility.value(impedance))
         term.SetReferenceTerminal(ref_term)
         if term:
             return term
         return False
 
     @pyaedt_function_handler()
     def create_port_on_component(
@@ -821,15 +805,15 @@
         do_pingroup=True,
         reference_net="gnd",
     ):
         """Create ports on given component.
 
         Parameters
         ----------
-        component : str or self._edb.Cell.Hierarchy.Component
+        component : str or  self._pedb.component
             EDB component or str component name.
         net_list : str or list of string.
             List of nets where ports must be created on the component.
             If the net is not part of the component, this parameter is skipped.
         port_type : SourceType enumerator, CoaxPort or CircuitPort
             Type of port to create. ``CoaxPort`` generates solder balls.
             ``CircuitPort`` generates circuit ports on pins belonging to the net list.
@@ -857,15 +841,15 @@
         if isinstance(component, str):
             component = self.instances[component].edbcomponent
         if not isinstance(net_list, list):
             net_list = [net_list]
         for net in net_list:
             if not isinstance(net, str):
                 try:
-                    net_name = net.GetName()
+                    net_name = net.name
                     if net_name != "":
                         net_list.append(net_name)
                 except:
                     pass
         if reference_net in net_list:
             net_list.remove(reference_net)
         cmp_pins = [
@@ -962,15 +946,15 @@
         pin_position = self.get_pin_position(pin)  # pragma no cover
         pin_pos = self._pedb.point_data(*pin_position)
         res, from_layer, _ = pin.GetLayerRange()
         cmp_name = pin.GetComponent().GetName()
         net_name = pin.GetNet().GetName()
         pin_name = pin.GetName()
         term_name = "{}.{}.{}".format(cmp_name, pin_name, net_name)
-        term = self._edb.Cell.Terminal.PointTerminal.Create(
+        term = self._edb.cell.terminal.PointTerminal.Create(
             pin.GetLayout(), pin.GetNet(), term_name, pin_pos, from_layer
         )
         return term
 
     @pyaedt_function_handler()
     def _get_closest_pin_from(self, pin, ref_pinlist):
         """Returns the closest pin from given pin among the list of reference pins.
@@ -1036,17 +1020,17 @@
         if isinstance(component, str):
             component = self.instances[component]
             if not component:
                 self._logger.error("component %s not found.", component)
                 return False
         component_type = component.edbcomponent.GetComponentType()
         if (
-            component_type == self._edb.Definition.ComponentType.Other
-            or component_type == self._edb.Definition.ComponentType.IC
-            or component_type == self._edb.Definition.ComponentType.IO
+            component_type == self._edb.definition.ComponentType.Other
+            or component_type == self._edb.definition.ComponentType.IC
+            or component_type == self._edb.definition.ComponentType.IO
         ):
             self._logger.info("Component %s passed to deactivate is not an RLC.", component.refdes)
             return False
         component.is_enabled = False
         if create_circuit_port:
             return self.add_port_on_rlc_component(component.refdes)
         return True
@@ -1073,39 +1057,39 @@
         self.set_component_rlc(component.refdes)
         pins = self.get_pin_from_component(component.refdes)
         if len(pins) == 2:  # pragma: no cover
             pos_pin_loc = self.get_pin_position(pins[0])
             pt = self._pedb.point_data(*pos_pin_loc)
 
             pin_layers = self._padstack._get_pin_layer_range(pins[0])
-            pos_pin_term = self._pedb.edb.Cell.Terminal.PointTerminal.Create(
+            pos_pin_term = self._pedb.edb_api.cell.terminal.PointTerminal.Create(
                 self._active_layout,
                 pins[0].GetNet(),
                 "{}_{}".format(component.refdes, pins[0].GetName()),
                 pt,
                 pin_layers[0],
             )
             if not pos_pin_term:  # pragma: no cover
                 return False
             neg_pin_loc = self.get_pin_position(pins[1])
             pt = self._pedb.point_data(*neg_pin_loc)
 
-            neg_pin_term = self._pedb.edb.Cell.Terminal.PointTerminal.Create(
+            neg_pin_term = self._pedb.edb_api.cell.terminal.PointTerminal.Create(
                 self._active_layout,
                 pins[1].GetNet(),
                 "{}_{}_ref".format(component.refdes, pins[1].GetName()),
                 pt,
                 pin_layers[0],
             )
             if not neg_pin_term:  # pragma: no cover
                 return False
-            pos_pin_term.SetBoundaryType(self._pedb.edb.Cell.Terminal.BoundaryType.PortBoundary)
+            pos_pin_term.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.PortBoundary)
             pos_pin_term.SetIsCircuitPort(True)
             pos_pin_term.SetName(component.refdes)
-            neg_pin_term.SetBoundaryType(self._pedb.edb.Cell.Terminal.BoundaryType.PortBoundary)
+            neg_pin_term.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.PortBoundary)
             neg_pin_term.SetIsCircuitPort(True)
             pos_pin_term.SetReferenceTerminal(neg_pin_term)
             self._logger.info("Component {} has been replaced by port".format(component.refdes))
             return True
 
     @pyaedt_function_handler()
     def _create_pin_group_terminal(self, pingroup, component=None, isref=False):
@@ -1120,67 +1104,69 @@
         isref : bool
 
         Returns
         -------
         Edb pin group terminal.
         """
         if component:
-            if not isinstance(component, self._edb.Cell.Hierarchy.Component):
+            if not isinstance(component, self._pedb.edb_api.cell.hierarchy.component):
                 cmp_name = component
             else:
                 cmp_name = component.GetName()
         else:
             cmp_name = pingroup.GetComponent().GetName()
         net_name = pingroup.GetNet().GetName()
         pin_name = list(pingroup.GetPins())[0].GetName()  # taking first pin name as convention.
         if cmp_name:
             term_name = "{0}.{1}.{2}".format(cmp_name, pin_name, net_name)
         else:
             term_name = "{0}.{1}".format(pin_name, net_name)
-        pingroup_term = self._edb.Cell.Terminal.PinGroupTerminal.Create(
+        pingroup_term = self._edb.cell.terminal.PinGroupTerminal.Create(
             self._active_layout, pingroup.GetNet(), term_name, pingroup, isref
         )
         return pingroup_term
 
     @pyaedt_function_handler()
     def _is_top_component(self, cmp):
         """Test the component placment layer.
 
         Parameters
         ----------
-        cmp : self._edb.Cell.Hierarchy.Component
+        cmp :  self._pedb.component
              Edb component.
 
         Returns
         -------
         bool
             ``True`` when component placed on top layer, ``False`` on bottom layer.
 
 
         """
-        signal_layers = cmp.GetLayout().GetLayerCollection().Layers(self._edb.Cell.LayerTypeSet.SignalLayerSet)
+        signal_layers = cmp.GetLayout().GetLayerCollection().Layers(self._edb.cell.layer_type_set.SignalLayerSet)
         if cmp.GetPlacementLayer() == signal_layers[0]:
             return True
         else:
             return False
 
     @pyaedt_function_handler()
     def _getComponentDefinition(self, name, pins):
-        componentDefinition = self._edb.Definition.ComponentDef.FindByName(self._db, name)
+        componentDefinition = self._pedb.edb_api.definition.ComponentDef.FindByName(self._db, name)
         if componentDefinition.IsNull():
-            componentDefinition = self._edb.Definition.ComponentDef.Create(self._db, name, None)
+            componentDefinition = self._pedb.edb_api.definition.ComponentDef.Create(self._db, name, None)
             if componentDefinition.IsNull():
                 self._logger.error("Failed to create component definition {}".format(name))
                 return None
             ind = 1
             for pin in pins:
                 if not pin.GetName():
                     pin.SetName(str(ind))
                 ind += 1
-                componentDefinitionPin = self._edb.Definition.ComponentDefPin.Create(componentDefinition, pin.GetName())
+                componentDefinitionPin = self._pedb.edb_api.definition.ComponentDefPin.Create(
+                    componentDefinition, pin.GetName()
+                )
                 if componentDefinitionPin.IsNull():
                     self._logger.error("Failed to create component definition pin {}-{}".format(name, pin.GetName()))
                     return None
         else:
             self._logger.warning("Found existing component definition for footprint {}".format(name))
         return componentDefinition
 
@@ -1276,34 +1262,34 @@
         """
         if component_part_name:
             compdef = self._getComponentDefinition(component_part_name, pins)
         else:
             compdef = self._getComponentDefinition(component_name, pins)
         if not compdef:
             return False
-        new_cmp = self._edb.Cell.Hierarchy.Component.Create(self._active_layout, component_name, compdef.GetName())
+        new_cmp = self._pedb.edb_api.cell.hierarchy.component.Create(
+            self._active_layout, component_name, compdef.GetName()
+        )
 
         if isinstance(pins[0], EDBPadstackInstance):
             pins = [i._edb_padstackinstance for i in pins]
         for pin in pins:
             pin.SetIsLayoutPin(True)
             new_cmp.AddMember(pin)
-        new_cmp.SetComponentType(self._edb.Definition.ComponentType.Other)
+        new_cmp.SetComponentType(self._edb.definition.ComponentType.Other)
         if not placement_layer:
             new_cmp_layer_name = pins[0].GetPadstackDef().GetData().GetLayerNames()[0]
         else:
             new_cmp_layer_name = placement_layer
-        new_cmp_placement_layer = self._edb.Cell.Layer.FindByName(
-            self._active_layout.GetLayerCollection(), new_cmp_layer_name
-        )
+        new_cmp_placement_layer = self._edb.cell.layer.FindByName(self._layout.layer_collection, new_cmp_layer_name)
         new_cmp.SetPlacementLayer(new_cmp_placement_layer)
         hosting_component_location = pins[0].GetComponent().GetTransform()
 
         if is_rlc:
-            rlc = self._edb.Utility.Rlc()
+            rlc = self._edb.utility.utility.Rlc()
             rlc.IsParallel = is_parallel
             if r_value:
                 rlc.REnabled = True
                 rlc.R = self._get_edb_value(r_value)
             else:
                 rlc.REnabled = False
             if l_value:
@@ -1313,26 +1299,26 @@
                 rlc.LEnabled = False
             if c_value:
                 rlc.CEnabled = True
                 rlc.C = self._get_edb_value(c_value)
             else:
                 rlc.CEnabled = False
             if rlc.REnabled and not rlc.CEnabled and not rlc.CEnabled:
-                new_cmp.SetComponentType(self._edb.Definition.ComponentType.Resistor)
+                new_cmp.SetComponentType(self._edb.definition.ComponentType.Resistor)
             elif rlc.CEnabled and not rlc.REnabled and not rlc.LEnabled:
-                new_cmp.SetComponentType(self._edb.Definition.ComponentType.Capacitor)
+                new_cmp.SetComponentType(self._edb.definition.ComponentType.Capacitor)
             elif rlc.LEnabled and not rlc.REnabled and not rlc.CEnabled:
-                new_cmp.SetComponentType(self._edb.Definition.ComponentType.Inductor)
+                new_cmp.SetComponentType(self._edb.definition.ComponentType.Inductor)
             else:
-                new_cmp.SetComponentType(self._edb.Definition.ComponentType.Resistor)
+                new_cmp.SetComponentType(self._edb.definition.ComponentType.Resistor)
 
-            pin_pair = self._edb.Utility.PinPair(pins[0].GetName(), pins[1].GetName())
-            rlc_model = self._edb.Cell.Hierarchy.PinPairModel()
+            pin_pair = self._edb.utility.utility.PinPair(pins[0].GetName(), pins[1].GetName())
+            rlc_model = self._edb.cell.hierarchy._hierarchy.PinPairModel()
             rlc_model.SetPinPairRlc(pin_pair, rlc)
-            edb_rlc_component_property = self._edb.Cell.Hierarchy.RLCComponentProperty()
+            edb_rlc_component_property = self._edb.cell.hierarchy._hierarchy.RLCComponentProperty()
             if not edb_rlc_component_property.SetModel(rlc_model) or not new_cmp.SetComponentProperty(
                 edb_rlc_component_property
             ):
                 return False  # pragma no cover
         new_cmp.SetTransform(hosting_component_location)
         new_edb_comp = EDBComponent(self, new_cmp)
         self._cmp[new_cmp.GetName()] = new_edb_comp
@@ -1427,15 +1413,15 @@
                 for line in f:
                     if "subckt" in line.lower():
                         pinNames = [i.strip() for i in re.split(" |\t", line) if i]
                         pinNames.remove(pinNames[0])
                         pinNames.remove(pinNames[0])
                         break
             if len(pinNames) == pinNumber:
-                spiceMod = self._edb.Cell.Hierarchy.SPICEModel()
+                spiceMod = self._edb.cell.hierarchy._hierarchy.SPICEModel()
                 spiceMod.SetModelPath(modelpath)
                 spiceMod.SetModelName(modelname)
                 terminal = 1
                 for pn in pinNames:
                     spiceMod.AddTerminalPinPair(pn, str(terminal))
                     terminal += 1
 
@@ -1446,21 +1432,21 @@
             else:
                 self._logger.error("Wrong number of Pins")
                 return False
 
         elif model_type == "Touchstone":  # pragma: no cover
             nPortModelName = modelname
             edbComponentDef = edbComponent.GetComponentDef()
-            nPortModel = self._edb.Definition.NPortComponentModel.FindByName(edbComponentDef, nPortModelName)
+            nPortModel = self._edb.definition.NPortComponentModel.FindByName(edbComponentDef, nPortModelName)
             if nPortModel.IsNull():
-                nPortModel = self._edb.Definition.NPortComponentModel.Create(nPortModelName)
+                nPortModel = self._edb.definition.NPortComponentModel.Create(nPortModelName)
                 nPortModel.SetReferenceFile(modelpath)
                 edbComponentDef.AddComponentModel(nPortModel)
 
-            sParameterMod = self._edb.Cell.Hierarchy.SParameterModel()
+            sParameterMod = self._edb.cell.hierarchy._hierarchy.SParameterModel()
             sParameterMod.SetComponentModelName(nPortModelName)
             gndnets = filter(lambda x: "gnd" in x.lower(), componentNets)
             if len(list(gndnets)) > 0:  # pragma: no cover
                 net = gndnets[0]
             else:  # pragma: no cover
                 net = componentNets[len(componentNets) - 1]
             sParameterMod.SetReferenceNet(net)
@@ -1498,22 +1484,22 @@
             self._logger.error("No pins specified for pin group %s", group_name)
             return (False, None)
         if len([pin for pin in pins if isinstance(pin, EDBPadstackInstance)]):
             _pins = [pin._edb_padstackinstance for pin in pins]
             if _pins:
                 pins = _pins
         if group_name is None:
-            group_name = self._edb.Cell.Hierarchy.PinGroup.GetUniqueName(self._active_layout)
+            group_name = self._edb.cell.hierarchy.pin_group.GetUniqueName(self._active_layout)
         for pin in pins:
             pin.SetIsLayoutPin(True)
         forbiden_car = "-><"
         group_name = group_name.translate({ord(i): "_" for i in forbiden_car})
         pingroup = _retry_ntimes(
             10,
-            self._edb.Cell.Hierarchy.PinGroup.Create,
+            self._edb.cell.hierarchy.pin_group.Create,
             self._active_layout,
             group_name,
             convert_py_list_to_net_list(pins),
         )
         if pingroup.IsNull():
             return False
         else:
@@ -1681,48 +1667,48 @@
         --------
 
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder")
         >>> edbapp.components.set_solder_ball("A1")
 
         """
-        if not isinstance(component, self._edb.Cell.Hierarchy.Component):
+        if not isinstance(component, self._pedb.edb_api.cell.hierarchy.component):
             edb_cmp = self.get_component_by_name(component)
-            cmp = self.components[component]
+            cmp = self.instances[component]
         else:
             edb_cmp = component
-            cmp = self.components[edb_cmp.GetName()]
+            cmp = self.instances[edb_cmp.GetName()]
         if edb_cmp:
             cmp_type = edb_cmp.GetComponentType()
             if bool(not sball_diam + sball_height):
                 pin1 = list(cmp.pins.values())[0].pin
                 pin_layers = pin1.GetPadstackDef().GetData().GetLayerNames()
                 pad_params = self._padstack.get_pad_parameters(pin=pin1, layername=pin_layers[0], pad_type=0)
                 _sb_diam = min([self._get_edb_value(val).ToDouble() for val in pad_params[1]])
                 sball_diam = _sb_diam
                 sball_height = sball_diam
 
             if not sball_mid_diam:
                 sball_mid_diam = sball_diam
 
             if shape == "Cylinder":
-                sball_shape = self._edb.Definition.SolderballShape.Cylinder
+                sball_shape = self._edb.definition.SolderballShape.Cylinder
             else:
-                sball_shape = self._edb.Definition.SolderballShape.Spheroid
+                sball_shape = self._edb.definition.SolderballShape.Spheroid
 
             cmp_property = edb_cmp.GetComponentProperty().Clone()
-            if cmp_type == self._edb.Definition.ComponentType.IC:
+            if cmp_type == self._edb.definition.ComponentType.IC:
                 ic_die_prop = cmp_property.GetDieProperty().Clone()
-                ic_die_prop.SetType(self._edb.Definition.DieType.FlipChip)
+                ic_die_prop.SetType(self._edb.definition.DieType.FlipChip)
                 if chip_orientation.lower() == "chip_down":
-                    ic_die_prop.SetOrientation(self._edb.Definition.DieOrientation.ChipDown)
+                    ic_die_prop.SetOrientation(self._edb.definition.DieOrientation.ChipDown)
                 if chip_orientation.lower() == "chip_up":
-                    ic_die_prop.SetOrientation(self._edb.Definition.DieOrientation.ChipUp)
+                    ic_die_prop.SetOrientation(self._edb.definition.DieOrientation.ChipUp)
                 else:
-                    ic_die_prop.SetOrientation(self._edb.Definition.DieOrientation.ChipDown)
+                    ic_die_prop.SetOrientation(self._edb.definition.DieOrientation.ChipDown)
                 cmp_property.SetDieProperty(ic_die_prop)
 
             solder_ball_prop = cmp_property.GetSolderBallProperty().Clone()
             solder_ball_prop.SetDiameter(self._get_edb_value(sball_diam), self._get_edb_value(sball_mid_diam))
             solder_ball_prop.SetHeight(self._get_edb_value(sball_height))
 
             solder_ball_prop.SetShape(sball_shape)
@@ -1776,21 +1762,21 @@
 
         """
         if res_value is None and ind_value is None and cap_value is None:
             self.instances[componentname].is_enabled = False
             self._logger.info("No parameters passed, component %s  is disabled.", componentname)
             return True
         edb_component = self.get_component_by_name(componentname)
-        edb_rlc_component_property = self._edb.Cell.Hierarchy.RLCComponentProperty()
+        edb_rlc_component_property = self._edb.cell.hierarchy._hierarchy.RLCComponentProperty()
         component_pins = self.get_pin_from_component(componentname)
         pin_number = len(component_pins)
         if pin_number == 2:
             from_pin = component_pins[0]
             to_pin = component_pins[1]
-            rlc = self._edb.Utility.Rlc()
+            rlc = self._edb.utility.utility.Rlc()
             rlc.IsParallel = isparallel
             if res_value is not None:
                 rlc.REnabled = True
                 rlc.R = self._get_edb_value(res_value)
             else:
                 rlc.REnabled = False
             if ind_value is not None:
@@ -1799,16 +1785,16 @@
             else:
                 rlc.LEnabled = False
             if cap_value is not None:
                 rlc.CEnabled = True
                 rlc.C = self._get_edb_value(cap_value)
             else:
                 rlc.CEnabled = False
-            pin_pair = self._edb.Utility.PinPair(from_pin.GetName(), to_pin.GetName())
-            rlc_model = self._edb.Cell.Hierarchy.PinPairModel()
+            pin_pair = self._edb.utility.utility.PinPair(from_pin.GetName(), to_pin.GetName())
+            rlc_model = self._edb.cell.hierarchy._hierarchy.PinPairModel()
             rlc_model.SetPinPairRlc(pin_pair, rlc)
             if not edb_rlc_component_property.SetModel(rlc_model) or not edb_component.SetComponentProperty(
                 edb_rlc_component_property
             ):
                 self._logger.error("Failed to set RLC model on component")
                 return False
         else:
@@ -1939,17 +1925,17 @@
                     part_name = l[part_name_col]
                     if comp.partname == part_name:
                         pass
                     else:
                         pinlist = self.get_pin_from_component(refdes)
                         if not part_name in self.definitions:
                             footprint_cell = self.definitions[comp.partname]._edb_comp_def.GetFootprintCell()
-                            comp_def = self._edb.Definition.ComponentDef.Create(self._db, part_name, footprint_cell)
+                            comp_def = self._edb.definition.ComponentDef.Create(self._db, part_name, footprint_cell)
                             for pin in pinlist:
-                                self._edb.Definition.ComponentDefPin.Create(comp_def, pin.GetName())
+                                self._edb.definition.ComponentDefPin.Create(comp_def, pin.GetName())
 
                         p_layer = comp.placement_layer
                         refdes_temp = comp.refdes + "_temp"
                         comp.refdes = refdes_temp
 
                         unmount_comp_list.remove(refdes)
                         comp.edbcomponent.Ungroup(True)
@@ -2037,27 +2023,19 @@
         --------
 
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder", "project name", "release version")
         >>> edbapp.components.get_pin_from_component("R1", refdes)
 
         """
-        if not isinstance(component, self._edb.Cell.Hierarchy.Component):
-            component = self._edb.Cell.Hierarchy.Component.FindByName(self._active_layout, component)
+        if not isinstance(component, self._pedb.edb_api.cell.hierarchy.component):
+            component = self._pedb.edb_api.cell.hierarchy.component.FindByName(self._active_layout, component)
         if netName:
             if not isinstance(netName, list):
                 netName = [netName]
-            # pins = []
-            # cmp_obj = list(cmp.LayoutObjs)
-            # for p in cmp_obj:
-            #    if p.GetObjType() == 1:
-            #        if p.IsLayoutPin():
-            #            pin_net_name = p.GetNet().GetName()
-            #            if pin_net_name in netName:
-            #                pins.append(p)
             pins = [
                 p
                 for p in list(component.LayoutObjs)
                 if int(p.GetObjType()) == 1 and p.IsLayoutPin() and p.GetNet().GetName() in netName
             ]
         elif pinName:
             if not isinstance(pinName, list):
@@ -2098,18 +2076,18 @@
         >>> edbapp.components.get_aedt_pin_name(pin)
 
         """
         if isinstance(pin, EDBPadstackInstance):
             pin = pin._edb_padstackinstance
         if is_ironpython:
             name = _clr.Reference[String]()
-            pin.GetProductProperty(self._edb.ProductId.Designer, 11, name)
+            pin.GetProductProperty(self._edb.edb_api.ProductId.Designer, 11, name)
         else:
             val = String("")
-            _, name = pin.GetProductProperty(self._edb.ProductId.Designer, 11, val)
+            _, name = pin.GetProductProperty(self._edb.edb_api.ProductId.Designer, 11, val)
         name = str(name).strip("'")
         return name
 
     @pyaedt_function_handler()
     def get_pin_position(self, pin):
         """Retrieve the pin position in meters.
 
@@ -2133,15 +2111,15 @@
         """
         res, pt_pos, rot_pos = pin.GetPositionAndRotation()
 
         if pin.GetComponent().IsNull():
             transformed_pt_pos = pt_pos
         else:
             transformed_pt_pos = pin.GetComponent().GetTransform().TransformPoint(pt_pos)
-        pin_xy = self._edb.Geometry.PointData(
+        pin_xy = self._edb.geometry.point_data(
             self._get_edb_value(str(transformed_pt_pos.X.ToDouble())),
             self._get_edb_value(str(transformed_pt_pos.Y.ToDouble())),
         )
         return [pin_xy.X.ToDouble(), pin_xy.Y.ToDouble()]
 
     @pyaedt_function_handler()
     def get_pins_name_from_net(self, pin_list, net_name):
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/components_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         Returns
         -------
         dict of :class:`pyaedt.edb_core.edb_data.components_data.EDBComponent`
         """
         comp_list = [
             EDBComponent(self._pcomponents, l)
-            for l in self._pcomponents._edb.Cell.Hierarchy.Component.FindByComponentDef(
+            for l in self._pcomponents._pedb.edb_api.cell.hierarchy.component.FindByComponentDef(
                 self._pcomponents._pedb.active_layout, self.part_name
             )
         ]
         return {comp.refdes: comp for comp in comp_list}
 
     @pyaedt_function_handler
     def assign_rlc_model(self, res=None, ind=None, cap=None, is_parallel=False):
@@ -272,17 +272,15 @@
         self.edbcomponent = cmp
         self._layout_instance = None
         self._comp_instance = None
 
     @property
     def layout_instance(self):
         """Edb layout instance object."""
-        if self._layout_instance is None:
-            self._layout_instance = self._pcomponents._pedb.layout_instance
-        return self._layout_instance
+        return self._pcomponents._pedb.layout_instance
 
     @property
     def component_instance(self):
         """Edb component instance."""
         if self._comp_instance is None:
             self._comp_instance = self.layout_instance.GetLayoutObjInstance(self.edbcomponent, None)
         return self._comp_instance
@@ -423,34 +421,34 @@
         return pin_pair.rlc_values
 
     @rlc_values.setter
     def rlc_values(self, value):
         if isinstance(value, list):  # pragma no cover
             rlc_enabled = [True if i else False for i in value]
             rlc_values = [self._get_edb_value(i) for i in value]
-            model = self._edb.Cell.Hierarchy.PinPairModel()
+            model = self._edb.cell.hierarchy._hierarchy.PinPairModel()
             pin_names = list(self.pins.keys())
             for idx, i in enumerate(np.arange(len(pin_names) // 2)):
-                pin_pair = self._edb.Utility.PinPair(pin_names[idx], pin_names[idx + 1])
-                rlc = self._edb.Utility.Rlc(
+                pin_pair = self._edb.utility.utility.PinPair(pin_names[idx], pin_names[idx + 1])
+                rlc = self._edb.utility.utility.Rlc(
                     rlc_values[0], rlc_enabled[0], rlc_values[1], rlc_enabled[1], rlc_values[2], rlc_enabled[2], False
                 )
                 model.SetPinPairRlc(pin_pair, rlc)
             self._set_model(model)
 
     @property
     def value(self):
         """Retrieve discrete component value.
 
         Returns
         -------
         str
             Value. ``None`` if not an RLC Type.
         """
-        if self.model_type == "RLC":
+        if self.model_type == "RLC" and self._pin_pairs:
             pin_pair = self._pin_pairs[0]
             if len([i for i in pin_pair.rlc_enable if i]) == 1:
                 return [pin_pair.rlc_values[idx] for idx, val in enumerate(pin_pair.rlc_enable) if val][0]
             else:
                 return pin_pair.rlc_values
         elif self.model_type == "SPICEModel":
             return self.spice_model.file_path
@@ -461,19 +459,19 @@
 
     @value.setter
     def value(self, value):
         rlc_enabled = [True if i == self.type else False for i in ["Resistor", "Inductor", "Capacitor"]]
         rlc_values = [value if i == self.type else 0 for i in ["Resistor", "Inductor", "Capacitor"]]
         rlc_values = [self._get_edb_value(i) for i in rlc_values]
 
-        model = self._edb.Cell.Hierarchy.PinPairModel()
+        model = self._edb.cell.hierarchy._hierarchy.PinPairModel()
         pin_names = list(self.pins.keys())
         for idx, i in enumerate(np.arange(len(pin_names) // 2)):
-            pin_pair = self._edb.Utility.PinPair(pin_names[idx], pin_names[idx + 1])
-            rlc = self._edb.Utility.Rlc(
+            pin_pair = self._edb.utility.utility.PinPair(pin_names[idx], pin_names[idx + 1])
+            rlc = self._edb.utility.utility.Rlc(
                 rlc_values[0], rlc_enabled[0], rlc_values[1], rlc_enabled[1], rlc_values[2], rlc_enabled[2], False
             )
             model.SetPinPairRlc(pin_pair, rlc)
         self._set_model(model)
 
     @property
     def res_value(self):
@@ -645,15 +643,15 @@
         -------
         list
             List of Pins of Component.
         """
         pins = [
             p
             for p in self.edbcomponent.LayoutObjs
-            if p.GetObjType() == self._edb.Cell.LayoutObjType.PadstackInstance
+            if p.GetObjType() == self._edb.cell.layout_object_type.PadstackInstance
             and p.IsLayoutPin()
             and p.GetComponent().GetName() == self.refdes
         ]
         return pins
 
     @property
     def nets(self):
@@ -713,25 +711,25 @@
         Parameters
         ----------
         new_type : str
             Type of the component. Options are ``"Resistor"``,  ``"Inductor"``, ``"Capacitor"``,
             ``"IC"``, ``"IO"`` and ``"Other"``.
         """
         if new_type == "Resistor":
-            type_id = self._edb.Definition.ComponentType.Resistor
+            type_id = self._edb.definition.ComponentType.Resistor
         elif new_type == "Inductor":
-            type_id = self._edb.Definition.ComponentType.Inductor
+            type_id = self._edb.definition.ComponentType.Inductor
         elif new_type == "Capacitor":
-            type_id = self._edb.Definition.ComponentType.Capacitor
+            type_id = self._edb.definition.ComponentType.Capacitor
         elif new_type == "IC":
-            type_id = self._edb.Definition.ComponentType.IC
+            type_id = self._edb.definition.ComponentType.IC
         elif new_type == "IO":
-            type_id = self._edb.Definition.ComponentType.IO
+            type_id = self._edb.definition.ComponentType.IO
         elif new_type == "Other":
-            type_id = self._edb.Definition.ComponentType.Other
+            type_id = self._edb.definition.ComponentType.Other
         else:
             return
         self.edbcomponent.SetComponentType(type_id)
 
     @property
     def numpins(self):
         """Number of Pins of Component.
@@ -865,15 +863,15 @@
             for line in f:
                 if "subckt" in line.lower():
                     pinNames = [i.strip() for i in re.split(" |\t", line) if i]
                     pinNames.remove(pinNames[0])
                     pinNames.remove(pinNames[0])
                     break
         if len(pinNames) == self.numpins:
-            model = self._edb.Cell.Hierarchy.SPICEModel()
+            model = self._edb.cell.hierarchy._hierarchy.SPICEModel()
             model.SetModelPath(file_path)
             model.SetModelName(name)
             terminal = 1
             for pn in pinNames:
                 model.AddTerminalPinPair(pn, str(terminal))
                 terminal += 1
         else:  # pragma: no cover
@@ -896,21 +894,21 @@
         -------
 
         """
         if not name:
             name = get_filename_without_extension(file_path)
 
         edbComponentDef = self.edbcomponent.GetComponentDef()
-        nPortModel = self._edb.Definition.NPortComponentModel.FindByName(edbComponentDef, name)
+        nPortModel = self._edb.definition.NPortComponentModel.FindByName(edbComponentDef, name)
         if nPortModel.IsNull():
-            nPortModel = self._edb.Definition.NPortComponentModel.Create(name)
+            nPortModel = self._edb.definition.NPortComponentModel.Create(name)
             nPortModel.SetReferenceFile(file_path)
             edbComponentDef.AddComponentModel(nPortModel)
 
-        model = self._edb.Cell.Hierarchy.SParameterModel()
+        model = self._edb.cell.hierarchy._hierarchy.SParameterModel()
         model.SetComponentModelName(name)
         if reference_net:
             model.SetReferenceNet(reference_net)
         return self._set_model(model)
 
     @pyaedt_function_handler
     def assign_rlc_model(self, res=None, ind=None, cap=None, is_parallel=False):
@@ -933,21 +931,21 @@
         r_enabled = True if res else False
         l_enabled = True if ind else False
         c_enabled = True if cap else False
         res = 0 if res is None else res
         ind = 0 if ind is None else ind
         cap = 0 if cap is None else cap
         res, ind, cap = self._get_edb_value(res), self._get_edb_value(ind), self._get_edb_value(cap)
-        model = self._edb.Cell.Hierarchy.PinPairModel()
+        model = self._edb.cell.hierarchy._hierarchy.PinPairModel()
 
         pin_names = list(self.pins.keys())
         for idx, i in enumerate(np.arange(len(pin_names) // 2)):
-            pin_pair = self._edb.Utility.PinPair(pin_names[idx], pin_names[idx + 1])
+            pin_pair = self._edb.utility.utility.PinPair(pin_names[idx], pin_names[idx + 1])
 
-            rlc = self._edb.Utility.Rlc(res, r_enabled, ind, l_enabled, cap, c_enabled, is_parallel)
+            rlc = self._edb.utility.utility.Rlc(res, r_enabled, ind, l_enabled, cap, c_enabled, is_parallel)
             model.SetPinPairRlc(pin_pair, rlc)
         return self._set_model(model)
 
     @pyaedt_function_handler
     def create_clearance_on_component(self, extra_soldermask_clearance=1e-4):
         """Create a Clearance on Soldermask layer by drawing a rectangle.
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/control_file.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/control_file.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyaedt.edb_core.edb_data.edbvalue import EdbValue
-from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
+from pyaedt.edb_core.edb_data.primitives_data import cast
 from pyaedt.edb_core.general import convert_pytuple_to_nettuple
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class HfssExtentInfo:
@@ -15,22 +15,22 @@
         Inherited AEDT object.
     """
 
     def __init__(self, pedb):
         self._pedb = pedb
 
         self._hfss_extent_info_type = {
-            "BoundingBox": self._pedb.edb.Utility.HFSSExtentInfoType.BoundingBox,
-            "Conforming": self._pedb.edb.Utility.HFSSExtentInfoType.Conforming,
-            "ConvexHull": self._pedb.edb.Utility.HFSSExtentInfoType.ConvexHull,
-            "Polygon": self._pedb.edb.Utility.HFSSExtentInfoType.Polygon,
+            "BoundingBox": self._pedb.edb_api.utility.utility.HFSSExtentInfoType.BoundingBox,
+            "Conforming": self._pedb.edb_api.utility.utility.HFSSExtentInfoType.Conforming,
+            "ConvexHull": self._pedb.edb_api.utility.utility.HFSSExtentInfoType.ConvexHull,
+            "Polygon": self._pedb.edb_api.utility.utility.HFSSExtentInfoType.Polygon,
         }
         self._open_region_type = {
-            "Radiation": self._pedb.edb.Utility.OpenRegionType.Radiation,
-            "PML": self._pedb.edb.Utility.OpenRegionType.PML,
+            "Radiation": self._pedb.edb_api.utility.utility.OpenRegionType.Radiation,
+            "PML": self._pedb.edb_api.utility.utility.OpenRegionType.PML,
         }
 
     @pyaedt_function_handler
     def _get_edb_value(self, value):
         """Get EDB value."""
         return self._pedb.edb_value(value)
 
@@ -122,15 +122,15 @@
     def base_polygon(self):
         """Base polygon.
 
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitive`
         """
-        return EDBPrimitives(self._edb_hfss_extent_info.BasePolygon, self._pedb)
+        return cast(self._edb_hfss_extent_info.BasePolygon, self._pedb)
 
     @base_polygon.setter
     def base_polygon(self, value):
         info = self._edb_hfss_extent_info
         info.BasePolygon = value.primitive_object
         self._update_hfss_extent_info(info)
 
@@ -138,15 +138,15 @@
     def dielectric_base_polygon(self):
         """Dielectric base polygon.
 
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitive`
         """
-        return EDBPrimitives(self._edb_hfss_extent_info.DielectricBasePolygon, self._pedb)
+        return cast(self._edb_hfss_extent_info.DielectricBasePolygon, self._pedb)
 
     @dielectric_base_polygon.setter
     def dielectric_base_polygon(self, value):
         info = self._edb_hfss_extent_info
         info.DielectricBasePolygon = value.primitive_object
         self._update_hfss_extent_info(info)
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1722,30 +1722,30 @@
             if not name:
                 self._edb_sim_setup_info.Name = generate_unique_name("hfss")
             else:
                 self._edb_sim_setup_info.Name = name
             self._name = name
             self.hfss_solver_settings.order_basis = "mixed"
 
-            self._edb_sim_setup = self._edb.edb.Utility.HFSSSimulationSetup(self._edb_sim_setup_info)
+            self._edb_sim_setup = self._edb.edb_api.utility.utility.HFSSSimulationSetup(self._edb_sim_setup_info)
             self._update_setup()
 
     @property
     def edb_sim_setup_info(self):
         """EDB internal simulation setup object."""
         return self._edb_sim_setup_info
 
     @pyaedt_function_handler()
     def _update_setup(self):
         mesh_operations = self._edb_sim_setup_info.SimulationSettings.MeshOperations
         mesh_operations.Clear()
         for mop in self.mesh_operations.values():
             mesh_operations.Add(mop.mesh_operation)
 
-        self._edb_sim_setup = self._edb.edb.Utility.HFSSSimulationSetup(self._edb_sim_setup_info)
+        self._edb_sim_setup = self._edb.edb_api.utility.utility.HFSSSimulationSetup(self._edb_sim_setup_info)
 
         if self._name in self._edb.setups:
             self._edb.active_cell.DeleteSimulationSetup(self._name)
         self._name = self.name
         self._edb.active_cell.AddSimulationSetup(self._edb_sim_setup)
         for i in list(self._edb.active_cell.SimulationSetups):
             if i.GetSimSetupInfo().Name == self._name:
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             self._upper_elevation = self._edb_layer.GetUpperElevation()
         except:
             pass
         return self._upper_elevation
 
     @property
     def _edb(self):
-        return self._pclass._pedb.edb
+        return self._pclass._pedb.edb_api
 
     @property
     def _edb_layer(self):
         for l in self._pclass._edb_layer_list:
             if l.GetName() == self._name:
                 return l.Clone()
 
@@ -165,18 +165,18 @@
         return re.sub(r"Layer$", "", self._edb_layer.GetLayerType().ToString()).lower()
 
     @type.setter
     def type(self, new_type):
         if new_type == self.type:
             return
         if new_type == "signal":
-            self._edb_layer.SetLayerType(self._edb.Cell.LayerType.SignalLayer)
+            self._edb_layer.SetLayerType(self._edb.cell.layer_type.SignalLayer)
             self._type = new_type
         elif new_type == "dielectric":
-            self._edb_layer.SetLayerType(self._edb.Cell.LayerType.DielectricLayer)
+            self._edb_layer.SetLayerType(self._edb.cell.layer_type.DielectricLayer)
             self._type = new_type
         else:
             return
 
     @property
     def material(self):
         """Get/Set the material loss_tangent.
@@ -413,19 +413,19 @@
         -------
         ``"Ansys.Ansoft.Edb.Cell.RoughnessModel"``
 
         """
         if not self.is_stackup_layer:  # pragma: no cover
             return
         if surface == "top":
-            return self._edb_layer.GetRoughnessModel(self._pclass._pedb.edb.Cell.RoughnessModel.Region.Top)
+            return self._edb_layer.GetRoughnessModel(self._pclass._pedb.edb_api.Cell.RoughnessModel.Region.Top)
         elif surface == "bottom":
-            return self._edb_layer.GetRoughnessModel(self._pclass._pedb.edb.Cell.RoughnessModel.Region.Bottom)
+            return self._edb_layer.GetRoughnessModel(self._pclass._pedb.edb_api.Cell.RoughnessModel.Region.Bottom)
         elif surface == "side":
-            return self._edb_layer.GetRoughnessModel(self._pclass._pedb.edb.Cell.RoughnessModel.Region.Side)
+            return self._edb_layer.GetRoughnessModel(self._pclass._pedb.edb_api.Cell.RoughnessModel.Region.Side)
 
     @pyaedt_function_handler()
     def assign_roughness_model(
         self,
         model_type="huray",
         huray_radius="0.5um",
         huray_surface_ratio="2.9",
@@ -459,35 +459,35 @@
         surface_ratio = self._pclass._edb_value(huray_surface_ratio)
         self._hurray_surface_ratio = huray_surface_ratio
         groisse_roughness = self._pclass._edb_value(groisse_roughness)
         regions = []
         if apply_on_surface == "all":
             self._side_roughness = "all"
             regions = [
-                self._pclass._pedb.edb.Cell.RoughnessModel.Region.Top,
-                self._pclass._pedb.edb.Cell.RoughnessModel.Region.Side,
-                self._pclass._pedb.edb.Cell.RoughnessModel.Region.Bottom,
+                self._pclass._pedb.edb_api.Cell.RoughnessModel.Region.Top,
+                self._pclass._pedb.edb_api.Cell.RoughnessModel.Region.Side,
+                self._pclass._pedb.edb_api.Cell.RoughnessModel.Region.Bottom,
             ]
         elif apply_on_surface == "top":
             self._side_roughness = "top"
-            regions = [self._pclass._pedb.edb.Cell.RoughnessModel.Region.Top]
+            regions = [self._pclass._pedb.edb_api.Cell.RoughnessModel.Region.Top]
         elif apply_on_surface == "bottom":
             self._side_roughness = "bottom"
-            regions = [self._pclass._pedb.edb.Cell.RoughnessModel.Region.Bottom]
+            regions = [self._pclass._pedb.edb_api.Cell.RoughnessModel.Region.Bottom]
         elif apply_on_surface == "side":
             self._side_roughness = "side"
-            regions = [self._pclass._pedb.edb.Cell.RoughnessModel.Region.Side]
+            regions = [self._pclass._pedb.edb_api.Cell.RoughnessModel.Region.Side]
 
         layer_clone = self._edb_layer
         layer_clone.SetRoughnessEnabled(True)
         for r in regions:
             if model_type == "huray":
-                model = self._pclass._pedb.edb.Cell.HurrayRoughnessModel(radius, surface_ratio)
+                model = self._pclass._pedb.edb_api.Cell.HurrayRoughnessModel(radius, surface_ratio)
             else:
-                model = self._pclass._pedb.edb.Cell.GroisseRoughnessModel(groisse_roughness)
+                model = self._pclass._pedb.edb_api.Cell.GroisseRoughnessModel(groisse_roughness)
             layer_clone.SetRoughnessModel(r, model)
         return self._pclass._set_layout_stackup(layer_clone, "change_attribute")
 
     @pyaedt_function_handler()
     def _json_format(self):
         dict_out = {}
         self._color = self.color
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,14 @@
         return self._pedbpadstack._padstack_methods
 
     @property
     def _stackup_layers(self):
         return self._pedbpadstack._stackup_layers
 
     @property
-    def _builder(self):
-        return self._pedbpadstack._builder
-
-    @property
     def _edb(self):
         return self._pedbpadstack._edb
 
     def _get_edb_value(self, value):
         return self._pedbpadstack._get_edb_value(value)
 
     @property
@@ -333,15 +329,15 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         originalPadstackDefinitionData = self._edb_padstack.GetData()
-        newPadstackDefinitionData = self._edb.Definition.PadstackDefData(originalPadstackDefinitionData)
+        newPadstackDefinitionData = self._edb.definition.PadstackDefData(originalPadstackDefinitionData)
         if not pad_type:
             pad_type = self.pad_type
         if not geom_type:
             geom_type = self.geometry_type
         if params:
             params = convert_py_list_to_net_list(params)
         else:
@@ -408,18 +404,14 @@
         return self._ppadstack._padstack_methods
 
     @property
     def _stackup_layers(self):
         return self._ppadstack._stackup_layers
 
     @property
-    def _builder(self):
-        return self._ppadstack._builder
-
-    @property
     def _edb(self):
         return self._ppadstack._edb
 
     def _get_edb_value(self, value):
         return self._ppadstack._get_edb_value(value)
 
     @property
@@ -494,15 +486,15 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         originalPadstackDefinitionData = self.edb_padstack.GetData()
-        newPadstackDefinitionData = self._edb.Definition.PadstackDefData(originalPadstackDefinitionData)
+        newPadstackDefinitionData = self._edb.definition.PadstackDefData(originalPadstackDefinitionData)
         if not hole_type:
             hole_type = self.hole_type
         if not params:
             params = self.hole_parameters
         if isinstance(params, list):
             params = convert_py_list_to_net_list(params)
         if not offsetx:
@@ -608,20 +600,20 @@
         """Hole plating ratio.
 
         Returns
         -------
         float
             Percentage for the hole plating.
         """
-        return self._edb.Definition.PadstackDefData(self.edb_padstack.GetData()).GetHolePlatingPercentage()
+        return self._edb.definition.PadstackDefData(self.edb_padstack.GetData()).GetHolePlatingPercentage()
 
     @hole_plating_ratio.setter
     def hole_plating_ratio(self, ratio):
         originalPadstackDefinitionData = self.edb_padstack.GetData()
-        newPadstackDefinitionData = self._edb.Definition.PadstackDefData(originalPadstackDefinitionData)
+        newPadstackDefinitionData = self._edb.definition.PadstackDefData(originalPadstackDefinitionData)
         newPadstackDefinitionData.SetHolePlatingPercentage(self._get_edb_value(ratio))
         self.edb_padstack.SetData(newPadstackDefinitionData)
 
     @property
     def hole_plating_thickness(self):
         """Hole plating thickness.
 
@@ -671,15 +663,15 @@
             Material of the hole.
         """
         return self.edb_padstack.GetData().GetMaterial()
 
     @material.setter
     def material(self, materialname):
         originalPadstackDefinitionData = self.edb_padstack.GetData()
-        newPadstackDefinitionData = self._edb.Definition.PadstackDefData(originalPadstackDefinitionData)
+        newPadstackDefinitionData = self._edb.definition.PadstackDefData(originalPadstackDefinitionData)
         newPadstackDefinitionData.SetMaterial(materialname)
         self.edb_padstack.SetData(newPadstackDefinitionData)
 
     @property
     def padstack_instances(self):
         """Get all the vias that belongs to active Padstack definition.
 
@@ -707,15 +699,15 @@
 
         Returns
         -------
         bool
         """
         if self.via_start_layer == self.via_stop_layer:
             self._ppadstack._pedb.logger.error("Microvias cannot be applied when Start and Stop Layers are the same.")
-        layout = self._ppadstack._pedb._active_layout
+        layout = self._ppadstack._pedb.active_layout
         layers = self._ppadstack._pedb.stackup.signal_layers
         layer_names = [i for i in list(layers.keys())]
         if convert_only_signal_vias:
             signal_nets = [i for i in list(self._ppadstack._pedb.nets.signal_nets.keys())]
         topl, topz, bottoml, bottomz = self._ppadstack._pedb.stackup.stackup_limits(True)
         start_elevation = layers[self.via_start_layer].lower_elevation
         diel_thick = abs(start_elevation - layers[self.via_stop_layer].upper_elevation)
@@ -726,73 +718,73 @@
             rad1, rad2 = rad2, rad1
         i = 0
         for via in list(self.padstack_instances.values()):
             if convert_only_signal_vias and via.net_name in signal_nets or not convert_only_signal_vias:
                 pos = via.position
                 started = False
                 if len(self.pad_by_layer[self.via_start_layer].parameters) == 0:
-                    self._edb.Cell.Primitive.Polygon.Create(
+                    self._edb.cell.primitive.polygon.create(
                         layout,
                         self.via_start_layer,
                         via._edb_padstackinstance.GetNet(),
                         self.pad_by_layer[self.via_start_layer].polygon_data,
                     )
                 else:
-                    self._edb.Cell.Primitive.Circle.Create(
+                    self._edb.cell.primitive.circle.create(
                         layout,
                         self.via_start_layer,
                         via._edb_padstackinstance.GetNet(),
                         self._get_edb_value(pos[0]),
                         self._get_edb_value(pos[1]),
                         self._get_edb_value(self.pad_by_layer[self.via_start_layer].parameters_values[0] / 2),
                     )
                 if len(self.pad_by_layer[self.via_stop_layer].parameters) == 0:
-                    self._edb.Cell.Primitive.Polygon.Create(
+                    self._edb.cell.primitive.polygon.create(
                         layout,
                         self.via_stop_layer,
                         via._edb_padstackinstance.GetNet(),
                         self.pad_by_layer[self.via_stop_layer].polygon_data,
                     )
                 else:
-                    self._edb.Cell.Primitive.Circle.Create(
+                    self._edb.cell.primitive.circle.create(
                         layout,
                         self.via_stop_layer,
                         via._edb_padstackinstance.GetNet(),
                         self._get_edb_value(pos[0]),
                         self._get_edb_value(pos[1]),
                         self._get_edb_value(self.pad_by_layer[self.via_stop_layer].parameters_values[0] / 2),
                     )
                 for layer_name in layer_names:
                     stop = ""
                     if layer_name == via.start_layer or started:
                         start = layer_name
                         stop = layer_names[layer_names.index(layer_name) + 1]
-                        cloned_circle = self._edb.Cell.Primitive.Circle.Create(
+                        cloned_circle = self._edb.cell.primitive.circle.create(
                             layout,
                             start,
                             via._edb_padstackinstance.GetNet(),
                             self._get_edb_value(pos[0]),
                             self._get_edb_value(pos[1]),
                             self._get_edb_value(rad1),
                         )
-                        cloned_circle2 = self._edb.Cell.Primitive.Circle.Create(
+                        cloned_circle2 = self._edb.cell.primitive.circle.create(
                             layout,
                             stop,
                             via._edb_padstackinstance.GetNet(),
                             self._get_edb_value(pos[0]),
                             self._get_edb_value(pos[1]),
                             self._get_edb_value(rad2),
                         )
-                        s3d = self._edb.Cell.Hierarchy.Structure3D.Create(
+                        s3d = self._edb.cell.hierarchy._hierarchy.Structure3D.Create(
                             layout, generate_unique_name("via3d_" + via.aedt_name.replace("via_", ""), n=3)
                         )
-                        s3d.AddMember(cloned_circle)
-                        s3d.AddMember(cloned_circle2)
+                        s3d.AddMember(cloned_circle.prim_obj)
+                        s3d.AddMember(cloned_circle2.prim_obj)
                         s3d.SetMaterial(self.material)
-                        s3d.SetMeshClosureProp(self._edb.Cell.Hierarchy.Structure3D.TClosure.EndsClosed)
+                        s3d.SetMeshClosureProp(self._edb.cell.hierarchy._hierarchy.Structure3D.TClosure.EndsClosed)
                         started = True
                         i += 1
                     if stop == via.stop_layer:
                         break
                 via.delete()
         self._ppadstack._pedb.logger.info("{} Converted successfully to 3D Objects.".format(i))
         return True
@@ -803,15 +795,15 @@
 
         Returns
         -------
         List of :class:`pyaedt.edb_core.padstackEDBPadstack`
         """
         if self.via_start_layer == self.via_stop_layer:
             self._ppadstack._pedb.logger.error("Microvias cannot be applied when Start and Stop Layers are the same.")
-        layout = self._ppadstack._pedb._active_layout
+        layout = self._ppadstack._pedb.active_layout
         layers = self._ppadstack._pedb.stackup.signal_layers
         layer_names = [i for i in list(layers.keys())]
         if abs(layer_names.index(self.via_start_layer) - layer_names.index(self.via_stop_layer)) < 2:
             self._ppadstack._pedb.logger.error(
                 "Conversion can be applied only if Padstack definition is composed by more than 2 layers."
             )
             return False
@@ -821,21 +813,21 @@
         for layer_name in layer_names:
             stop = ""
             if layer_name == self.via_start_layer or started:
                 start = layer_name
                 stop = layer_names[layer_names.index(layer_name) + 1]
                 new_padstack_name = "MV_{}_{}_{}".format(self.name, start, stop)
                 included = [start, stop]
-                new_padstack_definition_data = self._ppadstack._pedb.edb.Definition.PadstackDefData.Create()
+                new_padstack_definition_data = self._ppadstack._pedb.edb_api.definition.PadstackDefData.Create()
                 new_padstack_definition_data.AddLayers(convert_py_list_to_net_list(included))
                 for layer in included:
                     pl = self.pad_by_layer[layer]
                     new_padstack_definition_data.SetPadParameters(
                         layer,
-                        self._ppadstack._pedb.edb.Definition.PadType.RegularPad,
+                        self._ppadstack._pedb.edb_api.definition.PadType.RegularPad,
                         pl.int_to_geometry_type(pl.geometry_type),
                         list(
                             pl._edb_padstack.GetData().GetPadParametersValue(
                                 pl.layer_name, pl.int_to_pad_type(pl.pad_type)
                             )
                         )[2],
                         pl._edb_padstack.GetData().GetPadParametersValue(
@@ -847,15 +839,15 @@
                         pl._edb_padstack.GetData().GetPadParametersValue(
                             pl.layer_name, pl.int_to_pad_type(pl.pad_type)
                         )[5],
                     )
                     pl = self.antipad_by_layer[layer]
                     new_padstack_definition_data.SetPadParameters(
                         layer,
-                        self._ppadstack._pedb.edb.Definition.PadType.AntiPad,
+                        self._ppadstack._pedb.edb_api.definition.PadType.AntiPad,
                         pl.int_to_geometry_type(pl.geometry_type),
                         list(
                             pl._edb_padstack.GetData().GetPadParametersValue(
                                 pl.layer_name, pl.int_to_pad_type(pl.pad_type)
                             )
                         )[2],
                         pl._edb_padstack.GetData().GetPadParametersValue(
@@ -867,15 +859,15 @@
                         pl._edb_padstack.GetData().GetPadParametersValue(
                             pl.layer_name, pl.int_to_pad_type(pl.pad_type)
                         )[5],
                     )
                     pl = self.thermalpad_by_layer[layer]
                     new_padstack_definition_data.SetPadParameters(
                         layer,
-                        self._ppadstack._pedb.edb.Definition.PadType.ThermalPad,
+                        self._ppadstack._pedb.edb_api.definition.PadType.ThermalPad,
                         pl.int_to_geometry_type(pl.geometry_type),
                         list(
                             pl._edb_padstack.GetData().GetPadParametersValue(
                                 pl.layer_name, pl.int_to_pad_type(pl.pad_type)
                             )
                         )[2],
                         pl._edb_padstack.GetData().GetPadParametersValue(
@@ -893,16 +885,16 @@
                     self.hole_parameters,
                     self._get_edb_value(self.hole_offset_x),
                     self._get_edb_value(self.hole_offset_y),
                     self._get_edb_value(self.hole_rotation),
                 )
                 new_padstack_definition_data.SetMaterial(self.material)
                 new_padstack_definition_data.SetHolePlatingPercentage(self._get_edb_value(self.hole_plating_ratio))
-                padstack_definition = self._edb.Definition.PadstackDef.Create(
-                    self._ppadstack._pedb.db, new_padstack_name
+                padstack_definition = self._edb.definition.PadstackDef.Create(
+                    self._ppadstack._pedb.active_db, new_padstack_name
                 )
                 padstack_definition.SetData(new_padstack_definition_data)
                 new_instances.append(EDBPadstack(padstack_definition, self._ppadstack))
                 started = True
             if self.via_stop_layer == stop:
                 break
         i = 0
@@ -915,15 +907,15 @@
                     if l.GetName() == list(instance.GetData().GetLayerNames())[0]
                 ][0]
                 to_layer = [
                     l
                     for l in self._ppadstack._pedb.stackup._edb_layer_list
                     if l.GetName() == list(instance.GetData().GetLayerNames())[-1]
                 ][0]
-                padstack_instance = self._edb.Cell.Primitive.PadstackInstance.Create(
+                padstack_instance = self._edb.cell.primitive.padstack_instance.create(
                     layout,
                     via._edb_padstackinstance.GetNet(),
                     generate_unique_name(instance.GetName()),
                     instance,
                     via._edb_padstackinstance.GetPositionAndRotationValue()[1],
                     via._edb_padstackinstance.GetPositionAndRotationValue()[2],
                     from_layer,
@@ -953,16 +945,16 @@
     >>> from pyaedt import Edb
     >>> edb = Edb(myedb, edbversion="2021.2")
     >>> edb_padstack_instance = edb.padstacks.instances[0]
     """
 
     def __getattr__(self, key):
         try:
-            return self[key]
-        except:
+            return super().__getattribute__(key)
+        except AttributeError:
             try:
                 return getattr(self._edb_padstackinstance, key)
             except AttributeError:
                 raise AttributeError("Attribute not present")
 
     def __init__(self, edb_padstackinstance, _pedb):
         self._edb_padstackinstance = edb_padstackinstance
@@ -1068,19 +1060,19 @@
         """Backdrill layer from top.
 
         Returns
         -------
         tuple
             Tuple of the layer name and drill diameter.
         """
-        layer = self._pedb.edb.Cell.Layer("", self._pedb.edb.Cell.LayerType.SignalLayer)
+        layer = self._pedb.edb_api.cell.layer("", self._pedb.edb_api.cell.layer_type.SignalLayer)
         val = self._pedb.edb_value(0)
         if is_ironpython:  # pragma: no cover
             diameter = _clr.StrongBox[type(val)]()
-            drill_to_layer = _clr.StrongBox[self._pedb.edb.Cell.ILayerReadOnly]()
+            drill_to_layer = _clr.StrongBox[self._pedb.edb_api.Cell.ILayerReadOnly]()
             flag = self._edb_padstackinstance.GetBackDrillParametersLayerValue(drill_to_layer, diameter, False)
         else:
             (
                 flag,
                 drill_to_layer,
                 diameter,
             ) = self._edb_padstackinstance.GetBackDrillParametersLayerValue(layer, val, False)
@@ -1113,19 +1105,19 @@
         """Backdrill layer from bottom.
 
         Returns
         -------
         tuple
             Tuple of the layer name and drill diameter.
         """
-        layer = self._pedb.edb.Cell.Layer("", self._pedb.edb.Cell.LayerType.SignalLayer)
+        layer = self._pedb.edb_api.cell.layer("", self._pedb.edb_api.cell.layer_type.SignalLayer)
         val = self._pedb.edb_value(0)
         if is_ironpython:  # pragma: no cover
             diameter = _clr.StrongBox[type(val)]()
-            drill_to_layer = _clr.StrongBox[self._pedb.edb.Cell.ILayerReadOnly]()
+            drill_to_layer = _clr.StrongBox[self._pedb.edb_api.Cell.ILayerReadOnly]()
             flag = self._edb_padstackinstance.GetBackDrillParametersLayerValue(drill_to_layer, diameter, True)
         else:
             (
                 flag,
                 drill_to_layer,
                 diameter,
             ) = self._edb_padstackinstance.GetBackDrillParametersLayerValue(layer, val, True)
@@ -1158,15 +1150,15 @@
         """Starting layer.
 
         Returns
         -------
         str
             Name of the starting layer.
         """
-        layer = self._pedb.edb.Cell.Layer("", self._pedb.edb.Cell.LayerType.SignalLayer)
+        layer = self._pedb.edb_api.cell.layer("", self._pedb.edb_api.cell.layer_type.SignalLayer)
         _, start_layer, stop_layer = self._edb_padstackinstance.GetLayerRange()
 
         if start_layer:
             return start_layer.GetName()
         return None
 
     @start_layer.setter
@@ -1180,15 +1172,15 @@
         """Stopping layer.
 
         Returns
         -------
         str
             Name of the stopping layer.
         """
-        layer = self._pedb.edb.Cell.Layer("", self._pedb.edb.Cell.LayerType.SignalLayer)
+        layer = self._pedb.edb_api.cell.layer("", self._pedb.edb_api.cell.layer_type.SignalLayer)
         _, start_layer, stop_layer = self._edb_padstackinstance.GetLayerRange()
 
         if stop_layer:
             return stop_layer.GetName()
         return None
 
     @stop_layer.setter
@@ -1233,15 +1225,15 @@
         """
         return self._edb_padstackinstance.GetNet().GetName()
 
     @net_name.setter
     def net_name(self, val):
         if not isinstance(val, str):
             try:
-                self._edb_padstackinstance.SetNet(val)
+                self._edb_padstackinstance.SetNet(val.net_obj)
             except:
                 raise AttributeError("Value inserted not found. Input has to be net name or net object.")
         elif val in self._pedb.nets.netlist:
             net = self._pedb.nets.nets[val].net_object
             self._edb_padstackinstance.SetNet(net)
         else:
             raise AttributeError("Value inserted not found. Input has to be net name or net object.")
@@ -1290,27 +1282,27 @@
     def position(self, value):
         pos = []
         for v in value:
             if isinstance(v, (float, int, str)):
                 pos.append(self._pedb.edb_value(v))
             else:
                 pos.append(v)
-        point_data = self._pedb.edb.Geometry.PointData(pos[0], pos[1])
+        point_data = self._pedb.edb_api.geometry.point_data(pos[0], pos[1])
         self._edb_padstackinstance.SetPositionAndRotation(point_data, self._pedb.edb_value(self.rotation))
 
     @property
     def rotation(self):
         """Padstack instance rotation.
 
         Returns
         -------
         float
             Rotatation value for the padstack instance.
         """
-        point_data = self._pedb.edb.Geometry.PointData(self._pedb.edb_value(0.0), self._pedb.edb_value(0.0))
+        point_data = self._pedb.edb_api.geometry.point_data(self._pedb.edb_value(0.0), self._pedb.edb_value(0.0))
         out = self._edb_padstackinstance.GetPositionAndRotationValue()
 
         if out[0]:
             return out[2].ToDouble()
 
     @property
     def id(self):
@@ -1332,15 +1324,15 @@
             return "-".join([comp_name, pin_name])
         else:
             return self._edb_padstackinstance.GetName()
 
     @name.setter
     def name(self, value):
         self._edb_padstackinstance.SetName(value)
-        self._edb_padstackinstance.SetProductProperty(self._pedb.edb.ProductId.Designer, 11, value)
+        self._edb_padstackinstance.SetProductProperty(self._pedb.edb_api.ProductId.Designer, 11, value)
 
     @property
     def pin_number(self):
         """Get pin number."""
         return self._edb_padstackinstance.GetName()
 
     @property
@@ -1361,18 +1353,18 @@
         >>> from pyaedt import Edb
         >>> edbapp = Edb("myaedbfolder", "project name", "release version")
         >>> edbapp.padstacks.instances[111].get_aedt_pin_name()
 
         """
         if is_ironpython:
             name = _clr.Reference[String]()
-            self._edb_padstackinstance.GetProductProperty(self._pedb.edb.ProductId.Designer, 11, name)
+            self._edb_padstackinstance.GetProductProperty(self._pedb.edb_api.ProductId.Designer, 11, name)
         else:
             val = String("")
-            _, name = self._edb_padstackinstance.GetProductProperty(self._pedb.edb.ProductId.Designer, 11, val)
+            _, name = self._edb_padstackinstance.GetProductProperty(self._pedb.edb_api.ProductId.Designer, 11, val)
         name = str(name).strip("'")
         return name
 
     @pyaedt_function_handler()
     def parametrize_position(self, prefix=None):
         """Parametrize the instance position.
 
@@ -1428,15 +1420,15 @@
         Returns
         -------
         list
             List of the voids that include this padstack instance.
         """
         x_pos = self._pedb.edb_value(self.position[0])
         y_pos = self._pedb.edb_value(self.position[1])
-        point_data = self._pedb.modeler._edb.Geometry.PointData(x_pos, y_pos)
+        point_data = self._pedb.modeler._edb.geometry.point_data(x_pos, y_pos)
 
         voids = []
         for prim in self._pedb.modeler.get_primitives(net_name, layer_name, is_void=True):
             if prim.primitive_object.GetPolygonData().PointInPolygon(point_data):
                 voids.append(prim)
         return voids
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,175 @@
 import math
 
+from pyaedt.edb_core.dotnet.primitive import BondwireDotNet
+from pyaedt.edb_core.dotnet.primitive import CircleDotNet
+from pyaedt.edb_core.dotnet.primitive import PathDotNet
+from pyaedt.edb_core.dotnet.primitive import PolygonDotNet
+from pyaedt.edb_core.dotnet.primitive import RectangleDotNet
+from pyaedt.edb_core.dotnet.primitive import TextDotNet
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
-class EDBPrimitives(object):
+def cast(raw_primitive, core_app):
+    """Cast the primitive object to correct concrete type.
+
+    Returns
+    -------
+    Primitive
+    """
+    if isinstance(raw_primitive, RectangleDotNet):
+        return EdbRectangle(raw_primitive.prim_obj, core_app)
+    elif isinstance(raw_primitive, PolygonDotNet):
+        return EdbPolygon(raw_primitive.prim_obj, core_app)
+    elif isinstance(raw_primitive, PathDotNet):
+        return EdbPath(raw_primitive.prim_obj, core_app)
+    elif isinstance(raw_primitive, BondwireDotNet):
+        return EdbBondwire(raw_primitive.prim_obj, core_app)
+    elif isinstance(raw_primitive, TextDotNet):
+        return EdbText(raw_primitive.prim_obj, core_app)
+    elif isinstance(raw_primitive, CircleDotNet):
+        return EdbCircle(raw_primitive.prim_obj, core_app)
+    else:
+        try:
+            prim_type = raw_primitive.GetPrimitiveType()
+            if prim_type == prim_type.Rectangle:
+                return EdbRectangle(raw_primitive, core_app)
+            elif prim_type == prim_type.Polygon:
+                return EdbPolygon(raw_primitive, core_app)
+            elif prim_type == prim_type.Path:
+                return EdbPath(raw_primitive, core_app)
+            elif prim_type == prim_type.Bondwire:
+                return EdbBondwire(raw_primitive, core_app)
+            elif prim_type == prim_type.Text:
+                return EdbText(raw_primitive, core_app)
+            elif prim_type == prim_type.Circle:
+                return EdbCircle(raw_primitive, core_app)
+            else:
+                return None
+        except:
+            return None
+
+
+class EDBPrimitivesMain:
     """Manages EDB functionalities for a primitives.
     It Inherits EDB Object properties.
 
     Examples
     --------
     >>> from pyaedt import Edb
     >>> edb = Edb(myedb, edbversion="2021.2")
     >>> edb_prim = edb.modeler.primitives[0]
     >>> edb_prim.is_void # Class Property
     >>> edb_prim.IsVoid() # EDB Object Property
     """
 
-    def __getattr__(self, key):
-        try:
-            return self[key]
-        except:
-            try:
-                return getattr(self.primitive_object, key)
-            except AttributeError:
-                raise AttributeError("Attribute not present")
-
     def __init__(self, raw_primitive, core_app):
         self._app = core_app
         self._core_stackup = core_app.stackup
         self._core_net = core_app.nets
         self.primitive_object = raw_primitive
 
     @property
-    def width(self):
-        """Path width.
+    def id(self):
+        """Primitive ID.
 
         Returns
         -------
-        float
-            Path width or None.
+        int
         """
-        if self.type == "Path":
-            return self.primitive_object.GetWidth()
-        return
+        return self.GetId()
 
-    @width.setter
-    def width(self, value):
-        if self.type == "Path":
-            if isinstance(value, (int, str, float)):
-                self.primitive_object.SetWidth(self._app.edb_value(value))
-            else:
-                self.primitive_object.SetWidth(value)
+    @property
+    def type(self):
+        """Return the type of the primitive.
+        Allowed outputs are ``"Circle"``, ``"Rectangle"``,``"Polygon"``,``"Path"`` or ``"Bondwire"``.
+
+        Returns
+        -------
+        str
+        """
+        types = ["Circle", "Path", "Polygon", "Rectangle", "Bondwire"]
+        str_type = self.primitive_type.ToString().split(".")
+        if str_type[-1] in types:
+            return str_type[-1]
+        return None
+
+    @property
+    def net_name(self):
+        """Get or Set the primitive net name.
+
+        Returns
+        -------
+        str
+        """
+        return self.net.GetName()
+
+    @net_name.setter
+    def net_name(self, name):
+        if isinstance(name, str):
+            self.net.SetName(name)
+        else:
+            try:
+                self.net.SetName(name.GetName())
+            except:
+                self._app.logger.error("Failed to set net name.")
+
+    @pyaedt_function_handler()
+    def delete(self):
+        """Delete this primitive."""
+        return self.primitive_object.Delete()
+
+    @property
+    def layer(self):
+        """Get the primitive edb layer object."""
+        return self.primitive_object.GetLayer()
+
+    @property
+    def layer_name(self):
+        """Get or Set the primitive layer name.
+
+        Returns
+        -------
+        str
+        """
+        return self.layer.GetName()
+
+    @layer_name.setter
+    def layer_name(self, val):
+        if val in self._core_stackup.stackup_layers.layers:
+            lay = self._core_stackup.stackup_layers.layers[val]._edb_layer
+            self.primitive_object.SetLayer(lay)
+        elif not isinstance(val, str):
+            try:
+                self.primitive_object.SetLayer(val)
+            except:
+                raise AttributeError("Value inserted not found. Input has to be layer name or layer object.")
+        else:
+            raise AttributeError("Value inserted not found. Input has to be layer name or layer object.")
+
+
+class EDBPrimitives(EDBPrimitivesMain):
+    """Manages EDB functionalities for a primitives.
+    It Inherits EDB Object properties.
+
+    Examples
+    --------
+    >>> from pyaedt import Edb
+    >>> edb = Edb(myedb, edbversion="2021.2")
+    >>> edb_prim = edb.modeler.primitives[0]
+    >>> edb_prim.is_void # Class Property
+    >>> edb_prim.IsVoid() # EDB Object Property
+    """
+
+    def __init__(self, raw_primitive, core_app):
+        EDBPrimitivesMain.__init__(self, raw_primitive, core_app)
 
     @pyaedt_function_handler()
     def area(self, include_voids=True):
         """Return the total area.
 
         Parameters
         ----------
@@ -98,24 +209,14 @@
         """
         return self.primitive_object.GetIsNegative()
 
     @is_negative.setter
     def is_negative(self, value):
         self.primitive_object.SetIsNegative(value)
 
-    @property
-    def id(self):
-        """Primitive ID.
-
-        Returns
-        -------
-        int
-        """
-        return self.GetId()
-
     @staticmethod
     def _eval_arc_points(p1, p2, h, n=6, tol=1e-12):
         """Get the points of the arc
 
         Parameters
         ----------
         p1 : list
@@ -208,71 +309,14 @@
                 x_arc, y_arc = self._eval_arc_points(p1, p2, arc_h, num)
                 x.extend(x_arc)
                 y.extend(y_arc)
                 # i += 1
         # fmt: on
         return x, y
 
-    @pyaedt_function_handler()
-    def points(self, arc_segments=6):
-        """Return the list of points with arcs converted to segments.
-
-        Parameters
-        ----------
-        arc_segments : int
-            Number of facets to convert an arc. Default is `6`.
-
-        Returns
-        -------
-        tuple
-            The tuple contains 2 lists made of X and Y points coordinates.
-        """
-        try:
-            my_net_points = list(self.primitive_object.GetPolygonData().Points)
-            xt, yt = self._get_points_for_plot(my_net_points, arc_segments)
-            if not xt:
-                return []
-            x, y = GeometryOperators.orient_polygon(xt, yt, clockwise=True)
-            return x, y
-        except:
-            x = []
-            y = []
-        return x, y
-
-    @property
-    def voids(self):
-        """Return a list of voids of the given primitive if any.
-
-        Returns
-        -------
-        list of :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
-        """
-        voids = []
-        for void in self.primitive_object.Voids:
-            voids.append(EDBPrimitives(void, self._app))
-        return voids
-
-    @pyaedt_function_handler()
-    def points_raw(self):
-        """Return a list of Edb points.
-
-        Returns
-        -------
-        list
-            Edb Points.
-        """
-        points = []
-        try:
-            my_net_points = list(self.primitive_object.GetPolygonData().Points)
-            for point in my_net_points:
-                points.append(point)
-            return points
-        except:
-            return points
-
     @property
     def bbox(self):
         """Return the primitive bounding box points. Lower left corner, upper right corner.
 
         Returns
         -------
         list
@@ -291,118 +335,24 @@
         list
             [x, y]
 
         """
         bbox = self.bbox
         return [(bbox[0] + bbox[2]) / 2, (bbox[1] + bbox[3]) / 2]
 
-    @pyaedt_function_handler
-    def get_center_line(self, to_string=False):
-        """Get the center line of the trace.
-
-        Parameters
-        ----------
-        to_string : bool, optional
-            Type of return. The default is ``"False"``.
-        Returns
-        -------
-        list
-
-        """
-        if to_string:
-            return [[p.X.ToString(), p.Y.ToString()] for p in list(self.primitive_object.GetCenterLine().Points)]
-        else:
-            return [[p.X.ToDouble(), p.Y.ToDouble()] for p in list(self.primitive_object.GetCenterLine().Points)]
-
     @pyaedt_function_handler()
     def is_arc(self, point):
         """Either if a point is an arc or not.
 
         Returns
         -------
         bool
         """
         return point.IsArc()
 
-    @property
-    def type(self):
-        """Return the type of the primitive.
-        Allowed outputs are ``"Circle"``, ``"Rectangle"``,``"Polygon"``,``"Path"`` or ``"Bondwire"``.
-
-        Returns
-        -------
-        str
-        """
-        types = ["Circle", "Path", "Polygon", "Rectangle", "Bondwire"]
-        str_type = self.primitive_object.ToString().split(".")
-        if str_type[-1] in types:
-            return str_type[-1]
-        return None
-
-    @property
-    def net(self):
-        """Return EDB Net Object."""
-        return self.primitive_object.GetNet()
-
-    @property
-    def net_name(self):
-        """Get or Set the primitive net name.
-
-        Returns
-        -------
-        str
-        """
-        return self.net.GetName()
-
-    @net_name.setter
-    def net_name(self, val):
-        if not isinstance(val, str):
-            try:
-                self.primitive_object.SetNet(val)
-            except:
-                raise AttributeError("Value inserted not found. Input has to be layer name or net object.")
-        elif val in self._core_net.nets:
-            net = self._core_net.nets[val].net_object
-            self.primitive_object.SetNet(net)
-        else:
-            raise AttributeError("Value inserted not found. Input has to be layer name or net object.")
-
-    @property
-    def layer(self):
-        """Get the primitive edb layer object."""
-        return self.primitive_object.GetLayer()
-
-    @property
-    def layer_name(self):
-        """Get or Set the primitive layer name.
-
-        Returns
-        -------
-        str
-        """
-        return self.layer.GetName()
-
-    @layer_name.setter
-    def layer_name(self, val):
-        if val in self._core_stackup.stackup_layers.layers:
-            lay = self._core_stackup.stackup_layers.layers[val]._edb_layer
-            self.primitive_object.SetLayer(lay)
-        elif not isinstance(val, str):
-            try:
-                self.primitive_object.SetLayer(val)
-            except:
-                raise AttributeError("Value inserted not found. Input has to be layer name or layer object.")
-        else:
-            raise AttributeError("Value inserted not found. Input has to be layer name or layer object.")
-
-    @pyaedt_function_handler()
-    def delete(self):
-        """Delete this primitive."""
-        return self.primitive_object.Delete()
-
     @pyaedt_function_handler()
     def get_connected_object_id_set(self):
         """Produce a list of all geometries physically connected to a given layout object.
 
         Returns
         -------
         list
@@ -424,43 +374,14 @@
         if self.type == "Path":
             polygon_data = self.primitive_object.GetPolygonData()
             polygon = self._app.modeler.create_polygon(polygon_data, self.layer_name, [], self.net_name)
             self.primitive_object.Delete()
             return polygon
 
     @pyaedt_function_handler()
-    def add_void(self, point_list):
-        """Add a void to current primitive.
-
-        Parameters
-        ----------
-        point_list : list or  :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives` or EDB Primitive Object
-            Point list in the format of `[[x1,y1], [x2,y2],..,[xn,yn]]`.
-
-        Returns
-        -------
-        bool
-            ``True`` if successful, either  ``False``.
-        """
-        if isinstance(point_list, list):
-            plane = self._app.modeler.Shape("polygon", points=point_list)
-            _poly = self._app.modeler.shape_to_polygon_data(plane)
-            if _poly is None or _poly.IsNull() or _poly is False:
-                self._logger.error("Failed to create void polygon data")
-                return False
-            prim = self._app.edb.Cell.Primitive.Polygon.Create(
-                self._app.active_layout, self.layer_name, self.primitive_object.GetNet(), _poly
-            )
-        elif isinstance(point_list, EDBPrimitives):
-            prim = point_list.primitive_object
-        else:
-            prim = point_list
-        return self.primitive_object.AddVoid(prim)
-
-    @pyaedt_function_handler()
     def subtract(self, primitives):
         """Subtract active primitive with one or more primitives.
 
         Parameters
         ----------
         primitives : :class:`pyaedt.edb_core.edb_data.EDBPrimitives` or EDB PolygonData or EDB Primitive or list
 
@@ -487,47 +408,47 @@
             for p in list_poly:
                 if p.IsNull():
                     continue
                 list_void = []
                 void_to_subtract = []
                 if voids:
                     for void in voids:
-                        void_pdata = void.primitive_object.GetPolygonData()
+                        void_pdata = void.polygon_data
                         int_data2 = p.GetIntersectionType(void_pdata)
                         if int_data2 > 2 or int_data2 == 1:
                             void_to_subtract.append(void_pdata)
                         elif int_data2 == 2:
                             list_void.append(void_pdata)
                     if void_to_subtract:
                         polys_cleans = p.Subtract(
                             convert_py_list_to_net_list(p), convert_py_list_to_net_list(void_to_subtract)
                         )
                         for polys_clean in polys_cleans:
                             if not polys_clean.IsNull():
                                 void_to_append = [v for v in list_void if polys_clean.GetIntersectionType(v) == 2]
                                 new_polys.append(
-                                    EDBPrimitives(
+                                    cast(
                                         self._app.modeler.create_polygon(
                                             polys_clean, self.layer_name, net_name=self.net_name, voids=void_to_append
                                         ),
                                         self._app,
                                     )
                                 )
                     else:
                         new_polys.append(
-                            EDBPrimitives(
+                            cast(
                                 self._app.modeler.create_polygon(
                                     p, self.layer_name, net_name=self.net_name, voids=list_void
                                 ),
                                 self._app,
                             )
                         )
                 else:
                     new_polys.append(
-                        EDBPrimitives(
+                        cast(
                             self._app.modeler.create_polygon(
                                 p, self.layer_name, net_name=self.net_name, voids=list_void
                             ),
                             self._app,
                         )
                     )
         self.delete()
@@ -586,33 +507,33 @@
                         polys_cleans = p.Subtract(
                             convert_py_list_to_net_list(p), convert_py_list_to_net_list(void_to_subtract)
                         )
                         for polys_clean in polys_cleans:
                             if not polys_clean.IsNull():
                                 void_to_append = [v for v in list_void if polys_clean.GetIntersectionType(v) == 2]
                         new_polys.append(
-                            EDBPrimitives(
+                            cast(
                                 self._app.modeler.create_polygon(
                                     polys_clean, self.layer_name, net_name=self.net_name, voids=void_to_append
                                 ),
                                 self._app,
                             )
                         )
                     else:
                         new_polys.append(
-                            EDBPrimitives(
+                            cast(
                                 self._app.modeler.create_polygon(
                                     p, self.layer_name, net_name=self.net_name, voids=list_void
                                 ),
                                 self._app,
                             )
                         )
                 else:
                     new_polys.append(
-                        EDBPrimitives(
+                        cast(
                             self._app.modeler.create_polygon(
                                 p, self.layer_name, net_name=self.net_name, voids=list_void
                             ),
                             self._app,
                         )
                     )
         self.delete()
@@ -661,15 +582,15 @@
                 if voids:
                     for void in voids:
                         void_pdata = void.primitive_object.GetPolygonData()
                         int_data2 = p.GetIntersectionType(void_pdata)
                         if int_data2 > 1:
                             list_void.append(void_pdata)
                 new_polys.append(
-                    EDBPrimitives(
+                    cast(
                         self._app.modeler.create_polygon(p, self.layer_name, net_name=self.net_name, voids=list_void),
                         self._app,
                     )
                 )
         self.delete()
         for prim in primitives:
             if isinstance(prim, EDBPrimitives):
@@ -677,19 +598,14 @@
             else:
                 try:
                     prim.Delete()
                 except AttributeError:
                     continue
         return new_polys
 
-    @property
-    def polygon_data(self):
-        """Get the Primitive Polygon data object."""
-        return self.primitive_object.GetPolygonData()
-
     @pyaedt_function_handler()
     def intersection_type(self, primitive):
         """Get intersection type between actual primitive and another primitive or polygon data.
 
         Parameters
         ----------
         primitive : :class:`pyaeedt.edb_core.edb_data.primitives_data.EDBPrimitives` or `PolygonData`
@@ -701,16 +617,18 @@
             0 - objects do not intersect,
             1 - this object fully inside other (no common contour points),
             2 - other object fully inside this,
             3 - common contour points,
             4 - undefined intersection.
         """
         poly = primitive
-        if isinstance(primitive, EDBPrimitives):
+        try:
             poly = primitive.polygon_data
+        except AttributeError:
+            pass
         return int(self.polygon_data.GetIntersectionType(poly))
 
     @pyaedt_function_handler()
     def is_intersecting(self, primitive):
         """Check if actual primitive and another primitive or polygon data intesects.
 
         Parameters
@@ -732,15 +650,15 @@
         point : list of float or PointData
 
         Returns
         -------
         list of float
         """
         if isinstance(point, list):
-            point = self._app.edb.Geometry.PointData(self._app.edb_value(point[0]), self._app.edb_value(point[1]))
+            point = self._app.edb_api.geometry.point_data(self._app.edb_value(point[0]), self._app.edb_value(point[1]))
 
         p0 = self.polygon_data.GetClosestPoint(point)
         return [p0.X.ToDouble(), p0.Y.ToDouble()]
 
     @pyaedt_function_handler()
     def get_closest_arc_midpoint(self, point):
         """Get the closest arc midpoint of the primitive to the input data.
@@ -749,15 +667,15 @@
         ----------
         point : list of float or PointData
 
         Returns
         -------
         list of float
         """
-        if isinstance(point, self._app.edb.Geometry.PointData):
+        if isinstance(point, self._app.edb_api.geometry.geometry.PointData):
             point = [point.X.ToDouble(), point.Y.ToDouble()]
         dist = 1e12
         out = None
         for arc in self.arcs:
             mid_point = arc.mid_point
             mid_point = [mid_point.X.ToDouble(), mid_point.Y.ToDouble()]
             if GeometryOperators.points_distance(mid_point, point) < dist:
@@ -791,14 +709,119 @@
         arc = None
         for i in self.arcs:
             if i.is_segment and i.length < len:
                 arc = i
                 len = i.length
         return arc
 
+
+class EdbPath(EDBPrimitives, PathDotNet):
+    def __init__(self, raw_primitive, core_app):
+        EDBPrimitives.__init__(self, raw_primitive, core_app)
+        PathDotNet.__init__(self, self._app, raw_primitive)
+
+    @property
+    def width(self):
+        """Path width.
+
+        Returns
+        -------
+        float
+            Path width or None.
+        """
+        if self.type == "Path":
+            return self.primitive_object.GetWidth()
+        return
+
+    @width.setter
+    def width(self, value):
+        if self.type == "Path":
+            if isinstance(value, (int, str, float)):
+                self.primitive_object.SetWidth(self._app.edb_value(value))
+            else:
+                self.primitive_object.SetWidth(value)
+
+    @pyaedt_function_handler
+    def get_center_line(self, to_string=False):
+        """Get the center line of the trace.
+
+        Parameters
+        ----------
+        to_string : bool, optional
+            Type of return. The default is ``"False"``.
+        Returns
+        -------
+        list
+
+        """
+        if to_string:
+            return [[p.X.ToString(), p.Y.ToString()] for p in list(self.primitive_object.GetCenterLine().Points)]
+        else:
+            return [[p.X.ToDouble(), p.Y.ToDouble()] for p in list(self.primitive_object.GetCenterLine().Points)]
+
+    @pyaedt_function_handler
+    def clone(self):
+        """Clone a primitive object with keeping same definition and location.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+        """
+        center_line = self.center_line
+        width = self.width
+        corner_style = self.corner_style
+        end_cap_style = self.end_cap_style
+        cloned_path = self._app.edb_api.cell.primitive.path.create(
+            self._app.active_layout,
+            self.layer_name,
+            self.net,
+            width,
+            end_cap_style[1],
+            end_cap_style[2],
+            corner_style,
+            center_line,
+        )
+        if cloned_path:
+            return cloned_path
+
+
+class EdbRectangle(EDBPrimitives, RectangleDotNet):
+    def __init__(self, raw_primitive, core_app):
+        EDBPrimitives.__init__(self, raw_primitive, core_app)
+        RectangleDotNet.__init__(self, self._app, raw_primitive)
+
+
+class EdbCircle(EDBPrimitives, CircleDotNet):
+    def __init__(self, raw_primitive, core_app):
+        EDBPrimitives.__init__(self, raw_primitive, core_app)
+        CircleDotNet.__init__(self, self._app, raw_primitive)
+
+
+class EdbPolygon(EDBPrimitives, PolygonDotNet):
+    def __init__(self, raw_primitive, core_app):
+        EDBPrimitives.__init__(self, raw_primitive, core_app)
+        PolygonDotNet.__init__(self, self._app, raw_primitive)
+
+    @pyaedt_function_handler
+    def clone(self):
+        """Clone a primitive object with keeping same definition and location.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+        """
+        cloned_poly = self._app.edb_api.cell.primitive.polygon.create(
+            self._app.active_layout, self.layer_name, self.net, self.polygon_data
+        )
+        if cloned_poly:
+            return cloned_poly
+        return False
+
     @pyaedt_function_handler()
     def in_polygon(
         self,
         point_data,
         include_partial=True,
     ):
         """Check if padstack Instance is in given polygon data.
@@ -811,15 +834,15 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         if isinstance(point_data, list):
-            point_data = self._app.edb.Geometry.PointData(
+            point_data = self._app.edb_api.geometry.point_data(
                 self._app.edb_value(point_data[0]), self._app.edb_value(point_data[1])
             )
         int_val = int(self.polygon_data.PointInPolygon(point_data))
 
         # Intersection type:
         # 0 = objects do not intersect
         # 1 = this object fully inside other (no common contour points)
@@ -830,46 +853,54 @@
         elif include_partial:
             return True
         elif int_val < 3:
             return True
         else:
             return False
 
-    @pyaedt_function_handler
-    def clone(self):
-        """Clone a primitive object with keeping same definition and location.
+    # @pyaedt_function_handler()
+    # def add_void(self, point_list):
+    #     """Add a void to current primitive.
+    #
+    #     Parameters
+    #     ----------
+    #     point_list : list or  :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives` or EDB Primitive Object
+    #         Point list in the format of `[[x1,y1], [x2,y2],..,[xn,yn]]`.
+    #
+    #     Returns
+    #     -------
+    #     bool
+    #         ``True`` if successful, either  ``False``.
+    #     """
+    #     if isinstance(point_list, list):
+    #         plane = self._app.modeler.Shape("polygon", points=point_list)
+    #         _poly = self._app.modeler.shape_to_polygon_data(plane)
+    #         if _poly is None or _poly.IsNull() or _poly is False:
+    #             self._logger.error("Failed to create void polygon data")
+    #             return False
+    #         prim = self._app.edb_api.cell.primitive.polygon.create(
+    #             self._app.active_layout, self.layer_name, self.primitive_object.GetNet(), _poly
+    #         )
+    #     elif isinstance(point_list, EDBPrimitives):
+    #         prim = point_list.primitive_object
+    #     else:
+    #         prim = point_list
+    #     return self.add_void(prim)
 
-        Returns
-        -------
-        bool
-            ``True`` when successful, ``False`` when failed.
-        """
-        if self.type == "Path":
-            center_line = self.primitive_object.GetCenterLine()
-            width = self.primitive_object.GetWidthValue()
-            corner_style = self.primitive_object.GetCornerStyle()
-            end_cap_style = self.primitive_object.GetEndCapStyle()
-            cloned_path = self._app.edb.Cell.Primitive.Path.Create(
-                self._app.active_layout,
-                self.layer_name,
-                self.net,
-                width,
-                end_cap_style[1],
-                end_cap_style[2],
-                corner_style,
-                center_line,
-            )
-            if cloned_path:
-                return cloned_path
-        cloned_poly = self._app.edb.Cell.Primitive.Polygon.Create(
-            self._app.active_layout, self.layer_name, self.net, self.polygon_data
-        )
-        if cloned_poly:
-            return cloned_poly
-        return False
+
+class EdbText(EDBPrimitivesMain, TextDotNet):
+    def __init__(self, raw_primitive, core_app):
+        TextDotNet.__init__(self, self._app, raw_primitive)
+        EDBPrimitives.__init__(self, raw_primitive, core_app)
+
+
+class EdbBondwire(EDBPrimitivesMain, BondwireDotNet):
+    def __init__(self, raw_primitive, core_app):
+        BondwireDotNet.__init__(self, self._app, raw_primitive)
+        EDBPrimitives.__init__(self, raw_primitive, core_app)
 
 
 class EDBArcs(object):
     """Manages EDB Arc Data functionalities.
     It Inherits EDB primitives arcs properties.
 
     Examples
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         self._signal_nets = []
         self._power_nets = []
         self._components = []
         self._cutout_subdesign_type = CutoutSubdesignType.Conformal  # Conformal
         self._cutout_subdesign_expansion = 0.001
         self._cutout_subdesign_round_corner = True
         self._use_default_cutout = True
+        self._generate_excitations = True
+        self._add_frequency_sweep = True
+        self._include_only_selected_nets = False
         self._generate_solder_balls = True
         self._coax_solder_ball_diameter = []
         self._use_default_coax_port_radial_extension = True
         self._trim_reference_size = False
         self._output_aedb = None
         self._signal_layers_properties = {}
         self._coplanar_instances = []
@@ -557,14 +560,66 @@
         return self._signal_layers_properties
 
     @signal_layers_properties.setter
     def signal_layers_properties(self, value):  # pragma: no cover
         if isinstance(value, dict):
             self._signal_layers_properties = value
 
+    @property
+    def generate_excitations(self):
+        """Activate ports and sources for DC generation when build project with the class.
+
+        Returns
+        -------
+        bool
+            ``True`` ports are created, ``False`` skip port generation. Default value is ``True``.
+
+        """
+        return self._generate_excitations
+
+    @generate_excitations.setter
+    def generate_excitations(self, value):
+        if isinstance(value, bool):
+            self._generate_excitations = value
+
+    @property
+    def add_frequency_sweep(self):
+        """Activate the frequency sweep creation when build project with the class.
+
+        Returns
+        -------
+        bool
+            ``True`` frequency sweep is created, ``False`` skip sweep adding. Default value is ``True``.
+
+        """
+        return self._add_frequency_sweep
+
+    @add_frequency_sweep.setter
+    def add_frequency_sweep(self, value):
+        if isinstance(value, bool):
+            self._add_frequency_sweep = value
+
+    @property
+    def include_only_selected_nets(self):
+        """Include only net selection in the project. It is only used when ``do_cutout`` is set to ``False``.
+        Will also be ignored if signal_nets and power_nets are ``None``, resulting project will have all nets included.
+
+        Returns
+        -------
+        bool
+            ``True`` or ``False``. Default value is ``False``.
+
+        """
+        return self._include_only_selected_nets
+
+    @include_only_selected_nets.setter
+    def include_only_selected_nets(self, value):
+        if isinstance(value, bool):
+            self._include_only_selected_nets = value
+
 
 class SimulationConfigurationDc(object):
     """Contains all DC analysis settings.
     The class is part of `SimulationConfiguration` class as a property.
 
     """
 
@@ -2211,18 +2266,18 @@
 
         Returns
         -------
         :class:`pyaedt.edb_core_edb_data.simulationconfiguration.SimulationConfigurationBatch`
         """
         return self._batch_solve_settings
 
+    @pyaedt_function_handler()
     def build_simulation_project(self):
         """Build active simulation project. This method requires to be run inside Edb Class."""
-        if self._pedb:
-            return self._pedb.build_simulation_project(self)
+        return self._pedb.build_simulation_project(self)
 
     @property
     def solver_type(self):  # pragma: no cover
         """Retrieve the SolverType class to select the solver to be called during the project build.
 
         Returns
         -------
@@ -2315,14 +2370,17 @@
                 self.signal_layers_properties.update({lp[0]: [lp[1], lp[2], lp[3], lp[4], lp[5]]})
             except:
                 print("Missing parameter for layer {0}".format(lp[0]))
 
     def _read_cfg(self):  # pragma: no cover
         """Configuration file reader.
 
+        .. deprecated:: 0.6.78
+           Use :func:`import_json` instead.
+
         Examples
         --------
 
         >>> from pyaedt import Edb
         >>> from pyaedt.edb_core.edb_data.simulation_configuration import SimulationConfiguration
         >>> config_file = path_configuration_file
         >>> source_file = path_to_edb_folder
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -709,18 +709,18 @@
     @property
     def edb_sim_setup_info(self):
         """EDB internal simulation setup object."""
         return self._edb_sim_setup_info
 
     @pyaedt_function_handler()
     def _update_setup(self):
-        self._edb_sim_setup = self._edb.edb.Utility.SIWaveSimulationSetup(self._edb_sim_setup_info)
+        self._edb_sim_setup = self._edb.edb_api.utility.utility.SIWaveSimulationSetup(self._edb_sim_setup_info)
         if self.name in self._edb.setups:
-            self._edb._active_layout.GetCell().DeleteSimulationSetup(self.name)
-        self._edb._active_layout.GetCell().AddSimulationSetup(self._edb_sim_setup)
+            self._edb.layout.cell.DeleteSimulationSetup(self.name)
+        self._edb.layout.cell.AddSimulationSetup(self._edb_sim_setup)
         return True
 
     @property
     def dc_settings(self):
         """Siwave DC settings.
 
         Returns
@@ -953,17 +953,17 @@
     @property
     def edb_sim_setup_info(self):
         """EDB internal simulation setup object."""
         return self._edb_sim_setup_info
 
     @pyaedt_function_handler()
     def _update_setup(self):
-        edb_sim_setup = self._edb.edb.Utility.SIWaveDCIRSimulationSetup(self._edb_sim_setup_info)
+        edb_sim_setup = self._edb.edb_api.utility.utility.SIWaveDCIRSimulationSetup(self._edb_sim_setup_info)
         if self.name in self._edb.setups:
-            self._edb._active_layout.GetCell().DeleteSimulationSetup(self.name)
+            self._edb.layout.cell.DeleteSimulationSetup(self.name)
         self._edb.active_cell.AddSimulationSetup(edb_sim_setup)
         return True
 
     @property
     def name(self):
         """Setup name."""
         return self._edb_sim_setup_info.Name
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 
 # from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.edb_core.edb_data.nets_data import EDBNetsData
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstackInstance
-from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
+from pyaedt.edb_core.edb_data.primitives_data import cast
 from pyaedt.generic.constants import NodeType
 from pyaedt.generic.constants import SourceType
 
 
 class Node(object):
     """Provides for handling nodes for Siwave sources."""
 
@@ -283,44 +283,44 @@
     @pyaedt_function_handler()
     def _create_terminal(self, is_reference=False):
         pg_term = self._edb_pin_group.GetPinGroupTerminal()
         pin_group_net = self._edb_pin_group.GetNet()
         if pin_group_net.IsNull():  # pragma: no cover
             pin_group_net = list(self._edb_pin_group.GetPins())[0].GetNet()
         if pg_term.IsNull():
-            return self._pedb.edb.Cell.Terminal.PinGroupTerminal.Create(
+            return self._pedb.edb_api.cell.terminal.PinGroupTerminal.Create(
                 self._active_layout,
                 pin_group_net,
                 self.name,
                 self._edb_pin_group,
                 is_reference,
             )
         else:
             return pg_term
 
     @pyaedt_function_handler()
     def create_current_source_terminal(self, magnitude=1, phase=0):
         terminal = self._create_terminal()
-        terminal.SetBoundaryType(self._pedb.edb.Cell.Terminal.BoundaryType.kCurrentSource)
+        terminal.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.kCurrentSource)
         terminal.SetSourceAmplitude(self._pedb.edb_value(magnitude))
-        terminal.SetSourcePhase(self._pedb.edb.Utility.Value(phase))
+        terminal.SetSourcePhase(self._pedb.edb_api.utility.value(phase))
         return terminal
 
     @pyaedt_function_handler()
     def create_voltage_source_terminal(self, magnitude=1, phase=0):
         terminal = self._create_terminal()
-        terminal.SetBoundaryType(self._pedb.edb.Cell.Terminal.BoundaryType.kVoltageSource)
+        terminal.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.kVoltageSource)
         terminal.SetSourceAmplitude(self._pedb.edb_value(magnitude))
-        terminal.SetSourcePhase(self._pedb.edb.Utility.Value(phase))
+        terminal.SetSourcePhase(self._pedb.edb_api.utility.value(phase))
         return terminal
 
     @pyaedt_function_handler()
     def create_port_terminal(self, impedance=50):
         terminal = self._create_terminal()
-        terminal.SetBoundaryType(self._pedb.edb.Cell.Terminal.BoundaryType.PortBoundary)
+        terminal.SetBoundaryType(self._pedb.edb_api.cell.terminal.BoundaryType.PortBoundary)
         terminal.SetImpedance(self._pedb.edb_value(impedance))
         terminal.SetIsCircuitPort(True)
         return terminal
 
     @pyaedt_function_handler()
     def delete(self):
         """Delete active pin group.
@@ -486,15 +486,15 @@
     def __init__(self, pedb, edb_terminal):
         self._pedb = pedb
         self._edb_terminal = edb_terminal
         self._reference_object = None
 
     @property
     def _edb(self):
-        return self._pedb.edb
+        return self._pedb.edb_api
 
     @property
     def name(self):
         """Port Name.
 
         Returns
         -------
@@ -551,26 +551,26 @@
         -------
         :class:`pyaedt.edb_core.edb_data.padstacks_data.EDBPadstackInstance` or
         :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
         """
         if not self._reference_object:
             term = self._edb_terminal
             try:
-                if self.terminal_type == self._pedb.edb.Cell.Terminal.TerminalType.EdgeTerminal:
+                if self.terminal_type == self._pedb.edb_api.cell.terminal.TerminalType.EdgeTerminal:
                     edges = self._edb_terminal.GetEdges()
                     edgeType = edges[0].GetEdgeType()
-                    if edgeType == self._pedb.edb.Cell.Terminal.EdgeType.PadEdge:
+                    if edgeType == self._pedb.edb_api.cell.terminal.EdgeType.PadEdge:
                         self._reference_object = self.get_pad_edge_terminal_reference_pin()
                     else:
                         self._reference_object = self.get_edge_terminal_reference_primitive()
-                elif self.terminal_type == self._pedb.edb.Cell.Terminal.TerminalType.PinGroupTerminal:
+                elif self.terminal_type == self._pedb.edb_api.cell.terminal.TerminalType.PinGroupTerminal:
                     self._reference_object = self.get_pin_group_terminal_reference_pin()
-                elif self.terminal_type == self._pedb.edb.Cell.Terminal.TerminalType.PointTerminal:
+                elif self.terminal_type == self._pedb.edb_api.cell.terminal.TerminalType.PointTerminal:
                     self._reference_object = self.get_point_terminal_reference_primitive()
-                elif self.terminal_type == self._pedb.edb.Cell.Terminal.TerminalType.PadstackInstanceTerminal:
+                elif self.terminal_type == self._pedb.edb_api.cell.terminal.TerminalType.PadstackInstanceTerminal:
                     self._reference_object = self.get_padstack_terminal_reference_pin()
                 else:
                     self._pedb.logger.warning(
                         "Invalid Terminal Type={}".format(term.GetTerminalType())
                     )  # pragma: no cover
             except:
                 pass
@@ -622,22 +622,25 @@
 
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.padstack_data.EDBPadstackInstance`
         """
 
         refTerm = self._edb_terminal.GetReferenceTerminal()
-        if self._edb_terminal.GetTerminalType() == self._pedb.edb.Cell.Terminal.TerminalType.PinGroupTerminal:
+        if self._edb_terminal.GetTerminalType() == self._pedb.edb_api.cell.terminal.TerminalType.PinGroupTerminal:
             padStackInstance = self._edb_terminal.GetPinGroup().GetPins()[0]
             pingroup = refTerm.GetPinGroup()
             refPinList = pingroup.GetPins()
             return self._get_closest_pin(padStackInstance, refPinList, gnd_net_name_preference)
-        elif self._edb_terminal.GetTerminalType() == self._pedb.edb.Cell.Terminal.TerminalType.PadstackInstanceTerminal:
+        elif (
+            self._edb_terminal.GetTerminalType()
+            == self._pedb.edb_api.cell.terminal.TerminalType.PadstackInstanceTerminal
+        ):
             _, padStackInstance, layer = self._edb_terminal.GetParameters()
-            if refTerm.GetTerminalType() == self._pedb.edb.Cell.Terminal.TerminalType.PinGroupTerminal:
+            if refTerm.GetTerminalType() == self._pedb.edb_api.cell.terminal.TerminalType.PinGroupTerminal:
                 pingroup = refTerm.GetPinGroup()
                 refPinList = pingroup.GetPins()
                 return self._get_closest_pin(padStackInstance, refPinList, gnd_net_name_preference)
             else:
                 try:
                     returnOK, refTermPSI, layer = refTerm.GetParameters()
                     return EDBPadstackInstance(refTermPSI, self._pedb)
@@ -656,21 +659,21 @@
         """
 
         ref_layer = self._edb_terminal.GetReferenceLayer()
         edges = self._edb_terminal.GetEdges()
         _, prim_value, point_data = edges[0].GetParameters()
         X = point_data.X
         Y = point_data.Y
-        shape_pd = self._pedb.edb.Geometry.PointData(X, Y)
+        shape_pd = self._pedb.edb_api.geometry.point_data(X, Y)
         layer_name = ref_layer.GetName()
-        for primitive in self._pedb.active_layout.Primitives:
+        for primitive in self._pedb.layout.primitives:
             if primitive.GetLayer().GetName() == layer_name or not layer_name:
                 prim_shape_data = primitive.GetPolygonData()
                 if prim_shape_data.PointInPolygon(shape_pd):
-                    return EDBPrimitives(primitive, self._pedb)
+                    return cast(primitive, self._pedb)
         return None  # pragma: no cover
 
     @pyaedt_function_handler()
     def get_point_terminal_reference_primitive(self):
         """Find and return the primitive reference for the point terminal or the padstack instance.
 
         Returns
@@ -679,21 +682,21 @@
         :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
         """
 
         ref_term = self._edb_terminal.GetReferenceTerminal()  # return value is type terminal
         _, point_data, layer = ref_term.GetParameters()
         X = point_data.X
         Y = point_data.Y
-        shape_pd = self._pedb.edb.Geometry.PointData(X, Y)
+        shape_pd = self._pedb.edb_api.geometry.point_data(X, Y)
         layer_name = layer.GetName()
-        for primitive in self._pedb.active_layout.Primitives:
+        for primitive in self._pedb.layout.primitives:
             if primitive.GetLayer().GetName() == layer_name:
                 prim_shape_data = primitive.GetPolygonData()
                 if prim_shape_data.PointInPolygon(shape_pd):
-                    return EDBPrimitives(primitive, self._pedb)
+                    return cast(primitive, self._pedb)
         for vias in self._pedb.padstacks.instances.values():
             if layer_name in vias.layer_range_names:
                 plane = self._pedb.modeler.Shape(
                     "rectangle", pointA=vias.position, pointB=vias.padstack_definition.bounding_box[1]
                 )
                 rectangle_data = vias._pedb.modeler.shape_to_polygon_data(plane)
                 if rectangle_data.PointInPolygon(shape_pd):
@@ -775,20 +778,20 @@
     """
 
     def __init__(self, pedb, edb_terminal):
         CommonExcitation.__init__(self, pedb, edb_terminal)
 
     @property
     def _edb_properties(self):
-        p = self._edb_terminal.GetProductSolverOption(self._edb.ProductId.Designer, "HFSS")
+        p = self._edb_terminal.GetProductSolverOption(self._edb.edb_api.ProductId.Designer, "HFSS")
         return p
 
     @_edb_properties.setter
     def _edb_properties(self, value):
-        self._edb_terminal.SetProductSolverOption(self._edb.ProductId.Designer, "HFSS", value)
+        self._edb_terminal.SetProductSolverOption(self._edb.edb_api.ProductId.Designer, "HFSS", value)
 
     @property
     def hfss_type(self):
         """HFSS port type."""
         temp = re.search(r"'HFSS Type'='.*?'", self._edb_properties)
         if temp:
             txt = temp.group()
@@ -951,24 +954,24 @@
     @property
     def magnitude(self):
         """Get the magnitude of the source."""
         return self._edb_terminal.GetSourceAmplitude().ToDouble()
 
     @magnitude.setter
     def magnitude(self, value):
-        self._edb_terminal.SetSourceAmplitude(self._edb.Utility.Value(value))
+        self._edb_terminal.SetSourceAmplitude(self._edb.utility.value(value))
 
     @property
     def phase(self):
         """Get the phase of the source."""
         return self._edb_terminal.GetSourcePhase().ToDouble()
 
     @phase.setter
     def phase(self, value):
-        self._edb_terminal.SetSourcePhase(self._edb.Utility.Value(value))
+        self._edb_terminal.SetSourcePhase(self._edb.utility.value(value))
 
 
 class ExcitationProbes(CommonExcitation):
     """Manage probes properties.
 
     Parameters
     ----------
@@ -1002,15 +1005,15 @@
     def name(self):
         """Port Name."""
         return self._edb_bundle_terminal.GetName()
 
     @property
     def edb(self):  # pragma: no cover
         """Get edb."""
-        return self._pedb.edb
+        return self._pedb.edb_api
 
     @property
     def terminals(self):
         """Get terminals belonging to this excitation."""
         return {i.GetName(): ExcitationPorts(self._pedb, i) for i in list(self._edb_bundle_terminal.GetTerminals())}
 
     @property
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,20 +80,14 @@
         if isinstance(value, float):
             self._occupying_surface = value
 
     @property
     def layout_size(self):
         return self._layout_size
 
-    @layout_size.setter
-    def layout_size(self, value):
-        if isinstance(value, list):
-            if len([pt for pt in value if isinstance(pt, float)]) == len(value):
-                self._layout_size = value
-
     @property
     def num_polygons(self):
         return self._nb_polygons
 
     @num_polygons.setter
     def num_polygons(self, value):
         if isinstance(value, int):
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.79/pyaedt/edb_core/edb_data/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             return True
 
     @property
     def _var_server(self):
         if self._is_design_varible:
             return self._pedb.active_cell.GetVariableServer()
         else:
-            return self._pedb.db.GetVariableServer()
+            return self._pedb.active_db.GetVariableServer()
 
     @property
     def name(self):
         """Get the name of this variable."""
         return self._name
 
     @property
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/general.py` & `pyaedt-0.6.79/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.79/pyaedt/edb_core/hfss.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,31 +46,31 @@
     def _edb(self):
         """EDB object.
 
         Returns
         -------
         Ansys.Ansoft.Edb
         """
-        return self._pedb.edb
+        return self._pedb.edb_api
 
     @property
     def _active_layout(self):
         return self._pedb.active_layout
 
     @property
+    def _layout(self):
+        return self._pedb.layout
+
+    @property
     def _cell(self):
         return self._pedb.cell
 
     @property
     def _db(self):
-        return self._pedb.db
-
-    @property
-    def _builder(self):
-        return self._pedb.builder
+        return self._pedb.active_db
 
     @property
     def excitations(self):
         """Get all excitations."""
         return self._pedb.excitations
 
     @property
@@ -105,25 +105,25 @@
             Whether it is a reference terminal. The default is ``False``.
         Returns
         -------
         Edb.Cell.Terminal.EdgeTerminal
         """
         if not terminal_name:
             terminal_name = generate_unique_name("Terminal_")
-        if not isinstance(point_on_edge, self._edb.Geometry.PointData):
-            point_on_edge = self._edb.Geometry.PointData(
+        if isinstance(point_on_edge, (list, tuple)):
+            point_on_edge = self._edb.geometry.point_data(
                 self._get_edb_value(point_on_edge[0]), self._get_edb_value(point_on_edge[1])
             )
         if hasattr(prim_id, "GetId"):
             prim = prim_id
         else:
             prim = [i for i in self._pedb.modeler.primitives if i.id == prim_id][0].primitive_object
-        pos_edge = self._edb.Cell.Terminal.PrimitiveEdge.Create(prim, point_on_edge)
-        pos_edge = convert_py_list_to_net_list(pos_edge, self._edb.Cell.Terminal.Edge)
-        return self._edb.Cell.Terminal.EdgeTerminal.Create(
+        pos_edge = self._edb.cell.terminal.PrimitiveEdge.Create(prim, point_on_edge)
+        pos_edge = convert_py_list_to_net_list(pos_edge, self._edb.cell.terminal.Edge)
+        return self._edb.cell.terminal.EdgeTerminal.Create(
             prim.GetLayout(), prim.GetNet(), terminal_name, pos_edge, isRef=is_ref
         )
 
     @pyaedt_function_handler()
     def get_trace_width_for_traces_with_ports(self):
         """Retrieve the trace width for traces with ports.
 
@@ -451,15 +451,15 @@
                         res,
                         from_layer_pos,
                         to_layer_pos,
                     ) = py_inst.pin.GetLayerRange()
                     if (
                         res
                         and from_layer_pos
-                        and self._edb.Cell.Terminal.PadstackInstanceTerminal.Create(
+                        and self._edb.cell.terminal.PadstackInstanceTerminal.Create(
                             self._active_layout,
                             py_inst.pin.GetNet(),
                             port_name,
                             py_inst.pin,
                             to_layer_pos,
                         )
                     ):
@@ -533,17 +533,17 @@
             negative_primitive_id,
             negative_points_on_edge,
             horizontal_extent_factor=horizontal_extent_factor,
             vertical_extent_factor=vertical_extent_factor,
             pec_launch_width=pec_launch_width,
         )
         edb_list = convert_py_list_to_net_list(
-            [pos_term._edb_terminal, neg_term._edb_terminal], self._edb.Cell.Terminal.Terminal
+            [pos_term._edb_terminal, neg_term._edb_terminal], self._edb.cell.terminal.Terminal
         )
-        _edb_boundle_terminal = self._edb.Cell.Terminal.BundleTerminal.Create(edb_list)
+        _edb_boundle_terminal = self._edb.cell.terminal.BundleTerminal.Create(edb_list)
         return port_name, ExcitationDifferential(self._pedb, _edb_boundle_terminal)
 
     @pyaedt_function_handler
     def create_bundle_wave_port(
         self,
         primitives_id,
         points_on_edge,
@@ -596,16 +596,16 @@
                 horizontal_extent_factor=horizontal_extent_factor,
                 vertical_extent_factor=vertical_extent_factor,
                 pec_launch_width=pec_launch_width,
             )
             _port_name = None
             terminals.append(term)
 
-        edb_list = convert_py_list_to_net_list([i._edb_terminal for i in terminals], self._edb.Cell.Terminal.Terminal)
-        _edb_bundle_terminal = self._edb.Cell.Terminal.BundleTerminal.Create(edb_list)
+        edb_list = convert_py_list_to_net_list([i._edb_terminal for i in terminals], self._edb.cell.terminal.Terminal)
+        _edb_bundle_terminal = self._edb.cell.terminal.BundleTerminal.Create(edb_list)
         return port_name, ExcitationBundle(self._pedb, _edb_bundle_terminal)
 
     @pyaedt_function_handler()
     def create_hfss_ports_on_padstack(self, pinpos, portname=None):
         """Create an HFSS port on a padstack.
 
         Parameters
@@ -621,15 +621,15 @@
         bool
             ``True`` when successful, ``False`` when failed.
         """
         res, fromLayer_pos, toLayer_pos = pinpos.GetLayerRange()
 
         if not portname:
             portname = generate_unique_name("Port_" + pinpos.GetNet().GetName())
-        edbpointTerm_pos = self._edb.Cell.Terminal.PadstackInstanceTerminal.Create(
+        edbpointTerm_pos = self._edb.cell.terminal.PadstackInstanceTerminal.Create(
             self._active_layout, pinpos.GetNet(), portname, pinpos, toLayer_pos
         )
         if edbpointTerm_pos:
             return True
         else:
             return False
 
@@ -680,15 +680,15 @@
         ports.
 
         Examples
         --------
 
         >>> edb_path = path_to_edb
         >>> edb = Edb(edb_path)
-        >>> poly_list = [poly for poly in list(edb.active_layout.Primitives) if poly.GetPrimitiveType() == 2]
+        >>> poly_list = [poly for poly in list(edb.layout.primitives) if poly.GetPrimitiveType() == 2]
         >>> port_poly = [poly for poly in poly_list if poly.GetId() == 17][0]
         >>> ref_poly = [poly for poly in poly_list if poly.GetId() == 19][0]
         >>> port_location = [-65e-3, -13e-3]
         >>> ref_location = [-63e-3, -13e-3]
         >>> edb.hfss.create_edge_port_on_polygon(polygon=port_poly, reference_polygon=ref_poly,
         >>> terminal_point=port_location, reference_point=ref_location)
 
@@ -699,40 +699,40 @@
         if reference_layer:
             reference_layer = self._pedb.stackup.signal_layers[reference_layer]._edb_layer
             if not reference_layer:
                 self._logger.error("Specified layer for port {} creation was not found".format(port_name))
         if not isinstance(terminal_point, list):
             self._logger.error("Terminal point must be a list of float with providing the point location in meter")
             return False
-        terminal_point = self._edb.Geometry.PointData(
+        terminal_point = self._edb.geometry.point_data(
             self._get_edb_value(terminal_point[0]), self._get_edb_value(terminal_point[1])
         )
         if reference_point and isinstance(reference_point, list):
-            reference_point = self._edb.Geometry.PointData(
+            reference_point = self._edb.geometry.point_data(
                 self._get_edb_value(reference_point[0]), self._get_edb_value(reference_point[1])
             )
         if not port_name:
             port_name = generate_unique_name("Port_")
-        edge = self._edb.Cell.Terminal.PrimitiveEdge.Create(polygon, terminal_point)
-        edges = convert_py_list_to_net_list(edge, self._edb.Cell.Terminal.Edge)
-        edge_term = self._edb.Cell.Terminal.EdgeTerminal.Create(
+        edge = self._edb.cell.terminal.PrimitiveEdge.Create(polygon.prim_obj, terminal_point)
+        edges = convert_py_list_to_net_list(edge, self._edb.cell.terminal.Edge)
+        edge_term = self._edb.cell.terminal.EdgeTerminal.Create(
             polygon.GetLayout(), polygon.GetNet(), port_name, edges, isRef=False
         )
         if force_circuit_port:
             edge_term.SetIsCircuitPort(True)
         else:
             edge_term.SetIsCircuitPort(False)
 
         if port_impedance:
             edge_term.SetImpedance(self._pedb.edb_value(port_impedance))
         edge_term.SetName(port_name)
         if reference_polygon and reference_point:
-            ref_edge = self._edb.Cell.Terminal.PrimitiveEdge.Create(reference_polygon, reference_point)
-            ref_edges = convert_py_list_to_net_list(ref_edge, self._edb.Cell.Terminal.Edge)
-            ref_edge_term = self._edb.Cell.Terminal.EdgeTerminal.Create(
+            ref_edge = self._edb.cell.terminal.PrimitiveEdge.Create(reference_polygon.prim_obj, reference_point)
+            ref_edges = convert_py_list_to_net_list(ref_edge, self._edb.cell.terminal.Edge)
+            ref_edge_term = self._edb.cell.terminal.EdgeTerminal.Create(
                 reference_polygon.GetLayout(), reference_polygon.GetNet(), port_name + "_ref", ref_edges, isRef=True
             )
             if reference_layer:
                 ref_edge_term.SetReferenceLayer(reference_layer)
             if force_circuit_port:
                 ref_edge_term.SetIsCircuitPort(True)
             else:
@@ -798,15 +798,15 @@
                 "HFSS('HFSS Type'='Wave'",
                 " 'Horizontal Extent Factor'='{}'".format(horizontal_extent_factor),
                 " 'Vertical Extent Factor'='{}'".format(vertical_extent_factor),
                 " 'PEC Launch Width'='{}')".format(pec_launch_width),
             ]
         )
         pos_edge_term.SetProductSolverOption(
-            self._pedb.edb.ProductId.Designer,
+            self._pedb.edb_api.ProductId.Designer,
             "HFSS",
             prop,
         )
         if pos_edge_term:
             return port_name, self._pedb.hfss.excitations[port_name]
         else:
             return False
@@ -870,15 +870,15 @@
                 " 'Layer Alignment'='Upper'",
                 " 'Horizontal Extent Factor'='{}'".format(horizontal_extent_factor),
                 " 'Vertical Extent Factor'='{}'".format(vertical_extent_factor),
                 " 'PEC Launch Width'='{}')".format(pec_launch_width),
             ]
         )
         pos_edge_term.SetProductSolverOption(
-            self._pedb.edb.ProductId.Designer,
+            self._pedb.edb_api.ProductId.Designer,
             "HFSS",
             prop,
         )
         if pos_edge_term:
             return port_name, self._pedb.hfss.excitations[port_name]
         else:
             return False
@@ -925,15 +925,15 @@
         neg_edge_term = self._create_edge_terminal(ref_prim_id, point_on_ref_edge, port_name + "_ref", is_ref=True)
 
         pos_edge_term.SetImpedance(self._pedb.edb_value(impedance))
         pos_edge_term.SetReferenceTerminal(neg_edge_term)
         if not layer_alignment == "Upper":
             layer_alignment = "Lower"
         pos_edge_term.SetProductSolverOption(
-            self._pedb.edb.ProductId.Designer,
+            self._pedb.edb_api.ProductId.Designer,
             "HFSS",
             "HFSS('HFSS Type'='Gap(coax)', Orientation='Horizontal', 'Layer Alignment'='{}')".format(layer_alignment),
         )
         if pos_edge_term:
             return port_name
         else:
             return False
@@ -969,23 +969,23 @@
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         if not isinstance(nets, list):
             if isinstance(nets, str):
-                nets = [self._edb.Cell.Net.FindByName(self._active_layout, nets)]
-            elif isinstance(nets, self._edb.Cell.Net):
+                nets = [self._edb.cell.net.find_by_name(self._active_layout, nets)]
+            elif isinstance(nets, self._edb.cell.net.net):
                 nets = [nets]
         else:
             temp_nets = []
             for nn in nets:
                 if isinstance(nn, str):
-                    temp_nets.append(self._edb.Cell.Net.FindByName(self._active_layout, nn))
-                elif isinstance(nn, self._edb.Cell.Net):
+                    temp_nets.append(self._edb.cell.net.find_by_name(self._active_layout, nn))
+                elif isinstance(nn, self._edb.cell.net.net):
                     temp_nets.append(nn)
             nets = temp_nets
         if nets:
             edges_pts = []
             if isinstance(reference_layer, str):
                 try:
                     reference_layer = self._pedb.stackup.signal_layers[reference_layer]._edb_layer
@@ -994,19 +994,19 @@
             if not isinstance(reference_layer, self._edb.Cell.ILayerReadOnly):
                 return False
             layout = nets[0].GetLayout()
             layout_bbox = self.get_layout_bounding_box(layout, digit_resolution)
             for net in nets:
                 net_primitives = list(net.Primitives)
                 net_paths = [
-                    pp for pp in net_primitives if pp.GetPrimitiveType() == self._edb.Cell.Primitive.PrimitiveType.Path
+                    pp for pp in net_primitives if pp.GetPrimitiveType() == self._edb.cell.primitive.PrimitiveType.Path
                 ]
                 for path in net_paths:
                     trace_path_pts = list(path.GetCenterLine().Points)
-                    port_name = "{}_{}".format(net.GetName(), path.GetId())
+                    port_name = "{}_{}".format(net.name, path.GetId())
                     for pt in trace_path_pts:
                         _pt = [
                             round(pt.X.ToDouble(), digit_resolution),
                             round(pt.Y.ToDouble(), digit_resolution),
                         ]
                         if at_bounding_box:
                             if not set(layout_bbox).isdisjoint(_pt):
@@ -1069,30 +1069,30 @@
                             _y.append(pt.Y.ToDouble())
                     user_defined_extent = [_x, _y]
             terminal_info = []
             for net in nets:
                 net_polygons = [
                     pp
                     for pp in net.primitives
-                    if pp.GetPrimitiveType() == self._edb.Cell.Primitive.PrimitiveType.Polygon
+                    if pp.GetPrimitiveType() == self._edb.cell.primitive.PrimitiveType.Polygon
                 ]
                 for poly in net_polygons:
                     mid_points = [[arc.mid_point.X.ToDouble(), arc.mid_point.Y.ToDouble()] for arc in poly.arcs]
                     for mid_point in mid_points:
                         if GeometryOperators.point_in_polygon(mid_point, user_defined_extent) == 0:
                             port_name = generate_unique_name("{}_{}".format(poly.GetNet().GetName(), poly.GetId()))
                             term = self._create_edge_terminal(poly.GetId(), mid_point, port_name)  # pragma no cover
                             if not term.IsNull():
                                 self._logger.info("Terminal {} created".format(term.GetName()))
                                 term.SetIsCircuitPort(True)
                                 terminal_info.append(
                                     [poly.GetNet().GetName(), mid_point[0], mid_point[1], term.GetName()]
                                 )
-                                mid_pt_data = self._edb.Geometry.PointData(
-                                    self._edb.Utility.Value(mid_point[0]), self._edb.Utility.Value(mid_point[1])
+                                mid_pt_data = self._edb.geometry.point_data(
+                                    self._edb.utility.value(mid_point[0]), self._edb.utility.value(mid_point[1])
                                 )
                                 ref_prim = [
                                     prim
                                     for prim in reference_net.primitives
                                     if prim.polygon_data.PointInPolygon(mid_pt_data)
                                 ]
                                 if not ref_prim:
@@ -1100,16 +1100,16 @@
                                     scanning_zone = [
                                         (mid_point[0] - mid_point[0] * 1e-3, mid_point[1] - mid_point[1] * 1e-3),
                                         (mid_point[0] - mid_point[0] * 1e-3, mid_point[1] + mid_point[1] * 1e-3),
                                         (mid_point[0] + mid_point[0] * 1e-3, mid_point[1] + mid_point[1] * 1e-3),
                                         (mid_point[0] + mid_point[0] * 1e-3, mid_point[1] - mid_point[1] * 1e-3),
                                     ]
                                     for new_point in scanning_zone:
-                                        mid_pt_data = self._edb.Geometry.PointData(
-                                            self._edb.Utility.Value(new_point[0]), self._edb.Utility.Value(new_point[1])
+                                        mid_pt_data = self._edb.geometry.point_data(
+                                            self._edb.utility.value(new_point[0]), self._edb.utility.value(new_point[1])
                                         )
                                         ref_prim = [
                                             prim
                                             for prim in reference_net.primitives
                                             if prim.polygon_data.PointInPolygon(mid_pt_data)
                                         ]
                                         if ref_prim:
@@ -1143,15 +1143,15 @@
         if layout == None:
             return False
         layout_obj_instances = layout.GetLayoutInstance().GetAllLayoutObjInstances()
         tuple_list = []
         for lobj in layout_obj_instances.Items:
             lobj_bbox = lobj.GetLayoutInstanceContext().GetBBox(False)
             tuple_list.append(lobj_bbox)
-        _bbox = self._edb.Geometry.PolygonData.GetBBoxOfBoxes(convert_py_list_to_net_list(tuple_list))
+        _bbox = self._edb.geometry.polygon_data.get_bbox_of_boxes(tuple_list)
         layout_bbox = [
             round(_bbox.Item1.X.ToDouble(), digit_resolution),
             round(_bbox.Item1.Y.ToDouble(), digit_resolution),
             round(_bbox.Item2.X.ToDouble(), digit_resolution),
             round(_bbox.Item2.Y.ToDouble(), digit_resolution),
         ]
         return layout_bbox
@@ -1172,21 +1172,21 @@
         """
 
         if not isinstance(simulation_setup, SimulationConfiguration):
             self._logger.error(
                 "Configure HFSS extent requires edb_data.simulation_configuration.SimulationConfiguration object"
             )
             return False
-        hfss_extent = self._edb.Utility.HFSSExtentInfo()
+        hfss_extent = self._edb.utility.utility.HFSSExtentInfo()
         if simulation_setup.radiation_box == RadiationBoxType.BoundingBox:
-            hfss_extent.ExtentType = self._edb.Utility.HFSSExtentInfoType.BoundingBox
+            hfss_extent.ExtentType = self._edb.utility.utility.HFSSExtentInfoType.BoundingBox
         elif simulation_setup.radiation_box == RadiationBoxType.Conformal:
-            hfss_extent.ExtentType = self._edb.Utility.HFSSExtentInfoType.Conforming
+            hfss_extent.ExtentType = self._edb.utility.utility.HFSSExtentInfoType.Conforming
         else:
-            hfss_extent.ExtentType = self._edb.Utility.HFSSExtentInfoType.ConvexHull
+            hfss_extent.ExtentType = self._edb.utility.utility.HFSSExtentInfoType.ConvexHull
         hfss_extent.DielectricExtentSize = convert_pytuple_to_nettuple(
             (simulation_setup.dielectric_extent, simulation_setup.use_dielectric_extent_multiple)
         )
         hfss_extent.AirBoxHorizontalExtent = convert_pytuple_to_nettuple(
             (simulation_setup.airbox_horizontal_extent, simulation_setup.use_airbox_horizontal_extent_multiple)
         )
         hfss_extent.AirBoxNegativeVerticalExtent = convert_pytuple_to_nettuple(
@@ -1200,15 +1200,15 @@
                 simulation_setup.airbox_positive_vertical_extent,
                 simulation_setup.use_airbox_positive_vertical_extent_multiple,
             )
         )
         hfss_extent.HonorUserDielectric = simulation_setup.honor_user_dielectric
         hfss_extent.TruncateAirBoxAtGround = simulation_setup.truncate_airbox_at_ground
         hfss_extent.UseOpenRegion = simulation_setup.use_radiation_boundary
-        self._active_layout.GetCell().SetHFSSExtentInfo(hfss_extent)  # returns void
+        self._layout.cell.SetHFSSExtentInfo(hfss_extent)  # returns void
         return True
 
     @pyaedt_function_handler()
     def configure_hfss_analysis_setup(self, simulation_setup=None):
         """
         Configure HFSS analysis setup.
 
@@ -1257,50 +1257,54 @@
         simsetup_info.SimulationSettings.HFSSSolverSettings.OrderBasis = simulation_setup.basis_order
         simsetup_info.SimulationSettings.HFSSSolverSettings.UseHFSSIterativeSolver = False
         simsetup_info.SimulationSettings.DefeatureSettings.UseDefeature = False  # set True when using defeature ratio
         simsetup_info.SimulationSettings.DefeatureSettings.UseDefeatureAbsLength = simulation_setup.defeature_layout
         simsetup_info.SimulationSettings.DefeatureSettings.DefeatureAbsLength = simulation_setup.defeature_abs_length
 
         try:
-            sweep = self._pedb.simsetupdata.SweepData(simulation_setup.sweep_name)
-            sweep.IsDiscrete = False
-            sweep.UseQ3DForDC = simulation_setup.use_q3d_for_dc
-            sweep.RelativeSError = simulation_setup.relative_error
-            sweep.InterpUsePortImpedance = False
-            sweep.EnforceCausality = simulation_setup.enforce_causality
-            # sweep.EnforceCausality = False
-            sweep.EnforcePassivity = simulation_setup.enforce_passivity
-            sweep.PassivityTolerance = simulation_setup.passivity_tolerance
-            sweep.Frequencies.Clear()
-
-            if simulation_setup.sweep_type == SweepType.LogCount:  # setup_info.SweepType == 'DecadeCount'
-                self._setup_decade_count_sweep(
-                    sweep,
-                    str(simulation_setup.start_freq),
-                    str(simulation_setup.stop_freq),
-                    str(simulation_setup.decade_count),
-                )  # Added DecadeCount as a new attribute
+            if simulation_setup.add_frequency_sweep:
+                self._logger.info("Adding frequency sweep")
+                sweep = self._pedb.simsetupdata.SweepData(simulation_setup.sweep_name)
+                sweep.IsDiscrete = False
+                sweep.UseQ3DForDC = simulation_setup.use_q3d_for_dc
+                sweep.RelativeSError = simulation_setup.relative_error
+                sweep.InterpUsePortImpedance = False
+                sweep.EnforceCausality = simulation_setup.enforce_causality
+                # sweep.EnforceCausality = False
+                sweep.EnforcePassivity = simulation_setup.enforce_passivity
+                sweep.PassivityTolerance = simulation_setup.passivity_tolerance
+                sweep.Frequencies.Clear()
+
+                if simulation_setup.sweep_type == SweepType.LogCount:  # setup_info.SweepType == 'DecadeCount'
+                    self._setup_decade_count_sweep(
+                        sweep,
+                        str(simulation_setup.start_freq),
+                        str(simulation_setup.stop_freq),
+                        str(simulation_setup.decade_count),
+                    )  # Added DecadeCount as a new attribute
+
+                else:
+                    sweep.Frequencies = self._pedb.simsetupdata.SweepData.SetFrequencies(
+                        simulation_setup.start_freq,
+                        simulation_setup.stop_freq,
+                        simulation_setup.step_freq,
+                    )
 
+                simsetup_info.SweepDataList.Add(sweep)
             else:
-                sweep.Frequencies = self._pedb.simsetupdata.SweepData.SetFrequencies(
-                    simulation_setup.start_freq,
-                    simulation_setup.stop_freq,
-                    simulation_setup.step_freq,
-                )
-
-            simsetup_info.SweepDataList.Add(sweep)
+                self._logger.info("Adding frequency sweep disabled")
 
         except Exception as err:
             self._logger.error("Exception in Sweep configuration: {0}".format(err))
 
-        sim_setup = self._edb.Utility.HFSSSimulationSetup(simsetup_info)
-        for setup in self._active_layout.GetCell().SimulationSetups:
-            self._active_layout.GetCell().DeleteSimulationSetup(setup.GetName())
+        sim_setup = self._edb.utility.utility.HFSSSimulationSetup(simsetup_info)
+        for setup in self._layout.cell.SimulationSetups:
+            self._layout.cell.DeleteSimulationSetup(setup.GetName())
             self._logger.warning("Setup {} has been deleted".format(setup.GetName()))
-        return self._active_layout.GetCell().AddSimulationSetup(sim_setup)
+        return self._layout.cell.AddSimulationSetup(sim_setup)
 
     def _setup_decade_count_sweep(self, sweep, start_freq="1", stop_freq="1MHz", decade_count="10"):
         start_f = GeometryOperators.parse_dim_arg(start_freq)
         if start_f == 0.0:
             start_f = 10
             self._logger.warning("Decade Count sweep does not support DC value, defaulting starting frequency to 10Hz")
 
@@ -1344,30 +1348,30 @@
         if not simulation_setup.components:  # pragma: no cover
             return
 
         layout = self._cell.GetLayout()
         l_inst = layout.GetLayoutInstance()
 
         for inst in simulation_setup.components:  # pragma: no cover
-            comp = self._edb.Cell.Hierarchy.Component.FindByName(layout, inst)
+            comp = self._pedb.edb_api.cell.hierarchy.component.FindByName(layout, inst)
             if comp.IsNull():
                 continue
 
             terms_bbox_pts = self._get_terminals_bbox(comp, l_inst, trim_to_terminals)
             if not terms_bbox_pts:
                 continue
 
-            terms_bbox = self._edb.Geometry.PolygonData.CreateFromBBox(terms_bbox_pts)
+            terms_bbox = self._edb.geometry.polygon_data.create_from_bbox(terms_bbox_pts)
 
             if trim_to_terminals:
                 # Remove any pins that aren't interior to the Terminals bbox
                 pin_list = [
                     obj
                     for obj in list(comp.LayoutObjs)
-                    if obj.GetObjType() == self._edb.Cell.LayoutObjType.PadstackInstance
+                    if obj.GetObjType() == self._edb.cell.layout_object_type.PadstackInstance
                 ]
                 for pin in pin_list:
                     loi = l_inst.GetLayoutObjInstance(pin, None)
                     bb_c = loi.GetCenter()
                     if not terms_bbox.PointInPolygon(bb_c):
                         comp.RemoveMember(pin)
 
@@ -1400,41 +1404,41 @@
 
         if not isinstance(simulation_setup, SimulationConfiguration):
             self._logger.error(
                 "Set coax port attribute requires an edb_data.simulation_configuration.SimulationConfiguration object \
             as argument."
             )
             return False
-        net_names = [net.GetName() for net in list(self._active_layout.Nets) if not net.IsPowerGround()]
+        net_names = [net.name for net in self._layout.nets if not net.IsPowerGround()]
         cmp_names = (
-            simulation_setup.components
-            if simulation_setup.components
-            else [gg.GetName() for gg in self._active_layout.Groups]
+            simulation_setup.components if simulation_setup.components else [gg.GetName() for gg in self._layout.groups]
         )
         ii = 0
         for cc in cmp_names:
-            cmp = self._edb.Cell.Hierarchy.Component.FindByName(self._active_layout, cc)
+            cmp = self._pedb.edb_api.cell.hierarchy.component.FindByName(self._active_layout, cc)
             if cmp.IsNull():
                 self._logger.warning("RenamePorts: could not find component {0}".format(cc))
                 continue
-            terms = [obj for obj in list(cmp.LayoutObjs) if obj.GetObjType() == self._edb.Cell.LayoutObjType.Terminal]
+            terms = [
+                obj for obj in list(cmp.LayoutObjs) if obj.GetObjType() == self._edb.cell.layout_object_type.Terminal
+            ]
             for nn in net_names:
                 for tt in [term for term in terms if term.GetNet().GetName() == nn]:
                     if not tt.SetImpedance(self._pedb.edb_value("50ohm")):
                         self._logger.warning("Could not set terminal {0} impedance as 50ohm".format(tt.GetName()))
                         continue
                     ii += 1
 
             if not simulation_setup.use_default_coax_port_radial_extension:
                 # Set the Radial Extent Factor
                 typ = cmp.GetComponentType()
                 if typ in [
-                    self._edb.Definition.ComponentType.Other,
-                    self._edb.Definition.ComponentType.IC,
-                    self._edb.Definition.ComponentType.IO,
+                    self._edb.definition.ComponentType.Other,
+                    self._edb.definition.ComponentType.IC,
+                    self._edb.definition.ComponentType.IO,
                 ]:
                     cmp_prop = cmp.GetComponentProperty().Clone()
                     (
                         success,
                         diam1,
                         diam2,
                     ) = cmp_prop.GetSolderBallProperty().GetDiameter()
@@ -1445,34 +1449,34 @@
                             "'Layer Alignment'='Upper', "
                             "'Horizontal Extent Factor'='5', "
                             "'Vertical Extent Factor'='3', "
                             "'Radial Extent Factor'='0.25', "
                             "'PEC Launch Width'='0mm')"
                         )
                         for tt in terms:
-                            tt.SetProductSolverOption(self._edb.ProductId.Designer, "HFSS", option)
+                            tt.SetProductSolverOption(self._edb.edb_api.ProductId.Designer, "HFSS", option)
         return True
 
     @pyaedt_function_handler()
     def _get_terminals_bbox(self, comp, l_inst, terminals_only):
         terms_loi = []
         if terminals_only:
             term_list = [
-                obj for obj in list(comp.LayoutObjs) if obj.GetObjType() == self._edb.Cell.LayoutObjType.Terminal
+                obj for obj in list(comp.LayoutObjs) if obj.GetObjType() == self._edb.cell.layout_object_type.Terminal
             ]
             for tt in term_list:
                 success, p_inst, lyr = tt.GetParameters()
                 if success and lyr:
                     loi = l_inst.GetLayoutObjInstance(p_inst, None)
                     terms_loi.append(loi)
         else:
             pin_list = [
                 obj
                 for obj in list(comp.LayoutObjs)
-                if obj.GetObjType() == self._edb.Cell.LayoutObjType.PadstackInstance
+                if obj.GetObjType() == self._edb.cell.layout_object_type.PadstackInstance
             ]
             for pi in pin_list:
                 loi = l_inst.GetLayoutObjInstance(pi, None)
                 terms_loi.append(loi)
 
         if len(terms_loi) == 0:
             return None
@@ -1482,16 +1486,18 @@
             # Need to account for the coax port dimension
             bb = loi.GetBBox()
             ll = [bb.Item1.X.ToDouble(), bb.Item1.Y.ToDouble()]
             ur = [bb.Item2.X.ToDouble(), bb.Item2.Y.ToDouble()]
             # dim = 0.26 * max(abs(UR[0]-LL[0]), abs(UR[1]-LL[1]))  # 0.25 corresponds to the default 0.5
             # Radial Extent Factor, so set slightly larger to avoid validation errors
             dim = 0.30 * max(abs(ur[0] - ll[0]), abs(ur[1] - ll[1]))  # 0.25 corresponds to the default 0.5
-            terms_bbox.append(self._edb.Geometry.PolygonData(ll[0] - dim, ll[1] - dim, ur[0] + dim, ur[1] + dim))
-        return self._edb.Geometry.PolygonData.GetBBoxOfPolygons(convert_py_list_to_net_list(terms_bbox))
+            terms_bbox.append(
+                self._edb.geometry.polygon_data.dotnetobj(ll[0] - dim, ll[1] - dim, ur[0] + dim, ur[1] + dim)
+            )
+        return self._edb.geometry.polygon_data.get_bbox_of_polygons(terms_bbox)
 
     @pyaedt_function_handler()
     def get_ports_number(self):
         """Return the total number of excitation ports in a layout.
 
         Parameters
         ----------
@@ -1499,15 +1505,15 @@
 
         Returns
         -------
         int
            Number of ports.
 
         """
-        terms = [term for term in list(self._active_layout.Terminals) if int(term.GetBoundaryType()) == 0]
+        terms = [term for term in self._layout.terminals if int(term.GetBoundaryType()) == 0]
         return len([i for i in terms if not i.IsReferenceTerminal()])
 
     @pyaedt_function_handler()
     def layout_defeaturing(self, simulation_setup=None):
         """Defeature the layout by reducing the number of points for polygons based on surface deviation criteria.
 
         Parameters
@@ -1578,17 +1584,17 @@
             ``True`` when successful, ``False`` when failed.
 
         """
 
         if positive_pin and negative_pin:
             positive_pin_term = self._pedb.components._create_terminal(positive_pin)
             negative_pin_term = self._pedb.components._create_terminal(negative_pin)
-            positive_pin_term.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.RlcBoundary)
-            negative_pin_term.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.RlcBoundary)
-            rlc = self._edb.Utility.Rlc()
+            positive_pin_term.SetBoundaryType(self._edb.cell.terminal.BoundaryType.RlcBoundary)
+            negative_pin_term.SetBoundaryType(self._edb.cell.terminal.BoundaryType.RlcBoundary)
+            rlc = self._edb.utility.utility.Rlc()
             rlc.IsParallel = True
             rlc.REnabled = True
             rlc.LEnabled = True
             rlc.CEnabled = True
             rlc.R = self._get_edb_value(rvalue)
             rlc.L = self._get_edb_value(lvalue)
             rlc.C = self._get_edb_value(cvalue)
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def write_xml(self, entry_standard):  # pragma no cover
         standard_circle = ET.SubElement(entry_standard, "Circle")
         standard_circle.set("diameter", self.diameter)
         fill = ET.SubElement(standard_circle, "FillDescRef")
         fill.set("id", self.fill_id)
 
 
-class Rectangle(object):
+class RectangleDotNet(object):
     def __init__(self):
         self.width = ""
         self.height = ""
         self.fill_id = ""
 
     def write_xml(self, entry_standard):  # pragma no cover
         standard_rectanlgle = ET.SubElement(entry_standard, "RectCenter")
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
                 bom_item.add_refdes(
                     component_name=cmp.refdes, placement_layer=cmp.placement_layer, package_def="", populate=True
                 )
             self.bom.bom_items.append(bom_item)
 
     @pyaedt_function_handler()
     def add_layers_info(self):
-        self.design_name = self._pedb._active_layout.GetCell().GetName()
+        self.design_name = self._pedb.layout.cell.GetName()
         self.ecad.design_name = self.design_name
         self.ecad.cad_header.units = self.units
         self.ecad.cad_data.stackup.total_thickness = self.from_meter_to_units(
             self._pedb.stackup.get_layout_thickness(), self.units
         )
         self.ecad.cad_data.stackup.stackup_group.thickness = self.ecad.cad_data.stackup.total_thickness
         self.layers_name = list(self._pedb.stackup.signal_layers.keys())
@@ -243,31 +243,33 @@
             layer_type = "CONDUCTOR"
             conductivity = 5e6
             permitivity = 1
             loss_tg = 0
             embedded = "NOT_EMBEDDED"
             # try:
             material_name = self._pedb.stackup.layers[layer_name]._edb_layer.GetMaterial()
-            edb_material = self._pedb.edb.Definition.MaterialDef.FindByName(self._pedb.db, material_name)
+            edb_material = self._pedb.edb_api.definition.MaterialDef.FindByName(self._pedb.active_db, material_name)
             material_type = "CONDUCTOR"
             if self._pedb.stackup.layers[layer_name].type == "dielectric":
                 layer_type = "DIELPREG"
                 material_type = "DIELECTRIC"
 
-                permitivity = edb_material.GetProperty(self._pedb.edb.Definition.MaterialPropertyId.Permittivity)[1]
+                permitivity = edb_material.GetProperty(self._pedb.edb_api.definition.MaterialPropertyId.Permittivity)[1]
                 if not isinstance(permitivity, float):
                     permitivity = permitivity.ToDouble()
-                loss_tg = edb_material.GetProperty(self._pedb.edb.Definition.MaterialPropertyId.DielectricLossTangent)[
-                    1
-                ]
+                loss_tg = edb_material.GetProperty(
+                    self._pedb.edb_api.definition.MaterialPropertyId.DielectricLossTangent
+                )[1]
                 if not isinstance(loss_tg, float):
                     loss_tg = loss_tg.ToDouble()
                 conductivity = 0
             if layer_type == "CONDUCTOR":
-                conductivity = edb_material.GetProperty(self._pedb.edb.Definition.MaterialPropertyId.Conductivity)[1]
+                conductivity = edb_material.GetProperty(self._pedb.edb_api.definition.MaterialPropertyId.Conductivity)[
+                    1
+                ]
                 if not isinstance(conductivity, float):
                     conductivity = conductivity.ToDouble()
             self.ecad.cad_header.add_spec(
                 name=layer_name,
                 material=self._pedb.stackup.layers[layer_name]._edb_layer.GetMaterial(),
                 layer_type=material_type,
                 conductivity=str(conductivity),
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.79/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/layout.py` & `pyaedt-0.6.79/pyaedt/edb_core/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """
 This module contains these classes: `EdbLayout` and `Shape`.
 """
 import math
 import warnings
 
+from pyaedt.edb_core.dotnet.primitive import BondwireDotNet
+from pyaedt.edb_core.dotnet.primitive import CircleDotNet
+from pyaedt.edb_core.dotnet.primitive import PathDotNet
+from pyaedt.edb_core.dotnet.primitive import PolygonDotNet
+from pyaedt.edb_core.dotnet.primitive import RectangleDotNet
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
+from pyaedt.edb_core.edb_data.primitives_data import cast
 from pyaedt.edb_core.edb_data.utilities import EDBStatistics
 from pyaedt.edb_core.general import convert_py_list_to_net_list
-from pyaedt.generic.clr_module import Tuple
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EdbLayout(object):
     """Manages EDB methods for primitives management accessible from `Edb.modeler` property.
@@ -24,44 +29,44 @@
     """
 
     def __init__(self, p_edb):
         self._pedb = p_edb
 
     @property
     def _edb(self):
-        return self._pedb.edb
+        return self._pedb.edb_api
 
     def _get_edb_value(self, value):
         return self._pedb.edb_value(value)
 
     @property
     def _logger(self):
         """Logger."""
         return self._pedb.logger
 
     @property
-    def _builder(self):
-        return self._pedb.builder
-
-    @property
     def _edbutils(self):
         return self._pedb.edbutils
 
     @property
     def _active_layout(self):
         return self._pedb.active_layout
 
     @property
+    def _layout(self):
+        return self._pedb.layout
+
+    @property
     def _cell(self):
         return self._pedb.active_cell
 
     @property
     def db(self):
         """Db object."""
-        return self._pedb.db
+        return self._pedb.active_db
 
     @property
     def layers(self):
         """Dictionary of layers.
 
         Returns
         -------
@@ -77,16 +82,16 @@
         Returns
         -------
         list of :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
             List of primitives.
         """
         _prims = []
         if self._active_layout:
-            for lay_obj in list(self._active_layout.Primitives):
-                _prims.append(EDBPrimitives(lay_obj, self._pedb))
+            for lay_obj in self._layout.primitives:
+                _prims.append(cast(lay_obj, self._pedb))
         return _prims
 
     @property
     def polygons_by_layer(self):
         """Primitives with layer names as keys.
 
         Returns
@@ -105,93 +110,91 @@
 
         Returns
         -------
         dict
             Dictionary of primitives with nat names as keys.
         """
         _prim_by_net = {}
-        for net in list(self._pedb.nets.nets.keys()):
-            _prim_by_net[net] = [
-                EDBPrimitives(i, self._pedb) for i in self._active_layout.Primitives if i.GetNet().GetName() == net
-            ]
+        for net, net_obj in self._pedb.nets.nets.items():
+            _prim_by_net[net] = [cast(i, self._pedb) for i in net_obj.primitives]
         return _prim_by_net
 
     @property
     def primitives_by_layer(self):
         """Primitives with layer names as keys.
 
         Returns
         -------
         dict
             Dictionary of primitives with layer names as keys.
         """
         _primitives_by_layer = {}
         for lay in self.layers:
             _primitives_by_layer[lay] = []
-        for i in self._active_layout.Primitives:
+        for i in self._layout.primitives:
             lay = i.GetLayer().GetName()
-            _primitives_by_layer[lay].append(EDBPrimitives(i, self._pedb))
+            _primitives_by_layer[lay].append(cast(i, self._pedb))
         return _primitives_by_layer
 
     @property
     def rectangles(self):
         """Rectangles.
 
         Returns
         -------
         list of :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
             List of rectangles.
 
         """
-        return [i for i in self.primitives if i.type == "Rectangle"]
+        return [i for i in self.primitives if isinstance(i, RectangleDotNet)]
 
     @property
     def circles(self):
         """Circles.
 
         Returns
         -------
         list of :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
             List of circles.
 
         """
-        return [i for i in self.primitives if i.type == "Circle"]
+        return [i for i in self.primitives if isinstance(i, CircleDotNet)]
 
     @property
     def paths(self):
         """Paths.
 
         Returns
         -------
         list of :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
             List of paths.
         """
-        return [i for i in self.primitives if i.type == "Path"]
+        return [i for i in self.primitives if isinstance(i, PathDotNet)]
 
     @property
     def bondwires(self):
         """Bondwires.
 
         Returns
         -------
         list of :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
             List of bondwires.
         """
-        return [i for i in self.primitives if i.type == "Bondwire"]
+        return [i for i in self.primitives if isinstance(i, BondwireDotNet)]
 
     @property
     def polygons(self):
         """Polygons.
 
         Returns
         -------
         list of :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
             List of polygons.
         """
-        return [i for i in self.primitives if i.type == "Polygon"]
+        return [i for i in self.primitives if isinstance(i, PolygonDotNet)]
 
     @pyaedt_function_handler()
     def get_polygons_by_layer(self, layer_name, net_list=None):
         """Retrieve polygons by a layer.
 
         Parameters
         ----------
@@ -412,48 +415,48 @@
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
             ``True`` when successful, ``False`` when failed.
         """
         net = self._pedb.nets.find_or_create_net(net_name)
         if start_cap_style.lower() == "round":
-            start_cap_style = self._edb.Cell.Primitive.PathEndCapStyle.Round
+            start_cap_style = self._edb.cell.primitive.PathEndCapStyle.Round
         elif start_cap_style.lower() == "extended":
-            start_cap_style = self._edb.Cell.Primitive.PathEndCapStyle.Extended  # pragma: no cover
+            start_cap_style = self._edb.cell.primitive.PathEndCapStyle.Extended  # pragma: no cover
         else:
-            start_cap_style = self._edb.Cell.Primitive.PathEndCapStyle.Flat  # pragma: no cover
+            start_cap_style = self._edb.cell.primitive.PathEndCapStyle.Flat  # pragma: no cover
         if end_cap_style.lower() == "round":
-            end_cap_style = self._edb.Cell.Primitive.PathEndCapStyle.Round  # pragma: no cover
+            end_cap_style = self._edb.cell.primitive.PathEndCapStyle.Round  # pragma: no cover
         elif end_cap_style.lower() == "extended":
-            end_cap_style = self._edb.Cell.Primitive.PathEndCapStyle.Extended  # pragma: no cover
+            end_cap_style = self._edb.cell.primitive.PathEndCapStyle.Extended  # pragma: no cover
         else:
-            end_cap_style = self._edb.Cell.Primitive.PathEndCapStyle.Flat
+            end_cap_style = self._edb.cell.primitive.PathEndCapStyle.Flat
         if corner_style.lower() == "round":
-            corner_style = self._edb.Cell.Primitive.PathCornerStyle.RoundCorner
+            corner_style = self._edb.cell.primitive.PathCornerStyle.RoundCorner
         elif corner_style.lower() == "sharp":
-            corner_style = self._edb.Cell.Primitive.PathCornerStyle.SharpCorner  # pragma: no cover
+            corner_style = self._edb.cell.primitive.PathCornerStyle.SharpCorner  # pragma: no cover
         else:
-            corner_style = self._edb.Cell.Primitive.PathCornerStyle.MiterCorner  # pragma: no cover
+            corner_style = self._edb.cell.primitive.PathCornerStyle.MiterCorner  # pragma: no cover
 
         pointlists = [self._pedb.point_data(i[0], i[1]) for i in path_list.points]
-        polygonData = self._edb.Geometry.PolygonData(convert_py_list_to_net_list(pointlists), False)
-        polygon = self._edb.Cell.Primitive.Path.Create(
+        polygonData = self._edb.geometry.polygon_data.dotnetobj(convert_py_list_to_net_list(pointlists), False)
+        polygon = self._edb.cell.primitive.path.create(
             self._active_layout,
             layer_name,
             net,
             self._get_edb_value(width),
             start_cap_style,
             end_cap_style,
             corner_style,
             polygonData,
         )
-        if polygon.IsNull():
+        if polygon.IsNull():  # pragma: no cover
             self._logger.error("Null path created")
             return False
-        return EDBPrimitives(polygon, self._pedb)
+        return cast(polygon, self._pedb)
 
     @pyaedt_function_handler()
     def create_trace(
         self,
         path_list,
         layer_name,
         width=1,
@@ -526,41 +529,55 @@
         Returns
         -------
         bool, :class:`pyaedt.edb_core.edb_data.primitives.EDBPrimitives`
             Polygon when successful, ``False`` when failed.
         """
         net = self._pedb.nets.find_or_create_net(net_name)
         if isinstance(main_shape, list):
-            shape = self.Shape("polygon", points=main_shape)
-            polygonData = self.shape_to_polygon_data(shape)
+            arcs = []
+            for _ in range(len(main_shape)):
+                arcs.append(
+                    self._edb.Geometry.ArcData(
+                        self._pedb.point_data(0, 0),
+                        self._pedb.point_data(0, 0),
+                    )
+                )
+            polygonData = self._edb.Geometry.PolygonData.CreateFromArcs(convert_py_list_to_net_list(arcs), True)
+
+            for idx, i in enumerate(main_shape):
+                pdata_0 = self._pedb.edb_value(i[0])
+                pdata_1 = self._pedb.edb_value(i[1])
+                new_points = self._edb.Geometry.PointData(pdata_0, pdata_1)
+                polygonData.SetPoint(idx, new_points)
+
         elif isinstance(main_shape, EdbLayout.Shape):
             polygonData = self.shape_to_polygon_data(main_shape)
         else:
             polygonData = main_shape
-        if polygonData is None or polygonData.IsNull() or polygonData is False:
+        if polygonData is False or polygonData is None or polygonData.IsNull():
             self._logger.error("Failed to create main shape polygon data")
             return False
         for void in voids:
             if isinstance(void, list):
                 void = self.Shape("polygon", points=void)
                 voidPolygonData = self.shape_to_polygon_data(void)
             elif isinstance(void, EdbLayout.Shape):
                 voidPolygonData = self.shape_to_polygon_data(void)
             else:
                 voidPolygonData = void
-            if voidPolygonData is None or voidPolygonData.IsNull() or polygonData is False:
+            if voidPolygonData is False or voidPolygonData is None or voidPolygonData.IsNull():
                 self._logger.error("Failed to create void polygon data")
                 return False
             polygonData.AddHole(voidPolygonData)
-        polygon = self._edb.Cell.Primitive.Polygon.Create(self._active_layout, layer_name, net, polygonData)
-        if polygon.IsNull() or polygonData is False:
+        polygon = self._edb.cell.primitive.polygon.create(self._active_layout, layer_name, net, polygonData)
+        if polygon.IsNull() or polygonData is False:  # pragma: no cover
             self._logger.error("Null polygon created")
             return False
         else:
-            return EDBPrimitives(polygon, self._pedb)
+            return cast(polygon, self._pedb)
 
     @pyaedt_function_handler()
     def create_polygon_from_points(self, point_list, layer_name, net_name=""):
         """Create a new polygon from a point list.
 
         .. deprecated:: 0.6.73
         Use :func:`create_polygon` method instead. It now supports point lists as arguments.
@@ -630,43 +647,43 @@
         Returns
         -------
          :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
             Rectangle when successful, ``False`` when failed.
         """
         edb_net = self._pedb.nets.find_or_create_net(net_name)
         if representation_type == "LowerLeftUpperRight":
-            rep_type = self._edb.Cell.Primitive.RectangleRepresentationType.LowerLeftUpperRight
-            rect = self._edb.Cell.Primitive.Rectangle.Create(
+            rep_type = self._edb.cell.primitive.RectangleRepresentationType.LowerLeftUpperRight
+            rect = self._edb.cell.primitive.rectangle.create(
                 self._active_layout,
                 layer_name,
-                edb_net,
+                edb_net.net_obj,
                 rep_type,
                 self._get_edb_value(lower_left_point[0]),
                 self._get_edb_value(lower_left_point[1]),
                 self._get_edb_value(upper_right_point[0]),
                 self._get_edb_value(upper_right_point[1]),
                 self._get_edb_value(corner_radius),
                 self._get_edb_value(rotation),
             )
         else:
-            rep_type = self._edb.Cell.Primitive.RectangleRepresentationType.CenterWidthHeight
-            rect = self._edb.Cell.Primitive.Rectangle.Create(
+            rep_type = self._edb.cell.primitive.RectangleRepresentationType.CenterWidthHeight
+            rect = self._edb.cell.primitive.rectangle.create(
                 self._active_layout,
                 layer_name,
-                edb_net,
+                edb_net.net_obj,
                 rep_type,
                 self._get_edb_value(center_point[0]),
                 self._get_edb_value(center_point[1]),
                 self._get_edb_value(width),
                 self._get_edb_value(height),
                 self._get_edb_value(corner_radius),
                 self._get_edb_value(rotation),
             )
         if rect:
-            return EDBPrimitives(rect, self._pedb)
+            return cast(rect, self._pedb)
         return False  # pragma: no cover
 
     @pyaedt_function_handler()
     def create_circle(self, layer_name, x, y, radius, net_name=""):
         """Create a circle on a specified layer.
 
         Parameters
@@ -686,24 +703,24 @@
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
             Objects of the circle created when successful.
         """
         edb_net = self._pedb.nets.find_or_create_net(net_name)
 
-        circle = self._edb.Cell.Primitive.Circle.Create(
+        circle = self._edb.cell.primitive.circle.create(
             self._active_layout,
             layer_name,
             edb_net,
             self._get_edb_value(x),
             self._get_edb_value(y),
             self._get_edb_value(radius),
         )
         if circle:
-            return EDBPrimitives(circle, self._pedb)
+            return cast(circle, self._pedb)
         return False  # pragma: no cover
 
     @pyaedt_function_handler
     def delete_primitives(self, net_names):
         """Delete primitives by net names.
 
         Parameters
@@ -781,15 +798,15 @@
             (
                 res,
                 center_x,
                 center_y,
                 radius,
             ) = void_circle.primitive_object.GetParameters()
 
-            cloned_circle = self._edb.Cell.Primitive.Circle.Create(
+            cloned_circle = self._edb.cell.primitive.circle.create(
                 self._active_layout,
                 void_circle.layer_name,
                 void_circle.net,
                 self._get_edb_value(center_x),
                 self._get_edb_value(center_y),
                 self._get_edb_value(radius),
             )
@@ -867,67 +884,67 @@
                 is_parametric = (
                     is_parametric
                     or startPoint[0].IsParametric()
                     or startPoint[1].IsParametric()
                     or endPoint[0].IsParametric()
                     or endPoint[1].IsParametric()
                 )
-                arc = self._edb.Geometry.ArcData(
-                    self._pedb.point_data(startPoint[0], startPoint[1]),
-                    self._pedb.point_data(endPoint[0], endPoint[1]),
+                arc = self._edb.geometry.arc_data(
+                    self._pedb.point_data(startPoint[0].ToDouble(), startPoint[1].ToDouble()),
+                    self._pedb.point_data(endPoint[0].ToDouble(), endPoint[1].ToDouble()),
                 )
                 arcs.append(arc)
             elif len(endPoint) == 3:
                 is_parametric = (
                     is_parametric
                     or startPoint[0].IsParametric()
                     or startPoint[1].IsParametric()
                     or endPoint[0].IsParametric()
                     or endPoint[1].IsParametric()
                     or endPoint[2].IsParametric()
                 )
-                arc = self._edb.Geometry.ArcData(
-                    self._pedb.point_data(startPoint[0], startPoint[1]),
-                    self._pedb.point_data(endPoint[0], endPoint[1]),
+                arc = self._edb.geometry.arc_data(
+                    self._pedb.point_data(startPoint[0].ToDouble(), startPoint[1].ToDouble()),
+                    self._pedb.point_data(endPoint[0].ToDouble(), endPoint[1].ToDouble()),
                     endPoint[2].ToDouble(),
                 )
                 arcs.append(arc)
             elif len(endPoint) == 5:
                 is_parametric = (
                     is_parametric
                     or startPoint[0].IsParametric()
                     or startPoint[1].IsParametric()
                     or endPoint[0].IsParametric()
                     or endPoint[1].IsParametric()
                     or endPoint[3].IsParametric()
                     or endPoint[4].IsParametric()
                 )
-                rotationDirection = self._edb.Geometry.RotationDirection.Colinear
+                rotationDirection = self._edb.geometry.geometry.RotationDirection.Colinear
                 if endPoint[2].ToString() == "cw":
-                    rotationDirection = self._edb.Geometry.RotationDirection.CW
+                    rotationDirection = self._edb.geometry.geometry.RotationDirection.CW
                 elif endPoint[2].ToString() == "ccw":
-                    rotationDirection = self._edb.Geometry.RotationDirection.CCW
+                    rotationDirection = self._edb.geometry.geometry.RotationDirection.CCW
                 else:
                     self._logger.error("Invalid rotation direction %s is specified.", endPoint[2])
                     return None
-                arc = self._edb.Geometry.ArcData(
-                    self._pedb.point_data(startPoint[0], startPoint[1]),
-                    self._pedb.point_data(endPoint[0], endPoint[1]),
+                arc = self._edb.geometry.arc_data(
+                    self._pedb.point_data(startPoint[0].ToDouble(), startPoint[1].ToDouble()),
+                    self._pedb.point_data(endPoint[0].ToDouble(), endPoint[1].ToDouble()),
                     rotationDirection,
-                    self._pedb.point_data(endPoint[3], endPoint[4]),
+                    self._pedb.point_data(endPoint[3].ToDouble(), endPoint[4].ToDouble()),
                 )
                 arcs.append(arc)
-        polygon = self._edb.Geometry.PolygonData.CreateFromArcs(convert_py_list_to_net_list(arcs), True)
+        polygon = self._edb.geometry.polygon_data.create_from_arcs(arcs, True)
         if not is_parametric:
             return polygon
         else:
             k = 0
             for pt in points:
                 point = [self._get_edb_value(i) for i in pt]
-                new_points = self._edb.Geometry.PointData(point[0], point[1])
+                new_points = self._edb.geometry.point_data(point[0], point[1])
                 if len(point) > 2:
                     k += 1
                 polygon.SetPoint(k, new_points)
                 k += 1
         return polygon
 
     @pyaedt_function_handler()
@@ -937,62 +954,61 @@
                 self._logger.error("Point X value must be a number.")
                 return False
             if not isinstance(point[1], (int, float, str)):
                 self._logger.error("Point Y value must be a number.")
                 return False
             return True
         elif len(point) == 3:
-            if not allowArcs:
+            if not allowArcs:  # pragma: no cover
                 self._logger.error("Arc found but arcs are not allowed in _validatePoint.")
                 return False
-            if not isinstance(point[0], (int, float, str)):
+            if not isinstance(point[0], (int, float, str)):  # pragma: no cover
                 self._logger.error("Point X value must be a number.")
                 return False
-            if not isinstance(point[1], (int, float, str)):
+            if not isinstance(point[1], (int, float, str)):  # pragma: no cover
                 self._logger.error("Point Y value must be a number.")
                 return False
-            if not isinstance(point[1], (int, float, str)):
+            if not isinstance(point[1], (int, float, str)):  # pragma: no cover
                 self._logger.error("Invalid point height.")
                 return False
             return True
         elif len(point) == 5:
-            if not allowArcs:
+            if not allowArcs:  # pragma: no cover
                 self._logger.error("Arc found but arcs are not allowed in _validatePoint.")
                 return False
-            if not isinstance(point[0], (int, float, str)):
+            if not isinstance(point[0], (int, float, str)):  # pragma: no cover
                 self._logger.error("Point X value must be a number.")
                 return False
-            if not isinstance(point[1], (int, float, str)):
+            if not isinstance(point[1], (int, float, str)):  # pragma: no cover
                 self._logger.error("Point Y value must be a number.")
                 return False
             if not isinstance(point[2], str) or point[2] not in ["cw", "ccw"]:
                 self._logger.error("Invalid rotation direction {} is specified.")
                 return False
-            if not isinstance(point[3], (int, float, str)):
+            if not isinstance(point[3], (int, float, str)):  # pragma: no cover
                 self._logger.error("Arc center point X value must be a number.")
                 return False
-            if not isinstance(point[4], (int, float, str)):
+            if not isinstance(point[4], (int, float, str)):  # pragma: no cover
                 self._logger.error("Arc center point Y value must be a number.")
                 return False
             return True
-        else:
+        else:  # pragma: no cover
             self._logger.error("Arc point descriptor has incorrect number of elements (%s)", len(point))
             return False
 
     def _createPolygonDataFromRectangle(self, shape):
         if not self._validatePoint(shape.pointA, False) or not self._validatePoint(shape.pointB, False):
             return None
-        pointA = self._edb.Geometry.PointData(
+        pointA = self._edb.geometry.point_data(
             self._get_edb_value(shape.pointA[0]), self._get_edb_value(shape.pointA[1])
         )
-        pointB = self._edb.Geometry.PointData(
+        pointB = self._edb.geometry.point_data(
             self._get_edb_value(shape.pointB[0]), self._get_edb_value(shape.pointB[1])
         )
-        points = Tuple[self._edb.Geometry.PointData, self._edb.Geometry.PointData](pointA, pointB)
-        return self._edb.Geometry.PolygonData.CreateFromBBox(points)
+        return self._edb.geometry.polygon_data.create_from_bbox((pointA, pointB))
 
     class Shape(object):
         """Shape class.
 
         Parameters
         ----------
         type : str, optional
@@ -1113,24 +1129,24 @@
                             poly_by_nets[poly.GetNet().GetName()] = [poly]
                     else:
                         if poly.GetNet().GetName():
                             poly_by_nets[poly.GetNet().GetName()].append(poly)
             for net in poly_by_nets:
                 list_polygon_data = [i.GetPolygonData() for i in poly_by_nets[net]]
                 all_voids = [i.Voids for i in poly_by_nets[net]]
-                a = self._edb.Geometry.PolygonData.Unite(convert_py_list_to_net_list(list_polygon_data))
+                a = self._edb.geometry.polygon_data.unite(convert_py_list_to_net_list(list_polygon_data))
                 for item in a:
                     for v in all_voids:
                         for void in v:
                             if int(item.GetIntersectionType(void.GetPolygonData())) == 2:
                                 item.AddHole(void.GetPolygonData())
-                    poly = self._edb.Cell.Primitive.Polygon.Create(
+                    poly = self._edb.cell.primitive.polygon.create(
                         self._active_layout,
                         lay,
-                        self._pedb.nets.nets[net].net_object,
+                        self._pedb.nets.nets[net],
                         item,
                     )
                 list_to_delete = [i for i in poly_by_nets[net]]
                 for v in all_voids:
                     for void in v:
                         for poly in poly_by_nets[net]:
                             if int(void.GetPolygonData().GetIntersectionType(poly.GetPolygonData())) >= 2:
@@ -1148,110 +1164,34 @@
             for pad in self._pedb.padstacks.definitions:
                 p1 = self._pedb.padstacks.definitions[pad].edb_padstack.GetData()
                 if len(p1.GetLayerNames()) > 1:
                     self._pedb.padstacks.remove_pads_from_padstack(pad)
         return True
 
     @pyaedt_function_handler()
-    def defeature_polygon(self, setup_info, poly, max_surface_deviation=0.001):
+    def defeature_polygon(self, poly, tolerance=0.001):
         """Defeature the polygon based on the maximum surface deviation criteria.
 
         Parameters
         ----------
-        setup_info : EDB_Data_SimulatiomConfiguratio object
-            When the ``setup_info`` argument is provided, it overwrites the
-            ``maximum_surface_deviation`` value.
-
+        maximum_surface_deviation : float
         poly : Edb Polygon primitive
             Polygon to defeature.
-
-        max_surface_deviation : float, optional
-            Maximum surface deviation criteria. The default is ``0.001``.
+        tolerance : float, optional
+            Maximum tolerance criteria. The default is ``0.001``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
-        try:
-            if setup_info:
-                max_surface_deviation = setup_info.max_suf_dev
-            poly_data = poly.GetPolygonData()
-            pts_list = []
-            pts = poly_data.Points
-            defeaturing_step = 1e-6
-            if len(poly_data) <= 16:
-                # Defeaturing skipped for polygons with less than 16 points
-                self._logger.info(
-                    "Polygon {} is skipped for defeaturing because its number of point is less than 16. ".format(
-                        poly.GetId()
-                    )
-                )
-                return poly_data
-
-            for pt in pts:
-                pts_list.append(pt)
-            nb_ini_pts = len(pts_list)
-            minimum_distance = defeaturing_step  # 1e-6
-            init_surf = poly_data.Area()
-            nb_pts_removed = 0
-            surf_dev = 0
-            new_poly = None
-            while (surf_dev < max_surface_deviation and pts_list.Count > 16 and minimum_distance < 1000e-6) and float(
-                nb_pts_removed
-            ) / float(nb_ini_pts) < 0.4:
-                pts_list, nb_pts_removed = self._trim_polygon_points(pts, minimum_distance)
-                new_poly = self._edb.Geometry.PolygonData(pts_list, True)
-                current_surf = new_poly.Area()
-                if current_surf == 0:
-                    surf_dev = 1
-                else:
-                    surf_dev = abs(init_surf - current_surf) / init_surf
-                    minimum_distance = minimum_distance + defeaturing_step
-            self._logger.info(
-                "Defeaturing polygon {0}: Final surface deviation = {1} , Maximum distance(um) = {2}, "
-                "Number of points removed = {3}/{4}".format(
-                    str(poly.GetId()),
-                    str(surf_dev),
-                    str(minimum_distance * 1e6),
-                    str(nb_pts_removed),
-                    str(nb_ini_pts),
-                )
-            )
-            return new_poly
-        except:
-            return False
-
-    @pyaedt_function_handler()
-    def _trim_polygon_points(self, points, minimum_distance):
-        pts_list = []
-        ind = 0
-
-        nb_pts_removed = 0
-        for pt in points:
-            pts_list.append(pt)
-        # NbIniPts = pts_list.Count
-
-        while ind < pts_list.Count - 2:
-            pts_list, nb_pts_removed = self._get_point_list_with_minimum_distance(
-                pts_list, minimum_distance, ind, nb_pts_removed
-            )
-            ind = ind + 1
-
-        return pts_list, nb_pts_removed
-
-    @pyaedt_function_handler()
-    def _get_point_list_with_minimum_distance(self, pts_list, minimum_distance, ind, nb_pts_removed):
-        pt_ind = ind + 1
-        while pts_list[ind].Distance(pts_list[pt_ind]) < minimum_distance and pt_ind < pts_list.Count - 2:
-            pts_list.RemoveAt(pt_ind)
-            nb_pts_removed += 1
-            pt_ind += 1
-
-        return pts_list, nb_pts_removed
+        poly_data = poly.polygon_data
+        new_poly = poly_data.Defeature(tolerance)
+        poly.polygon_data = new_poly
+        return True
 
     @pyaedt_function_handler()
     def get_layout_statistics(self, evaluate_area=False, net_list=None):
         """Return EDBStatistics object from a layout.
 
         Parameters
         ----------
@@ -1267,15 +1207,16 @@
 
         """
         stat_model = EDBStatistics()
         stat_model.num_layers = len(list(self._pedb.stackup.stackup_layers.values()))
         stat_model.num_capacitors = len(self._pedb.components.capacitors)
         stat_model.num_resistors = len(self._pedb.components.resistors)
         stat_model.num_inductors = len(self._pedb.components.inductors)
-        stat_model.layout_size = self._pedb._hfss.get_layout_bounding_box(self._active_layout)
+        bbox = self._pedb._hfss.get_layout_bounding_box(self._active_layout)
+        stat_model._layout_size = bbox[2] - bbox[0], bbox[3] - bbox[1]
         stat_model.num_discrete_components = (
             len(self._pedb.components.Others) + len(self._pedb.components.ICs) + len(self._pedb.components.IOs)
         )
         stat_model.num_inductors = len(self._pedb.components.inductors)
         stat_model.num_resistors = len(self._pedb.components.resistors)
         stat_model.num_capacitors = len(self._pedb.components.capacitors)
         stat_model.num_nets = len(self._pedb.nets.nets)
@@ -1286,12 +1227,10 @@
         if evaluate_area:
             if net_list:
                 netlist = list(self._pedb.nets.nets.keys())
                 _poly = self._pedb.get_conformal_polygon_from_netlist(netlist)
             else:
                 _poly = self._pedb.get_conformal_polygon_from_netlist()
             stat_model.occupying_surface = _poly.Area()
-            outline_surface = (stat_model.layout_size[2] - stat_model.layout_size[0]) * (
-                stat_model.layout_size[3] - stat_model.layout_size[1]
-            )
+            outline_surface = stat_model.layout_size[0] * stat_model.layout_size[1]
             stat_model.occupying_ratio = stat_model.occupying_surface / outline_surface
         return stat_model
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/materials.py` & `pyaedt-0.6.79/pyaedt/edb_core/materials.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,61 +65,61 @@
             if isinstance(property_box, float):
                 return property_box
             else:
                 return property_box.ToDouble()
 
     @property
     def conductivity(self):
-        material_id = self._edb.Definition.MaterialPropertyId.Conductivity
+        material_id = self._edb.definition.MaterialPropertyId.Conductivity
         self._conductivity = self._get_property(material_id)
         return self._conductivity
 
     @conductivity.setter
     def conductivity(self, value):
         """Retrieve material conductivity."""
-        material_id = self._edb.Definition.MaterialPropertyId.Conductivity
+        material_id = self._edb.definition.MaterialPropertyId.Conductivity
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._conductivity = value
 
     @property
     def permittivity(self):
         """Retrieve material permittivity."""
-        material_id = self._edb.Definition.MaterialPropertyId.Permittivity
+        material_id = self._edb.definition.MaterialPropertyId.Permittivity
         self._permittivity = self._get_property(material_id)
         return self._permittivity
 
     @permittivity.setter
     def permittivity(self, value):
-        material_id = self._edb.Definition.MaterialPropertyId.Permittivity
+        material_id = self._edb.definition.MaterialPropertyId.Permittivity
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._permittivity = value
 
     @property
     def permeability(self):
         """Retrieve material permeability."""
-        material_id = self._edb.Definition.MaterialPropertyId.Permeability
+        material_id = self._edb.definition.MaterialPropertyId.Permeability
         self._permeability = self._get_property(material_id)
         return self._permeability
 
     @permeability.setter
     def permeability(self, value):
-        material_id = self._edb.Definition.MaterialPropertyId.Permeability
+        material_id = self._edb.definition.MaterialPropertyId.Permeability
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._permeability = value
 
     @property
     def loss_tangent(self):
         """Retrieve material loss tangent."""
-        material_id = self._edb.Definition.MaterialPropertyId.DielectricLossTangent
+        material_id = self._edb.definition.MaterialPropertyId.DielectricLossTangent
         self._loss_tangent = self._get_property(material_id)
         return self._loss_tangent
 
     @loss_tangent.setter
     def loss_tangent(self, value):
-        material_id = self._edb.Definition.MaterialPropertyId.DielectricLossTangent
+        material_id = self._edb.definition.MaterialPropertyId.DielectricLossTangent
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._loss_tangent = value
 
     @property
     def dc_conductivity(self):
         """"""
         if self._edb_material_def.GetDielectricMaterialModel():
@@ -176,99 +176,99 @@
     def permittivity_at_frequency(self, value):
         if self._edb_material_def.GetDielectricMaterialModel():
             self._edb_material_def.GetDielectricMaterialModel().SetRelativePermitivityAtFrequency(value)
 
     @property
     def magnetic_loss_tangent(self):
         """Retrieve material magnetic loss tangent."""
-        material_id = self._edb.Definition.MaterialPropertyId.MagneticLossTangent
+        material_id = self._edb.definition.MaterialPropertyId.MagneticLossTangent
         self._magnetic_loss_tangent = self._get_property(material_id)
         return self._magnetic_loss_tangent
 
     @magnetic_loss_tangent.setter
     def magnetic_loss_tangent(self, value):
-        material_id = self._edb.Definition.MaterialPropertyId.MagneticLossTangent
+        material_id = self._edb.definition.MaterialPropertyId.MagneticLossTangent
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._magnetic_loss_tangent = value
 
     @property
     def thermal_conductivity(self):
         """Retrieve material thermal conductivity."""
-        material_id = self._edb.Definition.MaterialPropertyId.ThermalConductivity
+        material_id = self._edb.definition.MaterialPropertyId.ThermalConductivity
         self._thermal_conductivity = self._get_property(material_id)
         return self._thermal_conductivity
 
     @thermal_conductivity.setter
     def thermal_conductivity(self, value):
-        material_id = self._edb.Definition.MaterialPropertyId.ThermalConductivity
+        material_id = self._edb.definition.MaterialPropertyId.ThermalConductivity
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._thermal_conductivity = value
 
     @property
     def mass_density(self):
         """Retrieve material mass density."""
-        material_id = self._edb.Definition.MaterialPropertyId.MassDensity
+        material_id = self._edb.definition.MaterialPropertyId.MassDensity
         self._mass_density = self._get_property(material_id)
         return self._mass_density
 
     @mass_density.setter
     def mass_density(self, value):
-        material_id = self._edb.Definition.MaterialPropertyId.MassDensity
+        material_id = self._edb.definition.MaterialPropertyId.MassDensity
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._mass_density = value
 
     @property
     def youngs_modulus(self):
         """Retrieve material Young's Modulus."""
-        material_id = self._edb.Definition.MaterialPropertyId.YoungsModulus
+        material_id = self._edb.definition.MaterialPropertyId.YoungsModulus
         self._youngs_modulus = self._get_property(material_id)
         return self._youngs_modulus
 
     @youngs_modulus.setter
     def youngs_modulus(self, value):
-        material_id = self._edb.Definition.MaterialPropertyId.YoungsModulus
+        material_id = self._edb.definition.MaterialPropertyId.YoungsModulus
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._youngs_modulus = value
 
     @property
     def specific_heat(self):
         """Retrieve material Specific Heat."""
-        material_id = self._edb.Definition.MaterialPropertyId.SpecificHeat
+        material_id = self._edb.definition.MaterialPropertyId.SpecificHeat
         self._specific_heat = self._get_property(material_id)
         return self._specific_heat
 
     @specific_heat.setter
     def specific_heat(self, value):
-        material_id = self._edb.Definition.MaterialPropertyId.SpecificHeat
+        material_id = self._edb.definition.MaterialPropertyId.SpecificHeat
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._specific_heat = value
 
     @property
     def poisson_ratio(self):
         """Retrieve material Poisson Ratio."""
-        material_id = self._edb.Definition.MaterialPropertyId.PoissonsRatio
+        material_id = self._edb.definition.MaterialPropertyId.PoissonsRatio
         self._poisson_ratio = self._get_property(material_id)
         return self._poisson_ratio
 
     @poisson_ratio.setter
     def poisson_ratio(self, value):
-        material_id = self._edb.Definition.MaterialPropertyId.PoissonsRatio
+        material_id = self._edb.definition.MaterialPropertyId.PoissonsRatio
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._poisson_ratio = value
 
     @property
     def thermal_expansion_coefficient(self):
         """Retrieve material Thermal Coefficient.."""
-        material_id = self._edb.Definition.MaterialPropertyId.ThermalExpansionCoefficient
+        material_id = self._edb.definition.MaterialPropertyId.ThermalExpansionCoefficient
         self._thermal_expansion_coefficient = self._get_property(material_id)
         return self._thermal_expansion_coefficient
 
     @thermal_expansion_coefficient.setter
     def thermal_expansion_coefficient(self, value):
-        material_id = self._edb.Definition.MaterialPropertyId.ThermalExpansionCoefficient
+        material_id = self._edb.definition.MaterialPropertyId.ThermalExpansionCoefficient
         self._edb_material_def.SetProperty(material_id, self._edb_value(value))
         self._thermal_expansion_coefficient = value
 
     @pyaedt_function_handler()
     def _json_format(self):
         out_dict = {}
         if self.permittivity == 0:  # pragma no cover
@@ -356,19 +356,19 @@
 
     @pyaedt_function_handler()
     def _edb_value(self, value):
         return self._pedb.edb_value(value)
 
     @property
     def _edb(self):
-        return self._pedb.edb
+        return self._pedb.edb_api
 
     @property
     def _db(self):
-        return self._pedb.db
+        return self._pedb.active_db
 
     @property
     def materials(self):
         """Retrieve dictionary of material from material library."""
         return {obj.GetName(): Material(self, obj) for obj in list(self._db.MaterialDefs)}
 
     @pyaedt_function_handler
@@ -399,15 +399,15 @@
             Material magnetic loss tangent. The default is ``0``.
 
         Returns
         -------
         :class:`pyaedt.edb_core.materials.Material`
         """
         if not name in self.materials:
-            self._edb.Definition.MaterialDef.Create(self._db, name)
+            self._edb.definition.MaterialDef.Create(self._db, name)
             new_material = self.materials[name]
             new_material.permittivity = permittivity
             new_material.permeability = permeability
             new_material.conductivity = conductivity
             new_material.loss_tangent = dielectric_loss_tangent
             new_material.magnetic_loss_tangent = magnetic_loss_tangent
             return new_material
@@ -428,15 +428,15 @@
 
         Returns
         -------
         :class:`pyaedt.edb_core.materials.Material`
 
         """
         if not name in self.materials:
-            self._edb.Definition.MaterialDef.Create(self._db, name)
+            self._edb.definition.MaterialDef.Create(self._db, name)
             new_material = self.materials[name]
             new_material.conductivity = conductivity
             new_material.permittivity = 1
             new_material.permeability = 1
             return new_material
         else:  # pragma: no cover
             warnings.warn("Material {} already exists in material library.".format(name))
@@ -458,15 +458,15 @@
             Permeability of the new material.
 
         Returns
         -------
         :class:`pyaedt.edb_core.materials.Material`
         """
         if not name in self.materials:
-            self._edb.Definition.MaterialDef.Create(self._db, name)
+            self._edb.definition.MaterialDef.Create(self._db, name)
             new_material = self.materials[name]
             new_material.permittivity = permittivity
             new_material.loss_tangent = loss_tangent
             new_material.permeability = permeability
             return new_material
         else:
             warnings.warn("Material {} already exists in material library.".format(name))
@@ -510,15 +510,15 @@
             DC Conductivity of the dielectric.
 
         Returns
         -------
         :class:`pyaedt.edb_core.materials.Material`
             Material definition.
         """
-        material_def = self._edb.Definition.DjordjecvicSarkarModel()
+        material_def = self._edb.definition.DjordjecvicSarkarModel()
         material_def.SetFrequency(test_frequency)
         material_def.SetLossTangentAtFrequency(self._edb_value(loss_tangent))
         material_def.SetRelativePermitivityAtFrequency(permittivity)
         if dc_conductivity is not None:
             material_def.SetDCConductivity(dc_conductivity)
         if dc_permittivity is not None:
             material_def.SetUseDCRelativePermitivity(True)
@@ -560,15 +560,15 @@
             Value for the higher frequency.
 
         Returns
         -------
         :class:`pyaedt.edb_core.materials.Material`
             Material definition.
         """
-        material_def = self._edb.Definition.DebyeModel()
+        material_def = self._edb.definition.DebyeModel()
         material_def.SetFrequencyRange(lower_freqency, higher_frequency)
         material_def.SetLossTangentAtHighLowFrequency(loss_tangent_low, loss_tangent_high)
         material_def.SetRelativePermitivityAtHighLowFrequency(
             self._edb_value(permittivity_low), self._edb_value(permittivity_high)
         )
         return self._add_dielectric_material_model(name, material_def)
 
@@ -606,27 +606,27 @@
         >>> rel_perm = [1e9, 1.1e9, 1.2e9, 1.3e9, 1.5e9, 1.6e9]
         >>> loss_tan = [0.025, 0.026, 0.027, 0.028, 0.029, 0.030]
         >>> diel = edb.materials.add_multipole_debye_material("My_MP_Debye", freq, rel_perm, loss_tan)
         """
         frequencies = [float(i) for i in frequencies]
         permittivities = [float(i) for i in permittivities]
         loss_tangents = [float(i) for i in loss_tangents]
-        material_def = self._edb.Definition.MultipoleDebyeModel()
+        material_def = self._edb.definition.MultipoleDebyeModel()
         material_def.SetParameters(
             convert_py_list_to_net_list(frequencies),
             convert_py_list_to_net_list(permittivities),
             convert_py_list_to_net_list(loss_tangents),
         )
         return self._add_dielectric_material_model(name, material_def)
 
     @pyaedt_function_handler()
     def _add_dielectric_material_model(self, name, material_model):
-        if self._edb.Definition.MaterialDef.FindByName(self._db, name).IsNull():
-            self._edb.Definition.MaterialDef.Create(self._db, name)
-        material_def = self._edb.Definition.MaterialDef.FindByName(self._db, name)
+        if self._edb.definition.MaterialDef.FindByName(self._db, name).IsNull():
+            self._edb.definition.MaterialDef.Create(self._db, name)
+        material_def = self._edb.definition.MaterialDef.FindByName(self._db, name)
         succeeded = material_def.SetDielectricMaterialModel(material_model)
         if succeeded:
             return material_def
         return False
 
     @pyaedt_function_handler()
     def duplicate(self, material_name, new_material_name):
@@ -638,15 +638,15 @@
         material_name : str
             Name of the existing material.
         new_material_name : str
             Name of the new duplicated material.
 
         Returns
         -------
-        EDB material : class: 'Ansys.Ansoft.Edb.Definition.MaterialDef'
+        EDB material : class: 'Ansys.Ansoft.Edb.definition.MaterialDef'
 
 
         Examples
         --------
 
         >>> from pyaedt import Edb
         >>> edb_app = Edb()
@@ -663,30 +663,30 @@
             magnetic_loss_tangent = self._edb_value(self.materials[material_name].magnetic_loss_tangent)
             thermal_conductivity = self._edb_value(self.materials[material_name].thermal_conductivity)
             thermal_expansion_coefficient = self._edb_value(self.materials[material_name].thermal_expansion_coefficient)
             youngs_modulus = self._edb_value(self.materials[material_name].youngs_modulus)
             poisson_ratio = self._edb_value(self.materials[material_name].poisson_ratio)
             mass_density = self._edb_value(self.materials[material_name].mass_density)
             material_model = self.materials[material_name]._edb_material_def.GetDielectricMaterialModel()
-            edb_material = self._edb.Definition.MaterialDef.Create(self._db, new_material_name)
-            edb_material.SetProperty(self._edb.Definition.MaterialPropertyId.Permittivity, permittivity)
-            edb_material.SetProperty(self._edb.Definition.MaterialPropertyId.Permeability, permeability)
-            edb_material.SetProperty(self._edb.Definition.MaterialPropertyId.Conductivity, conductivity)
+            edb_material = self._edb.definition.MaterialDef.Create(self._db, new_material_name)
+            edb_material.SetProperty(self._edb.definition.MaterialPropertyId.Permittivity, permittivity)
+            edb_material.SetProperty(self._edb.definition.MaterialPropertyId.Permeability, permeability)
+            edb_material.SetProperty(self._edb.definition.MaterialPropertyId.Conductivity, conductivity)
             edb_material.SetProperty(
-                self._edb.Definition.MaterialPropertyId.DielectricLossTangent, dielectric_loss_tangent
+                self._edb.definition.MaterialPropertyId.DielectricLossTangent, dielectric_loss_tangent
             )
-            edb_material.SetProperty(self._edb.Definition.MaterialPropertyId.ThermalConductivity, thermal_conductivity)
+            edb_material.SetProperty(self._edb.definition.MaterialPropertyId.ThermalConductivity, thermal_conductivity)
             edb_material.SetProperty(
-                self._edb.Definition.MaterialPropertyId.ThermalExpansionCoefficient, thermal_expansion_coefficient
+                self._edb.definition.MaterialPropertyId.ThermalExpansionCoefficient, thermal_expansion_coefficient
             )
-            edb_material.SetProperty(self._edb.Definition.MaterialPropertyId.MassDensity, mass_density)
-            edb_material.SetProperty(self._edb.Definition.MaterialPropertyId.YoungsModulus, youngs_modulus)
-            edb_material.SetProperty(self._edb.Definition.MaterialPropertyId.PoissonsRatio, poisson_ratio)
-            edb_material.SetProperty(self._edb.Definition.MaterialPropertyId.MagneticLossTangent, magnetic_loss_tangent)
-            edb_material.SetProperty(self._edb.Definition.MaterialPropertyId.MagneticLossTangent, magnetic_loss_tangent)
+            edb_material.SetProperty(self._edb.definition.MaterialPropertyId.MassDensity, mass_density)
+            edb_material.SetProperty(self._edb.definition.MaterialPropertyId.YoungsModulus, youngs_modulus)
+            edb_material.SetProperty(self._edb.definition.MaterialPropertyId.PoissonsRatio, poisson_ratio)
+            edb_material.SetProperty(self._edb.definition.MaterialPropertyId.MagneticLossTangent, magnetic_loss_tangent)
+            edb_material.SetProperty(self._edb.definition.MaterialPropertyId.MagneticLossTangent, magnetic_loss_tangent)
             edb_material.SetDielectricMaterialModel(material_model)
 
             return edb_material
 
     @pyaedt_function_handler()
     def _load_materials(self, material=None):
         if self.materials:
@@ -717,33 +717,33 @@
             Name of the material property.
 
         Returns
         -------
         ID of the material property.
         """
         props = {
-            "Permittivity": self._edb.Definition.MaterialPropertyId.Permittivity,
-            "Permeability": self._edb.Definition.MaterialPropertyId.Permeability,
-            "Conductivity": self._edb.Definition.MaterialPropertyId.Conductivity,
-            "DielectricLossTangent": self._edb.Definition.MaterialPropertyId.DielectricLossTangent,
-            "MagneticLossTangent": self._edb.Definition.MaterialPropertyId.MagneticLossTangent,
-            "ThermalConductivity": self._edb.Definition.MaterialPropertyId.ThermalConductivity,
-            "MassDensity": self._edb.Definition.MaterialPropertyId.MassDensity,
-            "SpecificHeat": self._edb.Definition.MaterialPropertyId.SpecificHeat,
-            "YoungsModulus": self._edb.Definition.MaterialPropertyId.YoungsModulus,
-            "PoissonsRatio": self._edb.Definition.MaterialPropertyId.PoissonsRatio,
-            "ThermalExpansionCoefficient": self._edb.Definition.MaterialPropertyId.ThermalExpansionCoefficient,
-            "InvalidProperty": self._edb.Definition.MaterialPropertyId.InvalidProperty,
+            "Permittivity": self._edb.definition.MaterialPropertyId.Permittivity,
+            "Permeability": self._edb.definition.MaterialPropertyId.Permeability,
+            "Conductivity": self._edb.definition.MaterialPropertyId.Conductivity,
+            "DielectricLossTangent": self._edb.definition.MaterialPropertyId.DielectricLossTangent,
+            "MagneticLossTangent": self._edb.definition.MaterialPropertyId.MagneticLossTangent,
+            "ThermalConductivity": self._edb.definition.MaterialPropertyId.ThermalConductivity,
+            "MassDensity": self._edb.definition.MaterialPropertyId.MassDensity,
+            "SpecificHeat": self._edb.definition.MaterialPropertyId.SpecificHeat,
+            "YoungsModulus": self._edb.definition.MaterialPropertyId.YoungsModulus,
+            "PoissonsRatio": self._edb.definition.MaterialPropertyId.PoissonsRatio,
+            "ThermalExpansionCoefficient": self._edb.definition.MaterialPropertyId.ThermalExpansionCoefficient,
+            "InvalidProperty": self._edb.definition.MaterialPropertyId.InvalidProperty,
         }
 
         found_el = difflib.get_close_matches(property_name, list(props.keys()), 1, 0.7)
         if found_el:
             return props[found_el[0]]
         else:
-            return self._edb.Definition.MaterialPropertyId.InvalidProperty
+            return self._edb.definition.MaterialPropertyId.InvalidProperty
 
     @pyaedt_function_handler()
     def get_property_by_material_name(self, property_name, material_name):
         """Get the property of a material. If it is executed in IronPython,
          you must only use the first element of the returned tuple, which is a float.
 
         Parameters
@@ -769,18 +769,18 @@
         >>> from pyaedt import Edb
         >>> edb_app = Edb()
         >>> returned_tuple = edb_app.materials.get_property_by_material_name("conductivity", "copper")
         >>> edb_value = returned_tuple[0]
         >>> float_value = returned_tuple[1]
 
         """
-        if self._edb.Definition.MaterialDef.FindByName(self._pedb._db, material_name).IsNull():
+        if self._edb.definition.MaterialDef.FindByName(self._pedb._db, material_name).IsNull():
             self._pedb.logger.error("This material doesn't exists.")
         else:
-            original_material = self._edb.Definition.MaterialDef.FindByName(self._pedb._db, material_name)
+            original_material = self._edb.definition.MaterialDef.FindByName(self._pedb._db, material_name)
             if is_ironpython:  # pragma: no cover
                 property_box = _clr.StrongBox[float]()
                 original_material.GetProperty(self.material_name_to_id(property_name), property_box)
                 return float(property_box)
             else:
                 _, property_box = original_material.GetProperty(
                     self.material_name_to_id(property_name), self._edb_value(0.0)
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/nets.py` & `pyaedt-0.6.79/pyaedt/edb_core/nets.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,37 +46,37 @@
         self._pedb.logger.error("Component or definition not found.")
         return
 
     def __init__(self, p_edb):
         self._pedb = p_edb
 
     @property
-    def _builder(self):
-        """ """
-        return self._pedb.builder
-
-    @property
     def _edb(self):
         """ """
-        return self._pedb.edb
+        return self._pedb.edb_api
 
     @property
     def _active_layout(self):
         """ """
         return self._pedb.active_layout
 
     @property
+    def _layout(self):
+        """ """
+        return self._pedb.layout
+
+    @property
     def _cell(self):
         """ """
         return self._pedb.cell
 
     @property
     def db(self):
         """Db object."""
-        return self._pedb.db
+        return self._pedb.active_db
 
     @property
     def _logger(self):
         """Edb logger."""
         return self._pedb.logger
 
     @property
@@ -85,16 +85,16 @@
 
         Returns
         -------
         dict[str, :class:`pyaedt.edb_core.edb_data.nets_data.EDBNetsData`]
             Dictionary of nets.
         """
         nets = {}
-        for net in self._active_layout.Nets:
-            nets[net.GetName()] = EDBNetsData(net, self._pedb)
+        for net in self._layout.nets:
+            nets[net.name] = EDBNetsData(net.api_object, self._pedb)
         return nets
 
     @property
     def netlist(self):
         """Return the cell netlist.
 
         Returns
@@ -175,33 +175,32 @@
            Area ratio used by the ``get_power_ground_nets`` method.
 
         Returns
         -------
         list of  :class:`pyaedt.edb_core.edb_data.EDBNetsData`
         """
         pwr_gnd_nets = []
-        nets = list(self._active_layout.Nets)
-        for net in nets:
+        for net in self._layout.nets[:]:
             total_plane_area = 0.0
             total_trace_area = 0.0
             for primitive in net.Primitives:
-                if primitive.GetPrimitiveType() == self._edb.Cell.Primitive.PrimitiveType.Bondwire:
+                if primitive.GetPrimitiveType() == self._edb.cell.primitive.PrimitiveType.Bondwire:
                     continue
-                if primitive.GetPrimitiveType() != self._edb.Cell.Primitive.PrimitiveType.Path:
+                if primitive.GetPrimitiveType() != self._edb.cell.primitive.PrimitiveType.Path:
                     total_plane_area += float(primitive.GetPolygonData().Area())
                 else:
                     total_trace_area += float(primitive.GetPolygonData().Area())
             if total_plane_area == 0.0:
                 continue
             if total_trace_area == 0.0:
-                pwr_gnd_nets.append(EDBNetsData(net, self._pedb))
+                pwr_gnd_nets.append(EDBNetsData(net.api_object, self._pedb))
                 continue
             if total_plane_area > 0.0 and total_trace_area > 0.0:
                 if total_plane_area / (total_plane_area + total_trace_area) > threshold:
-                    pwr_gnd_nets.append(EDBNetsData(net, self._pedb))
+                    pwr_gnd_nets.append(EDBNetsData(net.api_object, self._pedb))
         return pwr_gnd_nets
 
     @staticmethod
     def _eval_arc_points(p1, p2, h, n=6, tol=1e-12):
         """Get the points of the arc.
 
         Parameters
@@ -670,15 +669,15 @@
             If ``True`` the legend is shown in the plot. (default)
             If ``False`` the legend is not shown.
         save_plot : str, optional
             If ``None`` the plot will be shown.
             If a file path is specified the plot will be saved to such file.
         outline : list, optional
             List of points of the outline to plot.
-        size : tuple, optional
+        size : tuple, int, optional
             Image size in pixel (width, height). Default value is ``(2000, 1000)``
         plot_components_on_top : bool, optional
             If ``True``  the components placed on top layer are plotted.
             If ``False`` the components are not plotted. (default)
             If nets and/or layers is specified, only the components belonging to the specified nets/layers are plotted.
         plot_components_on_bottom : bool, optional
             If ``True``  the components placed on bottom layer are plotted.
@@ -694,14 +693,21 @@
             nets,
             layers,
             color_by_net,
             outline,
             plot_components_on_top,
             plot_components_on_bottom,
         )
+
+        if isinstance(size, int):  # pragma: no cover
+            board_size_x, board_size_y = self._pedb.get_statistics().layout_size
+            fig_size_x = size
+            fig_size_y = board_size_y * fig_size_x / board_size_x
+            size = (fig_size_x, fig_size_y)
+
         plot_matplotlib(
             object_lists,
             size,
             show_legend,
             "X (m)",
             "Y (m)",
             self._pedb.active_cell.GetName(),
@@ -840,15 +846,15 @@
             "pin_list",
         ]
         return component_list, component_list_columns, net_group
 
     @pyaedt_function_handler()
     def get_net_by_name(self, net_name):
         """Find a net by name."""
-        edb_net = self._edb.Cell.Net.FindByName(self._active_layout, net_name)
+        edb_net = self._edb.cell.net.find_by_name(self._active_layout, net_name)
         if edb_net is not None:
             return edb_net
 
     @pyaedt_function_handler()
     def delete_nets(self, netlist):
         """Delete one or more nets from EDB.
 
@@ -927,21 +933,21 @@
         Returns
         -------
         object
             Net Object.
         """
         if not net_name and not start_with and not contain and not end_with:
             net_name = generate_unique_name("NET_")
-            net = self._edb.Cell.Net.Create(self._active_layout, net_name)
+            net = self._edb.cell.net.create(self._active_layout, net_name)
             return net
         else:
             if not start_with and not contain and not end_with:
-                net = self._edb.Cell.Net.FindByName(self._active_layout, net_name)
+                net = self._edb.cell.net.find_by_name(self._active_layout, net_name)
                 if net.IsNull():
-                    net = self._edb.Cell.Net.Create(self._active_layout, net_name)
+                    net = self._edb.cell.net.create(self._active_layout, net_name)
                 return net
             elif start_with:
                 nets_found = [
                     self.nets[net].net_object for net in list(self.nets.keys()) if net.lower().startswith(start_with)
                 ]
                 return nets_found
             elif start_with and end_with:
@@ -1161,17 +1167,17 @@
                     for _pp in list(pp):
                         _voids = list(_pp.Obj.Voids)
                         void_list.extend(_pp.Obj.Voids)
                 for poly_list in list(connected_polygons):
                     layer = list(poly_list)[0].Obj.GetLayer().GetName()
                     net = list(poly_list)[0].Obj.GetNet()
                     _poly_list = convert_py_list_to_net_list([obj.Poly for obj in list(poly_list)])
-                    merged_polygon = list(self._edb.Geometry.PolygonData.Unite(_poly_list))
+                    merged_polygon = list(self._edb.geometry.polygon_data.unite(_poly_list))
                     for poly in merged_polygon:
                         for void in void_list:
                             poly.AddHole(void.GetPolygonData())
-                        _new_poly = self._edb.Cell.Primitive.Polygon.Create(self._active_layout, layer, net, poly)
+                        _new_poly = self._edb.cell.primitive.polygon.create(self._active_layout, layer, net, poly)
                         returned_poly.append(_new_poly)
                 for init_poly in list(list(connected_polygons)):
                     for _pp in list(init_poly):
                         _pp.Obj.Delete()
         return returned_poly
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.79/pyaedt/edb_core/padstack.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,35 +48,35 @@
         self._pedb.logger.error("Component or definition not found.")
         return
 
     def __init__(self, p_edb):
         self._pedb = p_edb
 
     @property
-    def _builder(self):
-        """ """
-        return self._pedb.builder
-
-    @property
     def _edb(self):
         """ """
-        return self._pedb.edb
+        return self._pedb.edb_api
 
     def _get_edb_value(self, value):
         return self._pedb.edb_value(value)
 
     @property
     def _active_layout(self):
         """ """
         return self._pedb.active_layout
 
     @property
+    def _layout(self):
+        """ """
+        return self._pedb.layout
+
+    @property
     def db(self):
         """Db object."""
-        return self._pedb.db
+        return self._pedb.active_db
 
     @property
     def _logger(self):
         """ """
         return self._pedb.logger
 
     @property
@@ -95,23 +95,23 @@
         Returns
         -------
         object
             EDB.PadType enumerator value.
         """
 
         if val == 0:
-            return self._edb.Definition.PadType.RegularPad
+            return self._edb.definition.PadType.RegularPad
         elif val == 1:
-            return self._edb.Definition.PadType.AntiPad
+            return self._edb.definition.PadType.AntiPad
         elif val == 2:
-            return self._edb.Definition.PadType.ThermalPad
+            return self._edb.definition.PadType.ThermalPad
         elif val == 3:
-            return self._edb.Definition.PadType.Hole
+            return self._edb.definition.PadType.Hole
         elif val == 4:
-            return self._edb.Definition.PadType.UnknownGeomType
+            return self._edb.definition.PadType.UnknownGeomType
         else:
             return val
 
     @pyaedt_function_handler()
     def int_to_geometry_type(self, val=0):
         """Convert an integer to an EDB.PadGeometryType.
 
@@ -121,54 +121,54 @@
 
         Returns
         -------
         object
             EDB.PadGeometryType enumerator value.
         """
         if val == 0:
-            return self._edb.Definition.PadGeometryType.NoGeometry
+            return self._edb.definition.PadGeometryType.NoGeometry
         elif val == 1:
-            return self._edb.Definition.PadGeometryType.Circle
+            return self._edb.definition.PadGeometryType.Circle
         elif val == 2:
-            return self._edb.Definition.PadGeometryType.Square
+            return self._edb.definition.PadGeometryType.Square
         elif val == 3:
-            return self._edb.Definition.PadGeometryType.Rectangle
+            return self._edb.definition.PadGeometryType.Rectangle
         elif val == 4:
-            return self._edb.Definition.PadGeometryType.Oval
+            return self._edb.definition.PadGeometryType.Oval
         elif val == 5:
-            return self._edb.Definition.PadGeometryType.Bullet
+            return self._edb.definition.PadGeometryType.Bullet
         elif val == 6:
-            return self._edb.Definition.PadGeometryType.NSidedPolygon
+            return self._edb.definition.PadGeometryType.NSidedPolygon
         elif val == 7:
-            return self._edb.Definition.PadGeometryType.Polygon
+            return self._edb.definition.PadGeometryType.Polygon
         elif val == 8:
-            return self._edb.Definition.PadGeometryType.Round45
+            return self._edb.definition.PadGeometryType.Round45
         elif val == 9:
-            return self._edb.Definition.PadGeometryType.Round90
+            return self._edb.definition.PadGeometryType.Round90
         elif val == 10:
-            return self._edb.Definition.PadGeometryType.Square45
+            return self._edb.definition.PadGeometryType.Square45
         elif val == 11:
-            return self._edb.Definition.PadGeometryType.Square90
+            return self._edb.definition.PadGeometryType.Square90
         elif val == 12:
-            return self._edb.Definition.PadGeometryType.InvalidGeometry
+            return self._edb.definition.PadGeometryType.InvalidGeometry
         else:
             return val
 
     @property
     def definitions(self):
         """Padstack definitions.
 
         Returns
         -------
         dict[str, :class:`pyaedt.edb_core.edb_data.padstacks_data.EdbPadstack`]
             List of definitions via padstack definitions.
 
         """
         _padstacks = {}
-        for padstackdef in self.db.PadstackDefs:
+        for padstackdef in self._pedb.padstack_defs:
             PadStackData = padstackdef.GetData()
             if len(PadStackData.GetLayerNames()) >= 1:
                 _padstacks[padstackdef.GetName()] = EDBPadstack(padstackdef, self)
         return _padstacks
 
     @property
     def padstacks(self):
@@ -194,15 +194,15 @@
         -------
         dict[str, :class:`pyaedt.edb_core.edb_data.padstacks_data.EDBPadstackInstance`]
             List of padstack instances.
 
         """
 
         padstack_instances = {}
-        edb_padstack_inst_list = list(self._active_layout.PadstackInstances)
+        edb_padstack_inst_list = self._pedb.layout.padstack_instances
         for edb_padstack_instance in edb_padstack_inst_list:
             padstack_instances[edb_padstack_instance.GetId()] = EDBPadstackInstance(edb_padstack_instance, self._pedb)
         return padstack_instances
 
     @property
     def pins(self):
         """Dictionary  of all pins instances (belonging to component).
@@ -265,29 +265,29 @@
 
         Returns
         -------
         list
             List of all layout pin groups.
         """
         pingroups = []
-        for el in self._active_layout.PinGroups:
+        for el in self._layout.pin_groups:
             pingroups.append(el)
         return pingroups
 
     @property
     def pad_type(self):
         """Return a PadType Enumerator."""
 
         class PadType:
             (RegularPad, AntiPad, ThermalPad, Hole, UnknownGeomType) = (
-                self._edb.Definition.PadType.RegularPad,
-                self._edb.Definition.PadType.AntiPad,
-                self._edb.Definition.PadType.ThermalPad,
-                self._edb.Definition.PadType.Hole,
-                self._edb.Definition.PadType.UnknownGeomType,
+                self._edb.definition.PadType.RegularPad,
+                self._edb.definition.PadType.AntiPad,
+                self._edb.definition.PadType.ThermalPad,
+                self._edb.definition.PadType.Hole,
+                self._edb.definition.PadType.UnknownGeomType,
             )
 
         return PadType
 
     @pyaedt_function_handler()
     def create_circular_padstack(
         self,
@@ -319,73 +319,73 @@
 
         Returns
         -------
         str
             Name of the padstack if the operation is successful.
         """
 
-        PadStack = self._edb.Definition.PadstackDef.Create(self._active_layout.GetCell().GetDatabase(), padstackname)
-        new_PadStackData = self._edb.Definition.PadstackDefData.Create()
+        PadStack = self._edb.definition.PadstackDef.Create(self._layout.cell.GetDatabase(), padstackname)
+        new_PadStackData = self._edb.definition.PadstackDefData.Create()
         list_values = convert_py_list_to_net_list(
             [self._get_edb_value(holediam), self._get_edb_value(paddiam), self._get_edb_value(antipaddiam)]
         )
         value0 = self._get_edb_value(0.0)
         new_PadStackData.SetHoleParameters(
-            self._edb.Definition.PadGeometryType.Circle,
+            self._edb.definition.PadGeometryType.Circle,
             list_values,
             value0,
             value0,
             value0,
         )
-        new_PadStackData.SetHoleRange(self._edb.Definition.PadstackHoleRange.UpperPadToLowerPad)
+        new_PadStackData.SetHoleRange(self._edb.definition.PadstackHoleRange.UpperPadToLowerPad)
         layers = list(self._pedb.stackup.signal_layers.keys())
         if not startlayer:
             startlayer = layers[0]
         if not endlayer:
             endlayer = layers[len(layers) - 1]
 
-        antipad_shape = self._edb.Definition.PadGeometryType.Circle
+        antipad_shape = self._edb.definition.PadGeometryType.Circle
         started = False
         new_PadStackData.SetPadParameters(
             "Default",
-            self._edb.Definition.PadType.RegularPad,
-            self._edb.Definition.PadGeometryType.Circle,
+            self._edb.definition.PadType.RegularPad,
+            self._edb.definition.PadGeometryType.Circle,
             convert_py_list_to_net_list([self._get_edb_value(paddiam)]),
             value0,
             value0,
             value0,
         )
 
         new_PadStackData.SetPadParameters(
             "Default",
-            self._edb.Definition.PadType.AntiPad,
+            self._edb.definition.PadType.AntiPad,
             antipad_shape,
             convert_py_list_to_net_list([self._get_edb_value(antipaddiam)]),
             value0,
             value0,
             value0,
         )
         for layer in layers:
             if layer == startlayer:
                 started = True
             if layer == endlayer:
                 started = False
             if started:
                 new_PadStackData.SetPadParameters(
                     layer,
-                    self._edb.Definition.PadType.RegularPad,
-                    self._edb.Definition.PadGeometryType.Circle,
+                    self._edb.definition.PadType.RegularPad,
+                    self._edb.definition.PadGeometryType.Circle,
                     convert_py_list_to_net_list([self._get_edb_value(paddiam)]),
                     value0,
                     value0,
                     value0,
                 )
                 new_PadStackData.SetPadParameters(
                     layer,
-                    self._edb.Definition.PadType.AntiPad,
+                    self._edb.definition.PadType.AntiPad,
                     antipad_shape,
                     convert_py_list_to_net_list([self._get_edb_value(antipaddiam)]),
                     value0,
                     value0,
                     value0,
                 )
         PadStack.SetData(new_PadStackData)
@@ -440,21 +440,21 @@
         """
         if isinstance(padstackInst, int):
             psdef = self.definitions[self.instances[padstackInst].padstack_definition].edb_padstack
             padstackInst = self.instances[padstackInst]._edb_padstackinstance
 
         else:
             psdef = padstackInst.GetPadstackDef()
-        newdefdata = self._edb.Definition.PadstackDefData(psdef.GetData())
-        newdefdata.SetSolderBallShape(self._edb.Definition.SolderballShape.Cylinder)
+        newdefdata = self._edb.definition.PadstackDefData(psdef.GetData())
+        newdefdata.SetSolderBallShape(self._edb.definition.SolderballShape.Cylinder)
         newdefdata.SetSolderBallParameter(self._get_edb_value(ballDiam), self._get_edb_value(ballDiam))
         sball_placement = (
-            self._edb.Definition.SolderballPlacement.AbovePadstack
+            self._edb.definition.SolderballPlacement.AbovePadstack
             if isTopPlaced
-            else self._edb.Definition.SolderballPlacement.BelowPadstack
+            else self._edb.definition.SolderballPlacement.BelowPadstack
         )
         newdefdata.SetSolderBallPlacement(sball_placement)
         psdef.SetData(newdefdata)
         sball_layer = [lay._edb_layer for lay in list(self._layers.values()) if lay.name == sballLayer_name][0]
         if sball_layer is not None:
             padstackInst.SetSolderBallLayer(sball_layer)
             return True
@@ -496,15 +496,15 @@
             port_name = "{0}.{1}.{2}".format(cmp_name, pin_name, net_name)
         else:
             port_name = "{0}_{1}_{2}".format(cmp_name, pin_name, net_name)
         if not padstackinstance.IsLayoutPin():
             padstackinstance.SetIsLayoutPin(True)
 
         res = padstackinstance.GetLayerRange()
-        self._edb.Cell.Terminal.PadstackInstanceTerminal.Create(
+        self._edb.cell.terminal.PadstackInstanceTerminal.Create(
             self._active_layout,
             padstackinstance.GetNet(),
             port_name,
             padstackinstance,
             res[2],
         )
         if res[0]:
@@ -550,15 +550,15 @@
 
     @pyaedt_function_handler()
     def get_pad_parameters(self, pin, layername, pad_type=0):
         """Get Padstack Parameters from Pin or Padstack Definition.
 
         Parameters
         ----------
-        pin : Edb.Definition.PadstackDef or Edb.Definition.PadstackInstance
+        pin : Edb.definition.PadstackDef or Edb.definition.PadstackInstance
             Pin or PadstackDef on which get values.
         layername : str
             Layer on which get properties.
         pad_type : int
             Pad Type.
 
         Returns
@@ -566,31 +566,31 @@
         tuple
             Tuple of (GeometryType, ParameterList, OffsetX, OffsetY, Rot).
         """
 
         if "PadstackDef" in str(type(pin)):
             padparams = pin.GetData().GetPadParametersValue(layername, self.int_to_pad_type(pad_type))
         else:
-            padparams = self._edb.Definition.PadstackDefData(pin.GetPadstackDef().GetData()).GetPadParametersValue(
+            padparams = self._edb.definition.PadstackDefData(pin.GetPadstackDef().GetData()).GetPadParametersValue(
                 layername, self.int_to_pad_type(pad_type)
             )
         if padparams[2]:
             geometry_type = int(padparams[1])
             parameters = [i.ToString() for i in padparams[2]]
             offset_x = padparams[3].ToDouble()
             offset_y = padparams[4].ToDouble()
             rotation = padparams[5].ToDouble()
             return geometry_type, parameters, offset_x, offset_y, rotation
         else:
-            if isinstance(pin, self._edb.Definition.PadstackDef):
-                padparams = self._edb.Definition.PadstackDefData(pin.GetData()).GetPolygonalPadParameters(
+            if isinstance(pin, self._edb.definition.PadstackDef):
+                padparams = self._edb.definition.PadstackDefData(pin.GetData()).GetPolygonalPadParameters(
                     layername, self.int_to_pad_type(pad_type)
                 )
             else:
-                padparams = self._edb.Definition.PadstackDefData(
+                padparams = self._edb.definition.PadstackDefData(
                     pin.GetPadstackDef().GetData()
                 ).GetPolygonalPadParameters(layername, self.int_to_pad_type(pad_type))
 
             if padparams[0]:
                 parameters = [
                     padparams[1].GetBBox().Item1.X.ToDouble(),
                     padparams[1].GetBBox().Item1.Y.ToDouble(),
@@ -616,30 +616,30 @@
         Returns
         -------
         bool
             ``True`` when successful, ``False`` if an anti-pad value fails to be assigned.
         """
         if self.definitions:
             for padstack in list(self.definitions.values()):
-                cloned_padstack_data = self._edb.Definition.PadstackDefData(padstack.edb_padstack.GetData())
+                cloned_padstack_data = self._edb.definition.PadstackDefData(padstack.edb_padstack.GetData())
                 layers_name = cloned_padstack_data.GetLayerNames()
                 all_succeed = True
                 for layer in layers_name:
                     geom_type, parameters, offset_x, offset_y, rot = self.get_pad_parameters(
                         padstack.edb_padstack, layer, 1
                     )
                     if geom_type == 1:  # pragma no cover
                         params = convert_py_list_to_net_list(
                             [self._pedb.edb_value(value)] * len(parameters)
                         )  # pragma no cover
-                        geom = self._edb.Definition.PadGeometryType.Circle
+                        geom = self._edb.definition.PadGeometryType.Circle
                         offset_x = self._pedb.edb_value(offset_x)
                         offset_y = self._pedb.edb_value(offset_y)
                         rot = self._pedb.edb_value(rot)
-                        antipad = self._edb.Definition.PadType.AntiPad
+                        antipad = self._edb.definition.PadType.AntiPad
                         if cloned_padstack_data.SetPadParameters(
                             layer, antipad, geom, params, offset_x, offset_y, rot
                         ):  # pragma no cover
                             self._logger.info(
                                 "Pad-stack definition {}, anti-pad on layer {}, has been set to {}".format(
                                     padstack.edb_padstack.GetName(), layer, str(value)
                                 )
@@ -695,15 +695,15 @@
             List of EDB vias.
         """
         if net_list == None:
             net_list = []
 
         if not isinstance(net_list, list):
             net_list = [net_list]
-        layout_lobj_collection = list(self._active_layout.PadstackInstances)
+        layout_lobj_collection = self._layout.padstack_instances
         via_list = []
         for lobj in layout_lobj_collection:
             pad_layers_name = lobj.GetPadstackDef().GetData().GetLayerNames()
             if len(pad_layers_name) > 1:
                 if not net_list:
                     via_list.append(lobj)
                 elif lobj.GetNet().GetName() in net_list:
@@ -807,14 +807,17 @@
         offset_x="0.0",
         offset_y="0.0",
         rotation="0.0",
         has_hole=True,
         pad_offset_x="0.0",
         pad_offset_y="0.0",
         pad_rotation="0.0",
+        start_layer=None,
+        stop_layer=None,
+        add_default_layer=False,
     ):
         """Create a padstack.
 
         Parameters
         ----------
         padstackname : str, optional
             Name of the padstack. The default is ``None``.
@@ -844,32 +847,38 @@
             Whether this padstack has a hole.
         pad_offset_x : str, optional
             Padstack offset in X direction.
         pad_offset_y : str, optional
             Padstack offset in Y direction.
         pad_rotation : str, optional
             Padstack rotation.
+        start_layer : str, optional
+            Start layer of the padstack definition.
+        stop_layer : str, optional
+            Stop layer of the padstack definition.
+        add_default_layer : bool, optional
+            Add ``"Default"`` to padstack definition. Default is ``False``.
 
         Returns
         -------
         str
             Name of the padstack if the operation is successful.
         """
         holediam = self._get_edb_value(holediam)
         paddiam = self._get_edb_value(paddiam)
         antipaddiam = self._get_edb_value(antipaddiam)
 
         if not padstackname:
             padstackname = generate_unique_name("VIA")
         # assert not self.isreadonly, "Write Functions are not available within AEDT"
-        padstackData = self._edb.Definition.PadstackDefData.Create()
+        padstackData = self._edb.definition.PadstackDefData.Create()
         if has_hole:
-            ptype = self._edb.Definition.PadGeometryType.Circle
+            ptype = self._edb.definition.PadGeometryType.Circle
         else:
-            ptype = self._edb.Definition.PadGeometryType.NoGeometry
+            ptype = self._edb.definition.PadGeometryType.NoGeometry
         holparam = Array[type(holediam)]([holediam])
         value0 = self._get_edb_value("0.0")
         x_size = self._get_edb_value(x_size)
         y_size = self._get_edb_value(y_size)
         corner_radius = self._get_edb_value(corner_radius)
         offset_x = self._get_edb_value(offset_x)
         offset_y = self._get_edb_value(offset_y)
@@ -878,54 +887,58 @@
         pad_offset_x = self._get_edb_value(pad_offset_x)
         pad_offset_y = self._get_edb_value(pad_offset_y)
         pad_rotation = self._get_edb_value(pad_rotation)
 
         padstackData.SetHoleParameters(ptype, holparam, value0, value0, value0)
 
         padstackData.SetHolePlatingPercentage(self._get_edb_value(20.0))
-        padstackData.SetHoleRange(self._edb.Definition.PadstackHoleRange.UpperPadToLowerPad)
+        padstackData.SetHoleRange(self._edb.definition.PadstackHoleRange.UpperPadToLowerPad)
         padstackData.SetMaterial("copper")
-        layers = list(self._pedb.stackup.signal_layers.keys())
-
+        layers = list(self._pedb.stackup.signal_layers.keys())[:]
+        if start_layer and start_layer in layers:
+            layers = layers[layers.index(start_layer) :]
+        if stop_layer and stop_layer in layers:
+            layers = layers[: layers.index(stop_layer) + 1]
+        pad_array = Array[type(paddiam)]([paddiam])
         if pad_shape == "Circle":
-            pad_array = Array[type(paddiam)]([paddiam])
-            pad_shape = self._edb.Definition.PadGeometryType.Circle
+            pad_shape = self._edb.definition.PadGeometryType.Circle
         elif pad_shape == "Rectangle":
             pad_array = Array[type(x_size)]([x_size, y_size])
-            pad_shape = self._edb.Definition.PadGeometryType.Rectangle
+            pad_shape = self._edb.definition.PadGeometryType.Rectangle
         if antipad_shape == "Bullet":
             antipad_array = Array[type(x_size)]([x_size, y_size, corner_radius])
-            antipad_shape = self._edb.Definition.PadGeometryType.Bullet
+            antipad_shape = self._edb.definition.PadGeometryType.Bullet
         else:
             antipad_array = Array[type(antipaddiam)]([antipaddiam])
-            antipad_shape = self._edb.Definition.PadGeometryType.Circle
-
-        for layer in ["Default"] + layers:
+            antipad_shape = self._edb.definition.PadGeometryType.Circle
+        if add_default_layer:
+            layers = layers + ["Default"]
+        for layer in layers:
             # padparam_array = Array[type(paddiam)]([paddiam])
             padstackData.SetPadParameters(
                 layer,
-                self._edb.Definition.PadType.RegularPad,
+                self._edb.definition.PadType.RegularPad,
                 pad_shape,
                 pad_array,
                 pad_offset_x,
                 pad_offset_y,
                 pad_rotation,
             )
 
             padstackData.SetPadParameters(
                 layer,
-                self._edb.Definition.PadType.AntiPad,
+                self._edb.definition.PadType.AntiPad,
                 antipad_shape,
                 antipad_array,
                 offset_x,
                 offset_y,
                 rotation,
             )
 
-        padstackDefinition = self._edb.Definition.PadstackDef.Create(self.db, padstackname)
+        padstackDefinition = self._edb.definition.PadstackDef.Create(self.db, padstackname)
         padstackDefinition.SetData(padstackData)
         self._logger.info("Padstack %s create correctly", padstackname)
         return padstackname
 
     @pyaedt_function_handler()
     def _get_pin_layer_range(self, pin):
         res, fromlayer, tolayer = pin.GetLayerRange()
@@ -967,20 +980,20 @@
             Name of the new padstack.
         Returns
         -------
         str
             Name of the new padstack.
         """
         p1 = self.definitions[target_padstack_name].edb_padstack.GetData()
-        new_padstack_definition_data = self._edb.Definition.PadstackDefData(p1)
+        new_padstack_definition_data = self._edb.definition.PadstackDefData(p1)
 
         if not new_padstack_name:
             new_padstack_name = generate_unique_name(target_padstack_name)
 
-        padstack_definition = self._edb.Definition.PadstackDef.Create(self.db, new_padstack_name)
+        padstack_definition = self._edb.definition.PadstackDef.Create(self.db, new_padstack_name)
         padstack_definition.SetData(new_padstack_definition_data)
 
         return new_padstack_name
 
     @pyaedt_function_handler()
     def place(
         self,
@@ -1022,45 +1035,51 @@
         -------
         :class:`pyaedt.edb_core.edb_data.padstacks_data.EDBPadstackInstance`
         """
         padstack = None
         for pad in list(self.definitions.keys()):
             if pad == definition_name:
                 padstack = self.definitions[pad].edb_padstack
-        position = self._edb.Geometry.PointData(self._get_edb_value(position[0]), self._get_edb_value(position[1]))
+        position = self._edb.geometry.point_data(position[0], position[1])
         net = self._pedb.nets.find_or_create_net(net_name)
         rotation = self._get_edb_value(rotation * math.pi / 180)
         sign_layers_values = {i: v for i, v in self._pedb.stackup.signal_layers.items()}
         sign_layers = list(sign_layers_values.keys())
         if not fromlayer:
-            fromlayer = sign_layers_values[sign_layers[0]]._edb_layer
+            try:
+                fromlayer = sign_layers_values[list(self.definitions[pad].pad_by_layer.keys())[0]]._edb_layer
+            except KeyError:
+                fromlayer = sign_layers_values[sign_layers[0]]._edb_layer
         else:
             fromlayer = sign_layers_values[fromlayer]._edb_layer
 
         if not tolayer:
-            tolayer = sign_layers_values[sign_layers[-1]]._edb_layer
+            try:
+                tolayer = sign_layers_values[list(self.definitions[pad].pad_by_layer.keys())[-1]]._edb_layer
+            except KeyError:
+                tolayer = sign_layers_values[sign_layers[-1]]._edb_layer
         else:
             tolayer = sign_layers_values[tolayer]._edb_layer
         if solderlayer:
             solderlayer = sign_layers_values[solderlayer]._edb_layer
         if padstack:
-            padstack_instance = self._edb.Cell.Primitive.PadstackInstance.Create(
+            padstack_instance = self._edb.cell.primitive.padstack_instance.create(
                 self._active_layout,
                 net,
                 via_name,
                 padstack,
                 position,
                 rotation,
                 fromlayer,
                 tolayer,
                 solderlayer,
                 None,
             )
             padstack_instance.SetIsLayoutPin(is_pin)
-            py_padstack_instance = EDBPadstackInstance(padstack_instance, self._pedb)
+            py_padstack_instance = EDBPadstackInstance(padstack_instance.api_object, self._pedb)
 
             return py_padstack_instance
         else:
             return False
 
     @pyaedt_function_handler()
     def place_padstack(
@@ -1129,20 +1148,20 @@
             Layer name on which remove the PadParameters. If None, all layers will be taken.
 
         Returns
         -------
         bool
             ``True`` if successful.
         """
-        pad_type = self._edb.Definition.PadType.RegularPad
-        pad_geo = self._edb.Definition.PadGeometryType.Circle
+        pad_type = self._edb.definition.PadType.RegularPad
+        pad_geo = self._edb.definition.PadGeometryType.Circle
         vals = self._get_edb_value(0)
         params = convert_py_list_to_net_list([self._get_edb_value(0)])
         p1 = self.definitions[padstack_name].edb_padstack.GetData()
-        newPadstackDefinitionData = self._edb.Definition.PadstackDefData(p1)
+        newPadstackDefinitionData = self._edb.definition.PadstackDefData(p1)
 
         if not layer_name:
             layer_name = list(self._pedb.stackup.signal_layers.keys())
         elif isinstance(layer_name, str):
             layer_name = [layer_name]
         for lay in layer_name:
             newPadstackDefinitionData.SetPadParameters(lay, pad_type, pad_geo, params, vals, vals, vals)
@@ -1198,19 +1217,19 @@
 
         Returns
         -------
         bool
             ``True`` if successful.
         """
         shape_dict = {
-            "Circle": self._edb.Definition.PadGeometryType.Circle,
-            "Square": self._edb.Definition.PadGeometryType.Square,
-            "Rectangle": self._edb.Definition.PadGeometryType.Rectangle,
-            "Oval": self._edb.Definition.PadGeometryType.Oval,
-            "Bullet": self._edb.Definition.PadGeometryType.Bullet,
+            "Circle": self._edb.definition.PadGeometryType.Circle,
+            "Square": self._edb.definition.PadGeometryType.Square,
+            "Rectangle": self._edb.definition.PadGeometryType.Rectangle,
+            "Oval": self._edb.definition.PadGeometryType.Oval,
+            "Bullet": self._edb.definition.PadGeometryType.Bullet,
         }
         pad_shape = shape_dict[pad_shape]
         if not isinstance(pad_params, list):
             pad_params = [pad_params]
         pad_params = convert_py_list_to_net_list([self._get_edb_value(i) for i in pad_params])
         pad_x_offset = self._get_edb_value(pad_x_offset)
         pad_y_offset = self._get_edb_value(pad_y_offset)
@@ -1221,32 +1240,32 @@
             antipad_params = [antipad_params]
         antipad_params = convert_py_list_to_net_list([self._get_edb_value(i) for i in antipad_params])
         antipad_x_offset = self._get_edb_value(antipad_x_offset)
         antipad_y_offset = self._get_edb_value(antipad_y_offset)
         antipad_rotation = self._get_edb_value(antipad_rotation)
 
         p1 = self.definitions[padstack_name].edb_padstack.GetData()
-        new_padstack_def = self._edb.Definition.PadstackDefData(p1)
+        new_padstack_def = self._edb.definition.PadstackDefData(p1)
         if not layer_name:
             layer_name = list(self._pedb.stackup.signal_layers.keys())
         elif isinstance(layer_name, str):
             layer_name = [layer_name]
         for layer in layer_name:
             new_padstack_def.SetPadParameters(
                 layer,
-                self._edb.Definition.PadType.RegularPad,
+                self._edb.definition.PadType.RegularPad,
                 pad_shape,
                 pad_params,
                 pad_x_offset,
                 pad_y_offset,
                 pad_rotation,
             )
             new_padstack_def.SetPadParameters(
                 layer,
-                self._edb.Definition.PadType.AntiPad,
+                self._edb.definition.PadType.AntiPad,
                 antipad_shape,
                 antipad_params,
                 antipad_x_offset,
                 antipad_y_offset,
                 antipad_rotation,
             )
         self.definitions[padstack_name].edb_padstack.SetData(new_padstack_def)
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.79/pyaedt/edb_core/siwave.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,17 @@
     >>> edb_siwave = edbapp.siwave
     """
 
     def __init__(self, p_edb):
         self._pedb = p_edb
 
     @property
-    def _builder(self):
-        """Builder."""
-        return self._pedb.builder
-
-    @property
     def _edb(self):
         """EDB."""
-        return self._pedb.edb
+        return self._pedb.edb_api
 
     def _get_edb_value(self, value):
         """Get the Edb value."""
         return self._pedb.edb_value(value)
 
     @property
     def _logger(self):
@@ -65,22 +60,27 @@
 
     @property
     def _active_layout(self):
         """Active layout."""
         return self._pedb.active_layout
 
     @property
+    def _layout(self):
+        """Active layout."""
+        return self._pedb.layout
+
+    @property
     def _cell(self):
         """Cell."""
         return self._pedb.active_cell
 
     @property
     def _db(self):
         """ """
-        return self._pedb.db
+        return self._pedb.active_db
 
     @property
     def excitations(self):
         """Get all excitations."""
         return self._pedb.excitations
 
     @property
@@ -99,15 +99,15 @@
 
         Returns
         -------
         list
             List of all layout pin groups.
         """
         _pingroups = {}
-        for el in self._active_layout.PinGroups:
+        for el in self._layout.pin_groups:
             _pingroups[el.GetName()] = PinGroup(el.GetName(), el, self._pedb)
         return _pingroups
 
     @pyaedt_function_handler()
     def _create_terminal_on_pins(self, source):
         """Create a terminal on pins.
 
@@ -121,77 +121,77 @@
         neg_pin = source.negative_node.node_pins
 
         res, fromLayer_pos, toLayer_pos = pos_pin.GetLayerRange()
         res, fromLayer_neg, toLayer_neg = neg_pin.GetLayerRange()
 
         pos_pingroup_terminal = _retry_ntimes(
             10,
-            self._edb.Cell.Terminal.PadstackInstanceTerminal.Create,
+            self._edb.cell.terminal.PadstackInstanceTerminal.Create,
             self._active_layout,
             pos_pin.GetNet(),
             pos_pin.GetName(),
             pos_pin,
             toLayer_pos,
         )
         time.sleep(0.5)
         neg_pingroup_terminal = _retry_ntimes(
             20,
-            self._edb.Cell.Terminal.PadstackInstanceTerminal.Create,
+            self._edb.cell.terminal.PadstackInstanceTerminal.Create,
             self._active_layout,
             neg_pin.GetNet(),
             neg_pin.GetName(),
             neg_pin,
             toLayer_neg,
         )
         if source.source_type in [SourceType.CoaxPort, SourceType.CircPort, SourceType.LumpedPort]:
-            pos_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.PortBoundary)
-            neg_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.PortBoundary)
+            pos_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.PortBoundary)
+            neg_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.PortBoundary)
             pos_pingroup_terminal.SetImpedance(self._get_edb_value(source.impedance))
             if source.source_type == SourceType.CircPort:
                 pos_pingroup_terminal.SetIsCircuitPort(True)
                 neg_pingroup_terminal.SetIsCircuitPort(True)
             pos_pingroup_terminal.SetReferenceTerminal(neg_pingroup_terminal)
             try:
                 pos_pingroup_terminal.SetName(source.name)
             except:
                 name = generate_unique_name(source.name)
                 pos_pingroup_terminal.SetName(name)
                 self._logger.warning("%s already exists. Renaming to %s", source.name, name)
         elif source.source_type == SourceType.Isource:
-            pos_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kCurrentSource)
-            neg_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kCurrentSource)
+            pos_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kCurrentSource)
+            neg_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kCurrentSource)
             pos_pingroup_terminal.SetSourceAmplitude(self._get_edb_value(source.magnitude))
             pos_pingroup_terminal.SetSourcePhase(self._get_edb_value(source.phase))
             pos_pingroup_terminal.SetReferenceTerminal(neg_pingroup_terminal)
             try:
                 pos_pingroup_terminal.SetName(source.name)
             except Exception as e:
                 name = generate_unique_name(source.name)
                 pos_pingroup_terminal.SetName(name)
                 self._logger.warning("%s already exists. Renaming to %s", source.name, name)
 
         elif source.source_type == SourceType.Vsource:
-            pos_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kVoltageSource)
-            neg_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kVoltageSource)
+            pos_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kVoltageSource)
+            neg_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kVoltageSource)
             pos_pingroup_terminal.SetSourceAmplitude(self._get_edb_value(source.magnitude))
             pos_pingroup_terminal.SetSourcePhase(self._get_edb_value(source.phase))
             pos_pingroup_terminal.SetReferenceTerminal(neg_pingroup_terminal)
             try:
                 pos_pingroup_terminal.SetName(source.name)
             except:
                 name = generate_unique_name(source.name)
                 pos_pingroup_terminal.SetName(name)
                 self._logger.warning("%s already exists. Renaming to %s", source.name, name)
 
         elif source.source_type == SourceType.Rlc:
-            pos_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.RlcBoundary)
-            neg_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.RlcBoundary)
+            pos_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.RlcBoundary)
+            neg_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.RlcBoundary)
             pos_pingroup_terminal.SetReferenceTerminal(neg_pingroup_terminal)
             pos_pingroup_terminal.SetSourceAmplitude(self._get_edb_value(source.rvalue))
-            Rlc = self._edb.Utility.Rlc()
+            Rlc = self._edb.utility.utility.Rlc()
             Rlc.CEnabled = False
             Rlc.LEnabled = False
             Rlc.REnabled = True
             Rlc.R = self._get_edb_value(source.rvalue)
             pos_pingroup_terminal.SetRlcBoundaryParameters(Rlc)
             try:
                 pos_pingroup_terminal.SetName(source.name)
@@ -280,48 +280,48 @@
             if not reference_net:
                 self._logger.info("no reference net provided, searching net {} instead.".format(layer_name))
                 reference_net = self._pedb.nets.get_net_by_name(layer_name)
                 if not reference_net:  # pragma no cover
                     self._logger.error("reference net {} not found.".format(layer_name))
                     return False
             else:
-                if not isinstance(reference_net, self._edb.Cell.Net):  # pragma no cover
+                if not isinstance(reference_net, self._edb.cell.net.net):  # pragma no cover
                     reference_net = self._pedb.nets.get_net_by_name(reference_net)
                 if not reference_net:
                     self._logger.error("Net {} not found".format(reference_net))
                     return False
             for pin_name in pins_name:  # pragma no cover
                 pin = [
                     pin
                     for pin in self._pedb.padstacks.get_pinlist_from_component_and_net(component_name)
                     if pin.GetName() == pin_name
                 ][0]
                 term_name = "{}_{}_{}".format(pin.GetComponent().GetName(), pin.GetNet().GetName(), pin.GetName())
                 res, start_layer, stop_layer = pin.GetLayerRange()
                 if res:
                     pin_instance = pin._edb_padstackinstance
-                    positive_terminal = self._edb.Cell.Terminal.PadstackInstanceTerminal.Create(
+                    positive_terminal = self._edb.cell.terminal.PadstackInstanceTerminal.Create(
                         self._active_layout, pin_instance.GetNet(), term_name, pin_instance, start_layer
                     )
-                    positive_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.PortBoundary)
-                    positive_terminal.SetImpedance(self._edb.Utility.Value(impedance))
+                    positive_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.PortBoundary)
+                    positive_terminal.SetImpedance(self._edb.utility.value(impedance))
                     positive_terminal.SetIsCircuitPort(True)
                     pos = self._pedb.components.get_pin_position(pin_instance)
-                    position = self._edb.Geometry.PointData(
-                        self._edb.Utility.Value(pos[0]), self._edb.Utility.Value(pos[1])
+                    position = self._edb.geometry.point_data(
+                        self._edb.utility.value(pos[0]), self._edb.utility.value(pos[1])
                     )
-                    negative_terminal = self._edb.Cell.Terminal.PointTerminal.Create(
+                    negative_terminal = self._edb.cell.terminal.PointTerminal.Create(
                         self._active_layout,
-                        reference_net,
+                        reference_net.net_obj,
                         "{}_ref".format(term_name),
                         position,
                         self._pedb.stackup.signal_layers[layer_name]._edb_layer,
                     )
-                    negative_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.PortBoundary)
-                    negative_terminal.SetImpedance(self._edb.Utility.Value(impedance))
+                    negative_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.PortBoundary)
+                    negative_terminal.SetImpedance(self._edb.utility.value(impedance))
                     negative_terminal.SetIsCircuitPort(True)
                     if positive_terminal.SetReferenceTerminal(negative_terminal):
                         self._logger.info("Port {} successfully created".format(term_name))
                         return positive_terminal
             return False
 
     @pyaedt_function_handler()
@@ -861,99 +861,99 @@
 
         Parameters
         ----------
         source : VoltageSource, CircuitPort, CurrentSource, DCTerminal or ResistorSource
             Name of the source.
 
         """
-        if source.name in [i.GetName() for i in list(self._active_layout.Terminals)]:
+        if source.name in [i.GetName() for i in self._layout.terminals]:
             source.name = generate_unique_name(source.name, n=3)
             self._logger.warning("Port already exists with same name. Renaming to {}".format(source.name))
         pos_pin_group = self._pedb.components.create_pingroup_from_pins(source.positive_node.node_pins)
         pos_node_net = self._pedb.nets.get_net_by_name(source.positive_node.net)
 
         pos_pingroup_term_name = source.name
         pos_pingroup_terminal = _retry_ntimes(
             10,
-            self._edb.Cell.Terminal.PinGroupTerminal.Create,
+            self._edb.cell.terminal.PinGroupTerminal.Create,
             self._active_layout,
-            pos_node_net,
+            pos_node_net.net_obj,
             pos_pingroup_term_name,
             pos_pin_group,
             False,
         )
         time.sleep(0.5)
         if source.negative_node.node_pins:
             neg_pin_group = self._pedb.components.create_pingroup_from_pins(source.negative_node.node_pins)
             neg_node_net = self._pedb.nets.get_net_by_name(source.negative_node.net)
             neg_pingroup_term_name = source.name + "_N"
             neg_pingroup_terminal = _retry_ntimes(
                 20,
-                self._edb.Cell.Terminal.PinGroupTerminal.Create,
+                self._edb.cell.terminal.PinGroupTerminal.Create,
                 self._active_layout,
-                neg_node_net,
+                neg_node_net.net_obj,
                 neg_pingroup_term_name,
                 neg_pin_group,
                 False,
             )
 
         if source.source_type in [SourceType.CoaxPort, SourceType.CircPort, SourceType.LumpedPort]:
-            pos_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.PortBoundary)
-            neg_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.PortBoundary)
+            pos_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.PortBoundary)
+            neg_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.PortBoundary)
             pos_pingroup_terminal.SetSourceAmplitude(self._get_edb_value(source.impedance))
             if source.source_type == SourceType.CircPort:
                 pos_pingroup_terminal.SetIsCircuitPort(True)
                 neg_pingroup_terminal.SetIsCircuitPort(True)
             pos_pingroup_terminal.SetReferenceTerminal(neg_pingroup_terminal)
             try:
                 pos_pingroup_terminal.SetName(source.name)
             except:
                 name = generate_unique_name(source.name)
                 pos_pingroup_terminal.SetName(name)
                 self._logger.warning("%s already exists. Renaming to %s", source.name, name)
 
         elif source.source_type == SourceType.Isource:
-            pos_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kCurrentSource)
-            neg_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kCurrentSource)
+            pos_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kCurrentSource)
+            neg_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kCurrentSource)
             pos_pingroup_terminal.SetSourceAmplitude(self._get_edb_value(source.magnitude))
-            pos_pingroup_terminal.SetSourcePhase(self._edb.Utility.Value(source.phase))
+            pos_pingroup_terminal.SetSourcePhase(self._edb.utility.value(source.phase))
             pos_pingroup_terminal.SetReferenceTerminal(neg_pingroup_terminal)
             try:
                 pos_pingroup_terminal.SetName(source.name)
             except Exception as e:
                 name = generate_unique_name(source.name)
                 pos_pingroup_terminal.SetName(name)
                 self._logger.warning("%s already exists. Renaming to %s", source.name, name)
 
         elif source.source_type == SourceType.Vsource:
-            pos_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kVoltageSource)
-            neg_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kVoltageSource)
+            pos_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kVoltageSource)
+            neg_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kVoltageSource)
             pos_pingroup_terminal.SetSourceAmplitude(self._get_edb_value(source.magnitude))
             pos_pingroup_terminal.SetSourcePhase(self._get_edb_value(source.phase))
             pos_pingroup_terminal.SetReferenceTerminal(neg_pingroup_terminal)
             try:
                 pos_pingroup_terminal.SetName(source.name)
             except:
                 name = generate_unique_name(source.name)
                 pos_pingroup_terminal.SetName(name)
                 self._logger.warning("%s already exists. Renaming to %s", source.name, name)
 
         elif source.source_type == SourceType.Rlc:
-            pos_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.RlcBoundary)
-            neg_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.RlcBoundary)
+            pos_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.RlcBoundary)
+            neg_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.RlcBoundary)
             pos_pingroup_terminal.SetReferenceTerminal(neg_pingroup_terminal)
             pos_pingroup_terminal.SetSourceAmplitude(self._get_edb_value(source.rvalue))
-            Rlc = self._edb.Utility.Rlc()
+            Rlc = self._edb.utility.utility.Rlc()
             Rlc.CEnabled = False
             Rlc.LEnabled = False
             Rlc.REnabled = True
             Rlc.R = self._get_edb_value(source.rvalue)
             pos_pingroup_terminal.SetRlcBoundaryParameters(Rlc)
         elif source.source_type == SourceType.DcTerminal:
-            pos_pingroup_terminal.SetBoundaryType(self._edb.Cell.Terminal.BoundaryType.kDcTerminal)
+            pos_pingroup_terminal.SetBoundaryType(self._edb.cell.terminal.BoundaryType.kDcTerminal)
         else:
             pass
         return pos_pingroup_terminal.GetName()
 
     @pyaedt_function_handler()
     def configure_siw_analysis_setup(self, simulation_setup=None, delete_existing_setup=True):
         """Configure Siwave analysis setup.
@@ -1010,38 +1010,42 @@
             if simulation_setup.ignore_non_functional_pads:  # pragma: no cover
                 simsetup_info.SimulationSettings.AdvancedSettings.IgnoreNonFunctionalPads = (
                     simulation_setup.ignore_non_functional_pads
                 )
             if simulation_setup.min_void_area:  # pragma: no cover
                 simsetup_info.SimulationSettings.DCAdvancedSettings.DcMinVoidAreaToMesh = simulation_setup.min_void_area
             try:
-                sweep = self._pedb.simsetupdata.SweepData(simulation_setup.sweep_name)
-                sweep.IsDiscrete = False  # need True for package??
-                sweep.UseQ3DForDC = simulation_setup.use_q3d_for_dc
-                sweep.RelativeSError = simulation_setup.relative_error
-                sweep.InterpUsePortImpedance = False
-                sweep.EnforceCausality = (GeometryOperators.parse_dim_arg(simulation_setup.start_freq) - 0) < 1e-9
-                sweep.EnforcePassivity = simulation_setup.enforce_passivity
-                sweep.PassivityTolerance = simulation_setup.passivity_tolerance
-                sweep.Frequencies.Clear()
-                if simulation_setup.sweep_type == SweepType.LogCount:  # pragma: no cover
-                    self._setup_decade_count_sweep(
-                        sweep,
-                        simulation_setup.start_freq,
-                        simulation_setup.stop_freq,
-                        simulation_setup.decade_count,
-                    )
+                if simulation_setup.add_frequency_sweep:
+                    self._logger.info("Adding frequency sweep")
+                    sweep = self._pedb.simsetupdata.SweepData(simulation_setup.sweep_name)
+                    sweep.IsDiscrete = False  # need True for package??
+                    sweep.UseQ3DForDC = simulation_setup.use_q3d_for_dc
+                    sweep.RelativeSError = simulation_setup.relative_error
+                    sweep.InterpUsePortImpedance = False
+                    sweep.EnforceCausality = (GeometryOperators.parse_dim_arg(simulation_setup.start_freq) - 0) < 1e-9
+                    sweep.EnforcePassivity = simulation_setup.enforce_passivity
+                    sweep.PassivityTolerance = simulation_setup.passivity_tolerance
+                    sweep.Frequencies.Clear()
+                    if simulation_setup.sweep_type == SweepType.LogCount:  # pragma: no cover
+                        self._setup_decade_count_sweep(
+                            sweep,
+                            simulation_setup.start_freq,
+                            simulation_setup.stop_freq,
+                            simulation_setup.decade_count,
+                        )
+                    else:
+                        sweep.Frequencies = self._pedb.simsetupdata.SweepData.SetFrequencies(
+                            simulation_setup.start_freq, simulation_setup.stop_freq, simulation_setup.step_freq
+                        )
+                    simsetup_info.SweepDataList.Add(sweep)
                 else:
-                    sweep.Frequencies = self._pedb.simsetupdata.SweepData.SetFrequencies(
-                        simulation_setup.start_freq, simulation_setup.stop_freq, simulation_setup.step_freq
-                    )
-                simsetup_info.SweepDataList.Add(sweep)
+                    self._logger.info("Adding frequency sweep disabled")
             except Exception as err:
                 self._logger.error("Exception in sweep configuration: {0}.".format(err))
-            edb_sim_setup = self._edb.Utility.SIWaveSimulationSetup(simsetup_info)
+            edb_sim_setup = self._edb.utility.utility.SIWaveSimulationSetup(simsetup_info)
             for setup in self._cell.SimulationSetups:
                 self._cell.DeleteSimulationSetup(setup.GetName())
                 self._logger.warning("Setup {} has been deleted".format(setup.GetName()))
             return self._cell.AddSimulationSetup(edb_sim_setup)
         if simulation_setup.solver_type == SolverType.SiwaveDC:  # pragma: no cover
             dcir_setup = self._pedb.simsetupdata.SimSetupInfo[
                 self._pedb.simsetupdata.SIwave.SIWDCIRSimulationSettings
@@ -1089,15 +1093,15 @@
             dcir_setup.SimulationSettings.DCIRSettings.PerPinUsePinFormat = simulation_setup.dc_per_pin_use_pin_format
             dcir_setup.SimulationSettings.DCIRSettings.UseLoopResForPerPin = (
                 simulation_setup.dc_use_loop_res_for_per_pin
             )
             dcir_setup.SimulationSettings.DCIRSettings.ViaReportPath = simulation_setup.dc_via_report_path
             dcir_setup.SimulationSettings.DCIRSettings.SourceTermsToGround = simulation_setup.dc_source_terms_to_ground
             dcir_setup.Name = simulation_setup.setup_name
-            sim_setup = self._edb.Utility.SIWaveDCIRSimulationSetup(dcir_setup)
+            sim_setup = self._edb.utility.utility.SIWaveDCIRSimulationSetup(dcir_setup)
             for setup in self._cell.SimulationSetups:
                 self._cell.DeleteSimulationSetup(setup.GetName())
                 self._logger.warning("Setup {} has been delete".format(setup.GetName()))
             return self._cell.AddSimulationSetup(sim_setup)
 
     @pyaedt_function_handler()
     def _setup_decade_count_sweep(self, sweep, start_freq, stop_freq, decade_count):
@@ -1183,18 +1187,18 @@
         -------
         PinGroup
         """
         if not isinstance(pin_numbers, list):
             pin_numbers = [pin_numbers]
         pin_numbers = [str(p) for p in pin_numbers]
         if group_name is None:
-            group_name = self._edb.Cell.Hierarchy.PinGroup.GetUniqueName(self._active_layout)
+            group_name = self._edb.cell.hierarchy.pin_group.GetUniqueName(self._active_layout)
         comp = self._pedb.components.components[reference_designator]
         pins = [pin.pin for name, pin in comp.pins.items() if name in pin_numbers]
-        edb_pingroup = self._edb.Cell.Hierarchy.PinGroup.Create(
+        edb_pingroup = self._edb.cell.hierarchy.pin_group.Create(
             self._active_layout, group_name, convert_py_list_to_net_list(pins)
         )
 
         if edb_pingroup.IsNull():  # pragma: no cover
             return False
         else:
             edb_pingroup.SetNet(pins[0].GetNet())
```

### Comparing `pyaedt-0.6.78/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.79/pyaedt/edb_core/stackup.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         """Layer types.
 
         Returns
         -------
         type
             Types of layers.
         """
-        return self._pedb.edb.Cell.LayerType
+        return self._pedb.edb_api.cell.layer_type
 
     @property
     def thickness(self):
         """Retrieve Stackup thickness.
 
         Returns
         -------
@@ -288,30 +288,32 @@
                 method="insert_above",
             )
         return True
 
     @pyaedt_function_handler()
     def refresh_layer_collection(self):
         """Refresh layer collection from Edb. This method is run on demand after all edit operations on stackup."""
-        lc_readonly = self._pedb._active_layout.GetLayerCollection()
-        layers = [i.Clone() for i in list(list(lc_readonly.Layers(self._pedb.edb.Cell.LayerTypeSet.StackupLayerSet)))]
+        lc_readonly = self._pedb.layout.layer_collection
+        layers = [
+            i.Clone() for i in list(list(lc_readonly.Layers(self._pedb.edb_api.cell.layer_type_set.StackupLayerSet)))
+        ]
         non_stackup = [
-            i.Clone() for i in list(list(lc_readonly.Layers(self._pedb.edb.Cell.LayerTypeSet.NonStackupLayerSet)))
+            i.Clone() for i in list(list(lc_readonly.Layers(self._pedb.edb_api.cell.layer_type_set.NonStackupLayerSet)))
         ]
-        self._lc = self._pedb.edb.Cell.LayerCollection()
+        self._lc = self._pedb.edb_api.cell._cell.LayerCollection()
         mode = lc_readonly.GetMode()
         self._lc.SetMode(lc_readonly.GetMode())
         if str(mode) == "Overlapping":
             for layer in layers:
                 self._lc.AddStackupLayerAtElevation(layer)
         elif str(mode) == "Laminate":
             for layer in layers:
                 self._lc.AddLayerBottom(layer)
         else:
-            self._lc.AddLayers(convert_py_list_to_net_list(layers, self._pedb.edb.Cell.Layer))
+            self._lc.AddLayers(convert_py_list_to_net_list(layers, self._pedb.edb_api.cell.layer))
         for layer in non_stackup:
             self._lc.AddLayerBottom(layer)
         self._lc.SetMode(lc_readonly.GetMode())
 
     @property
     def _layer_collection(self):
         """Copy of EDB layer collection.
@@ -339,30 +341,30 @@
             * 2 - MultiZone
         """
         self._stackup_mode = self._layer_collection.GetMode()
         return str(self._stackup_mode)
 
     @stackup_mode.setter
     def stackup_mode(self, value):
-        mode = self._pedb.edb.Cell.LayerCollectionMode
+        mode = self._pedb.edb_api.Cell.LayerCollectionMode
         if value == 0 or value == mode.Laminate or value == "Laminate":
             self._layer_collection.SetMode(mode.Laminate)
         elif value == 1 or value == mode.Overlapping or value == "Overlapping":
             self._layer_collection.SetMode(mode.Overlapping)
         elif value == 2 or value == mode.MultiZone or value == "MultiZone":
             self._layer_collection.SetMode(mode.MultiZone)
-        self._pedb._active_layout.SetLayerCollection(self._layer_collection)
+        self._pedb.layout.layer_collection = self._layer_collection
 
     @property
     def _edb_layer_list(self):
-        return list(self._layer_collection.Layers(self._pedb.edb.Cell.LayerTypeSet.AllLayerSet))
+        return list(self._layer_collection.Layers(self._pedb.edb_api.cell.layer_type_set.AllLayerSet))
 
     @property
     def _edb_layer_list_nonstackup(self):
-        return list(self._layer_collection.Layers(self._pedb.edb.Cell.LayerTypeSet.NonStackupLayerSet))
+        return list(self._layer_collection.Layers(self._pedb.edb_api.cell.layer_type_set.NonStackupLayerSet))
 
     @property
     def layers(self):
         """Retrieve the dictionary of layers.
 
         Returns
         -------
@@ -378,15 +380,15 @@
     def signal_layers(self):
         """Retrieve the dictionary of signal layers.
 
         Returns
         -------
         Dict[str, :class:`pyaedt.edb_core.edb_data.layer_data.LayerEdbClass`]
         """
-        layer_type = self._pedb.edb.Cell.LayerType.SignalLayer
+        layer_type = self._pedb.edb_api.cell.layer_type.SignalLayer
         _lays = OrderedDict()
         for name, obj in self.layers.items():
             if obj._edb_layer.GetLayerType() == layer_type:
                 _lays[name] = obj
         return _lays
 
     @property
@@ -394,16 +396,16 @@
         """Retrieve the dictionary of signal and dielectric layers.
 
         Returns
         -------
         Dict[str, :class:`pyaedt.edb_core.edb_data.layer_data.LayerEdbClass`]
         """
         layer_type = [
-            self._pedb.edb.Cell.LayerType.SignalLayer,
-            self._pedb.edb.Cell.LayerType.DielectricLayer,
+            self._pedb.edb_api.cell.layer_type.SignalLayer,
+            self._pedb.edb_api.cell.layer_type.DielectricLayer,
         ]
         _lays = OrderedDict()
         for name, obj in self.layers.items():
             if obj._edb_layer.GetLayerType() in layer_type:
                 _lays[name] = obj
         return _lays
 
@@ -412,15 +414,15 @@
         """Dielectric layers.
 
         Returns
         -------
         dict[str, :class:`pyaedt.edb_core.edb_data.layer_data.EDBLayer`]
             Dictionary of dielectric layers.
         """
-        layer_type = self._pedb.edb.Cell.LayerType.DielectricLayer
+        layer_type = self._pedb.edb_api.cell.layer_type.DielectricLayer
         _lays = OrderedDict()
         for name, obj in self.layers.items():
             if obj._edb_layer.GetLayerType() == layer_type:
                 _lays[name] = obj
         return _lays
 
     @property
@@ -451,22 +453,24 @@
             Name of the base layer. The default value is ``None``.
         Returns
         -------
 
         """
         _lc = self._layer_collection
         if operation in ["change_position", "change_attribute", "change_name"]:
-            lc_readonly = self._pedb._active_layout.GetLayerCollection()
+            lc_readonly = self._pedb.layout.layer_collection
             layers = [
-                i.Clone() for i in list(list(lc_readonly.Layers(self._pedb.edb.Cell.LayerTypeSet.StackupLayerSet)))
+                i.Clone()
+                for i in list(list(lc_readonly.Layers(self._pedb.edb_api.cell.layer_type_set.StackupLayerSet)))
             ]
             non_stackup = [
-                i.Clone() for i in list(list(lc_readonly.Layers(self._pedb.edb.Cell.LayerTypeSet.NonStackupLayerSet)))
+                i.Clone()
+                for i in list(list(lc_readonly.Layers(self._pedb.edb_api.cell.layer_type_set.NonStackupLayerSet)))
             ]
-            _lc = self._pedb.edb.Cell.LayerCollection()
+            _lc = self._pedb.edb_api.cell._cell.LayerCollection()
             mode = lc_readonly.GetMode()
             _lc.SetMode(lc_readonly.GetMode())
             if str(mode) == "Overlapping":
                 for layer in layers:
                     if layer.GetName() == layer_clone.GetName() or layer.GetName() == base_layer:
                         _lc.AddStackupLayerAtElevation(layer_clone)
                     else:
@@ -488,84 +492,84 @@
             _lc.AddLayerTop(layer_clone)
         elif operation == "add_on_bottom":
             _lc.AddLayerBottom(layer_clone)
         elif operation == "add_at_elevation":
             _lc.AddStackupLayerAtElevation(layer_clone)
         elif operation == "non_stackup":
             _lc.AddLayerBottom(layer_clone)
-        result = self._pedb._active_layout.SetLayerCollection(_lc)
+        self._pedb.layout.layer_collection = _lc
         self.refresh_layer_collection()
-        return result
+        return True
 
     @pyaedt_function_handler()
     def _create_stackup_layer(self, layer_name, thickness, layer_type="signal"):
         if layer_type == "signal":
-            _layer_type = self._pedb.edb.Cell.LayerType.SignalLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.SignalLayer
         else:
-            _layer_type = self._pedb.edb.Cell.LayerType.DielectricLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.DielectricLayer
 
-        result = self._pedb.edb.Cell.StackupLayer(
+        result = self._pedb.edb_api.cell._cell.StackupLayer(
             layer_name,
             _layer_type,
             self._edb_value(thickness),
             self._edb_value(0),
             "",
         )
         self.refresh_layer_collection()
         return result
 
     @pyaedt_function_handler()
     def _create_nonstackup_layer(self, layer_name, layer_type):
         if layer_type == "conducting":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.ConductingLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.ConductingLayer
         elif layer_type == "airlines":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.AirlinesLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.AirlinesLayer
         elif layer_type == "error":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.ErrorsLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.ErrorsLayer
         elif layer_type == "symbol":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.SymbolLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.SymbolLayer
         elif layer_type == "measure":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.MeasureLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.MeasureLayer
         elif layer_type == "assembly":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.AssemblyLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.AssemblyLayer
         elif layer_type == "silkscreen":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.SilkscreenLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.SilkscreenLayer
         elif layer_type == "soldermask":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.SolderMaskLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.SolderMaskLayer
         elif layer_type == "solderpaste":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.SolderPasteLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.SolderPasteLayer
         elif layer_type == "glue":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.GlueLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.GlueLayer
         elif layer_type == "wirebond":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.WirebondLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.WirebondLayer
         elif layer_type == "user":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.UserLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.UserLayer
         elif layer_type == "siwavehfsssolverregions":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.SIwaveHFSSSolverRegions
+            _layer_type = self._pedb.edb_api.cell.layer_type.SIwaveHFSSSolverRegions
         elif layer_type == "outline":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.OutlineLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.OutlineLayer
         elif layer_type == "postprocessing":  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.PostprocessingLayer
+            _layer_type = self._pedb.edb_api.cell.layer_type.PostprocessingLayer
         else:  # pragma: no cover
-            _layer_type = self._pedb.edb.Cell.LayerType.UndefinedLayerType
+            _layer_type = self._pedb.edb_api.cell.layer_type.UndefinedLayerType
 
-        result = self._pedb.edb.Cell.Layer(layer_name, _layer_type)
+        result = self._pedb.edb_api.cell.layer(layer_name, _layer_type)
         self.refresh_layer_collection()
         return result
 
     @pyaedt_function_handler()
     def add_outline_layer(self, outline_name="Outline"):
         """Add an outline layer named ``"Outline"`` if it is not present.
 
         Returns
         -------
         bool
             "True" if successful, ``False`` if failed.
         """
-        outlineLayer = self._pedb.edb.Cell.Layer.FindByName(self._pedb.active_layout.GetLayerCollection(), outline_name)
+        outlineLayer = self._pedb.edb_api.cell.layer.FindByName(self._pedb.layout.layer_collection, outline_name)
         if outlineLayer.IsNull():
             return self.add_layer(
                 outline_name,
                 layer_type="outline",
                 material="",
                 fillMaterial="",
                 thickness="",
@@ -677,22 +681,22 @@
         name : str
             Name of the layer to remove.
 
         Returns
         -------
 
         """
-        new_layer_collection = self._pedb.edb.Cell.LayerCollection()
+        new_layer_collection = self._pedb.edb_api.Cell.LayerCollection()
         for lyr in self._edb_layer_list:
             if not (lyr.GetName() == name):
                 new_layer_collection.AddLayerBottom(lyr)
 
-        result = self._pedb._active_layout.SetLayerCollection(new_layer_collection)
+        self._pedb.layout.layer_collection = new_layer_collection
         self.refresh_layer_collection()
-        return result
+        return True
 
     @pyaedt_function_handler
     def export(self, fpath, file_format="xml", include_material_with_layer=False):
         """Export stackup definition to a CSV or JSON file.
 
         Parameters
         ----------
@@ -895,17 +899,17 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         if only_metals:
-            input_layers = self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet
+            input_layers = self._pedb.edb_api.cell.layer_type_set.SignalLayerSet
         else:
-            input_layers = self._pedb.edb.Cell.LayerTypeSet.StackupLayerSet
+            input_layers = self._pedb.edb_api.cell.layer_type_set.StackupLayerSet
 
         res, topl, topz, bottoml, bottomz = self._layer_collection.GetTopBottomStackupLayers(input_layers)
         return topl.GetName(), topz, bottoml.GetName(), bottomz
 
     @pyaedt_function_handler()
     def flip_design(self):
         """Flip the current design of a layout.
@@ -920,109 +924,115 @@
         >>> edb = Edb(edbpath=targetfile,  edbversion="2021.2")
         >>> edb.stackup.flip_design()
         >>> edb.save()
         >>> edb.close_edb()
         """
         try:
             lc = self._layer_collection
-            new_lc = self._pedb.edb.Cell.LayerCollection()
+            new_lc = self._pedb.edb_api.Cell.LayerCollection()
             lc_mode = lc.GetMode()
             new_lc.SetMode(lc_mode)
             max_elevation = 0.0
-            for layer in lc.Layers(self._pedb.edb.Cell.LayerTypeSet.StackupLayerSet):
+            for layer in lc.Layers(self._pedb.edb_api.cell.layer_type_set.StackupLayerSet):
                 if "RadBox" not in layer.GetName():  # Ignore RadBox
                     lower_elevation = layer.Clone().GetLowerElevation() * 1.0e6
                     upper_elevation = layer.Clone().GetUpperElevation() * 1.0e6
                     max_elevation = max([max_elevation, lower_elevation, upper_elevation])
 
             non_stackup_layers = []
-            for layer in lc.Layers(self._pedb.edb.Cell.LayerTypeSet.AllLayerSet):
+            for layer in lc.Layers(self._pedb.edb_api.cell.layer_type_set.AllLayerSet):
                 cloned_layer = layer.Clone()
                 if not cloned_layer.IsStackupLayer():
                     non_stackup_layers.append(cloned_layer)
                     continue
                 if "RadBox" not in cloned_layer.GetName() and not cloned_layer.IsViaLayer():
                     upper_elevation = cloned_layer.GetUpperElevation() * 1.0e6
                     updated_lower_el = max_elevation - upper_elevation
                     val = self._edb_value("{}um".format(updated_lower_el))
                     cloned_layer.SetLowerElevation(val)
-                    if cloned_layer.GetTopBottomAssociation() == self._pedb.edb.Cell.TopBottomAssociation.TopAssociated:
-                        cloned_layer.SetTopBottomAssociation(self._pedb.edb.Cell.TopBottomAssociation.BottomAssociated)
+                    if (
+                        cloned_layer.GetTopBottomAssociation()
+                        == self._pedb.edb_api.Cell.TopBottomAssociation.TopAssociated
+                    ):
+                        cloned_layer.SetTopBottomAssociation(
+                            self._pedb.edb_api.Cell.TopBottomAssociation.BottomAssociated
+                        )
                     else:
-                        cloned_layer.SetTopBottomAssociation(self._pedb.edb.Cell.TopBottomAssociation.TopAssociated)
+                        cloned_layer.SetTopBottomAssociation(self._pedb.edb_api.Cell.TopBottomAssociation.TopAssociated)
                     new_lc.AddStackupLayerAtElevation(cloned_layer)
 
             vialayers = [
-                lay for lay in lc.Layers(self._pedb.edb.Cell.LayerTypeSet.StackupLayerSet) if lay.Clone().IsViaLayer()
+                lay
+                for lay in lc.Layers(self._pedb.edb_api.cell.layer_type_set.StackupLayerSet)
+                if lay.Clone().IsViaLayer()
             ]
             for layer in vialayers:
                 cloned_via_layer = layer.Clone()
                 upper_ref_name = cloned_via_layer.GetRefLayerName(True)
                 lower_ref_name = cloned_via_layer.GetRefLayerName(False)
                 upper_ref = [
                     lay
-                    for lay in lc.Layers(self._pedb.edb.Cell.LayerTypeSet.AllLayerSet)
+                    for lay in lc.Layers(self._pedb.edb_api.cell.layer_type_set.AllLayerSet)
                     if lay.GetName() == upper_ref_name
                 ][0]
                 lower_ref = [
                     lay
-                    for lay in lc.Layers(self._pedb.edb.Cell.LayerTypeSet.AllLayerSet)
+                    for lay in lc.Layers(self._pedb.edb_api.cell.layer_type_set.AllLayerSet)
                     if lay.GetName() == lower_ref_name
                 ][0]
                 cloned_via_layer.SetRefLayer(lower_ref, True)
                 cloned_via_layer.SetRefLayer(upper_ref, False)
                 ref_layer_in_flipped_stackup = [
                     lay
-                    for lay in new_lc.Layers(self._pedb.edb.Cell.LayerTypeSet.AllLayerSet)
+                    for lay in new_lc.Layers(self._pedb.edb_api.cell.layer_type_set.AllLayerSet)
                     if lay.GetName() == upper_ref_name
                 ][0]
                 via_layer_lower_elevation = (
                     ref_layer_in_flipped_stackup.GetLowerElevation() + ref_layer_in_flipped_stackup.GetThickness()
                 )
                 cloned_via_layer.SetLowerElevation(self._edb_value(via_layer_lower_elevation))
                 new_lc.AddStackupLayerAtElevation(cloned_via_layer)
 
             layer_list = convert_py_list_to_net_list(non_stackup_layers)
             new_lc.AddLayers(layer_list)
-            if not self._pedb.active_layout.SetLayerCollection(new_lc):
-                self._pedb.logger.error("Failed to Flip Stackup.")
-                return False
+            self._pedb.layout.layer_collection = new_lc
+
             for pyaedt_cmp in list(self._pedb.components.components.values()):
                 cmp = pyaedt_cmp.edbcomponent
                 cmp_type = cmp.GetComponentType()
                 cmp_prop = cmp.GetComponentProperty().Clone()
                 try:
                     if (
                         cmp_prop.GetSolderBallProperty().GetPlacement()
-                        == self._pedb.Definition.SolderballPlacement.AbovePadstack
+                        == self._pedb.definition.SolderballPlacement.AbovePadstack
                     ):
                         sball_prop = cmp_prop.GetSolderBallProperty().Clone()
-                        sball_prop.SetPlacement(self._pedb.Definition.SolderballPlacement.BelowPadstack)
+                        sball_prop.SetPlacement(self._pedb.definition.SolderballPlacement.BelowPadstack)
                         cmp_prop.SetSolderBallProperty(sball_prop)
                     elif (
                         cmp_prop.GetSolderBallProperty().GetPlacement()
-                        == self._pedb.Definition.SolderballPlacement.BelowPadstack
+                        == self._pedb.definition.SolderballPlacement.BelowPadstack
                     ):
                         sball_prop = cmp_prop.GetSolderBallProperty().Clone()
-                        sball_prop.SetPlacement(self._pedb.Definition.SolderballPlacement.AbovePadstack)
+                        sball_prop.SetPlacement(self._pedb.definition.SolderballPlacement.AbovePadstack)
                         cmp_prop.SetSolderBallProperty(sball_prop)
                 except:
                     pass
-                if cmp_type == self._pedb.Definition.ComponentType.IC:
+                if cmp_type == self._pedb.definition.ComponentType.IC:
                     die_prop = cmp_prop.GetDieProperty().Clone()
                     chip_orientation = die_prop.GetOrientation()
-                    if chip_orientation == self._pedb.Definition.DieOrientation.ChipDown:
-                        die_prop.SetOrientation(self._pedb.Definition.DieOrientation.ChipUp)
+                    if chip_orientation == self._pedb.definition.DieOrientation.ChipDown:
+                        die_prop.SetOrientation(self._pedb.definition.DieOrientation.ChipUp)
                         cmp_prop.SetDieProperty(die_prop)
                     else:
-                        die_prop.SetOrientation(self._pedb.Definition.DieOrientation.ChipDown)
+                        die_prop.SetOrientation(self._pedb.definition.DieOrientation.ChipDown)
                         cmp_prop.SetDieProperty(die_prop)
                 cmp.SetComponentProperty(cmp_prop)
 
-            lay_list = list(new_lc.Layers(self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet))
+            lay_list = list(new_lc.Layers(self._pedb.edb_api.cell.layer_type_set.SignalLayerSet))
             for padstack in list(self._pedb.padstacks.instances.values()):
                 start_layer_id = [lay.GetLayerId() for lay in list(lay_list) if lay.GetName() == padstack.start_layer]
                 stop_layer_id = [lay.GetLayerId() for lay in list(lay_list) if lay.GetName() == padstack.stop_layer]
                 layer_map = padstack._edb_padstackinstance.GetLayerMap()
                 layer_map.SetMapping(stop_layer_id[0], start_layer_id[0])
                 padstack._edb_padstackinstance.SetLayerMap(layer_map)
             self.refresh_layer_collection()
@@ -1165,37 +1175,36 @@
             self.flip_design()
         edb_cell = edb.active_cell
         _angle = self._edb_value(angle * math.pi / 180.0)
         _offset_x = self._edb_value(offset_x)
         _offset_y = self._edb_value(offset_y)
 
         if edb_cell.GetName() not in self._pedb.cell_names:
-            _dbCell = convert_py_list_to_net_list([edb_cell])
-            list_cells = self._pedb.db.CopyCells(_dbCell)
+            list_cells = self._pedb.copy_cells([edb_cell.api_object])
             edb_cell = list_cells[0]
-        self._pedb.active_layout.GetCell().SetBlackBox(True)
-        cell_inst2 = self._pedb.edb.Cell.Hierarchy.CellInstance.Create(
-            edb_cell.GetLayout(), self._pedb.active_layout.GetCell().GetName(), self._pedb.active_layout
+        self._pedb.layout.cell.SetBlackBox(True)
+        cell_inst2 = self._pedb.edb_api.cell.hierarchy.cell_instance.Create(
+            edb_cell.GetLayout(), self._pedb.layout.cell.GetName(), self._pedb.active_layout
         )
         cell_trans = cell_inst2.GetTransform()
         cell_trans.SetRotationValue(_angle)
         cell_trans.SetXOffsetValue(_offset_x)
         cell_trans.SetYOffsetValue(_offset_y)
         cell_trans.SetMirror(flipped_stackup)
         cell_inst2.SetTransform(cell_trans)
         cell_inst2.SetSolveIndependentPreference(False)
         stackup_target = edb_cell.GetLayout().GetLayerCollection()
 
         if place_on_top:
             cell_inst2.SetPlacementLayer(
-                list(stackup_target.Layers(self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet))[0]
+                list(stackup_target.Layers(self._pedb.edb_api.cell.layer_type_set.SignalLayerSet))[0]
             )
         else:
             cell_inst2.SetPlacementLayer(
-                list(stackup_target.Layers(self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet))[-1]
+                list(stackup_target.Layers(self._pedb.edb_api.cell.layer_type_set.SignalLayerSet))[-1]
             )
         self.refresh_layer_collection()
         return True
 
     @pyaedt_function_handler()
     def place_in_layout_3d_placement(
         self,
@@ -1275,35 +1284,34 @@
             rotation = self._edb_value(math.pi)
 
         edb_cell = edb.active_cell
         _offset_x = self._edb_value(offset_x)
         _offset_y = self._edb_value(offset_y)
 
         if edb_cell.GetName() not in self._pedb.cell_names:
-            _dbCell = convert_py_list_to_net_list([edb_cell])
-            list_cells = self._pedb.db.CopyCells(_dbCell)
+            list_cells = self._pedb.copy_cells(edb_cell.api_object)
             edb_cell = list_cells[0]
-        self._pedb.active_layout.GetCell().SetBlackBox(True)
-        cell_inst2 = self._pedb.edb.Cell.Hierarchy.CellInstance.Create(
-            edb_cell.GetLayout(), self._pedb.active_layout.GetCell().GetName(), self._pedb.active_layout
+        self._pedb.layout.cell.SetBlackBox(True)
+        cell_inst2 = self._pedb.edb_api.cell.hierarchy.cell_instance.Create(
+            edb_cell.GetLayout(), self._pedb.layout.cell.GetName(), self._pedb.active_layout
         )
 
-        stackup_target = self._pedb.edb.Cell.LayerCollection(edb_cell.GetLayout().GetLayerCollection())
-        stackup_source = self._pedb.edb.Cell.LayerCollection(self._pedb.active_layout.GetLayerCollection())
+        stackup_target = self._pedb.edb_api.Cell.LayerCollection(edb_cell.GetLayout().GetLayerCollection())
+        stackup_source = self._pedb.edb_api.Cell.LayerCollection(self._pedb.layout.layer_collection)
 
         if place_on_top:
             cell_inst2.SetPlacementLayer(
-                list(stackup_target.Layers(self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet))[0]
+                list(stackup_target.Layers(self._pedb.edb_api.cell.layer_type_set.SignalLayerSet))[0]
             )
         else:
             cell_inst2.SetPlacementLayer(
-                list(stackup_target.Layers(self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet))[-1]
+                list(stackup_target.Layers(self._pedb.edb_api.cell.layer_type_set.SignalLayerSet))[-1]
             )
         cell_inst2.SetIs3DPlacement(True)
-        sig_set = self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet
+        sig_set = self._pedb.edb_api.cell.layer_type_set.SignalLayerSet
         res = stackup_target.GetTopBottomStackupLayers(sig_set)
         target_top_elevation = res[2]
         target_bottom_elevation = res[4]
         res_s = stackup_source.GetTopBottomStackupLayers(sig_set)
         source_stack_top_elevation = res_s[2]
         source_stack_bot_elevation = res_s[4]
 
@@ -1415,48 +1423,47 @@
                     solder_height = max(lay_solder_height, solder_height)
                     component_edb.stackup._remove_solder_pec(lay.name)
         edb_cell = component_edb.active_cell
         _offset_x = self._edb_value(offset_x)
         _offset_y = self._edb_value(offset_y)
 
         if edb_cell.GetName() not in self._pedb.cell_names:
-            _dbCell = convert_py_list_to_net_list([edb_cell])
-            list_cells = self._pedb.db.CopyCells(_dbCell)
+            list_cells = self._pedb.copy_cells(edb_cell.api_object)
             edb_cell = list_cells[0]
-        for cell in list(self._pedb.db.CircuitCells):
+        for cell in list(self._pedb.active_db.CircuitCells):
             if cell.GetName() == edb_cell.GetName():
                 edb_cell = cell
         # Keep Cell Independent
         edb_cell.SetBlackBox(True)
         rotation = self._edb_value(0.0)
         if flipped_stackup:
             rotation = self._edb_value(math.pi)
 
         _offset_x = self._edb_value(offset_x)
         _offset_y = self._edb_value(offset_y)
 
         instance_name = generate_unique_name(edb_cell.GetName(), n=2)
 
-        cell_inst2 = self._pedb.edb.Cell.Hierarchy.CellInstance.Create(
+        cell_inst2 = self._pedb.edb_api.cell.hierarchy.cell_instance.Create(
             self._pedb.active_layout, instance_name, edb_cell.GetLayout()
         )
 
-        stackup_source = self._pedb.edb.Cell.LayerCollection(edb_cell.GetLayout().GetLayerCollection())
-        stackup_target = self._pedb.edb.Cell.LayerCollection(self._pedb.active_layout.GetLayerCollection())
+        stackup_source = self._pedb.edb_api.Cell.LayerCollection(edb_cell.GetLayout().GetLayerCollection())
+        stackup_target = self._pedb.edb_api.Cell.LayerCollection(self._pedb.layout.layer_collection)
 
         if place_on_top:
             cell_inst2.SetPlacementLayer(
-                list(stackup_target.Layers(self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet))[0]
+                list(stackup_target.Layers(self._pedb.edb_api.cell.layer_type_set.SignalLayerSet))[0]
             )
         else:
             cell_inst2.SetPlacementLayer(
-                list(stackup_target.Layers(self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet))[-1]
+                list(stackup_target.Layers(self._pedb.edb_api.cell.layer_type_set.SignalLayerSet))[-1]
             )
         cell_inst2.SetIs3DPlacement(True)
-        sig_set = self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet
+        sig_set = self._pedb.edb_api.cell.layer_type_set.SignalLayerSet
         res = stackup_target.GetTopBottomStackupLayers(sig_set)
         target_top_elevation = res[2]
         target_bottom_elevation = res[4]
         res_s = stackup_source.GetTopBottomStackupLayers(sig_set)
         source_stack_top_elevation = res_s[2]
         source_stack_bot_elevation = res_s[4]
 
@@ -1532,29 +1539,29 @@
         zero_data = self._edb_value(0.0)
         one_data = self._edb_value(1.0)
         local_origin = self._pedb.point_3d(0.0, 0.0, 0.0)
         rotation_axis_from = self._pedb.point_3d(1.0, 0.0, 0.0)
         _angle = angle * math.pi / 180.0
         rotation_axis_to = self._pedb.point_3d(math.cos(_angle), -1 * math.sin(_angle), 0.0)
 
-        stackup_target = self._pedb.edb.Cell.LayerCollection(self._pedb.active_layout.GetLayerCollection())
-        sig_set = self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet
+        stackup_target = self._pedb.edb_api.cell._cell.LayerCollection(self._pedb.layout.layer_collection)
+        sig_set = self._pedb.edb_api.cell.layer_type_set.SignalLayerSet
         res = stackup_target.GetTopBottomStackupLayers(sig_set)
         target_top_elevation = res[2]
         target_bottom_elevation = res[4]
         flip_angle = self._edb_value("0deg")
         if place_on_top:
             elevation = target_top_elevation + offset_z
         else:
             flip_angle = self._edb_value("180deg")
             elevation = target_bottom_elevation - offset_z
         h_stackup = self._edb_value(elevation)
         location = self._pedb.point_3d(offset_x, offset_y, h_stackup)
 
-        mcad_model = self._pedb.edb.McadModel.Create3DComp(self._pedb.active_layout, a3dcomp_path)
+        mcad_model = self._pedb.edb_api.McadModel.Create3DComp(self._pedb.active_layout, a3dcomp_path)
         if mcad_model.IsNull():  # pragma: no cover
             logger.error("Failed to create MCAD model from a3dcomp")
             return False
 
         cell_instance = mcad_model.GetCellInstance()
         if cell_instance.IsNull():  # pragma: no cover
             logger.error("Cell instance of a3dcomp is null")
@@ -1950,18 +1957,19 @@
             material = {}
             for i in list(m):
                 material[i.tag] = list(i)[0].text
             material_dict[m.attrib["Name"]] = material
 
         self._add_materials_from_dictionary(material_dict)
 
-        new_layer_collection = self._pedb.edb.Cell.LayerCollection()
+        new_layer_collection = self._pedb.edb_api.Cell.LayerCollection()
         result = new_layer_collection.ImportFromControlFile(file_path)
         if result:
-            return self._pedb._active_layout.SetLayerCollection(new_layer_collection)
+            self._pedb.layout.layer_collection = new_layer_collection
+            return True
 
     @pyaedt_function_handler
     def _export_xml(self, file_path):
         """Export stackup information to an external XMLfile.
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.6.78/pyaedt/emit.py` & `pyaedt-0.6.79/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.79/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/emit_core/EmitConstants.py` & `pyaedt-0.6.79/pyaedt/emit_core/EmitConstants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.79/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.79/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.79/pyaedt/emit_core/results/revision.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,16 +144,14 @@
         ----------
         >>> domain = aedtapp.results.interaction_domain()
         >>> rev.run(domain)
 
         """
         self._load_revision()
         engine = self.emit_project._emit_api.get_engine()
-        if domain.interferer_names and engine.max_simultaneous_interferers != len(domain.interferer_names):
-            raise ValueError("The max_simultaneous_interferers must equal the number of interferers in the domain.")
         interaction = engine.run(domain)
         # save the revision
         self.emit_project._emit_api.save_project()
         return interaction
 
     @pyaedt_function_handler()
     def is_domain_valid(self, domain):
@@ -352,7 +350,37 @@
         design = self.emit_project.odesign
         return design.GetResultNotes(self.name)
 
     @notes.setter
     def notes(self, notes):
         self.emit_project.odesign.SetResultNotes(self.name, notes)
         self.emit_project._emit_api.save_project()
+
+    @property
+    def max_n_to_1_instances(self):
+        """
+        The maximum number of instances per band combination allowed to run for N to 1.
+        A value of 0 disables N to 1 entirely.
+        A value of -1 allows unlimited N to 1 instances.
+
+        Examples
+        ----------
+        >>> aedtapp.results.current_revision.max_n_to_1_instances = 2**20
+        >>> aedtapp.results.current_revision.max_n_to_1_instances
+        1048576
+        """
+        if self.emit_project._aedt_version < "2024.1":  # pragma: no cover
+            raise RuntimeError("This function only supported in AEDT version 2024.1 and later.")
+        if self.revision_loaded:
+            engine = self.emit_project._emit_api.get_engine()
+            max_instances = engine.max_n_to_1_instances
+        else:  # pragma: no cover
+            max_instances = None
+        return max_instances
+
+    @max_n_to_1_instances.setter
+    def max_n_to_1_instances(self, max_instances):
+        if self.emit_project._aedt_version < "2024.1":  # pragma: no cover
+            raise RuntimeError("This function only supported in AEDT version 2024.1 and later.")
+        if self.revision_loaded:
+            engine = self.emit_project._emit_api.get_engine()
+            engine.max_n_to_1_instances = max_instances
```

### Comparing `pyaedt-0.6.78/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.79/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.79/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/clr_module.py` & `pyaedt-0.6.79/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/configurations.py` & `pyaedt-0.6.79/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/constants.py` & `pyaedt-0.6.79/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/design_types.py` & `pyaedt-0.6.79/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/filesystem.py` & `pyaedt-0.6.79/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/general_methods.py` & `pyaedt-0.6.79/pyaedt/generic/general_methods.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.79/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.79/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/pdf.py` & `pyaedt-0.6.79/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/plot.py` & `pyaedt-0.6.79/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/process.py` & `pyaedt-0.6.79/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.79/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.79/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/toolkit.py` & `pyaedt-0.6.79/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.79/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/hfss.py` & `pyaedt-0.6.79/pyaedt/hfss.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,24 +211,36 @@
     class BoundaryType(object):
         """Creates and manages boundaries."""
 
         (PerfectE, PerfectH, Aperture, Radiation, Impedance, LayeredImp, LumpedRLC, FiniteCond, Hybrid) = range(0, 9)
 
     @property
     def hybrid(self):
-        """HFSS hybrid mode for the active solution."""
+        """HFSS hybrid mode for the active solution.
+
+        For instance, it must be set to ``True`` to define the solution type as 'HFSS with Hybrid and Arrays'.
+
+        Returns
+        -------
+        bool
+        """
         return self.design_solutions.hybrid
 
     @hybrid.setter
     def hybrid(self, value):
         self.design_solutions.hybrid = value
 
     @property
     def composite(self):
-        """HFSS composite mode for the active solution."""
+        """HFSS composite mode for the active solution.
+
+        Returns
+        -------
+        bool
+        """
         return self.design_solutions.composite
 
     @composite.setter
     def composite(self, value):
         self.design_solutions.composite = value
 
     @pyaedt_function_handler()
```

### Comparing `pyaedt-0.6.78/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.79/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/icepak.py` & `pyaedt-0.6.79/pyaedt/icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/maxwell.py` & `pyaedt-0.6.79/pyaedt/maxwell.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.79/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/mechanical.py` & `pyaedt-0.6.79/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/Console.py_build` & `pyaedt-0.6.79/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.79/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.79/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.79/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.79/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.79/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/amat.xml` & `pyaedt-0.6.79/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/console_setup.py` & `pyaedt-0.6.79/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.79/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.79/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.79/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.79/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/misc.py` & `pyaedt-0.6.79/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.79/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.79/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.79/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.79/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.79/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.79/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/misc/template.acf` & `pyaedt-0.6.79/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.79/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.79/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.79/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.79/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.79/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.79/pyaedt/modeler/cad/Modeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,19 +142,19 @@
         >>> from pyaedt import Maxwell2d
         >>> app = Maxwell2d()
         >>> cs_copy = [i for i in app.modeler.coordinate_systems]
         >>> [i.delete() for i in cs_copy]
         """
         try:
             self._modeler.oeditor.Delete(["NAME:Selections", "Selections:=", self.name])
-            if "ref_cs" in dir(self):
-                for cs in range(0, len(self._modeler.coordinate_systems)):
-                    if self._modeler.coordinate_systems[cs].ref_cs == self.name:
-                        self._modeler.coordinate_systems.pop(cs)
             self._modeler.coordinate_systems.pop(self._modeler.coordinate_systems.index(self))
+            coordinate_systems = self._modeler._app.oeditor.GetRelativeCoordinateSystems()
+            for cs in self._modeler.coordinate_systems[:]:
+                if cs.name not in coordinate_systems:
+                    self._modeler.coordinate_systems.pop(self._modeler.coordinate_systems.index(cs))
             self._modeler.cleanup_objects()
         except:
             self._modeler._app.logger.warning("Coordinate system does not exist")
         return True
 
     @pyaedt_function_handler()
     def set_as_working_cs(self):
```

### Comparing `pyaedt-0.6.78/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.79/pyaedt/modeler/cad/Primitives.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.79/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.79/pyaedt/modeler/cad/Primitives3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.79/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.79/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.79/pyaedt/modeler/cad/object3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.79/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/calculators.py` & `pyaedt-0.6.79/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.79/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.79/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.79/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.79/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.79/pyaedt/modeler/modeler3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -857,42 +857,47 @@
                     and bounding_box[2] <= bound[5] <= bounding_box[5]
                 ):
                     objects.append(obj)
 
         return objects
 
     @pyaedt_function_handler()
-    def import_nastran(self, file_path, import_lines=True, lines_thickness=0):
-        """Import Nastran file into 3D Modeler by converting it to stl and reading it.
+    def import_nastran(self, file_path, import_lines=True, lines_thickness=0, import_solids=True):
+        """Import Nastran file into 3D Modeler by converting the faces to stl and reading it. The solids are
+        translated directly to AEDT format.
 
         Parameters
         ----------
         file_path : str
             Path to .nas file.
         import_lines : bool, optional
             Whether to import the lines or only triangles. Default is ``True``.
         lines_thickness : float, optional
             Whether to thicken lines after creation and it's default value.
             Every line will be parametrized with a design variable called ``xsection_linename``.
+        import_solids : bool, optional
+            Whether to import the solids or only triangles. Default is ``True``.
 
         Returns
         -------
         List of :class:`pyaedt.modeler.Object3d.Object3d`
         """
-        nas_to_dict = {"Points": {}, "PointsId": {}, "Triangles": {}, "Lines": {}}
+        nas_to_dict = {"Points": {}, "PointsId": {}, "Triangles": {}, "Lines": {}, "Solids": {}}
+
+        self.logger.reset_timer()
+        self.logger.info("Loading file")
         with open(file_path, "r") as f:
             lines = f.read().splitlines()
             id = 0
             for line in lines:
                 line_split = [line[i : i + 8] for i in range(0, len(line), 8)]
                 if len(line_split) < 5:
                     continue
                 if line_split[0].startswith("GRID"):
                     try:
-                        n_1_3 = line[24:48]
                         import re
 
                         out = re.findall("^.{24}(.{8})(.{8})(.{8})", line)[0]
                         n1 = out[0].replace(".-", ".e-").strip()
                         n2 = out[1].replace(".-", ".e-").strip()
                         n3 = out[2].replace(".-", ".e-").strip()
 
@@ -924,85 +929,211 @@
                         nas_to_dict["Triangles"][int(line_split[2])] = [
                             [
                                 int(line_split[3]),
                                 int(line_split[4]),
                                 int(line_split[5]),
                             ]
                         ]
+                elif line_split[0].startswith("CPENTA"):
+                    if int(line_split[2]) in nas_to_dict["Solids"]:
+                        nas_to_dict["Solids"][int(line_split[2])].append(
+                            [
+                                line_split[0].strip(),
+                                int(line_split[3]),
+                                int(line_split[4]),
+                                int(line_split[5]),
+                                int(line_split[6]),
+                                int(line_split[7]),
+                                int(line_split[8]),
+                            ]
+                        )
+                    else:
+                        nas_to_dict["Solids"][int(line_split[2])] = [
+                            [
+                                line_split[0].strip(),
+                                int(line_split[3]),
+                                int(line_split[4]),
+                                int(line_split[5]),
+                                int(line_split[6]),
+                                int(line_split[7]),
+                                int(line_split[8]),
+                            ]
+                        ]
+                elif line_split[0].startswith("CHEXA"):
+                    if int(line_split[2]) in nas_to_dict["Solids"]:
+                        nas_to_dict["Solids"][int(line_split[2])].append(
+                            [
+                                line_split[0].strip(),
+                                int(line_split[3]),
+                                int(line_split[4]),
+                                int(line_split[5]),
+                                int(line_split[6]),
+                                int(line_split[7]),
+                                int(line_split[8]),
+                                int(line_split[9]),
+                                int(line_split[10]),
+                            ]
+                        )
+                    else:
+                        nas_to_dict["Solids"][int(line_split[2])] = [
+                            [
+                                line_split[0].strip(),
+                                int(line_split[3]),
+                                int(line_split[4]),
+                                int(line_split[5]),
+                                int(line_split[6]),
+                                int(line_split[7]),
+                                int(line_split[8]),
+                                int(line_split[9]),
+                                int(line_split[10]),
+                            ]
+                        ]
+                elif line_split[0].startswith("CTETRA"):
+                    if int(line_split[2]) in nas_to_dict["Solids"]:
+                        nas_to_dict["Solids"][int(line_split[2])].append(
+                            [
+                                line_split[0].strip(),
+                                int(line_split[3]),
+                                int(line_split[4]),
+                                int(line_split[5]),
+                                int(line_split[6]),
+                            ]
+                        )
+                    else:
+                        nas_to_dict["Solids"][int(line_split[2])] = [
+                            [
+                                line_split[0].strip(),
+                                int(line_split[3]),
+                                int(line_split[4]),
+                                int(line_split[5]),
+                                int(line_split[6]),
+                            ]
+                        ]
                 elif line_split[0].startswith("CROD") or line_split[0].startswith("CBEAM"):
                     if int(line_split[2]) in nas_to_dict["Lines"]:
                         nas_to_dict["Lines"][int(line_split[2])].append([int(line_split[3]), int(line_split[4])])
                     else:
                         nas_to_dict["Lines"][int(line_split[2])] = [[int(line_split[3]), int(line_split[4])]]
+        self.logger.info_timer("File loaded")
         objs_before = [i for i in self.object_names]
-        f = open(os.path.join(self._app.working_directory, self._app.design_name + "_test.stl"), "w")
-        f.write("solid PyaedtStl\n")
-        for triangles in nas_to_dict["Triangles"].values():
-            for triangle in triangles:
-                try:
-                    points = [nas_to_dict["Points"][id] for id in triangle]
-                except KeyError:
-                    continue
-                fc = GeometryOperators.get_polygon_centroid(points)
-                v1 = points[0]
-                v2 = points[1]
-                cv1 = GeometryOperators.v_points(fc, v1)
-                cv2 = GeometryOperators.v_points(fc, v2)
-                if cv2[0] == cv1[0] == 0.0 and cv2[1] == cv1[1] == 0.0:
-                    n = [0, 0, 1]
-                elif cv2[0] == cv1[0] == 0.0 and cv2[2] == cv1[2] == 0.0:
-                    n = [0, 1, 0]
-                elif cv2[1] == cv1[1] == 0.0 and cv2[2] == cv1[2] == 0.0:
-                    n = [1, 0, 0]
-                else:
-                    n = GeometryOperators.v_cross(cv1, cv2)
-                normal = GeometryOperators.normalize_vector(n)
-                if normal:
-                    f.write(" facet normal {} {} {}\n".format(normal[0], normal[1], normal[2]))
-                    f.write("  outer loop\n")
-                    f.write("   vertex {} {} {}\n".format(points[0][0], points[0][1], points[0][2]))
-                    f.write("   vertex {} {} {}\n".format(points[1][0], points[1][1], points[1][2]))
-                    f.write("   vertex {} {} {}\n".format(points[2][0], points[2][1], points[2][2]))
-                    f.write("  endloop\n")
-                    f.write(" endfacet\n")
-
-        f.write("endsolid\n")
-        f.close()
-        self.import_3d_cad(os.path.join(self._app.working_directory, self._app.design_name + "_test.stl"))
-        if not import_lines:
-            return True
-
-        for line_name, lines in nas_to_dict["Lines"].items():
-            if lines_thickness:
-                self._app["x_section_{}".format(line_name)] = lines_thickness
-            polys = []
-            id = 0
-            for line in lines:
-                try:
-                    points = [nas_to_dict["Points"][line[0]], nas_to_dict["Points"][line[1]]]
-                except KeyError:
-                    continue
+        if nas_to_dict["Triangles"]:
+            self.logger.reset_timer()
+            self.logger.info("Creating STL file with detected faces")
+            f = open(os.path.join(self._app.working_directory, self._app.design_name + "_test.stl"), "w")
+            f.write("solid PyaedtStl\n")
+            for triangles in nas_to_dict["Triangles"].values():
+                for triangle in triangles:
+                    try:
+                        points = [nas_to_dict["Points"][id] for id in triangle]
+                    except KeyError:
+                        continue
+                    fc = GeometryOperators.get_polygon_centroid(points)
+                    v1 = points[0]
+                    v2 = points[1]
+                    cv1 = GeometryOperators.v_points(fc, v1)
+                    cv2 = GeometryOperators.v_points(fc, v2)
+                    if cv2[0] == cv1[0] == 0.0 and cv2[1] == cv1[1] == 0.0:
+                        n = [0, 0, 1]
+                    elif cv2[0] == cv1[0] == 0.0 and cv2[2] == cv1[2] == 0.0:
+                        n = [0, 1, 0]
+                    elif cv2[1] == cv1[1] == 0.0 and cv2[2] == cv1[2] == 0.0:
+                        n = [1, 0, 0]
+                    else:
+                        n = GeometryOperators.v_cross(cv1, cv2)
+                    normal = GeometryOperators.normalize_vector(n)
+                    if normal:
+                        f.write(" facet normal {} {} {}\n".format(normal[0], normal[1], normal[2]))
+                        f.write("  outer loop\n")
+                        f.write("   vertex {} {} {}\n".format(points[0][0], points[0][1], points[0][2]))
+                        f.write("   vertex {} {} {}\n".format(points[1][0], points[1][1], points[1][2]))
+                        f.write("   vertex {} {} {}\n".format(points[2][0], points[2][1], points[2][2]))
+                        f.write("  endloop\n")
+                        f.write(" endfacet\n")
+
+            f.write("endsolid\n")
+            f.close()
+            self.logger.info("STL file created")
+            self.import_3d_cad(os.path.join(self._app.working_directory, self._app.design_name + "_test.stl"))
+            self.logger.info_timer("Faces imported")
+
+        if import_lines:
+            for line_name, lines in nas_to_dict["Lines"].items():
                 if lines_thickness:
-                    polys.append(
-                        self.create_polyline(
-                            points,
-                            name="Poly_{}_{}".format(line_name, id),
-                            xsection_type="Circle",
-                            xsection_width="x_section_{}".format(line_name),
-                            xsection_num_seg=6,
-                        )
-                    )
-                else:
-                    polys.append(self.create_polyline(points, name="Poly_{}_{}".format(line_name, id)))
-                id += 1
-
-            if len(polys) > 1:
-                out_poly = self.unite(polys, purge=not lines_thickness)
-                if not lines_thickness and out_poly:
-                    self.generate_object_history(out_poly)
+                    self._app["x_section_{}".format(line_name)] = lines_thickness
+                polys = []
+                id = 0
+                for line in lines:
+                    try:
+                        points = [nas_to_dict["Points"][line[0]], nas_to_dict["Points"][line[1]]]
+                    except KeyError:
+                        continue
+                    if lines_thickness:
+                        polys.append(
+                            self.create_polyline(
+                                points,
+                                name="Poly_{}_{}".format(line_name, id),
+                                xsection_type="Circle",
+                                xsection_width="x_section_{}".format(line_name),
+                                xsection_num_seg=6,
+                            )
+                        )
+                    else:
+                        polys.append(self.create_polyline(points, name="Poly_{}_{}".format(line_name, id)))
+                    id += 1
+
+                if len(polys) > 1:
+                    out_poly = self.unite(polys, purge=not lines_thickness)
+                    if not lines_thickness and out_poly:
+                        self.generate_object_history(out_poly)
+
+        if import_solids and nas_to_dict["Solids"]:
+            self.logger.reset_timer()
+            self.logger.info("Loading solids")
+            for solid_pid in nas_to_dict["Solids"].keys():
+                for solid in nas_to_dict["Solids"][solid_pid]:
+                    points = [nas_to_dict["Points"][id] for id in solid[1:]]
+                    if solid[0] == "CPENTA":
+                        element1 = self._app.modeler.create_polyline(
+                            position_list=[points[0], points[1], points[2]], close_surface=True, cover_surface=True
+                        )
+                        element2 = self._app.modeler.create_polyline(
+                            position_list=[points[3], points[4], points[5]], close_surface=True, cover_surface=True
+                        )
+                        self._app.modeler.connect([element1.name, element2.name])
+                        element1.group_name = "PID_" + str(solid_pid)
+                    elif solid[0] == "CHEXA":
+                        element1 = self._app.modeler.create_polyline(
+                            position_list=[points[0], points[1], points[2], points[3]],
+                            close_surface=True,
+                            cover_surface=True,
+                        )
+                        element2 = self._app.modeler.create_polyline(
+                            position_list=[points[4], points[5], points[6], points[7]],
+                            close_surface=True,
+                            cover_surface=True,
+                        )
+                        self._app.modeler.connect([element1.name, element2.name])
+                        element1.group_name = "PID_" + str(solid_pid)
+                    elif solid[0] == "CTETRA":
+                        element1 = self._app.modeler.create_polyline(
+                            position_list=[points[0], points[1], points[2]], close_surface=True, cover_surface=True
+                        )
+                        element2 = self._app.modeler.create_polyline(
+                            position_list=[points[0], points[1], points[3]], close_surface=True, cover_surface=True
+                        )
+                        element3 = self._app.modeler.create_polyline(
+                            position_list=[points[0], points[2], points[3]], close_surface=True, cover_surface=True
+                        )
+                        element4 = self._app.modeler.create_polyline(
+                            position_list=[points[1], points[2], points[3]], close_surface=True, cover_surface=True
+                        )
+                        self._app.modeler.unite([element1.name, element2.name, element3.name, element4.name])
+                        element1.group_name = "PID_" + str(solid_pid)
+
+            self.logger.info_timer("Solids loaded")
 
         objs_after = [i for i in self.object_names]
         new_objects = [self[i] for i in objs_after if i not in objs_before]
         return new_objects
 
     @pyaedt_function_handler()
     def import_from_openstreet_map(
```

### Comparing `pyaedt-0.6.78/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.79/pyaedt/modeler/modelerpcb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.79/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.79/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modeler/schematic.py` & `pyaedt-0.6.79/pyaedt/modeler/schematic.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.79/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/Boundary.py` & `pyaedt-0.6.79/pyaedt/modules/Boundary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.79/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.79/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.79/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.79/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/Material.py` & `pyaedt-0.6.79/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.79/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/Mesh.py` & `pyaedt-0.6.79/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.79/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.79/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.79/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.79/pyaedt/modules/PostProcessor.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.79/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.79/pyaedt/modules/SolveSetup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.79/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.79/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/report_templates.py` & `pyaedt-0.6.79/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/modules/solutions.py` & `pyaedt-0.6.79/pyaedt/modules/solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/q3d.py` & `pyaedt-0.6.79/pyaedt/q3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/rmxprt.py` & `pyaedt-0.6.79/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.79/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.79/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.79/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.79/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.79/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyaedt/siwave.py` & `pyaedt-0.6.79/pyaedt/siwave.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         return self._version_keys
 
     @property
     def current_version(self):
         """Current version of AEDT."""
         return self.version_keys[0]
 
-    def __init__(self, specified_version=None):  # pragma: no cover
+    def __init__(self, specified_version=None):
         if is_ironpython:
             _com = "pythonnet"
             import System
         elif is_windows:  # pragma: no cover
             modules = [tup[1] for tup in pkgutil.iter_modules()]
             if _clr:
                 import win32com.client
```

### Comparing `pyaedt-0.6.78/pyaedt/twinbuilder.py` & `pyaedt-0.6.79/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.78/pyproject.toml` & `pyaedt-0.6.79/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -32,43 +32,43 @@
     "psutil",
     "dotnetcore2 ==3.1.23;platform_system=='Linux'",
 ]
 
 [project.optional-dependencies]
 tests = [
     "ipython==8.13.0",
-    "imageio==2.29.0",
+    "imageio==2.30.0",
     "joblib==1.2.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
-    "pandas==2.0.1; python_version > '3.7'",
+    "pandas==2.0.2; python_version > '3.7'",
     "pytest==7.3.1",
     "pytest-cov==4.0.0",
     "pytest-xdist==3.3.1",
     "pyvista==0.39.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "scikit-learn==1.2.2",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
     "ansys-sphinx-theme==0.9.9",
-    "imageio==2.29.0",
+    "imageio==2.30.0",
     "imageio-ffmpeg==0.4.8",
     "ipython==8.13.0",
     "ipywidgets==8.0.6",
     "joblib==1.2.0",
-    "jupyterlab==4.0.0",
+    "jupyterlab==4.0.1",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "nbsphinx==0.9.2",
     "numpydoc==1.5.0",
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
@@ -85,37 +85,37 @@
     "sphinxcontrib-websupport==1.2.4",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 full = [
-    "imageio==2.29.0",
+    "imageio==2.30.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
-    "pandas==2.0.1; python_version > '3.7'",
+    "pandas==2.0.2; python_version > '3.7'",
     "osmnx",
     "pyvista==0.39.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 all = [
-    "imageio==2.29.0",
+    "imageio==2.30.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
-    "pandas==2.0.1; python_version > '3.7'",
+    "pandas==2.0.2; python_version > '3.7'",
     "osmnx",
     "pyvista==0.39.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
```

### Comparing `pyaedt-0.6.78/PKG-INFO` & `pyaedt-0.6.79/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.78
+Version: 0.6.79
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -17,35 +17,35 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: cffi == 1.15.1;platform_system=='Linux'
 Requires-Dist: pywin32 >= 303;platform_system=='Windows'
 Requires-Dist: pythonnet == 3.0.1
 Requires-Dist: rpyc==5.3.1
 Requires-Dist: psutil
 Requires-Dist: dotnetcore2 ==3.1.23;platform_system=='Linux'
-Requires-Dist: imageio==2.29.0 ; extra == "all"
+Requires-Dist: imageio==2.30.0 ; extra == "all"
 Requires-Dist: matplotlib==3.5.3 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "all" and ( python_version <= '3.7')
-Requires-Dist: pandas==2.0.1 ; extra == "all" and ( python_version > '3.7')
+Requires-Dist: pandas==2.0.2 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
 Requires-Dist: pyvista==0.39.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
-Requires-Dist: imageio==2.29.0 ; extra == "doc"
+Requires-Dist: imageio==2.30.0 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
 Requires-Dist: ipython==8.13.0 ; extra == "doc"
 Requires-Dist: ipywidgets==8.0.6 ; extra == "doc"
 Requires-Dist: joblib==1.2.0 ; extra == "doc"
-Requires-Dist: jupyterlab==4.0.0 ; extra == "doc"
+Requires-Dist: jupyterlab==4.0.1 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: nbsphinx==0.9.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
@@ -60,39 +60,39 @@
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: scikit-rf ; extra == "doc"
 Requires-Dist: openpyxl==3.1.2 ; extra == "doc"
-Requires-Dist: imageio==2.29.0 ; extra == "full"
+Requires-Dist: imageio==2.30.0 ; extra == "full"
 Requires-Dist: matplotlib==3.5.3 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "full" and ( python_version <= '3.7')
-Requires-Dist: pandas==2.0.1 ; extra == "full" and ( python_version > '3.7')
+Requires-Dist: pandas==2.0.2 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
 Requires-Dist: pyvista==0.39.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.1.2 ; extra == "full"
 Requires-Dist: ipython==8.13.0 ; extra == "tests"
-Requires-Dist: imageio==2.29.0 ; extra == "tests"
+Requires-Dist: imageio==2.30.0 ; extra == "tests"
 Requires-Dist: joblib==1.2.0 ; extra == "tests"
 Requires-Dist: matplotlib==3.5.3 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
-Requires-Dist: pandas==2.0.1 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: pandas==2.0.2 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
 Requires-Dist: pytest-xdist==3.3.1 ; extra == "tests"
 Requires-Dist: pyvista==0.39.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: scikit-learn==1.2.2 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
```

