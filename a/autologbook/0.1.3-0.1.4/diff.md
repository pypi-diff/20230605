# Comparing `tmp/autologbook-0.1.3.tar.gz` & `tmp/autologbook-0.1.4.tar.gz`

## Comparing `autologbook-0.1.3.tar` & `autologbook-0.1.4.tar`

### file list

```diff
@@ -1,251 +1,252 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 autologbook-0.1.3/.flake8
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 autologbook-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 autologbook-0.1.3/pyqt5ac-config.yml
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 autologbook-0.1.3/requirements-dev.txt
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 autologbook-0.1.3/requirements.txt
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/__init__.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/__main__.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/about_dialog_ui.py
--rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/attachment.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/autocli.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/autoconfig.py
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/autoerror.py
--rw-r--r--   0        0        0    83315 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/autogui.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/autologbook_app.py
--rw-r--r--   0        0        0    45077 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/autoprotocol.py
--rw-r--r--   0        0        0    61067 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/autotools.py
--rw-r--r--   0        0        0    84523 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/autowatchdog.py
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/change_sample_dialog_ui.py
--rw-r--r--   0        0        0    60429 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/configuration_editor_ui.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/containers.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/context_menu.py
--rw-r--r--   0        0        0    24576 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/dialog_windows.py
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/edit_lock_dialog_ui.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/elog_interface.py
--rw-r--r--   0        0        0    29184 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/elog_post_splitter.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/file_system_command.py
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/file_type_guesser.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/html_helpers.py
--rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/jinja_integration.py
--rw-r--r--   0        0        0    33823 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/main_window_ui.py
--rw-r--r--   0        0        0    79538 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/microscope_picture.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/model_test_ui.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/navigation_image.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/object_factoy.py
--rw-r--r--   0        0        0    17942 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/optical_image.py
--rw-r--r--   0        0        0   157375 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/protocol_editor.py
--rw-r--r--   0        0        0    22485 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/protocol_editor_models.py
--rw-r--r--   0        0        0    27651 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/protocol_editor_ui.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/qt_signal_dispatcher.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/rename_dialog_ui.py
--rw-r--r--   0        0        0   464489 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/resource_rc.py
--rw-r--r--   0        0        0    39102 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/resource_rc.rcc
--rw-r--r--   0        0        0    14444 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/restore_element.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/restore_element_dialog_ui.py
--rw-r--r--   0        0        0    16776 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/sample.py
--rw-r--r--   0        0        0    14839 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/thread_worker.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/user_editor_ui.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/video.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/conf/type_guesser_regexp.yaml
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/attachment_base_template.yammy
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/digital_camera_optical_image_gps_template.yammy
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/digital_camera_optical_image_template.yammy
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/empty_page_template.yammy
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/fei_microscope_picture_template.yammy
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/general_attachment_base_template.yammy
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/general_optical_images_base_template.yammy
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/keyence_optical_image_template.yammy
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/macros.yammy
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/microscope_list_post_base_template.yammy
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/microscope_list_post_url_only_template.yammy
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/microscope_picture_base_template.yammy
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/multi_microscope_protocol_template.yammy
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/navigation_base_template.yammy
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/navigation_image_template.yammy
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/optical_image_base_template.yammy
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/protocol_base_template.yammy
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/quattro_protocol_template.yammy
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/sample_attachment_base_template.yammy
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/sample_base_template.yammy
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/sample_list_base_template.yammy
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/sample_microscope_picture_base_template.yammy
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/sample_optical_image_base_template.yammy
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/sample_video_base_template.yammy
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/scripts.yammy
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/title_base_template.yammy
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/vega_microscope_picture_base_template.yammy
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/vega_microscope_picture_jpeg_full_template.yammy
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/vega_microscope_picture_jpeg_simple_template.yammy
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/vega_microscope_picture_jpeg_template.yammy
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/video_base_template.yammy
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/xl40_microscope_picture_base_template.yammy
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/xl40_microscope_picture_multi_template.yammy
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/templates/xl40_microscope_picture_single_template.yammy
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/about_dialog.ui
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/change_sample_dialog.ui
--rw-r--r--   0        0        0    58393 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/configuration_editor.ui
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/edit_lock_dialog.ui
--rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/main_window.ui
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/model_test.ui
--rw-r--r--   0        0        0    36028 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/protocol_editor.ui
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/rename_dialog.ui
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resource.qrc
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/restore_element_dialog.ui
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/user_editor.ui
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-attach-48.png
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-bold-48.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-bulleted-list-48.png
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-cancel-32.png
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-cancel-48.png
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-choose-font-48.png
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-close-30.png
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-code-48.png
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-collapse-arrow-48.png
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-compact-camera-32.png
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-compact-camera-64.png
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-copy-48.png
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-copy-all-48.png
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-copy-caption-48.png
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-copy-description-48.png
--rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-copy-extra-48.png
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-copy-link-48.png
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-copy-pair-48.png
--rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-copy-single-48.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-design-48.png
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-edit-30.png
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-edit-user-30.png
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-expand-arrow-48.png
--rw-r--r--   0        0        0    29688 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-expand-arrow.gif
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-expand-arrows-48.png
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-folder-48.png
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-fullscreen-48.png
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-green-circle-48.png
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-high-importance-30.png
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-home-48.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-hyperlink-48.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-ice-48.png
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-image-48.png
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-internet-folder-30.png
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-italic-48.png
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-link-folder-48.png
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-logbook-64.png
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-map-marker-48.png
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-markdown-48.png
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-move-up-row-48.png
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-numbered-list-48.png
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-ok-30.png
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-open-envelope-30.png
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-opened-folder-30.png
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-opened-folder-48.png
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-optical-microscope-64.png
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-paste-all-48.png
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-paste-caption-48.png
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-paste-description-48.png
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-paste-extra-48.png
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-paste-special-48.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-pause-48.png
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-pencil-48.png
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-picture-48.png
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-pictures-folder-30.png
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-pictures-folder-48.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-play-48.png
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-recycle-48.png
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-red-circle-48.png
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-rename-48.png
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-save-30.png
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-save-as-48.png
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-search-48.png
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-section-48.png
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-select-all-48.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-sniper-48.png
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-start-30.png
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-start-48.png
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-stop-sign-30.png
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-stop-sign-48.png
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-strikethrough-48.png
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-subscript-48.png
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-superscript-48.png
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-support-48.png
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-sync-48.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-text-48.png
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-tools-48.png
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-trash-can-48.png
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-trash-restore-48.png
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-underline-48.png
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-update-left-rotation-48.png
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-upload-to-cloud-48.png
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-user-secured-48.png
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-video-clip-48.png
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 autologbook-0.1.3/autologbook/ui/resources/icons8-website-48.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/__init__.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/constants.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/dialog_compare_experiment_file.py
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/dialog_compare_experiment_file_ui.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/dialog_select_experiment_file.py
--rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/dialog_select_experiment_file_ui.py
--rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/experiment_wizard.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/experiment_wizard_app.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ini_syntax_highlighter.py
--rw-r--r--   0        0        0   153977 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/resources_rc.py
--rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/search_results_model.py
--rw-r--r--   0        0        0    10242 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_commit_new_experiment_page.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_commit_new_experiment_page_ui.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_conclusion_page.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_conclusion_page_ui.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_introduction_page.py
--rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_introduction_page_ui.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_new_experiment_page.py
--rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_new_experiment_page_ui.py
--rw-r--r--   0        0        0    14027 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_review_configuration_page.py
--rw-r--r--   0        0        0    29347 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_review_configuration_page_ui.py
--rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_search_experiment_page.py
--rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/wizard_search_experiment_page_ui.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/conf/unit_list.yaml
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/dialog_compare_experiment_file.ui
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/dialog_select_experiment_file.ui
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/wizard_commit_new_experiment_page.ui
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/wizard_conclusion_page.ui
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/wizard_introduction_page.ui
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/wizard_new_experiment_page.ui
--rw-r--r--   0        0        0    31336 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/wizard_review_configuration_page.ui
--rw-r--r--   0        0        0    11031 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/wizard_search_experiment_page.ui
--rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/ec-logo.jpg
--rw-r--r--   0        0        0    20260 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/glossy-microscope.png
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/icons8-done-48.png
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/icons8-error-48.png
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/icons8-fantasy-48.png
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/icons8-folder-48.png
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/icons8-new-48.png
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/icons8-new-96.png
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/icons8-question-mark-48.png
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/icons8-website-48.png
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 autologbook-0.1.3/expwizard/ui/resources/resources.qrc
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/__init__.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/about_image_converter_ui.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/event_logger.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/fei_image_manipulator.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/image_converter.py
--rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/image_converter_gui.py
--rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/main_window_image_converter_ui.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/metadata_dumper.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/mirror_maker.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/qt_exception_handler.py
--rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/resource_rc.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/util.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/ui/about_image_converter.ui
--rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/ui/main_window_image_converter.ui
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/ui/resource.qrc
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 autologbook-0.1.3/labtools/ui/resources/icons8-picture-64.png
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 autologbook-0.1.3/test/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 autologbook-0.1.3/test/test_autotools.py
--rw-r--r--   0        0        0    28142 2020-02-02 00:00:00.000000 autologbook-0.1.3/test/test_element_type_guesser.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 autologbook-0.1.3/test/test_enums.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 autologbook-0.1.3/test/test_file_utils.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 autologbook-0.1.3/test/test_picture_resolution.py
--rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 autologbook-0.1.3/test/test_protocol_elements.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 autologbook-0.1.3/test/test_url_guessing.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 autologbook-0.1.3/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autologbook-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0    19134 2020-02-02 00:00:00.000000 autologbook-0.1.3/README.md
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 autologbook-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    21337 2020-02-02 00:00:00.000000 autologbook-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 autologbook-0.1.4/.flake8
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 autologbook-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 autologbook-0.1.4/pyqt5ac-config.yml
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 autologbook-0.1.4/requirements-dev.txt
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 autologbook-0.1.4/requirements.txt
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/__init__.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/__main__.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/about_dialog_ui.py
+-rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/attachment.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autocli.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autoconfig.py
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autoerror.py
+-rw-r--r--   0        0        0    83315 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autogui.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autologbook_app.py
+-rw-r--r--   0        0        0    45270 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autoprotocol.py
+-rw-r--r--   0        0        0    61480 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autotools.py
+-rw-r--r--   0        0        0    84283 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/autowatchdog.py
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/change_sample_dialog_ui.py
+-rw-r--r--   0        0        0    60429 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/configuration_editor_ui.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/containers.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/context_menu.py
+-rw-r--r--   0        0        0    24576 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/dialog_windows.py
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/edit_lock_dialog_ui.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/elog_interface.py
+-rw-r--r--   0        0        0    29594 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/elog_post_splitter.py
+-rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/file_system_command.py
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/file_type_guesser.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/html_helpers.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/jinja_integration.py
+-rw-r--r--   0        0        0    33823 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/main_window_ui.py
+-rw-r--r--   0        0        0    80159 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/microscope_picture.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/model_test_ui.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/navigation_image.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/object_factoy.py
+-rw-r--r--   0        0        0    17906 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/optical_image.py
+-rw-r--r--   0        0        0   157866 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/protocol_editor.py
+-rw-r--r--   0        0        0    22485 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/protocol_editor_models.py
+-rw-r--r--   0        0        0    27651 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/protocol_editor_ui.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/qt_signal_dispatcher.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/rename_dialog_ui.py
+-rw-r--r--   0        0        0   464489 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/resource_rc.py
+-rw-r--r--   0        0        0    39102 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/resource_rc.rcc
+-rw-r--r--   0        0        0    14444 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/restore_element.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/restore_element_dialog_ui.py
+-rw-r--r--   0        0        0    16776 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/sample.py
+-rw-r--r--   0        0        0    14839 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/thread_worker.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/user_editor_ui.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/video.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/conf/type_guesser_regexp.yaml
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/attachment_base_template.yammy
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/digital_camera_optical_image_gps_template.yammy
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/digital_camera_optical_image_template.yammy
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/empty_page_template.yammy
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/fei_microscope_picture_template.yammy
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/footer_base_template.yammy
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/general_attachment_base_template.yammy
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/general_optical_images_base_template.yammy
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/keyence_optical_image_template.yammy
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/macros.yammy
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/microscope_list_post_base_template.yammy
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/microscope_list_post_url_only_template.yammy
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/microscope_picture_base_template.yammy
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/multi_microscope_protocol_template.yammy
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/navigation_base_template.yammy
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/navigation_image_template.yammy
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/optical_image_base_template.yammy
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/protocol_base_template.yammy
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/quattro_protocol_template.yammy
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_attachment_base_template.yammy
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_base_template.yammy
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_list_base_template.yammy
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_microscope_picture_base_template.yammy
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_optical_image_base_template.yammy
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/sample_video_base_template.yammy
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/scripts.yammy
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/title_base_template.yammy
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/vega_microscope_picture_base_template.yammy
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/vega_microscope_picture_jpeg_full_template.yammy
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/vega_microscope_picture_jpeg_simple_template.yammy
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/vega_microscope_picture_jpeg_template.yammy
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/video_base_template.yammy
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/xl40_microscope_picture_base_template.yammy
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/xl40_microscope_picture_multi_template.yammy
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/templates/xl40_microscope_picture_single_template.yammy
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/about_dialog.ui
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/change_sample_dialog.ui
+-rw-r--r--   0        0        0    58393 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/configuration_editor.ui
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/edit_lock_dialog.ui
+-rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/main_window.ui
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/model_test.ui
+-rw-r--r--   0        0        0    36028 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/protocol_editor.ui
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/rename_dialog.ui
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resource.qrc
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/restore_element_dialog.ui
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/user_editor.ui
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-attach-48.png
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-bold-48.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-bulleted-list-48.png
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-cancel-32.png
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-cancel-48.png
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-choose-font-48.png
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-close-30.png
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-code-48.png
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-collapse-arrow-48.png
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-compact-camera-32.png
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-compact-camera-64.png
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-48.png
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-all-48.png
+-rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-caption-48.png
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-description-48.png
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-extra-48.png
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-link-48.png
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-pair-48.png
+-rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-copy-single-48.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-design-48.png
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-edit-30.png
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-edit-user-30.png
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-expand-arrow-48.png
+-rw-r--r--   0        0        0    29688 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-expand-arrow.gif
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-expand-arrows-48.png
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-folder-48.png
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-fullscreen-48.png
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-green-circle-48.png
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-high-importance-30.png
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-home-48.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-hyperlink-48.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-ice-48.png
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-image-48.png
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-internet-folder-30.png
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-italic-48.png
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-link-folder-48.png
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-logbook-64.png
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-map-marker-48.png
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-markdown-48.png
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-move-up-row-48.png
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-numbered-list-48.png
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-ok-30.png
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-open-envelope-30.png
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-opened-folder-30.png
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-opened-folder-48.png
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-optical-microscope-64.png
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-paste-all-48.png
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-paste-caption-48.png
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-paste-description-48.png
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-paste-extra-48.png
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-paste-special-48.png
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-pause-48.png
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-pencil-48.png
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-picture-48.png
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-pictures-folder-30.png
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-pictures-folder-48.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-play-48.png
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-recycle-48.png
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-red-circle-48.png
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-rename-48.png
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-save-30.png
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-save-as-48.png
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-search-48.png
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-section-48.png
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-select-all-48.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-sniper-48.png
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-start-30.png
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-start-48.png
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-stop-sign-30.png
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-stop-sign-48.png
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-strikethrough-48.png
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-subscript-48.png
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-superscript-48.png
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-support-48.png
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-sync-48.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-text-48.png
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-tools-48.png
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-trash-can-48.png
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-trash-restore-48.png
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-underline-48.png
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-update-left-rotation-48.png
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-upload-to-cloud-48.png
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-user-secured-48.png
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-video-clip-48.png
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 autologbook-0.1.4/autologbook/ui/resources/icons8-website-48.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/__init__.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/constants.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/dialog_compare_experiment_file.py
+-rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/dialog_compare_experiment_file_ui.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/dialog_select_experiment_file.py
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/dialog_select_experiment_file_ui.py
+-rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/experiment_wizard.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/experiment_wizard_app.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ini_syntax_highlighter.py
+-rw-r--r--   0        0        0   153977 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/resources_rc.py
+-rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/search_results_model.py
+-rw-r--r--   0        0        0    10242 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_commit_new_experiment_page.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_commit_new_experiment_page_ui.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_conclusion_page.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_conclusion_page_ui.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_introduction_page.py
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_introduction_page_ui.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_new_experiment_page.py
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_new_experiment_page_ui.py
+-rw-r--r--   0        0        0    14027 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_review_configuration_page.py
+-rw-r--r--   0        0        0    29347 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_review_configuration_page_ui.py
+-rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_search_experiment_page.py
+-rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/wizard_search_experiment_page_ui.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/conf/unit_list.yaml
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/dialog_compare_experiment_file.ui
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/dialog_select_experiment_file.ui
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_commit_new_experiment_page.ui
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_conclusion_page.ui
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_introduction_page.ui
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_new_experiment_page.ui
+-rw-r--r--   0        0        0    31336 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_review_configuration_page.ui
+-rw-r--r--   0        0        0    11031 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/wizard_search_experiment_page.ui
+-rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/ec-logo.jpg
+-rw-r--r--   0        0        0    20260 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/glossy-microscope.png
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-done-48.png
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-error-48.png
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-fantasy-48.png
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-folder-48.png
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-new-48.png
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-new-96.png
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-question-mark-48.png
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/icons8-website-48.png
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 autologbook-0.1.4/expwizard/ui/resources/resources.qrc
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/__init__.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/about_image_converter_ui.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/event_logger.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/fei_image_manipulator.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/image_converter.py
+-rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/image_converter_gui.py
+-rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/main_window_image_converter_ui.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/metadata_dumper.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/mirror_maker.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/qt_exception_handler.py
+-rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/resource_rc.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/util.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/ui/about_image_converter.ui
+-rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/ui/main_window_image_converter.ui
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/ui/resource.qrc
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 autologbook-0.1.4/labtools/ui/resources/icons8-picture-64.png
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_autotools.py
+-rw-r--r--   0        0        0    28142 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_element_type_guesser.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_enums.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_file_utils.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_picture_resolution.py
+-rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_protocol_elements.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 autologbook-0.1.4/test/test_url_guessing.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 autologbook-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autologbook-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0    19134 2020-02-02 00:00:00.000000 autologbook-0.1.4/README.md
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 autologbook-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    21337 2020-02-02 00:00:00.000000 autologbook-0.1.4/PKG-INFO
```

