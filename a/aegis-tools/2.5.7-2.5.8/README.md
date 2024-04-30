# Comparing `tmp/aegis-tools-2.5.7.tar.gz` & `tmp/aegis-tools-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.5.7.tar", last modified: Mon Apr 22 18:30:08 2024, max compression
+gzip compressed data, was "aegis-tools-2.5.8.tar", last modified: Tue Apr 30 00:21:21 2024, max compression
```

## Comparing `aegis-tools-2.5.7.tar` & `aegis-tools-2.5.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-22 18:30:08.403842 aegis-tools-2.5.7/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-22 18:30:08.403842 aegis-tools-2.5.7/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-22 18:30:08.383842 aegis-tools-2.5.7/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20800 2024-03-21 19:10:22.000000 aegis-tools-2.5.7/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19045 2024-01-31 22:09:14.000000 aegis-tools-2.5.7/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.5.7/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    24750 2024-03-21 19:10:22.000000 aegis-tools-2.5.7/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27302 2024-04-22 18:29:41.000000 aegis-tools-2.5.7/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.5.7/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46086 2024-04-02 02:17:33.000000 aegis-tools-2.5.7/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-22 18:30:08.391842 aegis-tools-2.5.7/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.5.7/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.5.7/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.5.7/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.5.7/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.5.7/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    37012 2024-04-18 02:54:56.000000 aegis-tools-2.5.7/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-22 18:30:08.403842 aegis-tools-2.5.7/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.5.7/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.5.7/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.5.7/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.5.7/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.5.7/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.5.7/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.5.7/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.5.7/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.5.7/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.5.7/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.5.7/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.5.7/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.5.7/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.5.7/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78603 2024-04-02 02:17:33.000000 aegis-tools-2.5.7/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-22 18:30:08.403842 aegis-tools-2.5.7/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-22 18:30:08.000000 aegis-tools-2.5.7/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-04-22 18:30:08.000000 aegis-tools-2.5.7/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-04-22 18:30:08.000000 aegis-tools-2.5.7/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-04-22 18:30:08.000000 aegis-tools-2.5.7/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-04-22 18:30:08.000000 aegis-tools-2.5.7/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-04-22 18:30:08.000000 aegis-tools-2.5.7/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-04-22 18:30:08.403842 aegis-tools-2.5.7/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.5.7/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-30 00:21:21.197231 aegis-tools-2.5.8/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-30 00:21:21.197231 aegis-tools-2.5.8/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-30 00:21:21.185230 aegis-tools-2.5.8/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20802 2024-04-30 00:13:47.000000 aegis-tools-2.5.8/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19087 2024-04-30 00:19:28.000000 aegis-tools-2.5.8/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.5.8/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    24772 2024-04-30 00:13:47.000000 aegis-tools-2.5.8/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27302 2024-04-22 18:29:41.000000 aegis-tools-2.5.8/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.5.8/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46029 2024-04-30 00:13:47.000000 aegis-tools-2.5.8/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-30 00:21:21.189231 aegis-tools-2.5.8/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.5.8/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.5.8/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.5.8/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.5.8/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.5.8/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    37012 2024-04-18 02:54:56.000000 aegis-tools-2.5.8/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-30 00:21:21.193230 aegis-tools-2.5.8/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.5.8/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.5.8/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.5.8/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.5.8/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.5.8/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.5.8/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.5.8/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.5.8/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.5.8/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.5.8/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.5.8/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.5.8/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.5.8/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.5.8/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78528 2024-04-30 00:13:28.000000 aegis-tools-2.5.8/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-30 00:21:21.197231 aegis-tools-2.5.8/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-30 00:21:21.000000 aegis-tools-2.5.8/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-04-30 00:21:21.000000 aegis-tools-2.5.8/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-04-30 00:21:21.000000 aegis-tools-2.5.8/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-04-30 00:21:21.000000 aegis-tools-2.5.8/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-04-30 00:21:21.000000 aegis-tools-2.5.8/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-04-30 00:21:21.000000 aegis-tools-2.5.8/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-04-30 00:21:21.197231 aegis-tools-2.5.8/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.5.8/setup.py
```

### Comparing `aegis-tools-2.5.7/LICENSE` & `aegis-tools-2.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/PKG-INFO` & `aegis-tools-2.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.5.7
+Version: 2.5.8
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.5.7/README.md` & `aegis-tools-2.5.8/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/aegis_.py` & `aegis-tools-2.5.8/aegis/aegis_.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         logging.error("postgres=# CREATE DATABASE %s OWNER=%s;" % (options.pg_database, options.pg_username))
         exit(1)
     except aegis.database.MysqlOperationalError as ex:
         logging.error("Could not connect to database. Do you need to log into mysql and run:")
         logging.error("mysql> CREATE DATABASE %s" % (options.mysql_database))
         logging.error("mysql> USE %s" % (options.mysql_database))
         logging.error("mysql> CREATE USER '%s'@'%s' IDENTIFIED BY '%s'" % (options.mysql_username, '%', options.mysql_password))
