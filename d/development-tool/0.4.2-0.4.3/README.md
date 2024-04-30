# Comparing `tmp/development-tool-0.4.2.tar.gz` & `tmp/development-tool-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/development-tool-0.4.2.tar", last modified: Fri Apr 26 14:51:41 2024, max compression
+gzip compressed data, was "dist/development-tool-0.4.3.tar", last modified: Tue Apr 30 06:57:39 2024, max compression
```

## Comparing `development-tool-0.4.2.tar` & `development-tool-0.4.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:41.000000 development-tool-0.4.2/
--rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:44.000000 development-tool-0.4.2/License.txt
--rw-r--r--   0 alex       (501) staff       (20)      237 2024-04-26 14:51:41.000000 development-tool-0.4.2/PKG-INFO
--rwx------   0 alex       (501) staff       (20)        9 2024-03-26 13:20:44.000000 development-tool-0.4.2/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/
--rwx------   0 alex       (501) staff       (20)      237 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/PKG-INFO
--rwx------   0 alex       (501) staff       (20)     5336 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/SOURCES.txt
--rwx------   0 alex       (501) staff       (20)        1 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/dependency_links.txt
--rwx------   0 alex       (501) staff       (20)       76 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/entry_points.txt
--rwx------   0 alex       (501) staff       (20)       14 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/namespace_packages.txt
--rwx------   0 alex       (501) staff       (20)        6 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/requires.txt
--rwx------   0 alex       (501) staff       (20)       14 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/
--rwx------   0 alex       (501) staff       (20)       55 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/
--rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/
--rwx------   0 alex       (501) staff       (20)      799 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/Gpt4AllManagement.py
--rwx------   0 alex       (501) staff       (20)    14328 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/MetManagement.py
--rwx------   0 alex       (501) staff       (20)     4882 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/VarManagement.py
--rwx------   0 alex       (501) staff       (20)     2087 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/WrapMessageBox.py
--rwx------   0 alex       (501) staff       (20)      324 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/dataset_devellopper/
--rwx------   0 alex       (501) staff       (20)       87 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/dataset_devellopper/fake_input.csv
--rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/dataset_devellopper/fakeows.ows
--rwx------   0 alex       (501) staff       (20)       49 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/dataset_devellopper/readme.txt
--rw-r--r--   0 alex       (501) staff       (20)     9163 2024-04-26 14:50:42.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/document_eater.py
--rwx------   0 alex       (501) staff       (20)    20858 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/goto.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/
--rwx------   0 alex       (501) staff       (20)   269355 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Emblem_of_Napoleon_Bonaparte.svg
--rwx------   0 alex       (501) staff       (20)     4161 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH.svg
--rwx------   0 alex       (501) staff       (20)     4259 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH_4.svg
--rwx------   0 alex       (501) staff       (20)     6129 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH_4_jc.svg
--rwx------   0 alex       (501) staff       (20)  1310135 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Napoleon2.svg
--rwx------   0 alex       (501) staff       (20)    82296 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Pikachu SVG File.svg
--rwx------   0 alex       (501) staff       (20)     1364 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Workflow.svg
--rwx------   0 alex       (501) staff       (20)      506 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/category.svg
--rwx------   0 alex       (501) staff       (20)    17140 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/chat-bot.png
--rwx------   0 alex       (501) staff       (20)     9815 2024-03-27 16:51:28.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/data-integration.png
--rwx------   0 alex       (501) staff       (20)     6493 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/database.svg
--rwx------   0 alex       (501) staff       (20)    16824 2024-03-13 15:23:26.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/documents.png
--rwx------   0 alex       (501) staff       (20)     1402 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/download-svgrepo-com.svg
--rwx------   0 alex       (501) staff       (20)    10205 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/duplicate.png
--rwx------   0 alex       (501) staff       (20)    40437 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/ecriture.svg
--rwx------   0 alex       (501) staff       (20)    24354 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/file-transfer.png
--rwx------   0 alex       (501) staff       (20)    21756 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/goto.png
--rwx------   0 alex       (501) staff       (20)    38778 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/icon_surrogate_learner.png
--rwx------   0 alex       (501) staff       (20)    40434 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/icon_surrogate_predict.png
--rwx------   0 alex       (501) staff       (20)    16844 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/input.png
--rwx------   0 alex       (501) staff       (20)     4781 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/interrupteur.svg
--rwx------   0 alex       (501) staff       (20)    29352 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_export_score.png
--rwx------   0 alex       (501) staff       (20)    20371 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_open_file_resize_alpha_channel.png
--rwx------   0 alex       (501) staff       (20)    30017 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_optuna_parameters_setting.png
--rwx------   0 alex       (501) staff       (20)    12060 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_output_table.png
--rwx------   0 alex       (501) staff       (20)     1801 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/label.svg
--rwx------   0 alex       (501) staff       (20)    10741 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/lecture.svg
--rwx------   0 alex       (501) staff       (20)      631 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/mywidget.svg
--rwx------   0 alex       (501) staff       (20)     1738 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/openai.svg
--rwx------   0 alex       (501) staff       (20)     3945 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/optuna.svg
--rwx------   0 alex       (501) staff       (20)    16483 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/output.png
--rwx------   0 alex       (501) staff       (20)     3591 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tank-canon-svgrepo-com.svg
--rwx------   0 alex       (501) staff       (20)    23619 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tool.png
--rwx------   0 alex       (501) staff       (20)     2880 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tutoriel_bouton.svg
--rwx------   0 alex       (501) staff       (20)      394 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/upload-svgrepo-com.svg
--rwx------   0 alex       (501) staff       (20)     2516 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/variable_editor.svg
--rwx------   0 alex       (501) staff       (20)    24762 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/war-svgrepo-com.png
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/
--rwx------   0 alex       (501) staff       (20)    15981 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange.png
--rwx------   0 alex       (501) staff       (20)     9070 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_18px.png
--rwx------   0 alex       (501) staff       (20)    15224 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_30px.png
--rwx------   0 alex       (501) staff       (20)     2746 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/interrupteur_ferme.svg
--rwx------   0 alex       (501) staff       (20)     3530 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/interrupteur_ouvert.svg
--rwx------   0 alex       (501) staff       (20)     9329 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/khk_label_explanation.svg
--rwx------   0 alex       (501) staff       (20)     2597 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh.svg
--rwx------   0 alex       (501) staff       (20)     2598 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh2.svg
--rwx------   0 alex       (501) staff       (20)     2606 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh_with_txt.svg
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/
--rwx------   0 alex       (501) staff       (20)    19522 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/Table_management.py
--rwx------   0 alex       (501) staff       (20)     2136 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/Utils_box.py
--rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis.tab
--rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis_permutation_tototo.tab
--rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/zoubida.dada
--rwx------   0 alex       (501) staff       (20)     1082 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/zoubida2.dada
--rwx------   0 alex       (501) staff       (20)     3610 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/llm.py
--rwx------   0 alex       (501) staff       (20)     3928 2024-03-26 15:12:50.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/load_workflow.py
--rwx------   0 alex       (501) staff       (20)    15322 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/orange_sub_workflow.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:41.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/
--rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example1.ows
--rwx------   0 alex       (501) staff       (20)      642 2024-03-26 13:33:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example1.txt
--rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example2.ows
--rwx------   0 alex       (501) staff       (20)      695 2024-03-26 13:33:34.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example2.txt
--rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example3.ows
--rwx------   0 alex       (501) staff       (20)      703 2024-03-26 13:33:28.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example3.txt
--rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example4.ows
--rwx------   0 alex       (501) staff       (20)      787 2024-03-26 13:33:14.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example4.txt
--rwx------   0 alex       (501) staff       (20)     6790 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/shared_functions.py
--rwx------   0 alex       (501) staff       (20)      682 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/shared_variables.py
--rwx------   0 alex       (501) staff       (20)    33276 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/subworkflow_input.py
--rwx------   0 alex       (501) staff       (20)     3987 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/subworkflow_output.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:41.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/widget_designer/
--rw-r--r--   0 alex       (501) staff       (20)     2625 2024-04-26 14:51:03.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/widget_designer/document_eater.ui
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-26 14:51:41.000000 development-tool-0.4.2/setup.cfg
--rwx------   0 alex       (501) staff       (20)     1904 2024-04-26 14:51:31.000000 development-tool-0.4.2/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/
+-rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:44.000000 development-tool-0.4.3/License.txt
+-rw-r--r--   0 alex       (501) staff       (20)      237 2024-04-30 06:57:39.000000 development-tool-0.4.3/PKG-INFO
+-rwx------   0 alex       (501) staff       (20)        9 2024-03-26 13:20:44.000000 development-tool-0.4.3/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/development_tool.egg-info/
+-rwx------   0 alex       (501) staff       (20)      237 2024-04-30 06:57:39.000000 development-tool-0.4.3/development_tool.egg-info/PKG-INFO
+-rwx------   0 alex       (501) staff       (20)     5336 2024-04-30 06:57:39.000000 development-tool-0.4.3/development_tool.egg-info/SOURCES.txt
+-rwx------   0 alex       (501) staff       (20)        1 2024-04-30 06:57:39.000000 development-tool-0.4.3/development_tool.egg-info/dependency_links.txt
+-rwx------   0 alex       (501) staff       (20)       76 2024-04-30 06:57:39.000000 development-tool-0.4.3/development_tool.egg-info/entry_points.txt
+-rwx------   0 alex       (501) staff       (20)       14 2024-04-30 06:57:39.000000 development-tool-0.4.3/development_tool.egg-info/namespace_packages.txt
+-rwx------   0 alex       (501) staff       (20)        6 2024-04-30 06:57:39.000000 development-tool-0.4.3/development_tool.egg-info/requires.txt
+-rwx------   0 alex       (501) staff       (20)       14 2024-04-30 06:57:39.000000 development-tool-0.4.3/development_tool.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/orangecontrib/
+-rwx------   0 alex       (501) staff       (20)       55 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/orangecontrib/development_tool/
+-rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/
+-rwx------   0 alex       (501) staff       (20)      799 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/Gpt4AllManagement.py
+-rwx------   0 alex       (501) staff       (20)    14328 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/MetManagement.py
+-rwx------   0 alex       (501) staff       (20)     4882 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/VarManagement.py
+-rwx------   0 alex       (501) staff       (20)     2087 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/WrapMessageBox.py
+-rwx------   0 alex       (501) staff       (20)      324 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/dataset_devellopper/
+-rwx------   0 alex       (501) staff       (20)       87 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/dataset_devellopper/fake_input.csv
+-rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/dataset_devellopper/fakeows.ows
+-rwx------   0 alex       (501) staff       (20)       49 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/dataset_devellopper/readme.txt
+-rw-r--r--   0 alex       (501) staff       (20)     9167 2024-04-30 06:57:32.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/document_eater.py
+-rwx------   0 alex       (501) staff       (20)    20858 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/goto.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/
+-rwx------   0 alex       (501) staff       (20)   269355 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Emblem_of_Napoleon_Bonaparte.svg
+-rwx------   0 alex       (501) staff       (20)     4161 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Logo_HKH.svg
+-rwx------   0 alex       (501) staff       (20)     4259 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Logo_HKH_4.svg
+-rwx------   0 alex       (501) staff       (20)     6129 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Logo_HKH_4_jc.svg
+-rwx------   0 alex       (501) staff       (20)  1310135 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Napoleon2.svg
+-rwx------   0 alex       (501) staff       (20)    82296 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Pikachu SVG File.svg
+-rwx------   0 alex       (501) staff       (20)     1364 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Workflow.svg
+-rwx------   0 alex       (501) staff       (20)      506 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/category.svg
+-rwx------   0 alex       (501) staff       (20)    17140 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/chat-bot.png
+-rwx------   0 alex       (501) staff       (20)     9815 2024-03-27 16:51:28.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/data-integration.png
+-rwx------   0 alex       (501) staff       (20)     6493 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/database.svg
+-rwx------   0 alex       (501) staff       (20)    16824 2024-03-13 15:23:26.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/documents.png
+-rwx------   0 alex       (501) staff       (20)     1402 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/download-svgrepo-com.svg
+-rwx------   0 alex       (501) staff       (20)    10205 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/duplicate.png
+-rwx------   0 alex       (501) staff       (20)    40437 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/ecriture.svg
+-rwx------   0 alex       (501) staff       (20)    24354 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/file-transfer.png
+-rwx------   0 alex       (501) staff       (20)    21756 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/goto.png
+-rwx------   0 alex       (501) staff       (20)    38778 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/icon_surrogate_learner.png
+-rwx------   0 alex       (501) staff       (20)    40434 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/icon_surrogate_predict.png
+-rwx------   0 alex       (501) staff       (20)    16844 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/input.png
+-rwx------   0 alex       (501) staff       (20)     4781 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/interrupteur.svg
+-rwx------   0 alex       (501) staff       (20)    29352 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/jcm_export_score.png
+-rwx------   0 alex       (501) staff       (20)    20371 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/jcm_open_file_resize_alpha_channel.png
+-rwx------   0 alex       (501) staff       (20)    30017 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/jcm_optuna_parameters_setting.png
+-rwx------   0 alex       (501) staff       (20)    12060 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/jcm_output_table.png
+-rwx------   0 alex       (501) staff       (20)     1801 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/label.svg
+-rwx------   0 alex       (501) staff       (20)    10741 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/lecture.svg
+-rwx------   0 alex       (501) staff       (20)      631 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/mywidget.svg
+-rwx------   0 alex       (501) staff       (20)     1738 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/openai.svg
+-rwx------   0 alex       (501) staff       (20)     3945 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/optuna.svg
+-rwx------   0 alex       (501) staff       (20)    16483 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/output.png
+-rwx------   0 alex       (501) staff       (20)     3591 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/tank-canon-svgrepo-com.svg
+-rwx------   0 alex       (501) staff       (20)    23619 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/tool.png
+-rwx------   0 alex       (501) staff       (20)     2880 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/tutoriel_bouton.svg
+-rwx------   0 alex       (501) staff       (20)      394 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/upload-svgrepo-com.svg
+-rwx------   0 alex       (501) staff       (20)     2516 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/variable_editor.svg
+-rwx------   0 alex       (501) staff       (20)    24762 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/war-svgrepo-com.png
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/img/
+-rwx------   0 alex       (501) staff       (20)    15981 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/img/bandeau_pour_orange.png
+-rwx------   0 alex       (501) staff       (20)     9070 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_18px.png
+-rwx------   0 alex       (501) staff       (20)    15224 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_30px.png
+-rwx------   0 alex       (501) staff       (20)     2746 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/img/interrupteur_ferme.svg
+-rwx------   0 alex       (501) staff       (20)     3530 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/img/interrupteur_ouvert.svg
+-rwx------   0 alex       (501) staff       (20)     9329 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/img/khk_label_explanation.svg
+-rwx------   0 alex       (501) staff       (20)     2597 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/img/refresh.svg
+-rwx------   0 alex       (501) staff       (20)     2598 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/img/refresh2.svg
+-rwx------   0 alex       (501) staff       (20)     2606 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/img/refresh_with_txt.svg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/
+-rwx------   0 alex       (501) staff       (20)    19522 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/Table_management.py
+-rwx------   0 alex       (501) staff       (20)     2136 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/Utils_box.py
+-rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis.tab
+-rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis_permutation_tototo.tab
+-rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/zoubida.dada
+-rwx------   0 alex       (501) staff       (20)     1082 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/zoubida2.dada
+-rwx------   0 alex       (501) staff       (20)     3610 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/llm.py
+-rwx------   0 alex       (501) staff       (20)     3928 2024-03-26 15:12:50.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/load_workflow.py
+-rwx------   0 alex       (501) staff       (20)    15322 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/orange_sub_workflow.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/
+-rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example1.ows
+-rwx------   0 alex       (501) staff       (20)      642 2024-03-26 13:33:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example1.txt
+-rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example2.ows
+-rwx------   0 alex       (501) staff       (20)      695 2024-03-26 13:33:34.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example2.txt
+-rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example3.ows
+-rwx------   0 alex       (501) staff       (20)      703 2024-03-26 13:33:28.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example3.txt
+-rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example4.ows
+-rwx------   0 alex       (501) staff       (20)      787 2024-03-26 13:33:14.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example4.txt
+-rwx------   0 alex       (501) staff       (20)     6790 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/shared_functions.py
+-rwx------   0 alex       (501) staff       (20)      682 2024-03-26 13:20:46.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/shared_variables.py
+-rwx------   0 alex       (501) staff       (20)    33276 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/subworkflow_input.py
+-rwx------   0 alex       (501) staff       (20)     3987 2024-03-26 13:20:44.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/subworkflow_output.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-30 06:57:39.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/widget_designer/
+-rw-r--r--   0 alex       (501) staff       (20)     2625 2024-04-26 14:51:03.000000 development-tool-0.4.3/orangecontrib/development_tool/widgets/widget_designer/document_eater.ui
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-30 06:57:39.000000 development-tool-0.4.3/setup.cfg
+-rwx------   0 alex       (501) staff       (20)     1904 2024-04-30 06:57:15.000000 development-tool-0.4.3/setup.py
```

### Comparing `development-tool-0.4.2/development_tool.egg-info/SOURCES.txt` & `development-tool-0.4.3/development_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/Gpt4AllManagement.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/Gpt4AllManagement.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/MetManagement.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/MetManagement.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/VarManagement.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/VarManagement.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/WrapMessageBox.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/WrapMessageBox.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/document_eater.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/document_eater.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
                     self.progressBar.setValue(i + 1)
                     # Generate embeddings for the current row
                     embeddings.append(model.encode(str(row[selected_column_name])))
                 # Create new metas domains for embeddings
 
                 #embeddings = [model.encode(str(row["content"])) for row in data]
                 n_columns = len(embeddings[0])