### Comparing `autologbook-0.1.3/.pre-commit-config.yaml` & `autologbook-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/requirements-dev.txt` & `autologbook-0.1.4/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/__init__.py` & `autologbook-0.1.4/autologbook/__init__.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/__main__.py` & `autologbook-0.1.4/autologbook/__main__.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/about_dialog_ui.py` & `autologbook-0.1.4/autologbook/about_dialog_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.retranslateUi(About)
         QtCore.QMetaObject.connectSlotsByName(About)
 
     def retranslateUi(self, About):
         _translate = QtCore.QCoreApplication.translate
         About.setWindowTitle(_translate("About", "About Autologbook"))
         self.label.setText(_translate("About", "<html><head/><body><p align=\"center\"><img src=\":/resources/icons8-logbook-64.png\"/></p><p\n"
-"       align=\"center\"><br/></p><p align=\"center\">AUTOLOGBOOK v0.1.3</p><p\n"
+"       align=\"center\"><br/></p><p align=\"center\">AUTOLOGBOOK v0.1.4</p><p\n"
 "       align=\"center\">A script for automatic logbook generation in microscopy</p><p align=\"center\">GitHub\n"
 "       <a href=\"https://github.com/abulgher/autologbook\"><span style=\" text-decoration:\n"
 "       underline; color:#0000ff;\">Source Code</span></a></p><p align=\"center\">(C)\n"
 "       Antonio Bulgheroni - 2022</p><p align=\"center\"><br/><a href=\"https://icons8.com/icon/pNYOTp5DinZ3/copy\"><span\n"
 "       style=\" text-decoration: underline; color:#0000ff;\">Copy</span></a> icon by <a href=\"https://icons8.com\"><span\n"
 "       style=\" text-decoration: underline; color:#0000ff;\">Icons8</span></a></p></body></html>\n"
 "      "))