-        logging.error("mysql> GRANT ALL PRIVILEGES ON %s TO '%s'@'%%'" % (options.mysql_database, options.mysql_username))
+        logging.error("mysql> GRANT ALL PRIVILEGES ON %s.* TO '%s'@'%%'" % (options.mysql_database, options.mysql_username))
         logging.error("mysql> FLUSH PRIVILEGES")
         exit(1)
 
     except Exception as ex:
         logging.error("Unknown Error Occurred")
         logging.exception(ex)
         exit(1)
```

### Comparing `aegis-tools-2.5.7/aegis/build.py` & `aegis-tools-2.5.8/aegis/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,17 +165,15 @@
         main_is_hydra = __main__.__file__.endswith('%s.py' % options.deploy_hydra_name)
         processes, stderr, exit_status = aegis.stdlib.shell("sudo /usr/bin/supervisorctl status")
         processes = [process.split(' ')[0] for process in processes.splitlines() if process.split(':')[0].endswith('_'+env) or process.split(':')[0].endswith('_'+env+'-admin')]
         num_procs = 1 if main_is_hydra else 0
         if len(processes) == num_procs:
             aegis.stdlib.loge(processes, "No processes ending with _%s to restart." % env)
         # Set up a set of <env>_prev-# to use with try_files in nginx
-
-        # XXX Make sure to only rotate admin if it's admin
-
+        # XXX Make sure to only rotate admin if it's admin   I can't remember what this comment means.
         prev_version = self.build_row['previous_version']
         if prev_version:
             for prev_num in range(1, 6):
                 link_file = os.path.join(app_dir, '%s_prev-%s' % (env, prev_num))
                 link_target = os.path.join(app_dir, prev_version)
                 if self._shell_exec("rm -f %s" % link_file, build_step=build_step, cwd=app_dir):
                     return
```

### Comparing `aegis-tools-2.5.7/aegis/config.py` & `aegis-tools-2.5.8/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/database.py` & `aegis-tools-2.5.8/aegis/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         # Autocommit==True we can cache the database connection and let autocommit handle cursor-transaction-safety
         pg_database = kwargs.get('pg_database') or options.pg_database
         if pg_database not in dbconns.databases[pid]:
             dbconns.databases[pid][pg_database] = PostgresConnection.connect(**kwargs)
         if not use_schema:
             use_schema = pg_database
     if mysql_available:
-        mysql_database = kwargs.get('mysql_database') or options.mysql_schema
+        mysql_database = kwargs.get('mysql_database') or options.mysql_database
         if mysql_database not in dbconns.databases[pid]:
             dbconns.databases[pid][mysql_database] = MysqlConnection.connect(**kwargs)
         if not use_schema:
             use_schema = mysql_database
     # Default situation - much better to be explicit which database we're connecting to!
     if not use_schema and len(dbconns.databases[pid]) == 1:
         use_schema = [dbconn for dbconn in dbconns.databases[pid].keys()][0]
@@ -322,35 +322,35 @@
         except Exception:
             logging.error("Cannot connect to MySQL on %s", self.hostname, exc_info=True)
 
     threads = {}
 
     @classmethod
     def connect(cls, **kwargs):
-        if 'mysql_schema' in kwargs:
+        if 'mysql_database' in kwargs:
             hostname = kwargs['mysql_hostname']
