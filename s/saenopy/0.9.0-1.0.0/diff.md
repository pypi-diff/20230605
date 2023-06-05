# Comparing `tmp/saenopy-0.9.0.tar.gz` & `tmp/saenopy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saenopy-0.9.0.tar", max compression
+gzip compressed data, was "saenopy-1.0.0.tar", max compression
```

## Comparing `saenopy-0.9.0.tar` & `saenopy-1.0.0.tar`

### file list

```diff
@@ -1,117 +1,101 @@
--rw-r--r--   0        0        0     1065 2023-05-03 13:41:00.082380 saenopy-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     1187 2023-05-03 13:41:00.082380 saenopy-0.9.0/README.md
--rw-r--r--   0        0        0     1268 2023-05-03 13:41:00.202382 saenopy-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      451 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/__init__.py
--rw-r--r--   0        0        0     1467 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/buildBeams.py
--rw-r--r--   0        0        0     1329 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/conjugateGradient.py
--rw-r--r--   0        0        0     6868 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/examples.py
--rw-r--r--   0        0        0    15348 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/getDeformations.py
--rw-r--r--   0        0        0        0 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/code/__init__.py
--rw-r--r--   0        0        0     3918 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/code/code_editor.py
--rw-r--r--   0        0        0     7389 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/code/gui_code.py
--rw-r--r--   0        0        0     4605 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/code/script_file.py
--rw-r--r--   0        0        0     7099 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/code/syntax.py
--rw-r--r--   0        0        0    19372 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/common/QExtendedGraphicsView.py
--rw-r--r--   0        0        0    45878 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/common/QtShortCuts.py
--rw-r--r--   0        0        0        0 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/common/__init__.py
--rw-r--r--   0        0        0    21865 2023-05-03 13:41:00.202382 saenopy-0.9.0/saenopy/gui/common/gui_classes.py
--rw-r--r--   0        0        0    33197 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/lif_reader.py
--rw-r--r--   0        0        0     6027 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/patch_lifreader.py
--rw-r--r--   0        0        0      282 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/resources.py
--rw-r--r--   0        0        0    15449 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/sigmoid_widget.py
--rw-r--r--   0        0        0     6583 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/stack_preview.py
--rw-r--r--   0        0        0     3888 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/stack_selector.py
--rw-r--r--   0        0        0     9342 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/stack_selector_crop.py
--rw-r--r--   0        0        0     3096 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/stack_selector_leica.py
--rw-r--r--   0        0        0    11924 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/common/stack_selector_tif.py
--rw-r--r--   0        0        0     6616 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/gui_master.py
--rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/orientation/__init__.py
--rw-r--r--   0        0        0    51641 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/orientation/gui_orientation.py
--rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/analyze/__init__.py
--rw-r--r--   0        0        0    20407 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/analyze/plot_window.py
--rw-r--r--   0        0        0     1575 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/gui_solver.py
--rw-r--r--   0        0        0    16164 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/BatchEvaluate.py
--rw-r--r--   0        0        0    11509 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/DeformationDetector.py
--rw-r--r--   0        0        0     4242 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/FittedMesh.py
--rw-r--r--   0        0        0    11457 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/MeshCreator.py
--rw-r--r--   0        0        0     9449 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/PipelineModule.py
--rw-r--r--   0        0        0     1103 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/QTimeSlider.py
--rw-r--r--   0        0        0    13629 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/Regularizer.py
--rw-r--r--   0        0        0    10923 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/ResultView.py
--rw-r--r--   0        0        0    19430 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/StackDisplay.py
--rw-r--r--   0        0        0    12999 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/VTK_Toolbar.py
--rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/__init__.py
--rw-r--r--   0        0        0      541 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/code_export.py
--rw-r--r--   0        0        0     6446 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py
--rw-r--r--   0        0        0    47962 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/Exporter.py
--rw-r--r--   0        0        0    13663 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/ExporterRender2D.py
--rw-r--r--   0        0        0    17535 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/ExporterRender3D.py
--rw-r--r--   0        0        0    18777 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/FiberViewer.py
--rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/exporter/__init__.py
--rw-r--r--   0        0        0    11018 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/load_measurement_dialog.py
--rw-r--r--   0        0        0     3854 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/path_editor.py
--rw-r--r--   0        0        0    11908 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/solver/modules/showVectorField.py
--rw-r--r--   0        0        0        0 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/spheroid/__init__.py
--rw-r--r--   0        0        0    92474 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/gui/spheroid/gui_deformation_spheroid.py
--rw-r--r--   0        0        0    53944 2023-05-03 13:41:00.206382 saenopy-0.9.0/saenopy/img/Icon.ico
--rw-r--r--   0        0        0    42003 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/Logo.png
--rw-r--r--   0        0        0    77561 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/Logo.svg
--rw-r--r--   0        0        0    37691 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/Logo_black.png
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/arrowscale.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/autoscale0.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/autoscale1.ico
--rw-r--r--   0        0        0    48947 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/buttons.svg
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/center0.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/center1.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/contrast0.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/contrast1.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/grid.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/grid2.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/grid3.ico
--rw-r--r--   0        0        0    38885 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/logo_splash.png
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/nan0.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/nan1.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/show_image.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/show_image2.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/show_image3.ico
--rw-r--r--   0        0        0     3606 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/slice0.ico
--rw-r--r--   0        0        0     3606 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/slice1.ico
--rw-r--r--   0        0        0     3606 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/slice2.ico
--rw-r--r--   0        0        0     1150 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/slice_all.ico
--rw-r--r--   0        0        0   121664 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/thumbnails/BFTFM.png
--rw-r--r--   0        0        0   132449 2023-05-03 13:41:00.210382 saenopy-0.9.0/saenopy/img/thumbnails/BFTFM_2.png
--rw-r--r--   0        0        0   180081 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/thumbnails/Bead_example_icon.png
--rw-r--r--   0        0        0   202759 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/thumbnails/Dynamic_icon.png
--rw-r--r--   0        0        0   554429 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/thumbnails/StainedOrganoid_icon.png
--rw-r--r--   0        0        0   263760 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/thumbnails/liver_fibroblast_icon.png
--rw-r--r--   0        0        0     3606 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/view_single.ico
--rw-r--r--   0        0        0     3606 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/img/view_two.ico
--rw-r--r--   0        0        0     4021 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/loadHelpers.py
--rw-r--r--   0        0        0    17511 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/macro.py
--rw-r--r--   0        0        0    12590 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/materials.py
--rw-r--r--   0        0        0    22326 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/multigridHelper.py
--rw-r--r--   0        0        0      923 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/numbaOverload.py
--rw-r--r--   0        0        0    13782 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/result_file.py
--rw-r--r--   0        0        0     6611 2023-05-03 13:41:00.214383 saenopy-0.9.0/saenopy/saveable.py
--rw-r--r--   0        0        0    75256 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/solver.py
--rw-r--r--   0        0        0    11684 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/stack.py
--rw-r--r--   0        0        0    22838 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/VirtualBeads.py
--rw-r--r--   0        0        0        0 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/__init__.py
--rw-r--r--   0        0        0     3583 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/configHelper.py
--rw-r--r--   0        0        0     2788 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/convert_solver_to_result.py
--rw-r--r--   0        0        0    15114 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_deformation.py
--rw-r--r--   0        0        0    24879 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_deformation_wizard.py
--rw-r--r--   0        0        0     1225 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_master.spec
--rw-r--r--   0        0        0    13703 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_mpl.py
--rw-r--r--   0        0        0     3016 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_reorder.py
--rw-r--r--   0        0        0    15886 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/gui_vtk.py
--rw-r--r--   0        0        0    22642 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/load.py
--rw-r--r--   0        0        0    14055 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/main.py
--rw-r--r--   0        0        0    12568 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/meshViewer.py
--rw-r--r--   0        0        0      167 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/requirements.txt
--rw-r--r--   0        0        0     5639 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/save.py
--rw-r--r--   0        0        0    28379 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/stack3DHelper.py
--rw-r--r--   0        0        0    12051 2023-05-03 13:41:00.218382 saenopy-0.9.0/saenopy/unused/tfjit.py
--rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 saenopy-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-05 15:22:18.996823 saenopy-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     2183 2023-06-05 15:22:18.996823 saenopy-1.0.0/README.md
+-rw-r--r--   0        0        0     1307 2023-06-05 15:22:19.104823 saenopy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      348 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/__init__.py
+-rw-r--r--   0        0        0     1347 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/build_beams.py
+-rw-r--r--   0        0        0     1279 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/conjugate_gradient.py
+-rw-r--r--   0        0        0     7716 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/examples.py
+-rw-r--r--   0        0        0    15307 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/get_deformations.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/code/__init__.py
+-rw-r--r--   0        0        0     3918 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/code/code_editor.py
+-rw-r--r--   0        0        0     7389 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/code/gui_code.py
+-rw-r--r--   0        0        0     4605 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/code/script_file.py
+-rw-r--r--   0        0        0     7099 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/code/syntax.py
+-rw-r--r--   0        0        0    19372 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/QExtendedGraphicsView.py
+-rw-r--r--   0        0        0    46067 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/QtShortCuts.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/__init__.py
+-rw-r--r--   0        0        0    21886 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/gui_classes.py
+-rw-r--r--   0        0        0    33197 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/lif_reader.py
+-rw-r--r--   0        0        0     6027 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/patch_lifreader.py
+-rw-r--r--   0        0        0      282 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/resources.py
+-rw-r--r--   0        0        0    15449 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/sigmoid_widget.py
+-rw-r--r--   0        0        0     6583 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/stack_preview.py
+-rw-r--r--   0        0        0     3848 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/stack_selector.py
+-rw-r--r--   0        0        0     9342 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/stack_selector_crop.py
+-rw-r--r--   0        0        0     3096 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/stack_selector_leica.py
+-rw-r--r--   0        0        0    12078 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/stack_selector_tif.py
+-rw-r--r--   0        0        0     7192 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/gui_master.py
+-rw-r--r--   0        0        0    16079 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/material_fit/gui_fit.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/orientation/__init__.py
+-rw-r--r--   0        0        0    51650 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/orientation/gui_orientation.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/solver/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/solver/analyze/__init__.py
+-rw-r--r--   0        0        0    20577 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/solver/analyze/plot_window.py
+-rw-r--r--   0        0        0     1575 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/gui_solver.py
+-rw-r--r--   0        0        0    16165 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/BatchEvaluate.py
+-rw-r--r--   0        0        0    11795 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/DeformationDetector.py
+-rw-r--r--   0        0        0     4203 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/FittedMesh.py
+-rw-r--r--   0        0        0    11660 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/MeshCreator.py
+-rw-r--r--   0        0        0    10563 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/PipelineModule.py
+-rw-r--r--   0        0        0     1103 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/QTimeSlider.py
+-rw-r--r--   0        0        0    14384 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/Regularizer.py
+-rw-r--r--   0        0        0    11278 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/ResultView.py
+-rw-r--r--   0        0        0    20033 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/StackDisplay.py
+-rw-r--r--   0        0        0    12999 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/VTK_Toolbar.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/__init__.py
+-rw-r--r--   0        0        0      541 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/code_export.py
+-rw-r--r--   0        0        0     6645 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py
+-rw-r--r--   0        0        0    48390 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/Exporter.py
+-rw-r--r--   0        0        0    13704 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExporterRender2D.py
+-rw-r--r--   0        0        0    17357 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExporterRender3D.py
+-rw-r--r--   0        0        0    18697 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/FiberViewer.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/__init__.py
+-rw-r--r--   0        0        0    11681 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/load_measurement_dialog.py
+-rw-r--r--   0        0        0     3868 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/path_editor.py
+-rw-r--r--   0        0        0    12003 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/showVectorField.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/spheroid/__init__.py
+-rw-r--r--   0        0        0    93350 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/spheroid/gui_deformation_spheroid.py
+-rw-r--r--   0        0        0    53944 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/Icon.ico
+-rw-r--r--   0        0        0    42003 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/Logo.png
+-rw-r--r--   0        0        0    77561 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/Logo.svg
+-rw-r--r--   0        0        0    37691 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/Logo_black.png
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/arrowscale.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/autoscale0.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/autoscale1.ico
+-rw-r--r--   0        0        0    48947 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/buttons.svg
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/center0.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/center1.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/contrast0.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/contrast1.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/grid.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/grid2.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/grid3.ico
+-rw-r--r--   0        0        0    38885 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/logo_splash.png
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/nan0.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/nan1.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/show_image.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/show_image2.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/show_image3.ico
+-rw-r--r--   0        0        0     3606 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/slice0.ico
+-rw-r--r--   0        0        0     3606 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/slice1.ico
+-rw-r--r--   0        0        0     3606 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/slice2.ico
+-rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/slice_all.ico
+-rw-r--r--   0        0        0   121664 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/thumbnails/BFTFM.png
+-rw-r--r--   0        0        0   132449 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/thumbnails/BFTFM_2.png
+-rw-r--r--   0        0        0   180081 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/thumbnails/Bead_example_icon.png
+-rw-r--r--   0        0        0   202759 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/thumbnails/Dynamic_icon.png
+-rw-r--r--   0        0        0   554429 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/img/thumbnails/StainedOrganoid_icon.png
+-rw-r--r--   0        0        0   263760 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/img/thumbnails/liver_fibroblast_icon.png
+-rw-r--r--   0        0        0     3606 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/img/view_single.ico
+-rw-r--r--   0        0        0     3606 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/img/view_two.ico
+-rw-r--r--   0        0        0    12192 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/macro.py
+-rw-r--r--   0        0        0    12253 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/materials.py
+-rw-r--r--   0        0        0     3701 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/mesh.py
+-rw-r--r--   0        0        0     5635 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/multigrid_helper.py
+-rw-r--r--   0        0        0    22502 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/result_file.py
+-rw-r--r--   0        0        0     7754 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/saveable.py
+-rw-r--r--   0        0        0    46114 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/solver.py
+-rw-r--r--   0        0        0    11190 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/stack.py
+-rw-r--r--   0        0        0    17259 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/unused/macro.py
+-rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 saenopy-1.0.0/PKG-INFO
```

### Comparing `saenopy-0.9.0/LICENSE.txt` & `saenopy-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/README.md` & `saenopy-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,53 @@
 SAENOPY
 =======
 
 [![DOC](https://readthedocs.org/projects/saenopy/badge/)](https://saenopy.readthedocs.io)
+[![Coverage Status](https://coveralls.io/repos/github/rgerum/saenopy/badge.svg?branch=master)](https://coveralls.io/github/rgerum/saenopy?branch=master)
 [![PyTest](https://github.com/rgerum/saenopy/actions/workflows/test.yml/badge.svg)](https://github.com/rgerum/saenopy/actions/workflows/test.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 <p align="center">
   <img src="saenopy/img/Logo.png" />
 </p>
 
 
 SAENOPY is a free open source 3D traction force microscopy software. Its material model is especially well suited for
 tissue-mimicking and typically highly non-linear biopolymer matrices such as collagen, fibrin, or Matrigel. 
 
 It features a python package to use in scripts and an extensive graphical user interface.
 
-Check out our [Documentation](https://saenopy.readthedocs.io) on how to install and use it or our preprint:
+Check out our [Documentation](https://saenopy.readthedocs.io) on how to install and use it.
+
+## Installation
+
+### Standalone
+To use saenopy without a complicated installation you can use our standalone binaries to get started right away on Windows or Linux.
+
+Windows
+https://github.com/rgerum/saenopy/releases/download/v1.0.0/saenopy.exe
+
+Linux
+https://github.com/rgerum/saenopy/releases/download/v1.0.0/saenopy
+
+### Using Python
+
+If you are experienced with python or even want to use our Python API, you need to install saenopy as a python package.
+Saenopy can be installed directly using pip:
+
+    ``pip install saenopy``
+
+Now you can start the user interface with:
+
+    ``saenopy``
+
+## Getting started
+To get started you can have a look at our collection of [example datasets](https://saenopy.readthedocs.io/en/latest/auto_examples/index.html).
+
+## Preprint
+If you want to cite saenopy you can reference our preprint.
 
 *Dynamic traction force measurements of migrating immune cells in 3D matrices*
 David Böhringer, Mar Cóndor, Lars Bischof, Tina Czerwinski, Andreas Bauer, Caroline Voskens, Silvia Budday, 
 Christoph Mark, Ben Fabry, Richard Gerum
 **bioRxiv 2022.11.16.516758**; doi: https://doi.org/10.1101/2022.11.16.516758
```

### Comparing `saenopy-0.9.0/pyproject.toml` & `saenopy-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saenopy"
-version = "0.9.0"
+version = "1.0.0"
 description = "Semi-elastic fiber optimisation in python."
 authors = ["rgerum <14153051+rgerum@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "saenopy"}]
 
 
@@ -27,14 +27,15 @@
 sphinx-rtd-theme = { version = "^1.2.0", optional = true }
 nbsphinx = { version = "^0.8.10", optional = true }
 sphinx-gallery = {version = "^0.11.1", optional = true }
 appdirs = "^1.4.4"
 nptyping = "^2.4.1"
 qtrangeslider = "^0.1.5"
 h5py = "^3.8.0"
+pyfields = "^1.7.0"
 
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-rtd-theme", "nbsphinx", "sphinx-gallery"]
 
 
 [tool.poetry.scripts]
@@ -44,11 +45,12 @@
 [tool.poetry.group.dev.dependencies]
 pyinstaller = "^5.9.0"
 auto-py-to-exe = "^2.33.0"
 pytest = "^7.2.2"
 coverage = "^5.0.0"
 hypothesis = "^6.74.1"
 coveralls = "^3.3.1"
+findiff = "^0.9.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `saenopy-0.9.0/saenopy/buildBeams.py` & `saenopy-1.0.0/saenopy/build_beams.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,47 @@
-import numpy as np
-
-
-def MakeFromPolar(r: float, theta: float, phi: float) -> np.ndarray:
-    """
-    Convert from polar coordinates to cartesian coordinates
-    """
-    # get sine and cosine of the angles
-    ct = np.cos(theta)
-    st = np.sin(theta)
-    cp = np.cos(phi)
-    sp = np.sin(phi)
-    # and convert to cartesian coordinates
-    x = r * st * cp
-    y = r * st * sp
-    z = r * ct
-    # create the array
-    return np.array([x, y, z])
-
-
-def buildBeams(N: int) -> np.ndarray:
-    """
-    Builds a sphere of unit vectors with N beams in the xy plane.
-    """
-    N = int(np.floor(np.sqrt(int(N) * np.pi + 0.5)))
-
-    # start with an empty list
-    beams = []
-
-    # iterate over the whole angle in the xy plane
-    for i in range(N):
-        # get the Nth part of the total rotation
-        theta = (2 * np.pi / N) * i
-
-        # estimate how many vectors we need to cover the phi angle (for the z direction)
-        jmax = int(np.floor(N * np.sin(theta) + 0.5))
-
-        # iterate over those angles to get beams in every direction
-        for j in range(jmax):
-            # get the phi angle
-            phi = (2 * np.pi / jmax) * j
-
-            # and create a unit vector from the polar coordinates theta and phi
-            beams.append(MakeFromPolar(1.0, theta, phi))
-
-    # return all the vectors
-    return np.array(beams)
-
-
-def saveBeams(beams: np.ndarray, fname: str):
-    np.savetxt(fname, beams)
+import numpy as np
+
+
+def make_from_polar(r: float, theta: float, phi: float) -> np.ndarray:
+    """
+    Convert from polar coordinates to cartesian coordinates
+    """
+    # get sine and cosine of the angles
+    ct = np.cos(theta)
+    st = np.sin(theta)
+    cp = np.cos(phi)
+    sp = np.sin(phi)
+    # and convert to cartesian coordinates
+    x = r * st * cp
+    y = r * st * sp
+    z = r * ct
+    # create the array
+    return np.array([x, y, z])
+
+
+def build_beams(n: int) -> np.ndarray:
+    """
+    Builds a sphere of unit vectors with N beams in the xy plane.
+    """
+    n = int(np.floor(np.sqrt(int(n) * np.pi + 0.5)))
+
+    # start with an empty list
+    beams = []
+
+    # iterate over the whole angle in the xy plane
+    for i in range(n):
+        # get the Nth part of the total rotation
+        theta = (2 * np.pi / n) * i
+
+        # estimate how many vectors we need to cover the phi angle (for the z direction)
+        j_max = int(np.floor(n * np.sin(theta) + 0.5))
+
+        # iterate over those angles to get beams in every direction
+        for j in range(j_max):
+            # get the phi angle
+            phi = (2 * np.pi / j_max) * j
+
+            # and create a unit vector from the polar coordinates theta and phi
+            beams.append(make_from_polar(1.0, theta, phi))
+
+    # return all the vectors
+    return np.array(beams)
```

### Comparing `saenopy-0.9.0/saenopy/conjugateGradient.py` & `saenopy-1.0.0/saenopy/conjugate_gradient.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import numpy as np
-
-
-def cg(A: np.ndarray, b: np.ndarray, maxiter: int = 1000, tol: float = 0.00001, verbose: bool = False):
-    """ solve the equation Ax=b with the conjugate gradient method """
-    def norm(x):
-        return np.inner(x.flatten(), x.flatten())
-
-    # calculate the total force "amplitude"
-    normb = norm(b)
-
-    # if it is not 0 (always has to be positive)
-    if normb == 0:
-        return 0
-
-    x = np.zeros_like(b)
-
-    # the difference between the desired force deviations and the current force deviations
-    r = b - A @ x
-
-    # and store it also in pp
-    p = r
-
-    # calculate the total force deviation "amplitude"
-    resid = norm(p)
-
-    # iterate maxiter iterations
-    for i in range(1, maxiter + 1):
-        Ap = A @ p
-
-        alpha = resid / np.sum(p * Ap)
-
-        x = x + alpha * p
-        r = r - alpha * Ap
-
-        rsnew = norm(r)
-
-        # check if we are already below the convergence tolerance
-        if rsnew < tol * normb:
-            break
-
-        beta = rsnew / resid
-
-        # update pp and resid
-        p = r + beta * p
-        resid = rsnew
-
-        # print status every 100 frames
-        if i % 100 == 0 and verbose:
-            print(i, ":", resid, "alpha=", alpha, "du=", np.sum(x ** 2))  # , end="\r")
-
-    return x
+import numpy as np
+
+
+def cg(A: np.ndarray, b: np.ndarray, maxiter: int = 1000, tol: float = 0.00001, verbose: bool = False):
+    """ solve the equation Ax=b with the conjugate gradient method """
+    def norm(x):
+        return np.inner(x.flatten(), x.flatten())
+
+    # calculate the total force "amplitude"
+    normb = norm(b)
+
+    # if it is not 0 (always has to be positive)
+    if normb == 0:
+        return 0
+
+    x = np.zeros_like(b)
+
+    # the difference between the desired force deviations and the current force deviations
+    r = b - A @ x
+
+    # and store it also in pp
+    p = r
+
+    # calculate the total force deviation "amplitude"
+    resid = norm(p)
+
+    # iterate maxiter iterations
+    for i in range(1, maxiter + 1):
+        Ap = A @ p
+
+        alpha = resid / np.sum(p * Ap)
+
+        x = x + alpha * p
+        r = r - alpha * Ap
+
+        rsnew = norm(r)
+
+        # check if we are already below the convergence tolerance
+        if rsnew < tol * normb:
+            break
+
+        beta = rsnew / resid
+
+        # update pp and resid
+        p = r + beta * p
+        resid = rsnew
+
+        # print status every 100 frames
+        if i % 100 == 0 and verbose:
+            print(i, ":", resid, "alpha=", alpha, "du=", np.sum(x ** 2))  # , end="\r")
+
+    return x
```

### Comparing `saenopy-0.9.0/saenopy/examples.py` & `saenopy-1.0.0/saenopy/examples.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     speed = int(progress_size / (1024 * duration + 0.001))
     percent = int(count * block_size * 100 / total_size)
     sys.stdout.write("\r...%d%%, %d MB, %d KB/s, %d seconds passed" %
                     (percent, progress_size / (1024 * 1024), speed, duration))
     sys.stdout.flush()
 
 
-def downloadFiles(url, target_folder=None, progress_callback=None):
+def download_files(url, target_folder=None, progress_callback=None):
     file = Path(url).name
     target = Path(file)
     output_folder = Path(target.stem)
     if target_folder is not None:
         output_folder = Path(target_folder) / output_folder
     file_download_path = str(Path(output_folder).parent / file)
     if progress_callback is None:
@@ -39,75 +39,88 @@
         Path(output_folder).parent.mkdir(parents=True, exist_ok=True)
         urlretrieve(str(url), file_download_path, progress_callback)
         progress_callback(None, None, None, msg="unzipping...")
         shutil.unpack_archive(file_download_path, output_folder.parent)
         os.remove(file_download_path)
 
 
-def loadExample(name, target_folder=None, progress_callback=None):
+def load_example(name, target_folder=None, progress_callback=None, evaluated=False):
     if target_folder is None:
         target_folder = appdirs.user_data_dir("saenopy", "rgerum")
-    if name == "ClassicSingleCellTFM":
-        downloadFiles("https://github.com/rgerum/saenopy/releases/download/v0.7.4/1_ClassicSingleCellTFM.zip", target_folder, progress_callback=progress_callback)
-    if name == "DynamicalSingleCellTFM":
-        downloadFiles("https://github.com/rgerum/saenopy/releases/download/v0.7.4/2_DynamicalSingleCellTFM.zip", target_folder, progress_callback=progress_callback)
-    if name == "OrganoidTFM":
-        downloadFiles("https://github.com/rgerum/saenopy/releases/download/v0.7.4/4_OrganoidTFM.zip", target_folder, progress_callback=progress_callback)
-    if name == "BrightfieldTFM":
-        downloadFiles("https://github.com/rgerum/saenopy/releases/download/v0.7.4/6_BrightfieldNK92Data.zip", target_folder, progress_callback=progress_callback)
-    
+    example = get_examples()[name]
+    url = example["url"]
+    download_files(url, target_folder, progress_callback=progress_callback)
+
+    if evaluated:
+        evaluated_folder = Path(target_folder) / Path(Path(url).name).stem / "example_output"
+        if not (evaluated_folder / example["url_evaluated_file"][0]).exists():
+            download_files(example["url_evaluated"], evaluated_folder, progress_callback=progress_callback)
+        return [evaluated_folder / file for file in example["url_evaluated_file"]]
 
 
-def getExamples():
+def get_examples():
     example_path = Path(appdirs.user_data_dir("saenopy", "rgerum"))
     image_path = Path(resource_path("thumbnails"))
     return {
         "ClassicSingleCellTFM": {
             "desc": "Hepatic stellate cells in 1.2mg/ml collagen with relaxed and deformed stacks.\nRelaxed state induced with cytochalasin D.\n3 examples",
             "img": image_path / "liver_fibroblast_icon.png",
             "voxel_size": [0.7211, 0.7211, 0.988],
             "stack": example_path / '1_ClassicSingleCellTFM/Deformed/Mark_and_Find_001/Pos*_S001_z{z}_ch{c:00}.tif',
             "reference_stack": example_path / '1_ClassicSingleCellTFM/Relaxed/Mark_and_Find_001/Pos*_S001_z{z}_ch{c:00}.tif',
             "output_path": example_path / '1_ClassicSingleCellTFM/example_output',
-            "piv_parameter": {'win_um': 35.0, 'elementsize': 14.0, 'signoise_filter': 1.3, 'drift_correction': True},
-            "interpolate_parameter": {'reference_stack': 'first', 'element_size': 14.0, 'inner_region': 200.0, 'thinning_factor': 0, 'mesh_size_same': True, 'mesh_size_x': 200.0, 'mesh_size_y': 200.0, 'mesh_size_z': 200.0},
-            "solve_parameter": {'k': 6062.0, 'd0': 0.0025, 'lambda_s': 0.0804, 'ds':  0.034, 'alpha': 10**10, 'stepper': 0.33, 'i_max': 400, 'rel_conv_crit': 0.009},
+            "piv_parameters": {'window_size': 35.0, 'element_size': 14.0, 'signal_to_noise': 1.3, 'drift_correction': True},
+            "mesh_parameters": {'reference_stack': 'first', 'element_size': 14.0, 'mesh_size': 'piv'},
+            "material_parameters": {'k': 6062.0, 'd_0': 0.0025, 'lambda_s': 0.0804, 'd_s':  0.034},
+            "solve_parameters": {'alpha': 10**10, 'step_size': 0.33, 'max_iterations': 400, 'rel_conv_crit': 0.009},
+            "url": "https://github.com/rgerum/saenopy/releases/download/v0.7.4/1_ClassicSingleCellTFM.zip",
+            "url_evaluated": "https://github.com/rgerum/saenopy/releases/download/v0.7.4/1_ClassicSingleCellTFM_evaluated.zip",
+            "url_evaluated_file": ["Pos004_S001_z{z}_ch{c00}.saenopy", "Pos007_S001_z{z}_ch{c00}.saenopy", "Pos008_S001_z{z}_ch{c00}.saenopy"],
         },
         "DynamicalSingleCellTFM": {
             "desc": "Single natural killer cell that migrated through 1.2mg/ml collagen, recorded for 24min.\n1 example",
             "img": image_path / "Dynamic_icon.png",
             "voxel_size": [0.2407, 0.2407, 1.0071],
             "time_delta": 60,
             "stack": example_path / '2_DynamicalSingleCellTFM/data/Pos*_S001_t{t}_z{z}_ch{c:00}.tif',
             "output_path": example_path / '2_DynamicalSingleCellTFM/example_output',
-            "piv_parameter": {'win_um': 12.0, 'elementsize': 4.0, 'signoise_filter': 1.3, 'drift_correction': True},
-            "interpolate_parameter": {'reference_stack': 'median', 'element_size': 4.0, 'inner_region': 100.0, 'thinning_factor': 0, 'mesh_size_same': True, 'mesh_size_x': 200.0, 'mesh_size_y': 200.0, 'mesh_size_z': 200.0},
-            "solve_parameter": {'k': 1449.0, 'd0': 0.0022, 'lambda_s': 0.032, 'ds': 0.055, 'alpha':  10**10, 'stepper': 0.33, 'i_max': 100},
+            "piv_parameters": {'window_size': 12.0, 'element_size': 4.0, 'signal_to_noise': 1.3, 'drift_correction': True},
+            "mesh_parameters": {'reference_stack': 'median', 'element_size': 4.0, 'mesh_size': 'piv'},
+            "material_parameters": {'k': 1449.0, 'd_0': 0.0022, 'lambda_s': 0.032, 'd_s': 0.055},
+            "solve_parameters": {'alpha': 10**10, 'step_size': 0.33, 'max_iterations': 100},
             "crop": {"z": (20, -20)},
+            "url": "https://github.com/rgerum/saenopy/releases/download/v0.7.4/2_DynamicalSingleCellTFM.zip",
+            "url_evaluated": "https://github.com/rgerum/saenopy/releases/download/v0.7.4/2_DynamicalSingleCellTFM_evaluated.zip",
+            "url_evaluated_file": ["Pos002_S001_t{t}_z{z}_ch{c00}.saenopy"],
         },
         "OrganoidTFM": {
             "desc": "Intestinal organoid in 1.2mg/ml collagen",
             "img": image_path / "StainedOrganoid_icon.png",
             "voxel_size": [1.444, 1.444, 1.976],
             "stack": example_path / '4_OrganoidTFM/Pos007_S001_t50_z{z}_ch00.tif',
             "reference_stack": example_path / '4_OrganoidTFM/Pos007_S001_t6_z{z}_ch00.tif',
             "output_path": example_path / '4_OrganoidTFM/example_output',
-            "piv_parameter": {'win_um': 40.0, 'elementsize': 30.0, 'signoise_filter': 1.3, 'drift_correction': True},
-            "interpolate_parameter": {'reference_stack': 'first', 'element_size': 30, 'inner_region': 100.0, 'thinning_factor': 0, 'mesh_size_same': False, 'mesh_size_x': 738.0, 'mesh_size_y': 738.0, 'mesh_size_z': 738.0},
-            "solve_parameter": {'k': 6062.0, 'd0': 0.0025, 'lambda_s': 0.0804, 'ds':  0.034, 'alpha':  10**10, 'stepper': 0.33, 'i_max': 1400,  'rel_conv_crit': 1e-7},
-    },
+            "piv_parameters": {'window_size': 40.0, 'element_size': 30.0, 'signal_to_noise': 1.3, 'drift_correction': True},
+            "mesh_parameters": {'reference_stack': 'first', 'element_size': 30, 'mesh_size': (738.0, 738.0, 738.0)},
+            "material_parameters": {'k': 6062.0, 'd_0': 0.0025, 'lambda_s': 0.0804, 'd_s': 0.034},
+            "solve_parameters": {'alpha':  10**10, 'step_size': 0.33, 'max_iterations': 1400,  'rel_conv_crit': 1e-7},
+            "url": "https://github.com/rgerum/saenopy/releases/download/v0.7.4/4_OrganoidTFM.zip",
+            "url_evaluated": "https://github.com/rgerum/saenopy/releases/download/v0.7.4/4_OrganoidTFM_evaluated.zip",
+            "url_evaluated_file": ["Pos007_S001_t50_z{z}_ch00.saenopy"],
+        },
         "BrightfieldTFM": {
             "desc": "Traction forces around an immune cell in collagen 1.2mg/ml calculated on simple brightfield images",
             "img": image_path / "BFTFM_2.png",
             "voxel_size": [0.15, 0.15, 2.0],
             "crop": {'x': (1590, 2390), 'y': (878, 1678), 'z': (30, 90)},
-            "stack": example_path / 'BrightfieldNK92Data/2023_02_14_12_0920_stack.tif[z]',
-            "reference_stack": example_path / 'BrightfieldNK92Data/2023_02_14_12_0850_stack.tif[z]',
-            "output_path": example_path / 'BrightfieldNK92Data/example_output',
-            "piv_parameter": {'win_um': 12.0, 'elementsize': 4.8, 'signoise_filter': 1.3, 'drift_correction': True},
-            "interpolate_parameter": {'reference_stack': 'next', 'element_size': 4.0, 'mesh_size_same': True, 'mesh_size_x': 200.0, 'mesh_size_y': 200.0, 'mesh_size_z': 200.0},
-            "solve_parameter": {'k': 6062.0, 'd0': 0.0025, 'lambda_s': 0.0804, 'ds':  0.034, 'alpha':  10**11, 'stepper': 0.33, 'i_max': 300, 'rel_conv_crit': 0.01},
-
+            "stack": example_path / '6_BrightfieldNK92Data/2023_02_14_12_0920_stack.tif[z]',
+            "reference_stack": example_path / '6_BrightfieldNK92Data/2023_02_14_12_0850_stack.tif[z]',
+            "output_path": example_path / '6_BrightfieldNK92Data/example_output',
+            "piv_parameters": {'window_size': 12.0, 'element_size': 4.8, 'signal_to_noise': 1.3, 'drift_correction': True},
+            "mesh_parameters": {'reference_stack': 'next', 'element_size': 4.0, 'mesh_size': 'piv'},
+            "material_parameters": {'k': 6062.0, 'd_0': 0.0025, 'lambda_s': 0.0804, 'ds':  0.034},
+            "solve_parameters": {'alpha': 10**11, 'step_size': 0.33, 'max_iterations': 300, 'rel_conv_crit': 0.01},
+            "url": "https://github.com/rgerum/saenopy/releases/download/v0.7.4/6_BrightfieldNK92Data.zip",
+            "url_evaluated": "https://github.com/rgerum/saenopy/releases/download/v0.7.4/6_BrightfieldNK92Data_evaluated.zip",
+            "url_evaluated_file": ["2023_02_14_12_0920_stack.saenopy"],
         },
-    
-
     }
```

### Comparing `saenopy-0.9.0/saenopy/getDeformations.py` & `saenopy-1.0.0/saenopy/get_deformations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,80 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Oct 15 11:41:50 2020
-
-@author: david
-"""
-
 import numpy as np
 from openpiv.pyprocess3D import extended_search_area_piv3D
 from scipy import interpolate
 
+from nptyping import NDArray, Shape, Float
+from pyfields import field
+
+from saenopy.mesh import Mesh, check_node_vector_field
+from saenopy.stack import Stack
+from saenopy.multigrid_helper import create_box_mesh
+
+
+class PivMesh(Mesh):
+    __save_parameters__ = ["nodes", "tetrahedra", "displacements_measured"]
+
+    displacements_measured: NDArray[Shape["N_c, 3"], Float] = field(doc="the measured displacements of each node, dimensions: N_c x 3",
+                                                                    validators=check_node_vector_field, default=None)
 
-def get_displacements_from_stacks(stack_relaxed, stack_deformed, win_um, elementsize, signoise_filter, drift_correction):
-    fac_overlap = 1 - (elementsize/win_um)
+
+def get_displacements_from_stacks(stack_relaxed: Stack, stack_deformed: Stack, window_size: float,
+                                  element_size: float, signal_to_noise: float, drift_correction: bool) -> PivMesh:
+    fac_overlap = 1 - (element_size/window_size)
     voxel_size1 = stack_deformed.voxel_size
     voxel_size2 = stack_relaxed.voxel_size
 
-    np.testing.assert_equal(voxel_size1, voxel_size2, f"The two stacks do not have the same voxel size. {voxel_size1}, {voxel_size2}")
+    np.testing.assert_equal(voxel_size1, voxel_size2,
+                            f"The two stacks do not have the same voxel size. {voxel_size1}, {voxel_size2}")
 
-    np.testing.assert_equal(stack_deformed.shape, stack_relaxed.shape, f"The two stacks do not have the same voxel count. {stack_deformed.shape}, {stack_relaxed.shape}")
+    np.testing.assert_equal(stack_deformed.shape, stack_relaxed.shape,
+                            f"The two stacks do not have the same voxel count. {stack_deformed.shape}, {stack_relaxed.shape}")
 
     # mean over the rgb channels
     stack_deformed = np.mean(np.array(stack_deformed), axis=2)
     stack_relaxed = np.mean(np.array(stack_relaxed), axis=2)
-    M = getDisplacementsFromStacks_old(stack_deformed, stack_relaxed, voxel_size1,
-                                        win_um=win_um,
-                                        fac_overlap=fac_overlap,
-                                        signoise_filter=signoise_filter,
-                                        drift_correction=drift_correction,
-                                        return_mesh=True)
+    piv_mesh = _get_displacements_from_stacks_old(stack_deformed, stack_relaxed, voxel_size1,
+                                                  window_size=window_size,
+                                                  fac_overlap=fac_overlap,
+                                                  signal_to_noise=signal_to_noise,
+                                                  drift_correction=drift_correction,
+                                                  )
     # center
-    M.R = (M.R - np.min(M.R, axis=0)) - (np.max(M.R, axis=0) - np.min(M.R, axis=0)) / 2
-    return M
+    piv_mesh.nodes = (piv_mesh.nodes - np.min(piv_mesh.nodes, axis=0)) - (np.max(piv_mesh.nodes, axis=0) - np.min(piv_mesh.nodes, axis=0)) / 2
+    return piv_mesh
 
 
-def sig2noise_filtering( u, v, sig2noise, w=None, threshold = 1.3):
+def sig2noise_filtering(u, v, sig2noise, w=None, threshold=1.3):
     """
-    As integrted into OpenPiv Jun 19, 2020.
-    Since OpenPIV changed this function lateron, we use this version
-    to replace outliers with np.nan dependend on the signal2noise ratio here
+    As integrated into OpenPiv Jun 19, 2020.
+    Since OpenPIV changed this function later on, we use this version
+    to replace outliers with np.nan depending on the signal-to-noise ratio
     """
 
     ind = sig2noise < threshold
 
     u[ind] = np.nan
     v[ind] = np.nan
-    if isinstance(w, np.ndarray):
-        w[ind] = np.nan
-        return u, v, w, ind
-
-    return u, v, ind
+    w[ind] = np.nan
+    return u, v, w, ind
 
 
-def replace_outliers( u, v, w=None, method='localmean', max_iter=5, tol=1e-3, kernel_size=1):
+def replace_outliers(u, v, w=None, method='localmean', max_iter=5, tol=1e-3, kernel_size=1):
     """
-    As integrted into OpenPiv Jun 19, 2020.
-    Since OpenPIV changed several functions lateron, we use this version
-    to replace outliers with np.nan dependend on the signal2noise ratio here
+    As integrated into OpenPiv Jun 19, 2020.
+    Since OpenPIV changed several functions later on, we use this version
+    to replace outliers with np.nan depending on the signal-to-noise ratio
 
-    Replace invalid vectors in an velocity field using an iterative image inpainting algorithm.
+    Replace invalid vectors in a velocity field using an iterative image inpainting algorithm.
 
     The algorithm is the following:
 
     1) For each element in the arrays of the ``u`` and ``v`` components, replace it by a weighted average
-       of the neighbouring elements which are not invalid themselves. The weights depends
-       of the method type. If ``method=localmean`` weight are equal to 1/( (2*kernel_size+1)**2 -1 )
+       of the neighbouring elements which are not invalid themselves. The weights depend
+       on the method type. If ``method=localmean`` weight are equal to 1/( (2*kernel_size+1)**2 -1 )
 
     2) Several iterations are needed if there are adjacent invalid elements.
        If this is the case, inforation is "spread" from the edges of the missing
        regions iteratively, until the variation is below a certain threshold.
 
     Parameters
     ----------
@@ -100,23 +107,24 @@
         the smoothed w velocity component field, where invalid vectors have been replaced
 
     """
     uf = replace_nans_py(u, method=method, max_iter=max_iter, tol=tol, kernel_size=kernel_size)
     vf = replace_nans_py(v, method=method, max_iter=max_iter, tol=tol, kernel_size=kernel_size)
 
     if isinstance(w, np.ndarray):
-        wf =  replace_nans_py(w, method=method, max_iter=max_iter, tol=tol, kernel_size=kernel_size)
+        wf = replace_nans_py(w, method=method, max_iter=max_iter, tol=tol, kernel_size=kernel_size)
         return uf, vf, wf
 
     return uf, vf
 
-def get_dist(kernel,kernel_size):
+
+def get_dist(kernel, kernel_size):
     """
-    As integrted into OpenPiv Jun 19, 2020.
-    Since OpenPIV changed several functions lateron, we use this version
+    As integrated into OpenPiv Jun 19, 2020.
+    Since OpenPIV changed several functions later on, we use this version
     """
     # generates a map of distances to the center of the kernel. This is later used to generate disk-shaped kernels and
     # fill in distance based weights
 
     if len(kernel.shape) == 2:
         # x and y coordinates for each points
         xs, ys = np.indices(kernel.shape)
@@ -130,17 +138,17 @@
         dist_inv = np.sqrt(3) * kernel_size - dist
 
     return dist, dist_inv
 
 
 def replace_nans_py(array, max_iter, tol, kernel_size = 2, method = 'disk'):
     """
-    As integrted into OpenPiv Jun 19, 2020.
-    Since OpenPIV changed several functions lateron, we use this version
-    to replace outliers with np.nan dependend on the signal2noise ratio here
+    As integrated into OpenPiv Jun 19, 2020.
+    Since OpenPIV changed several functions later on, we use this version
+    to replace outliers with np.nan depend ing on the signal2noise ratio
 
 
     Replace NaN elements in an array using an iterative image inpainting algorithm.
       The algorithm is the following:
       1) For each element in the input array, replace it by a weighted average
          of the neighbouring elements which are not NaN themselves. The weights
          depend on the method type. See Methods below.
@@ -223,63 +231,60 @@
     # make several passes
     # until we reach convergence
     for it in range(max_iter):
         # note: identifying new nan indices and looping other the new indices would give slightly different result
 
         # for each NaN element
         for k in range(n_nans):
-            ind = nan_indices[k] #2 or 3 indices indicating the position of a nan element
+            ind = nan_indices[k]  # 2 or 3 indices indicating the position of a nan element
             # init to 0.0
             replaced_new[k] = 0.0
             n = 0.0
 
             # generating a list of indices of the convolution window in the array
-            slice_indices = np.array(np.meshgrid(*[range(i-kernel_size,i+kernel_size+1) for i in ind]))
-            slice_indices = np.reshape(slice_indices,( n_dim, (2 * kernel_size + 1) ** n_dim), order="C").T
+            slice_indices = np.array(np.meshgrid(*[range(i-kernel_size, i+kernel_size+1) for i in ind]))
+            slice_indices = np.reshape(slice_indices, (n_dim, (2 * kernel_size + 1) ** n_dim), order="C").T
 
             # loop over the kernel
             for s_index, k_index in zip(slice_indices, kernel_indices):
-                s_index = tuple(s_index) # this is necessary for numpy array indexing
+                s_index = tuple(s_index)  # this is necessary for numpy array indexing
                 k_index = tuple(k_index)
 
-                # skip if we are outside of array boundaries, if the array element is nan or if the kernel element is zero
-                if all([s >= 0 and s < bound for s, bound  in zip(s_index, filled.shape)]):
+                # skip if we are outside of array boundaries, if the array element is nan or
+                # if the kernel element is zero
+                if all([s >= 0 and s < bound for s, bound in zip(s_index, filled.shape)]):
                     if not np.isnan(filled[s_index]) and kernel[k_index] != 0:
-                    # convolve kernel with original array
+                        # convolve kernel with original array
                         replaced_new[k] = replaced_new[k] + filled[s_index] * kernel[k_index]
                         n = n + kernel[k_index]
 
-                    # divide value by effective number of added elements
+            # divide value by effective number of added elements
             if n > 0:
                 replaced_new[k] = replaced_new[k] / n
             else:
                 replaced_new[k] = np.nan
 
         # bulk replace all new values in array
         for k in range(n_nans):
             filled[tuple(nan_indices[k])] = replaced_new[k]
 
-        # elements is below a certain tolerance
-        if np.mean((replaced_new - replaced_old) ** 2) < tol:
+        # elements are below a certain tolerance
+        if len(replaced_new) and np.mean((replaced_new - replaced_old) ** 2) < tol:
             break
         else:
-                replaced_old = replaced_new
+            replaced_old = replaced_new
     return filled
 
 
 # Full 3D Deformation analysis
-def getDisplacementsFromStacks_old(stack_deformed, stack_relaxed, voxel_size, win_um=12, fac_overlap=0.6,
-                               signoise_filter=1.3, drift_correction=True, return_mesh=False):
-    from saenopy.multigridHelper import createBoxMesh
-    from saenopy import Solver
-
-    # set properties
+def _get_displacements_from_stacks_old(stack_deformed, stack_relaxed, voxel_size, window_size=12, fac_overlap=0.6,
+                                       signal_to_noise=1.3, drift_correction=True):    # set properties
     voxel_size = np.array(voxel_size)
-    window_size = (win_um / voxel_size).astype(int)
-    overlap = ((fac_overlap * win_um) / voxel_size).astype(int)
+    window_size = (window_size / voxel_size).astype(int)
+    overlap = (fac_overlap * window_size).astype(int)
     du, dv, dw = voxel_size
     print("Calculate Deformations", stack_relaxed.shape, window_size, overlap)
 
     # calculate deformations
     u, v, w, sig2noise = extended_search_area_piv3D(stack_relaxed, stack_deformed,
                                                     window_size=window_size,
                                                     overlap=overlap,
@@ -293,70 +298,48 @@
     # correcting stage drift between the field of views
     if drift_correction:
         u -= np.nanmean(u)
         v -= np.nanmean(v)
         w -= np.nanmean(w)
 
     # filter deformations
-    uf, vf, wf, mask = sig2noise_filtering(u, v,sig2noise, w=w, threshold=signoise_filter)
+    uf, vf, wf, mask = sig2noise_filtering(u, v, sig2noise, w=w, threshold=signal_to_noise)
     uf, vf, wf = replace_outliers(uf, vf, wf, max_iter=1, tol=100, kernel_size=2, method='disk')
 
     # get coordinates (by multiplication with the ratio of image dimension and deformation grid)
     y, x, z = np.indices(u.shape)
     y, x, z = (y * stack_deformed.shape[0] * dv / u.shape[0],
                x * stack_deformed.shape[1] * du / u.shape[1],
                z * stack_deformed.shape[2] * dw / u.shape[2])
 
     # create a box mesh - convert to meters for saenopy conversion
-    R, T = createBoxMesh(np.unique(y.ravel()) * 1e-6,  # saeno x
-                         np.unique(x.ravel()) * 1e-6,  # saeno y
-                         np.unique(z.ravel()) * 1e-6)  # saeno z
+    R, T = create_box_mesh(np.unique(y.ravel()) * 1e-6,  # saeno x
+                           np.unique(x.ravel()) * 1e-6,  # saeno y
+                           np.unique(z.ravel()) * 1e-6)  # saeno z
 
     # bring deformations in right order (switch from OpenPIV conversion ot saenopy conversion)
     # - convert to meters for saenopy conversion
     U = np.vstack([v.ravel() * 1e-6, -u.ravel() * 1e-6, w.ravel() * 1e-6]).T
 
-    if return_mesh is True:
-        from saenopy.solver import Mesh
-        M = Mesh(R, T)
-        M.setNodeVar("U_measured", U)
-        return M
-    M = Solver()
-    # provide the node data
-    M.setNodes(R)
-    # and the tetrahedron data
-    M.setTetrahedra(T)
-    # set the deformations
-    M.setTargetDisplacements(U)
-    return M
-
-
-def center_field(U, R):
-    # find center of deformation field analog to force field in Saeno/Saenopy for deformation field
-    # U = U[~np.isnan(U)]
-    # R = R[~np.isnan(R)]
-    Usum = np.sum(U, axis=0)
-    B1 = np.einsum("kj,ki->j", R, U ** 2)
-    B2 = np.einsum("kj,ki,ki->j", U, R, U)
-    A = np.sum(np.einsum("ij,kl,kl->kij", np.eye(3), U, U) - np.einsum("ki,kj->kij", U, U), axis=0)
-    B = B1 - B2
-    center = np.linalg.inv(A) @ B
-    return center
+    from saenopy.mesh import Mesh
+    mesh = PivMesh(R, T)
+    mesh.displacements_measured = U
+    return mesh
 
 
 def interpolate_different_mesh(R, U, Rnew):
     """
     Interpolate Deformations (or any quantity) from one mesh to another.
     
-    Nonoverlapping regimes between meshes are filled with nans - linear interpolation.
+    Non overlapping regimes between meshes are filled with nans - linear interpolation.
 
     Parameters
     ----------
-    R : Old coordinates (saenopy format: M.R)
-    U : Old deformations (saenopy format: M.U)
+    R : Old coordinates (saenopy format: M.mesh.R)
+    U : Old deformations (saenopy format: M.mesh.U)
     Rnew: New coordinates
 
     Returns
     -------
     Unew : New interpolated deformations 
 
     """
```

### Comparing `saenopy-0.9.0/saenopy/gui/code/code_editor.py` & `saenopy-1.0.0/saenopy/gui/code/code_editor.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/code/gui_code.py` & `saenopy-1.0.0/saenopy/gui/code/gui_code.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/code/script_file.py` & `saenopy-1.0.0/saenopy/gui/code/script_file.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/code/syntax.py` & `saenopy-1.0.0/saenopy/gui/code/syntax.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/common/QExtendedGraphicsView.py` & `saenopy-1.0.0/saenopy/gui/common/QExtendedGraphicsView.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/common/QtShortCuts.py` & `saenopy-1.0.0/saenopy/gui/common/QtShortCuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,24 +287,25 @@
     def value(self):
         return self.spin_box.value()
 
 
 class QInputString(QInput):
     error = None
 
-    def __init__(self, layout=None, name=None, value="", allow_none=True, type=str, unit=None, name_post=None, validator=None, **kwargs):
+    def __init__(self, layout=None, name=None, value="", allow_none=True, none_value="None", type=str, unit=None, name_post=None, validator=None, **kwargs):
         # initialize the super widget
         QInput.__init__(self, layout, name, **kwargs)
+        self.none_value = none_value
 
         if self.settings is not None:
             value = self.settings.value(self.settings_key, value)
 
         self.line_edit = QtWidgets.QLineEdit()
         self.layout().addWidget(self.line_edit)
-        self.line_edit.editingFinished.connect(lambda: self._valueChangedEvent(self.value()))
+        self.line_edit.editingFinished.connect(self.editingFinishedCall)
         if type is int or type is float or type == "exp":
             self.line_edit.setAlignment(QtCore.Qt.AlignRight)
         if unit is not None:
             self.label_unit = QtWidgets.QLabel(unit)
             self.layout().addWidget(self.label_unit)
 
         self.allow_none = allow_none
@@ -316,14 +317,20 @@
             self.layout().addWidget(self.label2)
 
         self.setValue(value)
         self.emitValueChanged()
 
         self.line_edit.textChanged.connect(self.emitValueChanged)
 
+    def editingFinishedCall(self):
+        try:
+            self._valueChangedEvent(self.value())
+        except ValueError:
+            return
+
     def emitValueChanged(self):
         """ connected to the textChanged signal """
         try:
             value = self.value()
             if self.validator is not None:
                 if self.validator(value) is False:
                     raise ValueError
@@ -336,15 +343,15 @@
             self.line_edit.setText(f"10**{np.format_float_positional(np.log10(float(value)), precision=2, unique=True, fractional=True, trim='-')}")
         else:
             self.line_edit.setText(str(value))
 
     def value(self):
         text = self.line_edit.text()
         if self.allow_none is True and (text == "None" or text == ""):
-            return "None"
+            return self.none_value
         if self.type == int:
             return int(text)
         if self.type == float:
             return float(text)
         if self.type == "exp":
             if text.startswith("1e"):
                 return 10**float(text[2:])
```

### Comparing `saenopy-0.9.0/saenopy/gui/common/gui_classes.py` & `saenopy-1.0.0/saenopy/gui/common/gui_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,19 +382,19 @@
                 menu.exec_(self.viewport().mapToGlobal(position))
 
     def change_color(self):
         import matplotlib as mpl
         index = self.currentRow()
 
         # get new color from color picker
-        color = QtWidgets.QColorDialog.getColor(QtGui.QColor(*mpl.colors.to_rgb(self.data[index][3])))
+        color = QtWidgets.QColorDialog.getColor(QtGui.QColor(*[int(i) for i in mpl.colors.to_rgb(self.data[index][3])]))\
         # if a color is set, apply it
         if color.isValid():
             self.data[index][3] = "#%02x%02x%02x" % color.getRgb()[:3]
-            self.item(index).setIcon(qta.icon("fa5.circle", options=[dict(color=color)]))
+            self.item(index).setIcon(qta.icon("fa5s.circle", options=[dict(color=color)]))
 
     def delete_item(self):
         index = self.currentRow()
         self.data.pop(index)
         self.takeItem(index)
         self.setCurrentRow(index)
 
@@ -432,15 +432,15 @@
         self.addAddItem()
         self.no_list_change = False
         return item
 
     def customAddItem(self, d, checked, color):
         item = QtWidgets.QListWidgetItem(d, self)
         if color is not None:
-            item.setIcon(qta.icon("fa5.circle", options=[dict(color=color)]))
+            item.setIcon(qta.icon("fa5s.circle", options=[dict(color=color)]))
         item.setFlags(self.flags)
         item.setCheckState(QtCore.Qt.Checked if checked else QtCore.Qt.Unchecked)
         return item
 
 
 from multiprocessing import Process, Queue
```

### Comparing `saenopy-0.9.0/saenopy/gui/common/lif_reader.py` & `saenopy-1.0.0/saenopy/gui/common/lif_reader.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/common/patch_lifreader.py` & `saenopy-1.0.0/saenopy/gui/common/patch_lifreader.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/common/sigmoid_widget.py` & `saenopy-1.0.0/saenopy/gui/common/sigmoid_widget.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/common/stack_preview.py` & `saenopy-1.0.0/saenopy/gui/common/stack_preview.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/common/stack_selector.py` & `saenopy-1.0.0/saenopy/gui/common/stack_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 
     def setImage(self, im):
         self.im = im
         self.pixmap.setPixmap(QtGui.QPixmap(array2qimage(im)))
         self.view.setExtend(im.shape[1], im.shape[0])
 
     def file_changed(self, filename):
-        print("file_changed", filename)
         for selector_instance in self.selectors:
             selector_instance.setVisible(False)
 
         for selector_instance in self.selectors:
             if selector_instance.checkAcceptFilename(filename):
                 self.active = selector_instance
                 selector_instance.setImage(filename)
```

### Comparing `saenopy-0.9.0/saenopy/gui/common/stack_selector_crop.py` & `saenopy-1.0.0/saenopy/gui/common/stack_selector_crop.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/common/stack_selector_leica.py` & `saenopy-1.0.0/saenopy/gui/common/stack_selector_leica.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/common/stack_selector_tif.py` & `saenopy-1.0.0/saenopy/gui/common/stack_selector_tif.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 from pathlib import Path
 import imageio
 import tifffile
 from qtpy import QtWidgets
 from saenopy.gui.common import QtShortCuts
 import appdirs
-from saenopy.stack import readTiff
+from saenopy.stack import read_tiff
 from typing import List
 
 
 voxel_size_file = Path(appdirs.user_data_dir("saenopy", "rgerum")) / 'voxel_sizes.txt'
 time_delta_file = Path(appdirs.user_data_dir("saenopy", "rgerum")) / 'time_deltas.txt'
 
 
@@ -152,23 +152,24 @@
 
         selected_prop = filename_to_prop_dict(regexpr, filename)
 
         properties = []
         for file in filenames:
             prop = filename_to_prop_dict(regexpr, file)
             if file.suffix in [".tif", ".tiff"]:
-                tif = tifffile.TiffReader(file)
-                if len(tif.pages) > 1:
-                    selected_prop["tiff pages"] = 0
+                with tifffile.TiffReader(file) as tif:
+                    if len(tif.pages) > 1:
+                        selected_prop["tiff pages"] = 0
             prop["filename"] = file
             if file.suffix in [".tif", ".tiff"]:
-                for page in range(0, len(tif.pages)):
-                    prop["tiff pages"] = page
-                    prop["filename"] = str(file)+f"[{page}]"
-                    properties.append(prop.copy())
+                with tifffile.TiffReader(file) as tif:
+                    for page in range(0, len(tif.pages)):
+                        prop["tiff pages"] = page
+                        prop["filename"] = str(file)+f"[{page}]"
+                        properties.append(prop.copy())
             else:
                 properties.append(prop.copy())
         df = pd.DataFrame(properties)
 
         self.format_template = self.format_template.replace("{", "{{{{").replace("}", "}}}}")
 
         for key, value in selected_prop.items():
@@ -249,37 +250,36 @@
             else:
                 selected_props_dict[prop.name] = str(prop.value())
 
         self.stack_obj = []
         from saenopy.stack import Stack
         if not self.use_time or t_prop_name == "None":
             d = d.sort_values(z_prop_name)
-            self.stack_obj = [Stack()]
+            self.stack_obj = [Stack("", (1, 1, 1), {}, image_filenames=[[str(f)] for f in d.filename])]
             self.stack_obj[0].image_filenames = [[str(f)] for f in d.filename]
         else:
             d = d.sort_values([t_prop_name, z_prop_name])
             self.stack_obj = []
             for t, dd in d.groupby(t_prop_name):
-                s = Stack()
-                s.image_filenames = [[str(f)] for f in dd.filename]
+                s = Stack("", (1, 1, 1), {}, image_filenames=[[str(f)] for f in dd.filename])
                 self.stack_obj.append(s)
 
         self.target_glob = self.format_template.format(**selected_props_dict)
         if z_prop_name == "tiff pages":
             self.target_glob += "[z]"
         elif z_prop_name == "tiff pages":
             self.target_glob += "[t]"
         elif ("tiff pages" in selected_props_dict) and (selected_props_dict["tiff pages"] != 0):
             self.target_glob += f'[{selected_props_dict["tiff pages"]}]'
         self.parent_selector.stack_changed.emit()
         self.parent_selector.glob_string_changed.emit('getstack', self.target_glob)
 
         #self.parent_selector.setZCount(len(d))
         self.d = d
-        im = readTiff(d.iloc[0].filename)
+        im = read_tiff(d.iloc[0].filename)
         if len(im.shape) == 3:
             im = im[:, :, 0]
         self.stack = np.zeros((im.shape[0], im.shape[1], len(d)), dtype=im.dtype)
         self.stack_initialized = np.zeros(len(d), dtype=bool)
         self.stack_initialized[0] = True
         self.stack[:, :, 0] = im
 
@@ -294,15 +294,15 @@
             index = [index]
 
         for i in index:
             if self.stack_initialized is not None and self.stack_initialized[i] == False:
                 if str(self.d.iloc[i].filename).endswith(".tif"):
                     im = tifffile.imread(str(self.d.iloc[i].filename))
                 else:
-                    im = imageio.imread(str(self.d.iloc[i].filename))
+                    im = imageio.v2.imread(str(self.d.iloc[i].filename))
                 if len(im.shape) == 3:
                     im = im[:, :, 0]
                 self.stack[:, :, i] = im
                 self.stack_initialized[i] = True
 
     def showImage(self):
         if self.no_update is True or self.stack is None:
```

### Comparing `saenopy-0.9.0/saenopy/gui/gui_master.py` & `saenopy-1.0.0/saenopy/gui/gui_master.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import sys
+import traceback
+
 from qtpy import QtCore, QtWidgets, QtGui
 import multiprocessing
 # keep import for pyinstaller
 import skimage.filters.ridges
 import skimage.filters.thresholding
 
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.solver.gui_solver import MainWindowSolver as SolverMain
 from saenopy.gui.spheroid.gui_deformation_spheroid import MainWindow as SpheroidMain
 from saenopy.gui.orientation.gui_orientation import MainWindow as OrientationMain
 from saenopy.gui.code.gui_code import MainWindowCode
+from saenopy.gui.material_fit.gui_fit import MainWindowFit
 from saenopy.gui.common.resources import resource_path, resource_icon
 
 
 class InfoBox(QtWidgets.QWidget):
     def __init__(self, name, func):
         super().__init__()
         self.setMinimumWidth(200)
@@ -56,21 +59,25 @@
                         self.image.setPixmap(QtGui.QPixmap(resource_path("Logo.png")))
                         self.image.setScaledContents(True)
                         self.image.setMaximumWidth(400)
                         self.image.setMaximumHeight(200)
                         layout.addStretch()
                     with QtShortCuts.QHBoxLayout() as layout2:
                         layout2.addStretch()
-                        InfoBox("Solver", lambda: self.setTab(1)).addToLayout()
+                        InfoBox("Solver", lambda: self.setTab(2)).addToLayout()
                         layout2.addStretch()
-                        InfoBox("Spheroid", lambda: self.setTab(2)).addToLayout()
+                        InfoBox("Spheroid", lambda: self.setTab(3)).addToLayout()
                         layout2.addStretch()
-                        InfoBox("Orientation", lambda: self.setTab(3)).addToLayout()
+                        InfoBox("Orientation", lambda: self.setTab(4)).addToLayout()
                         layout2.addStretch()
                     layout.addStretch()
+                with self.tabs.createTab("Material Fit") as self.layout_code:
+                    QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+                    self.fitter = MainWindowFit().addToLayout()
+
                 with self.tabs.createTab("Solver") as self.layout_solver:
                     QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
 
                 with self.tabs.createTab("Spheroid") as self.layout_spheroid:
                     QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
 
                 with self.tabs.createTab("Orientation") as self.layout_orientation:
@@ -87,38 +94,38 @@
     solver = None
     spheroid = None
     orientation = None
     def changedTab(self, value):
         if self.first_tab_change is False:
             self.settings.setValue("master_tab", value)
 
-        if value == 1 and self.solver is None:
+        if value == 2 and self.solver is None:
             self.solver = SolverMain().addToLayout(self.layout_solver)
             self.setMinimumWidth(1600)
             self.setMinimumHeight(900)
-        if value == 2 and self.spheroid is None:
+        if value == 3 and self.spheroid is None:  # pragma: no cover
             self.spheroid = SpheroidMain().addToLayout(self.layout_spheroid)
             self.setMinimumWidth(1600)
             self.setMinimumHeight(900)
-        if value == 3 and self.orientation is None:
+        if value == 4 and self.orientation is None:  # pragma: no cover
             self.orientation = OrientationMain().addToLayout(self.layout_orientation)
             self.setMinimumWidth(1600)
             self.setMinimumHeight(900)
 
     def setTab(self, value):
         self.tabs.setCurrentIndex(value)
 
 
 def main():  # pragma: no cover
     app = QtWidgets.QApplication(sys.argv)
     if sys.platform.startswith('win'):
         import ctypes
         myappid = 'fabrylab.saenopy.master'  # arbitrary string
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
-    print(sys.argv)
+
     window = MainWindow()
     window.show()
     try:
         import pyi_splash
 
         # Update the text on the splash screen
         pyi_splash.update_text("PyInstaller is a great software!")
@@ -126,15 +133,24 @@
 
         # Close the splash screen. It does not matter when the call
         # to this function is made, the splash screen remains open until
         # this function is called or the Python program is terminated.
         pyi_splash.close()
     except (ImportError, RuntimeError):
         pass
-    sys.exit(app.exec_())
+
+    while True:
+        try:
+            res = app.exec_()
+            break
+        except Exception as err:
+            traceback.print_traceback(err)
+            QtWidgets.QMessageBox.critical(window, "Error", f"An Error occurred:\n{err}")
+            continue
+    sys.exit(res)
 
 
 if __name__ == '__main__':  # pragma: no cover
     # On Windows calling this function is necessary.
     multiprocessing.freeze_support()
 
     if len(sys.argv) >= 2 and sys.argv[1].endswith(".py"):
```

### Comparing `saenopy-0.9.0/saenopy/gui/orientation/gui_orientation.py` & `saenopy-1.0.0/saenopy/gui/orientation/gui_orientation.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,22 +487,22 @@
                 self.seg_gaus2_indi.setValue(attr["seg_gaus2"])
                 print("->", [v is None for v in attr.values()])
                 if np.all([v is None for v in attr.values()]):
                     self.individual_data.setValue(False)
                 else:
                     self.individual_data.setValue(True)
             self.last_cell = self.list.currentRow()
-            im_cell = imageio.imread(data[1])
+            im_cell = imageio.v2.imread(data[1])
             from CompactionAnalyzer.CompactionFunctions import segment_cell, normalize
             im_cell = normalize(im_cell, 1, 99)
 
             self.pixmap.setPixmap(get_pixmap(im_cell))
             self.label.setExtend(im_cell.shape[1], im_cell.shape[0])
 
-            im_fiber = imageio.imread(data[0])
+            im_fiber = imageio.v2.imread(data[0])
             im_fiber = normalize(im_fiber, 1, 99)
             self.pixmap2.setPixmap(get_pixmap(im_fiber))
             self.label2.setExtend(im_fiber.shape[1], im_fiber.shape[0])
 
             result = segment_cell(im_cell,
                                   thres=self.segmention_thres.value() if attr["segmention_thres"] is None else attr["segmention_thres"],
                                   seg_gaus1=self.seg_gaus1.value() if attr["seg_gaus1"] is None else attr["seg_gaus1"],
@@ -894,15 +894,15 @@
             button.setChecked(False)
         self.button_run.setChecked(True)
         self.current_plot_func = self.run2
 
         self.button_export.setDisabled(True)
 
         data = self.list2.data[self.list2.currentRow()][2]
-        im = imageio.imread(data["image"])
+        im = imageio.v2.imread(data["image"])
 
         plot_color = self.list.data[self.list.currentRow()][3]
 
         self.canvas.setActive()
         plt.cla()
         plt.axis("auto")
         if self.type.value() == "global orientation":
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/analyze/plot_window.py` & `saenopy-1.0.0/saenopy/gui/solver/analyze/plot_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,53 @@
 from qtpy import QtWidgets, QtCore, QtGui
 
 from saenopy import Result
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.common.gui_classes import ListWidget, MatplotlibWidget, execute
 
 
+class AddFilesDialog(QtWidgets.QDialog):
+    def __init__(self, parent, settings):
+        super().__init__(parent)
+        self.setWindowTitle("Add Files")
+        with QtShortCuts.QVBoxLayout(self) as layout:
+            self.label = QtWidgets.QLabel(
+                "Select a path as an input wildcard. Use * to specify a placeholder. All paths that match the wildcard will be added.")
+            layout.addWidget(self.label)
+
+            def checker(filename):
+                return filename + "/**/*.saenopy"
+
+            self.inputText = QtShortCuts.QInputFolder(None, None, settings=settings, filename_checker=checker,
+                                                      settings_key="batch_eval/analyse_force_wildcard", allow_edit=True)
+            with QtShortCuts.QHBoxLayout() as layout3:
+                # self.button_clear = QtShortCuts.QPushButton(None, "clear list", self.clear_files)
+                layout3.addStretch()
+                self.button_addList = QtShortCuts.QPushButton(None, "cancel", self.reject)
+                self.button_addList = QtShortCuts.QPushButton(None, "ok", self.accept)
+
+
+class ExportDialog(QtWidgets.QDialog):
+    def __init__(self, parent, settings):
+        super().__init__(parent)
+        self.setWindowTitle("Export Plot")
+        with QtShortCuts.QVBoxLayout(self) as layout:
+            self.label = QtWidgets.QLabel("Select a path to export the plot script with the data.")
+            layout.addWidget(self.label)
+            self.inputText = QtShortCuts.QInputFilename(None, None, file_type="Python Script (*.py)", settings=settings,
+                                                        settings_key="batch_eval/export_plot", existing=False)
+            self.strip_data = QtShortCuts.QInputBool(None, "export only essential data columns", True, settings=settings, settings_key="batch_eval/export_complete_df")
+            self.include_df = QtShortCuts.QInputBool(None, "include dataframe in script", True, settings=settings, settings_key="batch_eval/export_include_df")
+            with QtShortCuts.QHBoxLayout() as layout3:
+                # self.button_clear = QtShortCuts.QPushButton(None, "clear list", self.clear_files)
+                layout3.addStretch()
+                self.button_addList = QtShortCuts.QPushButton(None, "cancel", self.reject)
+                self.button_addList = QtShortCuts.QPushButton(None, "ok", self.accept)
+
+
 class PlottingWindow(QtWidgets.QWidget):
     progress_signal = QtCore.Signal(int, int, int, int)
     finished_signal = QtCore.Signal()
     thread = None
 
     def __init__(self, parent=None):
         super().__init__(parent)
@@ -83,14 +122,16 @@
         self.list.setData(self.data_folders)
         self.addGroup()
         self.current_plot_func = self.run2
 
     def save(self):
         new_path = QtWidgets.QFileDialog.getSaveFileName(None, "Save Session", os.getcwd(), "JSON File (*.json)")
         if new_path:
+            if not new_path.endswith(".json"):
+                new_path += ".json"
             list_new = []
             for item in self.list.data:
                 list_new.append({"name": item[0], "selected": item[1], "color": item[3], "paths": []})
                 for item2 in item[2]:
                     list_new[-1]["paths"].append({"path": item2[0], "selected": item[1]})
 
             with open(new_path, "w") as fp:
@@ -100,25 +141,24 @@
         new_path = QtWidgets.QFileDialog.getOpenFileName(None, "Load Session", os.getcwd(), "JSON File (*.json)")
         if new_path:
             with open(new_path, "r") as fp:
                 list_new = json.load(fp)
             self.list.clear()
             self.list.setData([[i["name"], i["selected"], [], i["color"]] for i in list_new])
             self.data_folders = self.list.data
-            print("y", self.list.data)
+
             for i, d in enumerate(list_new):
                 self.list.setCurrentRow(i)
                 self.list.listSelected()
                 self.listSelected()
                 self.list2.data = self.list.data[i][2]
-                self.add_files([d0["path"] for d0 in d["paths"]])
-                print("xxx", self.list.data)
-                for ii, d0 in enumerate(d["paths"]):
-                    self.list2.data[ii][1] = d0["selected"]
-            print("x", self.list.data)
+                self.add_files([d_0["path"] for d_0 in d["paths"]])
+
+                for ii, d_0 in enumerate(d["paths"]):
+                    self.list2.data[ii][1] = d_0["selected"]
 
     def dragEnterEvent(self, event: QtGui.QDragEnterEvent):
         # accept url lists (files by drag and drop)
         for url in event.mimeData().urls():
             # if str(url.toString()).strip().endswith(".npz"):
             event.accept()
             return
@@ -126,54 +166,68 @@
 
     def dragMoveEvent(self, event: QtGui.QDragMoveEvent):
         event.acceptProposedAction()
 
     def dropEvent(self, event: QtCore.QEvent):
         urls = []
         for url in event.mimeData().urls():
-            print(url)
             url = url.toLocalFile()
             if url[0] == "/" and url[2] == ":":
                 url = url[1:]
-            print(url)
-            if url.endswith(".npz"):
+            if url.endswith(".saenopy"):
                 urls += [url]
             else:
-                urls += glob.glob(url + "/**/*.npz", recursive=True)
+                urls += glob.glob(url + "/**/*.saenopy", recursive=True)
         self.add_files(urls)
 
     def add_files(self, urls):
         current_group = self.list2.data
         current_files = [d[0] for d in current_group]
         for file in urls:
             if file in current_files:
                 print("File already in list", file)
                 continue
             try:
                 print("Add file", file)
-                res = Result.load(file)
+                res: Result = Result.load(file)
                 res.resulting_data = []
-                for i, M in enumerate(res.solver):
+                if len(res.solvers) == 0 or res.solvers[0] is None or res.solvers[0].regularisation_results is None:
+                    continue
+                for i, M in enumerate(res.solvers):
                     res.resulting_data.append({
                         "t": i*res.time_delta if res.time_delta else 0,
-                        "strain_energy": M.E_glo,
-                        "contractility": M.getContractility(center_mode="force"),
-                        "polarity": M.getPolarity(),
-                        "99_percentile_deformation": np.nanpercentile(np.linalg.norm(M.U_target[M.reg_mask], axis=1), 99),
-                        "99_percentile_force": np.nanpercentile(np.linalg.norm(M.f[M.reg_mask], axis=1), 99),
+                        "strain_energy": M.mesh.strain_energy,
+                        "contractility": M.get_contractility(center_mode="force"),
+                        "polarity": M.get_polarity(),
+                        "99_percentile_deformation": np.nanpercentile(np.linalg.norm(M.mesh.displacements_target[M.mesh.regularisation_mask], axis=1), 99),
+                        "99_percentile_force": np.nanpercentile(np.linalg.norm(M.mesh.forces[M.mesh.regularisation_mask], axis=1), 99),
                         "filename": file,
                     })
                 res.resulting_data = pd.DataFrame(res.resulting_data)
                 if self.list2.data is current_group:
                     self.list2.addData(file, True, res)
-                    print("replot")
                     self.replot()
                 #app.processEvents()
             except FileNotFoundError:
                 continue
+        self.check_results_with_time()
+
+    def check_results_with_time(self):
+        time_values = False
+        for name, checked, files, color in self.data_folders:
+            if checked != 0:
+                for name2, checked2, res, color in files:
+                    if len(res.solvers) > 1:
+                        time_values = True
+        if time_values is False:
+            self.barplot()
+        self.agg.setEnabled(time_values)
+        self.button_run.setEnabled(time_values)
+        self.button_run2.setEnabled(time_values)
+
 
     def update_group_name(self):
         if self.list.currentItem() is not None:
             self.box_group.setTitle(f"Files for '{self.list.currentItem().text()}'")
             self.box_group.setEnabled(True)
         else:
             self.box_group.setEnabled(False)
@@ -181,49 +235,23 @@
     def addGroup(self):
         text = f"Group{1+len(self.data_folders)}"
         item = self.list.addData(text, True, [], mpl.colors.to_hex(f"C{len(self.data_folders)}"))
         self.list.setCurrentItem(item)
         self.list.editItem(item)
 
     def addFiles(self):
-        settings = self.settings
-        class AddFilesDialog(QtWidgets.QDialog):
-            def __init__(self, parent):
-                super().__init__(parent)
-                self.setWindowTitle("Add Files")
-                with QtShortCuts.QVBoxLayout(self) as layout:
-                    self.label = QtWidgets.QLabel("Select a path as an input wildcard. Use * to specify a placeholder. All paths that match the wildcard will be added.")
-                    layout.addWidget(self.label)
-                    def checker(filename):
-                        return filename + "/**/*.npz"
-                    self.inputText = QtShortCuts.QInputFolder(None, None, settings=settings, filename_checker=checker,
-                                                                settings_key="batch_eval/analyse_force_wildcard", allow_edit=True)
-                    with QtShortCuts.QHBoxLayout() as layout3:
-                        # self.button_clear = QtShortCuts.QPushButton(None, "clear list", self.clear_files)
-                        layout3.addStretch()
-                        self.button_addList = QtShortCuts.QPushButton(None, "cancel", self.reject)
-                        self.button_addList = QtShortCuts.QPushButton(None, "ok", self.accept)
-
-        dialog = AddFilesDialog(self)
+        dialog = AddFilesDialog(self, self.settings)
         if not dialog.exec():
             return
 
         text = os.path.normpath(dialog.inputText.value())
         files = glob.glob(text, recursive=True)
 
         self.add_files(files)
 
-    def getPandasData(self, file):
-        res = pd.read_excel(file)
-        res["filename"] = file
-        res["index"] = res["Unnamed: 0"]
-        del res["Unnamed: 0"]
-        res["group"] = file
-        return res
-
     def listSelected(self):
         try:
             data = self.data_folders[self.list.currentRow()]
         except IndexError:
             return
         self.update_group_name()
         self.list2.setData(data[2])
@@ -268,23 +296,20 @@
             mu_name = '99_percentile_force'
             y_label = 'Force'
 
         # get all the data as a pandas dataframe
         res = self.getAllCurrentPandasData()
 
         # limit the dataframe to the comparison time
-        print(res)
-        print(res.columns)
         res0 = res.groupby("filename").agg("max")
+        del res["group"]
         res = res.groupby("filename").agg(self.agg.value())
         res["group"] = res0["group"]
         #index = self.get_comparison_index()
         #res = res[res.index == index]
-        print(res)
-        print(res.columns, self.agg.value())
 
         code_data = [res, ["group", mu_name]]
 
         color_dict = {d[0]: d[3] for d in self.data_folders}
 
         def plot(res, mu_name, y_label, color_dict2):
             # define the colors
@@ -365,14 +390,16 @@
 
         code = execute(plot, code_data[0][code_data[1]], mu_name=mu_name, y_label=y_label, color_dict2=color_dict)
 
         self.export_data = [code, code_data]
         return
 
     def run2(self):
+        if not self.button_run.isEnabled():
+            return
         for button in self.plot_buttons:
             button.setChecked(False)
         self.button_run.setChecked(True)
         #return
         self.current_plot_func = self.run2
         if self.type.value() == "strain_energy":
             mu_name = 'strain_energy'
@@ -429,33 +456,15 @@
             self.canvas.draw()
 
         code = execute(plot, code_data[0][code_data[1]], mu_name=mu_name, y_label=y_label, plot_color=self.data_folders[self.list.currentRow()][3])
 
         self.export_data = [code, code_data]
 
     def export(self):
-        settings = self.settings
-        class AddFilesDialog(QtWidgets.QDialog):
-            def __init__(self, parent):
-                super().__init__(parent)
-                self.setWindowTitle("Export Plot")
-                with QtShortCuts.QVBoxLayout(self) as layout:
-                    self.label = QtWidgets.QLabel("Select a path to export the plot script with the data.")
-                    layout.addWidget(self.label)
-                    self.inputText = QtShortCuts.QInputFilename(None, None, file_type="Python Script (*.py)", settings=settings,
-                                                                settings_key="batch_eval/export_plot", existing=False)
-                    self.strip_data = QtShortCuts.QInputBool(None, "export only essential data columns", True, settings=settings, settings_key="batch_eval/export_complete_df")
-                    self.include_df = QtShortCuts.QInputBool(None, "include dataframe in script", True, settings=settings, settings_key="batch_eval/export_include_df")
-                    with QtShortCuts.QHBoxLayout() as layout3:
-                        # self.button_clear = QtShortCuts.QPushButton(None, "clear list", self.clear_files)
-                        layout3.addStretch()
-                        self.button_addList = QtShortCuts.QPushButton(None, "cancel", self.reject)
-                        self.button_addList = QtShortCuts.QPushButton(None, "ok", self.accept)
-
-        dialog = AddFilesDialog(self)
+        dialog = ExportDialog(self, self.settings)
         if not dialog.exec():
             return
 
         with open(str(dialog.inputText.value()), "wb") as fp:
             code = ""
             code += "import matplotlib.pyplot as plt\n"
             code += "import pandas as pd\n"
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/gui_solver.py` & `saenopy-1.0.0/saenopy/gui/solver/gui_solver.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/BatchEvaluate.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/BatchEvaluate.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .MeshCreator import MeshCreator
 from .Regularizer import Regularizer
 from .ResultView import ResultView
 from .StackDisplay import StackDisplay
 from saenopy.gui.solver.modules.exporter.Exporter import ExportViewer
 from .load_measurement_dialog import AddFilesDialog, FileExistsDialog
 from .path_editor import start_path_change
-from saenopy.examples import getExamples
+from saenopy.examples import get_examples
 
 
 class SharedProperties:
     properties = None
 
     def __init__(self):
         self.properties = {}
@@ -65,15 +65,16 @@
                     layout.setContentsMargins(0, 0, 0, 0)
                     self.list = ListWidget(layout, add_item_button="add measurements", copy_params=True, allow_paste_callback=self.allow_paste)
                     self.list.addItemClicked.connect(self.add_measurement)
                     self.list.signal_act_copy_clicked.connect(self.copy_params)
                     self.list.signal_act_paste_clicked.connect(self.paste_params)
                     self.list.signal_act_paths_clicked.connect(self.path_editor)
                     self.list.itemSelectionChanged.connect(self.listSelected)
-                    self.progressbar = QProgressBar().addToLayout()
+                    self.progressbar = QtWidgets.QProgressBar().addToLayout()
+                    self.progressbar.setOrientation(QtCore.Qt.Horizontal)
                 with QtShortCuts.QHBoxLayout() as layout:
                     layout.setContentsMargins(0, 0, 0, 0)
                     with QtShortCuts.QTabWidget(layout) as self.tabs:
                         self.tabs.setMinimumWidth(500)
                         old_tab = None
                         cam_pos = None
                         def tab_changed(x):
@@ -113,22 +114,27 @@
 
         self.tasks = []
         self.current_task_id = 0
         self.thread = None
         self.signal_task_finished.connect(self.run_finished)
 
         # load paths
-        self.load_from_path([arg for arg in sys.argv if arg.endswith(".npz")])
+        self.load_from_path([arg for arg in sys.argv if arg.endswith(".saenopy")])
+
+        # disable all tabs
+        for i in range(self.tabs.count()-1, -1, -1):
+            self.tabs.setTabEnabled(i, False)
 
     def copy_params(self):
         result = self.list.data[self.list.currentRow()][2]
         params = {
-            "piv_parameter": result.piv_parameter_tmp,
-            "interpolate_parameter": result.interpolate_parameter_tmp,
-            "solve_parameter": result.solve_parameter_tmp,
+            "piv_parameters": result.piv_parameters_tmp,
+            "mesh_parameters": result.mesh_parameters_tmp,
+            "material_parameters": result.material_parameters_tmp,
+            "solve_parameters": result.solve_parameters_tmp,
         }
         print(params)
         for group in params:
             if params[group] is None:
                 continue
             for g in params[group]:
                 if type(params[group][g]) == np.bool_:
@@ -140,31 +146,32 @@
         cb.setText(text, mode=cb.Clipboard)
 
     def allow_paste(self):
         cb = QtGui.QGuiApplication.clipboard()
         text = cb.text(mode=cb.Clipboard)
         try:
             data = json.loads(text)
-            if "piv_parameter" in data and \
-                "interpolate_parameter" in data and \
-                "solve_parameter" in data:
+            if "piv_parameters" in data and \
+                "mesh_parameters" in data and \
+                "material_parameters" in data and \
+                "solve_parameters" in data:
                 return True
         except (ValueError, TypeError):
             return False
         return False
 
     def paste_params(self):
         cb = QtGui.QGuiApplication.clipboard()
         text = cb.text(mode=cb.Clipboard)
         try:
             data = json.loads(text)
         except ValueError:
             return False
         result = self.list.data[self.list.currentRow()][2]
-        params = ["piv_parameter", "interpolate_parameter", "solve_parameter"]
+        params = ["piv_parameters", "mesh_parameters", "material_parameters", "solve_parameters"]
         for par in params:
             if par in data:
                 setattr(result, par+"_tmp", data[par])
         self.set_current_result.emit(result)
 
     def path_editor(self):
         result = self.list.data[self.list.currentRow()][2]
@@ -185,15 +192,15 @@
             import_code = ""
             run_code = ""
             for module in [self.sub_module_stacks, self.sub_module_deformation, self.sub_module_mesh, self.sub_module_regularize]:
                 code1, code2 = module.get_code()
                 import_code += code1
                 run_code += code2 +"\n"
             run_code = import_code + "\n\n" + run_code
-            print(run_code)
+            #print(run_code)
             with open(new_path, "w") as fp:
                 fp.write(run_code)
 
     def run_all(self):
         for i in range(len(self.data)):
             if not self.data[i][1]:
                 continue
@@ -202,15 +209,14 @@
                 self.sub_module_deformation.start_process(result=result)
             if self.sub_module_mesh.group.value() is True:
                 self.sub_module_mesh.start_process(result=result)
             if self.sub_module_regularize.group.value() is True:
                 self.sub_module_regularize.start_process(result=result)
 
     def addTask(self, task, result, params, name):
-        print("add task", task, result, params, name)
         self.tasks.append([task, result, params, name])
         if self.thread is None:
             self.run_next()
 
     signal_task_finished = QtCore.Signal()
 
     def run_next(self):
@@ -260,22 +266,23 @@
             paths = [paths]
 
         # iterate over all paths
         for path in paths:
             # if it is a directory search all saenopy files in it
             path = Path(path)
             if path.is_dir():
-                path = str(path) + "/**/*.npz"
+                path = str(path) + "/**/*.saenopy"
             # glob over the path (or just use the path if it does not contain a *)
             for p in sorted(glob.glob(str(path), recursive=True)):
                 print(p)
                 try:
                     self.add_data(Result.load(p))
                 except Exception as err:
                     QtWidgets.QMessageBox.critical(self, "Open Files", f"File {p} is not a valid Saenopy file.")
+                    raise
         self.update_icons()
 
     def add_data(self, data):
         self.list.addData(data.output, True, data, mpl.colors.to_hex(f"gray"))
 
     def update_icons(self):
         for j in range(self.list.count( ) -1):
@@ -286,15 +293,15 @@
 
     def add_measurement(self):
         last_decision = None
         def do_overwrite(filename):
             nonlocal last_decision
 
             # if we are in demo mode always load the files
-            if os.environ.get("DEMO") == "true":
+            if os.environ.get("DEMO") == "true":  # pragma: no cover
                 return "read"
 
             # if there is a last decistion stored use that
             if last_decision is not None:
                 return last_decision
 
             # ask the user if they want to overwrite or read the existing file
@@ -357,52 +364,37 @@
         # load existing files
         elif dialog.mode == "existing":
             self.load_from_path(dialog.outputText3.value())
 
         # load from the examples database
         elif dialog.mode == "example":
             # get the date from the example referenced by name
-            example = getExamples()[dialog.mode_data]
+            example = get_examples()[dialog.mode_data]
 
             # generate a stack with the examples data
             results = get_stacks(
                 example["stack"],
                 reference_stack=example.get("reference_stack", None),
                 output_path=example["output_path"],
                 voxel_size=example["voxel_size"],
                 time_delta=example.get("time_delta", None),
                 crop=example.get("crop", None),
                 exist_overwrite_callback=do_overwrite,
             )
             # load all the measurement objects
             for data in results:
-                data.piv_parameter = example["piv_parameter"]
-                data.interpolate_parameter = example["interpolate_parameter"]
-                data.solve_parameter = example["solve_parameter"]
+                if getattr(data, "is_read", False) is False:
+                    data.piv_parameters = example["piv_parameters"]
+                    data.mesh_parameters = example["mesh_parameters"]
+                    data.material_parameters = example["material_parameters"]
+                    data.solve_parameters = example["solve_parameters"]
                 self.add_data(data)
+        elif dialog.mode == "example_evaluated":
+                self.load_from_path(dialog.examples_output)
 
         # update the icons
         self.update_icons()
 
     def listSelected(self):
         if self.list.currentRow() is not None and self.list.currentRow() < len(self.data):
             pipe = self.data[self.list.currentRow()][2]
             self.set_current_result.emit(pipe)
-
-
-class QProgressBar(QtWidgets.QProgressBar):
-    signal_start = QtCore.Signal(int)
-    signal_progress = QtCore.Signal(int)
-
-    def __init__(self):
-        super().__init__()
-        self.setOrientation(QtCore.Qt.Horizontal)
-        self.signal_start.connect(lambda i: self.setRange(0, i))
-        self.signal_progress.connect(lambda i: self.setValue(i))
-
-    def iterator(self, iter):
-        print("iterator", iter)
-        self.signal_start.emit(len(iter))
-        for i, v in enumerate(iter):
-            yield i
-            print("emit", i)
-            self.signal_progress.emit(i+1)
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/DeformationDetector.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/DeformationDetector.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import numpy as np
 from pyvistaqt import QtInteractor
 import inspect
 import tqdm
 from typing import Tuple
 
 import saenopy
-import saenopy.multigridHelper
+import saenopy.multigrid_helper
 import saenopy.materials
 from saenopy import Result
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.common.gui_classes import CheckAbleGroup, QProcess, ProcessSimple
-import saenopy.getDeformations
+import saenopy.get_deformations
 
 from .PipelineModule import PipelineModule
 from .QTimeSlider import QTimeSlider
 from .VTK_Toolbar import VTK_Toolbar
 from .showVectorField import showVectorField, showVectorField2
 from .code_export import get_code
 
@@ -34,25 +34,25 @@
         super().__init__(parent, layout)
 
         with QtShortCuts.QVBoxLayout(self) as layout:
             layout.setContentsMargins(0, 0, 0, 0)
             with CheckAbleGroup(self, "find deformations (piv)", url="https://saenopy.readthedocs.io/en/latest/interface_solver.html#detect-deformations").addToLayout() as self.group:
                 with QtShortCuts.QVBoxLayout() as layout:
                     with QtShortCuts.QHBoxLayout():
-                        self.input_elementsize = QtShortCuts.QInputNumber(None, "piv elem. size", 15.0, step=1,
-                                                                          value_changed=self.valueChanged,
+                        self.input_element_size = QtShortCuts.QInputNumber(None, "piv elem. size", 15.0, step=1,
+                                                                          value_changed=self.valueChanged, unit="μm",
                                                                           tooltip="the grid size for deformation detection")
 
                         self.input_win = QtShortCuts.QInputNumber(None, "window size", 30,
                                                                   value_changed=self.valueChanged, unit="μm",
                                                                   tooltip="the size of the volume to look for a match")
                     with QtShortCuts.QHBoxLayout():
-                        self.input_signoise = QtShortCuts.QInputNumber(None, "signoise", 1.3, step=0.1,
+                        self.input_signoise = QtShortCuts.QInputNumber(None, "signal to noise", 1.3, step=0.1,
                                                                        tooltip="the signal to noise ratio threshold value, values below are ignore")
-                        self.input_driftcorrection = QtShortCuts.QInputBool(None, "driftcorrection", True,
+                        self.input_driftcorrection = QtShortCuts.QInputBool(None, "drift correction", True,
                                                                             tooltip="remove the mean displacement to correct for a global drift")
                     self.label = QtWidgets.QLabel().addToLayout()
                     self.input_button = QtShortCuts.QPushButton(None, "detect deformations", self.start_process)
 
         with self.parent.tabs.createTab("PIV Deformations") as self.tab:
             with QtShortCuts.QVBoxLayout() as layout:
                 self.label_tab = QtWidgets.QLabel(
@@ -71,47 +71,46 @@
                     parent.shared_properties.add_property("z_slider", self)
 
                 self.vtk_toolbar = VTK_Toolbar(self.plotter, self.update_display, "deformation", z_slider=self.z_slider, shared_properties=self.parent.shared_properties).addToLayout()
 
                 self.t_slider = QTimeSlider(connected=self.update_display).addToLayout()
                 self.tab.parent().t_slider = self.t_slider
 
-        self.setParameterMapping("piv_parameter", {
-            "win_um": self.input_win,
-            "elementsize": self.input_elementsize,
-            # "fac_overlap": self.input_overlap,
-            "signoise_filter": self.input_signoise,
+        self.setParameterMapping("piv_parameters", {
+            "window_size": self.input_win,
+            "element_size": self.input_element_size,
+            "signal_to_noise": self.input_signoise,
             "drift_correction": self.input_driftcorrection,
         })
 
     def z_slider_value_changed(self):
         self.update_display()
 
     def check_available(self, result: Result) -> bool:
-        return result is not None and result.stack is not None and len(result.stack)
+        return result is not None and result.stacks is not None and len(result.stacks)
 
     def check_evaluated(self, result: Result) -> bool:
         try:
             return self.result.mesh_piv[0] is not None
         except (AttributeError, IndexError):
             return False
 
     def property_changed(self, name, value):
         if name == "z_slider":
             self.z_slider.setValue(value)
 
     def setResult(self, result: Result):
         super().setResult(result)
-        if result and result.stack and result.stack[0]:
-            self.z_slider.setRange(0, result.stack[0].shape[2] - 1)
-            self.z_slider.setValue(result.stack[0].shape[2] // 2)
+        if result and result.stacks and result.stacks[0]:
+            self.z_slider.setRange(0, result.stacks[0].shape[2] - 1)
+            self.z_slider.setValue(result.stacks[0].shape[2] // 2)
 
-            if result.stack[0].channels:
+            if result.stacks[0].channels:
                 value = self.vtk_toolbar.channel_select.value()
-                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stack[0].channels)), result.stack[0].channels)
+                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stacks[0].channels)), result.stacks[0].channels)
                 self.vtk_toolbar.channel_select.setValue(value)
                 self.vtk_toolbar.channel_select.setVisible(True)
             else:
                 self.vtk_toolbar.channel_select.setValue(0)
                 self.vtk_toolbar.channel_select.setVisible(False)
 
     def update_display(self, *, plotter=None):
@@ -123,101 +122,105 @@
             plotter = self.plotter
         cam_pos = None
         if plotter.camera_position is not None and CamPos.cam_pos_initialized is True:
             cam_pos = self.plotter.camera_position
         CamPos.cam_pos_initialized = True
         plotter.interactor.setToolTip("")
         if self.result is None:
-            M = None
+            mesh = None
         else:
-            M = self.result.mesh_piv[self.t_slider.value()]
+            mesh = self.result.mesh_piv[self.t_slider.value()]
 
-        if M is None:
+        if mesh is None:
             plotter.show()
             return
 
         plotter.interactor.setToolTip(
-            str(self.result.piv_parameter) + f"\nNodes {self.result.mesh_piv[0].R.shape[0]}\nTets {self.result.mesh_piv[0].T.shape[0]}")
+            str(self.result.piv_parameters) + f"\nNodes {mesh.nodes.shape[0]}\nTets {mesh.tetrahedra.shape[0]}")
 
-        if M.hasNodeVar("U_measured"):
-            showVectorField2(self, M, "U_measured")
+        if mesh.displacements_measured is not None:
+            showVectorField2(self, mesh, "displacements_measured")
 
         if cam_pos is not None:
             plotter.camera_position = cam_pos
 
     def valueChanged(self):
         if self.check_available(self.result):
-            voxel_size1 = self.result.stack[0].voxel_size
-            stack_deformed = self.result.stack[0]
-            overlap = 1 - (self.input_elementsize.value() / self.input_win.value())
+            voxel_size1 = self.result.stacks[0].voxel_size
+            stack_deformed = self.result.stacks[0]
+            overlap = 1 - (self.input_element_size.value() / self.input_win.value())
             stack_size = np.array(stack_deformed.shape)[:3] * voxel_size1 - self.input_win.value()
             self.label.setText(
-                f"""Overlap between neighbouring windows\n(size={self.input_win.value()}µm or {(self.input_win.value() / np.array(voxel_size1)).astype(int)} px) is choosen \n to {int(overlap * 100)}% for an elementsize of {self.input_elementsize.value():.1f}μm elements.\nTotal region is {stack_size}.""")
+                f"""Overlap between neighbouring windows\n(size={self.input_win.value()}µm or {(self.input_win.value() / np.array(voxel_size1)).astype(int)} px) is choosen \n to {int(overlap * 100)}% for an element_size of {self.input_element_size.value():.1f}μm elements.\nTotal region is {stack_size}.""")
         else:
             self.label.setText("")
 
-    def process(self, result: Result, params: dict):
+    def process(self, result: Result, piv_parameters: dict):
         # demo run
         if os.environ.get("DEMO") == "true":
             self.parent.progressbar.setRange(0, 10)
             for i in range(11):
                 time.sleep(0.1)
                 self.parent.progressbar.setValue(i)
             result.mesh_piv = result.mesh_piv_demo
             return
 
         if not isinstance(result.mesh_piv, list):
-            result.mesh_piv = [None] * (len(result.stack) - 1)
+            result.mesh_piv = [None] * (len(result.stacks) - 1)
 
-        count = len(result.stack)
+        count = len(result.stacks)
         if result.stack_reference is None:
             count -= 1
 
         for i in range(count):
-            p = ProcessSimple(getDeformation, (i, result, params), {}, self.processing_progress, use_thread=self.use_thread)
+            p = ProcessSimple(getDeformation, (i, result, piv_parameters), {}, self.processing_progress, use_thread=self.use_thread)
             p.start()
-            result.mesh_piv[i] = p.join()
+            return_value = p.join()
+            if isinstance(return_value, Exception):
+                raise return_value
+            else:
+                result.mesh_piv[i] = return_value
 
-        result.solver = None
+        result.solvers = None
 
     def get_code(self) -> Tuple[str, str]:
         import_code = ""
 
         results = None
         def code(my_piv_params):  # pragma: no cover
             # define the parameters for the piv deformation detection
-            params = my_piv_params
+            piv_parameters = my_piv_params
 
             # iterate over all the results objects
             for result in results:
                 # set the parameters
-                result.piv_parameter = params
+                result.piv_parameters = params
                 # get count
-                count = len(result.stack)
+                count = len(result.stacks)
                 if result.stack_reference is None:
                     count -= 1
                 # iterate over all stack pairs
                 for i in range(count):
                     # get two consecutive stacks
                     if result.stack_reference is None:
-                        stack1, stack2 = result.stack[i], result.stack[i + 1]
+                        stack1, stack2 = result.stacks[i], result.stacks[i + 1]
                     # or reference stack and one from the list
                     else:
-                        stack1, stack2 = result.stack_reference, result.stack[i]
+                        stack1, stack2 = result.stack_reference, result.stacks[i]
                     # and calculate the displacement between them
                     result.mesh_piv[i] = saenopy.get_displacements_from_stacks(stack1, stack2,
-                                                                               params["win_um"],
-                                                                               params["elementsize"],
-                                                                               params["signoise_filter"],
-                                                                               params["drift_correction"])
+                                                                               piv_parameters["window_size"],
+                                                                               piv_parameters["element_size"],
+                                                                               piv_parameters["signal_to_noise"],
+                                                                               piv_parameters["drift_correction"])
                 # save the displacements
                 result.save()
 
         data = {
-            "my_piv_params": self.result.piv_parameter_tmp
+            "my_piv_params": self.result.piv_parameters_tmp
         }
 
         code = get_code(code, data)
 
         return import_code, code
 
 
@@ -239,19 +242,21 @@
             progress.put((0, self.total))
         return do_init
     tqdm.tqdm.__init__ = wrap_init(tqdm.tqdm.__init__)
     #tqdm.tqdm.__new__ = lambda cls, iter: progress.put(iter)
 
     try:
         if result.stack_reference is None:
-            stack1, stack2 = result.stack[i], result.stack[i + 1]
+            stack1, stack2 = result.stacks[i], result.stacks[i + 1]
         else:
-            stack1, stack2 = result.stack_reference, result.stack[i]
+            stack1, stack2 = result.stack_reference, result.stacks[i]
         mesh_piv = saenopy.get_displacements_from_stacks(stack1, stack2,
-                                                         params["win_um"],
-                                                         params["elementsize"],
-                                                         params["signoise_filter"],
+                                                         params["window_size"],
+                                                         params["element_size"],
+                                                         params["signal_to_noise"],
                                                          params["drift_correction"])
+    except Exception as err:
+        return err
     finally:
         tqdm.tqdm.update = old_update
         tqdm.tqdm.__init__ = old_init
     return mesh_piv
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/FittedMesh.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/FittedMesh.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,40 +36,38 @@
                     parent.shared_properties.add_property("z_slider", self)
 
                 self.vtk_toolbar = VTK_Toolbar(self.plotter, self.update_display, shared_properties=self.parent.shared_properties).addToLayout()
 
                 self.t_slider = QTimeSlider(connected=self.update_display).addToLayout()
                 self.tab.parent().t_slider = self.t_slider
 
-        self.setParameterMapping(None, {})
-
     def z_slider_value_changed(self):
         self.update_display()
 
     def check_available(self, result: Result):
-        return result is not None and result.solver is not None
+        return result is not None and result.solvers is not None
 
     def check_evaluated(self, result: Result) -> bool:
         try:
-            return getattr(self.result.solver[0], "regularisation_results", None) is not None
+            return getattr(self.result.solvers[0], "regularisation_results", None) is not None
         except (AttributeError, IndexError, TypeError):
             return False
 
     def property_changed(self, name, value):
         if name == "z_slider":
             self.z_slider.setValue(value)
 
     def setResult(self, result: Result):
         super().setResult(result)
-        if result and result.stack and result.stack[0]:
-            self.z_slider.setRange(0, result.stack[0].shape[2] - 1)
-            self.z_slider.setValue(self.result.stack[0].shape[2] // 2)
+        if result and result.stacks and result.stacks[0]:
+            self.z_slider.setRange(0, result.stacks[0].shape[2] - 1)
+            self.z_slider.setValue(self.result.stacks[0].shape[2] // 2)
 
-            if result.stack[0].channels:
-                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stack[0].channels)), result.stack[0].channels)
+            if result.stacks[0].channels:
+                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stacks[0].channels)), result.stacks[0].channels)
                 self.vtk_toolbar.channel_select.setVisible(True)
             else:
                 self.vtk_toolbar.channel_select.setValue(0)
                 self.vtk_toolbar.channel_select.setVisible(False)
 
     def update_display(self):
         if self.current_tab_selected is False:
@@ -77,16 +75,17 @@
             return
 
         if self.check_evaluated(self.result):
             cam_pos = None
             if self.plotter.camera_position is not None and CamPos.cam_pos_initialized is True:
                 cam_pos = self.plotter.camera_position
             CamPos.cam_pos_initialized = True
-            self.plotter.interactor.setToolTip(str(self.result.solve_parameter)+f"\nNodes {self.result.solver[self.t_slider.value()].R.shape[0]}\nTets {self.result.solver[self.t_slider.value()].T.shape[0]}")
-            M = self.result.solver[self.t_slider.value()]
-            showVectorField2(self, M, "U")
-            #showVectorField(self.plotter, M, M.U, "U", factor=0.1, scalebar_max=self.vtk_toolbar.getScaleMax(), show_nan=self.vtk_toolbar.use_nans.value())
+            M = self.result.solvers[self.t_slider.value()]
+            mesh = M.mesh
+            self.plotter.interactor.setToolTip(str(self.result.solve_parameters) + f"\nNodes {mesh.nodes.shape[0]}\nTets {mesh.tetrahedra.shape[0]}")
+            showVectorField2(self, mesh, "displacements")
+            #showVectorField(self.plotter, M, M.U, "displacements", factor=0.1, scalebar_max=self.vtk_toolbar.getScaleMax(), show_nan=self.vtk_toolbar.use_nans.value())
             if cam_pos is not None:
                 self.plotter.camera_position = cam_pos
         else:
             self.plotter.interactor.setToolTip("")
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/MeshCreator.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/MeshCreator.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,33 +20,81 @@
 
 from pathlib import Path
 import re
 import pandas as pd
 import matplotlib as mpl
 
 import saenopy
-import saenopy.multigridHelper
-from saenopy.multigridHelper import getScaledMesh, getNodesWithOneFace
-import saenopy.getDeformations
+import saenopy.multigrid_helper
+from saenopy.multigrid_helper import get_scaled_mesh, get_nodes_with_one_face
+import saenopy.get_deformations
 import saenopy.materials
-from saenopy.stack import Stack, getStack, format_glob
+from saenopy.stack import Stack, format_glob
 from saenopy.saveable import Saveable
 from saenopy import Result
 from saenopy.gui.common import QtShortCuts, QExtendedGraphicsView
 from saenopy.gui.common.gui_classes import Spoiler, CheckAbleGroup, QHLine, QVLine, MatplotlibWidget, NavigationToolbar, execute, kill_thread, ListWidget, QProcess, ProcessSimple
 from saenopy.gui.common.stack_selector import StackSelector
 
 
 from .PipelineModule import PipelineModule
 from .QTimeSlider import QTimeSlider
 from .VTK_Toolbar import VTK_Toolbar
 from .showVectorField import showVectorField, showVectorField2
 from .DeformationDetector import CamPos
 from .code_export import get_code
 
+class MeshSizeWidget(QtWidgets.QWidget):
+    valueChanged = QtCore.Signal(object)
+
+    def __init__(self):
+        super().__init__()
+        with QtShortCuts.QVBoxLayout(self):
+            with QtShortCuts.QHBoxLayout():
+                self.input_mesh_size_same = QtShortCuts.QInputBool(None, "mesh size same as stack", True,
+                                                                   #value_changed=self.valueChanged,
+                                                                   tooltip="make the mesh size the same as the piv mesh")
+            with QtShortCuts.QHBoxLayout():
+                self.input_mesh_size_x = QtShortCuts.QInputNumber(None, "x", 200, step=1, unit="μm",
+                                                                  tooltip="the custom new mesh size")
+                self.input_mesh_size_y = QtShortCuts.QInputNumber(None, "y", 200, step=1, unit="μm",
+                                                                  tooltip="the custom new mesh size")
+                self.input_mesh_size_z = QtShortCuts.QInputNumber(None, "z", 200, step=1, unit="μm",
+                                                                  tooltip="the custom new mesh size")
+            self.input_mesh_size_x.valueChanged.connect(self.valueChangedCallback)
+            self.input_mesh_size_y.valueChanged.connect(self.valueChangedCallback)
+            self.input_mesh_size_z.valueChanged.connect(self.valueChangedCallback)
+            self.input_mesh_size_same.valueChanged.connect(self.valueChangedCallback)
+
+            self.setValue("piv")
+
+    def valueChangedCallback(self):
+        self.input_mesh_size_x.setDisabled(self.input_mesh_size_same.value())
+        self.input_mesh_size_y.setDisabled(self.input_mesh_size_same.value())
+        self.input_mesh_size_z.setDisabled(self.input_mesh_size_same.value())
+        self.valueChanged.emit(self.value())
+
+    def value(self):
+        if self.input_mesh_size_same.value():
+            return "piv"
+        else:
+            return (self.input_mesh_size_x.value(), self.input_mesh_size_y.value(), self.input_mesh_size_z.value())
+
+    def setValue(self, value):
+        if value == "piv":
+            self.input_mesh_size_same.setValue(True)
+        else:
+            self.input_mesh_size_same.setValue(False)
+            self.input_mesh_size_x.setValue(value[0])
+            self.input_mesh_size_y.setValue(value[1])
+            self.input_mesh_size_z.setValue(value[2])
+        self.input_mesh_size_x.setDisabled(self.input_mesh_size_same.value())
+        self.input_mesh_size_y.setDisabled(self.input_mesh_size_same.value())
+        self.input_mesh_size_z.setDisabled(self.input_mesh_size_same.value())
+
 
 class MeshCreator(PipelineModule):
     mesh_size = [200, 200, 200]
     pipeline_name = "interpolate mesh"
 
     def __init__(self, parent: "BatchEvaluate", layout):
         super().__init__(parent, layout)
@@ -58,29 +106,17 @@
                 with QtShortCuts.QVBoxLayout():
 
                     with QtShortCuts.QHBoxLayout() as layout2:
                         self.input_reference = QtShortCuts.QInputChoice(None, "reference stack", "next",
                                                                         ["next", "median"], tooltip="the reference for the deformations")
                         self.input_reference.setEnabled(False)
                         self.input_element_size = QtShortCuts.QInputNumber(None, "mesh elem. size", 7, unit="μm", tooltip="the element size of the regularisatio mesh")
-                        #with QtShortCuts.QHBoxLayout() as layout2:
-                        self.input_inner_region = QtShortCuts.QInputNumber(None, "inner region", 100, unit="μm")
-                        self.input_inner_region.setVisible(False)
-                        self.input_thinning_factor = QtShortCuts.QInputNumber(None, "thinning factor", 0, step=0.1)
-                        self.input_thinning_factor.setVisible(False)
                         layout2.addStretch()
-                    with QtShortCuts.QHBoxLayout():
-                        self.input_mesh_size_same = QtShortCuts.QInputBool(None, "mesh size same as stack", True, value_changed=self.valueChanged, tooltip="make the mesh size the same as the piv mesh")
-                    with QtShortCuts.QHBoxLayout():
-                        self.input_mesh_size_x = QtShortCuts.QInputNumber(None, "x", 200, step=1, name_post="μm", tooltip="the custom new mesh size")
-                        self.input_mesh_size_y = QtShortCuts.QInputNumber(None, "y", 200, step=1, name_post="μm", tooltip="the custom new mesh size")
-                        self.input_mesh_size_z = QtShortCuts.QInputNumber(None, "z", 200, step=1, name_post="μm", tooltip="the custom new mesh size")
-                        #self.input_mesh_size_label = QtWidgets.QLabel("μm").addToLayout()
-                    self.valueChanged()
 
+                    self.input_mesh_size = MeshSizeWidget().addToLayout()
 
                     self.input_button = QtWidgets.QPushButton("interpolate mesh").addToLayout()
                     self.input_button.clicked.connect(self.start_process)
 
         with self.parent.tabs.createTab("Target Deformations") as self.tab:
             with QtShortCuts.QVBoxLayout() as layout:
                 self.label_tab = QtWidgets.QLabel("The deformations from the piv algorithm interpolated on the new mesh for regularisation.").addToLayout()
@@ -99,67 +135,41 @@
 
                 self.vtk_toolbar = VTK_Toolbar(self.plotter, self.update_display, shared_properties=self.parent.shared_properties).addToLayout()
 
 
                 self.t_slider = QTimeSlider(connected=self.update_display).addToLayout()
                 self.tab.parent().t_slider = self.t_slider
 
-        self.setParameterMapping("interpolate_parameter", {
+        self.setParameterMapping("mesh_parameters", {
             "reference_stack": self.input_reference,
             "element_size": self.input_element_size,
-            "inner_region": self.input_inner_region,
-            "thinning_factor": self.input_thinning_factor,
-            "mesh_size_same": self.input_mesh_size_same,
-            "mesh_size_x": self.input_mesh_size_x,
-            "mesh_size_y": self.input_mesh_size_y,
-            "mesh_size_z": self.input_mesh_size_z,
+            "mesh_size": self.input_mesh_size,
         })
 
-    def valueChanged(self):
-        self.input_mesh_size_x.setDisabled(self.input_mesh_size_same.value())
-        self.input_mesh_size_y.setDisabled(self.input_mesh_size_same.value())
-        self.input_mesh_size_z.setDisabled(self.input_mesh_size_same.value())
-        self.deformation_detector_mesh_size_changed()
-
-    def deformation_detector_mesh_size_changed(self):
-        if self.input_mesh_size_same.value():
-            try:
-                valid = self.result.mesh_piv[0] is not None
-            except (AttributeError, IndexError, TypeError):
-                valid = False
-            if valid:
-                x, y, z = (self.result.mesh_piv[0].R.max(axis=0) - self.result.mesh_piv[0].R.min(axis=0))*1e6
-                self.input_mesh_size_x.setValue(x)
-                self.setParameter("mesh_size_x", x)
-                self.input_mesh_size_y.setValue(y)
-                self.setParameter("mesh_size_y", y)
-                self.input_mesh_size_z.setValue(z)
-                self.setParameter("mesh_size_z", z)
-
     def z_slider_value_changed(self):
         self.update_display()
 
     def check_available(self, result: Result):
         return result is not None and result.mesh_piv is not None and len(result.mesh_piv) and result.mesh_piv[0] is not None
 
     def check_evaluated(self, result: Result) -> bool:
-        return result is not None and result.solver is not None and len(result.solver) and result.solver[0] is not None
+        return result is not None and result.solvers is not None and len(result.solvers) and result.solvers[0] is not None
 
     def property_changed(self, name, value):
         if name == "z_slider":
             self.z_slider.setValue(value)
 
     def setResult(self, result: Result):
         super().setResult(result)
-        if result and result.stack and result.stack[0]:
-            self.z_slider.setRange(0, result.stack[0].shape[2] - 1)
-            self.z_slider.setValue(self.result.stack[0].shape[2] // 2)
+        if result and result.stacks and result.stacks[0]:
+            self.z_slider.setRange(0, result.stacks[0].shape[2] - 1)
+            self.z_slider.setValue(self.result.stacks[0].shape[2] // 2)
 
-            if result.stack[0].channels:
-                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stack[0].channels)), result.stack[0].channels)
+            if result.stacks[0].channels:
+                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stacks[0].channels)), result.stacks[0].channels)
                 self.vtk_toolbar.channel_select.setVisible(True)
             else:
                 self.vtk_toolbar.channel_select.setValue(0)
                 self.vtk_toolbar.channel_select.setVisible(False)
 
             if result.stack_reference is None:
                 self.input_reference.setValues(["next", "median"])
@@ -178,62 +188,63 @@
         else:
             self.input_reference.setEnabled(False)
         if self.check_evaluated(self.result):
             cam_pos = None
             if self.plotter.camera_position is not None and CamPos.cam_pos_initialized is True:
                 cam_pos = self.plotter.camera_position
             CamPos.cam_pos_initialized = True
-            self.plotter.interactor.setToolTip(str(self.result.interpolate_parameter)+f"\nNodes {self.result.solver[self.t_slider.value()].R.shape[0]}\nTets {self.result.solver[self.t_slider.value()].T.shape[0]}")
-            M = self.result.solver[self.t_slider.value()]
-            showVectorField2(self, M, "U_target")
+            M = self.result.solvers[self.t_slider.value()]
+            mesh = M.mesh
+            self.plotter.interactor.setToolTip(str(self.result.mesh_parameters) + f"\nNodes {mesh.nodes.shape[0]}\nTets {mesh.tetrahedra.shape[0]}")
+            showVectorField2(self, mesh, "displacements_target")
             if cam_pos is not None:
                 self.plotter.camera_position = cam_pos
         else:
             self.plotter.interactor.setToolTip("")
 
-    def process(self, result: Result, params: dict):
+    def process(self, result: Result, mesh_parameters: dict):
         # demo run
-        if os.environ.get("DEMO") == "true":
-            result.solver = result.solver_demo
+        if os.environ.get("DEMO") == "true":  # pragma: no cover
+            result.solvers = result.solver_demo
             return
         
         # make sure the solver list exists and has the required length
-        if result.solver is None or len(result.solver) != len(result.mesh_piv):
-            result.solver = [None]*len(result.mesh_piv)
+        if result.solvers is None or len(result.solvers) != len(result.mesh_piv):
+            result.solvers = [None] * len(result.mesh_piv)
         
         # correct for the reference state
-        displacement_list = saenopy.subtract_reference_state(result.mesh_piv, params["reference_stack"])
+        displacement_list = saenopy.subtract_reference_state(result.mesh_piv, mesh_parameters["reference_stack"])
         
         # set the parameters
-        result.interpolate_parameter = params
+        result.mesh_parameters = mesh_parameters
         # iterate over all stack pairs
         for i in range(len(result.mesh_piv)):
             # and create the interpolated solver mesh
-            result.solver[i] = saenopy.interpolate_mesh(result.mesh_piv[i], displacement_list[i], params)
+            result.solvers[i] = saenopy.interpolate_mesh(result.mesh_piv[i], displacement_list[i], mesh_parameters)
         # save the meshes
         result.save()
 
     def get_code(self) -> Tuple[str, str]:
         import_code = ""
         results = None
         def code(my_mesh_params):  # pragma: no cover
             # define the parameters to generate the solver mesh and interpolate the piv mesh onto it
-            params = my_mesh_params
+            mesh_parameters = my_mesh_params
 
             # iterate over all the results objects
             for result in results:
                 # correct for the reference state
-                displacement_list = saenopy.subtract_reference_state(result.mesh_piv, params["reference_stack"])
+                displacement_list = saenopy.subtract_reference_state(result.mesh_piv, mesh_parameters["reference_stack"])
                 # set the parameters
-                result.interpolate_parameter = params
+                result.mesh_parameters = mesh_parameters
                 # iterate over all stack pairs
                 for i in range(len(result.mesh_piv)):
                     # and create the interpolated solver mesh
-                    result.solver[i] = saenopy.interpolate_mesh(result.mesh_piv[i], displacement_list[i], params)
+                    result.solvers[i] = saenopy.interpolate_mesh(result.mesh_piv[i], displacement_list[i], mesh_parameters)
                 # save the meshes
                 result.save()
         data = {
-            "my_mesh_params": self.result.interpolate_parameter_tmp,
+            "my_mesh_params": self.result.mesh_parameters_tmp,
         }
 
         code = get_code(code, data)
         return import_code, code
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/PipelineModule.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/PipelineModule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,79 @@
 import qtawesome as qta
 from qtpy import QtCore, QtWidgets
 from saenopy import Result
-from typing import Tuple
+from typing import Tuple, List
 import traceback
 
 
+class ParameterMapping:
+    params_name: str = None
+    parameter_dict: dict = None
+
+    result: Result = None
+
+    def __init__(self, params_name: str = None, parameter_dict: dict=None):
+        self.params_name = params_name
+        self.parameter_dict = parameter_dict
+        for name, widget in self.parameter_dict.items():
+            widget.valueChanged.connect(lambda x, name=name: self.setParameter(name, x))
+
+        self.setResult(None)
+
+    def setParameter(self, name: str, value):
+        if self.result is not None:
+            getattr(self.result, self.params_name + "_tmp")[name] = value
+
+    def ensure_tmp_params_initialized(self, result):
+        if self.params_name is None:
+            return
+        # if the results instance does not have the parameter dictionary yet, create it
+        if getattr(result, self.params_name + "_tmp", None) is None:
+            setattr(result, self.params_name + "_tmp", {})
+
+        # set the widgets to the value if the value exits
+        params = getattr(result, self.params_name)
+        params_tmp = getattr(result, self.params_name + "_tmp")
+        # iterate over the parameters
+        for name, widget in self.parameter_dict.items():
+            if name not in params_tmp:
+                if params is not None and name in params:
+                    params_tmp[name] = params[name]
+                else:
+                    params_tmp[name] = widget.value()
+
+    def setDisabled(self, disabled):
+        # disable all the widgets
+        for name, widget in self.parameter_dict.items():
+            widget.setDisabled(disabled)
+
+    def setResult(self, result: Result):
+        """ set a new active result object """
+        self.result = result
+
+        # if a result file is given
+        if result is not None:
+            self.ensure_tmp_params_initialized(result)
+            params_tmp = getattr(result, self.params_name + "_tmp")
+            # iterate over the parameters
+            for name, widget in self.parameter_dict.items():
+                # set the widgets to the value if the value exits
+                widget.setValue(params_tmp[name])
+
+
 class PipelineModule(QtWidgets.QWidget):
     processing_finished = QtCore.Signal()
     processing_progress = QtCore.Signal(tuple)
     processing_state_changed = QtCore.Signal(object)
     processing_error = QtCore.Signal(str)
     result: Result = None
     tab: QtWidgets.QTabWidget = None
-    params_name: str = None
-    parameter_dict: dict = None
+
+    parameter_mappings: List[ParameterMapping] = None
+    params_name: None
 
     def __init__(self, parent: "BatchEvaluate", layout):
         super().__init__()
         if layout is not None:
             layout.addWidget(self)
         if parent is None:
             return
@@ -30,21 +86,22 @@
 
         self.parent.result_changed.connect(self.resultChanged)
         self.parent.set_current_result.connect(self.setResult)
         self.parent.tab_changed.connect(self.tabChanged)
 
         self.processing_progress.connect(self.parent.progress)
 
+        self.parameter_mappings = []
+        self.params_name = None
+
     def setParameterMapping(self, params_name: str = None, parameter_dict: dict=None):
         self.params_name = params_name
-        self.parameter_dict = parameter_dict
-        for name, widget in self.parameter_dict.items():
-            widget.valueChanged.connect(lambda x, name=name: self.setParameter(name, x))
-
-        self.setResult(None)
+        if params_name is None:
+            return
+        self.parameter_mappings.append(ParameterMapping(params_name, parameter_dict))
 
     current_result_plotted = False
     current_tab_selected = False
     def tabChanged(self, tab):
         if self.tab is not None and self.tab.parent() == tab:
             self.current_tab_selected = True
             if self.current_result_plotted is False:
@@ -87,36 +144,39 @@
                 self.group.label.setToolTip("failed")
             else:
                 self.group.label.setIcon(qta.icon("fa5.circle", options=[dict(color="gray")]))
                 self.group.label.setToolTip("")
 
             if state == "scheduled" or state == "running":
                 # if not disable all the widgets
-                for name, widget in self.parameter_dict.items():
-                    widget.setDisabled(True)
+                for mapping in self.parameter_mappings:
+                    mapping.setDisabled(True)
                 if getattr(self, "input_button", None):
                     self.input_button.setEnabled(False)
             else:
                 # if not disable all the widgets
-                for name, widget in self.parameter_dict.items():
-                    widget.setDisabled(False)
+                for mapping in self.parameter_mappings:
+                    mapping.setDisabled(False)
                 if getattr(self, "input_button", None):
                     self.input_button.setEnabled(self.check_available(result))
             #if getattr(self, "input_button", None):
             #    self.input_button.setEnabled(self.check_available(result))
 
     def setResult(self, result: Result):
         """ set a new active result object """
         #if result == self.result:
         #    return
         self.current_result_plotted = False
         self.result = result
 
+        for mapping in self.parameter_mappings:
+            mapping.setResult(result)
+
         if result is not None:
-            self.t_slider.setRange(0, len(result.stack)-2)
+            self.t_slider.setRange(0, len(result.stacks) - 2)
 
         self.state_changed(result)
         if self.tab is not None:
             for i in range(self.parent.tabs.count()):
                 if self.parent.tabs.widget(i) == self.tab.parent():
                     self.parent.tabs.setTabEnabled(i, self.check_evaluated(result))
 
@@ -124,81 +184,59 @@
         #if self.check_available(result) is False:
         if getattr(self, "input_button", None):
             self.input_button.setEnabled(self.check_available(result))
         if result is None or \
                 (self.params_name and (getattr(result, self.params_name + "_state", "") == "scheduled"
                                        or getattr(result, self.params_name + "_state", "") == "running")):
             # if not disable all the widgets
-            for name, widget in self.parameter_dict.items():
-                widget.setDisabled(True)
+            for mapping in self.parameter_mappings:
+                mapping.setDisabled(True)
             if getattr(self, "input_button", None):
                 self.input_button.setEnabled(False)
         else:
-            self.ensure_tmp_params_initialized(result)
-            # iterate over the parameters
-            for name, widget in self.parameter_dict.items():
-                # enable them
-                widget.setDisabled(False)
-                # set the widgets to the value if the value exits
-                params_tmp = getattr(result, self.params_name + "_tmp")
-                widget.setValue(params_tmp[name])
+            # if not disable all the widgets
+            for mapping in self.parameter_mappings:
+                mapping.setDisabled(False)
             self.valueChanged()
         if self.current_tab_selected is True:
             self.update_display()
 
     def update_display(self):
         pass
 
-    def setParameter(self, name: str, value):
-        if self.result is not None:
-            getattr(self.result, self.params_name + "_tmp")[name] = value
-
     def valueChanged(self):
         pass
 
-    def ensure_tmp_params_initialized(self, result):
-        if self.params_name is None:
-            return
-        # if the results instance does not have the parameter dictionary yet, create it
-        if getattr(result, self.params_name + "_tmp", None) is None:
-            setattr(result, self.params_name + "_tmp", {})
-        # iterate over the parameters
-        for name, widget in self.parameter_dict.items():
-            # set the widgets to the value if the value exits
-            params = getattr(result, self.params_name, None)
-            params_tmp = getattr(result, self.params_name + "_tmp")
-            if name not in params_tmp:
-                if params is not None and name in params:
-                    params_tmp[name] = params[name]
-                else:
-                    params_tmp[name] = widget.value()
-
     def start_process(self, x=None, result=None):
         if result is None:
             result = self.result
         if result is None:
             return
         if getattr(result, self.params_name + "_state", "") == "scheduled" or \
             getattr(result, self.params_name + "_state", "") == "running":
             return
-        self.ensure_tmp_params_initialized(result)
-        params = getattr(result, self.params_name + "_tmp")
+
+        params = {}
+        for mapping in self.parameter_mappings:
+            mapping.ensure_tmp_params_initialized(result)
+            params[mapping.params_name] = getattr(result, mapping.params_name + "_tmp")
         setattr(result, self.params_name + "_state", "scheduled")
         self.processing_state_changed.emit(result)
         return self.parent.addTask(self.process_thread, result, params, "xx")
 
     def process_thread(self, result: Result, params: dict):
         #params = getattr(result, self.params_name + "_tmp")
         self.parent.progressbar.setRange(0, 0)
         setattr(result, self.params_name + "_state", "running")
         self.processing_state_changed.emit(result)
         try:
-            self.process(result, params)
+            self.process(result, **params)
             # store the parameters that have been used for evaluation
-            setattr(result, self.params_name, params.copy())
+            for mapping in self.parameter_mappings:
+                setattr(result, mapping.params_name, params[mapping.params_name].copy())
             result.save()
             setattr(result, self.params_name + "_state", "finished")
             self.parent.result_changed.emit(result)
             self.processing_finished.emit()
         except Exception as err:
             traceback.print_exc()
             setattr(result, self.params_name + "_state", "failed")
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/QTimeSlider.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/QTimeSlider.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/Regularizer.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/Regularizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from qtpy import QtCore, QtWidgets
 import numpy as np
 from pyvistaqt import QtInteractor
 import inspect
 from typing import Tuple
 
 import saenopy
-import saenopy.multigridHelper
+import saenopy.multigrid_helper
 from saenopy import Result
-import saenopy.getDeformations
+import saenopy.get_deformations
 import saenopy.materials
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.common.gui_classes import CheckAbleGroup, MatplotlibWidget, NavigationToolbar
 
 from .PipelineModule import PipelineModule
 from .QTimeSlider import QTimeSlider
 from .VTK_Toolbar import VTK_Toolbar
@@ -33,25 +33,25 @@
             layout.setContentsMargins(0, 0, 0, 0)
             with CheckAbleGroup(self, "fit forces (regularize)", url="https://saenopy.readthedocs.io/en/latest/interface_solver.html#fit-deformations-and-calculate-forces").addToLayout() as self.group:
 
                 with QtShortCuts.QVBoxLayout() as main_layout:
                     with QtShortCuts.QGroupBox(None, "Material Parameters") as self.material_parameters:
                         with QtShortCuts.QHBoxLayout() as layout2:
                             self.input_k = QtShortCuts.QInputString(None, "k", "1645", type=float, tooltip="the stiffness of the material's fibers")
-                            self.input_d0 = QtShortCuts.QInputString(None, "d_0", "0.0008", type=float, tooltip="the bluckling strength of the material's fibers")
+                            self.input_d_0 = QtShortCuts.QInputString(None, "d_0", "0.0008", type=float, tooltip="the bluckling strength of the material's fibers")
                             self.input_lamda_s = QtShortCuts.QInputString(None, "λ_s", "0.0075", type=float, tooltip="the length at which strain stiffening of the material's fibers starts")
-                            self.input_ds = QtShortCuts.QInputString(None, "d_s", "0.033", type=float, tooltip="the strain stiffening strength of the material's fibers")
+                            self.input_d_s = QtShortCuts.QInputString(None, "d_s", "0.033", type=float, tooltip="the strain stiffening strength of the material's fibers")
 
                     with QtShortCuts.QGroupBox(None, "Regularisation Parameters") as self.material_parameters:
                         with QtShortCuts.QHBoxLayout(None) as layout:
                             self.input_alpha = QtShortCuts.QInputString(None, "alpha", "1e10", type="exp", tooltip="the strength of the regularisation (higher values mean weaker forces)")
-                            self.input_stepper = QtShortCuts.QInputString(None, "stepper", "0.33", type=float, tooltip="the step with of the iteration algorithm")
+                            self.input_step_size = QtShortCuts.QInputString(None, "step size", "0.33", type=float, tooltip="the step with of the iteration algorithm")
                         with QtShortCuts.QHBoxLayout(None) as layout:
-                            self.input_imax = QtShortCuts.QInputNumber(None, "i_max", 100, float=False, tooltip="the maximum number of iterations after which to abort the iteration algorithm")
-                            self.input_conv_crit = QtShortCuts.QInputString(None, "rel_conv_crit", 0.01, type=float, tooltip="the convergence criterion of the iteration algorithm")
+                            self.input_imax = QtShortCuts.QInputNumber(None, "max iterations", 100, float=False, tooltip="the maximum number of iterations after which to abort the iteration algorithm")
+                            self.input_conv_crit = QtShortCuts.QInputString(None, "rel. conv. crit.", 0.01, type=float, tooltip="the convergence criterion of the iteration algorithm")
 
                     self.input_button = QtShortCuts.QPushButton(None, "calculate forces", self.start_process, tooltip="run the force calculation")
 
                     self.canvas = MatplotlibWidget(self).addToLayout()
                     #NavigationToolbar(self.canvas, self).addToLayout()
 
         with self.parent.tabs.createTab("Forces") as self.tab:
@@ -71,44 +71,46 @@
                     parent.shared_properties.add_property("z_slider", self)
 
                 self.vtk_toolbar = VTK_Toolbar(self.plotter, self.update_display, center=True, shared_properties=self.parent.shared_properties).addToLayout()
 
                 self.t_slider = QTimeSlider(connected=self.update_display).addToLayout()
                 self.tab.parent().t_slider = self.t_slider
 
-        self.setParameterMapping("solve_parameter", {
+        self.setParameterMapping("material_parameters", {
             "k": self.input_k,
-            "d0": self.input_d0,
+            "d_0": self.input_d_0,
             "lambda_s": self.input_lamda_s,
-            "ds": self.input_ds,
+            "d_s": self.input_d_s,
+        })
+        self.setParameterMapping("solve_parameters", {
             "alpha": self.input_alpha,
-            "stepper": self.input_stepper,
-            "i_max": self.input_imax,
+            "step_size": self.input_step_size,
+            "max_iterations": self.input_imax,
             "rel_conv_crit": self.input_conv_crit,
         })
 
         self.iteration_finished.connect(self.iteration_callback)
         self.iteration_finished.emit(None, np.ones([10, 3]), 0, None)
 
     def z_slider_value_changed(self):
         self.update_display()
 
     def check_available(self, result: Result):
         try:
-            return self.result.solver[0] is not None
+            return self.result.solvers[0] is not None
         except (AttributeError, IndexError, TypeError):
             return False
 
     def check_evaluated(self, result: Result) -> bool:
         try:
-            if self.result is not None and self.result.solver is not None:
-                relrec = getattr(self.result.solver[self.t_slider.value()], "relrec", None)
+            if self.result is not None and self.result.solvers is not None:
+                relrec = getattr(self.result.solvers[self.t_slider.value()], "relrec", None)
                 if relrec is not None:
                     return True
-            return getattr(self.result.solver[0], "regularisation_results", None) is not None
+            return getattr(self.result.solvers[0], "regularisation_results", None) is not None
         except (AttributeError, IndexError, TypeError):
             return False
 
     def iteration_callback(self, result, relrec, i=0, imax=None):
         if imax is not None:
             self.parent.progressbar.setRange(0, imax)
             self.parent.progressbar.setValue(i)
@@ -132,57 +134,57 @@
                 self.canvas.figure.axes[0].text(1, 0, "\n\niteration", ha="right", va="center", transform=self.canvas.figure.axes[0].transAxes)
                 try:
                     self.canvas.figure.tight_layout(pad=0)
                 except np.linalg.LinAlgError:
                     pass
                 self.canvas.draw()
 
-    def process(self, result: Result, params: dict):
+    def process(self, result: Result, material_parameters: dict, solve_parameters: dict):
         # demo run
         if os.environ.get("DEMO") == "true":
             imax = 100
             self.parent.progressbar.setRange(0, imax)
             for i in range(len(result.solver_relrec_demo)):
                 time.sleep(0.2)
                 self.iteration_finished.emit(result, result.solver_relrec_demo[:i], i, imax)
-            result.solver[0].regularisation_results = result.solver_relrec_demo
+            result.solvers[0].regularisation_results = result.solver_relrec_demo
             return
 
-        for i in range(len(result.solver)):
-            M = result.solver[i]
+        for i in range(len(result.solvers)):
+            M = result.solvers[i]
 
             def callback(M, relrec, i, imax):
                 self.iteration_finished.emit(result, relrec, i, imax)
 
-            M.setMaterialModel(saenopy.materials.SemiAffineFiberMaterial(
-                               params["k"],
-                               params["d0"] if params["d0"] != "None" else None,
-                               params["lambda_s"] if params["lambda_s"] != "None" else None,
-                               params["ds"] if params["ds"] != "None" else None,
+            M.set_material_model(saenopy.materials.SemiAffineFiberMaterial(
+                               material_parameters["k"],
+                               material_parameters["d_0"] if material_parameters["d_0"] != "None" else None,
+                               material_parameters["lambda_s"] if material_parameters["lambda_s"] != "None" else None,
+                               material_parameters["d_s"] if material_parameters["d_s"] != "None" else None,
                                ))
 
-            M.solve_regularized(stepper=params["stepper"], i_max=params["i_max"],
-                                alpha=params["alpha"], rel_conv_crit=params["rel_conv_crit"],
+            M.solve_regularized(step_size=solve_parameters["step_size"], max_iterations=solve_parameters["max_iterations"],
+                                alpha=solve_parameters["alpha"], rel_conv_crit=solve_parameters["rel_conv_crit"],
                                 callback=callback, verbose=True)
 
             # clear the cache of the solver
             result.clear_cache(i)
 
     def property_changed(self, name, value):
         if name == "z_slider":
             self.z_slider.setValue(value)
 
     def setResult(self, result: Result):
         super().setResult(result)
-        if result and result.stack and result.stack[0]:
-            self.z_slider.setRange(0, result.stack[0].shape[2] - 1)
-            self.z_slider.setValue(self.result.stack[0].shape[2] // 2)
+        if result and result.stacks and result.stacks[0]:
+            self.z_slider.setRange(0, result.stacks[0].shape[2] - 1)
+            self.z_slider.setValue(self.result.stacks[0].shape[2] // 2)
 
-            if result.stack[0].channels:
-                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stack[0].channels)), result.stack[0].channels)
+            if result.stacks[0].channels:
+                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stacks[0].channels)), result.stacks[0].channels)
                 self.vtk_toolbar.channel_select.setVisible(True)
             else:
                 self.vtk_toolbar.channel_select.setValue(0)
                 self.vtk_toolbar.channel_select.setVisible(False)
 
     def update_display(self):
         if self.current_tab_selected is False:
@@ -190,75 +192,77 @@
             return
 
         if self.check_evaluated(self.result):
             cam_pos = None
             if self.plotter.camera_position is not None and CamPos.cam_pos_initialized is True:
                 cam_pos = self.plotter.camera_position
             CamPos.cam_pos_initialized = True
-            self.plotter.interactor.setToolTip(str(self.result.solve_parameter)+f"\nNodes {self.result.solver[self.t_slider.value()].R.shape[0]}\nTets {self.result.solver[self.t_slider.value()].T.shape[0]}")
-            M = self.result.solver[self.t_slider.value()]
+            M = self.result.solvers[self.t_slider.value()]
+            mesh = M.mesh
+            self.plotter.interactor.setToolTip(str(self.result.solve_parameters) + f"\nNodes {mesh.nodes.shape[0]}\nTets {mesh.tetrahedra.shape[0]}")
             center = None
             if self.vtk_toolbar.use_center.value() is True:
-                center = M.getCenter(mode="Force")
+                center = M.get_center(mode="Force")
             display_image = getVectorFieldImage(self)
-            if len(self.result.stack):
-                stack_shape = np.array(self.result.stack[0].shape[:3]) * np.array(self.result.stack[0].voxel_size)
+            if len(self.result.stacks):
+                stack_shape = np.array(self.result.stacks[0].shape[:3]) * np.array(self.result.stacks[0].voxel_size)
             else:
                 stack_shape = None
                 
-            if M.reg_mask is not None:
-                f =  -M.f * M.reg_mask[:, None]   
+            if M.mesh.regularisation_mask is not None:
+                f = -M.mesh.forces * M.mesh.regularisation_mask[:, None]
             else:
-                f =  -M.f
+                f =  -M.mesh.forces
                 
-            showVectorField(self.plotter, M, f, "f", center=center,
+            showVectorField(self.plotter, M.mesh, f, "forces", center=center,
                             factor=0.15 * self.vtk_toolbar.arrow_scale.value(),
                             colormap=self.vtk_toolbar.colormap_chooser.value(),
                             colormap2=self.vtk_toolbar.colormap_chooser2.value(),
                             scalebar_max=self.vtk_toolbar.getScaleMax(), show_nan=self.vtk_toolbar.use_nans.value(),
                             display_image=display_image, show_grid=self.vtk_toolbar.show_grid.value(),
                             stack_shape=stack_shape)
             if cam_pos is not None:
                 self.plotter.camera_position = cam_pos
-            relrec = getattr(self.result.solver[self.t_slider.value()], "relrec", None)
+            relrec = getattr(self.result.solvers[self.t_slider.value()], "relrec", None)
             if relrec is None:
-                relrec = self.result.solver[self.t_slider.value()].regularisation_results
+                relrec = self.result.solvers[self.t_slider.value()].regularisation_results
             self.iteration_callback(self.result, relrec)
         else:
             self.plotter.interactor.setToolTip("")
 
     def get_code(self) -> Tuple[str, str]:
         import_code = "import saenopy\n"
         results: Result = None
-        def code(my_reg_params):  # pragma: no cover
+        def code(my_reg_params1, my_reg_params2):  # pragma: no cover
             # define the parameters to generate the solver mesh and interpolate the piv mesh onto it
-            params = my_reg_params
+            material_parameters = my_reg_params1
+            solve_parameters = my_reg_params2
 
             # iterate over all the results objects
             for result in results:
-                result.solve_parameter = params
-                for index, M in enumerate(result.solver):
+                result.mesh_parameters = material_parameters
+                result.solve_parameters = solve_parameters
+                for index, M in enumerate(result.solvers):
                     # set the material model
-                    M.setMaterialModel(saenopy.materials.SemiAffineFiberMaterial(
-                        params["k"],
-                        params["d0"],
-                        params["lambda_s"],
-                        params["ds"],
+                    M.set_material_model(saenopy.materials.SemiAffineFiberMaterial(
+                        material_parameters["k"],
+                        material_parameters["d_0"],
+                        material_parameters["lambda_s"],
+                        material_parameters["ds"],
                     ))
                     # find the regularized force solution
-                    M.solve_regularized(stepper=params["stepper"], i_max=params["i_max"], alpha=params["alpha"], rel_conv_crit=params["rel_conv_crit"], verbose=True)
+                    M.solve_regularized(alpha=solve_parameters["alpha"], step_size=solve_parameters["step_size"],
+                                        max_iterations=solve_parameters["max_iterations"], rel_conv_crit=solve_parameters["rel_conv_crit"],
+                                        verbose=True)
                     # save the forces
                     result.save()
                     # clear the cache of the solver
                     result.clear_cache(index)
 
-        params = self.result.solve_parameter_tmp
-        # convert text Nones to real Nones
-        for name in params:
-            if params[name] == "None":
-                params[name] = None
+        # params with convert text Nones to real Nones
         data = {
-            "my_reg_params": params,
+            "my_reg_params1": {k: None if v == "None" else v for k, v in self.result.material_parameters_tmp.items()},
+            "my_reg_params2": {k: None if v == "None" else v for k, v in self.result.solve_parameters_tmp.items()},
         }
 
         code = get_code(code, data)
         return import_code, code
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/ResultView.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/ResultView.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         super().__init__(parent, layout)
         result_view = self
 
         with self.parent.tabs.createTab("View") as self.tab:
             with QtShortCuts.QVBoxLayout() as vlayout:
                 with QtShortCuts.QHBoxLayout() as layout_vert_plot:
                     self.input_checks = {}
-                    for name, dislay_name in {"U_target": "Target Deformations", "U": "Fitted Deformations", "f": "Forces", "stiffness": "Stiffness"}.items():
+                    for name, dislay_name in {"displacements_target": "Target Deformations", "displacements": "Fitted Deformations", "forces": "Forces", "stiffness": "Stiffness"}.items():
                         input_bool = QtShortCuts.QInputBool(layout_vert_plot, dislay_name, name != "stiffness")
                         input_bool.valueChanged.connect(self.replot)
                         self.input_checks[name] = input_bool
                     layout_vert_plot.addStretch()
                     self.button_export = QtWidgets.QPushButton(qta.icon("mdi.floppy"), "")
                     self.button_export.setToolTip("save image")
                     layout_vert_plot.addWidget(self.button_export)
@@ -45,61 +45,61 @@
 
                 self.plotter = QtInteractor(self.frame, auto_update=False)
                 self.plotter_layout.addWidget(self.plotter.interactor)
                 #vlayout.addLayout(self.plotter_layout)
                 #return
                 self.t_slider = QTimeSlider(connected=self.update_display).addToLayout()
                 self.tab.parent().t_slider = self.t_slider
-        self.setParameterMapping(None, {})
 
     def check_evaluated(self, result: Result) -> bool:
         try:
-            return getattr(self.result.solver[0], "regularisation_results", None) is not None
+            return getattr(self.result.solvers[0], "regularisation_results", None) is not None
         except (AttributeError, IndexError, TypeError):
             return False
 
     def update_display(self):
         if self.check_evaluated(self.result):
-            self.M = self.result.solver[self.t_slider.value()]
-            R = self.M.R
+            self.M = self.result.solvers[self.t_slider.value()]
+            mesh = self.M.mesh
+            R = mesh.nodes
             minR = np.min(R, axis=0)
             maxR = np.max(R, axis=0)
 
-            if self.M.reg_mask is None:
+            if mesh.regularisation_mask is None:
                 border = (R[:, 0] < minR[0] + 0.5e-6) | (R[:, 0] > maxR[0] - 0.5e-6) | \
                          (R[:, 1] < minR[1] + 0.5e-6) | (R[:, 1] > maxR[1] - 0.5e-6) | \
                          (R[:, 2] < minR[2] + 0.5e-6) | (R[:, 2] > maxR[2] - 0.5e-6)
-                self.M.reg_mask = ~border
+                mesh.regularisation_mask = ~border
 
-            self.point_cloud = pv.PolyData(self.M.R)
-            self.point_cloud.point_data["f"] = -self.M.f * self.M.reg_mask[:, None]
-            self.point_cloud["f_mag"] = np.linalg.norm(self.M.f * self.M.reg_mask[:, None], axis=1)
-            self.point_cloud.point_data["U"] = self.M.U
-            self.point_cloud["U_mag"] = np.linalg.norm(self.M.U, axis=1)
-            self.point_cloud.point_data["U_target"] = self.M.U_target
-            self.point_cloud["U_target_mag"] = np.linalg.norm(self.M.U_target, axis=1)
-            nan_values = np.isnan(self.M.U_target[:, 0])
-            self.point_cloud["U_target_mag"][nan_values] = 0
+            self.point_cloud = pv.PolyData(mesh.nodes)
+            self.point_cloud.point_data["forces"] = -mesh.forces * mesh.regularisation_mask[:, None]
+            self.point_cloud["forces_mag"] = np.linalg.norm(mesh.forces * mesh.regularisation_mask[:, None], axis=1)
+            self.point_cloud.point_data["displacements"] = mesh.displacements
+            self.point_cloud["displacements_mag"] = np.linalg.norm(mesh.displacements, axis=1)
+            self.point_cloud.point_data["displacements_target"] = mesh.displacements_target
+            self.point_cloud["displacements_target_mag"] = np.linalg.norm(mesh.displacements_target, axis=1)
+            nan_values = np.isnan(mesh.displacements_target[:, 0])
+            self.point_cloud["displacements_target_mag"][nan_values] = 0
 
             self.point_cloud2 = None
 
-            self.offset = np.min(self.M.R, axis=0)
+            self.offset = np.min(mesh.nodes, axis=0)
             self.replot()
         else:
             self.plotter.interactor.setToolTip("")
 
     def calculateStiffness(self):
-        self.point_cloud2 = pv.PolyData(np.mean(self.M.R[self.M.T], axis=1))
+        self.point_cloud2 = pv.PolyData(np.mean(self.M.mesh.nodes[self.M.mesh.tetrahedra], axis=1))
         # self.M.setMaterialModel(SemiAffineFiberMaterial(1645, 0.0008, 0.0075, 0.033), generate_lookup=False)
         if self.M.material_model is None:
             print("Warning using default material parameters")
-            self.M.setMaterialModel(SemiAffineFiberMaterial(1449, 0.00215, 0.055, 0.032), generate_lookup=False)
+            self.M.set_material_model(SemiAffineFiberMaterial(1449, 0.00215, 0.055, 0.032), generate_lookup=False)
         self.M._check_relax_ready()
         self.M._prepare_temporary_quantities()
-        self.point_cloud2["stiffness"] = self.M.getMaxTetStiffness() / 6
+        self.point_cloud2["stiffness"] = self.M.get_max_tet_stiffness() / 6
 
     point_cloud = None
 
     theme = None
     def setTheme(self, x):
         self.theme = x
         self.current_result_plotted = False
@@ -127,71 +127,71 @@
             self.plotter.set_background(self.theme.background)
 
         plotter = self.plotter
         # force rendering to be disabled while updating content to prevent flickering
         render = plotter.render
         plotter.render = lambda *args: None
         try:
-            xmin, ymin, zmin = self.M.R.min(axis=0)
-            xmax, ymax, zmax = self.M.R.max(axis=0)
+            xmin, ymin, zmin = self.M.mesh.nodes.min(axis=0)
+            xmax, ymax, zmax = self.M.mesh.nodes.max(axis=0)
             # color bar design properties
             # Set a custom position and size
             sargs = dict(#position_x=0.05, position_y=0.95,
                          title_font_size=15,
                          label_font_size=9,
                          n_labels=3,
                          #italic=True,  ##height=0.25, #vertical=True,
                          fmt="%.1e",
                          font_family="arial")
 
             for i, name in enumerate(names):
                 plotter.subplot(i // plotter.shape[1], i % plotter.shape[1])
                 # scale plot with axis length later
-                norm_stack_size = np.abs(np.max(self.M.R) - np.min(self.M.R))
+                norm_stack_size = np.abs(np.max(self.M.mesh.nodes) - np.min(self.M.mesh.nodes))
 
                 if name == "stiffness":
                     if self.point_cloud2 is None:
                         self.calculateStiffness()
                     # clim =  np.nanpercentile(self.point_cloud2["stiffness"], [50, 99.9])
                     sargs2 = sargs.copy()
                     sargs2["title"] = "Stiffness (Pa)"
                     plotter.add_mesh(self.point_cloud2, colormap="turbo", point_size=4., render_points_as_spheres=True,
                                      scalar_bar_args=sargs2, opacity="linear")
                     plotter.update_scalar_bar_range(np.nanpercentile(self.point_cloud2["stiffness"], [50, 99.9]))
-                elif name == "f":
-                    arrows = self.point_cloud.glyph(orient="f", scale="f_mag",
+                elif name == "forces":
+                    arrows = self.point_cloud.glyph(orient="forces", scale="forces_mag",
                                                     # Automatically scale maximal force to 15% of axis length
                                                     factor=0.15 * norm_stack_size / np.nanmax(
-                                                        np.linalg.norm(self.M.f * self.M.reg_mask[:, None], axis=1)))
+                                                        np.linalg.norm(self.M.mesh.forces * self.M.mesh.regularisation_mask[:, None], axis=1)))
                     sargs2 = sargs.copy()
                     sargs2["title"] = "Force (N)"
                     plotter.add_mesh(arrows, colormap='turbo', name="arrows", scalar_bar_args=sargs2)
-                    plotter.update_scalar_bar_range(np.nanpercentile(self.point_cloud["f_mag"], [50, 99.9]))
+                    plotter.update_scalar_bar_range(np.nanpercentile(self.point_cloud["forces_mag"], [50, 99.9]))
                     # plot center points if desired
                     # plotter.add_points(np.array([self.M.getCenter(mode="Force")]), color='r')
 
-                elif name == "U_target":
+                elif name == "displacements_target":
                     arrows2 = self.point_cloud.glyph(orient=name, scale=name + "_mag",
                                                      # Automatically scale maximal force to 10% of axis length
                                                      factor=0.1 * norm_stack_size / np.nanmax(
-                                                         np.linalg.norm(self.M.U_target, axis=1)))
+                                                         np.linalg.norm(self.M.mesh.displacements_target, axis=1)))
                     sargs2 = sargs.copy()
                     sargs2["title"] = "Deformations (m)"
                     plotter.add_mesh(arrows2, colormap='turbo', name="arrows2", scalar_bar_args=sargs2)  #
 
                     # plot center if desired
                     # plotter.add_points(np.array([self.M.getCenter(mode="deformation_target")]), color='w')
 
                     plotter.update_scalar_bar_range(np.nanpercentile(self.point_cloud[name + "_mag"], [50, 99.9]))
                     # plotter.update_scalar_bar_range([0,1.5e-6])
-                elif name == "U":
+                elif name == "displacements":
                     arrows3 = self.point_cloud.glyph(orient=name, scale=name + "_mag",
                                                      # Automatically scale maximal force to 10% of axis length
                                                      factor=0.1 * norm_stack_size / np.nanmax(
-                                                         np.linalg.norm(self.M.U, axis=1)))
+                                                         np.linalg.norm(self.M.mesh.displacements, axis=1)))
                     sargs2 = sargs.copy()
                     sargs2["title"] = "Fitted Deformations [m]"
                     plotter.add_mesh(arrows3, colormap='turbo', name="arrows3", scalar_bar_args=sargs2)
                     plotter.update_scalar_bar_range(np.nanpercentile(self.point_cloud[name + "_mag"], [50, 99.9]))
                     # plotter.update_scalar_bar_range([0,1.5e-6])
 
                 # plot center points if desired
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/StackDisplay.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/StackDisplay.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
+import traceback
+
 import qtawesome as qta
 from qtpy import QtCore, QtWidgets, QtGui
 import numpy as np
 
 from qimage2ndarray import array2qimage
 import imageio
 
 from pathlib import Path
 
 from typing import Tuple
 import tifffile
 
 import saenopy
-import saenopy.multigridHelper
+import saenopy.multigrid_helper
 from saenopy.gui.common import QtShortCuts, QExtendedGraphicsView
-import saenopy.getDeformations
-import saenopy.multigridHelper
+import saenopy.get_deformations
+import saenopy.multigrid_helper
 import saenopy.materials
 from saenopy import Result
 from saenopy.gui.common.resources import resource_icon
 
 
 from .PipelineModule import PipelineModule
 from .QTimeSlider import QTimeSlider
@@ -116,24 +118,23 @@
                         self.button2.clicked.connect(self.export)
 
                     self.t_slider = QTimeSlider(connected=self.z_slider_value_changed).addToLayout()
                     self.tab.parent().t_slider = self.t_slider
 
         self.view1.link(self.view2)
         self.current_tab_selected = True
-        self.setParameterMapping(None, {})
 
     def setZProj(self, value):
         if self.result:
             if value == 0:
-                self.result.stack_parameter["z_project_name"] = None
+                self.result.stack_parameters["z_project_name"] = None
             else:
-                self.result.stack_parameter["z_project_name"] = "maximum"
-            self.result.stack_parameter["z_project_range"] = value
-            self.result.stack_parameter["z_project_range"] = value
+                self.result.stack_parameters["z_project_name"] = "maximum"
+            self.result.stack_parameters["z_project_range"] = value
+            self.result.stack_parameters["z_project_range"] = value
             self.z_slider_value_changed()
 
     def setSingle(self, use_single):
         self.view_single = use_single
         self.view2.setVisible(not self.view_single)
         self.label1.setVisible(not self.view_single)
         self.label2.setVisible(not self.view_single)
@@ -145,18 +146,18 @@
         self.update_display()
 
     def viewSingleTimer(self):
         self.view_single_switch = 1-self.view_single_switch
         self.z_slider_value_changed()
 
     def check_evaluated(self, result: Result) -> bool:
-        return self.result is not None and result.stack is not None and len(result.stack) > 0
+        return self.result is not None and result.stacks is not None and len(result.stacks) > 0
 
     def check_available(self, result: Result) -> bool:
-        if result is not None and result.stack is not None and len(result.stack) > 0:
+        if result is not None and result.stacks is not None and len(result.stacks) > 0:
             return True
         return False
 
     def export(self):
         if self.result is None:
             return
         new_path = QtWidgets.QFileDialog.getSaveFileName(None, "Save Images", os.getcwd())
@@ -165,19 +166,23 @@
             new_path = new_path.strip(".gif").strip("_relaxed.tif").strip("_deformed.tif")
             new_path = Path(new_path)
             print(new_path.parent / (new_path.stem + "_deformed.tif"))
             t = self.t_slider.value()
             z = self.z_slider.value()
             c = self.channel_select.value()
             if self.result.stack_reference is not None:
-                stack1, stack2 = self.result.stack_reference[:, :, :, z, c], self.result.stack[t][:, :, :, z, c]
+                stack1, stack2 = self.result.stack_reference[:, :, :, z, c], self.result.stacks[t][:, :, :, z, c]
             else:
-                stack1, stack2 = self.result.stack[t][:, :, :, z, c], self.result.stack[t + 1][:, :, :, z, c]
-            tifffile.imsave(new_path.parent / (new_path.stem + "_relaxed.tif"), stack1)
-            tifffile.imsave(new_path.parent / (new_path.stem + "_deformed.tif"), stack2)
+                stack1, stack2 = self.result.stacks[t][:, :, :, z, c], self.result.stacks[t + 1][:, :, :, z, c]
+            tifffile.imwrite(new_path.parent / (new_path.stem + "_relaxed.tif"), stack1)
+            tifffile.imwrite(new_path.parent / (new_path.stem + "_deformed.tif"), stack2)
+            if len(stack1.shape) == 3 and stack1.shape[2] == 1:
+                stack1 = stack1[:, :, 0]
+            if len(stack2.shape) == 3 and stack2.shape[2] == 1:
+                stack2 = stack2[:, :, 0]
             imageio.mimsave(new_path.parent / (new_path.stem + ".gif"), [stack1, stack2], duration=1000 * 1./2)
 
     def update_display(self):
         return
 
     def property_changed(self, name, value):
         if name == "z_slider":
@@ -198,56 +203,63 @@
         if name == "contrast_enhance":
             if value != self.contrast_enhance.value():
                 self.contrast_enhance.setValue(value)
                 self.update_display()
 
     def setResult(self, result: Result):
         super().setResult(result)
-        if result and result.stack and result.stack[0]:
-            self.z_slider.setRange(0, result.stack[0].shape[2] - 1)
-            self.z_slider.setValue(self.result.stack[0].shape[2] // 2)
+        if result and result.stacks and result.stacks[0]:
+            self.z_slider.setRange(0, result.stacks[0].shape[2] - 1)
+            self.z_slider.setValue(self.result.stacks[0].shape[2] // 2)
             self.z_slider_value_changed()
 
-            if result.stack[0].channels:
-                self.channel_select.setValues(np.arange(len(result.stack[0].channels)),
-                                                          result.stack[0].channels)
+            if result.stacks[0].channels:
+                self.channel_select.setValues(np.arange(len(result.stacks[0].channels)),
+                                              result.stacks[0].channels)
                 self.channel_select.setVisible(True)
             else:
                 self.channel_select.setValue(0)
                 self.channel_select.setVisible(False)
 
     def z_slider_value_changed(self):
-        if self.result is not None and len(self.result.stack):
+        if self.result is not None and len(self.result.stacks):
             for i in range(2 - self.view_single):
                 if self.result.stack_reference is not None:
                     if i + self.view_single_switch == 0:
                         stack = self.result.stack_reference
                     else:
-                        stack = self.result.stack[self.t_slider.value()]
+                        stack = self.result.stacks[self.t_slider.value()]
                 else:
-                    stack = self.result.stack[self.t_slider.value() + i + self.view_single_switch]
+                    stack = self.result.stacks[self.t_slider.value() + i + self.view_single_switch]
                 [self.scale1, self.scale2][i].setScale(stack.voxel_size)
 
                 c = self.channel_select.value()
                 z = self.z_slider.value()
 
-                self.views[i].setToolTip(f"stack\n{stack.description(z)}")
+                try:
+                    self.views[i].setToolTip(f"stack\n{stack.description(z)}")
 
-                if self.result.stack_parameter["z_project_name"] == "maximum":
-                    start = np.clip(z-self.result.stack_parameter["z_project_range"], 0, stack.shape[2])
-                    end = np.clip(z+self.result.stack_parameter["z_project_range"], 0, stack.shape[2])
-                    im = stack[:, :, :, start:end, c]
-                    im = np.max(im, axis=3)
-                else:
-                    im = stack[:, :, :, z, c]
-                if self.contrast_enhance.value():
-                    (min, max) = np.percentile(im, (1, 99))
-                    im = im.astype(np.float32)-min
-                    im = im.astype(np.float64) * 255 / (max-min)
-                    im = np.clip(im, 0, 255).astype(np.uint8)
+                    if self.result.stack_parameters["z_project_name"] == "maximum":
+                        start = np.clip(z - self.result.stack_parameters["z_project_range"], 0, stack.shape[2])
+                        end = np.clip(z + self.result.stack_parameters["z_project_range"], 0, stack.shape[2])
+                        im = stack[:, :, :, start:end, c]
+                        im = np.max(im, axis=3)
+                    else:
+                        im = stack[:, :, :, z, c]
+                    if self.contrast_enhance.value():
+                        (min, max) = np.percentile(im, (1, 99))
+                        im = im.astype(np.float32)-min
+                        im = im.astype(np.float64) * 255 / (max-min)
+                        im = np.clip(im, 0, 255).astype(np.uint8)
+                except FileNotFoundError as err:
+                    traceback.print_exception(err)
+                    im = np.zeros([255, 255, 3], dtype=np.uint8)
+                    im[:, :, 0] = 255
+                    im[:, :, 2] = 255
+                    self.views[i].setToolTip(f"stack information not found")
                 self.pixmaps[i].setPixmap(QtGui.QPixmap(array2qimage(im)))
                 self.views[i].setExtend(im.shape[1], im.shape[0])
                 self.parent.display_image = (im, stack.voxel_size)
 
             self.z_slider.setToolTip(f"set z position\ncurrent position {self.z_slider.value()}")
 
     def get_code(self) -> Tuple[str, str]:
@@ -273,16 +285,16 @@
                     # use * to load multiple result files for batch processing
                     # results = saenopy.load_results(result_file)
 
                 data = dict(
                     filename=self.result.template,
                     reference_stack1=self.result.stack_reference.template,
                     output1=str(Path(self.result.output).parent),
-                    voxel_size1=self.result.stack[0].voxel_size,
-                    crop1=self.result.stack[0].crop,
+                    voxel_size1=self.result.stacks[0].voxel_size,
+                    crop1=self.result.stacks[0].crop,
                     result_file=str(self.result.output),
                 )
         else:
             if self.result.stack_reference is not None:
                 def code(filename, reference_stack1, output1, voxel_size1, time_delta1, result_file, crop1):  # pragma: no cover
                     # load the relaxed and the contracted stack
                     # {z} is the placeholder for the z stack
@@ -303,16 +315,16 @@
                     # results = saenopy.load_results(result_file)
 
                 data = dict(
                     filename=self.result.template,
                     reference_stack1=self.result.stack_reference.template,
                     output1=str(Path(self.result.output).parent),
                     result_file=str(self.result.output),
-                    voxel_size1=self.result.stack[0].voxel_size,
-                    crop1=self.result.stack[0].crop,
+                    voxel_size1=self.result.stacks[0].voxel_size,
+                    crop1=self.result.stacks[0].crop,
                     time_delta1=self.result.time_delta,
                 )
             else:
                 def code(filename, output1, voxel_size1, time_delta1, result_file, crop1):  # pragma: no cover
                     # load the relaxed and the contracted stack
                     # {z} is the placeholder for the z stack
                     # {c} is the placeholder for the channels
@@ -329,17 +341,17 @@
                     # or if you want to explicitly load existing results files
                     # use * to load multiple result files for batch processing
                     # results = saenopy.load_results(result_file)
 
                 data = dict(
                     filename=self.result.template,
                     output1=str(Path(self.result.output).parent),
-                    voxel_size1=self.result.stack[0].voxel_size,
+                    voxel_size1=self.result.stacks[0].voxel_size,
                     time_delta1=self.result.time_delta,
-                    crop1=self.result.stack[0].crop,
+                    crop1=self.result.stacks[0].crop,
                     result_file=str(self.result.output),
                 )
 
         code = get_code(code, data)
         return import_code, code
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/VTK_Toolbar.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/VTK_Toolbar.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/code_export.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/code_export.py`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 import datetime
 import numpy as np
 
 
 def get_mesh_arrows(params, result):
     if params["arrows"] == "piv":
         if result is not None:
-            M = result.mesh_piv[params["time"]["t"]]
-            if M is not None and M.hasNodeVar("U_measured"):
-                return M, M.getNodeVar("U_measured"), params["deformation_arrows"], "U_measured"
+            mesh = result.mesh_piv[params["time"]["t"]]
+            if mesh is not None and mesh.displacements_measured is not None:
+                return mesh, mesh.displacements_measured, params["deformation_arrows"], "displacements_measured"
     elif params["arrows"] == "target deformations":
-        M = result.solver[params["time"]["t"]]
+        M = result.solvers[params["time"]["t"]]
         if M is not None:
-            return M, M.U_target, params["deformation_arrows"], "U_target"
+            return M.mesh, M.mesh.displacements_target, params["deformation_arrows"], "displacements_target"
     elif params["arrows"] == "fitted deformations":
-        M = result.solver[params["time"]["t"]]
+        M = result.solvers[params["time"]["t"]]
         if M is not None:
-            return M, M.U, params["deformation_arrows"], "U"
+            return M.mesh, M.mesh.displacements, params["deformation_arrows"], "displacements"
     elif params["arrows"] == "fitted forces":
-        M = result.solver[params["time"]["t"]]
+        M = result.solvers[params["time"]["t"]]
         if M is not None:
-            return M, -M.f * M.reg_mask[:, None], params["force_arrows"], "f"
+            return M.mesh, -M.mesh.forces * M.mesh.regularisation_mask[:, None], params["force_arrows"], "forces"
     return None, None, {}, ""
 
 
 def get_mesh_extent(params, result):
     if params["arrows"] == "piv":
-        M = result.mesh_piv[params["time"]["t"]]
-        if M is not None and M.hasNodeVar("U_measured"):
-            return [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+        mesh = result.mesh_piv[params["time"]["t"]]
+        if mesh is not None and mesh.displacements_measured is not None:
+            return [mesh.nodes.min(axis=0) * 1e6, mesh.nodes.max(axis=0) * 1e6]
     elif params["arrows"] == "target deformations":
-        M = result.solver[params["time"]["t"]]
+        M = result.solvers[params["time"]["t"]]
         if M is not None:
-            return [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+            return [M.mesh.nodes.min(axis=0) * 1e6, M.mesh.nodes.max(axis=0) * 1e6]
     elif params["arrows"] == "fitted deformations":
-        M = result.solver[params["time"]["t"]]
+        M = result.solvers[params["time"]["t"]]
         if M is not None:
-            return [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+            return [M.mesh.nodes.min(axis=0) * 1e6, M.mesh.nodes.max(axis=0) * 1e6]
     elif params["arrows"] == "fitted forces":
-        M = result.solver[params["time"]["t"]]
+        M = result.solvers[params["time"]["t"]]
         if M is not None:
-            return [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+            return [M.mesh.nodes.min(axis=0) * 1e6, M.mesh.nodes.max(axis=0) * 1e6]
     else:
-        M = result.solver[params["time"]["t"]]
+        M = result.solvers[params["time"]["t"]]
         if M is not None:
-            return [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+            return [M.mesh.nodes.min(axis=0) * 1e6, M.mesh.nodes.max(axis=0) * 1e6]
         else:
             M = result.mesh_piv[params["time"]["t"]]
             if M is not None:
-                return [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+                return [M.mesh.nodes.min(axis=0) * 1e6, M.mesh.nodes.max(axis=0) * 1e6]
     return None
 
 
 def getVectorFieldImage(result, params, use_fixed_contrast_if_available=False, use_2D=False, exporter=None):
     try:
         image = params["stack"]["image"]
         if use_2D:
             image = 1
-        if image and params["time"]["t"] < len(result.stack):
+        if image and params["time"]["t"] < len(result.stacks):
             if params["stack"]["use_reference_stack"] and result.stack_reference:
                 stack = result.stack_reference
             else:
-                stack = result.stack[params["time"]["t"]]
+                stack = result.stacks[params["time"]["t"]]
             channel = params["stack"]["channel"]
             if isinstance(channel, str):
-                channel = result.stack[0].channels.index(channel)
+                try:
+                    channel = result.stacks[0].channels.index(channel)
+                except ValueError:
+                    channel = 0
             if channel >= len(stack.channels):
                 im = stack[:, :, :, params["stack"]["z"], 0]
             else:
                 im = stack[:, :, :, params["stack"]["z"], channel]
             if params["stack"]["z_proj"]:
                 z_range = [0, 5, 10, 1000][params["stack"]["z_proj"]]
                 start = np.clip(params["stack"]["z"] - z_range, 0, stack.shape[2])
@@ -93,15 +96,14 @@
             display_image = None
     except FileNotFoundError:
         display_image = None
     return display_image
 
 
 def get_time_text(params, result):
-    print("time", float(params["time"]["t"] * result.time_delta) + params["time"]["start"], float(params["time"]["t"] * result.time_delta), params["time"]["start"])
     return formatTimedelta(datetime.timedelta(seconds=float(params["time"]["t"] * result.time_delta) + params["time"]["start"]),
                            params["time"]["format"])
 
 
 def formatTimedelta(t: datetime.timedelta, fmt: str) -> str:
     sign = 1
     if t.total_seconds() < 0:
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/exporter/Exporter.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/exporter/Exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -627,58 +627,59 @@
         with Writer(self.outputText3.value(), self.zscan_fps.value(), self) as writer:
             for t in self.progress_iterator(range(0, self.z_slider.t_slider.maximum() + 1, self.zscan_steps.value())):
                 self.z_slider.setValue(t)
                 self.update_display()
                 writer.write(self.im)
 
     def check_evaluated(self, result: Result) -> bool:
-        return self.result is not None and result.stack is not None and len(result.stack) > 0
+        return self.result is not None and result.stacks is not None and len(result.stacks) > 0
 
     def setResult(self, result: Result, no_update_display=False):
-        if result and result.stack and result.stack[0]:
-            self.z_slider.setRange(0, result.stack[0].shape[2] - 1)
-            self.z_slider.setValue(result.stack[0].shape[2] // 2)
+        self.result = result
+        if result and result.stacks and result.stacks[0]:
+            self.z_slider.setRange(0, result.stacks[0].shape[2] - 1)
+            self.z_slider.setValue(result.stacks[0].shape[2] // 2)
 
-            if result.stack[0].channels:
+            if result.stacks[0].channels:
                 value = self.vtk_toolbar.channel_select.value()
-                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stack[0].channels)), result.stack[0].channels)
+                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stacks[0].channels)), result.stacks[0].channels)
                 self.vtk_toolbar.channel_select.setValue(value)
                 self.vtk_toolbar.channel_select.setVisible(True)
 
                 value = self.channel_selectB.value()
-                self.channel_selectB.setValues([-1]+list(np.arange(len(result.stack[0].channels))),
-                                                          [""]+result.stack[0].channels)
+                self.channel_selectB.setValues([-1] + list(np.arange(len(result.stacks[0].channels))),
+                                               [""] + result.stacks[0].channels)
                 self.channel_selectB.setValue("")
                 self.channel_selectB.setVisible(True)
 
                 value = self.channel1_properties.channel_select.value()
-                self.channel1_properties.channel_select.setValues(np.arange(len(result.stack[0].channels))[1:],
-                                               result.stack[0].channels[1:])
+                self.channel1_properties.channel_select.setValues(np.arange(len(result.stacks[0].channels))[1:],
+                                                                  result.stacks[0].channels[1:])
                 self.channel1_properties.channel_select.setValue(value)
                 self.channel1_properties.channel_select.setVisible(True)
             else:
                 self.vtk_toolbar.channel_select.setValue(0)
                 self.vtk_toolbar.channel_select.setVisible(False)
                 self.channel_selectB.setVisible(False)
 
-            shape = result.stack[0].shape
+            shape = result.stacks[0].shape
             self.input_cropx.setRange(0, shape[1])
             self.input_cropx.setValue((shape[1] // 2 - 100, shape[1] // 2 + 100))
             self.input_cropy.setRange(0, shape[0])
             self.input_cropy.setValue((shape[0] // 2 - 100, shape[0] // 2 + 100))
             self.input_cropz.setRange(0, shape[2])
             self.input_cropz.setValue((shape[2] // 2 - 25, shape[2] // 2 + 25))
 
-            if result.stack[0].shape[-1] == 1:
+            if result.stacks[0].shape[-1] == 1:
                 self.channel1_properties.input_show.setValue(False)
                 self.channel1_properties.setDisabled(True)
             else:
                 self.channel1_properties.setDisabled(False)
 
-            self.input_average_range.setRange(0, shape[2]*result.stack[0].voxel_size[2])
+            self.input_average_range.setRange(0, shape[2] * result.stacks[0].voxel_size[2])
             self.input_average_range.setValue(10)
 
         super().setResult(result)
         self.hide_timestamp()
         if not no_update_display:
             self.update_display()
 
@@ -720,99 +721,102 @@
             self.no_update = False
 
     def get_time_text(self):
         return formatTimedelta(datetime.timedelta(seconds=float(self.t_slider.value() * self.result.time_delta) + self.time_start.value()),
                         self.time_format.value())
 
     def get_current_arrow_data(self):
-        M = None
+        mesh = None
         field = None
         center = None
         name = ""
         colormap = None
         factor = None
         scale_max = self.vtk_toolbar.getScaleMax()
         stack_min_max = None
         skip = self.input_arrow_skip.value()
         if self.input_arrows.value() == "piv":
             if self.result is None:
-                M = None
+                mesh = None
             else:
-                M = self.result.mesh_piv[self.t_slider.value()]
+                mesh = self.result.mesh_piv[self.t_slider.value()]
 
-            if M is not None:
-                if M.hasNodeVar("U_measured"):
-                    # showVectorField2(self, M, "U_measured")
-                    field = M.getNodeVar("U_measured")
+            if mesh is not None:
+                if mesh.displacements_measured is not None:
+                    # showVectorField2(self, M, "displacements_measured")
+                    field = mesh.displacements_measured
                     factor = 0.1 * self.vtk_toolbar.arrow_scale.value()
-                    name = "U_measured"
+                    name = "displacements_measured"
                     colormap = self.vtk_toolbar.colormap_chooser.value()
-                    stack_min_max = [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+                    stack_min_max = [mesh.nodes.min(axis=0) * 1e6, mesh.nodes.max(axis=0) * 1e6]
         elif self.input_arrows.value() == "target deformations":
-            M = self.result.solver[self.t_slider.value()]
-            # showVectorField2(self, M, "U_target")
+            M = self.result.solvers[self.t_slider.value()]
+            # showVectorField2(self, M, "displacements_target")
             if M is not None:
-                field = M.U_target
+                mesh = M.mesh
+                field = mesh.displacements_target
                 factor = 0.1 * self.vtk_toolbar.arrow_scale.value()
-                name = "U_target"
+                name = "displacements_target"
                 colormap = self.vtk_toolbar.colormap_chooser.value()
-                stack_min_max = [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+                stack_min_max = [mesh.nodes.min(axis=0) * 1e6, mesh.nodes.max(axis=0) * 1e6]
         elif self.input_arrows.value() == "fitted deformations":
-            M = self.result.solver[self.t_slider.value()]
+            M = self.result.solvers[self.t_slider.value()]
             if M is not None:
-                field = M.U
+                mesh = M.mesh
+                field = mesh.displacements
                 factor = 0.1 * self.vtk_toolbar.arrow_scale.value()
-                name = "U"
+                name = "displacements"
                 colormap = self.vtk_toolbar.colormap_chooser.value()
-                stack_min_max = [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+                stack_min_max = [mesh.nodes.min(axis=0) * 1e6, mesh.nodes.max(axis=0) * 1e6]
         elif self.input_arrows.value() == "fitted forces":
-            M = self.result.solver[self.t_slider.value()]
+            M = self.result.solvers[self.t_slider.value()]
             if M is not None:
+                mesh = M.mesh
                 center = None
                 if self.vtk_toolbar2.use_center.value() is True:
-                    center = M.getCenter(mode="Force")
-                field = -M.f * M.reg_mask[:, None]
+                    center = mesh.get_center(mode="Force")
+                field = -mesh.forces * mesh.mesh.regularisation_mask[:, None]
                 factor = 0.15 * self.vtk_toolbar2.arrow_scale.value()
-                name = "f"
+                name = "forces"
                 colormap = self.vtk_toolbar2.colormap_chooser.value()
                 scale_max = self.vtk_toolbar2.getScaleMax()
-                stack_min_max = [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+                stack_min_max = [mesh.nodes.min(axis=0) * 1e6, mesh.nodes.max(axis=0) * 1e6]
                 skip = self.input_arrow_skip2.value()
         else:
             # get min/max of stack
-            M = self.result.solver[self.t_slider.value()]
+            M = self.result.solvers[self.t_slider.value()]
             if M is not None:
-                stack_min_max = [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+                mesh = M.mesh
+                stack_min_max = [mesh.nodes.min(axis=0) * 1e6, mesh.nodes.max(axis=0) * 1e6]
             else:
-                M = self.result.mesh_piv[self.t_slider.value()]
-                if M is not None:
-                    stack_min_max = [M.R.min(axis=0) * 1e6, M.R.max(axis=0) * 1e6]
+                mesh = self.result.mesh_piv[self.t_slider.value()]
+                if mesh is not None:
+                    stack_min_max = [mesh.nodes.min(axis=0) * 1e6, mesh.nodes.max(axis=0) * 1e6]
                 else:
                     stack_min_max = None
-        return M, field, center, name, colormap, factor, scale_max, stack_min_max, skip
+        return mesh, field, center, name, colormap, factor, scale_max, stack_min_max, skip
 
     def update_display(self):
         if self.no_update:
             return
-        print(self.get_parameters())
+        #print(self.get_parameters())
         #self.set_parameters(self.get_parameters())
         #if self.current_tab_selected is False:
         #    self.current_result_plotted = False
         #    return
 
         if self.check_evaluated(self.result):
             if self.input_use2D.value():
                 im = render_2d(self.get_parameters(), self.result, self)
                 self.pixmap1.setPixmap(QtGui.QPixmap(array2qimage(im)))
                 self.view1.setExtend(im.shape[1], im.shape[0])
                 self.view1.fitInView()
                 self.im = im
                 return
 
-
             self.render_view(True)
 
     def render_view(self, double_render=False):
         render = self.plotter.render
         self.plotter.render = lambda *args: None
         try:
             render_3d(self.get_parameters(), self.result, self.plotter, self)
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/exporter/ExporterRender2D.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExporterRender2D.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,46 +70,46 @@
         data = data.sort_values(by="length", ascending=False)
         d2 = data.groupby(["x", "y"]).first()
         # optional slice
         if skip > 1:
             d2 = d2.loc[(slice(None, None, skip), slice(None, None, skip)), :]
         return np.array([i for i in d2.index]), d2[["length", "angle"]]
 
-    M, field, params_arrows, name = get_mesh_arrows(params, result)
+    mesh, field, params_arrows, name = get_mesh_arrows(params, result)
 
-    if M is None:
+    if mesh is None:
         return pil_image
 
     scale_max = params_arrows["scale_max"] if params_arrows["autoscale"] else None
     colormap = params_arrows["colormap"]
     skip = params_arrows["skip"]
     alpha = params_arrows["arrow_opacity"]
 
     if field is not None:
         # rescale and offset
         scale = 1e6 / display_image[1][0]
         offset = np.array(display_image[0].shape[0:2]) / 2
 
-        R = M.R.copy()
+        R = mesh.nodes.copy()
         field = field.copy()
         R = R[:, :2][:, ::-1] * scale + offset
         field = field[:, :2][:, ::-1] * scale * params_arrows["arrow_scale"]
-        if name == "f":
+        if name == "forces":
             field *= 1e4
 
         if scale_max is None:
             max_length = np.nanmax(np.linalg.norm(field, axis=1))# * params_arrows["arrow_scale"]
         else:
             max_length = scale_max * params_arrows["arrow_scale"]
 
-        z_center = (params["averaging_size"] - result.stack[0].shape[2] / 2) * display_image[1][2] * 1e-6
+        z_center = (params["averaging_size"] - result.stacks[0].shape[2] / 2) * display_image[1][2] * 1e-6
         z_min = z_center - params["averaging_size"] * 1e-6
         z_max = z_center + params["averaging_size"] * 1e-6
 
-        index = (z_min < M.R[:, 2]) & (M.R[:, 2] < z_max)
+        index = (z_min < mesh.nodes[:, 2]) & (mesh.nodes[:, 2] < z_max)
 
         R = R[index]
         field = field[index]
         R, field = project_data(R, field, skip=skip)
         pil_image = add_quiver(pil_image, R, field.length, field.angle, max_length=max_length, cmap=colormap,
                                alpha=alpha,
                                scale=im_scale * aa_scale,
@@ -129,18 +129,18 @@
                 mu = old_v
                 break
             old_v = v
         pixel = mu / pixtomu * scale
         return pixel, mu
 
     if params["scalebar"]["length"] == 0:
-        pixel, mu = getBarParameters(result.stack[0].voxel_size[0])
+        pixel, mu = getBarParameters(result.stacks[0].voxel_size[0])
     else:
         mu = params["scalebar"]["length"]
-        pixel = mu / result.stack[0].voxel_size[0]
+        pixel = mu / result.stacks[0].voxel_size[0]
 
     pil_image = add_scalebar(pil_image, scale=1, image_scale=im_scale * aa_scale,
                              width=params["scalebar"]["width"] * aa_scale,
                              xpos=params["scalebar"]["xpos"] * aa_scale,
                              ypos=params["scalebar"]["ypos"] * aa_scale,
                              fontsize=params["scalebar"]["fontsize"] * aa_scale, pixel_width=pixel,
                              size_in_um=mu, color="w", unit="µm")
@@ -249,18 +249,18 @@
         # get the font
         try:
             font = ImageFont.truetype("arial", font_size)#ImageFont.truetype("tahoma.ttf", font_size)
         except IOError:
             font = ImageFont.truetype("times", font_size)
         # width and height of text elements
         text = "%d" % size_in_um
-        length_number = image.textsize(text, font=font)[0]
-        length_space = 0.5*image.textsize(" ", font=font)[0] # here we emulate a half-sized whitespace
-        length_unit = image.textsize(unit, font=font)[0]
-        height_number = image.textsize(text+unit, font=font)[1]
+        length_number = image.textlength(text, font=font)
+        length_space = 0.5*image.textlength(" ", font=font)  # here we emulate a half-sized whitespace
+        length_unit = image.textlength(unit, font=font)
+        height_number = image.textbbox((0, 0), text+unit, font=font)[3]
 
         total_length = length_number + length_space + length_unit
 
         # find the position for the text to have it centered and bottom aligned
         if pixel_offset_x > 0:
             x = pil_image.size[0] - pixel_offset_x - pixel_width * 0.5 - total_length * 0.5
         else:
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/exporter/ExporterRender3D.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExporterRender3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,25 +59,24 @@
         ("stack", "use_reference_stack"),
         ("channel0", ("show", "sigma_sato", "sigma_gauss", "range", "alpha", "cmap")),
         ("channel1", ("show", "sigma_sato", "sigma_gauss", "range", "alpha", "cmap", "channel")),
         "channel_thresh",
     ]
     params, changed = filter_params(params, used_values, getattr(plotter, "previous_plot_params", {}))
     if not changed and result == getattr(plotter, "previous_plot_result", {}):
-        print("skipped fibers")
         return
 
     crops = []
     for value in [params["crop"]["y"], params["crop"]["x"], params["crop"]["z"]]:
         crops.extend(value)
 
     t = params["time"]["t"]
     t_start = time.time()
     stack_data = None
-    stack = result.stack[t]
+    stack = result.stacks[t]
 
     if params["stack"]["use_reference_stack"]:
         stack = result.stack_reference
 
     if params["channel0"]["show"] and crops[0] != crops[1] and crops[2] != crops[3] and crops[4] != \
             crops[5]:
         stack_data1 = process_stack(stack, 0,
@@ -89,15 +88,15 @@
     else:
         stack_data1 = None
 
     if params["channel1"]["show"] and crops[0] != crops[1] and crops[2] != crops[3] and crops[4] != \
             crops[5]:
 
         if isinstance(params["channel1"]["channel"], str):
-            params["channel1"]["channel"] = result.stack[0].channels.index(params["channel1"]["channel"])
+            params["channel1"]["channel"] = result.stacks[0].channels.index(params["channel1"]["channel"])
         stack_data2 = process_stack(stack,
                                     crops=crops,
                                     **params["channel1"])
         if exporter is not None:
             exporter.channel1_properties.sigmoid.p.set_im(stack_data2["original"])
         if stack_data1 is not None:
             stack_data = join_stacks(stack_data1, stack_data2, params["channel_thresh"])
@@ -113,25 +112,24 @@
 
         plotter.add_volume(mesh,
                           cmap=stack_data["cmap"], opacity=stack_data["opacity"],
                           blending="composite", name="fiber", render=False)  # 1.0*x
         plotter.remove_scalar_bar("values")
     else:
         plotter.remove_actor("fiber")
-    print("plot time", f"{time.time() - t_start:.3f}s")
+    #print("plot time", f"{time.time() - t_start:.3f}s")
 
 
 def render_3d_text(params, result, plotter):
     used_values = [
         ("time", ("t", "display", "fontsize", "start", "format")),
         ("image", "height"),
     ]
     params, changed = filter_params(params, used_values, getattr(plotter, "previous_plot_params", {}))
     if not changed and result == getattr(plotter, "previous_plot_result", {}):
-        print("skipped text")
         return
 
     if result is not None and result.time_delta is not None and params["time"]["display"]:
         plotter.add_text(get_time_text(params, result), name="time_text", font_size=params["time"]["fontsize"],
                          position=(20, params["image"]["height"] - 20 - params["time"]["fontsize"] * 2))
     else:
         plotter.remove_actor("time_text")
@@ -142,17 +140,16 @@
         "use_nans",
         "arrows",
         ("time", "t"),
         ("deformation_arrows", ("scale_max", "autoscale", "skip", "arrow_opacity", "colormap", "arrow_scale")),
         ("force_arrows", ("scale_max", "autoscale", "skip", "arrow_opacity", "colormap", "arrow_scale", "use_center")),
     ]
     params, changed = filter_params(params, used_values, getattr(plotter, "previous_plot_params", {}))
-    print("arrows", changed, result == getattr(plotter, "previous_plot_result", {}))
+
     if not changed and result == getattr(plotter, "previous_plot_result", {}):
-        print("skipped arrows")
         return
 
     obj, field, params_arrows, name = get_mesh_arrows(params, result)
 
     if obj is None:
         plotter.remove_actor("arrows")
         plotter.remove_actor("nans")
@@ -162,15 +159,15 @@
     show_nan = params["use_nans"]
     scalebar_max = params_arrows["scale_max"] if params_arrows["autoscale"] else None
     colormap = params_arrows["colormap"]
     skip = params_arrows["skip"]
     arrow_opacity = params_arrows["arrow_opacity"]
 
     if field is not None:
-        obj_R = obj.R*1e6
+        obj_R = obj.nodes * 1e6
 
         if skip != 1:
             x_unique = len(np.unique(obj_R[:, 0]))
             y_unique = len(np.unique(obj_R[:, 1]))
             z_unique = len(np.unique(obj_R[:, 2]))
             obj_R = obj_R.reshape(x_unique, y_unique, z_unique, 3)[::skip, ::skip, ::skip].reshape(-1, 3)
             field = field.reshape(x_unique, y_unique, z_unique, 3)[::skip, ::skip, ::skip].reshape(-1, 3)
@@ -179,19 +176,19 @@
         nan_values = np.isnan(field[:, 0])
 
         # create a point cloud
         point_cloud = pv.PolyData(obj_R)
         point_cloud.point_data[name] = field
         point_cloud.point_data[name + "_mag"] = np.linalg.norm(field, axis=1)
         # convert to common units
-        if name == "U_measured" or name == "U_target" or name == "U":
+        if name == "displacements_measured" or name == "displacements_target" or name == "displacements":
             # scale deformations to µN
             point_cloud.point_data[name + "_mag2"] = 1e6*point_cloud.point_data[name + "_mag"].copy()
             factor = 0.1 * params_arrows["arrow_scale"]
-        if name == "f":
+        if name == "forces":
             # scale forces to pN
             point_cloud.point_data[name + "_mag2"] = 1e12*point_cloud.point_data[name + "_mag"].copy()
             factor = 0.15 * params_arrows["arrow_scale"]
         # hide nans
         point_cloud.point_data[name + "_mag2"][nan_values] = 0
 
         # scalebar scaling factor
@@ -201,17 +198,17 @@
         else:
             factor = factor * norm_stack_size / scalebar_max
 
         # generate the arrows
         arrows = point_cloud.glyph(orient=name, scale=name + "_mag2", factor=factor)
 
         title = name
-        if name == "U_measured" or name == "U_target" or name == "U":
+        if name == "displacements_measured" or name == "displacements_target" or name == "displacements":
             title = "Deformations (µm)"
-        elif name == "f":
+        elif name == "forces":
             title = "Forces (pN)"
 
         # show the nan points
         if show_nan:
             R = obj_R[nan_values]
             if R.shape[0]:
                 point_cloud2 = pv.PolyData(R)
@@ -234,30 +231,29 @@
         else:
             plotter.update_scalar_bar_range([0, scalebar_max])
     else:
         plotter.remove_actor("arrows")
 
     # plot center points if desired
     if params_arrows.get("use_center", False):
-        center = obj.getCenter(mode="Force")
+        center = obj.get_center(mode="Force")
         plotter.add_points(np.array([center])*1e6, color='m', point_size=10, render=False, name="center")
     else:
         plotter.remove_actor("center")
 
 
 def render_3d_image(params, result, plotter, exporter=None):
     used_values = [
         ("stack", ("image", "colormap", "use_reference_stack", "channel",
                    "z", "z_proj", "contrast_enhance", "use_contrast_enhance",
                    "channel_B", "colormap_B")),
         ("time", "t"),
     ]
     params, changed = filter_params(params, used_values, getattr(plotter, "previous_plot_params", {}))
     if not changed and result == getattr(plotter, "previous_plot_result", {}):
-        print("skipped image")
         return
     scale = 1
     colormap2 = params["stack"]["colormap"]
 
     display_image = getVectorFieldImage(result, params, use_fixed_contrast_if_available=True, exporter=exporter)
     params["stack"]["channel"] = params["stack"]["channel_B"]
     if params["stack"]["channel_B"] != "":
@@ -312,15 +308,14 @@
         "arrows",
         ("time", "t"),
         ("deformation_arrows", ("scale_max", "autoscale", "skip", "arrow_opacity", "colormap", "arrow_scale")),
         ("force_arrows", ("scale_max", "autoscale", "skip", "arrow_opacity", "colormap", "arrow_scale", "use_center")),
     ]
     params, changed = filter_params(params, used_values, getattr(plotter, "previous_plot_params", {}))
     if not changed and result == getattr(plotter, "previous_plot_result", {}):
-        print("skipped bounds")
         return
 
     show_grid = params["show_grid"]
 
     # show the mesh border cube
     if show_grid == 2:
         # get the mesh extent
@@ -335,17 +330,17 @@
                              name="border")
         # or remove the current cube
         else:
             plotter.remove_actor("border")
     # show the image stack border cube
     elif show_grid == 3:
         # get the stack shape
-        if len(result.stack):
-            stack_shape = np.array(result.stack[0].shape[:3]) * np.array(
-                result.stack[0].voxel_size)
+        if len(result.stacks):
+            stack_shape = np.array(result.stacks[0].shape[:3]) * np.array(
+                result.stacks[0].voxel_size)
         else:
             stack_shape = None
         # draw a cube around it
         if stack_shape is not None:
             xmin, xmax = -stack_shape[0] / 2, stack_shape[0] / 2
             ymin, ymax = -stack_shape[1] / 2, stack_shape[1] / 2
             zmin, zmax = -stack_shape[2] / 2, stack_shape[2] / 2
@@ -376,15 +371,14 @@
 
 def render_3d_camera(params, result, plotter, exporter=None, double_render=False):
     used_values = [
         ("camera", ("elevation", "azimuth", "distance", "offset_x", "offset_y", "roll")),
     ]
     params, changed = filter_params(params, used_values, getattr(plotter, "previous_plot_params", {}))
     if not changed and result == getattr(plotter, "previous_plot_result", {}):
-        print("skipped camera")
         return
 
     # reset the camera before rotating
     plotter.camera_position = "yz"
 
     # if the distance is not set use a reasonable default based on the current stack
     if params["camera"]["distance"] == 0:
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/exporter/FiberViewer.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/exporter/FiberViewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,28 +36,25 @@
 
 def cache_results():
     def wrapper(function):
         def apply(data, **params):
             cache_name = f"_saved_{function}"
             if "channel" in params:
                 cache_name = f"_saved_{function}_{params['channel']}"
-                print("channel", cache_name)
-            else:
-                print(cache_name, params)
             t = time.time()
             cache_obj = get_cache(data)
             cached = getattr(cache_obj, cache_name, None)
             cached_params = getattr(cache_obj, f"{cache_name}_params", None)
             if cached is not None and cached_params == params:
-                print("cache", function, "cached", params, f"{time.time()-t:.3f}s")
+                #print("cache", function, "cached", params, f"{time.time()-t:.3f}s")
                 return cached
             result = function(data, **params)
             setattr(cache_obj, cache_name, result)
             setattr(cache_obj, f"{cache_name}_params", params)
-            print("cache", function, "apply", params, f"{time.time()-t:.3f}s")
+            #print("cache", function, "apply", params, f"{time.time()-t:.3f}s")
             return result
         return apply
     return wrapper
 
 
 @cache_results()
 def sato_filter(data, sigma_sato=None):
@@ -310,27 +307,27 @@
                 self.t_slider = QTimeSlider(connected=self.update_display).addToLayout()
                 self.tab.parent().t_slider = self.t_slider
 
         self.setParameterMapping(None, {})
 
 
     def check_evaluated(self, result: Result) -> bool:
-        return self.result is not None and result.stack is not None and len(result.stack) > 0
+        return self.result is not None and result.stacks is not None and len(result.stacks) > 0
 
     def setResult(self, result: Result):
-        if result and result.stack and result.stack[0]:
-            shape = result.stack[0].shape
+        if result and result.stacks and result.stacks[0]:
+            shape = result.stacks[0].shape
             self.input_cropx.setRange(0, shape[1])
             self.input_cropx.setValue((shape[1] // 2 - 100, shape[1] // 2 + 100))
             self.input_cropy.setRange(0, shape[0])
             self.input_cropy.setValue((shape[0] // 2 - 100, shape[0] // 2 + 100))
             self.input_cropz.setRange(0, shape[2])
             self.input_cropz.setValue((shape[2] // 2 - 25, shape[2] // 2 + 25))
 
-            if result.stack[0].shape[-1] == 1:
+            if result.stacks[0].shape[-1] == 1:
                 self.channel1_properties.input_show.setValue(False)
                 self.channel1_properties.setDisabled(True)
             else:
                 self.channel1_properties.setDisabled(False)
         super().setResult(result)
 
     def update_display(self):
@@ -347,24 +344,24 @@
             crops = []
             for widged in [self.input_cropx, self.input_cropy, self.input_cropz]:
                 crops.extend(widged.value())
             t = self.t_slider.value()
             t_start = time.time()
             stack_data = None
             if self.channel0_properties.input_show.value():
-                stack_data1 = process_stack(self.result.stack[t], 0,
+                stack_data1 = process_stack(self.result.stacks[t], 0,
                                             crops=crops,
                                             **self.channel0_properties.value())
                 stack_data = stack_data1
                 self.channel0_properties.sigmoid.p.set_im(stack_data1["original"])
 
             else:
                 stack_data1 = None
             if self.channel1_properties.input_show.value():
-                stack_data2 = process_stack(self.result.stack[t], 1,
+                stack_data2 = process_stack(self.result.stacks[t], 1,
                                             crops=crops,
                                             **self.channel1_properties.value())
                 self.channel1_properties.sigmoid.p.set_im(stack_data2["original"])
                 if stack_data1 is not None:
                     stack_data = join_stacks(stack_data1, stack_data2, self.input_thresh.value())
                 else:
                     stack_data = stack_data2
@@ -380,18 +377,18 @@
                 self.canvas.figure.axes[0].set_ylim(0, 1)
                 self.canvas.draw()
 
             render = self.plotter.render
             self.plotter.render = lambda *args: None
             try:
                 if stack_data is not None:
-                    vol = self.plotter.add_volume(stack_data["data"], resolution=np.array(self.result.stack[0].voxel_size),
-                                              cmap=stack_data["cmap"], opacity=stack_data["opacity"],
-                                         blending="composite", name="fiber", render=False)  # 1.0*x
-                print("plot time", f"{time.time()-t_start:.3f}s")
+                    vol = self.plotter.add_volume(stack_data["data"], resolution=np.array(self.result.stacks[0].voxel_size),
+                                                  cmap=stack_data["cmap"], opacity=stack_data["opacity"],
+                                                  blending="composite", name="fiber", render=False)  # 1.0*x
+                #print("plot time", f"{time.time()-t_start:.3f}s")
                 self.plotter.remove_scalar_bar()
             finally:
                 self.plotter.render = render
                 self.plotter.render()
 
             if cam_pos is not None:
                 self.plotter.camera_position = cam_pos
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/load_measurement_dialog.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/load_measurement_dialog.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import sys
 from qtpy import QtCore, QtWidgets, QtGui
 import time
 
 import saenopy
-import saenopy.multigridHelper
-import saenopy.getDeformations
-import saenopy.multigridHelper
+import saenopy.multigrid_helper
+import saenopy.get_deformations
+import saenopy.multigrid_helper
 import saenopy.materials
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.common.stack_selector import StackSelector
 from saenopy.gui.common.stack_selector_crop import StackSelectorCrop
 from saenopy.gui.common.stack_preview import StackPreview
 
-from saenopy.examples import getExamples
+from saenopy.examples import get_examples
 
 
 class AddFilesDialog(QtWidgets.QDialog):
     mode: str = None
     mode_data: str = None
     start_time: float = 0
 
@@ -46,15 +46,15 @@
                                         def ref_changed():
                                             self.stack_reference.setVisible(self.reference_choice.value())
                                             self.place_holder_widget.setVisible(not self.reference_choice.value())
 
                                         self.reference_choice.valueChanged.connect(ref_changed)
                                         self.stack_reference = StackSelector(QtShortCuts.current_layout, "reference")
                                         self.stack_reference.glob_string_changed.connect \
-                                            (lambda x, y: (print("relaxed, y"), self.stack_reference_input.setText(y)))
+                                            (lambda x, y: self.stack_reference_input.setText(y))
                                         self.stack_reference.setVisible(self.reference_choice.value())
 
                                         self.stack_reference_input = QtWidgets.QLineEdit().addToLayout()
                                     with QtShortCuts.QVBoxLayout():
                                         QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
                                         self.stack_data = StackSelector(QtShortCuts.current_layout, "active stack(s)",
                                                                         self.stack_reference, use_time=True)
@@ -75,26 +75,26 @@
                         QtShortCuts.current_layout.addStretch()
                         self.button_addList00 = QtShortCuts.QPushButton(None, "cancel", self.reject)
 
                         self.button_addList0 = QtShortCuts.QPushButton(None, "ok", self.accept_new)
 
                 with self.tabs.createTab("Existing Measurement") as self.tab3:
                     self.outputText3 = QtShortCuts.QInputFilename(None, "output", settings=settings,
-                                                                  file_type="Results Files (*.npz)",
+                                                                  file_type="Results Files (*.saenopy)",
                                                                   settings_key="batch/wildcard_existing",
                                                                   allow_edit=True, existing=True)
                     self.tab3.addStretch()
                     with QtShortCuts.QHBoxLayout() as layout3:
                         layout3.addStretch()
                         self.button_addList6 = QtShortCuts.QPushButton(None, "cancel", self.reject)
 
                         self.button_addList5 = QtShortCuts.QPushButton(None, "ok", self.accept_existing)
 
                 with self.tabs.createTab("Examples") as self.tab4:
-                    examples = getExamples()
+                    examples = get_examples()
                     self.example_buttons = []
                     with QtShortCuts.QHBoxLayout() as lay:
                         for example_name, properties in examples.items():
                             with QtShortCuts.QGroupBox(None, example_name) as group:
                                 group[0].setMaximumWidth(240)
                                 label1 = QtWidgets.QLabel(properties["desc"]).addToLayout()
                                 label1.setWordWrap(True)
@@ -104,14 +104,19 @@
                                     int(200 * QtGui.QGuiApplication.primaryScreen().logicalDotsPerInch() / 96),
                                     QtCore.Qt.SmoothTransformation)
                                 label.setPixmap(pix)
                                 label.setSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
                                 self.button_example1 = QtShortCuts.QPushButton(None, "Open",
                                                            lambda *, example_name=example_name: self.load_example(example_name))
                                 self.example_buttons.append(self.button_example1)
+                                self.button_example2 = QtShortCuts.QPushButton(None, "Open (evaluated)",
+                                                           lambda *, example_name=example_name: self.load_example(
+                                                                                   example_name, evaluated=True))
+                                self.button_example2.setEnabled(properties.get("url_evaluated", None) is not None)
+                                self.example_buttons.append(self.button_example2)
                         lay.addStretch()
 
                     self.tab4.addStretch()
                     self.download_state = QtWidgets.QLabel("").addToLayout()
                     self.download_progress = QtWidgets.QProgressBar().addToLayout()
                     self.download_progress.setRange(0, 100)
 
@@ -135,17 +140,20 @@
         else:
             self.accept()
 
     def accept_existing(self):
         self.mode = "existing"
         self.accept()
 
-    def load_example(self, example_name):
-        saenopy.loadExample(example_name, None, self.reporthook)
-        self.mode = "example"
+    def load_example(self, example_name, evaluated=False):
+        self.examples_output = saenopy.load_example(example_name, None, self.reporthook, evaluated=evaluated)
+        if evaluated:
+            self.mode = "example_evaluated"
+        else:
+            self.mode = "example"
         self.mode_data = example_name
         self.accept()
 
     def reporthook(self, count, block_size, total_size, msg=None):
         if msg is not None:
             print(msg)
             self.download_state.setText(msg)
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/path_editor.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/path_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 
 def start_path_change(parent, result):
     path_editor = PathEditor(parent, result)
     if not path_editor.exec():
         return
 
     path_changer = PathChanger(result.template, path_editor.input_folder.value())
-    for stack in result.stack:
+    for stack in result.stacks:
         path_changer.stack_change(stack)
     result.template = path_changer.change_path(result.template)
 
     if path_editor.input_folder2 is not None:
         path_changer = PathChanger(result.stack_reference.template, path_editor.input_folder2.value())
         path_changer.stack_change(result.stack_reference)
 
     if path_editor.input_pack.value():
-        for stack in result.stack:
+        for stack in result.stacks:
             stack.pack_files()
         if result.stack_reference:
             result.stack_reference.pack_files()
 
     if path_editor.input_save.value():
         result.save()
-        print("saved")
+        #print("saved")
         return
 
 
 class PathEditor(QtWidgets.QDialog):
     def __init__(self, parent, result):
         super().__init__(parent)
         self.setWindowTitle("Change Path")
@@ -72,18 +72,18 @@
     def change_path(self, path):
         path_type = isinstance(path, Path)
         path = str(path)
         match = self.old_template_re.match(path)
         if match is None:
             raise ValueError(f"Path {path} does not fit template {self.old_template_re}")
         new = self.new_template_format.format(**match.groupdict())
-        print("change_path From", path)
-        print("change_path To  ", new)
+        #print("change_path From", path)
+        #print("change_path To  ", new)
         if path_type:
             return Path(new)
         return new
 
-    def stack_change(self, stack):
+    def stack_change(self, stack: "Stack"):
         for index in range(len(stack.image_filenames)):
             for index2 in range(len(stack.image_filenames[index])):
                 stack.image_filenames[index][index2] = self.change_path(stack.image_filenames[index][index2])
         stack.template = self.change_path(stack.template)
```

### Comparing `saenopy-0.9.0/saenopy/gui/solver/modules/showVectorField.py` & `saenopy-1.0.0/saenopy/gui/solver/modules/showVectorField.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 
 def getVectorFieldImage(self, use_fixed_contrast_if_available=False, use_2D=False):
     try:
         image = self.vtk_toolbar.show_image.value()
         if use_2D:
             image = 1
-        if image and self.t_slider.value() < len(self.result.stack):
+        if image and self.t_slider.value() < len(self.result.stacks):
             if getattr(self, "input_reference_stack", None) and self.input_reference_stack.value() and self.result.stack_reference:
                 stack = self.result.stack_reference
             else:
-                stack = self.result.stack[self.t_slider.value()]
+                stack = self.result.stacks[self.t_slider.value()]
             if self.vtk_toolbar.channel_select.value() >= len(stack.channels):
                 self.vtk_toolbar.channel_select.setValue(0)
                 im = stack[:, :, :, self.z_slider.value(), 0]
             else:
                 im = stack[:, :, :, self.z_slider.value(), self.vtk_toolbar.channel_select.value()]
             if self.vtk_toolbar.button_z_proj.value():
                 z_range = [0, 5, 10, 1000][self.vtk_toolbar.button_z_proj.value()]
@@ -51,18 +51,18 @@
 
 def showVectorField2(self, M, points_name):
     display_image = getVectorFieldImage(self)
 
     try:
         field = getattr(M, points_name)
     except AttributeError:
-        field = M.getNodeVar(points_name)
+        field = M.get_node_var(points_name)
 
-    if len(self.result.stack):
-        stack_shape = np.array(self.result.stack[0].shape[:3])*np.array(self.result.stack[0].voxel_size)
+    if len(self.result.stacks):
+        stack_shape = np.array(self.result.stacks[0].shape[:3]) * np.array(self.result.stacks[0].voxel_size)
     else:
         stack_shape = None
     showVectorField(self.plotter, M, field, points_name,
                     scalebar_max=self.vtk_toolbar.getScaleMax(), show_nan=self.vtk_toolbar.use_nans.value(),
                     display_image=display_image, show_grid=self.vtk_toolbar.show_grid.value(),
                     factor=0.1*self.vtk_toolbar.arrow_scale.value(),
                     colormap=self.vtk_toolbar.colormap_chooser.value(),
@@ -83,15 +83,15 @@
     try:
         plotter.renderer.remove_bounds_axes()
         plotter.renderer.remove_bounding_box()
 
         scale = 1  # 1e-6
 
         if field is not None:
-            obj_R = obj.R*1e6
+            obj_R = obj.nodes*1e6
 
             if skip != 1:
                 N = int(np.sqrt(obj_R.shape[0]))
                 x_unique = len(np.unique(obj_R[:, 0]))
                 y_unique = len(np.unique(obj_R[:, 1]))
                 z_unique = len(np.unique(obj_R[:, 2]))
                 obj_R = obj_R.reshape(x_unique, y_unique, z_unique, 3)[::skip, ::skip, ::skip].reshape(-1, 3)
@@ -101,18 +101,18 @@
             nan_values = np.isnan(field[:, 0])
 
             # create a point cloud
             point_cloud = pv.PolyData(obj_R)
             point_cloud.point_data[name] = field
             point_cloud.point_data[name + "_mag"] = np.linalg.norm(field, axis=1)
             # convert to common units
-            if name == "U_measured" or name == "U_target" or name == "U":
+            if name == "displacements_measured" or name == "displacements_target" or name == "displacements":
                   # scale deformations to µN
                   point_cloud.point_data[name + "_mag2"] = 1e6*point_cloud.point_data[name + "_mag"].copy()
-            if name == "f":
+            if name == "forces":
                   # scale forces to pN
                   point_cloud.point_data[name + "_mag2"] = 1e12*point_cloud.point_data[name + "_mag"].copy()
             # hide nans
             point_cloud.point_data[name + "_mag2"][nan_values] = 0
             # show nans
             if not show_all_points and show_nan:
                 R = obj_R[nan_values]
@@ -127,17 +127,17 @@
             else:
                 factor = factor * norm_stack_size / scalebar_max
 
             # generate the arrows
             arrows = point_cloud.glyph(orient=name, scale=name + "_mag2", factor=factor)
 
             title = name
-            if name == "U_measured" or name == "U_target" or name == "U":
+            if name == "displacements_measured" or name == "displacements_target" or name == "displacements":
                 title = "Deformations (µm)"
-            elif name == "f":
+            elif name == "forces":
                 title = "Forces (pN)"
 
             sargs = dict(#position_x=0.05, position_y=0.95,
                          title_font_size=15,
                          label_font_size=15,
                          n_labels=3,
                          title=title,
```

### Comparing `saenopy-0.9.0/saenopy/gui/spheroid/gui_deformation_spheroid.py` & `saenopy-1.0.0/saenopy/gui/spheroid/gui_deformation_spheroid.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,15 @@
         #p.setBrush(QtGui.QBrush(QtGui.QColor("gray")))
         top = 5
         p.drawRect(0, self.height()-1, self.width(), 0)
         p.drawRect(0, top, 0, self.height())
         p.drawRect(0, top, 7, 0)
         p.drawRect(self.width()-1, top, 0, self.height())
         super().paintEvent(ev)
-
+                    
     def toggle(self):
         self.setValue(not self.value())
         self.changedActive()
 
     def setValue(self, value):
         self.toggleButton.setValue(value)
         self.changedActive()
@@ -268,15 +268,15 @@
         self.settings = QtCore.QSettings("Saenopy", "Saenopy")
 
         with QtShortCuts.QHBoxLayout(self):
             with QtShortCuts.QVBoxLayout() as main_layout:
                 with QtShortCuts.QGroupBox(None, "Material Parameters") as (self.material_parameters, layout):
                     with QtShortCuts.QHBoxLayout():
                         self.input_k = QtShortCuts.QInputString(None, "k", "1449", type=float)
-                        self.input_d0 = QtShortCuts.QInputString(None, "d0", "0.00215", type=float)
+                        self.input_d_0 = QtShortCuts.QInputString(None, "d_0", "0.00215", type=float)
                     with QtShortCuts.QHBoxLayout():
                         self.input_lamda_s = QtShortCuts.QInputString(None, "lamdba_s", "0.032", type=float)
                         self.input_ds = QtShortCuts.QInputString(None, "ds", "0.055", type=float)
 
                 with QtShortCuts.QGroupBox(None, "Pressure Range") as (self.material_parameters, layout):
                     with QtShortCuts.QHBoxLayout():
                         self.start = QtShortCuts.QInputString(None, "min", "0.1", type=float)
@@ -313,17 +313,17 @@
             To calculate the contractile forces that multicellular aggregates excert on the surrounding
             matrix, we generate material lookup-tables that predict the contractile pressure
             from the size of the matrix deformations as a function of the distance to the spheroid center as 
             described in Mark et al. (2020, <a href="https://elifesciences.org/articles/51912">click here for more details</a>). <br/>
             <br/>
 
             To generate a material lookup-table, we model the nonlinear fiber material according to the
-            given material properties <b>k</b>, <b>d0</b>, <b>ds</b> and <b>lambda_s</b> 
+            given material properties <b>k</b>, <b>d_0</b>, <b>ds</b> and <b>lambda_s</b> 
             (<a href="https://saenopy.readthedocs.io/en/latest/">click here for more details</a>).<br/>
-            <i> Default values are taken from a collagen I hydrogel (1.2mg/ml) with k=1449, d0=0.00215, ds=0.055, lambda_s=0.032.</i><br/>
+            <i> Default values are taken from a collagen I hydrogel (1.2mg/ml) with k=1449, d_0=0.00215, ds=0.055, lambda_s=0.032.</i><br/>
             <br/>
 
             The simulations then approximate the multicellular aggregate as a spherical inclusion that is
             surrounded by the user-defined nonlinear material and excerts a contractile pressure on the matrix. We conduct a range of simulations   
             for n=<b>count</b> different pressures (default 150) that are spaced between a pressure of <b>min</b> Pa (default 600) 
             and <b>max</b> Pa (default 1000). <br/>
             <br/>
@@ -346,15 +346,15 @@
             arbitrary Young's modulus can be created without conducting simulations
             in the next step.
             """)
             self.description.setOpenExternalLinks(True)
 
         self.input_list = [
             self.input_k,
-            self.input_d0,
+            self.input_d_0,
             self.input_lamda_s,
             self.input_ds,
             self.start,
             self.end,
             self.n,
             self.max_iter,
             self.step,
@@ -398,15 +398,15 @@
         self.progressbar.setValue(i)
 
     def run_thread(self):
         out_table = Path(self.output.value())
         out_folder = out_table.parent / out_table.stem
 
         material = jf.materials.custom(self.input_k.value(),
-                                       self.input_d0.value(),
+                                       self.input_d_0.value(),
                                        self.input_lamda_s.value(),
                                        self.input_ds.value(),
                                        )
 
         jf.simulation.distribute_solver('jf.simulation.spherical_contraction_solver',
                                         const_args={'meshfile': self.localpath,
                                                     # path to the provided or the new generated mesh
@@ -749,33 +749,36 @@
 class QSlider(QtWidgets.QSlider):
     min = None
     max = None
     evaluated = 0
 
     def paintEvent(self, ev: QtGui.QPaintEvent) -> None:
         if self.maximum()-self.minimum():
-            if self.min is not None:
+           
+            if (self.min is not None) and (self.min != "None"):
                 self.drawRect(0, self.min, "gray", 0.2)
-            if self.max is not None:
+            if (self.max is not None) and (self.max != "None"):
                 value = self.max
                 if self.max < 0:
                     value = self.maximum()+self.max
                 self.drawRect(value, self.maximum(), "gray", 0.2)
-            if self.evaluated is not None:
+            if (self.evaluated is not None) and (self.min != "None"):
                 self.drawRect(self.min if self.min is not None else 0, self.evaluated, "lightgreen", 0.3)
         super().paintEvent(ev)
 
     def drawRect(self, start, end, color, border):
         p = QtGui.QPainter(self)
         p.setPen(QtGui.QPen(QtGui.QColor("transparent")))
-        p.setBrush(QtGui.QBrush(QtGui.QColor(color)))
-        s = self.width() * (start - self.minimum()) / (self.maximum() - self.minimum() + 1e-5)
-        e = self.width() * (end - self.minimum()) / (self.maximum() - self.minimum() + 1e-5)
-        p.drawRect(int(s), int(self.height()*border),
-                   int(e-s), int(self.height()*(1-border*2)))
+        p.setBrush(QtGui.QBrush(QtGui.QColor(color)))  
+            
+        if (self.min is not None) and (end != "None") and (start != "None"):
+            s = self.width() * (start - self.minimum()) / (self.maximum() - self.minimum() + 1e-5)
+            e = self.width() * (end - self.minimum()) / (self.maximum() - self.minimum() + 1e-5)
+            p.drawRect(int(s), int(self.height()*border),
+                       int(e-s), int(self.height()*(1-border*2)))
 
     def setEvaluated(self, value):
         self.evaluated = value
         self.update()
 
 
 class BatchEvaluate(QtWidgets.QWidget):
@@ -1040,15 +1043,15 @@
         if not dialog.exec():
             return
 
         import glob
         import re
         text = os.path.normpath(dialog.inputText.value())
         glob_string = text.replace("?", "*")
-        print("globbing", glob_string)
+        #print("globbing", glob_string)
         files = natsorted(glob.glob(glob_string))
 
         output_base = glob_string
         while "*" in str(output_base):
             output_base = Path(output_base).parent
 
         regex_string = re.escape(text).replace(r"\*", "(.*)").replace(r"\?", ".*")
@@ -1101,15 +1104,15 @@
                 attr["thres_segmentation"] = self.segmention_thres_indi.value()
                 #attr["seg_gaus1"] = self.seg_gaus1_indi.value()
                 #attr["seg_gaus2"] = self.seg_gaus2_indi.value()
             else:
                 self.segmention_thres_indi.setValue(attr["thres_segmentation"])
                 #self.seg_gaus1_indi.setValue(attr["seg_gaus1"])
                 #self.seg_gaus2_indi.setValue(attr["seg_gaus2"])
-                print("->", [attr[v] is None for v in ["thres_segmentation"]])
+                #print("->", [attr[v] is None for v in ["thres_segmentation"]])
                 if np.all([attr[v] is None for v in ["thres_segmentation"]]):
                     self.individual_data.setValue(False)
                 else:
                     self.individual_data.setValue(True)
             self.last_cell = self.list.currentRow()
             self.images = data["images"]
             self.last_image = None
@@ -1139,28 +1142,28 @@
     def slider_changed(self, i):
         data = self.data[self.list.currentRow()][2]
 
         thres_segmentation = self.thres_segmentation.value() if data["thres_segmentation"] is None else data["thres_segmentation"]
 
         if self.last_image is not None and self.last_image[0] == i:
             i, im, im0 = self.last_image
-            print("cached")
+            #print("cached")
         else:
-            im = imageio.imread(self.images[i]).astype(float)
+            im = imageio.v2.imread(self.images[i]).astype(float)
             if self.continous_segmentation.value() is True:
                 im0 = im
             else:
-                im0 = imageio.imread(self.images[0]).astype(float)
+                im0 = imageio.v2.imread(self.images[0]).astype(float)
             self.last_image = [i, im, im0]
 
         if self.last_seg is not None and \
                 self.last_seg[1] == thres_segmentation and \
                 self.continous_segmentation.value() is False:
             pass
-            print("cached")
+            #print("cached")
         else:
             print(self.last_seg, i, thres_segmentation)
             seg0 = jf.piv.segment_spheroid(im0, True, thres_segmentation)
             from skimage import measure
             # Find contours at a constant value of 0.8
             contours = measure.find_contours(seg0["mask"], 0.5)
 
@@ -1185,16 +1188,16 @@
         #buf = io.BytesIO()
         #import time
         #t = time.time()
         #dis_sum = np.load(str(data["output"]) + '/def' + str(i).zfill(6) + '.npy', allow_pickle=True).item()
         #print("loadtime", time.time()-t)
 
         try:
-            #im = imageio.imread(buf)
-            im = imageio.imread(str(data["output"]) + '/plot' + str(i).zfill(6) + '.png')
+            #im = imageio.v2.imread(buf)
+            im = imageio.v2.imread(str(data["output"]) + '/plot' + str(i).zfill(6) + '.png')
         except FileNotFoundError:
             im = np.zeros(im.shape)
         self.pixmap2.setPixmap(QtGui.QPixmap(array2qimage(im)))
         self.label2.setExtend(im.shape[1], im.shape[0])
 
         self.line_views()
 
@@ -1278,70 +1281,90 @@
             self.slider.setRange(1, i)
             # it the slider was at the last value, move it to the new maximum
             if self.slider.value() == i-1:
                 self.slider.setValue(i)
 
     def run_thread(self):
         try:
-            print("compute displacements")
+            #print("compute displacements")
             n = self.list.count() - 1
             for i in range(n):
                 try:
                     if not self.data[i][1]:
                         continue
                     data = self.data[i][2]
                     self.progress_signal.emit(i, n, 0, len(data["images"]))
                     folder, file = os.path.split(self.data[i][0])
 
                     continous_segmentation = self.continous_segmentation.value()
                     thres_segmentation = data["thres_segmentation"] or self.thres_segmentation.value()
-                    n_min = self.n_min.value()
-                    n_max = self.n_max.value()
-
+                    
+                    # set proper None values if no number set
+                    try:
+                        n_min = int(self.n_min.value())
+                    except:
+                        n_min = None
+                    try:
+                        n_max = int(self.n_max.value())
+                    except:
+                        n_max = None
+                    try:
+                        cbar_um_scale = float(self.cbar_um_scale.value())
+                    except:
+                        cbar_um_scale = None    
+                    try:
+                        r_max = float(self.x1.value())
+                    except:
+                        r_max = None    
+                    try:
+                        r_min = float(self.x0.value())
+                    except:
+                        r_min = None  
+                        
                     if self.deformation_data.value() is True:
                         jf.piv.compute_displacement_series(str(folder),
                                                        str(file),
                                                        str(data["output"]),
                                                        n_max=n_max,
                                                        n_min=n_min,
                                                        plot=self.plot_data.value(),
                                                        #plot=self.plot.value(),
                                                        draw_mask=False,
                                                        color_norm=self.color_norm.value(),
-                                                       cbar_um_scale=(self.cbar_um_scale.value()),
-                                                       quiver_scale=(self.quiver_scale.value()),
+                                                       cbar_um_scale= cbar_um_scale ,
+                                                       quiver_scale=self.quiver_scale.value(),
                                                        dpi=(self.dpi.value()),
                                                        continous_segmentation=continous_segmentation,
                                                        thres_segmentation=thres_segmentation,
                                                        window_size=(self.window_size.value()),
                                                        dt_min=(self.dt_min.value()),
                                                        cutoff=None, cmap="turbo",
                                                        callback=lambda ii, nn: self.progress_signal.emit(i, n, ii, nn))
 
                     elif self.plot_data.value() is True:
                         images = data["images"]
                         for ii in range(0, len(images)):
-                            im = imageio.imread(images[i]).astype(float)
+                            im = imageio.v2.imread(images[i]).astype(float)
                             if ii == 0 or self.continous_segmentation.value() is True:
                                 seg0 = jf.piv.segment_spheroid(im, True, self.thres_segmentation.value())
                             if ii > 0:
-                                print("self.dt_min.value()*ii if self.dt_min.value() is not None else None", self.dt_min.value()*ii if self.dt_min.value() is not None else None)
+                                #print("self.dt_min.value()*ii if self.dt_min.value() is not None else None", self.dt_min.value()*ii if self.dt_min.value() is not None else None)
                                 from jointforces.piv import save_displacement_plot
                                 dis_sum = np.load(str(data["output"]) + '/def' + str(ii).zfill(6) + '.npy', allow_pickle=True).item()
                                 save_displacement_plot(str(data["output"]) + '/plot' + str(ii).zfill(6) + '.png', im,
                                                        seg0, dis_sum,
                                                            quiver_scale=(self.quiver_scale.value()),
                                                        color_norm=self.color_norm.value(), cbar_um_scale=(self.cbar_um_scale.value()), dpi=(self.dpi.value()), t=self.dt_min.value()*ii if self.dt_min.value() is not None else None)
                             self.progress_signal.emit(i, n, ii, len(images))
 
                     if self.force_data.value() is True:
                         jf.force.reconstruct(str(data["output"]),  # PIV output folder
                                              str(self.lookup_table.value()),  # lookup table
                                              self.pixel_size.value(),  # pixel size (µm)
-                                             None, r_min=self.x0.value(), r_max=self.x1.value())
+                                             None, r_min=r_min, r_max=r_max)
                 except Exception as err:
                     import traceback
                     traceback.print_exc()
                     self.measurement_evaluated_signal.emit(i, -1)
                 self.progress_signal.emit(i+1, n, 0, len(data["images"]))
         finally:
             self.finished_signal.emit()
@@ -1590,25 +1613,24 @@
                 new_path = str(new_path)
             import json
             with open(new_path, "r") as fp:
                 list_new = json.load(fp)
             self.list.clear()
             self.list.setData([[i["name"], i["selected"], [], i["color"]] for i in list_new])
             self.data_folders = self.list.data
-            print("y", self.list.data)
+
             for i, d in enumerate(list_new):
                 self.list.setCurrentRow(i)
                 self.list.listSelected()
                 self.listSelected()
                 self.list2.data = self.list.data[i][2]
-                self.add_files([d0["path"] for d0 in d["paths"]])
-                print("xxx", self.list.data)
-                for ii, d0 in enumerate(d["paths"]):
-                    self.list2.data[ii][1] = d0["selected"]
-            print("x", self.list.data)
+                self.add_files([d_0["path"] for d_0 in d["paths"]])
+
+                for ii, d_0 in enumerate(d["paths"]):
+                    self.list2.data[ii][1] = d_0["selected"]
 
     def update_group_name(self):
         if self.list.currentItem() is not None:
             self.box_group.setTitle(f"Files for '{self.list.currentItem().text()}'")
             self.box_group.setEnabled(True)
         else:
             self.box_group.setEnabled(False)
@@ -1678,22 +1700,22 @@
         self.add_files(files)
 
     def add_files(self, files):
         current_group = self.list2.data
         current_files = [d[0] for d in current_group]
         for file in files:
             if file in current_files:
-                print("File already in list", file)
+                #print("File already in list", file)
                 continue
             try:
-                print("Add file", file)
+                #print("Add file", file)
                 res = self.getPandasData(file)
                 if self.list2.data is current_group:
                     self.list2.addData(file, True, res)
-                    print("replot")
+                    #print("replot")
                     self.replot()
                 app.processEvents()
             except FileNotFoundError:
                 continue
 
     def getPandasData(self, file):
         res = pd.read_excel(file)
```

### Comparing `saenopy-0.9.0/saenopy/img/Icon.ico` & `saenopy-1.0.0/saenopy/img/Icon.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/Logo.png` & `saenopy-1.0.0/saenopy/img/Logo.png`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/Logo.svg` & `saenopy-1.0.0/saenopy/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/Logo_black.png` & `saenopy-1.0.0/saenopy/img/Logo_black.png`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/arrowscale.ico` & `saenopy-1.0.0/saenopy/img/arrowscale.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/autoscale0.ico` & `saenopy-1.0.0/saenopy/img/autoscale0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/autoscale1.ico` & `saenopy-1.0.0/saenopy/img/autoscale1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/buttons.svg` & `saenopy-1.0.0/saenopy/img/buttons.svg`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/center0.ico` & `saenopy-1.0.0/saenopy/img/center0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/center1.ico` & `saenopy-1.0.0/saenopy/img/center1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/contrast0.ico` & `saenopy-1.0.0/saenopy/img/contrast0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/contrast1.ico` & `saenopy-1.0.0/saenopy/img/contrast1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/grid.ico` & `saenopy-1.0.0/saenopy/img/grid.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/grid2.ico` & `saenopy-1.0.0/saenopy/img/grid2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/grid3.ico` & `saenopy-1.0.0/saenopy/img/grid3.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/logo_splash.png` & `saenopy-1.0.0/saenopy/img/logo_splash.png`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/nan0.ico` & `saenopy-1.0.0/saenopy/img/nan0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/nan1.ico` & `saenopy-1.0.0/saenopy/img/nan1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/show_image.ico` & `saenopy-1.0.0/saenopy/img/show_image.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/show_image2.ico` & `saenopy-1.0.0/saenopy/img/show_image2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/show_image3.ico` & `saenopy-1.0.0/saenopy/img/show_image3.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/slice0.ico` & `saenopy-1.0.0/saenopy/img/slice0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/slice1.ico` & `saenopy-1.0.0/saenopy/img/slice1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/slice2.ico` & `saenopy-1.0.0/saenopy/img/slice2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/slice_all.ico` & `saenopy-1.0.0/saenopy/img/slice_all.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/thumbnails/BFTFM.png` & `saenopy-1.0.0/saenopy/img/thumbnails/BFTFM.png`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/thumbnails/BFTFM_2.png` & `saenopy-1.0.0/saenopy/img/thumbnails/BFTFM_2.png`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/thumbnails/Bead_example_icon.png` & `saenopy-1.0.0/saenopy/img/thumbnails/Bead_example_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/thumbnails/Dynamic_icon.png` & `saenopy-1.0.0/saenopy/img/thumbnails/Dynamic_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/thumbnails/StainedOrganoid_icon.png` & `saenopy-1.0.0/saenopy/img/thumbnails/StainedOrganoid_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/thumbnails/liver_fibroblast_icon.png` & `saenopy-1.0.0/saenopy/img/thumbnails/liver_fibroblast_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/view_single.ico` & `saenopy-1.0.0/saenopy/img/view_single.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/img/view_two.ico` & `saenopy-1.0.0/saenopy/img/view_two.ico`

 * *Files identical despite different names*

### Comparing `saenopy-0.9.0/saenopy/macro.py` & `saenopy-1.0.0/saenopy/unused/macro.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,516 +1,521 @@
-import numpy as np
-from .buildBeams import buildBeams
-from .materials import Material
-from typing import Sequence
-from scipy.interpolate import interp1d
-
-
-def getQuadrature(N: int, xmin: float, xmax: float) -> (np.ndarray, np.ndarray):
-    """
-    Provides N quadrature points for an integration from xmin to xmax together with their weights.
-
-    Parameters
-    ----------
-    N : int
-        The number of quadrature points to use. Has to be 1 <= N <= 5.
-    xmin : float
-        The start of the integration range
-    xmax : float
-        The end of the integration range
-
-    Returns
-    -------
-    points : np.ndarray
-        The points of the quadrature
-    w : np.ndarray
-        The weights of the points
-    """
-    if N < 1:
-        raise ValueError()
-
-    if N == 1:
-        points = [0]
-        w = [2]
-
-    if N == 2:
-        points = [-np.sqrt(1 / 3), np.sqrt(1 / 3)]
-        w = [1, 1]
-
-    if N == 3:
-        points = [-np.sqrt(3 / 5), 0, np.sqrt(3 / 5)]
-        w = [5 / 9, 8 / 9, 5 / 9]
-
-    if N == 4:
-        points = [-np.sqrt(3 / 7 - 2 / 7 * np.sqrt(6 / 5)), +np.sqrt(3 / 7 - 2 / 7 * np.sqrt(6 / 5)),
-                  -np.sqrt(3 / 7 + 2 / 7 * np.sqrt(6 / 5)), +np.sqrt(3 / 7 + 2 / 7 * np.sqrt(6 / 5))]
-        w = [(18 + np.sqrt(30)) / 36, (18 + np.sqrt(30)) / 36, (18 - np.sqrt(30)) / 36, (18 - np.sqrt(30)) / 36]
-
-    if N == 5:
-        points = [0,
-                  -1 / 3 * np.sqrt(5 - 2 * np.sqrt(10 / 7)), +1 / 3 * np.sqrt(5 - 2 * np.sqrt(10 / 7)),
-                  -1 / 3 * np.sqrt(5 + 2 * np.sqrt(10 / 7)), +1 / 3 * np.sqrt(5 + 2 * np.sqrt(10 / 7))]
-        w = [128 / 225, (322 + 13 * np.sqrt(70)) / 900, (322 + 13 * np.sqrt(70)) / 900, (322 - 13 * np.sqrt(70)) / 900,
-             (322 - 13 * np.sqrt(70)) / 900]
-
-    if N > 5:
-        raise ValueError()
-
-    points = np.array(points)
-    w = np.array(w)
-    factor = (xmax - xmin) / 2
-    points = factor * points + (xmax + xmin) / 2
-    w = w * factor
-    return points, w
-
-
-def combineQuadrature(p1_w1: Sequence, p2_w2: Sequence) -> (np.ndarray, np.ndarray, np.ndarray):
-    """
-    Combine the quadratures of two different axes.
-
-    Parameters
-    ----------
-    p1_w1 : tuple
-        the points and weights for the first axis
-    p2_w2 : tuple
-        the points and weights for the second axis
-
-    Returns
-    -------
-    x : np.ndarray
-        the points for the first axis
-    y : np.ndarray
-        the points for the second axis
-    w : np.ndarray
-        the combined weights for the points
-    """
-    p1, w1 = p1_w1
-    p2, w2 = p2_w2
-    x, y = [f.ravel() for f in np.meshgrid(p1, p2)]
-    w = (w1[:, None] * w2[None, :]).ravel()
-    return x, y, w
-
-
-def getShearRheometerStress(gamma: np.ndarray, material: Material, s: np.ndarray = None) -> (np.ndarray, np.ndarray):
-    r"""
-    This function returns the stress the material model generates when subjected to a shear strain,
-    as seen in a shear rheometer.
-
-    The shear strain is described using the following deformation gradient :math:`\mathbf{F}`:
-
-    .. math::
-        \mathbf{F}(\gamma) =
-        \begin{pmatrix}
-            1 & \gamma & 0 \\
-            0 & 1 & 0 \\
-            0 & 0 & 1 \\
-        \end{pmatrix}
-
-    and the resulting stress is obtained by calculating numerically the derivative of the energy density :math:`W` with
-    respect to the strain :math:`\gamma`:
-
-    .. math::
-        \sigma(\gamma) = \frac{dW(\mathbf{F}(\gamma))}{d\gamma}
-
-    Parameters
-    ----------
-    gamma : ndarray
-        The strain values for which to calculate the stress.
-    material : :py:class:`~.materials.Material`
-        The material model to use.
-
-    Returns
-    -------
-    strain : ndarray
-        The strain values.
-    stress : ndarray
-        The resulting stress.
-
-    """
-    if s is None:
-        s = buildBeams(30)
-
-    F = np.eye(3)
-    F = np.tile(F, (gamma.shape[0], 1, 1))
-    F[:, 0, 1] = gamma
-
-    s_bar = F @ s.T
-
-    s_abs = np.linalg.norm(s_bar, axis=-2)
-
-    eps = material.energy(s_abs - 1)
-
-    W = np.mean(eps, axis=-1)
-    dW = np.diff(W) / np.diff(gamma)
-    return gamma[:-1] + np.diff(gamma) / 2, dW
-
-
-def getShearRheometerStressRotation(gamma, material, H=1e-3, R=10e-3, s=30, q=2):
-    if isinstance(s, int):
-        s = buildBeams(s)
-
-    x_r, z_h, w = combineQuadrature(getQuadrature(q, 0, 1), getQuadrature(q, 0, 1))
-
-    F = np.zeros((gamma.shape[0], len(z_h), 3, 3))
-    theta = gamma * H / R
-    theta_p = theta[:, None] * z_h[None, :]
-
-    cos, sin = np.cos(theta_p), np.sin(theta_p)
-    xtheta_h = x_r * theta[:, None] * R / H
-    F[:, :, 0, 0], F[:, :, 0, 1], F[:, :, 0, 2] = cos, -sin, -sin * xtheta_h
-    F[:, :, 1, 0], F[:, :, 1, 1], F[:, :, 1, 2] = sin, cos, cos * xtheta_h
-    F[:, :, 2, 2] = 1
-
-    s_bar = F @ s.T
-
-    s_abs = np.linalg.norm(s_bar, axis=-2)
-    eps = material.energy(s_abs - 1)
-
-    W = np.mean(eps, axis=-1)
-    W = np.average(W, axis=-1, weights=w)
-    dW = np.diff(W) / np.diff(gamma)
-
-    return gamma[:-1] + np.diff(gamma) / 2, dW
-
-
-def getStretchThinning(gamma_h, gamma_v, material, s=None):
-    r"""
-    This function returns the vertical thinning (strain in z direction) of the material model
-    when the material model is stretched horizonally (strain in x direction), as seen in a stretcher device.
-
-    The strain in x and z direction is described using the following deformation gradient :math:`\mathbf{F}`:
-
-    .. math::
-        \mathbf{F}(\gamma) =
-        \begin{pmatrix}
-            \gamma_h & 0 & 0 \\
-            0 & 1 & 0 \\
-            0 & 0 & \gamma_v \\
-        \end{pmatrix}
-
-    the resulting energy density :math:`W(\mathbf{F}(\gamma_h,\gamma_v))` is then minimized numerically for every
-    :math:`\gamma_h` to obtain the :math:`\gamma_v` that results in the lowest energy of the system.
-
-    Parameters
-    ----------
-    gamma_h : ndarray
-        The applied strain in horizontal direction.
-    gamma_v : ndarray
-        The different values for thinning to test. The value with the lowest energy for each horizontal strain is
-        returned.
-    material : :py:class:`~.materials.Material`
-        The material model to use.
-
-    Returns
-    -------
-    gamma_h : ndarray
-        The horizontal strain values.
-    gamma_v : ndarray
-        The vertical strain that minimizes the energy for the horizontal strain.
-    """
-    if s is None:
-        s = buildBeams(30)
-
-    F00, F22 = np.meshgrid(gamma_v, gamma_h)
-    F11 = np.ones_like(F00)
-    F = np.dstack((F00, F11, F22))
-
-    s_bar = np.einsum("hvj,bj->hvjb", F, s)
-    s_abs = np.linalg.norm(s_bar, axis=-2)
-    eps = material.energy(s_abs - 1)
-    W = np.mean(eps, axis=-1)
-
-    index = np.argmin(W, axis=1)
-    return gamma_h, gamma_v[index]
-
-
-def getExtensionalRheometerStress(gamma, material, s=None):
-    r"""
-    This function returns the stress the material model generates when subjected to an extensional strain,
-    as seen in an extensional rheometer.
-
-    The extensional strain is described using the following deformation gradient :math:`\mathbf{F}`:
-
-    .. math::
-        \mathbf{F}(\gamma) =
-        \begin{pmatrix}
-            \gamma & 0 & 0 \\
-            0 & 1 & 0 \\
-            0 & 0 & 1 \\
-        \end{pmatrix}
-
-    and the resulting stress is obtained by calculating numerically the derivative of the energy density :math:`W` with
-    respect to the strain :math:`\gamma`:
-
-    .. math::
-        \sigma(\gamma) = \frac{dW(\mathbf{F}(\gamma))}{d\gamma}
-
-
-    Parameters
-    ----------
-    gamma : ndarray
-        The strain values for which to calculate the stress.
-    material : :py:class:`~.materials.Material`
-        The material model to use.
-
-    Returns
-    -------
-    strain : ndarray
-        The strain values.
-    stress : ndarray
-        The resulting stress.
-    """
-    if s is None:
-        s = buildBeams(30)
-
-    F = np.eye(3)
-    F = np.tile(F, (gamma.shape[0], 1, 1))
-    F[:, 0, 0] = gamma
-
-    s_bar = F @ s.T
-
-    s_abs = np.linalg.norm(s_bar, axis=-2)
-
-    eps = material.energy(s_abs - 1)
-
-    W = np.mean(eps, axis=-1)
-    dW = np.diff(W) / np.diff(gamma)
-    return gamma[:-1] + np.diff(gamma) / 2, dW
-
-
-import numpy as np
-from scipy import interpolate
-import matplotlib.pyplot as plt
-from saenopy.materials import SemiAffineFiberMaterial
-
-def fit_error(xy, xy0, w=None):
-    # split the data
-    x, y = xy
-    x0, y0 = xy0.T
-    # interpolate the fit to ensure we have values at the correct x positions
-    f = interpolate.interp1d(x, y, bounds_error=False)
-    # evaluate the interpolated fit at the x0 values and calculate the squared difference to the y0 values
-    difference = (y0-f(x0))**2
-    # if we have no weights
-    if w is None:
-        # just take the mean (ignoring nans)
-        return np.sqrt(np.nanmean(difference/np.nanmax(y0)))
-    # if not ignore the nans by finding the indices
-    indices = ~np.isnan(difference)
-    # and average with the given weights
-    return np.sqrt(np.average(difference[indices]/np.nanmax(y0[indices]), weights=w[indices]))
-
-
-def get_cost_function(func, data_shear1, params, MaterialClass, x_sample=100):
-    # find a reasonable range of shear values
-    x0 = data_shear1[:, 0]
-    dx = x0[1] - x0[0]
-    gamma1 = np.linspace(np.min(x0), np.max(x0), x_sample)
-
-    # define weights for logarithmic weighting of points of the shear data
-    weights1 = None#np.diff(np.log(x0), append=np.log(x0[-1] + dx))**2 #needs to be improved (based on spacing of data points in logarithmic space)
-
-    # weights1[:] = 1
-
-    def cost(p):
-        material = MaterialClass(*params(p))
-        # print(material)
-        offset = 0
-        for pp in p:
-            if pp < 0 :
-                offset += -pp
-        return fit_error(func(gamma1, material), data_shear1, weights1)+offset
-
-    def plot(p):
-        def plot_me():
-            material = MaterialClass(*params(p))
-            print(material, *params(p))
-            plt.plot(data_shear1[:, 0], data_shear1[:, 1], "o", label="data")
-
-            x, y = func(gamma1, material)
-            plt.plot(x, y, "r-", lw=3, label="model")
-        return plot_me
-
-    return cost, plot
-
-
-def minimize_old(cost_data: list, parameter_start: Sequence, method='Nelder-Mead', maxfev:int = 1e4, MaterialClass=SemiAffineFiberMaterial, x_sample=100, **kwargs):
-    costs = []
-    plots = []
-
-    for func, data, params in cost_data:
-        if func == getStretchThinning:
-            def func(x, material):
-                lambda_v = np.arange(0, 1.1, 0.01)
-                return getStretchThinning(x, lambda_v, material)
-        c, p = get_cost_function(func, data, params, x_sample=x_sample, MaterialClass=MaterialClass)
-        costs.append(c)
-        plots.append(p)
-
-    from tqdm import tqdm
-    pbar = tqdm(total=maxfev)
-
-    # define the cost function
-    def cost(p):
-        pbar.update(1)
-        return sum([c(p) for c in costs])
-
-    # minimize the cost with reasonable start parameters
-    from scipy.optimize import minimize
-    sol = minimize(cost, parameter_start, method=method, options={'maxfev': maxfev}, **kwargs)
-
-    if sol.success is True:
-        pbar.close()
-
-    def plot_all():
-        subplot_index = 0
-        subplot_dict = {}
-        for func, data, params in cost_data:
-            if func not in subplot_dict:
-                subplot_index += 1
-                subplot_dict[func] = subplot_index
-
-        for func in subplot_dict:
-            subplot_dict[func] = plt.subplot(1, subplot_index, subplot_dict[func])
-            if func == getShearRheometerStress or func == getExtensionalRheometerStress:
-                plt.xlabel("strain")
-                plt.ylabel("stress")
-            if func == getStretchThinning:
-                plt.xlabel("horizontal stretch")
-                plt.ylabel("vertical contraction")
-
-        for (func, data, params), p in zip(cost_data, plots):
-            plt.sca(subplot_dict[func])
-            p(sol.x)()
-
-    return sol.x, plot_all
-
-
-def getMaping(p, func, indices):
-    m = func(p)
-    mapping = []
-    for i in range(len(p)):
-        pp = p.copy()
-        pp[i] = pp[i]+1
-        mm = func(pp)
-        for i in indices:
-            if mm[i] != m[i]:
-                mapping.append(True)
-                break
-        else:
-            mapping.append(False)
-    return mapping
-
-
-def minimize(cost_data: list, parameter_start: Sequence, method='Powell', maxfev:int = 1e4, MaterialClass=SemiAffineFiberMaterial, x_sample=20, **kwargs):
-    parameter_start = np.array(parameter_start)
-
-    costs_shear = []
-    mapping_shear = np.array([False] * len(parameter_start))
-    plots_shear = []
-    costs_stretch = []
-    mapping_stretch = np.array([False] * len(parameter_start))
-    plots_stretch = []
-
-    for func, data, params in cost_data:
-        if func == getStretchThinning:
-            mapping_stretch |= getMaping(parameter_start, params, [1])
-
-            def getCost(func, data, params):
-                stretchx = data[:, 0]
-                stretchy = data[:, 1]
-
-                ###lambda_h = np.arange(1 - 0.05, 1 + 0.07, 0.01)
-                lambda_h = np.linspace(np.min(stretchx), np.max(stretchx), x_sample) ## fit complete input data regime
-                lambda_v = np.arange(0, 1.1, 0.001)
-
-                def cost(p):
-                    nonlocal parameter_start
-                    parameter_start = parameter_start.copy()
-                    parameter_start[mapping_stretch] = p
-                    p = params(parameter_start)
-                    material1 = MaterialClass(*p)
-                    x, y = getStretchThinning(lambda_h, lambda_v, material1)
-                    stretchy2 = interp1d(x, y, fill_value=np.nan, bounds_error=False)(stretchx)
-                    cost = np.nansum((stretchy2 - stretchy) ** 2)
-                    return cost
-
-                def plot_me():
-                    material = MaterialClass(*params(parameter_start))
-                    plt.plot(stretchx, stretchy, "o", label="data")
-
-                    x, y = getStretchThinning(lambda_h, lambda_v, material)
-                    plt.plot(x, y, "r-", lw=3, label="model")
-                return cost, plot_me
-            cost, plot = getCost(func, data, params)
-            costs_stretch.append(cost)
-            plots_stretch.append(plot)
-
-        if func == getShearRheometerStress:
-            mapping_shear |= getMaping(parameter_start, params, [0, 2, 3])
-
-            def getCost(func, data, params):
-                shearx = data[:, 0]
-                sheary = data[:, 1]
-
-                x0 = shearx
-                dx = x0[1] - x0[0]
-                weights = np.diff(np.log(x0), append=np.log(
-                    x0[-1] + dx)) ** 2  # needs to be improved (based on spacing of data points in logarithmic space)
-                gamma = np.linspace(np.min(x0), np.max(x0), x_sample)
-
-                def cost(p):
-                    nonlocal parameter_start
-                    parameter_start = parameter_start.copy()
-                    parameter_start[mapping_shear] = p
-                    p = params(parameter_start)
-                    material1 = MaterialClass(*p)
-                    x, y = getShearRheometerStress(gamma, material1)
-                    stretchy2 = interp1d(x, y, fill_value=np.nan, bounds_error=False)(shearx)
-                    cost = np.nansum((np.log(stretchy2) - np.log(sheary)) ** 2 * weights)
-                    return cost
-
-                def plot_me():
-                    material = MaterialClass(*params(parameter_start))
-                    plt.loglog(shearx, sheary, "o", label="data")
-
-                    x, y = getShearRheometerStress(gamma, material)
-                    plt.loglog(x, y, "r-", lw=3, label="model")
-
-                return cost, plot_me
-
-            cost, plot = getCost(func, data, params)
-            costs_shear.append(cost)
-            plots_shear.append(plot)
-
-    for i in range(5):
-        for mapping, costs in [[mapping_shear, costs_shear], [mapping_stretch, costs_stretch]]:
-            if len(costs) == 0:
-                continue
-            # define the cost function
-            def cost(p):
-                return sum([c(p) for c in costs])
-
-            # minimize the cost with reasonable start parameters
-            from scipy.optimize import minimize
-            sol = minimize(cost, parameter_start[mapping], method=method, options={'maxfev': maxfev}, **kwargs)
-            parameter_start[mapping] = sol["x"]
-
-        if len(costs_shear) == 0 or len(costs_stretch) == 0:
-            break
-
-    def plot_all():
-        subplot_count = (len(plots_stretch) > 0) + (len(plots_shear) > 0)
-        if len(plots_shear):
-            plt.subplot(1, subplot_count, 1)
-            for plot in plots_shear:
-                plot()
-            plt.xlabel("strain")
-            plt.ylabel("stress")
-        if len(plots_stretch):
-            plt.subplot(1, subplot_count, 1+(len(plots_stretch)>0))
-            for plot in plots_stretch:
-                plot()
-            plt.xlabel("horizontal stretch")
-            plt.ylabel("vertical contraction")
-
+import numpy as np
+from .build_beams import build_beams
+from .materials import Material
+from typing import Sequence
+from scipy.interpolate import interp1d
+
+
+def get_quadrature(n: int, x_min: float, x_max: float) -> (np.ndarray, np.ndarray):
+    """
+    Provides N quadrature points for an integration from x_min to x_max together with their weights.
+
+    Parameters
+    ----------
+    n : int
+        The number of quadrature points to use. Has to be 1 <= N <= 5.
+    x_min : float
+        The start of the integration range
+    x_max : float
+        The end of the integration range
+
+    Returns
+    -------
+    points : np.ndarray
+        The points of the quadrature
+    w : np.ndarray
+        The weights of the points
+    """
+    if n < 1:
+        raise ValueError()
+
+    if n == 1:
+        points = [0]
+        w = [2]
+
+    elif n == 2:
+        points = [-np.sqrt(1 / 3), np.sqrt(1 / 3)]
+        w = [1, 1]
+
+    elif n == 3:
+        points = [-np.sqrt(3 / 5), 0, np.sqrt(3 / 5)]
+        w = [5 / 9, 8 / 9, 5 / 9]
+
+    elif n == 4:
+        points = [-np.sqrt(3 / 7 - 2 / 7 * np.sqrt(6 / 5)), +np.sqrt(3 / 7 - 2 / 7 * np.sqrt(6 / 5)),
+                  -np.sqrt(3 / 7 + 2 / 7 * np.sqrt(6 / 5)), +np.sqrt(3 / 7 + 2 / 7 * np.sqrt(6 / 5))]
+        w = [(18 + np.sqrt(30)) / 36, (18 + np.sqrt(30)) / 36, (18 - np.sqrt(30)) / 36, (18 - np.sqrt(30)) / 36]
+
+    elif n == 5:
+        points = [0,
+                  -1 / 3 * np.sqrt(5 - 2 * np.sqrt(10 / 7)), +1 / 3 * np.sqrt(5 - 2 * np.sqrt(10 / 7)),
+                  -1 / 3 * np.sqrt(5 + 2 * np.sqrt(10 / 7)), +1 / 3 * np.sqrt(5 + 2 * np.sqrt(10 / 7))]
+        w = [128 / 225, (322 + 13 * np.sqrt(70)) / 900, (322 + 13 * np.sqrt(70)) / 900, (322 - 13 * np.sqrt(70)) / 900,
+             (322 - 13 * np.sqrt(70)) / 900]
+
+    else:
+        raise ValueError()
+
+    points = np.array(points)
+    w = np.array(w)
+    factor = (x_max - x_min) / 2
+    points = factor * points + (x_max + x_min) / 2
+    w = w * factor
+    return points, w
+
+
+def combine_quadrature(p1_w1: Sequence, p2_w2: Sequence) -> (np.ndarray, np.ndarray, np.ndarray):
+    """
+    Combine the quadratures of two different axes.
+
+    Parameters
+    ----------
+    p1_w1 : tuple
+        the points and weights for the first axis
+    p2_w2 : tuple
+        the points and weights for the second axis
+
+    Returns
+    -------
+    x : np.ndarray
+        the points for the first axis
+    y : np.ndarray
+        the points for the second axis
+    w : np.ndarray
+        the combined weights for the points
+    """
+    p1, w1 = p1_w1
+    p2, w2 = p2_w2
+    x, y = [f.ravel() for f in np.meshgrid(p1, p2)]
+    w = (w1[:, None] * w2[None, :]).ravel()
+    return x, y, w
+
+
+def get_shear_rheometer_stress(gamma: np.ndarray, material: Material, s: np.ndarray = None) -> (np.ndarray, np.ndarray):
+    r"""
+    This function returns the stress the material model generates when subjected to a shear strain,
+    as seen in a shear rheometer.
+
+    The shear strain is described using the following deformation gradient :math:`\mathbf{F}`:
+
+    .. math::
+        \mathbf{F}(\gamma) =
+        \begin{pmatrix}
+            1 & \gamma & 0 \\
+            0 & 1 & 0 \\
+            0 & 0 & 1 \\
+        \end{pmatrix}
+
+    and the resulting stress is obtained by calculating numerically the derivative of the energy density :math:`W` with
+    respect to the strain :math:`\gamma`:
+
+    .. math::
+        \sigma(\gamma) = \frac{dW(\mathbf{F}(\gamma))}{d\gamma}
+
+    Parameters
+    ----------
+    gamma : ndarray
+        The strain values for which to calculate the stress.
+    material : :py:class:`~.materials.Material`
+        The material model to use.
+
+    Returns
+    -------
+    strain : ndarray
+        The strain values.
+    stress : ndarray
+        The resulting stress.
+
+    """
+    if s is None:
+        s = build_beams(30)
+
+    F = np.eye(3)
+    F = np.tile(F, (gamma.shape[0], 1, 1))
+    F[:, 0, 1] = gamma
+
+    s_bar = F @ s.T
+
+    s_abs = np.linalg.norm(s_bar, axis=-2)
+
+    eps = material.energy(s_abs - 1)
+
+    W = np.mean(eps, axis=-1)
+    dW = np.diff(W) / np.diff(gamma)
+    return gamma[:-1] + np.diff(gamma) / 2, dW
+
+
+def get_shear_rheometer_stress_rotation(gamma, material, H=1e-3, R=10e-3, s=30, q=2):
+    if isinstance(s, int):
+        s = build_beams(s)
+
+    x_r, z_h, w = combine_quadrature(get_quadrature(q, 0, 1), get_quadrature(q, 0, 1))
+
+    F = np.zeros((gamma.shape[0], len(z_h), 3, 3))
+    theta = gamma * H / R
+    theta_p = theta[:, None] * z_h[None, :]
+
+    cos, sin = np.cos(theta_p), np.sin(theta_p)
+    xtheta_h = x_r * theta[:, None] * R / H
+    F[:, :, 0, 0], F[:, :, 0, 1], F[:, :, 0, 2] = cos, -sin, -sin * xtheta_h
+    F[:, :, 1, 0], F[:, :, 1, 1], F[:, :, 1, 2] = sin, cos, cos * xtheta_h
+    F[:, :, 2, 2] = 1
+
+    s_bar = F @ s.T
+
+    s_abs = np.linalg.norm(s_bar, axis=-2)
+    eps = material.energy(s_abs - 1)
+
+    W = np.mean(eps, axis=-1)
+    W = np.average(W, axis=-1, weights=w)
+    dW = np.diff(W) / np.diff(gamma)
+
+    return gamma[:-1] + np.diff(gamma) / 2, dW
+
+
+def get_stretch_thinning(gamma_h, gamma_v, material, s=None):
+    r"""
+    This function returns the vertical thinning (strain in z direction) of the material model
+    when the material model is stretched horizontally (strain in x direction), as seen in a stretcher device.
+
+    The strain in x and z direction is described using the following deformation gradient :math:`\mathbf{F}`:
+
+    .. math::
+        \mathbf{F}(\gamma) =
+        \begin{pmatrix}
+            \gamma_h & 0 & 0 \\
+            0 & 1 & 0 \\
+            0 & 0 & \gamma_v \\
+        \end{pmatrix}
+
+    the resulting energy density :math:`W(\mathbf{F}(\gamma_h,\gamma_v))` is then minimized numerically for every
+    :math:`\gamma_h` to obtain the :math:`\gamma_v` that results in the lowest energy of the system.
+
+    Parameters
+    ----------
+    gamma_h : ndarray
+        The applied strain in horizontal direction.
+    gamma_v : ndarray
+        The different values for thinning to test. The value with the lowest energy for each horizontal strain is
+        returned.
+    material : :py:class:`~.materials.Material`
+        The material model to use.
+
+    Returns
+    -------
+    gamma_h : ndarray
+        The horizontal strain values.
+    gamma_v : ndarray
+        The vertical strain that minimizes the energy for the horizontal strain.
+    """
+    if s is None:
+        s = build_beams(30)
+
+    F00, F22 = np.meshgrid(gamma_v, gamma_h)
+    F11 = np.ones_like(F00)
+    F = np.dstack((F00, F11, F22))
+
+    s_bar = np.einsum("hvj,bj->hvjb", F, s)
+    s_abs = np.linalg.norm(s_bar, axis=-2)
+    eps = material.energy(s_abs - 1)
+    W = np.mean(eps, axis=-1)
+
+    index = np.argmin(W, axis=1)
+    return gamma_h, gamma_v[index]
+
+
+def get_extensional_rheometer_stress(gamma, material, s=None):
+    r"""
+    This function returns the stress the material model generates when subjected to an extensional strain,
+    as seen in an extensional rheometer.
+
+    The extensional strain is described using the following deformation gradient :math:`\mathbf{F}`:
+
+    .. math::
+        \mathbf{F}(\gamma) =
+        \begin{pmatrix}
+            \gamma & 0 & 0 \\
+            0 & 1 & 0 \\
+            0 & 0 & 1 \\
+        \end{pmatrix}
+
+    and the resulting stress is obtained by calculating numerically the derivative of the energy density :math:`W` with
+    respect to the strain :math:`\gamma`:
+
+    .. math::
+        \sigma(\gamma) = \frac{dW(\mathbf{F}(\gamma))}{d\gamma}
+
+
+    Parameters
+    ----------
+    gamma : ndarray
+        The strain values for which to calculate the stress.
+    material : :py:class:`~.materials.Material`
+        The material model to use.
+
+    Returns
+    -------
+    strain : ndarray
+        The strain values.
+    stress : ndarray
+        The resulting stress.
+    """
+    if s is None:
+        s = build_beams(30)
+
+    F = np.eye(3)
+    F = np.tile(F, (gamma.shape[0], 1, 1))
+    F[:, 0, 0] = gamma
+
+    s_bar = F @ s.T
+
+    s_abs = np.linalg.norm(s_bar, axis=-2)
+
+    eps = material.energy(s_abs - 1)
+
+    W = np.mean(eps, axis=-1)
+    dW = np.diff(W) / np.diff(gamma)
+    return gamma[:-1] + np.diff(gamma) / 2, dW
+
+
+import numpy as np
+from scipy import interpolate
+import matplotlib.pyplot as plt
+from saenopy.materials import SemiAffineFiberMaterial
+
+def fit_error(xy, xy0, w=None):
+    # split the data
+    x, y = xy
+    x0, y0 = xy0.tetrahedra
+    # interpolate the fit to ensure we have values at the correct x positions
+    f = interpolate.interp1d(x, y, bounds_error=False)
+    # evaluate the interpolated fit at the x0 values and calculate the squared difference to the y0 values
+    difference = (y0-f(x0))**2
+    # if we have no weights
+    if w is None:
+        # just take the mean (ignoring nans)
+        return np.sqrt(np.nanmean(difference/np.nanmax(y0)))
+    # if not ignore the nans by finding the indices
+    indices = ~np.isnan(difference)
+    # and average with the given weights
+    return np.sqrt(np.average(difference[indices]/np.nanmax(y0[indices]), weights=w[indices]))
+
+
+def get_cost_function(func, data_shear1, params, MaterialClass, x_sample=100):
+    # find a reasonable range of shear values
+    x0 = data_shear1[:, 0]
+    dx = x0[1] - x0[0]
+    gamma1 = np.linspace(np.min(x0), np.max(x0), x_sample)
+
+    # define weights for logarithmic weighting of points of the shear data
+    weights1 = None#np.diff(np.log(x0), append=np.log(x0[-1] + dx))**2 #needs to be improved (based on spacing of data points in logarithmic space)
+
+    # weights1[:] = 1
+
+    def cost(p):
+        material = MaterialClass(*params(p))
+        # print(material)
+        offset = 0
+        for pp in p:
+            if pp < 0 :
+                offset += -pp
+        return fit_error(func(gamma1, material), data_shear1, weights1)+offset
+
+    def plot(p):
+        def plot_me():
+            material = MaterialClass(*params(p))
+            print(material, *params(p))
+            plt.plot(data_shear1[:, 0], data_shear1[:, 1], "o", label="data")
+
+            x, y = func(gamma1, material)
+            plt.plot(x, y, "r-", lw=3, label="model")
+        return plot_me
+
+    return cost, plot
+
+
+def minimize_old(cost_data: list, parameter_start: Sequence, method='Nelder-Mead', maxfev:int = 1e4, MaterialClass=SemiAffineFiberMaterial, x_sample=100, **kwargs):
+    costs = []
+    plots = []
+
+    for func, data, params in cost_data:
+        if func == get_stretch_thinning:
+            def func(x, material):
+                lambda_v = np.arange(0, 1.1, 0.01)
+                return get_stretch_thinning(x, lambda_v, material)
+        c, p = get_cost_function(func, data, params, x_sample=x_sample, MaterialClass=MaterialClass)
+        costs.append(c)
+        plots.append(p)
+
+    from tqdm import tqdm
+    pbar = tqdm(total=maxfev)
+
+    # define the cost function
+    def cost(p):
+        pbar.update(1)
+        return sum([c(p) for c in costs])
+
+    # minimize the cost with reasonable start parameters
+    from scipy.optimize import minimize
+    sol = minimize(cost, parameter_start, method=method, options={'maxfev': maxfev}, **kwargs)
+
+    if sol.success is True:
+        pbar.close()
+
+    def plot_all():
+        subplot_index = 0
+        subplot_dict = {}
+        for func, data, params in cost_data:
+            if func not in subplot_dict:
+                subplot_index += 1
+                subplot_dict[func] = subplot_index
+
+        for func in subplot_dict:
+            subplot_dict[func] = plt.subplot(1, subplot_index, subplot_dict[func])
+            if func == get_shear_rheometer_stress or func == get_extensional_rheometer_stress:
+                plt.xlabel("strain")
+                plt.ylabel("stress")
+            if func == get_stretch_thinning:
+                plt.xlabel("horizontal stretch")
+                plt.ylabel("vertical contraction")
+
+        for (func, data, params), p in zip(cost_data, plots):
+            plt.sca(subplot_dict[func])
+            p(sol.x)()
+
+    return sol.x, plot_all
+
+
+def get_maping(p, func, indices):
+    m = func(p)
+    mapping = []
+    for i in range(len(p)):
+        pp = p.copy()
+        pp[i] = pp[i]+1
+        mm = func(pp)
+        for i in indices:
+            if mm[i] != m[i]:
+                mapping.append(True)
+                break
+        else:
+            mapping.append(False)
+    return mapping
+
+
+def minimize(cost_data: list, parameter_start: Sequence, method='Powell', maxfev:int = 1e4, MaterialClass=SemiAffineFiberMaterial, x_sample=20, colors=None, **kwargs):
+    parameter_start = np.array(parameter_start)
+
+    costs_shear = []
+    mapping_shear = np.array([False] * len(parameter_start))
+    plots_shear = []
+    costs_stretch = []
+    mapping_stretch = np.array([False] * len(parameter_start))
+    plots_stretch = []
+
+    index = 0
+    for func, data, params in cost_data:
+        color = None
+        if colors is not None:
+            color = colors[index]
+            index += 1
+        if func == get_stretch_thinning:
+            mapping_stretch |= get_maping(parameter_start, params, [1])
+
+            def getCost(func, data, params):
+                stretchx = data[:, 0]
+                stretchy = data[:, 1]
+
+                ###lambda_h = np.arange(1 - 0.05, 1 + 0.07, 0.01)
+                lambda_h = np.linspace(np.min(stretchx), np.max(stretchx), x_sample) ## fit complete input data regime
+                lambda_v = np.arange(0, 1.1, 0.001)
+
+                def cost(p):
+                    nonlocal parameter_start
+                    parameter_start = parameter_start.copy()
+                    parameter_start[mapping_stretch] = p
+                    p = params(parameter_start)
+                    material1 = MaterialClass(*p)
+                    x, y = get_stretch_thinning(lambda_h, lambda_v, material1)
+                    stretchy2 = interp1d(x, y, fill_value=np.nan, bounds_error=False)(stretchx)
+                    cost = np.nansum((stretchy2 - stretchy) ** 2)
+                    return cost
+
+                def plot_me(color=color):
+                    material = MaterialClass(*params(parameter_start))
+                    plt.plot(stretchx, stretchy, "o", label="data", color=color)
+
+                    x, y = get_stretch_thinning(lambda_h, lambda_v, material)
+                    plt.plot(x, y, "r-", lw=3, label="model")
+                return cost, plot_me
+            cost, plot = getCost(func, data, params)
+            costs_stretch.append(cost)
+            plots_stretch.append(plot)
+
+        if func == get_shear_rheometer_stress:
+            mapping_shear |= get_maping(parameter_start, params, [0, 2, 3])
+
+            def get_cost(func, data, params):
+                shearx = data[:, 0]
+                sheary = data[:, 1]
+
+                x0 = shearx
+                dx = x0[1] - x0[0]
+                weights = np.diff(np.log(x0), append=np.log(
+                    x0[-1] + dx)) ** 2  # needs to be improved (based on spacing of data points in logarithmic space)
+                gamma = np.linspace(np.min(x0), np.max(x0), x_sample)
+
+                def cost(p):
+                    nonlocal parameter_start
+                    parameter_start = parameter_start.copy()
+                    parameter_start[mapping_shear] = p
+                    p = params(parameter_start)
+                    material1 = MaterialClass(*p)
+                    x, y = get_shear_rheometer_stress(gamma, material1)
+                    stretchy2 = interp1d(x, y, fill_value=np.nan, bounds_error=False)(shearx)
+                    cost = np.nansum((np.log(stretchy2) - np.log(sheary)) ** 2 * weights)
+                    return cost
+
+                def plot_me(color=color):
+                    material = MaterialClass(*params(parameter_start))
+                    plt.loglog(shearx, sheary, "o", label="data", color=color)
+
+                    x, y = get_shear_rheometer_stress(gamma, material)
+                    plt.loglog(x, y, "r-", lw=3, label="model")
+
+                return cost, plot_me
+
+            cost, plot = get_cost(func, data, params)
+            costs_shear.append(cost)
+            plots_shear.append(plot)
+
+    for i in range(5):
+        for mapping, costs in [[mapping_shear, costs_shear], [mapping_stretch, costs_stretch]]:
+            if len(costs) == 0:
+                continue
+            # define the cost function
+            def cost(p):
+                return sum([c(p) for c in costs])
+
+            # minimize the cost with reasonable start parameters
+            from scipy.optimize import minimize
+            sol = minimize(cost, parameter_start[mapping], method=method, options={'maxfev': maxfev}, **kwargs)
+            parameter_start[mapping] = sol["x"]
+
+        if len(costs_shear) == 0 or len(costs_stretch) == 0:
+            break
+
+    def plot_all():
+        subplot_count = (len(plots_stretch) > 0) + (len(plots_shear) > 0)
+        if len(plots_shear):
+            plt.subplot(1, subplot_count, 1)
+            for plot in plots_shear:
+                plot()
+            plt.xlabel("strain")
+            plt.ylabel("stress")
+        if len(plots_stretch):
+            plt.subplot(1, subplot_count, 1+(len(plots_stretch)>0))
+            for plot in plots_stretch:
+                plot()
+            plt.xlabel("horizontal stretch")
+            plt.ylabel("vertical contraction")
+
     return parameter_start, plot_all
```

### Comparing `saenopy-0.9.0/saenopy/materials.py` & `saenopy-1.0.0/saenopy/materials.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,14 @@
 import numpy as np
 from numba import njit
 import numba
 from saenopy.saveable import Saveable
 
 
-def saveEpsilon(epsilon, fname, CFG):
-    """
-    Save the material function to a file, e.g. for further plotting.
-    """
-    imax = int(np.ceil((CFG["EPSMAX"] + 1.0) / CFG["EPSSTEP"]))
-
-    with open(fname, "w") as fp:
-        for i in range(imax):
-            lambd = (i * CFG["EPSSTEP"]) - 1.0
-
-            fp.write(str(lambd) + " " + str(epsilon[i]) + "\n")
-
-    lambd = (np.arange(imax) * CFG["EPSSTEP"]) - 1.0
-    np.save(fname.replace(".dat", ".npy"), np.array([lambd, epsilon]).T)
-
-
-def sampleAndIntegrateFunction(func, min, max, step, zero_point=0, maximal_value=10e10):
-    def iToX(i):
-        return i * step + min
-
+def sample_and_integrate_function(func, min, max, step, zero_point=0, maximal_value=10e10):
     def xToI(x):
         return np.ceil((x - min) / step).astype(int)
 
     x = np.arange(min, max, step)
     y = func(x)
 
     if maximal_value is not None:
@@ -38,15 +19,15 @@
     int_y -= int_y[xToI(zero_point)]
 
     # integrate again
     int_int_y = np.cumsum(int_y * step)
     int_int_y -= int_int_y[xToI(zero_point)]
 
     @njit()
-    def lookUpY(x):
+    def look_up_y(x):
         shape = x.shape
         x = x.flatten()
         # we now have to pass this though the non-linearity function w (material model)
         # this function has been discretized and we interpolate between these discretisation steps
 
         # the discretisation step
         li = np.floor((x - min) / step)
@@ -65,32 +46,40 @@
         # interpolate between the two discretisation steps
         res0 = (1 - dli) * int_int_y[lii] + dli * int_int_y[lii + 1]
         res1 = (1 - dli) * int_y[lii] + dli * int_y[lii + 1]
         res2 = (1 - dli) * y[lii] + dli * y[lii + 1]
 
         return res0.reshape(shape), res1.reshape(shape), res2.reshape(shape)
 
-    return lookUpY
+    return look_up_y
 
 
 class Material:
     """
     The base class for all material models.
     """
     parameters = {}
     min = -1.0
     max = 4.0
     step = 0.000001
 
     def stiffness(self, s):
         # to be overloaded by a material implementation
-        return s
+        raise NotImplementedError
+
+    def energy(self, param):
+        # to be overloaded by a material implementation
+        raise NotImplementedError
+
+    def force(self, param):
+        # to be overloaded by a material implementation
+        raise NotImplementedError
 
     def generate_look_up_table(self):
-        return sampleAndIntegrateFunction(self.stiffness, self.min, self.max, self.step)
+        return sample_and_integrate_function(self.stiffness, self.min, self.max, self.step)
 
     def __str__(self):
         return self.__class__.__name__+"("+", ".join(key+"="+str(value) for key, value in self.parameters.items())+")"
 
 
 class SemiAffineFiberMaterial(Material, Saveable):
     """
@@ -98,246 +87,237 @@
     -1 < lambda < 0, a linear stiffness response for small strains 0 < lambda < lambda_s, and strain stiffening for
     large strains lambda_s < lambda.
 
     Parameters
     ----------
     k : float
         The stiffness of the material in the linear regime.
-    d0 : float, optional
+    d_0 : float, optional
         The decay parameter in the buckling regime. If omitted the material shows no buckling but has a linear response
         for compression.
     lambda_s : float, optional
         The stretching where the strain stiffening starts. If omitted the material shows no strain stiffening.
-    ds : float, optional
+    d_s : float, optional
         The parameter specifying how strong the strain stiffening is. If omitted the material shows no strain
         stiffening.
     """
-    __save_parameters__ = ["k", "d0", "lambda_s", "ds"]
+    __save_parameters__ = ["k", "d_0", "lambda_s", "d_s"]
     k: float = None
-    d0: float = None
+    d_0: float = None
     lambda_s: float = None
-    ds: float = None
+    d_s: float = None
 
-    def serialize(self):
-        return ["SemiAffineFiberMaterial", self.k, self.d0, self.lambda_s, self.ds]
-
-    def __init__(self, k, d0=None, lambda_s=None, ds=None):
+    def __init__(self, k, d_0=None, lambda_s=None, d_s=None):
+        super().__init__()
         # parameters
         self.k = k
-        self.d0 = d0 if d0 is not None and d0 >= 0 else None    
+        self.d_0 = d_0 if d_0 is not None and d_0 >= 0 else None
         # buckling None (constant stiffness) and buckling zero (drop in stiffness) is not the same 
-        if self.d0 is not None and self.d0 < 1e-30:  # approximate the zero case
-            self.d0 = 1e-30
+        if self.d_0 is not None and self.d_0 < 1e-30:  # approximate the zero case
+            self.d_0 = 1e-30
         self.lambda_s = lambda_s if lambda_s is not None and lambda_s >= 0 else None
-        self.ds = ds if ds is not None and ds >= 0 else None
-        self.parameters = dict(k=k, d0=d0, lambda_s=lambda_s, ds=ds)
+        self.d_s = d_s if d_s is not None and d_s >= 0 else None
+        self.parameters = dict(k=k, d_0=d_0, lambda_s=lambda_s, d_s=d_s)
 
     def stiffness(self, s):
-        self._check_parameters_valid()
-
         # the linear spring regime (1 < s < s1)
         stiff = np.ones_like(s) * self.k
 
         # buckling for compression
-        if self.d0 is not None:
+        if self.d_0 is not None:
             buckling = s < 0
-            stiff[buckling] = self.k * np.exp(s[buckling] / self.d0)
+            stiff[buckling] = self.k * np.exp(s[buckling] / self.d_0)
 
         # and exponential stretch for overstretching fibers
-        if self.ds is not None and self.lambda_s is not None:
+        if self.d_s is not None and self.lambda_s is not None:
             stretching = s > self.lambda_s
-            stiff[stretching] = self.k * np.exp((s[stretching] - self.lambda_s) / self.ds)
+            stiff[stretching] = self.k * np.exp((s[stretching] - self.lambda_s) / self.d_s)
 
         return stiff
 
     def energy(self, x0):
-        self._check_parameters_valid()
-
         # generate an empty target array
         x = x0.ravel()
         y = np.zeros_like(x)
 
         # find the buckling range
-        if self.d0 is not None:
+        if self.d_0 is not None:
             buckling = x < 0
         else:
             buckling = np.zeros_like(x) == 1
         # find the stretching range
-        if self.ds is not None and self.lambda_s is not None:
+        if self.d_s is not None and self.lambda_s is not None:
             stretching = self.lambda_s <= x
         else:
             stretching = np.zeros_like(x) == 1
         # and the rest is the linear range
         linear = (~buckling) & (~stretching)
 
-        if self.d0 is not None:
+        if self.d_0 is not None:
             # calculate the buckling energy
-            y[buckling] = self.k * self.d0 ** 2 * np.exp(x[buckling] / self.d0) - self.k * self.d0 * x[
-                buckling] - self.k * self.d0 ** 2
+            y[buckling] = self.k * self.d_0 ** 2 * np.exp(x[buckling] / self.d_0) - self.k * self.d_0 * x[
+                buckling] - self.k * self.d_0 ** 2
 
         # calculate the energy in the linear range
         y[linear] = 0.5 * self.k * x[linear] ** 2
 
-        if self.ds is not None and self.lambda_s is not None:
+        if self.d_s is not None and self.lambda_s is not None:
             # and in the stretching range
-            dk = self.ds * self.k
+            dk = self.d_s * self.k
             sk = self.lambda_s * self.k
-            d2k = self.ds * dk
-            y[stretching] = - 0.5 * self.lambda_s ** 2 * self.k + self.ds * self.k * self.lambda_s - d2k \
-                            + d2k * np.exp((x[stretching] - self.lambda_s) / self.ds) - dk * x[stretching] + sk * x[
+            d2k = self.d_s * dk
+            y[stretching] = - 0.5 * self.lambda_s ** 2 * self.k + self.d_s * self.k * self.lambda_s - d2k \
+                            + d2k * np.exp((x[stretching] - self.lambda_s) / self.d_s) - dk * x[stretching] + sk * x[
                                 stretching]
 
         # return the resulting energy
         return y.reshape(x0.shape)
 
     def force(self, x0):
-        self._check_parameters_valid()
-
         # generate an empty target array
         x = x0.ravel()
         y = np.zeros_like(x)
 
         # find the buckling range
-        if self.d0 is not None:
+        if self.d_0 is not None:
             buckling = x < 0
         else:
             buckling = np.zeros_like(x) == 1
         # find the stretching range
-        if self.ds is not None and self.lambda_s is not None:
+        if self.d_s is not None and self.lambda_s is not None:
             stretching = self.lambda_s <= x
         else:
             stretching = np.zeros_like(x) == 1
         # and the rest is the linear range
         linear = (~buckling) & (~stretching)
 
-        if self.d0 is not None:
+        if self.d_0 is not None:
             # calculate the buckling energy
-            y[buckling] = self.k * self.d0 * np.exp(x[buckling] / self.d0) - self.d0 * self.k
+            y[buckling] = self.k * self.d_0 * np.exp(x[buckling] / self.d_0) - self.d_0 * self.k
 
         # calculate the energy in the linear range
         y[linear] = self.k * x[linear]
-        if self.ds is not None and self.lambda_s is not None:
-            y[stretching] = self.k * self.lambda_s - self.ds * self.k + self.ds * self.k * np.exp(
-                (x[stretching] - self.lambda_s) / self.ds)
+        if self.d_s is not None and self.lambda_s is not None:
+            y[stretching] = self.k * self.lambda_s - self.d_s * self.k + self.d_s * self.k * np.exp(
+                (x[stretching] - self.lambda_s) / self.d_s)
 
         # return the resulting energy
         return y.reshape(x0.shape)
 
-    def _check_parameters_valid(self):
-        # stiffening is not allowed in the buckling regime
-        if self.lambda_s is not None and self.lambda_s <= 0:
-            self.lambda_s = 0
-
     def generate_look_up_table(self):
-        self._check_parameters_valid()
-
-        d0 = self.d0
+        d_0 = self.d_0
         lambda_s = self.lambda_s
-        ds = self.ds
+        d_s = self.d_s
         k = self.k
 
-        if self.d0 is None and self.ds is not None:
+        buckling = self.d_0 is not None
+        strain_stiffening = (self.lambda_s is not None and self.d_s is not None)
+
+        # no buckling but strain stiffening
+        if not buckling and strain_stiffening:
             @njit(numba.core.types.containers.UniTuple(numba.float64[:, :], 3)(numba.float64[:, :]))
             def get_all(s):
                 shape = s.shape
                 s = s.flatten()
 
                 stiff = np.zeros_like(s)
                 force = np.zeros_like(s)
                 energy = np.zeros_like(s)
 
-                dk = ds * k
+                dk = d_s * k
                 sk = lambda_s * k
-                d2k = ds * dk
+                d2k = d_s * dk
 
                 for i, x in enumerate(s):
                     if x < lambda_s:
                         stiff[i] = k
                         force[i] = k * x
                         energy[i] = 0.5 * k * x ** 2
                     else:
-                        stiff[i] = k * np.exp((x - lambda_s) / ds)
-                        force[i] = k * lambda_s - ds * k + ds * k * np.exp((x - lambda_s) / ds)
-                        energy[i] = - 0.5 * lambda_s ** 2 * k + ds * k * lambda_s - d2k + d2k * np.exp(
-                            (x - lambda_s) / ds) - dk * x + sk * x
+                        stiff[i] = k * np.exp((x - lambda_s) / d_s)
+                        force[i] = k * lambda_s - d_s * k + d_s * k * np.exp((x - lambda_s) / d_s)
+                        energy[i] = - 0.5 * lambda_s ** 2 * k + d_s * k * lambda_s - d2k + d2k * np.exp(
+                            (x - lambda_s) / d_s) - dk * x + sk * x
 
                 return energy.reshape(shape), force.reshape(shape), stiff.reshape(shape)
 
             return get_all
 
-        if self.ds is None and self.lambda_s is None:
+        # buckling but no strain stiffening
+        if buckling and not strain_stiffening:
             @njit(numba.core.types.containers.UniTuple(numba.float64[:, :], 3)(numba.float64[:, :]))
             def get_all(s):
                 shape = s.shape
                 s = s.flatten()
 
                 stiff = np.zeros_like(s)
                 force = np.zeros_like(s)
                 energy = np.zeros_like(s)
 
                 for i, x in enumerate(s):
-                    stiff[i] = k
-                    force[i] = k * x
-                    energy[i] = 0.5 * k * x ** 2
+                    if x < 0:
+                        stiff[i] = k * np.exp(x / d_0)
+                        force[i] = k * d_0 * np.exp(x / d_0) - d_0 * k
+                        energy[i] = k * d_0 ** 2 * np.exp(x / d_0) - k * d_0 * x - k * d_0 ** 2
+                    else:
+                        stiff[i] = k
+                        force[i] = k * x
+                        energy[i] = 0.5 * k * x ** 2
 
                 return energy.reshape(shape), force.reshape(shape), stiff.reshape(shape)
 
             return get_all
 
-        if self.lambda_s is None and self.d0 is not None:
+        # no buckling and no strain stiffening
+        if not buckling and not strain_stiffening:
             @njit(numba.core.types.containers.UniTuple(numba.float64[:, :], 3)(numba.float64[:, :]))
             def get_all(s):
                 shape = s.shape
                 s = s.flatten()
 
                 stiff = np.zeros_like(s)
                 force = np.zeros_like(s)
                 energy = np.zeros_like(s)
 
                 for i, x in enumerate(s):
-                    if x < 0:
-                        stiff[i] = k * np.exp(x / d0)
-                        force[i] = k * d0 * np.exp(x / d0) - d0 * k
-                        energy[i] = k * d0 ** 2 * np.exp(x / d0) - k * d0 * x - k * d0 ** 2
-                    else:
-                        stiff[i] = k
-                        force[i] = k * x
-                        energy[i] = 0.5 * k * x ** 2
+                    stiff[i] = k
+                    force[i] = k * x
+                    energy[i] = 0.5 * k * x ** 2
 
                 return energy.reshape(shape), force.reshape(shape), stiff.reshape(shape)
 
             return get_all
 
         @njit(numba.core.types.containers.UniTuple(numba.float64[:, :], 3)(numba.float64[:, :]))
         def get_all(s):
             shape = s.shape
             s = s.flatten()
 
             stiff = np.zeros_like(s)
             force = np.zeros_like(s)
             energy = np.zeros_like(s)
 
-            dk = ds * k
+            dk = d_s * k
             sk = lambda_s * k
-            d2k = ds * dk
+            d2k = d_s * dk
 
             for i, x in enumerate(s):
                 if x < 0:
-                    stiff[i] = k * np.exp(x / d0)
-                    force[i] = k * d0 * np.exp(x / d0) - d0 * k
-                    energy[i] = k * d0 ** 2 * np.exp(x / d0) - k * d0 * x - k * d0 ** 2
+                    stiff[i] = k * np.exp(x / d_0)
+                    force[i] = k * d_0 * np.exp(x / d_0) - d_0 * k
+                    energy[i] = k * d_0 ** 2 * np.exp(x / d_0) - k * d_0 * x - k * d_0 ** 2
                 elif x < lambda_s:
                     stiff[i] = k
                     force[i] = k * x
                     energy[i] = 0.5 * k * x ** 2
                 else:
-                    stiff[i] = k * np.exp((x - lambda_s) / ds)
-                    force[i] = k * lambda_s - ds * k + ds * k * np.exp((x - lambda_s) / ds)
-                    energy[i] = - 0.5 * lambda_s ** 2 * k + ds * k * lambda_s - d2k + d2k * np.exp(
-                        (x - lambda_s) / ds) - dk * x + sk * x
+                    stiff[i] = k * np.exp((x - lambda_s) / d_s)
+                    force[i] = k * lambda_s - d_s * k + d_s * k * np.exp((x - lambda_s) / d_s)
+                    energy[i] = - 0.5 * lambda_s ** 2 * k + d_s * k * lambda_s - d2k + d2k * np.exp(
+                        (x - lambda_s) / d_s) - dk * x + sk * x
 
             return energy.reshape(shape), force.reshape(shape), stiff.reshape(shape)
 
         return get_all
 
 
 class LinearMaterial(Material):
@@ -356,10 +336,13 @@
 
     def stiffness(self, s):
         # the linear spring regime (0 < s < s1)
         stiff = np.ones_like(s) * self.k
 
         return stiff
 
+    def force(self, x):
+        return self.k * x
+
     def energy(self, x):
         # calculate the energy in the linear range
         return 0.5 * self.k * x ** 2
```

### Comparing `saenopy-0.9.0/saenopy/saveable.py` & `saenopy-1.0.0/saenopy/saveable.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,72 +9,94 @@
         for name in kwargs:
             if name in self.__save_parameters__:
                 setattr(self, name, kwargs[name])
 
     def to_dict(self):
         data = {}
         for param in self.__save_parameters__:
-            attribute = getattr(self, param, None)
-            if attribute is not None:
-                if getattr(attribute, "to_dict", None) is not None:
-                    data[param] = getattr(attribute, "to_dict")()
-                elif isinstance(attribute, list) and len(attribute) and (getattr(attribute[0], "to_dict", None) is not None or attribute[0] is None):
-                    my_list = []
-                    for attr in attribute:
-                        value = attr
-                        if getattr(attribute[0], "to_dict", None):
-                            value = getattr(attr, "to_dict")()
-                        if attr is None:
-                            value = "__NONE__"
-                        my_list.append(value)
-                    data[param] = my_list
-                elif attribute is None:
-                    data[param] = "__NONE__"
-                else:
-                    data[param] = attribute
+            attribute = getattr(self, param)
+            if getattr(attribute, "to_dict", None) is not None:
+                data[param] = getattr(attribute, "to_dict")()
+            elif isinstance(attribute, list) and len(attribute) and (getattr(attribute[0], "to_dict", None) is not None or attribute[0] is None):
+                my_list = []
+                for attr in attribute:
+                    value = attr
+                    if getattr(attribute[0], "to_dict", None):
+                        value = getattr(attr, "to_dict")()
+                    if attr is None:
+                        value = "__NONE__"
+                    my_list.append(value)
+                data[param] = my_list
+            elif attribute is None:
+                data[param] = "__NONE__"
+            else:
+                data[param] = attribute
         return data
 
-    def save(self, filename: str):
+    def save(self, filename: str, file_format=None):
+        from pathlib import Path
+        if file_format is None:
+            file_format = Path(filename).suffix
+
         data = self.to_dict()
 
-        if filename.endswith("h5py") or filename.endswith("h5"):
+        if file_format == ".h5py" or file_format == ".h5":  # pragma: no cover
             return dict_to_h5(filename, flatten_dict(data))
-
-        #np.savez(filename, **data)
-        np.lib.npyio._savez(filename, [], flatten_dict(data), True, allow_pickle=False)
+        elif file_format == ".npz" or file_format == ".saenopy":
+            #np.savez(filename, **data)
+            np.lib.npyio._savez(filename, [], flatten_dict(data), True, allow_pickle=False)
+            import shutil
+            if file_format == ".saenopy":
+                shutil.move(filename+".npz", filename)
+        else:
+            raise ValueError("format not supported")
 
     @classmethod
     def from_dict(cls, data_dict):
         types = typing.get_type_hints(cls)
         data = {}
+        save_parameters = cls.__save_parameters__.copy()
         for name in data_dict:
+            if name not in cls.__save_parameters__:
+                raise ValueError(f"Cannot load {name}")
+            save_parameters.remove(name)
             if isinstance(data_dict[name], np.ndarray) and len(data_dict[name].shape) == 0:
                 data[name] = data_dict[name][()]
             else:
                 data[name] = data_dict[name]
             if name in types:
                 if getattr(types[name], "from_dict", None) is not None:
-                    data[name] = types[name].from_dict(data[name])
+                    if data[name] is not None:
+                        data[name] = types[name].from_dict(data[name])
                 elif typing.get_origin(types[name]) is list:
                     if isinstance(data[name], dict):
                         data[name] = typing.get_args(types[name])[0].from_dict(data[name])
+                    elif data[name] is None:
+                        pass
                     else:
-                        data[name] = [None if d == "__NONE__" else typing.get_args(types[name])[0].from_dict(d) for d in data[name]]
+                        data[name] = [None if d == "__NONE__" or d is None else typing.get_args(types[name])[0].from_dict(d) for d in data[name]]
+        if len(save_parameters):
+            raise ValueError(f"The following parameters were not found in the save file {save_parameters}")
         return cls(**data)
 
     @classmethod
-    def load(cls, filename):
-        if str(filename).endswith(".h5py") or str(filename).endswith(".h5"):
+    def load(cls, filename, file_format=None):
+        from pathlib import Path
+        if file_format is None:
+            file_format = Path(filename).suffix
+        if file_format == ".h5py" or file_format == ".h5":  # pragma: no cover
             import h5py
             data = h5py.File(filename, "a")
             result = cls.from_dict(unflatten_dict_h5(data))
-        else:
+        elif file_format == ".npz" or file_format == ".saenopy":
             data = np.load(filename, allow_pickle=False)
 
             result = cls.from_dict(unflatten_dict(data))
+        else:
+            raise ValueError("Unknown format")
         if getattr(result, 'on_load', None) is not None:
             getattr(result, 'on_load')(filename)
         return result
 
 
 def flatten_dict(data):
     result = {}
@@ -145,44 +167,47 @@
             if isinstance(item, str) and item == "__NONE__":
                 item = None
             r[names[-1]] = item
 
     return result
 
 
-def dict_to_h5(filename, data):
+def dict_to_h5(filename, data):  # pragma: no cover
     import h5py
     with h5py.File(filename, "w") as f:
         for key in data.keys():
             if isinstance(data[key], str):
                 if str(data[key]) == "list" or str(data[key]) == "dict" or str(data[key]) == "tuple":
                     grp = f.create_group(key)
                     grp.attrs["type"] = str(data[key])
                     continue
                 dset = f.create_dataset(key, data=str(data[key]))
-            elif str(data[key].dtype).startswith("<U"):
+            elif str(getattr(data[key], "dtype", "")).startswith("<U"):
                 dset = f.create_dataset(key, data=str(data[key]))
             else:
                 try:
                     f.create_dataset(key, data=data[key], compression="gzip")
                 except TypeError:
                     f.create_dataset(key, data=data[key])
 
 
-def unflatten_dict_h5(data):
+def unflatten_dict_h5(data):  # pragma: no cover
     import h5py
     if isinstance(data, h5py.Group):
         if data.attrs.get("type") == "list":
             result = [unflatten_dict_h5(v) for v in data.values()]
         elif data.attrs.get("type") == "tuple":
             result = tuple([unflatten_dict_h5(v) for v in data.values()])
         else:
             result = {k: unflatten_dict_h5(v) for k, v in data.items()}
         return result
     else:
         if data.shape == ():
             try:
-                return data.asstr()[()]
+                d = data.asstr()[()]
             except TypeError:
-                return data[()]
+                d = data[()]
         else:
-            return data
+            d = data
+        if d == "__NONE__":
+            d = None
+        return d
```

### Comparing `saenopy-0.9.0/saenopy/stack.py` & `saenopy-1.0.0/saenopy/stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,142 @@
-import glob as glob
 import re
 from pathlib import Path
 
-import imageio
 import natsort
 import numpy as np
 import pandas as pd
+
 import tifffile
-from skimage import io
+import imageio
 
 from saenopy.saveable import Saveable
 
 
 class Stack(Saveable):
-    __save_parameters__ = ['template', 'image_filenames', 'filename', 'voxel_size', 'shape', 'channels', 'crop', 'packed_files']
-    template: str = None
-    image_filenames: list = None
+    __save_parameters__ = ['template', 'voxel_size', 'crop', '_shape',
+                           'image_filenames', 'channels', # 'leica_file',
+                           'packed_files']
+    parent = None
 
-    packed_files: list = None
+    template: str = None
+    voxel_size: tuple = None
+    crop: dict = None
 
-    images: list = None
-    input: str = ""
     _shape = None
-    voxel_size: tuple = None
-    channels: list = None
-    images_channels: list = None
 
+    image_filenames: list = None
     leica_file = None
+    channels: list = None
 
-    def __init__(self, template=None, voxel_size=None, filename=None, shape=None, channels=None, image_filenames=None, crop=None, **kwargs):
-        print("stack",template)
-        if template is None:
-            if isinstance(filename, list):
-                template = filenames_to_channel_template(filename)
-            else:
-                template = filename
-        if template is not None:
-            template = template.replace("*", "{z}")
-        self.template = template
-        self.crop = crop
-        if image_filenames is None and template is not None:
+    packed_files: list = None
+
+    def __init__(self, template: str, voxel_size: tuple, crop: dict = None, **kwargs):
+        # reconstruct the stack savable
+        super().__init__(template=template, voxel_size=voxel_size, crop=crop, **kwargs)
+        # if the stack has not been initialized
+        if self.image_filenames is None:
+            # check if the template is a leica file
             match = re.match(r"(.*)\{f\:(\d*)\}\{c\:(\d*)\}(?:\{t\:(\d*)\})?.lif", template)
             if match:
                 from saenopy.gui.common.lif_reader import LifFile
                 self.leica_filename, self.leica_folder, self.leica_channel, self.leica_time = match.groups()
-                if self.leica_time is None:
+                if self.leica_time is None:  # pragma: no cover
                     self.leica_time = 0
                 else:
                     self.leica_time = int(self.leica_time)
                 self.leica_channel = int(self.leica_channel)
                 self.leica_file = LifFile(self.leica_filename + ".lif").get_image(self.leica_folder)
                 self.channels = [str(self.leica_channel)]
                 for i in range(0, self.leica_file.channels):
                     if i != self.leica_channel:
                         self.channels.append(str(i))
+            # or a tiff file
             else:
                 self.image_filenames, self.channels = template_to_array(template, crop)
+
+    def paths_relative(self, parent):
+        self.parent = parent
+
+        def normalize_path(template, output):
+            template = str(Path(template).absolute())
+            output = str(Path(output).absolute())
+            # relative and optionally go up to two folders up
+            try:
+                template = Path(template).relative_to(output)
+            except ValueError:
+                try:
+                    template = Path("..") / Path(template).relative_to(Path(output).parent)
+                except ValueError:
+                    try:
+                        template = Path("../..") / Path(template).relative_to(Path(output).parent.parent)
+                    except ValueError:
+                        pass
+            return str(template)
+
+        def process(image):
+            if isinstance(image, list):
+                return [process(i) for i in image]
+            return normalize_path(image, Path(self.parent.output).parent)
+
+        self.template = process(self.template)
+        #self.parent.template = process(self.parent.template)
+        print("template", self.template)
+        if self.image_filenames is not None:
+            self.image_filenames = process(self.image_filenames)
         else:
-            self.image_filenames = image_filenames
-            self.channels = channels
-        if shape is not None:
-            self._shape = shape
-        if 0:
-            self.channels = channels
-            if channels is not None:
-                self.filename = filename
-                self.images = natsort.natsorted(glob.glob(filename[0]))
-                self.images_channels = []
-                for filename_pattern in filename[1:]:
-                    self.images_channels.append(natsort.natsorted(glob.glob(filename_pattern)))
-            elif isinstance(filename, str):
-                self.filename = str(filename)
-                self.images = natsort.natsorted(glob.glob(filename))
-            else:
-                self.filename = list(filename)
-                self.images = list(filename)
-        self.voxel_size = voxel_size
-        super().__init__(**kwargs)
+            self.leica_filename = process(self.leica_filename)
+        print(self.image_filenames)
+
+    def paths_absolute(self):
+        def normalize_path(template, output):
+            if not Path(template).is_absolute():
+                return str(Path(output).absolute() / template)
+            return str(Path(template).absolute())
+
+        def process(image):
+            if isinstance(image, list):
+                return [process(i) for i in image]
+            return normalize_path(image, Path(self.parent.output).parent)
+
+        self.template = process(self.template)
+        if self.image_filenames is not None:
+            self.image_filenames = process(self.image_filenames)
+        else:
+            self.leica_filename = process(self.leica_filename)
 
     def pack_files(self):
         images = np.array(self.image_filenames)[:, :]
-        images = np.asarray(load_image_files_to_nparray(images, self.crop)).T
+        images = np.asarray(load_image_files_to_nparray(images, self.crop, self.parent)).T
 
         self.packed_files = images
 
     def description(self, z):
         try:
             return f"shape {self.shape}px\nsize {np.array(self.shape[:3])*np.array(self.voxel_size)}μm\nvoxel size {self.voxel_size}μm\n{self.image_filenames[z][0]}"
         except (IndexError, TypeError):
             return ""
 
     @property
     def shape(self) -> tuple:
         if self.leica_file is not None:
             return (self.leica_file.dims.y, self.leica_file.dims.x, self.leica_file.dims.z, 1)
         if self._shape is None:
-            im = readTiff(self.image_filenames[0][0])
+            filename = self.image_filenames[0][0]
+            if not Path(filename).is_absolute() and self.parent is not None:
+                filename = Path(self.parent.output).parent / filename
+            im = read_tiff(filename)
             if self.crop is not None and "x" in self.crop:
                 im = im[:, slice(*self.crop["x"])]
             if self.crop is not None and "y" in self.crop:
                 im = im[slice(*self.crop["y"])]
             self._shape = tuple(list(im.shape[:2]) + list(np.array(self.image_filenames).shape))
         return self._shape
 
     def get_image(self, z, channel):
-        return io.imread(self.image_filenames[z][channel])
+        return self[:, :, :, z, channel].squeeze()
 
     def __getitem__(self, index) -> np.ndarray:
         """ axes are y, x, rgb, z, c """
         if self.leica_file is not None:
             if isinstance(index[3], slice):
                 z_min = 0
                 if index[3].start is not None:
@@ -120,72 +148,28 @@
                 z_min = index[3]
                 z_max = z_min + 1
             images = []
             for z in range(z_min, z_max):
                 im = np.asarray(self.leica_file.get_frame(z, t=self.leica_time, c=int(self.channels[index[4]])))
                 images.append(im)
             images = np.asarray(images)
-            #np.asarray([self.leica_file.get_frame(z) for z in range(z_min, z_max)])
             images = images.transpose(1, 2, 0)[:, :, None, :]
             if isinstance(index[3], int):
                 images = images[:, :, :, 0]
             return images[index[0], index[1], index[2]]
         if self.packed_files is None:
             images = np.array(self.image_filenames)[index[3], index[4]]
-            images = np.asarray(load_image_files_to_nparray(images, self.crop)).T
+            images = np.asarray(load_image_files_to_nparray(images, self.crop, self.parent)).T
         else:
             images = self.packed_files[:, :, :, index[4], index[3]]
         images = np.swapaxes(images, 0, 2)
         return images[index[0], index[1], index[2]]
 
-        images = self.images
-        channel = 0
-        if len(index) == 4 and index[3] > 0 and self.images_channels is not None:
-            images = self.images_channels[index[3]-1]
-            channel = index[3]
-        if isinstance(index[2], slice):
-            return np.array([self.__getitem__(tuple([index[0], index[1], i, channel])) for i in range(index[2].start, index[2].stop, index[2].step if index[2].step is not None else 1)]).transpose(1, 2, 0)
-        try:
-            im = io.imread(images[index[2]])
-        except (IndexError, IOError) as err:
-            print("ERROR", err)
-            im = np.zeros(self.shape[:2])
-        if len(im.shape) == 3:
-            im = im[:, :, 0]
-        return im[index[0], index[1]]
-
     def __array__(self) -> np.ndarray:
         return self[:, :, :, :, 0]
-        return getStack(self.images)
-
-
-def filenames_to_channel_template(filenames):
-    for i in range(len(filenames[0])):
-        for file in filenames[1:]:
-            if file[:i] != filenames[0][:i]:
-                break
-        else:
-            continue
-        i -= 1
-        while filenames[0][i].isdigits():
-            i -= 1
-        i += 1
-        break
-    for j in range(len(filenames[0]) - 1, 0, -1):
-        for file in filenames[1:]:
-            if file[j:] != filenames[0][j:]:
-                break
-        else:
-            continue
-        j += 1
-        while filenames[0][j].isdigits():
-            j += 1
-        break
-    template = filenames[0][:i] + "{c:" + filenames[0][i:j] + "}" + filenames[0][j:]
-    return template
 
 
 def template_to_array(filename, crop):
     from saenopy.result_file import get_channel_placeholder
     filename, channel1 = get_channel_placeholder(filename)
     results1, output_base = format_glob(filename)
     for (template, d1) in results1.groupby("template"):
@@ -207,56 +191,47 @@
             image_filenames = []
             for z in z_indices:
                 image_filenames.append([template.format(z=z)])
             c_indices = [""]
     return image_filenames, c_indices
 
 
-def load_image_files_to_nparray(image_filenames, crop=None):
+def load_image_files_to_nparray(image_filenames, crop=None, parent=None):
     if isinstance(image_filenames, str):
-        im = readTiff(image_filenames)
+        # make relative paths relative to the .saenopy file
+        if not Path(image_filenames).is_absolute() and parent is not None:
+            image_filenames = str(Path(parent.output).absolute().parent / image_filenames)
+        im = read_tiff(image_filenames)
         if len(im.shape) == 2:
             im = im[:, :, None]
         if crop is not None and "x" in crop:
             im = im[:, slice(*crop["x"])]
         if crop is not None and "y" in crop:
             im = im[slice(*crop["y"])]
         return im
     else:
-        return [load_image_files_to_nparray(i, crop) for i in image_filenames]
+        return [load_image_files_to_nparray(i, crop, parent) for i in image_filenames]
 
 
-def readTiff(image_filenames):
+def read_tiff(image_filenames):
     if re.match(r".*\.tiff?(\[.*\])?$", str(image_filenames)):
         image_filenames = str(image_filenames)
         page = 0
         if image_filenames.endswith("]"):
             image_filenames, page = re.match(r"(.*)\[(\d*)\]", image_filenames).groups()
             page = int(page)
-        tif = tifffile.TiffReader(image_filenames)
-        page = tif.pages[page]
-        if isinstance(page, list):
+        with tifffile.TiffReader(image_filenames) as tif:
+            page = tif.pages[page]
+        if isinstance(page, list):  # pragma: no cover
             page = page[0]
         return page.asarray()
-    im = imageio.imread(image_filenames)
+    im = imageio.v2.imread(image_filenames)
     return im
 
 
-def getStack(filename):
-    if isinstance(filename, str):
-        images = glob.glob(filename)
-    else:
-        images = list(filename)
-    im = io.imread(images[0], as_gray=True)
-    stack = np.zeros((im.shape[0], im.shape[1], len(images)), dtype=im.dtype)
-    for i, im in enumerate(images):
-        stack[:, :, i] = io.imread(im, as_gray=True)
-    return stack
-
-
 def format_glob(pattern):
     pattern = str(Path(pattern))
 
     match = re.match(r"(.*\.tif)\[(.*)\]", pattern)
     page = 0
     if match:
         pattern, page = match.groups()
@@ -290,17 +265,17 @@
         template_name = re.sub(regexp_string3, replacement, file.replace("{", "{{").replace("}", "}}"))
         group["filename"] = file
         group["template"] = template_name
         try:
             page = int(page)
             if page != 0:
                 group["filename"] = file+f"[{page}]"
-                group["template"] = template_name + "[" + page + "]"
+                group["template"] = template_name + "[" + str(page) + "]"
             file_list.append(group)
         except ValueError:
-            tif = tifffile.TiffReader(file)
-            group["template"] = template_name + "[" + page + "]"
-            for i in range(len(tif.pages)):
-                group["filename"] = file+f"[{i}]"
-                group[page] = i
-                file_list.append(group.copy())
+            with tifffile.TiffReader(file) as tif:
+                group["template"] = template_name + "[" + str(page) + "]"
+                for i in range(len(tif.pages)):
+                    group["filename"] = file+f"[{i}]"
+                    group[page] = i
+                    file_list.append(group.copy())
     return pd.DataFrame(file_list), output_base
```