```

### Comparing `autologbook-0.1.3/autologbook/attachment.py` & `autologbook-0.1.4/autologbook/attachment.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/autocli.py` & `autologbook-0.1.4/autologbook/autocli.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/autoconfig.py` & `autologbook-0.1.4/autologbook/autoconfig.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 #
 # GENERAL
 #
 CUSTOMID_START = 1000
 CUSTOMID_TIFFCODE = 37510
 VEGA_TIFFCODE = 50431
 VEGA_JPEG_ID_CODE = piexif.ExifIFD.UserComment
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 THREAD_STATUS_UPDATE = 1000  # in ms
+AUTO_SAVE_INTERVAL = 300000  # in ms
 MAX_ATTACHMENTS = 50  # it is a limitation of elog
 ELOG_PAGE_SIZE_LIMIT = 240000  # the real max is 250000, I kept a 10k as a safety margin.
 #
 # ELOG PARAMETERS
 #
 ELOG_USER = 'log-robot'
 ELOG_PASSWORD = 'mTZtK2iFHhwqixkhJV0JkplSqMMu9ykWOhcNY/1WyL7'
@@ -66,15 +67,15 @@
 #
 # WATCHDOGS
 #
 AUTOLOGBOOK_WATCHDOG_MAX_ATTEMPTS = 5
 AUTOLOGBOOK_WATCHDOG_WAIT_MIN = 1
 AUTOLOGBOOK_WATCHDOG_WAIT_MAX = 5
 AUTOLOGBOOK_WATCHDOG_WAIT_INCREMENT = 1
-AUTOLOGBOOK_WATCHDOG_MIN_DELAY = 45
+AUTOLOGBOOK_WATCHDOG_MIN_DELAY = 600  # it is used to be 45, increased to 600 to avoid useless server overload.
 AUTOLOGBOOK_WATCHDOG_TIMEOUT = 0.5
 #
 # MIRRORING WATCHDOG
 #
 AUTOLOGBOOK_MIRRORING_MAX_ATTEMPTS = 2
 AUTOLOGBOOK_MIRRORING_WAIT = 0.5
 AUTOLOGBOOK_MIRRORING_TIMEOUT = 0.2
```

### Comparing `autologbook-0.1.3/autologbook/autoerror.py` & `autologbook-0.1.4/autologbook/autoerror.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/autogui.py` & `autologbook-0.1.4/autologbook/autogui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/autologbook_app.py` & `autologbook-0.1.4/autologbook/autologbook_app.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/autoprotocol.py` & `autologbook-0.1.4/autologbook/autoprotocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,14 +194,15 @@
         # initialize yaml_dict and its filename
         self.yamlDict = None
         self.yamlFilename = None
 
         # jinja2
         self.protocol_type = 'Generic'
         self.template = 'protocol_base_template.yammy'
+        self.last_update = f'{datetime.now():%Y-%m-%d %H:%M:%S}'
 
         # reset the picture ID list
         MicroscopePicture._reset_ids()
 
     def __str__(self) -> str:
         """Return basic string representation of a Protocol."""
         msg = (f'Protocol #{self.protocol} - {self.project} - {self.responsible}\n')
@@ -460,14 +461,15 @@
             log.debug('At the moment there are %s samples in the list' % len(self.samples))
         else:
             log.warning('Attempt to remove %s from the sample list, but it was not there' % sample_full_name)
 
     def render_html(self):
         log.info('Rendering HTML code for protocol %s' % self.protocol)
         jinja_template = jinja_env.get_template(self.template)
+        self.last_update = f'{datetime.now():%Y-%m-%d %H:%M:%S}'
         html_output = jinja_template.render(protocol=self)
         return html_output
 
     def recursive_append(self, sample_list: ResettableList):
         for sample in sample_list:
             self.ordered_sample_list.append(sample)
             self.recursive_append(self.samples[sample].subsamples)
@@ -830,33 +832,33 @@
                 log.exception('Logbook error', e)
             except elog.LogbookMessageRejected as e:
                 # this exception used to be thrown in case of a too large message. Now it should not happen anymore,
                 # but it is wise to catch it here and inform the user.
                 log.critical('ELOG Message was rejected!')
         else:
             # ok split the post
