# Comparing `tmp/smolqwery-0.1.2.tar.gz` & `tmp/smolqwery-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smolqwery-0.1.2.tar", max compression
+gzip compressed data, was "smolqwery-0.1.3.tar", max compression
```

## Comparing `smolqwery-0.1.2.tar` & `smolqwery-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     9165 2022-03-08 14:43:07.485982 smolqwery-0.1.2/README.md
--rw-r--r--   0        0        0      655 2022-09-13 10:42:50.890222 smolqwery-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       62 2022-03-08 14:43:07.493982 smolqwery-0.1.2/src/smolqwery/__init__.py
--rw-r--r--   0        0        0     6154 2022-03-08 14:43:07.493982 smolqwery-0.1.2/src/smolqwery/_utils.py
--rw-r--r--   0        0        0      225 2022-03-08 14:43:07.493982 smolqwery-0.1.2/src/smolqwery/apps.py
--rw-r--r--   0        0        0     3818 2022-03-08 14:43:07.493982 smolqwery-0.1.2/src/smolqwery/bigqwery.py
--rw-r--r--   0        0        0     3486 2022-03-08 14:43:07.493982 smolqwery-0.1.2/src/smolqwery/config.py
--rw-r--r--   0        0        0    18066 2022-03-08 14:43:07.493982 smolqwery-0.1.2/src/smolqwery/extractor.py
--rw-r--r--   0        0        0      894 2022-03-08 14:43:07.493982 smolqwery-0.1.2/src/smolqwery/management/commands/smolqwery_extract.py
--rw-r--r--   0        0        0     1203 2022-03-08 14:43:07.493982 smolqwery-0.1.2/src/smolqwery/management/commands/smolqwery_make_migrations.py
--rw-r--r--   0        0        0     2109 2022-03-08 14:43:07.493982 smolqwery-0.1.2/src/smolqwery/management/commands/smolqwery_print_extract.py
--rw-r--r--   0        0        0    13819 2022-09-13 10:38:38.272734 smolqwery-0.1.2/src/smolqwery/swallow.py
--rw-r--r--   0        0        0    10287 2022-09-13 10:44:44.669564 smolqwery-0.1.2/setup.py
--rw-r--r--   0        0        0     9927 2022-09-13 10:44:44.670758 smolqwery-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     9165 2022-03-08 14:43:07.000000 smolqwery-0.1.3/README.md
+-rw-r--r--   0        0        0      649 2024-04-30 13:14:42.796285 smolqwery-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       62 2022-03-08 14:43:07.000000 smolqwery-0.1.3/src/smolqwery/__init__.py
+-rw-r--r--   0        0        0     6154 2022-03-08 14:43:07.000000 smolqwery-0.1.3/src/smolqwery/_utils.py
+-rw-r--r--   0        0        0      225 2022-03-08 14:43:07.000000 smolqwery-0.1.3/src/smolqwery/apps.py
+-rw-r--r--   0        0        0     3818 2022-03-08 14:43:07.000000 smolqwery-0.1.3/src/smolqwery/bigqwery.py
+-rw-r--r--   0        0        0     3486 2022-03-08 14:43:07.000000 smolqwery-0.1.3/src/smolqwery/config.py
+-rw-r--r--   0        0        0    18066 2022-03-08 14:43:07.000000 smolqwery-0.1.3/src/smolqwery/extractor.py
+-rw-r--r--   0        0        0      894 2022-03-08 14:43:07.000000 smolqwery-0.1.3/src/smolqwery/management/commands/smolqwery_extract.py
+-rw-r--r--   0        0        0     1203 2022-03-08 14:43:07.000000 smolqwery-0.1.3/src/smolqwery/management/commands/smolqwery_make_migrations.py
+-rw-r--r--   0        0        0     2109 2022-03-08 14:43:07.000000 smolqwery-0.1.3/src/smolqwery/management/commands/smolqwery_print_extract.py
+-rw-r--r--   0        0        0    13819 2022-09-13 10:45:03.000000 smolqwery-0.1.3/src/smolqwery/swallow.py
+-rw-r--r--   0        0        0    10023 1970-01-01 00:00:00.000000 smolqwery-0.1.3/PKG-INFO
```

### Comparing `smolqwery-0.1.2/README.md` & `smolqwery-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `smolqwery-0.1.2/pyproject.toml` & `smolqwery-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "smolqwery"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Django-oriented tool to make analytics exports to BigQuery"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
 readme = "README.md"
 repository = "https://github.com/Xowap/smolqwery"
 homepage = "https://github.com/Xowap/smolqwery"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8"
 python-dateutil = ">=2"
 black = ">=20"
 google-cloud-bigquery = ">=2"
 rich = ">=11"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
```

