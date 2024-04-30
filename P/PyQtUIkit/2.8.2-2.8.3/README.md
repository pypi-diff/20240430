# Comparing `tmp/PyQtUIkit-2.8.2.tar.gz` & `tmp/PyQtUIkit-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.8.2.tar", last modified: Fri Apr 26 07:56:03 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.8.3.tar", last modified: Mon Apr 29 17:16:12 2024, max compression
```

## Comparing `PyQtUIkit-2.8.2.tar` & `PyQtUIkit-2.8.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 07:56:03.808869 PyQtUIkit-2.8.2/
--rw-rw-rw-   0        0        0     1090 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-26 07:56:03.808869 PyQtUIkit-2.8.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-26 07:56:03.777119 PyQtUIkit-2.8.2/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3896 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/_icons.py
--rw-rw-rw-   0        0        0     3271 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/_translate.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:56:03.777119 PyQtUIkit-2.8.2/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:56:03.777119 PyQtUIkit-2.8.2/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     5248 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:56:03.793349 PyQtUIkit-2.8.2/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-26 07:56:03.793349 PyQtUIkit-2.8.2/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     4222 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  2340473 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1830 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/themes/locale.py
--rw-rw-rw-   0        0        0     1470 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:56:03.808869 PyQtUIkit-2.8.2/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1734 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3304 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     7885 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2794 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    11413 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     8328 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5876 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2542 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/form.py
--rw-rw-rw-   0        0        0     4350 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/grid_layout.py
--rw-rw-rw-   0        0        0     2280 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     1578 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1171 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     5344 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/layout.py
--rw-rw-rw-   0        0        0     1697 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3671 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1758 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     4253 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     4948 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/menu_bar.py
--rw-rw-rw-   0        0        0     7145 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2647 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6805 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     4021 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7515 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    14123 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1297 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/tabs_layout.py
--rw-rw-rw-   0        0        0     4538 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    17878 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/PyQtUIkit/widgets/tree_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:56:03.777119 PyQtUIkit-2.8.2/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-26 07:56:03.000000 PyQtUIkit-2.8.2/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2024-04-26 07:56:03.000000 PyQtUIkit-2.8.2/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 07:56:03.000000 PyQtUIkit-2.8.2/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-04-26 07:56:03.000000 PyQtUIkit-2.8.2/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-04-26 07:56:03.000000 PyQtUIkit-2.8.2/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-26 07:56:03.000000 PyQtUIkit-2.8.2/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 07:56:03.808869 PyQtUIkit-2.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1474 2024-04-26 07:55:13.000000 PyQtUIkit-2.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:16:12.995680 PyQtUIkit-2.8.3/
+-rw-rw-rw-   0        0        0     1090 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-29 17:16:12.995680 PyQtUIkit-2.8.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 17:16:12.948808 PyQtUIkit-2.8.3/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3896 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/_icons.py
+-rw-rw-rw-   0        0        0     3271 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/_translate.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:16:12.964425 PyQtUIkit-2.8.3/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:16:12.964425 PyQtUIkit-2.8.3/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     5248 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:16:12.980054 PyQtUIkit-2.8.3/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-29 17:16:12.980054 PyQtUIkit-2.8.3/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     4222 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  2340473 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1830 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/themes/locale.py
+-rw-rw-rw-   0        0        0     1470 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:16:12.995680 PyQtUIkit-2.8.3/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1734 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3304 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     8034 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2794 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    11413 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     8328 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5876 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2542 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/form.py
+-rw-rw-rw-   0        0        0     4350 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/grid_layout.py
+-rw-rw-rw-   0        0        0     2280 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     1578 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1171 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     5436 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/layout.py
+-rw-rw-rw-   0        0        0     1697 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3671 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1758 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     4253 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     4948 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/menu_bar.py
+-rw-rw-rw-   0        0        0     7145 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6805 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     4021 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7515 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    14123 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1313 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/tabs_layout.py
+-rw-rw-rw-   0        0        0     4538 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    17878 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/PyQtUIkit/widgets/tree_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:16:12.964425 PyQtUIkit-2.8.3/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-29 17:16:12.000000 PyQtUIkit-2.8.3/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2024-04-29 17:16:12.000000 PyQtUIkit-2.8.3/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:16:12.000000 PyQtUIkit-2.8.3/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-04-29 17:16:12.000000 PyQtUIkit-2.8.3/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-04-29 17:16:12.000000 PyQtUIkit-2.8.3/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-29 17:16:12.000000 PyQtUIkit-2.8.3/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:16:12.995680 PyQtUIkit-2.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-04-29 17:15:13.000000 PyQtUIkit-2.8.3/setup.py
```

### Comparing `PyQtUIkit-2.8.2/LICENSE` & `PyQtUIkit-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PKG-INFO` & `PyQtUIkit-2.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.8.2
+Version: 2.8.3
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/_icons.py` & `PyQtUIkit-2.8.3/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/_translate.py` & `PyQtUIkit-2.8.3/PyQtUIkit/_translate.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.8.3/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.8.3/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.8.3/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/core/font.py` & `PyQtUIkit-2.8.3/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.8.3/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.8.3/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.8.3/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.8.3/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.8.3/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.8.3/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/themes/locale.py` & `PyQtUIkit-2.8.3/PyQtUIkit/themes/locale.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.8.3/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.8.3/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/button.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,48 +136,48 @@
 
     def __init__(self, orientation: Orientation = Orientation.HORIZONTAL):
         super().__init__()
         self.__orientation = orientation
         self.__layout = QHBoxLayout() if orientation == KitLayoutButton.Orientation.HORIZONTAL else QVBoxLayout()
         self.__layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(self.__layout)