-            log.info('Splitting original post in subpages.')
+            log.info('Splitting original post in subpages')
             elog_post_splitter = ELOGPostSplitter(html_content)
             if elog_post_splitter.num_of_pages == len(protocol_ids):
                 # we have just enough post
                 pass
             elif elog_post_splitter.num_of_pages > len(protocol_ids):
                 # we have more pages than already existing posts.
                 # we need to create more
                 while len(protocol_ids) < elog_post_splitter.num_of_pages:
                     try:
                         protocol_ids.append(
-                            elog_handle.post(jinja_env.get_template(empty_page_template).render(self),
+                            elog_handle.post(jinja_env.get_template(empty_page_template).render(protocol=self),
                                              reply=True, msg_id=protocol_ids[0],
                                              attributes=self.attributes, encoding='HTML',
                                              timeout=autoconfig.ELOG_TIMEOUT))
                     except elog.LogbookAuthenticationError as e:
                         log.exception('Logbook error', e)
 
-            else:  # elog_post_splitter.num_of_pages < len(real_ids)
+            else:  # elog_post_splitter.num_of_pages < len(protocol_ids)
                 # we have more existing posts than required pages.
                 # the extra posts have been already reset to empty message,
                 # we just need to limit the size of real_ids, and we leave the empty messages
                 protocol_ids = protocol_ids[:elog_post_splitter.num_of_pages]
 
             # rebuild the index of the post splitter
             elog_post_splitter.rebuild_index(base_url=self.elog_base_url, logbook=self.elog_logbook,
@@ -866,39 +868,40 @@
             self.elog_msg_id = []
             for i, page in enumerate(elog_post_splitter.get_all_pages()):
                 attachments = []
                 if page._type in [ELOGPageType.ELOGIntroConclusionType, ELOGPageType.ELOGIntroOpticalConclusionType,
                                   ELOGPageType.ELOGConclusionPageType]:
                     if not skip_attachments:
                         # we attach generic attachments here:
-                        for att in self.attachments:
+                        for att in self.attachments.get_upload_attachments():
                             if os.stat(att).st_size:
                                 attachments.append(att)
                 elif page._type in [ELOGPageType.ELOGSamplePageType, ELOGPageType.ELOGCombinedSamplePageType]:
                     if not skip_attachments:
                         # we attach here sample specific attachments.
                         if page._type == ELOGPageType.ELOGSamplePageType:
                             sample_name_list = [page.sample_name]
                         else:
                             sample_name_list = page.sample_name_list
 
                         for sample_name in sample_name_list:
                             sample = self.samples[sample_name]
-                            for att in sample.attachments:
+                            for att in sample.attachments.get_upload_attachments():
                                 if os.stat(att).st_size:
                                     attachments.append(att)
 
                 try:
                     self.elog_msg_id.append(
                         elog_handle.post(page.get_html(), msg_id=page._message_id, reply=False,
                                          attributes=self.attributes,
                                          attachments=attachments, encoding='HTML',
                                          timeout=autoconfig.ELOG_TIMEOUT))
                     log.info('Successfully posted eLog entry for protocol %s page %s of %s' %
                              (self.protocol, i + 1, elog_post_splitter.num_of_pages))
+
                 except elog.LogbookMessageRejected:
                     log.critical('ELOG Message too large, the attempt of splitting the post failed.')
                     log.critical('Page number %s of type %s is too big. Fix the content manually and try again' %
                                  (page.page_number + 1, page._type))
                     log.critical('Failed to post eLOG entry for protocol %s page %s of %s' %
                                  (self.protocol, i + 1, elog_post_splitter.num_of_pages))
                 except elog.LogbookAuthenticationError as e:
```

### Comparing `autologbook-0.1.3/autologbook/autotools.py` & `autologbook-0.1.4/autologbook/autotools.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,14 +599,25 @@
             f'# YAML FILE Dumped at {datetime.now():%Y-%m-%d %H:%M:%S}\n\n')
 
         yaml_dict = remove_empty_slots(yaml_dict)
         if len(yaml_dict) != 0:
             yaml.dump(yaml_dict, f, allow_unicode=True)
 
 
+def is_yaml_file_dumping_needed(yaml_dict: dict, yaml_file_name:str | Path):
+
+    with open(yaml_file_name, 'r', encoding='utf-8') as file:
+        stored = yaml.safe_load(file)
+    for key in yaml_dict.keys():
+        print(f'{key} current_dict = {yaml_dict[key]}, stored = {stored.get(key, "MISSING")}')
+
+    print(f'The two dictionaries are identical {stored==yaml_dict}')
+
+    return not yaml_dict == stored
+
 def remove_empty_slots(yaml_dict: dict) -> dict:
     empty_keys = list()
     for key, value in yaml_dict.items():
         empty_values = [subvalues == '' for subvalues in value.values()]
         if all(empty_values):
             empty_keys.append(key)
     for key in empty_keys:
```

### Comparing `autologbook-0.1.3/autologbook/autowatchdog.py` & `autologbook-0.1.4/autologbook/autowatchdog.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,20 +504,17 @@
 
     """
 
     def __init__(self, autoprotocol_instance, **kwargs):
 
         self.matching_patterns = regexp_repository.get_all_matching()
 
-        # We have to set the excluded patterns to None, in order not to exclude any files from the event handler.
-        # The reason is that navigation camera images must be excluded from optical images.
-        # So we don't exclude any pattern here, but we don't process excluded files later.
-        # In fact the element type guesser will apply the exclude patterns and eventually return None if any element
-        # could be found.
-        self.excluded_patterns = None
+        # We have to exclude whatever was excluded by the mirroring event handler. This means only the GENERIC
+        # exclude patterns that are temporary files.
+        self.excluded_patterns = regexp_repository.get_exclude('GENERIC')
         # set the protocol instance
         self.autoprotocol_instance = autoprotocol_instance
 
         # set the queue reference
         self.queue = None
 
         # a copy of the previous event. This is to avoid to dispatch and process duplicated events.
@@ -1317,24 +1314,24 @@
     def update_logbook(self, skip_attachments=True):
         """
         Update the logbook entry.
 
         Generate the HTML code of the whole protocol and post it to the
         server.
 
-        The positing will actually take place if the observer queue is 'almost empty' and if the last update was not
+        The posting will actually take place if the observer queue is 'almost empty' and if the last update was not
         too recent.
 
         Almost empty means that the size is below 2. In fact every time a creation event is generated there is at least
         one modified event for the file and also one for the directory coming along.
 
         Parameters
         ----------
         skip_attachments : bool, optional
-            Allows to skip the attachments in order to reduce the network_path trafic.
+            Allows to skip the attachments in order to reduce the network_path traffic.
             The default is True.
 
         """
         c = self.queue.qsize() < 2
         d = datetime.now().timestamp() - self.last_update.timestamp() > autoconfig.AUTOLOGBOOK_WATCHDOG_MIN_DELAY
         if c and d:
```

### Comparing `autologbook-0.1.3/autologbook/change_sample_dialog_ui.py` & `autologbook-0.1.4/autologbook/change_sample_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/configuration_editor_ui.py` & `autologbook-0.1.4/autologbook/configuration_editor_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/containers.py` & `autologbook-0.1.4/autologbook/containers.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/context_menu.py` & `autologbook-0.1.4/autologbook/context_menu.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/dialog_windows.py` & `autologbook-0.1.4/autologbook/dialog_windows.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/edit_lock_dialog_ui.py` & `autologbook-0.1.4/autologbook/edit_lock_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/elog_interface.py` & `autologbook-0.1.4/autologbook/elog_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
         self._connection_verified = status
 
     def get_base_url(self) -> str:
         return self._url.rstrip('/')
 
     def get_msg_ids(self, protocol_id: int | str) -> list[int]:
 
+        log.info('Getting message IDs for this protocol entry')
         msg_ids = self.search({self.protocol_id_key: protocol_id}, timeout=self.timeout)
         real_ids = list()
 
         for msg_id in msg_ids:
             _, attributes, __ = self.read(msg_id, timeout=self.timeout)
 
             if attributes[self.protocol_id_key] == protocol_id:
@@ -135,15 +136,15 @@
         try:
             self.get_last_message_id(timeout=self.timeout)
             self._connection_verified = True
         except elog.LogbookError as e:
             self._connection_verified = False
             raise e
 
-    def refresh(self) -> AdvLogbook :
+    def refresh(self) -> AdvLogbook:
         return elog_handle_factory.get_logbook_handle(self.logbook)
 
 
 
 class AnalysisLogbook(AdvLogbook):
     protocol_id_key = 'Protocol ID'
```

### Comparing `autologbook-0.1.3/autologbook/elog_post_splitter.py` & `autologbook-0.1.4/autologbook/elog_post_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     NavigationDiv = 'navigation_div'
     SampleDescriptionDiv = 'sample_description_div'
     SampleList = 'sample_list'
     GeneralOpticalImage = 'general_optical_image'
     SampleElements = 'sample_elements'
     ConclusionDiv = 'conclusion_div'
     GeneralAttachment = 'general_attachment'
+    Footer = 'footer'
     Script = 'script'
     HTMLNavigation = 'html_navigation'
 
 
 class SoupParser:
     """Mixin class to parse an HTML soup."""
 
@@ -328,14 +329,15 @@
         self._required_element_dict = {
             ELOGPostElement.TitleDiv: {'id': 'protocol_title_div'},
             ELOGPostElement.IntroductionDiv: {'class_': 'section_div', 'id': 'Introduction'},
             ELOGPostElement.NavigationDiv: {'class_': 'navigation_image_div'},
             ELOGPostElement.SampleDescriptionDiv: {'class_': 'section_div', 'id': 'Samples'},
             ELOGPostElement.SampleList: {'id': 'sample_list_div'},
             ELOGPostElement.HTMLNavigation: None,  # placeholder
+            ELOGPostElement.Footer: {'id': 'footer'},
             ELOGPostElement.Script: {'name': 'script'}
         }
         self._page_tags = self.build_page()
 
 
 class ELOGOpticalImagePage(ELOGPage):
 
@@ -343,14 +345,15 @@
                  **kwargs):
         super().__init__(html_soup, page_number, parent_page, *args, **kwargs)
         self._type = ELOGPageType.ELOGOpticalImagePageType
         self._required_element_dict = {
             ELOGPostElement.TitleDiv: {'id': 'protocol_title_div'},
             ELOGPostElement.GeneralOpticalImage: {'id': 'general_optical_image_section'},
             ELOGPostElement.HTMLNavigation: None,  # placeholder
+            ELOGPostElement.Footer: {'id': 'footer'},
             ELOGPostElement.Script: {'name': 'script'}
         }
         self._page_tags = self.build_page()
 
 
 class ELOGSamplePage(ELOGPage):
 
@@ -360,14 +363,15 @@
         super().__init__(html_soup, page_number, parent_page, *args, **kwargs)
         self._type = ELOGPageType.ELOGSamplePageType
         self._sample_full_name = sample_full_name
         self._required_element_dict = {
             ELOGPostElement.TitleDiv: {'id': 'protocol_title_div'},
             ELOGPostElement.SampleElements: {'name': 'div', 'class_': 'sample_div', 'id': self._sample_full_name},
             ELOGPostElement.HTMLNavigation: None,  # placeholder
+            ELOGPostElement.Footer: {'id': 'footer'},
             ELOGPostElement.Script: {'name': 'script'}
         }
         self._page_tags = self.build_page()
 
     @property
     def sample_name(self) -> str:
         return self._sample_full_name
@@ -396,28 +400,30 @@
         for sample in self._sample_full_name_list:
             element_dict[f'{ELOGPostElement.SampleElements}_{sample}'] = {
                 'name': 'div',
                 'class_': 'sample_div',
                 'id': sample
             }
         element_dict[ELOGPostElement.HTMLNavigation] = None  # placeholder
+        element_dict[ELOGPostElement.Footer] = {'id': 'footer'}
         element_dict[ELOGPostElement.Script] = {'name': 'script'}
         return element_dict
 
 
 class ELOGConclusionPage(ELOGPage):
     def __init__(self, html_soup: BeautifulSoup, page_number: int = None, parent_page: ELOGPage = None, *args,
                  **kwargs):
         super().__init__(html_soup, page_number, parent_page, *args, **kwargs)
         self._type = ELOGPageType.ELOGConclusionPageType
         self._required_element_dict = {
             ELOGPostElement.TitleDiv: {'id': 'protocol_title_div'},
             ELOGPostElement.ConclusionDiv: {'class_': 'section_div', 'id': 'Conclusion'},
             ELOGPostElement.GeneralAttachment: {'id': 'general_attachment'},
             ELOGPostElement.HTMLNavigation: None,  # placeholder
+            ELOGPostElement.Footer: {'id': 'footer'},
             ELOGPostElement.Script: {'name': 'script'}
         }
         self._page_tags = self.build_page()
 
 
 class ELOGIntroOpticalConclusionPage(ELOGPage):
     def __init__(self, html_soup: BeautifulSoup, *args, **kwargs):
@@ -429,14 +435,15 @@
             ELOGPostElement.NavigationDiv: {'class_': 'navigation_image_div'},
             ELOGPostElement.SampleDescriptionDiv: {'class_': 'section_div', 'id': 'Samples'},
             ELOGPostElement.SampleList: {'id': 'sample_list_div'},
             ELOGPostElement.GeneralOpticalImage: {'id': 'general_optical_image_section'},
             ELOGPostElement.ConclusionDiv: {'class_': 'section_div', 'id': 'Conclusion'},
             ELOGPostElement.GeneralAttachment: {'id': 'general_attachment'},
             ELOGPostElement.HTMLNavigation: None,  # placeholder
+            ELOGPostElement.Footer: {'id': 'footer'},
             ELOGPostElement.Script: {'name': 'script'}
         }
         self._page_tags = self.build_page()
 
 
 class ELOGIntroConclusionPage(ELOGPage):
     def __init__(self, html_soup: BeautifulSoup, *args, **kwargs):
@@ -447,14 +454,15 @@
             ELOGPostElement.IntroductionDiv: {'class_': 'section_div', 'id': 'Introduction'},
             ELOGPostElement.NavigationDiv: {'class_': 'navigation_image_div'},
             ELOGPostElement.SampleDescriptionDiv: {'class_': 'section_div', 'id': 'Samples'},
             ELOGPostElement.SampleList: {'id': 'sample_list_div'},
             ELOGPostElement.ConclusionDiv: {'class_': 'section_div', 'id': 'Conclusion'},
             ELOGPostElement.GeneralAttachment: {'id': 'general_attachment'},
             ELOGPostElement.HTMLNavigation: None,  # placeholder
+            ELOGPostElement.Footer: {'id': 'footer'},
             ELOGPostElement.Script: {'name': 'script'}
         }
         self._page_tags = self.build_page()
 
 
 class PageList(UserList):
     def __init__(self, initialdata=None):
```

### Comparing `autologbook-0.1.3/autologbook/file_system_command.py` & `autologbook-0.1.4/autologbook/file_system_command.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/file_type_guesser.py` & `autologbook-0.1.4/autologbook/file_type_guesser.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/html_helpers.py` & `autologbook-0.1.4/autologbook/html_helpers.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/jinja_integration.py` & `autologbook-0.1.4/autologbook/jinja_integration.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/main_window_ui.py` & `autologbook-0.1.4/autologbook/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/microscope_picture.py` & `autologbook-0.1.4/autologbook/microscope_picture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1689,25 +1689,32 @@
             # for HV add kV if > 1000
             self.params['hv'] = (
                 fei_metadata.get('Beam', 'HV') + 'V',
                 str(round(fei_metadata.getfloat('Beam', 'HV') / 1000)) + 'kV'
             )[fei_metadata.getfloat('Beam', 'HV') > 1000]
 
             self.params['beam'] = fei_metadata.get('Beam', 'Beam')
-            self.params['hfw'] = fei_metadata.getfloat(
-                self.params['beam'], 'HFW')
+            self.params['hfw'] = fei_metadata.getfloat(self.params['beam'], 'HFW')
+            self.params['magnificationmode'] = fei_metadata.getint('Image', 'Magnificationmode', fallback='2')
+            self.params['screenmagnificationmode'] = fei_metadata.getint('Image', 'Screenmagnificationmode',
+                                                                         fallback='2')
+            self.params['magcanvasrealwidth'] = fei_metadata.getfloat('Image', 'magcanvasrealwidth', fallback='0.41440')
+            self.params['screenmagcanvasrealwidth'] = fei_metadata.getfloat('Image', 'screenmagcanvasrealwidth',
+                                                                            fallback='0.41440')
+            if self.params['magnificationmode'] == 3:
+                self.params['magdivider'] = 2.
+            else:
+                self.params['magdivider'] = 1.
             try:
-                self.params['dispwidth'] = fei_metadata.getfloat(
-                    'System', 'DisplayWidth')
+                self.params['dispwidth'] = fei_metadata.getfloat('System', 'DisplayWidth')
                 # for magnification there is a mystery 1.25 scale factor
-                # add kx if > 1000
-                self.params['magnification'] = (
-                    str(round(self.params['dispwidth'] / self.params['hfw'] / 1.25)) + 'x',
-                    str(round(self.params['dispwidth'] / self.params['hfw'] / 1.25 / 1000)) + 'kx'
-                )[round(self.params['dispwidth'] / self.params['hfw'] / 1.25) > 1000]
+                self.params['magnification'] = autotools.pretty_fmt_magnification(
+                    float(self.params['dispwidth']) / float(self.params['hfw']) / 1.25 / self.params['magdivider']
+                )
+
             except ValueError:
                 self.params['dispwidth'] = 'Unknown'
                 self.params['magnification'] = 'Unknown'
 
             self.params['spotsize'] = fei_metadata.getfloat('Beam', 'Spot')
             try:
                 self.params['beamcurrent'] = fei_metadata.getfloat(
```

### Comparing `autologbook-0.1.3/autologbook/model_test_ui.py` & `autologbook-0.1.4/autologbook/model_test_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/navigation_image.py` & `autologbook-0.1.4/autologbook/navigation_image.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/object_factoy.py` & `autologbook-0.1.4/autologbook/object_factoy.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/optical_image.py` & `autologbook-0.1.4/autologbook/optical_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,17 +416,17 @@
                 elif image.format == 'PNG':
                     typ = OpticalImageFactory.guess_type_of_png(image)
                 else:
                     typ = OpticalImageType.GENERIC_OPTICAL_IMAGE
 
             except KeyError:
                 typ = OpticalImageType.GENERIC_OPTICAL_IMAGE
-            finally:
-                image.close()
-                return typ
+
+        image.close()
+        return typ
 
 
 optical_image_factory = OpticalImageFactory()
 optical_image_factory.register_type(OpticalImageType.GENERIC_OPTICAL_IMAGE, GenericOpticalImage)
 optical_image_factory.register_type(OpticalImageType.DIGITAL_CAMERA_OPTICAL_IMAGE, DigitalCameraOpticalImage)
 optical_image_factory.register_type(OpticalImageType.KEYENCE_OPTICAL_IMAGE, KeyenceMicroscopeImage)
 optical_image_factory.register_type(OpticalImageType.DIGITAL_CAMERA_OPTICAL_IMAGE_WITH_GPS,
```

### Comparing `autologbook-0.1.3/autologbook/protocol_editor.py` & `autologbook-0.1.4/autologbook/protocol_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""Module to a graphical protocol editor"""
+"""Module to generate a graphical protocol editor"""
 # ----------------------------------------------------------------------------------------------------------------------
 #  Copyright (c) 2023. Antonio Bulgheroni.
 #  Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 #  documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 #  rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
 #  permit persons to whom the Software is furnished to do so, subject to the following conditions:
 #  The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
@@ -30,14 +30,15 @@
     QMenu,
     QObject,
     QPixmap,
     QPoint,
     QRegExp,
     QStandardItemModel,
     QUrl,
+    QTimer,
 )
 from PyQt5.QtCore import (
     QItemSelection,
     QItemSelectionModel,
     QModelIndex,
     QPersistentModelIndex,
     QSortFilterProxyModel,
@@ -68,23 +69,24 @@
     SectionItem,
     TreeViewerProxyModel,
     UserRole,
     VideoItem,
 )
 from autologbook.protocol_editor_ui import Ui_tree_viewer_dialog
 from autologbook.restore_element import RecoverElementDialog
