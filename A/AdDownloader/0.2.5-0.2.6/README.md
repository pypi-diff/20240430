# Comparing `tmp/AdDownloader-0.2.5.tar.gz` & `tmp/AdDownloader-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addownloader-0.2.5.tar", last modified: Thu Apr 18 14:57:22 2024, max compression
+gzip compressed data, was "addownloader-0.2.6.tar", last modified: Tue Apr 30 14:27:13 2024, max compression
```

## Comparing `AdDownloader-0.2.5.tar` & `AdDownloader-0.2.6.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 14:57:22.211634 addownloader-0.2.5/
-drwxrwxrwx   0        0        0        0 2024-04-18 14:57:21.844635 addownloader-0.2.5/AdDownloader/
--rw-rw-rw-   0        0        0      266 2024-04-09 13:11:46.000000 addownloader-0.2.5/AdDownloader/__init__.py
--rw-rw-rw-   0        0        0      206 2024-02-08 14:42:41.000000 addownloader-0.2.5/AdDownloader/__main__.py
--rw-rw-rw-   0        0        0    11559 2024-04-18 14:06:40.000000 addownloader-0.2.5/AdDownloader/adlib_api.py
--rw-rw-rw-   0        0        0    34045 2024-04-18 14:15:06.000000 addownloader-0.2.5/AdDownloader/analysis.py
--rw-rw-rw-   0        0        0    33323 2024-04-18 14:17:56.000000 addownloader-0.2.5/AdDownloader/app.py
--rw-rw-rw-   0        0        0    11529 2024-04-18 14:48:18.000000 addownloader-0.2.5/AdDownloader/cli.py
--rw-rw-rw-   0        0        0    17852 2024-04-18 14:13:34.000000 addownloader-0.2.5/AdDownloader/helpers.py
--rw-rw-rw-   0        0        0    12007 2024-04-18 13:12:59.000000 addownloader-0.2.5/AdDownloader/media_download.py
--rw-rw-rw-   0        0        0      117 2024-04-02 13:27:27.000000 addownloader-0.2.5/AdDownloader/start_app.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:57:22.152750 addownloader-0.2.5/AdDownloader.egg-info/
--rw-rw-rw-   0        0        0    52812 2024-04-18 14:57:21.000000 addownloader-0.2.5/AdDownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2024-04-18 14:57:21.000000 addownloader-0.2.5/AdDownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 14:57:21.000000 addownloader-0.2.5/AdDownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-18 14:57:21.000000 addownloader-0.2.5/AdDownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      439 2024-04-18 14:57:21.000000 addownloader-0.2.5/AdDownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 14:57:21.000000 addownloader-0.2.5/AdDownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2024-01-17 12:27:17.000000 addownloader-0.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0    52812 2024-04-18 14:57:22.198135 addownloader-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     9675 2024-04-18 14:55:45.000000 addownloader-0.2.5/README.md
--rw-rw-rw-   0        0        0     2425 2024-04-17 11:51:07.000000 addownloader-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 14:57:22.232036 addownloader-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 14:57:22.104450 addownloader-0.2.5/tests/
--rw-rw-rw-   0        0        0    14386 2024-04-11 15:41:42.000000 addownloader-0.2.5/tests/test_AdDownloader.py
--rw-rw-rw-   0        0        0      218 2024-04-18 14:17:58.000000 addownloader-0.2.5/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:27:12.910694 addownloader-0.2.6/
+drwxrwxrwx   0        0        0        0 2024-04-30 14:27:12.250749 addownloader-0.2.6/AdDownloader/
+-rw-rw-rw-   0        0        0      258 2024-04-29 12:50:04.000000 addownloader-0.2.6/AdDownloader/__init__.py
+-rw-rw-rw-   0        0        0      206 2024-02-08 14:42:41.000000 addownloader-0.2.6/AdDownloader/__main__.py
+-rw-rw-rw-   0        0        0    11596 2024-04-29 15:58:10.000000 addownloader-0.2.6/AdDownloader/adlib_api.py
+-rw-rw-rw-   0        0        0    33936 2024-04-29 12:52:45.000000 addownloader-0.2.6/AdDownloader/analysis.py
+-rw-rw-rw-   0        0        0    33356 2024-04-29 12:52:18.000000 addownloader-0.2.6/AdDownloader/app.py
+-rw-rw-rw-   0        0        0    10098 2024-04-30 14:10:53.000000 addownloader-0.2.6/AdDownloader/cli.py
+-rw-rw-rw-   0        0        0    17686 2024-04-30 14:10:40.000000 addownloader-0.2.6/AdDownloader/helpers.py
+-rw-rw-rw-   0        0        0    12007 2024-04-18 13:12:59.000000 addownloader-0.2.6/AdDownloader/media_download.py
+-rw-rw-rw-   0        0        0      117 2024-04-02 13:27:27.000000 addownloader-0.2.6/AdDownloader/start_app.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:27:12.792375 addownloader-0.2.6/AdDownloader.egg-info/
+-rw-rw-rw-   0        0        0    52886 2024-04-30 14:27:11.000000 addownloader-0.2.6/AdDownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2024-04-30 14:27:11.000000 addownloader-0.2.6/AdDownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 14:27:11.000000 addownloader-0.2.6/AdDownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-30 14:27:11.000000 addownloader-0.2.6/AdDownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      415 2024-04-30 14:27:11.000000 addownloader-0.2.6/AdDownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 14:27:11.000000 addownloader-0.2.6/AdDownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2024-01-17 12:27:17.000000 addownloader-0.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0    52886 2024-04-30 14:27:12.871990 addownloader-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9687 2024-04-30 14:19:39.000000 addownloader-0.2.6/README.md
+-rw-rw-rw-   0        0        0     2479 2024-04-30 14:13:50.000000 addownloader-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 14:27:12.957578 addownloader-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 14:27:12.655772 addownloader-0.2.6/tests/
+-rw-rw-rw-   0        0        0    14865 2024-04-24 12:57:06.000000 addownloader-0.2.6/tests/test_AdDownloader.py
```

### Comparing `addownloader-0.2.5/AdDownloader/adlib_api.py` & `addownloader-0.2.6/AdDownloader/adlib_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module provides the call to the Meta Ad Library API for ad data retrieval."""
 
 import pandas as pd
+from collections.abc import Mapping
 import requests
 import os
 
 from datetime import datetime
 from AdDownloader.helpers import *
 
 class AdLibAPI:
```

### Comparing `addownloader-0.2.5/AdDownloader/analysis.py` & `addownloader-0.2.6/AdDownloader/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,44 +9,39 @@
 from collections import Counter
 from nltk.tokenize import word_tokenize
 from nltk.corpus import stopwords
 from nltk.sentiment import SentimentIntensityAnalyzer
 from nltk.stem import WordNetLemmatizer, SnowballStemmer
 from nltk import FreqDist
 import nltk
-#import spacy # use to lemmatize other languages than english
 import gensim.corpora as corpora
 from gensim.models.ldamodel import LdaModel
 from gensim.models.coherencemodel import CoherenceModel
 from wordcloud import WordCloud
 from textblob import TextBlob
 from gensim.parsing.preprocessing import remove_stopwords
 import plotly.express as px
 from PIL import Image
 from sklearn.cluster import KMeans
 from skimage import color as sk_color
 from skimage.feature import canny, corner_harris, corner_peaks
 import cv2
 from transformers import BlipProcessor, BlipForConditionalGeneration, BlipForQuestionAnswering
 
-# add to the dependencies: spacy==3.7.4
-
-#nltk.download('omw-1.4')
-
+#nltk.download('omw-1.4')s
 
 DATE_MIN = 'ad_delivery_start_time'
 DATE_MAX = 'ad_delivery_stop_time'
 
 GENDERS = ['female', 'male', 'unknown']
 AGE_RANGES = ['13-17', '18-24', '25-34', '35-44', '45-54', '55-64', '65+']
 
 AD_PATTERN = re.compile(r"ad_([0-9]+)_(img|frame[0-9]+)\.(png|jpeg|jpg)")
 
 
-
 def load_data(data_path):
     """
     Load ads data from an Excel file into a dataframe given a valid path.
 
     :param data_path: A valid path to an Excel file containing ad data.
     :type data_path: str
     :returns: A dataframe containing ads data and an additional campaign duration column.