-        self._widgets = []
+        self.__widgets = []
 
     def addWidget(self, widget: QWidget, stretch: int = None, alignment=None):
         if alignment is not None:
             self.__layout.addWidget(widget, stretch, alignment)
         elif stretch is not None:
             self.__layout.addWidget(widget, stretch)
         else:
             self.__layout.addWidget(widget)
-        self._widgets.append(widget)
+        self.__widgets.append(widget)
         if hasattr(widget, '_set_tm'):
             widget._set_tm(self._tm)
 
     def insertWidget(self, index: int, widget: QWidget, stretch: int = None, alignment=None):
         if alignment is not None:
             self.__layout.insertWidget(index, widget, stretch, alignment)
         elif stretch is not None:
             self.__layout.insertWidget(index, widget, stretch)
         else:
             self.__layout.insertWidget(index, widget)
-        self._widgets.insert(index, widget)
+        self.__widgets.insert(index, widget)
         if hasattr(widget, '_set_tm'):
             widget._set_tm(self._tm)
 
     def deleteWidget(self, w: int | QWidget):
         if isinstance(w, int):
             w = self.__layout.takeAt(w).widget()
         w.setParent(None)
         return w
 
     def clear(self):
         for _ in range(self.__layout.count()):
             self.__layout.takeAt(0).widget().setParent(None)
-        self._widgets.clear()
+        self.__widgets.clear()
 
     def setAlignment(self, a):
         self.__layout.setAlignment(a)
 
     def getAlignment(self):
         return self.__layout.alignment()
 
@@ -209,22 +209,27 @@
         return self.__layout.contentsMargins()
 
     def count(self):
         return self.__layout.count()
 
     def _set_tm(self, tm):
         super()._set_tm(tm)
-        for el in self._widgets:
+        for el in self.__widgets:
             if hasattr(el, '_set_tm'):
                 el._set_tm(tm)
 
+    def _apply_lang(self):
+        for el in self.__widgets:
+            if hasattr(el, '_apply_lang'):
+                el._apply_lang()
+
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         super()._apply_theme()
-        for el in self._widgets:
+        for el in self.__widgets:
             if hasattr(el, '_apply_theme'):
                 el._apply_theme()
 
     padding = MethodsProperty(getContentsMargins, _set_margins)
     spacing = MethodsProperty(getSpacing, setSpacing)
     alignment = MethodsProperty(getAlignment, setAlignment)