-            schema = kwargs['mysql_schema']
+            database = kwargs['mysql_database']
             user = kwargs['mysql_username']
             passwd = kwargs['mysql_password']
         else:
             hostname = options.mysql_hostname
-            schema = options.mysql_schema
+            database = options.mysql_database
             user = options.mysql_username
             passwd = options.mysql_password
         # force a new connection
         if kwargs.get('force', False):
-            return cls(hostname, schema, user, passwd)
+            return cls(hostname, database, user, passwd)
         # check existing connections
         ident = threading.current_thread().ident
-        target = '%s@%s' % (schema, hostname)
+        target = '%s@%s' % (database, hostname)
         connections = cls.threads.setdefault(ident, {})
         if not target in connections:
-            conn = cls(hostname, schema, user, passwd)
+            conn = cls(hostname, database, user, passwd)
             conn.execute("SET NAMES utf8mb4 COLLATE utf8mb4_unicode_ci", disable_audit_sql=True)
-            conn.schema = schema
+            conn.database = database
             cls.threads[ident][target] = conn
         #conn_debug = "%s %s %s" % (ident, target, connections)
         #aegis.stdlib.logw(conn_debug, "CONN DEBUG")
         return connections[target]
 
     def __del__(self):
         self.close()
```

### Comparing `aegis-tools-2.5.7/aegis/hydra.py` & `aegis-tools-2.5.8/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/mailer.py` & `aegis-tools-2.5.8/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/model.py` & `aegis-tools-2.5.8/aegis/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -936,53 +936,62 @@
 class Cache(aegis.database.Row):
     table_name = 'cache'
     id_column = 'cache_id'
 
     # External Interface for simplified usage
     @classmethod
     def get_cache(cls, cache_key):
-        cls.purge_expired()
         cache_obj = cls.get_key(cache_key)
         if cache_obj and type(cache_obj['cache_json']) is str:
             return json.loads(cache_obj['cache_json'])
         elif cache_obj:
             return cache_obj['cache_json']
 
     @classmethod
     def set_cache(cls, cache_key, cache_obj, duration_s):
         cache_json = json.dumps(cache_obj, cls=aegis.stdlib.DateTimeEncoder)
         cache_expiry = datetime.datetime.utcnow() + datetime.timedelta(seconds=duration_s) + datetime.timedelta(seconds=random.randint(0, duration_s))
         cache_id = cls.set_key(cache_key, cache_json, cache_expiry)
         return cls.get_cache(cache_key)
 
     @staticmethod
+    def del_star(cache_key):
+        cache_key = cache_key.replace('*', '%%')
+        sql = "DELETE FROM cache WHERE cache_key LIKE '" + cache_key + "'"
+        return db().execute_rowcount(sql)
+
+    @staticmethod
+    def del_key(cache_key):
+        sql = "DELETE FROM cache WHERE cache_key=%s"
+        return db().execute(sql, cache_key)
+
+    @staticmethod
     def purge_all():
         sql = "DELETE FROM cache"
         return db().execute(sql)
 
     # Internal Interface
     @staticmethod
     def insert(cache_key, cache_json, cache_expiry):
         sql = "INSERT INTO cache (cache_key, cache_json, cache_expiry) VALUES (%s, %s, %s)"
         if type(db()) is aegis.database.PostgresConnection:
             sql += ' RETURNING cache_id'
         try:
             return db().execute(sql, cache_key, cache_json, cache_expiry)
-        except aegis.database.PgsqlUniqueViolation as ex:
-            logging.warning("Ignoring duplicate key in cache")
-        except aegis.database.MysqlIntegrityError as ex:
+        except (aegis.database.MysqlIntegrityError, aegis.database.PgsqlUniqueViolation) as ex:
             logging.warning("Ignoring duplicate key in cache")
 
     @classmethod
     def get_key(cls, cache_key):
-        sql = "SELECT * FROM cache WHERE cache_key=%s"
+        sql = "SELECT * FROM cache WHERE cache_key=%s AND cache_expiry > NOW()"
         return db().get(sql, cache_key, cls=cls)
 
     @staticmethod
     def update_key(cache_key, cache_json, cache_expiry):