```

### Comparing `addownloader-0.2.5/AdDownloader/app.py` & `addownloader-0.2.6/AdDownloader/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+"""This module provides the AdDownloader Analytics Dashboard."""
+
 import base64
 import io
 import os
 from dash import Dash, dcc, html, callback, Input, Output, State, dash_table, no_update
-from matplotlib.pyplot import sca
 import plotly.express as px
 import pandas as pd
 from AdDownloader import analysis
 from AdDownloader.helpers import update_access_token
 from AdDownloader.media_download import start_media_download
```

### Comparing `addownloader-0.2.5/AdDownloader/cli.py` & `addownloader-0.2.6/AdDownloader/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,89 @@
 """This module provides the AdDownloader Command-line Interface."""
-"""
-Created on January 11, 2024
 
-@author: Paula G
-"""
 ########
-
 # to build new distributions (new versions), in the cmd inside the venv run 'python -m build'
-# then, to upload the dist archives to TestPyPi, run 'python -m twine upload --repository testpypi dist/*'
 # to upload to PyPi, run 'python -m twine upload dist/AdDownloader-0.2.5-py3-none-any.whl'
 # to install the package, inside the directory with venv run: 'python -m pip install AdDownloader'
 ########
 
 import typer
-from PyInquirer import prompt, style_from_dict, Token
+import inquirer3 
+from inquirer3.themes import load_theme_from_dict
 from rich import print as rprint