```

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/form.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/form.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/grid_layout.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/grid_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/layout.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class KitBoxLayout(QWidget, _KitWidget):
     border = IntProperty('border', 0)
     radius = IntProperty('radius', 4)
 
     def __init__(self, orientation=Qt.Orientation.Horizontal):
         super().__init__()
-        self._widgets = []
+        self.__widgets = []
         self._main_palette = 'Transparent'
 
         strange_layout = QVBoxLayout()
         strange_layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(strange_layout)
 
         strange_widget = QWidget()
@@ -31,42 +31,46 @@
     def addWidget(self, widget: QWidget, stretch: int = None, alignment=None):
         if alignment is not None:
             self.__layout.addWidget(widget, stretch, alignment)
         elif stretch is not None:
             self.__layout.addWidget(widget, stretch)
         else:
             self.__layout.addWidget(widget)
-        self._widgets.append(widget)
+        self.__widgets.append(widget)
         if hasattr(widget, '_set_tm'):
             widget._set_tm(self._tm)
 
     def insertWidget(self, index: int, widget: QWidget, stretch: int = None, alignment=None):
         if alignment is not None:
             self.__layout.insertWidget(index, widget, stretch, alignment)
         elif stretch is not None:
             self.__layout.insertWidget(index, widget, stretch)
         else:
             self.__layout.insertWidget(index, widget)
-        self._widgets.insert(index, widget)
+        self.__widgets.insert(index, widget)
         if hasattr(widget, '_set_tm'):
             widget._set_tm(self._tm)
 
     def removeWidget(self, w: int | QWidget):
         if isinstance(w, QWidget):
-            w = self._widgets.index(w)
+            w = self.__widgets.index(w)
 
-        self._widgets.pop(w)
+        self.__widgets.pop(w)
         w = self.__layout.takeAt(w).widget()
         w.setParent(None)
         return w
 
+    def widgets(self):
+        for el in self.__widgets:
+            yield el
+
     def clear(self):
         for _ in range(self.__layout.count()):
             self.__layout.takeAt(0).widget().setParent(None)
-        self._widgets.clear()
+        self.__widgets.clear()
 
     def setAlignment(self, a):
         self.__layout.setAlignment(a)
 
     def getAlignment(self):
         return self.__layout.alignment()
 
@@ -101,36 +105,36 @@
         return self.__layout.contentsMargins()
 
     def count(self):
         return self.__layout.count()
 
     def _set_tm(self, tm):
         super()._set_tm(tm)
-        for el in self._widgets:
+        for el in self.__widgets:
             if hasattr(el, '_set_tm'):
                 el._set_tm(tm)
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
-        for el in self._widgets:
+        for el in self.__widgets:
             if hasattr(el, '_apply_theme'):
                 el._apply_theme()
         self.setStyleSheet(f"""
         QWidget {{
             background-color: {self.main_palette.main};
             border: {self.border}px solid {self.border_palette.main};
             border-radius: {self.radius}px;
         }}
         """)
 
     def _apply_lang(self):
         if not self._tm or not self._tm.active:
             return
-        for el in self._widgets:
+        for el in self.__widgets:
             if hasattr(el, '_apply_theme'):
                 el._apply_lang()
 
     padding = MethodsProperty(getContentsMargins, _set_margins)
     spacing = MethodsProperty(getSpacing, setSpacing)
     alignment = MethodsProperty(getAlignment, setAlignment)
     max_width = MethodsProperty(QWidget.maximumWidth, QWidget.setMaximumWidth)
```

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/menu_bar.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/tab_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/tabs_layout.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/tabs_layout.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,21 +14,22 @@
         super().insertWidget(index, widget)
         if self.__current is None:
             self.__current = index
         else:
             widget.hide()
 
     def addWidget(self, widget: QWidget, *args):
-        self.insertWidget(len(self._widgets), widget)
+        self.insertWidget(self.count(), widget)
 
     def setCurrent(self, index):
-        if self.__current is not None and self.__current < len(self._widgets):
-            self._widgets[self.__current].hide()
+        widgets = list(self.widgets())
+        if self.__current is not None and self.__current < self.count():
+            widgets[self.__current].hide()
         self.__current = index
-        self._widgets[self.__current].show()
+        widgets[self.__current].show()
 
     def connect(self, widget: KitTabBar | KitNavigation | KitVRadio | KitHRadio):
         if self.__connected_widget is not None:
             raise Exception("can connect only one widget")
         self.__connected_widget = widget
         widget.currentChanged.connect(self.setCurrent)
         if widget.currentIndex():
```

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.8.3/PyQtUIkit/widgets/tree_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.8.3/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.8.2
+Version: 2.8.3
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.8.2/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.8.3/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.2/setup.py` & `PyQtUIkit-2.8.3/setup.py`

 * *Files identical despite different names*