-from autologbook import autogui
+from autologbook import autogui, autoconfig
 
 __author__ = 'Antonio Bulgheroni'
 __email__ = 'antonio.bulgheroni@gmail.com'
 
 Signal = QtCore.pyqtSignal
 Slot = QtCore.pyqtSlot
+Slot = QtCore.pyqtSlot
 
-log = logging.getLogger('__name__')
+log = logging.getLogger('__main__')
 
 
 class ProtocolEditor(HTMLHelperMixin, QDialog, Ui_tree_viewer_dialog):
     """Dialog window for the protocol editor."""
 
     # Signal to emit a file system command.
     # When the user is performing an operation on a protocol element, this is actually corresponding to a file system
@@ -165,16 +167,18 @@
         # This is linked to the same model as the autolog_tree_viewer and they share the same selection model.
         # At the beginning we set the root of the sample_list_view to the SectionItem named 'Samples'
         self.sample_list_view.setModel(self.tree_model_proxy)
         self.sample_list_view.setContextMenuPolicy(Qt.CustomContextMenu)
         self.sample_list_view_context_menu = self.generate_sample_list_view_context_menu()
         self.sample_list_view.customContextMenuRequested.connect(self.on_sample_list_context_menu_request)
         self.sample_list_view.setSelectionModel(self.autolog_tree_viewer.selectionModel())
