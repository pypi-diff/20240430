# Comparing `tmp/sphinx-nefertiti-0.3.2.tar.gz` & `tmp/sphinx_nefertiti-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-nefertiti-0.3.2.tar", last modified: Wed Mar 13 18:50:24 2024, max compression
+gzip compressed data, was "sphinx_nefertiti-0.3.3.tar", last modified: Tue Apr 30 13:40:18 2024, max compression
```

## Comparing `sphinx-nefertiti-0.3.2.tar` & `sphinx_nefertiti-0.3.3.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.091966 sphinx-nefertiti-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-03-13 18:50:24.091966 sphinx-nefertiti-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 18:50:24.091966 sphinx-nefertiti-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.059966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/breadcrumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.067966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/
--rw-r--r--   0 runner    (1001) docker     (127)   250921 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-blue.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    92420 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-blue.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   250905 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-default.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    92419 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-default.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   250900 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-green.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    92420 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-green.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   250925 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-indigo.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    92422 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-indigo.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   250903 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-orange.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    92421 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-orange.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   250925 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-pink.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    92420 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-pink.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   250927 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-purple.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    92422 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-purple.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   250907 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-red.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    92418 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-red.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   250901 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-teal.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    92419 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-teal.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   250888 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-yellow.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    92421 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-yellow.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets-dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/docsver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/extensions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.051966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.067966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/
--rwxr-xr-x   0 runner    (1001) docker     (127)    49304 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/Assistant-Bold.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)    49348 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/Assistant-Regular.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)    79660 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/Assistant-VariableFont_wght.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)     4708 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.071966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/
--rw-r--r--   0 runner    (1001) docker     (127)    90812 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/Exo-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    90988 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/Exo-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   145512 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/Exo-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.071966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/
--rwxr-xr-x   0 runner    (1001) docker     (127)   165196 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/FiraCode-Bold.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)   164712 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/FiraCode-Regular.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)   223136 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/FiraCode-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.075966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/
--rw-r--r--   0 runner    (1001) docker     (127)   198072 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/Montserrat-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   197976 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/Montserrat-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   394140 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/Montserrat-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.075966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/
--rw-r--r--   0 runner    (1001) docker     (127)   105904 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/Mulish-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   105860 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/Mulish-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   210380 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/Mulish-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.079966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/
--rw-r--r--   0 runner    (1001) docker     (127)   131672 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/Nunito-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   131736 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/Nunito-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   275644 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/Nunito-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.079966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)   129784 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/OpenSans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   129796 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/OpenSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/OpenSans-VariableFont_wdth,wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.079966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)    47320 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    47356 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    94800 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.083966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)    31548 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    31652 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    66064 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.083966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)   160304 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   160212 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   340612 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.083966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu/
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu/UFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)   270164 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu/Ubuntu-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   299684 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu/Ubuntu-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.087966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu-mono/
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu-mono/UFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)   174860 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu-mono/UbuntuMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   189892 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu-mono/UbuntuMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu-mono/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.087966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)    70356 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/Varta-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    70496 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/Varta-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   108608 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/Varta-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.087966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)   192304 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/WorkSans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   191916 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/WorkSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   359628 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/WorkSans-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-03-13 18:49:58.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/genindex-single.html
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/genindex-split.html
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/lightdark-dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/pager.html
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/pygments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/searchresults.html
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/sitemap.html
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/source-buttons.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.091966 sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/
--rw-r--r--   0 runner    (1001) docker     (127)    88494 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)   112440 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    45922 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/pygments.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/pygments.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/pygments_dark.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/pygments_dark.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    24130 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/sphinx-nefertiti.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    42093 2024-03-13 18:50:21.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/sphinx-nefertiti.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/theme.conf
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-03-13 18:49:59.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti/version-dropdown.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:50:24.091966 sphinx-nefertiti-0.3.2/sphinx_nefertiti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-03-13 18:50:24.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-03-13 18:50:24.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 18:50:24.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-13 18:50:24.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-13 18:50:24.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-13 18:50:24.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 18:50:24.000000 sphinx-nefertiti-0.3.2/sphinx_nefertiti.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:18.010648 sphinx_nefertiti-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-30 13:40:18.010648 sphinx_nefertiti-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:40:18.010648 sphinx_nefertiti-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:17.982648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/breadcrumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:17.990648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/
+-rw-r--r--   0 runner    (1001) docker     (127)   250921 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-blue.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    92420 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-blue.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   250905 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-default.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    92419 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-default.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   250900 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-green.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    92420 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-green.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   250925 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-indigo.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    92422 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-indigo.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   250903 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-orange.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    92421 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-orange.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   250925 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-pink.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    92420 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-pink.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   250927 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-purple.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    92422 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-purple.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   250907 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-red.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    92418 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-red.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   250901 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-teal.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    92419 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-teal.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   250888 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-yellow.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    92421 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-yellow.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets-dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/docsver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/extensions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:17.974648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:17.990648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49304 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/Assistant-Bold.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49348 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/Assistant-Regular.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    79660 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/Assistant-VariableFont_wght.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4708 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:17.990648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/
+-rw-r--r--   0 runner    (1001) docker     (127)    90812 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/Exo-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    90988 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/Exo-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   145512 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/Exo-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:17.994648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   165196 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/FiraCode-Bold.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   164712 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/FiraCode-Regular.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   223136 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/FiraCode-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:17.994648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/
+-rw-r--r--   0 runner    (1001) docker     (127)   198072 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/Montserrat-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   197976 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/Montserrat-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   394140 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/Montserrat-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:17.998648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/
+-rw-r--r--   0 runner    (1001) docker     (127)   105904 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/Mulish-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   105860 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/Mulish-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   210380 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/Mulish-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:17.998648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/
+-rw-r--r--   0 runner    (1001) docker     (127)   131672 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/Nunito-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   131736 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/Nunito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   275644 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/Nunito-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:17.998648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   129784 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/OpenSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   129796 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/OpenSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/OpenSans-VariableFont_wdth,wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:18.002648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    47320 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    47356 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    94800 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:18.002648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31548 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    31652 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    66064 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:18.002648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   160304 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   160212 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   340612 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:18.006648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu/UFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   270164 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu/Ubuntu-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   299684 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu/Ubuntu-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:18.006648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu-mono/
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu-mono/UFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174860 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu-mono/UbuntuMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   189892 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu-mono/UbuntuMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu-mono/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:18.006648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    70356 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/Varta-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    70496 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/Varta-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   108608 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/Varta-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:18.010648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   192304 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/WorkSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   191916 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/WorkSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   359628 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/WorkSans-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/genindex-single.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/genindex-split.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/lightdark-dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/pager.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/pygments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/searchresults.html
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/sitemap.html
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/source-buttons.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:18.010648 sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    88494 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)   112440 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    45922 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/pygments.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/pygments.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/pygments_dark.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/pygments_dark.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    24130 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/sphinx-nefertiti.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    42093 2024-04-30 13:40:15.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/sphinx-nefertiti.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-30 13:39:41.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti/version-dropdown.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:40:18.010648 sphinx_nefertiti-0.3.3/sphinx_nefertiti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-30 13:40:17.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-30 13:40:17.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:40:17.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 13:40:17.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 13:40:17.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 13:40:17.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:40:17.000000 sphinx_nefertiti-0.3.3/sphinx_nefertiti.egg-info/zip-safe
```

### Comparing `sphinx-nefertiti-0.3.2/LICENSE.txt` & `sphinx_nefertiti-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/PKG-INFO` & `sphinx_nefertiti-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-nefertiti
-Version: 0.3.2
+Version: 0.3.3
 Summary: The Nefertiti for Sphinx theme.
 Home-page: https://github.com/danirus/sphinx-nefertiti
 Author: Daniela Rus Morales
 Author-email: danirus@eml.cc
 Maintainer: Daniela Rus Morales
 Maintainer-email: danirus@eml.cc
 License: MIT