+import time
+import pandas as pd
 
 from AdDownloader.adlib_api import *
 from AdDownloader.media_download import *
 from AdDownloader.helpers import NumberValidator, DateValidator, CountryValidator, ExcelValidator, update_access_token
-import time
-import pandas as pd
 
-# global style for the cmd
-default_style = style_from_dict({
-    Token.QuestionMark: '#E91E63 bold',
-    Token.Selected: '#673AB7 bold',
-    Token.Instruction: '',  # default
-    Token.Answer: '#2196f3 bold',
-    Token.Question: '#FFD700 bold',
-})
+default_style = load_theme_from_dict(
+    {
+        "Question": {
+            "mark_color": "bold_firebrick3",
+            "brackets_color": "mediumpurple",
+            "default_color": "bold_blue"
+        },
+        "List": {
+            "selection_color": "bold_dodgerblue3_on_goldenrod1",
+            "selection_cursor": "➤",
+            "unselected_color": "dodgerblue2"
+        }
+    }
+)
 
 
 def request_params_task_AC():
     """
     Prompt user for additional parameters for the API request in tasks A and C that involve ad data download from the Meta Ad Library.
 
     :returns: User-provided parameters.
     :rtype: dict
     """
     add_questions = [
-        {
-            'type': 'list',
-            'name': 'ad_type',
-            'message': 'What type of ads do you want to search?',
-            'choices': ['All', 'Political/Elections']
-        },
-        {
-            'type': 'input',
-            'name': 'ad_reached_countries',
-            'message': 'What reached countries do you want? (Provide the code, default is "NL")',
-            'validate': CountryValidator
-        },
-        {
-            'type': 'input',
-            'name': 'ad_delivery_date_min',
-            'message': 'What is the minimum ad delivery date you want? (default is "2023-01-01")',
-            'validate': DateValidator
-        },
-        {
-            'type': 'input',
-            'name': 'ad_delivery_date_max',
-            'message': 'What is the maximum ad delivery date you want? (default is today\'s date)',
-            'validate': DateValidator
-        },
-        {
-            'type': 'list',
-            'name': 'search_by',
-            'message': 'Do you want to search by pages ID or by search terms?',
-            'choices': ['Pages ID', 'Search Terms']
-        },
-        {
-            'type': 'input',
-            'name': 'pages_id_path',
-            'message': 'Please provide the name of your Excel file with pages ID (needs to be inside the data folder)',
-            'when': lambda answers: answers['search_by'] == 'Pages ID',
-            'validate': ExcelValidator
-        },
-        {
-            'type': 'input',
-            'name': 'search_terms',
-            'message': 'Please provide one or more search terms, separated by a comma',
-            'when': lambda answers: answers['search_by'] == 'Search Terms'
-        }
+        inquirer3.List(
+            "ad_type", 
+            message="What type of ads do you want to search?", 
+            choices=['All', 'Political/Elections'],
+        ),
+        inquirer3.Text(
+            "ad_reached_countries",
+            message="What reached countries do you want? (Provide the code, default is 'NL')",
+            validate=CountryValidator.validate_country,
+        ),
+        inquirer3.Text(
+            "ad_delivery_date_min",
+            message="What is the minimum ad delivery date you want? (default is '2023-01-01')",
+            validate=DateValidator.validate_date,
+        ),
+        inquirer3.Text(
+            "ad_delivery_date_max",
+            message="What is the maximum ad delivery date you want? (default is today\'s date)",
+            validate=DateValidator.validate_date,
+        ),
+        inquirer3.List(
+            "search_by", 
+            message="Do you want to search by pages ID or by search terms?", 
+            choices=['Pages ID', 'Search Terms'],
+        ),
+        inquirer3.Text(
+            "pages_id_path",
+            message="Please provide the name of your Excel file with pages ID (needs to be inside the data folder)",
+            ignore=lambda answers: answers['search_by'] == 'Search Terms',
+            validate=ExcelValidator.validate_excel,
+        ),
+        inquirer3.Text(
+            "search_terms",
+            message="Please provide one or more search terms, separated by a comma",
+            ignore=lambda answers: answers['search_by'] == 'Pages ID',
+        )
     ]