+        cls.purge_expired()
         sql = "UPDATE cache SET cache_json=%s, cache_expiry=%s WHERE cache_key=%s"
         return db().execute(sql, cache_json, cache_expiry, cache_key)
 
     @classmethod
     def set_key(cls, cache_key, cache_json, cache_expiry):
         cache_obj = cls.get_key(cache_key)
         if cache_obj:
@@ -990,25 +999,14 @@
             cache_obj = cls.get_key(cache_key)
         else:
             cls.insert(cache_key, cache_json, cache_expiry)
             cache_obj = cls.get_key(cache_key)
         return cache_obj
 
     @staticmethod
-    def del_star(cache_key):
-        cache_key = cache_key.replace('*', '%%')
-        sql = "DELETE FROM cache WHERE cache_key LIKE '" + cache_key + "'"
-        return db().execute_rowcount(sql)
-
-    @staticmethod
-    def del_key(cache_key):
-        sql = "DELETE FROM cache WHERE cache_key=%s"
-        return db().execute(sql, cache_key)
-
-    @staticmethod
     def purge_expired():
         sql = "DELETE FROM cache WHERE cache_expiry < NOW()"
         return db().execute(sql)
 
 
 class AuditSession(aegis.database.Row):
     table_name = 'audit_session'
```

### Comparing `aegis-tools-2.5.7/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.5.8/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.5.8/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/sql/build-mysql.sql` & `aegis-tools-2.5.8/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/sql/build-pgsql.sql` & `aegis-tools-2.5.8/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.5.8/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/sql/google_signin.sql` & `aegis-tools-2.5.8/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.5.8/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.5.8/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/sql/member_auth.sql` & `aegis-tools-2.5.8/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.5.8/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/sql/reports.sql` & `aegis-tools-2.5.8/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/stdlib.py` & `aegis-tools-2.5.8/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/build.html` & `aegis-tools-2.5.8/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/build_confirm.html` & `aegis-tools-2.5.8/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/build_form.html` & `aegis-tools-2.5.8/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/build_view.html` & `aegis-tools-2.5.8/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/frame.html` & `aegis-tools-2.5.8/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/hydra.html` & `aegis-tools-2.5.8/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/hydra_form.html` & `aegis-tools-2.5.8/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/hydra_queue.html` & `aegis-tools-2.5.8/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/report.html` & `aegis-tools-2.5.8/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/report_form.html` & `aegis-tools-2.5.8/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/reports.html` & `aegis-tools-2.5.8/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/templates/w3.css` & `aegis-tools-2.5.8/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/threadpool.py` & `aegis-tools-2.5.8/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/aegis/webapp.py` & `aegis-tools-2.5.8/aegis/webapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1169,15 +1169,14 @@
         self.tmpl['hydra_queues'] = aegis.model.HydraQueue.scan(dbconn=self.dbconn)
         # Sort by priority that will run, then by if the item is claimed
         self.tmpl['hydra_queues'] = sorted(self.tmpl['hydra_queues'], key=operator.itemgetter('priority_ndx'))
         self.tmpl['hydra_queues'] = sorted(self.tmpl['hydra_queues'], key=lambda x: x.get('claimed_dttm') is None)
         # If the queue item is running internally, sort it to the top
         for hydra_queue in self.tmpl['hydra_queues']:
             hydra_queue['_running'] = (hydra_queue['next_run_sql'] and hydra_queue['status'] == 'running') or (not hydra_queue['next_run_sql'] and hydra_queue['claimed_dttm'])
-            logging.warning("RUNNING: %s", hydra_queue['hydra_type_name'])
         self.tmpl['hydra_queues'] = sorted(self.tmpl['hydra_queues'], key=lambda x: x.get('_running') is True, reverse=True)
         return self.render_path("hydra_queue.html", **self.tmpl)
 
     @tornado.web.authenticated
     def post(self, *args):
         self.enforce_admin()
         run_ids = [aegis.stdlib.validate_int(k.replace('run_', '')) for k in self.request.args.keys() if k.startswith('run_')]
```

### Comparing `aegis-tools-2.5.7/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.5.8/aegis_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.5.7
+Version: 2.5.8
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.5.7/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.5.8/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.7/setup.py` & `aegis-tools-2.5.8/setup.py`

 * *Files identical despite different names*