+
         self.sample_list_view.setRootIndex(
-            self.tree_model.findItems('Samples', QtCore.Qt.MatchExactly or QtCore.Qt.MatchRecursive, 0)[0].index()
+            self.tree_model_proxy.mapFromSource(
+                self.tree_model.findItems('Samples', QtCore.Qt.MatchExactly or QtCore.Qt.MatchRecursive, 0)[0].index())
         )
 
         # connect the inserted new rows signals
         self.tree_model.rowsInserted.connect(self.new_rows_added)
 
         # connect the selection changed of the selectionModel of the autolog_tree_viewer to the get_and_update_values.
         # This slot is responsible to handle the customization fields (caption, description, extra).
@@ -254,14 +258,19 @@
 
         # install the event filter for some widgets
         self.description_input.installEventFilter(self)
         self.caption_field.installEventFilter(self)
         self.extrainfo_input.installEventFilter(self)
         self.image_preview.installEventFilter(self)
 
+        # start the auto_save timer
+        self.auto_save_timer = QTimer(self)
+        self.auto_save_timer.timeout.connect(self.auto_save)
+        self.auto_save_timer.start(autoconfig.AUTO_SAVE_INTERVAL)
+
     def eventFilter(self, object_: QObject, event: QEvent) -> bool:
         """
         Overload the event filtering for the customized some specific events.
 
         In particular, we are taking care of the following events and sources:
             - FocusIn for caption_field, description_input and extrainfo_input:
                 -> Used to enable/disable the customization edit / special copy and paste tool buttons.
@@ -3041,14 +3050,20 @@
         if self.autolog_tree_viewer.selectionModel().currentIndex().isValid():
             self.update_values(self.autolog_tree_viewer.selectionModel().currentIndex())
             self.tree_model_last_selected_item = QPersistentModelIndex(
                 self.autolog_tree_viewer.selectionModel().currentIndex()
             )
         autotools.dump_yaml_file(self.autolog.yamlDict, self.autolog.yamlFilename)
 
+    @Slot()
+    def auto_save(self):
+        if self.isVisible():
+            log.info('Automatic save of the protocol customizations')
+            self.update_protocol()
+
     def scroll_to_last_selected_item(self):
         """
         Scroll the tree viewer down to the last selected item.
 
         This item is used when the protocol editor window is opened a second time.
         So that the user will be able to continue editing from the same item where he was when he left.
```

### Comparing `autologbook-0.1.3/autologbook/protocol_editor_models.py` & `autologbook-0.1.4/autologbook/protocol_editor_models.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/protocol_editor_ui.py` & `autologbook-0.1.4/autologbook/protocol_editor_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/qt_signal_dispatcher.py` & `autologbook-0.1.4/autologbook/qt_signal_dispatcher.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/rename_dialog_ui.py` & `autologbook-0.1.4/autologbook/rename_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/resource_rc.py` & `autologbook-0.1.4/autologbook/resource_rc.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/resource_rc.rcc` & `autologbook-0.1.4/autologbook/resource_rc.rcc`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/restore_element.py` & `autologbook-0.1.4/autologbook/restore_element.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/restore_element_dialog_ui.py` & `autologbook-0.1.4/autologbook/restore_element_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/sample.py` & `autologbook-0.1.4/autologbook/sample.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/thread_worker.py` & `autologbook-0.1.4/autologbook/thread_worker.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/user_editor_ui.py` & `autologbook-0.1.4/autologbook/user_editor_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/video.py` & `autologbook-0.1.4/autologbook/video.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/conf/type_guesser_regexp.yaml` & `autologbook-0.1.4/autologbook/conf/type_guesser_regexp.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 GENERIC:
   EXCLUDE_PATTERNS:
     - ^.*\.[Tt][Ee]?[Mm][Pp]$
     - ^.*~\$.*\.[Dd][Oo][Cc][Xx]?$
+    - ^.*~.*\.\w{3,4}$
+    - ^.*\\Thumbs.db$
 
 IMAGEFILE:
   EXCLUDE_PATTERNS:
     - ^.*[Cc][Rr][Oo][Pp]{1,2}[Ee]?[Dd}?[\s\S]*[-_][Cc][Rr][Oo][Pp]{1,2}[Ee]?[Dd]?\.[Tt][Ii][Ff]{1,2}$
     - ^.*\\[Ee][Xx][Cc][Ll][Uu][Dd][Ee][Dd]?\\[\s\S]*$
     - ^.*\\[Rr][Ee][Cc][Yy][Cc][Ll][Ee][Dd]?\\[\s\S]*$
   MATCHING_PATTERNS:
@@ -28,15 +30,21 @@
   MATCHING_PATTERNS:
     - ^.*\.[Pp][Dd][Ff]$
     - ^.*\.[Dd][Oo][Cc][Xx]?$
     - ^.*\.[Xx][Ll][Ss][XxMm]?$
     - ^.*\.[Ss][Tt][Gg]$
     - ^.*\.[Pp][Tt][Ff]$
     - ^.*\.[Ee][Xx][Pp]$
-    - ^.*\.[Tt][Xx][Tx]$
+    - ^.*\.[Tt][Xx][Tt]$
+    - ^.*\.[Rr][Tt][Xx]$ # bruker project files
+    - ^.*\.[Bb][Cc][Ff]$ # bruker map files
+    - ^.*\.[Ss][Pp][Xx]$ # bruker spectrum files
+    - ^.*\.[Rr][Tt][Oo]$ # bruker object files
+    - ^.*\.[Rr][Tt][Ll]$ # bruker linescan files
+    - ^.*\.[Rr][Pp][Tt]$ # bruker report files
   EXCLUDE_PATTERNS:
     - ^.*\\[Ee][Xx][Cc][Ll][Uu][Dd][Ee][Dd]?\\[\s\S]*$
     - ^.*\\[Rr][Ee][Cc][Yy][Cc][Ll][Ee][Dd]?\\[\s\S]*$
     - ^.*\.[Uu][Rr][Ll]$
     - ^.*~\$.*\.[Dd][Oo][Cc][Xx]?$
     - ^.*~\$.*\.[Tt][Ee]?[Mm][Pp]$
```