### Comparing `smolqwery-0.1.2/src/smolqwery/_utils.py` & `smolqwery-0.1.3/src/smolqwery/_utils.py`

 * *Files identical despite different names*

### Comparing `smolqwery-0.1.2/src/smolqwery/bigqwery.py` & `smolqwery-0.1.3/src/smolqwery/bigqwery.py`

 * *Files identical despite different names*

### Comparing `smolqwery-0.1.2/src/smolqwery/config.py` & `smolqwery-0.1.3/src/smolqwery/config.py`

 * *Files identical despite different names*

### Comparing `smolqwery-0.1.2/src/smolqwery/extractor.py` & `smolqwery-0.1.3/src/smolqwery/extractor.py`

 * *Files identical despite different names*

### Comparing `smolqwery-0.1.2/src/smolqwery/management/commands/smolqwery_extract.py` & `smolqwery-0.1.3/src/smolqwery/management/commands/smolqwery_extract.py`

 * *Files identical despite different names*

### Comparing `smolqwery-0.1.2/src/smolqwery/management/commands/smolqwery_make_migrations.py` & `smolqwery-0.1.3/src/smolqwery/management/commands/smolqwery_make_migrations.py`

 * *Files identical despite different names*

### Comparing `smolqwery-0.1.2/src/smolqwery/management/commands/smolqwery_print_extract.py` & `smolqwery-0.1.3/src/smolqwery/management/commands/smolqwery_print_extract.py`

 * *Files identical despite different names*

### Comparing `smolqwery-0.1.2/src/smolqwery/swallow.py` & `smolqwery-0.1.3/src/smolqwery/swallow.py`

 * *Files identical despite different names*

### Comparing `smolqwery-0.1.2/setup.py` & `smolqwery-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,289 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: smolqwery
+Version: 0.1.3
+Summary: A Django-oriented tool to make analytics exports to BigQuery
+Home-page: https://github.com/Xowap/smolqwery
+License: WTFPL
+Author: Rémy Sanchez
+Author-email: remy.sanchez@hyperthese.net
+Requires-Python: >=3.8
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: black (>=20)
+Requires-Dist: google-cloud-bigquery (>=2)
+Requires-Dist: python-dateutil (>=2)
+Requires-Dist: rich (>=11)
+Project-URL: Repository, https://github.com/Xowap/smolqwery
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Smolqwery
 