-    #TODO: check if the excel file is valid
-    """
-        {
-            'type': 'input',
-            'name': 'pages_id_path',
-            'message': 'Excel file not found or unable to open. Please provide a new path',
-            'when': lambda answers: (not is_valid_excel_file(answers['pages_id_path'])) and answers['search_by'] == 'Pages ID'
-        },
-    """
 
-    answers = prompt(add_questions, style=default_style)
+    answers = inquirer3.prompt(add_questions, theme=default_style)
     return answers
 
 
 def run_task_A(project_name, answers):
     """
     Run task A: Download ads data from the Meta Online Ad Library based on user-provided parameters.
 
@@ -153,42 +138,27 @@
 
         data = update_access_token(data, answers['access_token'])
        
         print("Starting downloading media content.")
 
         # if task C was chosen - continue with downloading media content
         questions_down = [
-            {
-                'type': 'list',
-                'name': 'nr_ads',
-                'message': f'You currently have {total_ads} ads in your search. For how many do you want to download media content?',
-                'choices': [
-                            {
-                                'name': 'A - 50',
-                            },
-                            {
-                                'name': 'B - 100',
-                            },
-                            {
-                                'name': 'C - 200',
-                            },
-                            {
-                                'name': 'D - insert a custom number',
-                            },
-                ]
-            },
-            { # if the user wants a custom number of media content
-                'type': 'input',
-                'name': 'custom_ads_nr',
-                'message': 'Please provide the number of ads you want to download media content for',
-                'when': lambda answers: answers['nr_ads'] == 'D - insert a custom number',
-                'validate': NumberValidator
-            }
+            inquirer3.List(
+                "nr_ads", 
+                message=f"You currently have {total_ads} ads in your search. For how many do you want to download media content?", 
+                choices=['A - 50', 'B - 100', 'C - 200', 'D - insert a custom number'],
+            ),
+            inquirer3.Text( # if the user wants a custom number of media content
+                "custom_ads_nr",
+                message="Please provide the number of ads you want to download media content for",
+                ignore=lambda answers: answers['nr_ads'] != 'D - insert a custom number',
+                validate=NumberValidator.validate_number,
+            ),
         ]
-        answers_down = prompt(questions_down, style=default_style)
+        answers_down = inquirer3.prompt(questions_down, theme=default_style)
         if answers_down["nr_ads"] == 'A - 50':
             nr_ads = 50
         elif answers_down["nr_ads"] == 'B - 100':
             nr_ads = 100
         elif answers_down["nr_ads"] == 'C - 200':
             nr_ads = 200
         else:
@@ -200,47 +170,29 @@
 
 def intro_messages():
     """
     Display introductory messages and gather user input and Meta developer access token for selected task.
     After selecting the task, the respective function will be run.
     """
     questions = [
-        {
-            'type': 'list',
-            'name': 'task',
-            'message': 'Welcome to the AdDownloader! Select the task you want to perform: ',
-            'choices': [
-                        {
-                            'name': 'A - download ads data only',
-                        },
-                        {
-                            'name': 'B - download ads media content only',
-                        },
-                        {
-                            'name': 'C - download both ads data and media content',
-                        },
-                        {
-                            'name': 'D - open dashboard (using existing data)'
-                        },
-            ],
-        },
-        {
-            'type': 'password',
-            'name': 'access_token',
-            'message': 'Please provide a valid access token',
-            'when': lambda answers: answers['task'] != 'D - open dashboard (using existing data)',
-        },
-        {
-            'type': 'confirm',
-            'name': 'start',
-            'message': 'Are you sure you want to proceed?',
-        }
+        inquirer3.List(
+            "task", 
+            message="Welcome to the AdDownloader! Select the task you want to perform: ", 
+            choices=['A - download ads data only', 'B - download ads media content only', 'C - download both ads data and media content',
+                     'D - open dashboard (using existing data)'],
+        ),
+        inquirer3.Password(
+            name="access_token", 
+            message='Please provide a valid access token',
+            ignore=lambda answers: answers['task'] == 'D - open dashboard (using existing data)',
+        ),
+        inquirer3.Confirm("start", message="Are you sure you want to proceed?", default=True),
     ]
 
-    answers = prompt(questions, style=default_style)
+    answers = inquirer3.prompt(questions, theme=default_style)
 
     rprint(f"[green bold]You have chosen task {answers['task']}.[green bold]")
 
     if answers['task'] == 'A - download ads data only':
         rprint("[yellow]Please enter a name for your project. All created folders will use this name:[yellow]")
         project_name = input()
         run_task_A(project_name, answers)
@@ -275,15 +227,15 @@
     """
     Main function to run the AdDownloader tool until the user stops the analysis.
     """
     
     while True:
         intro_messages()
 
-        # Prompt to ask if the user wants to perform another analysis
+        # ask if the user wants to perform another analysis
         rerun = typer.confirm("Do you want to perform a new analysis?")
         if not rerun:
             rprint("[yellow]=============================================[yello]")
             rprint("[yellow]Analysis completed. Thank you for using AdDownloader! [yello]")
             break
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `addownloader-0.2.5/AdDownloader/helpers.py` & `addownloader-0.2.6/AdDownloader/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 """This module provides different helper functions for the AdDownloader."""
 
 import json
 import pandas as pd
 import os
 import math
 from datetime import datetime, timedelta
-from prompt_toolkit.validation import Validator, ValidationError
+from inquirer3 import errors
 import logging
 import ast
+from collections.abc import Mapping
 import requests
 
 
-class NumberValidator(Validator):
-    """A class representing a number validator."""
-    def validate(self, document):
-        """
-        Checks whether the input is a valid number.
+class NumberValidator:
+    @staticmethod
+    def validate_number(answers, current):
+            """
+            Checks whether the input is a valid number.
+
+            :param document: A document representing user's number input.
+            :type document: document
+            :returns: True if the text of the document represents a valid number, False otherwise.
+            :rtype: bool
+            """
+            try:
+                int(current)
+            except ValueError:
+                raise errors.ValidationError('', reason='Please enter a valid number.')
+            
+            return True
 