### Comparing `autologbook-0.1.3/autologbook/templates/attachment_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/attachment_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/digital_camera_optical_image_gps_template.yammy` & `autologbook-0.1.4/autologbook/templates/digital_camera_optical_image_gps_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/digital_camera_optical_image_template.yammy` & `autologbook-0.1.4/autologbook/templates/digital_camera_optical_image_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/fei_microscope_picture_template.yammy` & `autologbook-0.1.4/autologbook/templates/fei_microscope_picture_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/general_optical_images_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/general_optical_images_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/macros.yammy` & `autologbook-0.1.4/autologbook/templates/macros.yammy`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,21 @@
 {%- endmacro %}
 
 
 {% macro include_element_custom_row(yaml_dict) -%}
     {% if 'Description' in yaml_dict %}
         {% set pairs = [('description', 'Description'), ('additional', 'Extra')] %}
         {% for class, key in pairs %}
-            tr
-                td
-                    - class {{ class }}
-                    - colspan 7
-                    | {{ yaml_dict[key]|from_markdown }}
+            {% if yaml_dict[key] %}
+                tr
+                    td
+                        - class {{ class }}
+                        - colspan 7
+                        | {{ yaml_dict[key]|from_markdown }}
+            {% endif %}
         {% endfor %}
     {% endif %}
 {%- endmacro %}
 
 {% macro include_hide_command(div) %}
     a.commands
         - onclick hideDiv('{{ div }}')
```

### Comparing `autologbook-0.1.3/autologbook/templates/microscope_picture_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/microscope_picture_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/navigation_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/navigation_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/navigation_image_template.yammy` & `autologbook-0.1.4/autologbook/templates/navigation_image_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/optical_image_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/optical_image_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/protocol_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/protocol_base_template.yammy`

 * *Files 5% similar despite different names*

```diff
@@ -26,8 +26,10 @@
             | No samples found for this protocol
     {% endif %}
 
     {{ include_text_section('Conclusion', include_section_title=True) }}
 
     {% include 'general_attachment_base_template.yammy' %}
 
+    {% include 'footer_base_template.yammy' %}
+
     {% include 'scripts.yammy' %}
```

### Comparing `autologbook-0.1.3/autologbook/templates/quattro_protocol_template.yammy` & `autologbook-0.1.4/autologbook/templates/quattro_protocol_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/sample_attachment_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/sample_attachment_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/sample_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/sample_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/sample_list_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/sample_list_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/sample_microscope_picture_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/sample_microscope_picture_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/sample_optical_image_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/sample_optical_image_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/sample_video_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/sample_video_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/scripts.yammy` & `autologbook-0.1.4/autologbook/templates/scripts.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/title_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/title_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/vega_microscope_picture_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/vega_microscope_picture_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/vega_microscope_picture_jpeg_simple_template.yammy` & `autologbook-0.1.4/autologbook/templates/vega_microscope_picture_jpeg_simple_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/vega_microscope_picture_jpeg_template.yammy` & `autologbook-0.1.4/autologbook/templates/vega_microscope_picture_jpeg_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/video_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/video_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/xl40_microscope_picture_base_template.yammy` & `autologbook-0.1.4/autologbook/templates/xl40_microscope_picture_base_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/templates/xl40_microscope_picture_multi_template.yammy` & `autologbook-0.1.4/autologbook/templates/xl40_microscope_picture_multi_template.yammy`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/about_dialog.ui` & `autologbook-0.1.4/autologbook/ui/about_dialog.ui`

 * *Files 4% similar despite different names*

#### Comparing `autologbook-0.1.3/autologbook/ui/about_dialog.ui` & `autologbook-0.1.4/autologbook/ui/about_dialog.ui`

```diff
@@ -23,15 +23,15 @@
       </iconset>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
         <widget class="QLabel" name="label">
           <property name="text">
             <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;center&quot;&gt;&lt;img src=&quot;:/resources/icons8-logbook-64.png&quot;/&gt;&lt;/p&gt;&lt;p
-       align=&quot;center&quot;&gt;&lt;br/&gt;&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;AUTOLOGBOOK v0.1.3&lt;/p&gt;&lt;p
+       align=&quot;center&quot;&gt;&lt;br/&gt;&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;AUTOLOGBOOK v0.1.4&lt;/p&gt;&lt;p
        align=&quot;center&quot;&gt;A script for automatic logbook generation in microscopy&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;GitHub
        &lt;a href=&quot;https://github.com/abulgher/autologbook&quot;&gt;&lt;span style=&quot; text-decoration:
        underline; color:#0000ff;&quot;&gt;Source Code&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;(C)
        Antonio Bulgheroni - 2022&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;&lt;br/&gt;&lt;a href=&quot;https://icons8.com/icon/pNYOTp5DinZ3/copy&quot;&gt;&lt;span
        style=&quot; text-decoration: underline; color:#0000ff;&quot;&gt;Copy&lt;/span&gt;&lt;/a&gt; icon by &lt;a href=&quot;https://icons8.com&quot;&gt;&lt;span
        style=&quot; text-decoration: underline; color:#0000ff;&quot;&gt;Icons8&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
           </property>
```

