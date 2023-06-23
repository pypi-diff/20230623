# Comparing `tmp/ovos-gui-plugin-shell-companion-0.0.0a8.tar.gz` & `tmp/ovos-gui-plugin-shell-companion-0.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-gui-plugin-shell-companion-0.0.0a8.tar", last modified: Wed Jun 21 14:59:01 2023, max compression
+gzip compressed data, was "ovos-gui-plugin-shell-companion-0.0.0a9.tar", last modified: Thu Jun 22 00:21:22 2023, max compression
```

## Comparing `ovos-gui-plugin-shell-companion-0.0.0a8.tar` & `ovos-gui-plugin-shell-companion-0.0.0a9.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.140413 ovos-gui-plugin-shell-companion-0.0.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-21 14:59:01.136413 ovos-gui-plugin-shell-companion-0.0.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.116413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/color_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/cui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/descriptions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.116413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.120413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_HtmlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.124413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.124413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/code/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js
--rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.124413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.124413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/NameSelect.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    10909 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.128413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3790 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    26178 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.128413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/snd/
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.136413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts
--rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/wigets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:59:01.120413 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:59:01.000000 ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:59:01.140413 ovos-gui-plugin-shell-companion-0.0.0a8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2949 2023-06-21 14:59:00.000000 ovos-gui-plugin-shell-companion-0.0.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.044116 ovos-gui-plugin-shell-companion-0.0.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-22 00:21:22.044116 ovos-gui-plugin-shell-companion-0.0.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.020115 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/color_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/cui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/descriptions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.016115 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.028115 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_HtmlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.032116 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.032116 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.036116 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.036116 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/NameSelect.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    10909 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.036116 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3790 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    26178 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.036116 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/snd/
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.044116 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/wigets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:21:22.024115 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-22 00:21:21.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-22 00:21:22.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:21:21.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 00:21:21.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 00:21:21.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 00:21:21.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:21:21.000000 ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:21:22.044116 ovos-gui-plugin-shell-companion-0.0.0a9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3190 2023-06-22 00:21:18.000000 ovos-gui-plugin-shell-companion-0.0.0a9/setup.py
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/LICENSE` & `ovos-gui-plugin-shell-companion-0.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/README.md` & `ovos-gui-plugin-shell-companion-0.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/__init__.py` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/brightness.py` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/brightness.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/color_manager.py` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/color_manager.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/config.py` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/config.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/cui.py` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/cui.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/descriptions.json` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/descriptions.json`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/snd/clicked.wav`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion/wigets.py` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion/wigets.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt` & `ovos-gui-plugin-shell-companion-0.0.0a9/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a8/setup.py` & `ovos-gui-plugin-shell-companion-0.0.0a9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,19 +46,27 @@
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join('..', path, filename))
     return paths
 
 
+def get_description():
+    with open(os.path.join(BASEDIR, "README.md"), "r") as f:
+        long_description = f.read()
+    return long_description
+
+
 PLUGIN_ENTRY_POINT = 'ovos-gui-plugin-shell-companion=ovos_gui_plugin_shell_companion:OVOSShellCompanionExtension'
 setup(
     name='ovos-gui-plugin-shell-companion',
     version=get_version(),
     description='GUI plugin for ovos-shell',
+    long_description=get_description(),
+    long_description_content_type="text/markdown",
     url='https://github.com/OpenVoiceOS/ovos-gui-plugin-shell-companion',
     author='Aiix',
     author_email='aix.m@outlook.com',
     license='Apache-2.0',
     packages=['ovos_gui_plugin_shell_companion'],
     package_data={'': package_files('ovos_gui_plugin_shell_companion')},
     install_requires=required("requirements.txt"),
```