-        :param document: A document representing user's number input.
-        :type document: document
-        :returns: True if the text of the document represents a valid number, False otherwise.
-        :rtype: bool
-        """
-        try:
-            int(document.text)
-        except ValueError:
-            raise ValidationError(
-                message='Please enter a number',
-                cursor_position=len(document.text))  # move cursor to end
         
-class DateValidator(Validator):
+class DateValidator:
     """A class representing a date validator."""
-    def validate(self, document):
+    @staticmethod
+    def validate_date(answers, current):
         """
         Checks whether the input is a valid date in the format Y-m-d (e.g. "2023-12-31").
 
         :param document: A document representing user's date input.
         :type document: document
         :returns: True if the text of the document represents a valid date, False otherwise.
         :rtype: bool
         """
         try:
-            datetime.strptime(document.text, '%Y-%m-%d')
+            datetime.strptime(current, '%Y-%m-%d')
         except ValueError:
-            raise ValidationError(
-                message='Please enter a valid date',
-                cursor_position=len(document.text))
+            raise errors.ValidationError('', reason='Please enter a valid date.')
+        
+        return True
 
-class CountryValidator(Validator):
+# check what argument to input here (was Validator before)
+class CountryValidator:
     """A class representing a country code validator."""
-    def validate(self, document):
+    @staticmethod
+    def validate_country(answers, current):
         """
         Checks whether the input is a valid country code.
 
         :param document: A document representing user's country code input.
         :type document: document
         :returns: True if the text of the document represents a valid country code, False otherwise.
         :rtype: bool