-                new_metas_dom = [StringVariable("embedding" + f"_{selected_column_name}" + f"_{i}") for i in range(n_columns)]
+                new_metas_dom = [ContinuousVariable("embedding" + f"_{selected_column_name}" + f"_{i}") for i in range(n_columns)]
 
                 # Create the new updated Domain
                 domain = Domain(attr_dom, metas=metas_dom + new_metas_dom)
                 rows = []
 
                 n = len(data)
                 for i in range(n):
```

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/goto.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/goto.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Emblem_of_Napoleon_Bonaparte.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Emblem_of_Napoleon_Bonaparte.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Logo_HKH.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH_4.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Logo_HKH_4.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH_4_jc.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Logo_HKH_4_jc.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Napoleon2.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Napoleon2.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Pikachu SVG File.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Pikachu SVG File.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Workflow.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/Workflow.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/chat-bot.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/chat-bot.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/data-integration.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/data-integration.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/database.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/database.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/documents.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/documents.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/download-svgrepo-com.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/download-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/duplicate.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/duplicate.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/ecriture.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/ecriture.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/file-transfer.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/file-transfer.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/goto.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/goto.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/icon_surrogate_learner.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/icon_surrogate_learner.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/icon_surrogate_predict.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/icon_surrogate_predict.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/input.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/input.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/interrupteur.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/interrupteur.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_export_score.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/jcm_export_score.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_open_file_resize_alpha_channel.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/jcm_open_file_resize_alpha_channel.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_optuna_parameters_setting.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/jcm_optuna_parameters_setting.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_output_table.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/jcm_output_table.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/label.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/label.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/lecture.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/lecture.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/mywidget.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/mywidget.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/openai.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/openai.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/optuna.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/optuna.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/output.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/output.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tank-canon-svgrepo-com.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/tank-canon-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tool.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/tool.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tutoriel_bouton.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/tutoriel_bouton.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/variable_editor.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/variable_editor.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/war-svgrepo-com.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/icons/war-svgrepo-com.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/img/bandeau_pour_orange.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_18px.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_18px.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_30px.png` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_30px.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/interrupteur_ferme.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/img/interrupteur_ferme.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/interrupteur_ouvert.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/img/interrupteur_ouvert.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/khk_label_explanation.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/img/khk_label_explanation.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/img/refresh.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh2.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/img/refresh2.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh_with_txt.svg` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/img/refresh_with_txt.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/Table_management.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/Table_management.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/Utils_box.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/Utils_box.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis.tab` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis.tab`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis_permutation_tototo.tab` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis_permutation_tototo.tab`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/zoubida.dada` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/zoubida.dada`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/zoubida2.dada` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/kernel_function/zoubida2.dada`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/llm.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/llm.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/load_workflow.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/load_workflow.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/orange_sub_workflow.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/orange_sub_workflow.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example1.ows` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example1.ows`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example1.txt` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example1.txt`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example2.ows` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example2.ows`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example2.txt` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example2.txt`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example3.ows` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example3.ows`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example3.txt` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example3.txt`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example4.ows` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example4.ows`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example4.txt` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/ows_example/example4.txt`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/shared_functions.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/shared_functions.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/shared_variables.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/shared_variables.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/subworkflow_input.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/subworkflow_input.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/subworkflow_output.py` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/subworkflow_output.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/orangecontrib/development_tool/widgets/widget_designer/document_eater.ui` & `development-tool-0.4.3/orangecontrib/development_tool/widgets/widget_designer/document_eater.ui`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.2/setup.py` & `development-tool-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install development-tool')
 NAME = "development-tool"
 
 # Version du package PyPI
-VERSION = "0.4.2" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.4.3" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = "alex_hkh"
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "Library of developed widgets"
 LICENSE = ""
```