### Comparing `autologbook-0.1.3/autologbook/ui/change_sample_dialog.ui` & `autologbook-0.1.4/autologbook/ui/change_sample_dialog.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/configuration_editor.ui` & `autologbook-0.1.4/autologbook/ui/configuration_editor.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/edit_lock_dialog.ui` & `autologbook-0.1.4/autologbook/ui/edit_lock_dialog.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/main_window.ui` & `autologbook-0.1.4/autologbook/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/model_test.ui` & `autologbook-0.1.4/autologbook/ui/model_test.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/protocol_editor.ui` & `autologbook-0.1.4/autologbook/ui/protocol_editor.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/rename_dialog.ui` & `autologbook-0.1.4/autologbook/ui/rename_dialog.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resource.qrc` & `autologbook-0.1.4/autologbook/ui/resource.qrc`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/restore_element_dialog.ui` & `autologbook-0.1.4/autologbook/ui/restore_element_dialog.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/user_editor.ui` & `autologbook-0.1.4/autologbook/ui/user_editor.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-attach-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-attach-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-bold-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-bold-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-cancel-32.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-cancel-32.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-cancel-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-cancel-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-choose-font-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-choose-font-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-close-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-close-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-code-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-code-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-compact-camera-64.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-compact-camera-64.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-copy-all-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-all-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-copy-caption-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-caption-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-copy-description-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-description-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-copy-extra-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-extra-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-copy-link-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-link-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-copy-pair-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-pair-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-copy-single-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-copy-single-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-design-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-design-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-edit-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-edit-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-edit-user-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-edit-user-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-expand-arrow.gif` & `autologbook-0.1.4/autologbook/ui/resources/icons8-expand-arrow.gif`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-green-circle-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-green-circle-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-high-importance-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-high-importance-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-home-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-home-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-hyperlink-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-hyperlink-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-ice-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-ice-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-image-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-image-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-internet-folder-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-internet-folder-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-link-folder-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-link-folder-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-logbook-64.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-logbook-64.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-map-marker-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-map-marker-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-markdown-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-markdown-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-move-up-row-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-move-up-row-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-numbered-list-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-numbered-list-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-ok-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-ok-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-open-envelope-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-open-envelope-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-opened-folder-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-opened-folder-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-opened-folder-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-opened-folder-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-optical-microscope-64.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-optical-microscope-64.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-paste-all-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-paste-all-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-paste-caption-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-paste-caption-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-paste-description-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-paste-description-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-paste-extra-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-paste-extra-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-paste-special-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-paste-special-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-pencil-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-pencil-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-picture-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-picture-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-pictures-folder-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-pictures-folder-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-pictures-folder-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-pictures-folder-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-play-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-play-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-recycle-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-recycle-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-red-circle-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-red-circle-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-save-as-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-save-as-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-search-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-search-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-section-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-section-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-sniper-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-sniper-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-start-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-start-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-start-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-start-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-stop-sign-30.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-stop-sign-30.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-stop-sign-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-stop-sign-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-strikethrough-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-strikethrough-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-support-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-support-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-sync-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-sync-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-tools-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-tools-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-trash-restore-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-trash-restore-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-underline-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-underline-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-update-left-rotation-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-update-left-rotation-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-upload-to-cloud-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-upload-to-cloud-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-user-secured-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-user-secured-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/autologbook/ui/resources/icons8-website-48.png` & `autologbook-0.1.4/autologbook/ui/resources/icons8-website-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/constants.py` & `autologbook-0.1.4/expwizard/constants.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/dialog_compare_experiment_file.py` & `autologbook-0.1.4/expwizard/dialog_compare_experiment_file.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/dialog_compare_experiment_file_ui.py` & `autologbook-0.1.4/expwizard/dialog_compare_experiment_file_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/dialog_select_experiment_file.py` & `autologbook-0.1.4/expwizard/dialog_select_experiment_file.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/dialog_select_experiment_file_ui.py` & `autologbook-0.1.4/expwizard/dialog_select_experiment_file_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/experiment_wizard.py` & `autologbook-0.1.4/expwizard/experiment_wizard.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/experiment_wizard_app.py` & `autologbook-0.1.4/expwizard/experiment_wizard_app.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ini_syntax_highlighter.py` & `autologbook-0.1.4/expwizard/ini_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/resources_rc.py` & `autologbook-0.1.4/expwizard/resources_rc.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/search_results_model.py` & `autologbook-0.1.4/expwizard/search_results_model.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_commit_new_experiment_page.py` & `autologbook-0.1.4/expwizard/wizard_commit_new_experiment_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_commit_new_experiment_page_ui.py` & `autologbook-0.1.4/expwizard/wizard_commit_new_experiment_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_conclusion_page.py` & `autologbook-0.1.4/expwizard/wizard_conclusion_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_conclusion_page_ui.py` & `autologbook-0.1.4/expwizard/wizard_conclusion_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_introduction_page.py` & `autologbook-0.1.4/expwizard/wizard_introduction_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_introduction_page_ui.py` & `autologbook-0.1.4/expwizard/wizard_introduction_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_new_experiment_page.py` & `autologbook-0.1.4/expwizard/wizard_new_experiment_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_new_experiment_page_ui.py` & `autologbook-0.1.4/expwizard/wizard_new_experiment_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_review_configuration_page.py` & `autologbook-0.1.4/expwizard/wizard_review_configuration_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_review_configuration_page_ui.py` & `autologbook-0.1.4/expwizard/wizard_review_configuration_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_search_experiment_page.py` & `autologbook-0.1.4/expwizard/wizard_search_experiment_page.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/wizard_search_experiment_page_ui.py` & `autologbook-0.1.4/expwizard/wizard_search_experiment_page_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/conf/unit_list.yaml` & `autologbook-0.1.4/expwizard/conf/unit_list.yaml`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/dialog_compare_experiment_file.ui` & `autologbook-0.1.4/expwizard/ui/dialog_compare_experiment_file.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/dialog_select_experiment_file.ui` & `autologbook-0.1.4/expwizard/ui/dialog_select_experiment_file.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/wizard_commit_new_experiment_page.ui` & `autologbook-0.1.4/expwizard/ui/wizard_commit_new_experiment_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/wizard_conclusion_page.ui` & `autologbook-0.1.4/expwizard/ui/wizard_conclusion_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/wizard_introduction_page.ui` & `autologbook-0.1.4/expwizard/ui/wizard_introduction_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/wizard_new_experiment_page.ui` & `autologbook-0.1.4/expwizard/ui/wizard_new_experiment_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/wizard_review_configuration_page.ui` & `autologbook-0.1.4/expwizard/ui/wizard_review_configuration_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/wizard_search_experiment_page.ui` & `autologbook-0.1.4/expwizard/ui/wizard_search_experiment_page.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/resources/ec-logo.jpg` & `autologbook-0.1.4/expwizard/ui/resources/ec-logo.jpg`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/resources/glossy-microscope.png` & `autologbook-0.1.4/expwizard/ui/resources/glossy-microscope.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/resources/icons8-error-48.png` & `autologbook-0.1.4/expwizard/ui/resources/icons8-error-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/resources/icons8-fantasy-48.png` & `autologbook-0.1.4/expwizard/ui/resources/icons8-fantasy-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/resources/icons8-new-48.png` & `autologbook-0.1.4/expwizard/ui/resources/icons8-new-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/resources/icons8-new-96.png` & `autologbook-0.1.4/expwizard/ui/resources/icons8-new-96.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/resources/icons8-question-mark-48.png` & `autologbook-0.1.4/expwizard/ui/resources/icons8-question-mark-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/expwizard/ui/resources/icons8-website-48.png` & `autologbook-0.1.4/expwizard/ui/resources/icons8-website-48.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/__init__.py` & `autologbook-0.1.4/labtools/__init__.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/about_image_converter_ui.py` & `autologbook-0.1.4/labtools/about_image_converter_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/event_logger.py` & `autologbook-0.1.4/labtools/event_logger.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/fei_image_manipulator.py` & `autologbook-0.1.4/labtools/fei_image_manipulator.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/image_converter.py` & `autologbook-0.1.4/labtools/image_converter.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/image_converter_gui.py` & `autologbook-0.1.4/labtools/image_converter_gui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/main_window_image_converter_ui.py` & `autologbook-0.1.4/labtools/main_window_image_converter_ui.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/metadata_dumper.py` & `autologbook-0.1.4/labtools/metadata_dumper.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/mirror_maker.py` & `autologbook-0.1.4/labtools/mirror_maker.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/qt_exception_handler.py` & `autologbook-0.1.4/labtools/qt_exception_handler.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/resource_rc.py` & `autologbook-0.1.4/labtools/resource_rc.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/util.py` & `autologbook-0.1.4/labtools/util.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/ui/about_image_converter.ui` & `autologbook-0.1.4/labtools/ui/about_image_converter.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/ui/main_window_image_converter.ui` & `autologbook-0.1.4/labtools/ui/main_window_image_converter.ui`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/labtools/ui/resources/icons8-picture-64.png` & `autologbook-0.1.4/labtools/ui/resources/icons8-picture-64.png`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/test/__init__.py` & `autologbook-0.1.4/test/__init__.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/test/test_autotools.py` & `autologbook-0.1.4/test/test_autotools.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/test/test_element_type_guesser.py` & `autologbook-0.1.4/test/test_element_type_guesser.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/test/test_enums.py` & `autologbook-0.1.4/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/test/test_file_utils.py` & `autologbook-0.1.4/test/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/test/test_picture_resolution.py` & `autologbook-0.1.4/test/test_picture_resolution.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/test/test_protocol_elements.py` & `autologbook-0.1.4/test/test_protocol_elements.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/test/test_url_guessing.py` & `autologbook-0.1.4/test/test_url_guessing.py`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/.gitignore` & `autologbook-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/LICENSE.txt` & `autologbook-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/README.md` & `autologbook-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `autologbook-0.1.3/pyproject.toml` & `autologbook-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 [tool.isort]
 line_length = 119
 multi_line_output = 3
 include_trailing_comma = true
 
 [project]
 name = "autologbook"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name = "Antonio Bulgheroni", email = "antonio.bulgheroni@gmail.com" },
 ]
 dependencies = [
   'py_elog >= 1.3.16',
   'Markdown ==3.4.1',
   'watchdog >= 2.1.9',
```

### Comparing `autologbook-0.1.3/PKG-INFO` & `autologbook-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autologbook
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python toolkit for the automatic generation of elog entries of SEM analysis.
 Project-URL: Homepage, https://github.com/abulgher/autologbook
 Author-email: Antonio Bulgheroni <antonio.bulgheroni@gmail.com>
 License: Copyright (c) 2022 Antonio Bulgheroni
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