```

### Comparing `sphinx-nefertiti-0.3.2/README.md` & `sphinx_nefertiti-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/setup.py` & `sphinx_nefertiti-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open(BASE_DIR / "requirements.txt", "r") as req_file:
     for item in req_file:
         requirements.append(item)
 
 
 setup(
     name="sphinx-nefertiti",
-    version="0.3.2",
+    version="0.3.3",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description="The Nefertiti for Sphinx theme.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Daniela Rus Morales",
```

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/__init__.py` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-blue.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-blue.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-blue.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-blue.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-default.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-default.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-default.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-default.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-green.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-green.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-green.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-green.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-indigo.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-indigo.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-indigo.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-indigo.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-orange.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-orange.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-orange.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-orange.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-pink.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-pink.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-pink.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-pink.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-purple.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-purple.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-purple.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-purple.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-red.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-red.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-red.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-red.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-teal.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-teal.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-teal.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-teal.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-yellow.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-yellow.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets/sphinx-nefertiti-yellow.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets/sphinx-nefertiti-yellow.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets-dropdown.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets-dropdown.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/colorsets.py` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/colorsets.py`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/docsver.py` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/docsver.py`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/domainindex.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/domainindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/extensions.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/extensions.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/Assistant-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/Assistant-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/Assistant-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/Assistant-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/Assistant-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/Assistant-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/assistant/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/assistant/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/Exo-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/Exo-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/Exo-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/Exo-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/Exo-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/Exo-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/exo/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/exo/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/FiraCode-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/FiraCode-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/FiraCode-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/FiraCode-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/FiraCode-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/FiraCode-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/fira-code/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/fira-code/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/Montserrat-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/Montserrat-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/Montserrat-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/Montserrat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/Montserrat-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/Montserrat-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/montserrat/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/montserrat/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/Mulish-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/Mulish-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/Mulish-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/Mulish-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/Mulish-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/Mulish-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/mulish/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/mulish/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/Nunito-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/Nunito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/Nunito-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/Nunito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/Nunito-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/Nunito-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/nunito/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/nunito/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/OpenSans-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/OpenSans-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/OpenSans-VariableFont_wdth,wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/OpenSans-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/open-sans/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/open-sans/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/RedHatDisplay-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-display/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-display/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/RedHatMono-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/red-hat-mono/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/red-hat-mono/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/SofiaSans-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/sofia-sans/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/sofia-sans/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu/UFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu/UFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu/Ubuntu-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu/Ubuntu-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu/Ubuntu-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu/Ubuntu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu-mono/UFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu-mono/UFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu-mono/UbuntuMono-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu-mono/UbuntuMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/ubuntu-mono/UbuntuMono-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/ubuntu-mono/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/Varta-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/Varta-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/Varta-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/Varta-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/Varta-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/Varta-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/varta/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/varta/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/OFL.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/WorkSans-Bold.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/WorkSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/WorkSans-Regular.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/WorkSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/WorkSans-VariableFont_wght.ttf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/WorkSans-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts/work-sans/stylesheet.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts/work-sans/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/fonts.py` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/fonts.py`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/footer.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/footer.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/genindex-single.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/genindex-single.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/genindex-split.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/genindex-split.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/genindex.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/globaltoc.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/globaltoc.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/layout.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/lightdark-dropdown.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/lightdark-dropdown.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/pager.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/pager.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/pygments.py` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/pygments.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,32 +60,33 @@
 # applying CSS classes that override the preferred color scheme.
 #
 # This Python class wraps the styles with those CSS classes.
 
 
 class PygmentsProvider:
     def __init__(self, app):
-        config = app.builder.theme.config
         theme_defaults = app.builder.theme.get_options()
         theme_user_prefs = app.config.html_theme_options
 
         self._index = -1
         self._assets = []
 
         for opt, filename, css in pygments_options:
+            asset = None
+
             if opt in theme_user_prefs and len(theme_user_prefs[opt]):
                 asset = PygmentsAsset(theme_user_prefs[opt], filename, css)
             elif opt in theme_defaults and len(theme_defaults[opt]):
                 asset = PygmentsAsset(theme_defaults[opt], filename, css)
             elif getattr(app.config, opt, False):
                 style_name = getattr(app.config, opt)
                 asset = PygmentsAsset(style_name, filename, css)
-            else:
-                asset = PygmentsAsset(config.get("theme", opt), filename, css)
-            self._assets.append(asset)
+
+            if asset:
+                self._assets.append(asset)
 
     def __iter__(self):
         return self
 
     def __next__(self):
         self._index += 1
         if self._index >= len(self._assets):
```

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/search.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/search.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/searchbox.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/searchresults.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/searchresults.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/source-buttons.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/source-buttons.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/bootstrap-icons.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/bootstrap-icons.woff2` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/bootstrap.bundle.min.js` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/pygments.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/pygments.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/pygments.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/pygments.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/pygments_dark.min.css` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/pygments_dark.min.css`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/pygments_dark.min.css.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/pygments_dark.min.css.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/sphinx-nefertiti.min.js` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/sphinx-nefertiti.min.js`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/static/sphinx-nefertiti.min.js.map` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/static/sphinx-nefertiti.min.js.map`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/theme.conf` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/theme.conf`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti/version-dropdown.html` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti/version-dropdown.html`

 * *Files identical despite different names*

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti.egg-info/PKG-INFO` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-nefertiti
-Version: 0.3.2
+Version: 0.3.3
 Summary: The Nefertiti for Sphinx theme.
 Home-page: https://github.com/danirus/sphinx-nefertiti
 Author: Daniela Rus Morales
 Author-email: danirus@eml.cc
 Maintainer: Daniela Rus Morales
 Maintainer-email: danirus@eml.cc
 License: MIT
```

### Comparing `sphinx-nefertiti-0.3.2/sphinx_nefertiti.egg-info/SOURCES.txt` & `sphinx_nefertiti-0.3.3/sphinx_nefertiti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