@@ -68,50 +73,46 @@
                 JE, GU, YE, ZM, IM, HT, KH, AW, PF, AF, BM, GY, AM, MW, AG, RW, GG, GM, FO, LC, KY, 
                 BJ, AD, GD, VI, BZ, VC, MN, MZ, ML, AO, GF, UZ, DJ, BF, MC, TG, GL, GA, GI, CD, KG, 
                 PG, BT, KN, SZ, LS, LA, LI, MP, SR, SC, VG, TC, DM, MR, AX, SM, SL, NE, CG, AI, YT, 
                 CV, GN, TM, BI, TJ, VU, SB, ER, WS, AS, FK, GQ, TO, KM, PW, FM, CF, SO, MH, VA, TD, 
                 KI, ST, TV, NR, RE, LR, ZW, CI, MM, AN, AQ, BQ, BV, IO, CX, CC, CK, CW, TF, GW, HM, 
                 XK, MS, NU, NF, PN, BL, SH, MF, PM, SX, GS, SS, SJ, TL, TK, UM, WF, EH"""
         country_codes = [code.strip() for code in country_codes.split(",")]
-        ok = document.text in country_codes
-        if not ok:
-            raise ValidationError(
-                message='Please enter a valid country code.',
-                cursor_position=len(document.text))
+        if not current in country_codes:
+            raise errors.ValidationError('', reason='Please enter a valid country code.')
+        
+        return True
 
 
-class ExcelValidator(Validator):
+class ExcelValidator:
     """A class representing a valid Excel file validator."""
-    def validate(self, document):
+    
+    def validate_excel(answers, current):
         """
         Checks whether the input is a valid Excel file.
 
         :param document: A document representing user's Excel file name input.
         :type document: document
         :returns: True if the text of the document represents a valid Excel file containing a column `page_id`, False otherwise.
         :rtype: bool
         """
-        if (not is_valid_excel_file(document.text)):
-            raise ValidationError(
-                    message='Excel file not found.',
-                    cursor_position=len(document.text))
+        if (not is_valid_excel_file(current)):
+            raise errors.ValidationError('', reason='Excel file not found.')
         try:
-            data_path = os.path.join("data", document.text)
+            data_path = os.path.join("data", current)
             data = pd.read_excel(data_path)
         except:
-            raise ValidationError(
-                message='Unable to load page ids data.',
-                cursor_position=len(document.text))
+            raise errors.ValidationError('', reason='Unable to load page ids data.')
             
         try:
             data['page_id'].astype(str).tolist()
         except:
-            raise ValidationError(
-                message='Unable to read the page ids. Check if there exists a column `page_id` in your data.',
-                cursor_position=len(document.text))
+            raise errors.ValidationError('', reason='Unable to read the page ids. Check if there exists a column `page_id` in your data.')
+        
+        return True
             
         
 
 def is_valid_excel_file(file):
     """
     Checks whether the input file name is a valid Excel file.
 
