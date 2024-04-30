# Comparing `tmp/lg_rez-4.0.5.tar.gz` & `tmp/lg_rez-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lg_rez-4.0.5.tar", last modified: Tue Apr 30 11:28:15 2024, max compression
+gzip compressed data, was "lg_rez-4.0.7.tar", last modified: Tue Apr 30 12:11:33 2024, max compression
```

## Comparing `lg_rez-4.0.5.tar` & `lg_rez-4.0.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:28:15.849809 lg_rez-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-30 11:28:08.000000 lg_rez-4.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-30 11:28:15.849809 lg_rez-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-30 11:28:08.000000 lg_rez-4.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:28:15.849809 lg_rez-4.0.5/lg_rez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-30 11:28:15.000000 lg_rez-4.0.5/lg_rez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-30 11:28:15.000000 lg_rez-4.0.5/lg_rez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:28:15.000000 lg_rez-4.0.5/lg_rez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-30 11:28:15.000000 lg_rez-4.0.5/lg_rez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 11:28:15.000000 lg_rez-4.0.5/lg_rez.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:28:15.845809 lg_rez-4.0.5/lgrez/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:28:15.845809 lg_rez-4.0.5/lgrez/bdd/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20725 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/bdd/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/bdd/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/bdd/model_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/bdd/model_ia.py
--rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/bdd/model_jeu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/bdd/model_joueurs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:28:15.845809 lg_rez-4.0.5/lgrez/blocs/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/blocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/blocs/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/blocs/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/blocs/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20325 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/blocs/journey.py
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/blocs/realshell.py
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/blocs/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    44961 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/blocs/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:28:15.849809 lg_rez-4.0.5/lgrez/features/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/actions_publiques.py
--rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/annexe.py
--rw-r--r--   0 runner    (1001) docker     (127)    18513 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/chans.py
--rw-r--r--   0 runner    (1001) docker     (127)    22570 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/gestion_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23562 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/gestion_ia.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/informations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/inscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    27484 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/open_close.py
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/special.py
--rw-r--r--   0 runner    (1001) docker     (127)    33108 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/taches.py
--rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/features/voter_agir.py
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-30 11:28:08.000000 lg_rez-4.0.5/lgrez/server_structure.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:28:15.849809 lg_rez-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-30 11:28:08.000000 lg_rez-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:33.263136 lg_rez-4.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-30 12:11:19.000000 lg_rez-4.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-30 12:11:33.263136 lg_rez-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-30 12:11:19.000000 lg_rez-4.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:33.263136 lg_rez-4.0.7/lg_rez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-30 12:11:33.000000 lg_rez-4.0.7/lg_rez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-30 12:11:33.000000 lg_rez-4.0.7/lg_rez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:11:33.000000 lg_rez-4.0.7/lg_rez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-30 12:11:33.000000 lg_rez-4.0.7/lg_rez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 12:11:33.000000 lg_rez-4.0.7/lg_rez.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:33.259135 lg_rez-4.0.7/lgrez/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:33.259135 lg_rez-4.0.7/lgrez/bdd/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20725 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/bdd/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/bdd/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/bdd/model_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/bdd/model_ia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/bdd/model_jeu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/bdd/model_joueurs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:33.263136 lg_rez-4.0.7/lgrez/blocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/blocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/blocs/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/blocs/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/blocs/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20325 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/blocs/journey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/blocs/realshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/blocs/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44961 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/blocs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:33.263136 lg_rez-4.0.7/lgrez/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/actions_publiques.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/annexe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18513 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/chans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22570 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/gestion_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23693 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/gestion_ia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/informations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/inscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27484 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/open_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33108 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/taches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/features/voter_agir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-30 12:11:19.000000 lg_rez-4.0.7/lgrez/server_structure.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:11:33.263136 lg_rez-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-30 12:11:19.000000 lg_rez-4.0.7/setup.py
```

### Comparing `lg_rez-4.0.5/LICENSE` & `lg_rez-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/PKG-INFO` & `lg_rez-4.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lg-rez
-Version: 4.0.5
+Version: 4.0.7
 Summary: Discord bot for organizing Werewolf RP games ESPCI-style
 Home-page: https://github.com/GRI-ESPCI/lg-rez
 Author: Loïc Simon, Tom Lacoma
 Author-email: loic.simon@espci.org, tom.lacoma@espci.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -89,20 +89,20 @@
 
 
 ## NOTE AUX GRIS / MJS
 
 Tout ce qui suit est du blabla READMEsque peu intéressant.
 
 Pour les trucs intéressants, c'est-à-dire les instructions pour lancer une 
-nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/Nouvelle%20saison.md).
+nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/Nouvelle%20saison.md).
 
 
 ## What's New in LG-Rez
 
-Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/CHANGELOG.md)
+Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/CHANGELOG.md)
 or in [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/changelog.html) for
 details.
 
 # 3.0
 
 * Changed all commands to Discord builtin slash commands, using Discordpy 2.0
 * Several major commands changes
@@ -144,28 +144,28 @@
 We strongly recommand to install this package in a dedicated virtualenv
 (`python3 -m venv <yourfolder>`).
 
 
 ### Dependencies
 
 * Python 3.10+
-* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/requirements.txt)
+* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/requirements.txt)
 
 
 
 ## Configuration
 
 To run correctly, the bot needs to be connected to several external services,
 each needing more or less sensitive tokens, stocked as environments variables.
 We support and encourage the use of
 [`python-dotenv`](https://pypi.org/project/python-dotenv/) to read them from
 a `.env` file, but you may prefer exporting them as environment variables.
 
 All necessary variables, prefixed by `LGREZ_`, are listed in
-[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/model.env).
+[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/model.env).
 
 
 ### Configuration Assistant Tool
 
 We provide a command-line assistant tool to help you set up every services and
 generate the `.env` file (which you can later `source` and delete if you wish).
 
@@ -178,15 +178,15 @@
 needed to run the bot (see *Usage* section below).
 
 
 ### Manual configuration
 
 You may prefer to manually write your environment variables, or just check
 instructions regarding a specific one: they can be found in
-[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/CONFIGURE.md).
+[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/CONFIGURE.md).
 
 **Warning**: the Configuration Assistant Tool checks every variable by
 running specific tests, which is not the case for manual configuration,
 so be sure of what you do!
 
 
 
@@ -221,15 +221,15 @@
 
 Since `LGBot` is a subclass of
 [`discord.ext.commands.Bot`](https://discordpy.readthedocs.io/en/latest/ext/commands/api.html#bot),
 you can use every arguments and methods it supports or subclass it to override
 existing behavior.
 
 We also provide a direct way to customize some parameters of the game and
-of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/lgrez/config.py) module:
+of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/lgrez/config.py) module:
 roles/channels/emoji names, date of season beginning, inscription
 customization... See
 [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/config.html)
 for full API usage information.
 
 See additional attributes and overriden methods on
 [the doc](https://lg-rez.readthedocs.io/) (mostly in French)
@@ -306,15 +306,15 @@
 
 Community contributions are not welcome for now. Get in touch with the authors
 (see below) for any question or suggestion about this project.
 
 
 
 ## License
-This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/LICENSE).
+This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/LICENSE).
 
 © 2020 - 2022 Loïc Simon, Tom Lacoma et al. – Club BD-Jeux × GRIs –
 ESPCI Paris - PSL
 
 Reach us on Discord:
 [LaCarpe#1674](https://discordapp.com/users/264482202966818825),
 [TaupeOrAfk#3218](https://discordapp.com/users/176763552202358785) or by mail: [loic.simon@espci.org](mailto:loic.simon@espci.org),
```

### Comparing `lg_rez-4.0.5/README.md` & `lg_rez-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lg_rez.egg-info/PKG-INFO` & `lg_rez-4.0.7/lg_rez.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lg-rez
-Version: 4.0.5
+Version: 4.0.7
 Summary: Discord bot for organizing Werewolf RP games ESPCI-style
 Home-page: https://github.com/GRI-ESPCI/lg-rez
 Author: Loïc Simon, Tom Lacoma
 Author-email: loic.simon@espci.org, tom.lacoma@espci.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -89,20 +89,20 @@
 
 
 ## NOTE AUX GRIS / MJS
 
 Tout ce qui suit est du blabla READMEsque peu intéressant.
 
 Pour les trucs intéressants, c'est-à-dire les instructions pour lancer une 
-nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/Nouvelle%20saison.md).
+nouvelle saison, voir [`Nouvelle saison.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/Nouvelle%20saison.md).
 
 
 ## What's New in LG-Rez
 
-Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/CHANGELOG.md)
+Only major features are reported here; see [`CHANGELOG.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/CHANGELOG.md)
 or in [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/changelog.html) for
 details.
 
 # 3.0
 
 * Changed all commands to Discord builtin slash commands, using Discordpy 2.0
 * Several major commands changes
@@ -144,28 +144,28 @@
 We strongly recommand to install this package in a dedicated virtualenv
 (`python3 -m venv <yourfolder>`).
 
 
 ### Dependencies
 
 * Python 3.10+
-* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/requirements.txt)
+* Packages: see [`requirements.txt`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/requirements.txt)
 
 
 
 ## Configuration
 
 To run correctly, the bot needs to be connected to several external services,
 each needing more or less sensitive tokens, stocked as environments variables.
 We support and encourage the use of
 [`python-dotenv`](https://pypi.org/project/python-dotenv/) to read them from
 a `.env` file, but you may prefer exporting them as environment variables.
 
 All necessary variables, prefixed by `LGREZ_`, are listed in
-[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/model.env).
+[`model.env`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/model.env).
 
 
 ### Configuration Assistant Tool
 
 We provide a command-line assistant tool to help you set up every services and
 generate the `.env` file (which you can later `source` and delete if you wish).
 
@@ -178,15 +178,15 @@
 needed to run the bot (see *Usage* section below).
 
 
 ### Manual configuration
 
 You may prefer to manually write your environment variables, or just check
 instructions regarding a specific one: they can be found in
-[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/CONFIGURE.md).
+[`CONFIGURE.md`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/CONFIGURE.md).
 
 **Warning**: the Configuration Assistant Tool checks every variable by
 running specific tests, which is not the case for manual configuration,
 so be sure of what you do!
 
 
 
@@ -221,15 +221,15 @@
 
 Since `LGBot` is a subclass of
 [`discord.ext.commands.Bot`](https://discordpy.readthedocs.io/en/latest/ext/commands/api.html#bot),
 you can use every arguments and methods it supports or subclass it to override
 existing behavior.
 
 We also provide a direct way to customize some parameters of the game and
-of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/lgrez/config.py) module:
+of the Discord server through [`config`](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/lgrez/config.py) module:
 roles/channels/emoji names, date of season beginning, inscription
 customization... See
 [the doc](https://lg-rez.readthedocs.io/fr/2.4.2/config.html)
 for full API usage information.
 
 See additional attributes and overriden methods on
 [the doc](https://lg-rez.readthedocs.io/) (mostly in French)
@@ -306,15 +306,15 @@
 
 Community contributions are not welcome for now. Get in touch with the authors
 (see below) for any question or suggestion about this project.
 
 
 
 ## License
-This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.5/LICENSE).
+This work is shared under [the MIT license](https://github.com/GRI-ESPCI/lg-rez/blob/4.0.7/LICENSE).
 
 © 2020 - 2022 Loïc Simon, Tom Lacoma et al. – Club BD-Jeux × GRIs –
 ESPCI Paris - PSL
 
 Reach us on Discord:
 [LaCarpe#1674](https://discordapp.com/users/264482202966818825),
 [TaupeOrAfk#3218](https://discordapp.com/users/176763552202358785) or by mail: [loic.simon@espci.org](mailto:loic.simon@espci.org),
```

### Comparing `lg_rez-4.0.5/lg_rez.egg-info/SOURCES.txt` & `lg_rez-4.0.7/lg_rez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lg_rez.egg-info/requires.txt` & `lg_rez-4.0.7/lg_rez.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/__main__.py` & `lg_rez-4.0.7/lgrez/__main__.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/bdd/__init__.py` & `lg_rez-4.0.7/lgrez/bdd/__init__.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/bdd/base.py` & `lg_rez-4.0.7/lgrez/bdd/base.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/bdd/enums.py` & `lg_rez-4.0.7/lgrez/bdd/enums.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/bdd/model_actions.py` & `lg_rez-4.0.7/lgrez/bdd/model_actions.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/bdd/model_ia.py` & `lg_rez-4.0.7/lgrez/bdd/model_ia.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/bdd/model_jeu.py` & `lg_rez-4.0.7/lgrez/bdd/model_jeu.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/bdd/model_joueurs.py` & `lg_rez-4.0.7/lgrez/bdd/model_joueurs.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/blocs/__init__.py` & `lg_rez-4.0.7/lgrez/blocs/__init__.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/blocs/console.py` & `lg_rez-4.0.7/lgrez/blocs/console.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/blocs/env.py` & `lg_rez-4.0.7/lgrez/blocs/env.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/blocs/gsheets.py` & `lg_rez-4.0.7/lgrez/blocs/gsheets.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/blocs/journey.py` & `lg_rez-4.0.7/lgrez/blocs/journey.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/blocs/realshell.py` & `lg_rez-4.0.7/lgrez/blocs/realshell.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/blocs/structure.py` & `lg_rez-4.0.7/lgrez/blocs/structure.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/blocs/tools.py` & `lg_rez-4.0.7/lgrez/blocs/tools.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/bot.py` & `lg_rez-4.0.7/lgrez/bot.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/commands.py` & `lg_rez-4.0.7/lgrez/commands.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/config.py` & `lg_rez-4.0.7/lgrez/config.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/__init__.py` & `lg_rez-4.0.7/lgrez/features/__init__.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/actions_publiques.py` & `lg_rez-4.0.7/lgrez/features/actions_publiques.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/annexe.py` & `lg_rez-4.0.7/lgrez/features/annexe.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/chans.py` & `lg_rez-4.0.7/lgrez/features/chans.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/communication.py` & `lg_rez-4.0.7/lgrez/features/communication.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/gestion_actions.py` & `lg_rez-4.0.7/lgrez/features/gestion_actions.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/gestion_ia.py` & `lg_rez-4.0.7/lgrez/features/gestion_ia.py`

 * *Files 1% similar despite different names*

```diff
@@ -628,14 +628,17 @@
 async def process_ia(message: discord.Message, send_callable: Callable[[str], Coroutine], debug: bool = False) -> None:
     """Exécute les règles d'IA.
 
     Args:
         message: Message auquel réagir.
         debug: Si ``True``, affiche les erreurs lors de l'évaluation des messages (voir :func:`.tools.eval_accols`).
     """
+    if message.type != discord.MessageType.default:  # Vérifie si le message n'est pas un message système
+        return
+    
     (
         await trigger_at_mj(message, send_callable)  # @MJ (aled)
         or await trigger_gif(message, send_callable)  # Un petit GIF ? (si FALS)
         or await trigger_roles(message, send_callable)  # Rôles
         or await trigger_reactions(message, send_callable, debug=debug)  # Table Reaction ("IA")
         or await trigger_sub_reactions(message, send_callable, debug=debug)  # IA sur les mots
         or await trigger_a_ou_b(message, send_callable)  # "a ou b" ==> "b"
```

### Comparing `lg_rez-4.0.5/lgrez/features/informations.py` & `lg_rez-4.0.7/lgrez/features/informations.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/inscription.py` & `lg_rez-4.0.7/lgrez/features/inscription.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/open_close.py` & `lg_rez-4.0.7/lgrez/features/open_close.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/special.py` & `lg_rez-4.0.7/lgrez/features/special.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/sync.py` & `lg_rez-4.0.7/lgrez/features/sync.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/taches.py` & `lg_rez-4.0.7/lgrez/features/taches.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/features/voter_agir.py` & `lg_rez-4.0.7/lgrez/features/voter_agir.py`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/lgrez/server_structure.json` & `lg_rez-4.0.7/lgrez/server_structure.json`

 * *Files identical despite different names*

### Comparing `lg_rez-4.0.5/setup.py` & `lg_rez-4.0.7/setup.py`

 * *Files identical despite different names*

