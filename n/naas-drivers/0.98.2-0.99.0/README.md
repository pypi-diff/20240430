# Comparing `tmp/naas-drivers-0.98.2.tar.gz` & `tmp/naas-drivers-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/naas-drivers-0.98.2.tar", last modified: Fri Jun  3 12:51:06 2022, max compression
+gzip compressed data, was "dist/naas-drivers-0.99.0.tar", last modified: Fri Jun  3 15:15:54 2022, max compression
```

## Comparing `naas-drivers-0.98.2.tar` & `naas-drivers-0.99.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 12:51:06.225178 naas-drivers-0.98.2/
--rw-r--r--   0 root         (0) root         (0)    34523 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3768 2022-06-03 12:51:06.225178 naas-drivers-0.98.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2221 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 12:51:06.217178 naas-drivers-0.98.2/naas_drivers/
--rw-r--r--   0 root         (0) root         (0)     8243 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1403 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/driver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 12:51:06.225178 naas-drivers-0.98.2/naas_drivers/tools/
--rw-r--r--   0 root         (0) root         (0)     1923 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/__crud.py
--rw-r--r--   0 root         (0) root         (0)     3035 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/__ftp.py
--rw-r--r--   0 root         (0) root         (0)     2743 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/__ftps.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1977 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/airtable.py
--rw-r--r--   0 root         (0) root         (0)     4807 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/awesomenotebook.py
--rw-r--r--   0 root         (0) root         (0)     1961 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/bazimo.py
--rw-r--r--   0 root         (0) root         (0)    11368 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/bobapp.py
--rw-r--r--   0 root         (0) root         (0)      486 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/bubble.py
--rw-r--r--   0 root         (0) root         (0)    11384 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/budgetinsight.py
--rw-r--r--   0 root         (0) root         (0)     2025 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/canny.py
--rw-r--r--   0 root         (0) root         (0)     2954 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/cityfalcon.py
--rw-r--r--   0 root         (0) root         (0)     6342 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/email.py
--rw-r--r--   0 root         (0) root         (0)    27214 2022-06-03 12:50:58.000000 naas-drivers-0.98.2/naas_drivers/tools/emailbuilder.py
--rw-r--r--   0 root         (0) root         (0)     1203 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/ftp.py
--rw-r--r--   0 root         (0) root         (0)     2504 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/geolocator.py
--rw-r--r--   0 root         (0) root         (0)     4178 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/git.py
--rw-r--r--   0 root         (0) root         (0)    30082 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/github.py
--rw-r--r--   0 root         (0) root         (0)    16344 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/googleanalytics.py
--rw-r--r--   0 root         (0) root         (0)     2993 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/gsheet.py
--rw-r--r--   0 root         (0) root         (0)     1716 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/healthcheck.py
--rw-r--r--   0 root         (0) root         (0)    16008 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/hubspot.py
--rw-r--r--   0 root         (0) root         (0)    12384 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/huggingface.py
--rw-r--r--   0 root         (0) root         (0)      459 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/ifttt.py
--rw-r--r--   0 root         (0) root         (0)      392 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/integromat.py
--rw-r--r--   0 root         (0) root         (0)     6759 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/jupyter.py
--rw-r--r--   0 root         (0) root         (0)    42902 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/linkedin.py
--rw-r--r--   0 root         (0) root         (0)      590 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/markdown.py
--rw-r--r--   0 root         (0) root         (0)     3848 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/mongo.py
--rw-r--r--   0 root         (0) root         (0)     1860 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/naas_auth.py
--rw-r--r--   0 root         (0) root         (0)     2716 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/naas_credits.py
--rw-r--r--   0 root         (0) root         (0)     2544 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/newsapi.py
--rw-r--r--   0 root         (0) root         (0)    48996 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/notion.py
--rw-r--r--   0 root         (0) root         (0)     1343 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/optimise.py
--rw-r--r--   0 root         (0) root         (0)     1192 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/pdf.py
--rw-r--r--   0 root         (0) root         (0)     3334 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/plotly.py
--rw-r--r--   0 root         (0) root         (0)     8164 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/prediction.py
--rw-r--r--   0 root         (0) root         (0)    21881 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/qonto.py
--rw-r--r--   0 root         (0) root         (0)     2833 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/sentiment.py
--rw-r--r--   0 root         (0) root         (0)     1573 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/sharepoint.py
--rw-r--r--   0 root         (0) root         (0)     1625 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/slack.py
--rw-r--r--   0 root         (0) root         (0)     1221 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/streamlit.py
--rw-r--r--   0 root         (0) root         (0)     2967 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/taggun.py
--rw-r--r--   0 root         (0) root         (0)      693 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/teams.py
--rw-r--r--   0 root         (0) root         (0)     8137 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/thinkific.py
--rw-r--r--   0 root         (0) root         (0)    21291 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/toucan.py
--rw-r--r--   0 root         (0) root         (0)      198 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/utils.py
--rw-r--r--   0 root         (0) root         (0)     2777 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/yahoofinance.py
--rw-r--r--   0 root         (0) root         (0)     9342 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/youtube.py
--rw-r--r--   0 root         (0) root         (0)      388 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/naas_drivers/tools/zapier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 12:51:06.217178 naas-drivers-0.98.2/naas_drivers.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3768 2022-06-03 12:51:06.000000 naas-drivers-0.98.2/naas_drivers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1794 2022-06-03 12:51:06.000000 naas-drivers-0.98.2/naas_drivers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-03 12:51:06.000000 naas-drivers-0.98.2/naas_drivers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     6236 2022-06-03 12:51:06.000000 naas-drivers-0.98.2/naas_drivers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-06-03 12:51:06.000000 naas-drivers-0.98.2/naas_drivers.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       70 2022-06-03 12:51:06.225178 naas-drivers-0.98.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4335 2022-06-03 12:50:32.000000 naas-drivers-0.98.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 15:15:54.188730 naas-drivers-0.99.0/
+-rw-r--r--   0 root         (0) root         (0)    34523 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3768 2022-06-03 15:15:54.188730 naas-drivers-0.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2221 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 15:15:54.180730 naas-drivers-0.99.0/naas_drivers/
+-rw-r--r--   0 root         (0) root         (0)     8243 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/driver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 15:15:54.188730 naas-drivers-0.99.0/naas_drivers/tools/
+-rw-r--r--   0 root         (0) root         (0)     1923 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/__crud.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/__ftp.py
+-rw-r--r--   0 root         (0) root         (0)     2743 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/__ftps.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/airtable.py
+-rw-r--r--   0 root         (0) root         (0)     4807 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/awesomenotebook.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/bazimo.py
+-rw-r--r--   0 root         (0) root         (0)    11368 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/bobapp.py
+-rw-r--r--   0 root         (0) root         (0)      486 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/bubble.py
+-rw-r--r--   0 root         (0) root         (0)    11384 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/budgetinsight.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/canny.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/cityfalcon.py
+-rw-r--r--   0 root         (0) root         (0)     6342 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/email.py
+-rw-r--r--   0 root         (0) root         (0)    27214 2022-06-03 15:15:45.000000 naas-drivers-0.99.0/naas_drivers/tools/emailbuilder.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/ftp.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/geolocator.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/git.py
+-rw-r--r--   0 root         (0) root         (0)    30082 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/github.py
+-rw-r--r--   0 root         (0) root         (0)    16344 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/googleanalytics.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/gsheet.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/healthcheck.py
+-rw-r--r--   0 root         (0) root         (0)    16008 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/hubspot.py
+-rw-r--r--   0 root         (0) root         (0)    12384 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)      459 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/ifttt.py
+-rw-r--r--   0 root         (0) root         (0)      392 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/integromat.py
+-rw-r--r--   0 root         (0) root         (0)     7103 2022-06-03 15:15:46.000000 naas-drivers-0.99.0/naas_drivers/tools/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)    42902 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/linkedin.py
+-rw-r--r--   0 root         (0) root         (0)      590 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/markdown.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/mongo.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/naas_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/naas_credits.py
+-rw-r--r--   0 root         (0) root         (0)     2544 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/newsapi.py
+-rw-r--r--   0 root         (0) root         (0)    48996 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/notion.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/optimise.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/pdf.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/plotly.py
+-rw-r--r--   0 root         (0) root         (0)     8164 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/prediction.py
+-rw-r--r--   0 root         (0) root         (0)    21881 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/qonto.py
+-rw-r--r--   0 root         (0) root         (0)     2833 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/sentiment.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/sharepoint.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/slack.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/streamlit.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/taggun.py
+-rw-r--r--   0 root         (0) root         (0)      693 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/teams.py
+-rw-r--r--   0 root         (0) root         (0)     8137 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/thinkific.py
+-rw-r--r--   0 root         (0) root         (0)    21291 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/toucan.py
+-rw-r--r--   0 root         (0) root         (0)      198 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2777 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/yahoofinance.py
+-rw-r--r--   0 root         (0) root         (0)     9342 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/youtube.py
+-rw-r--r--   0 root         (0) root         (0)      388 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/naas_drivers/tools/zapier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-03 15:15:54.180730 naas-drivers-0.99.0/naas_drivers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3768 2022-06-03 15:15:54.000000 naas-drivers-0.99.0/naas_drivers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1794 2022-06-03 15:15:54.000000 naas-drivers-0.99.0/naas_drivers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-03 15:15:54.000000 naas-drivers-0.99.0/naas_drivers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     6236 2022-06-03 15:15:54.000000 naas-drivers-0.99.0/naas_drivers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-06-03 15:15:54.000000 naas-drivers-0.99.0/naas_drivers.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2022-06-03 15:15:54.188730 naas-drivers-0.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4335 2022-06-03 15:15:19.000000 naas-drivers-0.99.0/setup.py
```

### Comparing `naas-drivers-0.98.2/LICENSE` & `naas-drivers-0.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/PKG-INFO` & `naas-drivers-0.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naas-drivers
-Version: 0.98.2
+Version: 0.99.0
 Summary: Drivers made to easy connect to any services
 Home-page: https://github.com/jupyter-naas/drivers
 Author: Maxime Jublou
 Author-email: maxime@naas.ai
 License: BSD
 Description: ![Bump version](https://github.com/jupyter-naas/drivers/workflows/Bump%20version/badge.svg)
         ![GitHub license](https://img.shields.io/github/license/jupyter-naas/drivers)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naas-drivers Version: 0.98.2 Summary: Drivers made
+Metadata-Version: 2.1 Name: naas-drivers Version: 0.99.0 Summary: Drivers made
 to easy connect to any services Home-page: https://github.com/jupyter-naas/
 drivers Author: Maxime Jublou Author-email: maxime@naas.ai License: BSD
 Description: ![Bump version](https://github.com/jupyter-naas/drivers/workflows/
 Bump%20version/badge.svg) ![GitHub license](https://img.shields.io/github/
 license/jupyter-naas/drivers) ![Test Python package](https://github.com/
 jupyter-naas/drivers/workflows/Test%20Python%20package/badge.svg) ![Upload
 Python Package](https://github.com/jupyter-naas/drivers/workflows/
```

### Comparing `naas-drivers-0.98.2/README.md` & `naas-drivers-0.99.0/README.md`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/__init__.py` & `naas-drivers-0.99.0/naas_drivers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 import os
 from mprop import mproperty
 from subprocess import Popen, PIPE
 import sys
 
-__version__ = "0.98.2"
+__version__ = "0.99.0"
 
 __github_repo = "jupyter-naas/drivers"
 
 __doc_url = "https://naas.gitbook.io/drivers/"
 
 __loaded_drivers = {}
```

### Comparing `naas-drivers-0.98.2/naas_drivers/driver.py` & `naas-drivers-0.99.0/naas_drivers/driver.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/__crud.py` & `naas-drivers-0.99.0/naas_drivers/tools/__crud.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/__ftp.py` & `naas-drivers-0.99.0/naas_drivers/tools/__ftp.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/__ftps.py` & `naas-drivers-0.99.0/naas_drivers/tools/__ftps.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/airtable.py` & `naas-drivers-0.99.0/naas_drivers/tools/airtable.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/awesomenotebook.py` & `naas-drivers-0.99.0/naas_drivers/tools/awesomenotebook.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/bazimo.py` & `naas-drivers-0.99.0/naas_drivers/tools/bazimo.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/bobapp.py` & `naas-drivers-0.99.0/naas_drivers/tools/bobapp.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/budgetinsight.py` & `naas-drivers-0.99.0/naas_drivers/tools/budgetinsight.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/canny.py` & `naas-drivers-0.99.0/naas_drivers/tools/canny.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/cityfalcon.py` & `naas-drivers-0.99.0/naas_drivers/tools/cityfalcon.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/email.py` & `naas-drivers-0.99.0/naas_drivers/tools/email.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/emailbuilder.py` & `naas-drivers-0.99.0/naas_drivers/tools/emailbuilder.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/ftp.py` & `naas-drivers-0.99.0/naas_drivers/tools/ftp.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/geolocator.py` & `naas-drivers-0.99.0/naas_drivers/tools/geolocator.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/git.py` & `naas-drivers-0.99.0/naas_drivers/tools/git.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/github.py` & `naas-drivers-0.99.0/naas_drivers/tools/github.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/googleanalytics.py` & `naas-drivers-0.99.0/naas_drivers/tools/googleanalytics.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/gsheet.py` & `naas-drivers-0.99.0/naas_drivers/tools/gsheet.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/healthcheck.py` & `naas-drivers-0.99.0/naas_drivers/tools/healthcheck.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/hubspot.py` & `naas-drivers-0.99.0/naas_drivers/tools/hubspot.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/huggingface.py` & `naas-drivers-0.99.0/naas_drivers/tools/huggingface.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/jupyter.py` & `naas-drivers-0.99.0/naas_drivers/tools/jupyter.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,7 +217,17 @@
     def restart_user(self, username):
         self.check_connect()
         if self.is_user_active(username):
             user = self.get_user(username)
             user_options = user.get("servers").get("").get("user_options")
             self.stop_user(username)
             self.start_user(username, user_options)
+
+    def get_jobs(self, username):
+        self.check_connect()
+        try:
+            headers = {"Authorization": f"token {self.token}"}
+            url = f"https://app.naas.ai/user/{username}/proxy/5000/job"
+            res = requests.get(url, headers=headers)
+            return res.json()
+        except ValueError:
+            return []
```

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/linkedin.py` & `naas-drivers-0.99.0/naas_drivers/tools/linkedin.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/markdown.py` & `naas-drivers-0.99.0/naas_drivers/tools/markdown.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/mongo.py` & `naas-drivers-0.99.0/naas_drivers/tools/mongo.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/naas_auth.py` & `naas-drivers-0.99.0/naas_drivers/tools/naas_auth.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/naas_credits.py` & `naas-drivers-0.99.0/naas_drivers/tools/naas_credits.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/newsapi.py` & `naas-drivers-0.99.0/naas_drivers/tools/newsapi.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/notion.py` & `naas-drivers-0.99.0/naas_drivers/tools/notion.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/optimise.py` & `naas-drivers-0.99.0/naas_drivers/tools/optimise.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/pdf.py` & `naas-drivers-0.99.0/naas_drivers/tools/pdf.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/plotly.py` & `naas-drivers-0.99.0/naas_drivers/tools/plotly.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/prediction.py` & `naas-drivers-0.99.0/naas_drivers/tools/prediction.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/qonto.py` & `naas-drivers-0.99.0/naas_drivers/tools/qonto.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/sentiment.py` & `naas-drivers-0.99.0/naas_drivers/tools/sentiment.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/sharepoint.py` & `naas-drivers-0.99.0/naas_drivers/tools/sharepoint.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/slack.py` & `naas-drivers-0.99.0/naas_drivers/tools/slack.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/streamlit.py` & `naas-drivers-0.99.0/naas_drivers/tools/streamlit.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/taggun.py` & `naas-drivers-0.99.0/naas_drivers/tools/taggun.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/teams.py` & `naas-drivers-0.99.0/naas_drivers/tools/teams.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/thinkific.py` & `naas-drivers-0.99.0/naas_drivers/tools/thinkific.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/toucan.py` & `naas-drivers-0.99.0/naas_drivers/tools/toucan.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/yahoofinance.py` & `naas-drivers-0.99.0/naas_drivers/tools/yahoofinance.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers/tools/youtube.py` & `naas-drivers-0.99.0/naas_drivers/tools/youtube.py`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers.egg-info/PKG-INFO` & `naas-drivers-0.99.0/naas_drivers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naas-drivers
-Version: 0.98.2
+Version: 0.99.0
 Summary: Drivers made to easy connect to any services
 Home-page: https://github.com/jupyter-naas/drivers
 Author: Maxime Jublou
 Author-email: maxime@naas.ai
 License: BSD
 Description: ![Bump version](https://github.com/jupyter-naas/drivers/workflows/Bump%20version/badge.svg)
         ![GitHub license](https://img.shields.io/github/license/jupyter-naas/drivers)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naas-drivers Version: 0.98.2 Summary: Drivers made
+Metadata-Version: 2.1 Name: naas-drivers Version: 0.99.0 Summary: Drivers made
 to easy connect to any services Home-page: https://github.com/jupyter-naas/
 drivers Author: Maxime Jublou Author-email: maxime@naas.ai License: BSD
 Description: ![Bump version](https://github.com/jupyter-naas/drivers/workflows/
 Bump%20version/badge.svg) ![GitHub license](https://img.shields.io/github/
 license/jupyter-naas/drivers) ![Test Python package](https://github.com/
 jupyter-naas/drivers/workflows/Test%20Python%20package/badge.svg) ![Upload
 Python Package](https://github.com/jupyter-naas/drivers/workflows/
```

### Comparing `naas-drivers-0.98.2/naas_drivers.egg-info/SOURCES.txt` & `naas-drivers-0.99.0/naas_drivers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/naas_drivers.egg-info/requires.txt` & `naas-drivers-0.99.0/naas_drivers.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `naas-drivers-0.98.2/setup.py` & `naas-drivers-0.99.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 extras_require['full'] = [env for env in extras_require if env != 'dev' for env in extras_require[env]]
 extras_require['fulldev'] = [env for env in extras_require for env in extras_require[env]]
 extras_require['all'] = extras_require['full']
 
 setup(
     name="naas-drivers",
-    version="0.98.2",
+    version="0.99.0",
     author="Maxime Jublou",
     author_email="maxime@naas.ai",
     license="BSD",
     description="Drivers made to easy connect to any services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jupyter-naas/drivers",
```