@@ -297,21 +298,22 @@
     """
 
     log_path = f"output/{project_name}"
     if not os.path.exists(log_path):
         os.makedirs(log_path)
 
     logger = logging.getLogger(project_name)
-    logger.setLevel(logging.DEBUG)
+    logger.propagate = False
+    logger.setLevel(logging.INFO)
 
     log_file = logging.FileHandler(os.path.join(log_path, "logs.log"), 'a')  # append mode
     formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s', datefmt='%d/%m/%Y %H:%M:%S')
     log_file.setFormatter(formatter)
 
-    # Check if the logger already has handlers to prevent adding multiple handlers that do the same thing
+    # check if the logger already has handlers to prevent adding multiple handlers that do the same thing
     if not logger.handlers:
         logger.addHandler(log_file)
 
     return logger
 
 
 def close_logger(logger):
```

### Comparing `addownloader-0.2.5/AdDownloader/media_download.py` & `addownloader-0.2.6/AdDownloader/media_download.py`

 * *Files identical despite different names*

### Comparing `addownloader-0.2.5/AdDownloader.egg-info/PKG-INFO` & `addownloader-0.2.6/AdDownloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdDownloader
-Version: 0.2.5
+Version: 0.2.6
 Summary: A cmd tool for downloading ads and their media content from the Meta Ad Library.
 Author-email: Paula-Alexandra Gitu <paula.gitu@maastrichtuniversity.nl>
 Maintainer-email: Paula-Alexandra Gitu <paula.gitu@maastrichtuniversity.nl>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -679,37 +679,38 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/Paularossi/AdDownloader
 Project-URL: Issues, https://github.com/Paularossi/AdDownloader/issues
 Keywords: CLI tool,MetaAPI,AdLibrary,image scraping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Requires-Python: ==3.9.*
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click==8.1.3
 Requires-Dist: dash==2.15.0
 Requires-Dist: datetime==5.4
 Requires-Dist: gensim==4.3.2
+Requires-Dist: inquirer3==0.4.0
 Requires-Dist: meson==1.3.1
 Requires-Dist: ninja==1.11.1.1
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: opencv-python==4.9.0.80
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pandas==2.0.3
 Requires-Dist: pillow==10.2.0
-Requires-Dist: prompt_toolkit==1.0.14
-Requires-Dist: PyInquirer==1.0.3
 Requires-Dist: pytest>=6.2.4
 Requires-Dist: requests==2.31.0
 Requires-Dist: rich==13.6.0
 Requires-Dist: scikit-image==0.22.0
 Requires-Dist: scikit-learn==1.4.1.post1
 Requires-Dist: scipy==1.12
 Requires-Dist: selenium==4.16.0
@@ -795,15 +796,15 @@
 8. 📈 **Optional - Explore Insights** → Perform ad creatives (text & image) analysis and visualize the outputs in a Dashboard.
 
 Each step in this pipeline is designed to ensure a smooth and efficient user experience, from data retrieval to processing and final output. Please note that this tool should only be used for research purposes.
 
 ## Prerequisities
 To download and run the AdDownloader, several prerequisities must be fullfilled:
 
-* Python 3.9.*
+* Python 3.9, 3.10 or 3.11
 * Verified identity and location on Facebook
 * A valid Meta developer access token
 
 
 
 ## Installation
```

### Comparing `addownloader-0.2.5/LICENSE.txt` & `addownloader-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `addownloader-0.2.5/PKG-INFO` & `addownloader-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdDownloader
-Version: 0.2.5
+Version: 0.2.6
 Summary: A cmd tool for downloading ads and their media content from the Meta Ad Library.
 Author-email: Paula-Alexandra Gitu <paula.gitu@maastrichtuniversity.nl>
 Maintainer-email: Paula-Alexandra Gitu <paula.gitu@maastrichtuniversity.nl>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -679,37 +679,38 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/Paularossi/AdDownloader
 Project-URL: Issues, https://github.com/Paularossi/AdDownloader/issues
 Keywords: CLI tool,MetaAPI,AdLibrary,image scraping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Requires-Python: ==3.9.*
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click==8.1.3
 Requires-Dist: dash==2.15.0
 Requires-Dist: datetime==5.4
 Requires-Dist: gensim==4.3.2
+Requires-Dist: inquirer3==0.4.0
 Requires-Dist: meson==1.3.1
 Requires-Dist: ninja==1.11.1.1
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: opencv-python==4.9.0.80
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pandas==2.0.3
 Requires-Dist: pillow==10.2.0
-Requires-Dist: prompt_toolkit==1.0.14
-Requires-Dist: PyInquirer==1.0.3
 Requires-Dist: pytest>=6.2.4
 Requires-Dist: requests==2.31.0
 Requires-Dist: rich==13.6.0
 Requires-Dist: scikit-image==0.22.0
 Requires-Dist: scikit-learn==1.4.1.post1
 Requires-Dist: scipy==1.12
 Requires-Dist: selenium==4.16.0
@@ -795,15 +796,15 @@
 8. 📈 **Optional - Explore Insights** → Perform ad creatives (text & image) analysis and visualize the outputs in a Dashboard.
 
 Each step in this pipeline is designed to ensure a smooth and efficient user experience, from data retrieval to processing and final output. Please note that this tool should only be used for research purposes.
 
 ## Prerequisities
 To download and run the AdDownloader, several prerequisities must be fullfilled:
 
-* Python 3.9.*
+* Python 3.9, 3.10 or 3.11
 * Verified identity and location on Facebook
 * A valid Meta developer access token
 
 
 
 ## Installation
```

### Comparing `addownloader-0.2.5/README.md` & `addownloader-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 8. 📈 **Optional - Explore Insights** → Perform ad creatives (text & image) analysis and visualize the outputs in a Dashboard.
 
 Each step in this pipeline is designed to ensure a smooth and efficient user experience, from data retrieval to processing and final output. Please note that this tool should only be used for research purposes.
 
 ## Prerequisities
 To download and run the AdDownloader, several prerequisities must be fullfilled:
 
-* Python 3.9.*
+* Python 3.9, 3.10 or 3.11
 * Verified identity and location on Facebook
 * A valid Meta developer access token
 
 
 
 ## Installation
```

#### html2text {}

```diff
@@ -56,21 +56,21 @@
 content. 7. ð **Check Output** â Review all the downloaded media content
 and data inside the output folder with your `project_name`. 8. ð **Optional
 - Explore Insights** â Perform ad creatives (text & image) analysis and
 visualize the outputs in a Dashboard. Each step in this pipeline is designed to
 ensure a smooth and efficient user experience, from data retrieval to
 processing and final output. Please note that this tool should only be used for
 research purposes. ## Prerequisities To download and run the AdDownloader,
-several prerequisities must be fullfilled: * Python 3.9.* * Verified identity
-and location on Facebook * A valid Meta developer access token ## Installation
-AdDownloader can be installed in three different ways: from source, from a
-built distribution, or as a package from *pip*. Open a command-line tool (or a
-terminal) and navigate to your folder with: ```bash cd "[path-to-your-project]/
-AdDownloader" ``` Then, create a virtual environment (venv) with: ```bash
-python -m venv venv ``` And activate the venv: ```bash
+several prerequisities must be fullfilled: * Python 3.9, 3.10 or 3.11 *
+Verified identity and location on Facebook * A valid Meta developer access
+token ## Installation AdDownloader can be installed in three different ways:
+from source, from a built distribution, or as a package from *pip*. Open a
+command-line tool (or a terminal) and navigate to your folder with: ```bash cd
+"[path-to-your-project]/AdDownloader" ``` Then, create a virtual environment
+(venv) with: ```bash python -m venv venv ``` And activate the venv: ```bash
 venv\Scripts\activate.bat ``` ### From source or built distribution Once you're
 inside your repository and the virtual environment, to install from the source
 file run: ```bash python -m pip install "dist/AdDownloader-0.2.5.tar.gz" ``` To
 install from the built distribution run: ```bash python -m pip install "dist/
 AdDownloader-0.2.5-py3-none-any.whl" ``` ### From pip To install AdDownloader
 as a Python package run: ```bash python -m pip install AdDownloader ```
 AdDownloader is now installed and can be run! ## Usage Once installed,
```

### Comparing `addownloader-0.2.5/pyproject.toml` & `addownloader-0.2.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 [project]
 name = "AdDownloader"
 # $ pip install AdDownloader
 # And where it will live on PyPI: https://pypi.org/project/AdDownloader/
 
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   {name = "Paula-Alexandra Gitu", email = "paula.gitu@maastrichtuniversity.nl"},
 ]
 maintainers = [
-  {name = "Paula-Alexandra Gitu", email = "paula.gitu@maastrichtuniversity.nl"} # Optional
+  {name = "Paula-Alexandra Gitu", email = "paula.gitu@maastrichtuniversity.nl"}
 ]
 
 # the description corresponds to the "Summary" metadata field:
 description = "A cmd tool for downloading ads and their media content from the Meta Ad Library."
 readme = "README.md"
-requires-python = "==3.9.*"
+requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
-keywords = ["CLI tool", "MetaAPI", "AdLibrary", "image scraping"]  # Optional
+keywords = ["CLI tool", "MetaAPI", "AdLibrary", "image scraping"]
 
 # For a list of valid classifiers, see https://pypi.org/classifiers/
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",    
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: Microsoft :: Windows",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
 ]
 
 # add the necessary packages here
 dependencies = [
   "click==8.1.3",
   "dash==2.15.0",
   "datetime==5.4",
   "gensim==4.3.2",
+  "inquirer3==0.4.0",
   "meson==1.3.1",
   "ninja==1.11.1.1",
   "nltk==3.8.1",
   "numpy==1.26.4",
   "opencv-python==4.9.0.80",
   "openpyxl==3.1.2",
   "pandas==2.0.3",
   "pillow==10.2.0",
-  "prompt_toolkit==1.0.14",
-  "PyInquirer==1.0.3",
   "pytest>=6.2.4",
   "requests==2.31.0",
   "rich==13.6.0",
   "scikit-image==0.22.0",
   "scikit-learn==1.4.1.post1",
   "scipy==1.12",
   "selenium==4.16.0",
@@ -72,9 +73,9 @@
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-exclude = ["data", "dist", "docs", "tests", "venv"]
+exclude = ["data", "dist", "docs", "tests", "myenv", "output"]
 namespaces = false
```

### Comparing `addownloader-0.2.5/tests/test_AdDownloader.py` & `addownloader-0.2.6/tests/test_AdDownloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -353,7 +353,23 @@
 # topic analysis time by ad type and sample size
 g = sns.FacetGrid(merged_df, col="ad_type", row="sample_size", margin_titles=True, height=3, aspect=1.3)
 g.map(sns.scatterplot, "nr_topics", "topic_analysis_time")
 g.figure.suptitle('Topic Analysis Time by Number of Topics, Ad Type, and Sample Size', fontsize=16)
 g.figure.subplots_adjust(top=0.9)  
 plt.show()
 
+
+
+
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.common.exceptions import NoSuchElementException
+import requests
+
+
+driver = webdriver.Chrome()
+
+driver.get("https://www.funda.nl/zoeken/koop?selected_area=%5B%22maastricht%22%5D")
+
+temp = driver.find_element(By.CLASS_NAME, "mt-4 font-semibold sm:mt-0")
```