-packages = \
-['smolqwery', 'smolqwery.management.commands']
+A Django-oriented micro-framework to help structuring BigQuery exports with Data
+Studio and analytics in mind.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['black>=20', 'google-cloud-bigquery>=2', 'python-dateutil>=2', 'rich>=11']
-
-setup_kwargs = {
-    'name': 'smolqwery',
-    'version': '0.1.2',
-    'description': 'A Django-oriented tool to make analytics exports to BigQuery',
-    'long_description': '# Smolqwery\n\nA Django-oriented micro-framework to help structuring BigQuery exports with Data\nStudio and analytics in mind.\n\nIt lets you write minimal extractors that will generate the statistics you need\nand it will manage everything around them (creating the tables on BigQuery,\nrunning the exports, etc).\n\n## Integration guide\n\nWe\'ll review here how you can integrate Smolqwery in your project.\n\n### Installation\n\nFirst step is (obviously to add it to the dependencies). You just need to\nspecify that you need the `smolqwery` package (use `pip`, `poetry` or whatever).\n\n### Django configuration\n\nYou can thank Google for that, the configuration is a bit complex. The first\nthing to do is to add it in your installed apps:\n\n```python\nINSTALLED_APPS = [\n    # your stuff\n    "smolqwery",\n    # more of your stuff\n]\n```\n\nThen there is _a few_ variables to configure:\n\n-   Things specific to your project\n    -   `SMOLQWERY_EXTRACTORS` &mdash; List of extractors, more on this below\n    -   `SMOLQWERY_DJANGO_APP` &mdash; App in which migrations must be created\n    -   `SMOLQWERY_FIRST_DATE` &mdash; First date of data to include in exports\n        (all days between this date and now will be exported)\n-   Things that you want to specify about BigQuery\n    -   `SMOLQWERY_DATASET` &mdash; Name of the dataset (database if you compare\n        to PostgreSQL for example). It will be created automatically by the\n        migrations, you don\'t need to create it yourself.\n    -   `SMOLQWERY_DATASET_LOCATION` &mdash; Location of the data. Unless you\n        want to be specific you can just say "EU" or "US"\n    -   `SMOLQWERY_ACL_GROUPS` &mdash; List of IAM groups emails that will\n        receive the read/write permissions on the created dataset\n-   Google credentials (more on this later)\n    -   `SMOLQWERY_GOOGLE_TYPE`\n    -   `SMOLQWERY_GOOGLE_PROJECT_ID`\n    -   `SMOLQWERY_GOOGLE_PRIVATE_KEY_ID`\n    -   `SMOLQWERY_GOOGLE_PRIVATE_KEY`\n    -   `SMOLQWERY_GOOGLE_CLIENT_EMAIL`\n    -   `SMOLQWERY_GOOGLE_CLIENT_ID`\n    -   `SMOLQWERY_GOOGLE_AUTH_URI`\n    -   `SMOLQWERY_GOOGLE_TOKEN_URI`\n    -   `SMOLQWERY_GOOGLE_AUTH_PROVIDER_X509_CERT_URL`\n    -   `SMOLQWERY_GOOGLE_CLIENT_X509_CERT_URL`\n\n### Getting Google credentials\n\nSo. There is a bunch of credentials to get. Roughly, the steps to get them is:\n\n-   Log into the Google Cloud Console\n-   Create a project (you can re-use this same project between several instances\n    of your code as long as you let each instance use a different dataset name)\n-   Create a service account within this project\n-   Download the credentials of this service account (as JSON file) and recopy\n    the contents of this file into the configuration. For example in the JSON\n    file there is a `project_id` entry, it matches the\n    `SMOLQWERY_GOOGLE_PROJECT_ID` setting\n\n### Creating extractors\n\nYou can now start creating extractors. It\'s the way your code will convert your\ndata into the statistics you want to store.\n\n#### Extractor type\n\nThe first step is to decide what kind of extractor you\'re going to do:\n\n-   Date-aggregated &mdash; Each row is a single date. By example "today there\n    was 345 new users and 23 new contracts"\n-   Individual rows &mdash; Each row is one entry. By example, each row can\n    represent one email that has been sent.\n\nHow to choose? If you\'re dealing with personal data, the only way you can use it\nfor statistics without consent is to aggregate it.\n\n> _Note_ &mdash; As long as an ID represents a single or a few users (hash,\n> fingerprint, etc) then it\'s considered to be a personal data. There is no such\n> thing as anonymization. The only way out is aggregation.\n\nThe way to handle dates is going to be different depending on the type:\n\n-   Date-aggregated extractors don\'t have to include a date in their data model,\n    since it\'s the system that decides which date range corresponds to which\n    date "row". For that matter, you need need to reply with the data you deduce\n    from the range you\'re asked to extract and that\'s it.\n-   Individual rows must contain a timestamp field which indicates to which date\n    this field is related. It can be a timestamp (date/time + timezone) or a\n    simple date. It will not be added automatically but it is expected to be\n    named `timestamp` (see below how to define fields). You can override this\n    name in the extractor if you need to.\n\n#### Dataclass\n\nYou declare what you\'re going to return using a dataclass. It\'s a bit like\nDjango models, it\'s used to define what are the fields.\n\nHere is type types mapping (in relation to Big Query\'s types):\n\n-   `int` &rarr; `INT64`\n-   `float` &rarr; `FLOAT64`\n-   `bool` &rarr; `BOOL`\n-   `str` &rarr; `STRING`\n-   `bytes` &rarr; `BYTES`\n-   `datetime.date` &rarr; `DATE`\n-   `datetime.datetime` &rarr; `TIMESTAMP` (make sure to use time-zone-aware\n    datetime instances, there is no check of this)\n\nIf you need your field to be nullable you can use the `Optional` type\nannotation.\n\nAnother thing is the "differentiated" fields. For example let\'s say that you\nhave a strictly growing metric ("number of users that ever registered") and you\nwant to easily know the difference from one date to the other ("number of users\nthat registered during the time range") in the data studio. You can mark a field\nas "differentiated", which will trigger the creation of a view where the metric\nis differentiated day-by-day.\n\nYou would have the `user` table with this data:\n\n| Date       | Registered |\n| ---------- | ---------- |\n| 2022-01-01 | 10         |\n| 2022-01-02 | 20         |\n| 2022-01-03 | 35         |\n\nAnd then the `user_delta` view with:\n\n| Date       | Registered |\n| ---------- | ---------- |\n| 2022-01-01 | 10         |\n| 2022-01-02 | 10         |\n| 2022-01-03 | 15         |\n\nThis can be done using the `sq_field(diffrentiate=True)` field (which is a\nshortcut to `dataclasses`\'s `field` created for our purpose).\n\nHere is an example of both a date-aggregated and individual-rows dataclasses:\n\n```python\nfrom dataclasses import dataclass\nfrom smolqwery import sq_field\nimport datetime\n\n@dataclass\nclass User:\n    users: int = sq_field(differentiate=True)\n    prospects: int = sq_field(differentiate=True)\n    clients: int = sq_field(differentiate=True)\n\n\n@dataclass\nclass Email:\n    timestamp: datetime.datetime\n    type: str\n```\n\n#### Extractor\n\nThe extractors themselves are a simple interface that you need to implement to\nreach your needs. For example:\n\n```python\nclass EmailExtractor(BaseExtractor[Email]):\n    def get_dataclass(self) -> Type[Email]:\n        return Email\n\n    def get_extractor_type(self) -> ExtractorType:\n        return ExtractorType.individual_rows\n\n    def extract(\n        self, date_start: datetime.datetime, date_end: datetime.datetime\n    ) -> Iterator[Email]:\n        for email in EmailMessage.objects.filter(\n            date_sent__gte=date_start, date_sent__lt=date_end\n        ):\n            yield Email(\n                timestamp=email.date_sent,\n                type=email.type,\n            )\n```\n\nLet\'s note here that `date_start` is inclusive and `date_end` is exclusive.\n\nYou need to declare your extractors in the settings, for example:\n\n```python\nSMOLQWERY_EXTRACTORS = [\n    "core.smolqwery.UserExtractor",\n    "core.smolqwery.EmailExtractor",\n]\n```\n\n#### Migrations\n\nLike Django, and using Django\'s system in part, Smolqwery will manage its table\nwithin BigQuery using migrations. Those schema are automatically created from\nthe dataclasses that you\'ve defined.\n\nHowever unlike Django you cannot change a data model once it has been created,\nbecause it would complicate things a lot for something that you don\'t really\nneed.\n\nSee it that way: you want to add a bunch of statistics to your BigQuery `user`\ntable. If your statistics can be computed from observing the data in your\ndatabase, you could just create a `user2` table and re-compute statistics from\nthe beginning into this table. This will provide the warranty that all fields\npresent indeed have a value (as opposed to having to keep all new columns at\nNULL).\n\nIt\'s quite flexible this way: you can either create a new table and put just the\nnew fields there, either forget about the old table and re-compute everything\nfrom the start in a new table, etc.\n\nSo, how do you migrate?\n\n```\n./manage.py smolqwery_make_migrations\n./manage.py migrate\n```\n\nLet\'s note that if you (or the next person) doesn\'t have the Google credentials\nconfigured, then you\'ll run into an issue.\n\n### Exporting\n\nNow you can run the export.\n\nEither with a test run\n\n```\n./manage.py smolqwery_print_extract -f 2022-01-01 -l 2022-01-05\n```\n\nEither with a real run, that will really insert the data\n\n```\n./manage.py smolqwery_extract\n```\n\nThe extract will look up for the date of the last extract table by table. If the\nextract was never done then it will fall back to the `SMOLQWERY_FIRST_DATE`\nsetting.\n\nAll the days between the last extract and the last revolute day (in Django\'s\ntime zone) will be extracted.\n\nYou can safely run this as a cron, several times a day if you want to.\n\n### Exploiting the data\n\nNow all your data is in BigQuery and you can start using it from Data Studio or\nother sources!\n',
-    'author': 'Rémy Sanchez',
-    'author_email': 'remy.sanchez@hyperthese.net',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/Xowap/smolqwery',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
+It lets you write minimal extractors that will generate the statistics you need
+and it will manage everything around them (creating the tables on BigQuery,
+running the exports, etc).
 
+## Integration guide
+
+We'll review here how you can integrate Smolqwery in your project.
+
+### Installation
+
+First step is (obviously to add it to the dependencies). You just need to
+specify that you need the `smolqwery` package (use `pip`, `poetry` or whatever).
+
+### Django configuration
+
+You can thank Google for that, the configuration is a bit complex. The first
+thing to do is to add it in your installed apps:
+
+```python
+INSTALLED_APPS = [
+    # your stuff
+    "smolqwery",
+    # more of your stuff
+]
+```
+
+Then there is _a few_ variables to configure:
+
+-   Things specific to your project
+    -   `SMOLQWERY_EXTRACTORS` &mdash; List of extractors, more on this below
+    -   `SMOLQWERY_DJANGO_APP` &mdash; App in which migrations must be created
+    -   `SMOLQWERY_FIRST_DATE` &mdash; First date of data to include in exports
+        (all days between this date and now will be exported)
+-   Things that you want to specify about BigQuery
+    -   `SMOLQWERY_DATASET` &mdash; Name of the dataset (database if you compare
+        to PostgreSQL for example). It will be created automatically by the
+        migrations, you don't need to create it yourself.
+    -   `SMOLQWERY_DATASET_LOCATION` &mdash; Location of the data. Unless you
+        want to be specific you can just say "EU" or "US"
+    -   `SMOLQWERY_ACL_GROUPS` &mdash; List of IAM groups emails that will
+        receive the read/write permissions on the created dataset
+-   Google credentials (more on this later)
+    -   `SMOLQWERY_GOOGLE_TYPE`
+    -   `SMOLQWERY_GOOGLE_PROJECT_ID`
+    -   `SMOLQWERY_GOOGLE_PRIVATE_KEY_ID`
+    -   `SMOLQWERY_GOOGLE_PRIVATE_KEY`
+    -   `SMOLQWERY_GOOGLE_CLIENT_EMAIL`
+    -   `SMOLQWERY_GOOGLE_CLIENT_ID`
+    -   `SMOLQWERY_GOOGLE_AUTH_URI`
+    -   `SMOLQWERY_GOOGLE_TOKEN_URI`
+    -   `SMOLQWERY_GOOGLE_AUTH_PROVIDER_X509_CERT_URL`
+    -   `SMOLQWERY_GOOGLE_CLIENT_X509_CERT_URL`
+
+### Getting Google credentials
+
+So. There is a bunch of credentials to get. Roughly, the steps to get them is:
+
+-   Log into the Google Cloud Console
+-   Create a project (you can re-use this same project between several instances
+    of your code as long as you let each instance use a different dataset name)
+-   Create a service account within this project
+-   Download the credentials of this service account (as JSON file) and recopy
+    the contents of this file into the configuration. For example in the JSON
+    file there is a `project_id` entry, it matches the
+    `SMOLQWERY_GOOGLE_PROJECT_ID` setting
+
+### Creating extractors
+
+You can now start creating extractors. It's the way your code will convert your
+data into the statistics you want to store.
+
+#### Extractor type
+
+The first step is to decide what kind of extractor you're going to do:
+
+-   Date-aggregated &mdash; Each row is a single date. By example "today there
+    was 345 new users and 23 new contracts"
+-   Individual rows &mdash; Each row is one entry. By example, each row can
+    represent one email that has been sent.
+
+How to choose? If you're dealing with personal data, the only way you can use it
+for statistics without consent is to aggregate it.
+
+> _Note_ &mdash; As long as an ID represents a single or a few users (hash,
+> fingerprint, etc) then it's considered to be a personal data. There is no such
+> thing as anonymization. The only way out is aggregation.
+
+The way to handle dates is going to be different depending on the type:
+
+-   Date-aggregated extractors don't have to include a date in their data model,
+    since it's the system that decides which date range corresponds to which
+    date "row". For that matter, you need need to reply with the data you deduce
+    from the range you're asked to extract and that's it.
+-   Individual rows must contain a timestamp field which indicates to which date
+    this field is related. It can be a timestamp (date/time + timezone) or a
+    simple date. It will not be added automatically but it is expected to be
+    named `timestamp` (see below how to define fields). You can override this
+    name in the extractor if you need to.
+
+#### Dataclass
+
+You declare what you're going to return using a dataclass. It's a bit like
+Django models, it's used to define what are the fields.
+
+Here is type types mapping (in relation to Big Query's types):
+
+-   `int` &rarr; `INT64`
+-   `float` &rarr; `FLOAT64`
+-   `bool` &rarr; `BOOL`
+-   `str` &rarr; `STRING`
+-   `bytes` &rarr; `BYTES`
+-   `datetime.date` &rarr; `DATE`
+-   `datetime.datetime` &rarr; `TIMESTAMP` (make sure to use time-zone-aware
+    datetime instances, there is no check of this)
+
+If you need your field to be nullable you can use the `Optional` type
+annotation.
+
+Another thing is the "differentiated" fields. For example let's say that you
+have a strictly growing metric ("number of users that ever registered") and you
+want to easily know the difference from one date to the other ("number of users
+that registered during the time range") in the data studio. You can mark a field
+as "differentiated", which will trigger the creation of a view where the metric
+is differentiated day-by-day.
+
+You would have the `user` table with this data:
+
+| Date       | Registered |
+| ---------- | ---------- |
+| 2022-01-01 | 10         |
+| 2022-01-02 | 20         |
+| 2022-01-03 | 35         |
+
+And then the `user_delta` view with:
+
+| Date       | Registered |
+| ---------- | ---------- |
+| 2022-01-01 | 10         |
+| 2022-01-02 | 10         |
+| 2022-01-03 | 15         |
+
+This can be done using the `sq_field(diffrentiate=True)` field (which is a
+shortcut to `dataclasses`'s `field` created for our purpose).
+
+Here is an example of both a date-aggregated and individual-rows dataclasses:
+
+```python
+from dataclasses import dataclass
+from smolqwery import sq_field
+import datetime
+
+@dataclass
+class User:
+    users: int = sq_field(differentiate=True)
+    prospects: int = sq_field(differentiate=True)
+    clients: int = sq_field(differentiate=True)
+
+
+@dataclass
+class Email:
+    timestamp: datetime.datetime
+    type: str
+```
+
+#### Extractor
+
+The extractors themselves are a simple interface that you need to implement to
+reach your needs. For example:
+
+```python
+class EmailExtractor(BaseExtractor[Email]):
+    def get_dataclass(self) -> Type[Email]:
+        return Email
+
+    def get_extractor_type(self) -> ExtractorType:
+        return ExtractorType.individual_rows
+
+    def extract(
+        self, date_start: datetime.datetime, date_end: datetime.datetime
+    ) -> Iterator[Email]:
+        for email in EmailMessage.objects.filter(
+            date_sent__gte=date_start, date_sent__lt=date_end
+        ):
+            yield Email(
+                timestamp=email.date_sent,
+                type=email.type,
+            )
+```
+
+Let's note here that `date_start` is inclusive and `date_end` is exclusive.
+
+You need to declare your extractors in the settings, for example:
+
+```python
+SMOLQWERY_EXTRACTORS = [
+    "core.smolqwery.UserExtractor",
+    "core.smolqwery.EmailExtractor",
+]
+```
+
+#### Migrations
+
+Like Django, and using Django's system in part, Smolqwery will manage its table
+within BigQuery using migrations. Those schema are automatically created from
+the dataclasses that you've defined.
+
+However unlike Django you cannot change a data model once it has been created,
+because it would complicate things a lot for something that you don't really
+need.
+
+See it that way: you want to add a bunch of statistics to your BigQuery `user`
+table. If your statistics can be computed from observing the data in your
+database, you could just create a `user2` table and re-compute statistics from
+the beginning into this table. This will provide the warranty that all fields
+present indeed have a value (as opposed to having to keep all new columns at
+NULL).
+
+It's quite flexible this way: you can either create a new table and put just the
+new fields there, either forget about the old table and re-compute everything
+from the start in a new table, etc.
+
+So, how do you migrate?
+
+```
+./manage.py smolqwery_make_migrations
+./manage.py migrate
+```
+
+Let's note that if you (or the next person) doesn't have the Google credentials
+configured, then you'll run into an issue.
+
+### Exporting
+
+Now you can run the export.
+
+Either with a test run
+
+```
+./manage.py smolqwery_print_extract -f 2022-01-01 -l 2022-01-05
+```
+
+Either with a real run, that will really insert the data
+
+```
+./manage.py smolqwery_extract
+```
+
+The extract will look up for the date of the last extract table by table. If the
+extract was never done then it will fall back to the `SMOLQWERY_FIRST_DATE`
+setting.
+
+All the days between the last extract and the last revolute day (in Django's
+time zone) will be extracted.
+
+You can safely run this as a cron, several times a day if you want to.
+
+### Exploiting the data
+
+Now all your data is in BigQuery and you can start using it from Data Studio or
+other sources!
 
-setup(**setup_kwargs)
```

