# Comparing `tmp/teamvault-0.9.2.tar.gz` & `tmp/teamvault-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamvault-0.9.2.tar", last modified: Mon Feb  8 12:56:45 2021, max compression
+gzip compressed data, was "teamvault-1.0.0rc3.tar", last modified: Tue Apr 30 11:49:15 2024, max compression
```

## Comparing `teamvault-0.9.2.tar` & `teamvault-1.0.0rc3.tar`

### file list

```diff
@@ -1,394 +1,244 @@
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.097219 teamvault-0.9.2/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3609 2021-02-08 12:54:08.000000 teamvault-0.9.2/CHANGELOG.md
--rw-r--r--   0 trehn     (1000) trehn     (1000)    35392 2019-10-23 08:34:39.000000 teamvault-0.9.2/LICENSE
--rw-r--r--   0 trehn     (1000) trehn     (1000)      356 2019-10-23 08:34:39.000000 teamvault-0.9.2/MANIFEST.in
--rw-r--r--   0 trehn     (1000) trehn     (1000)      742 2021-02-08 12:56:45.097219 teamvault-0.9.2/PKG-INFO
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1074 2019-10-23 08:34:39.000000 teamvault-0.9.2/README.md
--rw-r--r--   0 trehn     (1000) trehn     (1000)       70 2021-02-08 12:56:45.097219 teamvault-0.9.2/setup.cfg
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2912 2021-02-08 12:54:16.000000 teamvault-0.9.2/setup.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.007224 teamvault-0.9.2/teamvault/
--rw-r--r--   0 trehn     (1000) trehn     (1000)       73 2021-02-08 12:54:46.000000 teamvault-0.9.2/teamvault/__init__.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.007224 teamvault-0.9.2/teamvault/apps/
--rw-r--r--   0 trehn     (1000) trehn     (1000)        0 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/__init__.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.007224 teamvault-0.9.2/teamvault/apps/accounts/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      106 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/accounts/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      221 2021-01-29 10:24:24.000000 teamvault-0.9.2/teamvault/apps/accounts/auth.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      134 2021-01-28 15:17:40.000000 teamvault-0.9.2/teamvault/apps/accounts/context_processors.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.000558 teamvault-0.9.2/teamvault/apps/accounts/templates/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.007224 teamvault-0.9.2/teamvault/apps/accounts/templates/accounts/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1261 2021-02-08 12:51:37.000000 teamvault-0.9.2/teamvault/apps/accounts/templates/accounts/login.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)      454 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/apps/accounts/templates/accounts/logout.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3588 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/accounts/templates/accounts/user_detail.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2466 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/accounts/templates/accounts/user_list.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1115 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/accounts/urls.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3808 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/accounts/views.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.010557 teamvault-0.9.2/teamvault/apps/audit/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      100 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/audit/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      845 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/audit/admin.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      464 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/audit/auditlog.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.010557 teamvault-0.9.2/teamvault/apps/audit/migrations/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1588 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/audit/migrations/0001_initial.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1686 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/audit/migrations/0002_auto_20170313_1544.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)        0 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/audit/migrations/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1100 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/audit/models.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.000558 teamvault-0.9.2/teamvault/apps/audit/templates/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.010557 teamvault-0.9.2/teamvault/apps/audit/templates/audit/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1094 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/apps/audit/templates/audit/log.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)      158 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/audit/urls.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1503 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/audit/views.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.013890 teamvault-0.9.2/teamvault/apps/secrets/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      104 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2477 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/admin.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    14114 2021-01-28 09:00:05.000000 teamvault-0.9.2/teamvault/apps/secrets/api.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      938 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/api_urls.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      440 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/context_processors.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)       43 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/exceptions.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3384 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/forms.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.013890 teamvault-0.9.2/teamvault/apps/secrets/management/
--rw-r--r--   0 trehn     (1000) trehn     (1000)        0 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/management/__init__.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.013890 teamvault-0.9.2/teamvault/apps/secrets/management/commands/
--rw-r--r--   0 trehn     (1000) trehn     (1000)        0 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/management/commands/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      759 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/management/commands/update_search_index.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.017223 teamvault-0.9.2/teamvault/apps/secrets/migrations/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4810 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0001_initial.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      450 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0002_secret_filename.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      690 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0003_auto_20150113_1915.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      333 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0004_unaccent_extension.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      454 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0005_secret_search_index.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      382 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0006_auto_20150124_1103.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      517 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0007_auto_20150205_1918.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      789 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0008_auto_20150322_0944.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1417 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0009_auto_20150322_0949.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      399 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0011_remove_secret_search_index.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      533 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0012_secret_search_index.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      885 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0013_auto_20161021_1411.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2169 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0014_auto_20170313_1544.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      462 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0015_secretrevision_plaintext_data_sha256.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      766 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0016_auto_20180220_1053.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1308 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0017_auto_20180220_1115.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      502 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0018_auto_20180220_1244.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      578 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0019_secret_notify_on_access_request.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      752 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0020_auto_20180220_1356.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      440 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0021_auto_20180220_1428.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      498 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0022_secret_last_changed.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      713 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/0023_auto_20190822_1234.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)        0 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/migrations/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    22444 2020-11-12 14:23:29.000000 teamvault-0.9.2/teamvault/apps/secrets/models.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.000558 teamvault-0.9.2/teamvault/apps/secrets/static/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.017223 teamvault-0.9.2/teamvault/apps/secrets/static/css/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2753 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/static/css/secrets.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.017223 teamvault-0.9.2/teamvault/apps/secrets/templates/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      338 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/opensearch.xml
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.020556 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3117 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/accessrequest_detail.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1923 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/accessrequest_list.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)      910 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/dashboard.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)      151 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/mail_access_request_approved.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)      205 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/mail_access_request_denied.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)      226 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/mail_access_request_review.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)    12077 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/secret_addedit.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3309 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/secret_addedit_cc.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1332 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/secret_addedit_file.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2318 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/secret_addedit_password.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1282 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/secret_delete.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)    15094 2021-01-29 11:18:13.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/secret_detail.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)      946 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/secret_list.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1175 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/secret_restore.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1039 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/secret_row.html
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.020556 teamvault-0.9.2/teamvault/apps/secrets/templatetags/
--rw-r--r--   0 trehn     (1000) trehn     (1000)        0 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/templatetags/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      848 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/templatetags/smart_pagination.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1826 2021-01-28 10:56:31.000000 teamvault-0.9.2/teamvault/apps/secrets/urls.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      783 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/secrets/utils.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    17881 2021-01-28 10:56:48.000000 teamvault-0.9.2/teamvault/apps/secrets/views.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.020556 teamvault-0.9.2/teamvault/apps/settings/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      618 2021-01-28 14:47:38.000000 teamvault-0.9.2/teamvault/apps/settings/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      351 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/settings/admin.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    13134 2021-01-29 10:28:27.000000 teamvault-0.9.2/teamvault/apps/settings/config.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.020556 teamvault-0.9.2/teamvault/apps/settings/migrations/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      630 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/settings/migrations/0001_initial.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)        0 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/settings/migrations/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      857 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/apps/settings/models.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3230 2020-11-12 14:23:29.000000 teamvault-0.9.2/teamvault/cli.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3883 2021-01-28 15:18:01.000000 teamvault-0.9.2/teamvault/settings.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static/bundled/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.023889 teamvault-0.9.2/teamvault/static/bundled/bigtext/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      528 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bigtext/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1055 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bigtext/LICENSE
--rw-r--r--   0 trehn     (1000) trehn     (1000)      209 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bigtext/bower.json
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.023889 teamvault-0.9.2/teamvault/static/bundled/bigtext/dist/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     9459 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bigtext/dist/bigtext.js
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.023889 teamvault-0.9.2/teamvault/static/bundled/bootstrap/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      923 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1085 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/LICENSE
--rw-r--r--   0 trehn     (1000) trehn     (1000)      643 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/bower.json
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.030556 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/css/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    25682 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/css/bootstrap-theme.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    48005 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/css/bootstrap-theme.css.map
--rw-r--r--   0 trehn     (1000) trehn     (1000)    23411 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/css/bootstrap-theme.min.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    75600 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/css/bootstrap-theme.min.css.map
--rw-r--r--   0 trehn     (1000) trehn     (1000)   145933 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)   390887 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0 trehn     (1000) trehn     (1000)   121457 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)   540434 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.037222 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/fonts/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    20127 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 trehn     (1000) trehn     (1000)   108738 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 trehn     (1000) trehn     (1000)    45404 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 trehn     (1000) trehn     (1000)    23424 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 trehn     (1000) trehn     (1000)    18028 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.037222 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/js/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    75484 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    39680 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      484 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/dist/js/npm.js
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.037222 teamvault-0.9.2/teamvault/static/bundled/bootstrap/nuget/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      471 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/nuget/MyGet.ps1
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1507 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/nuget/bootstrap.less.nuspec
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1470 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/bootstrap/nuget/bootstrap.nuspec
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.037222 teamvault-0.9.2/teamvault/static/bundled/card/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      823 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/card/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1056 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/card/LICENSE
--rw-r--r--   0 trehn     (1000) trehn     (1000)      568 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/card/bower.json
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.040555 teamvault-0.9.2/teamvault/static/bundled/card/dist/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    24727 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/card/dist/card.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    99205 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/card/dist/card.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)   100307 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/card/dist/jquery.card.js
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.040555 teamvault-0.9.2/teamvault/static/bundled/clipboard/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      684 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/clipboard/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)      358 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/clipboard/bower.json
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.040555 teamvault-0.9.2/teamvault/static/bundled/clipboard/dist/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    24977 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/clipboard/dist/clipboard.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    10917 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/clipboard/dist/clipboard.min.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     7936 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/clipboard/readme.md
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.040555 teamvault-0.9.2/teamvault/static/bundled/font-awesome/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      712 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)      403 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/bower.json
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.040555 teamvault-0.9.2/teamvault/static/bundled/font-awesome/css/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    37414 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/css/font-awesome.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    21778 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/css/font-awesome.css.map
--rw-r--r--   0 trehn     (1000) trehn     (1000)    31000 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.047222 teamvault-0.9.2/teamvault/static/bundled/font-awesome/fonts/
--rw-r--r--   0 trehn     (1000) trehn     (1000)   134808 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 trehn     (1000) trehn     (1000)   165742 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 trehn     (1000) trehn     (1000)   444379 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 trehn     (1000) trehn     (1000)   165548 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 trehn     (1000) trehn     (1000)    98024 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 trehn     (1000) trehn     (1000)    77160 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.047222 teamvault-0.9.2/teamvault/static/bundled/jquery/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      526 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1095 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/LICENSE.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)      190 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/bower.json
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.050555 teamvault-0.9.2/teamvault/static/bundled/jquery/dist/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     9165 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/dist/core.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)   280364 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/dist/jquery.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    88145 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/dist/jquery.min.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)   227022 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/dist/jquery.slim.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    71037 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/dist/jquery.slim.min.js
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static/bundled/jquery/external/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.050555 teamvault-0.9.2/teamvault/static/bundled/jquery/external/sizzle/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1605 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/external/sizzle/LICENSE.txt
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.050555 teamvault-0.9.2/teamvault/static/bundled/jquery/external/sizzle/dist/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    65666 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/external/sizzle/dist/sizzle.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    19841 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/external/sizzle/dist/sizzle.min.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    30740 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/jquery/external/sizzle/dist/sizzle.min.map
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.053888 teamvault-0.9.2/teamvault/static/bundled/password-generator/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      831 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/password-generator/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)       29 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/password-generator/.gitattributes
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1061 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/password-generator/LICENSE
--rw-r--r--   0 trehn     (1000) trehn     (1000)      494 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/password-generator/bower.json
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.053888 teamvault-0.9.2/teamvault/static/bundled/password-generator/dist/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1452 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/password-generator/dist/password-generator.min.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      274 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/password-generator/index.d.ts
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.067220 teamvault-0.9.2/teamvault/static/bundled/select2/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      528 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)      938 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/LICENSE
--rw-r--r--   0 trehn     (1000) trehn     (1000)      206 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1732 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/component.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)      637 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/composer.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3347 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2-bootstrap.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1849 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2-spinner.gif
--rw-r--r--   0 trehn     (1000) trehn     (1000)    19223 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1030 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2.jquery.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)   156367 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    70142 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2.min.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      613 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2.png
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1389 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_ar.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1003 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_az.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1081 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_bg.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      952 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_ca.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1988 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_cs.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      853 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_da.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1014 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_de.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1128 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_el.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1102 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_en.js.template
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1177 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_es.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      886 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_et.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1313 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_eu.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1207 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_fa.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      940 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_fi.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1077 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_fr.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1339 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_gl.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      885 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_he.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1002 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_hr.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      802 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_hu.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1111 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_id.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      855 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_is.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      866 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_it.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      812 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_ja.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1078 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_ka.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      871 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_ko.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1144 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_lt.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      999 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_lv.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1064 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_mk.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1122 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_ms.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1145 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_nb.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      846 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_nl.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2015 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_pl.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      969 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_pt-BR.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      891 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_pt-PT.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      902 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_ro.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1058 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_rs.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1171 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_ru.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1948 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_sk.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      847 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_sv.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1063 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_th.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1070 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_tr.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      904 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_ug-CN.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1415 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_uk.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      910 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_vi.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      762 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_zh-CN.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      774 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2_locale_zh-TW.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)      845 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2/select2x2.png
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.067220 teamvault-0.9.2/teamvault/static/bundled/select2-bootstrap/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      596 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2-bootstrap/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1076 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2-bootstrap/LICENSE
--rw-r--r--   0 trehn     (1000) trehn     (1000)      245 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2-bootstrap/bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)    14948 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/select2-bootstrap/select2-bootstrap.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.070553 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      575 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1061 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/LICENSE
--rw-r--r--   0 trehn     (1000) trehn     (1000)      247 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/bower.json
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.070553 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/dist/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    33197 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/dist/bloodhound.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    12998 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/dist/bloodhound.min.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    96186 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/dist/typeahead.bundle.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    39749 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/dist/typeahead.bundle.min.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    63136 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/dist/typeahead.jquery.js
--rw-r--r--   0 trehn     (1000) trehn     (1000)    26900 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/typeahead.js/dist/typeahead.jquery.min.js
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.073886 teamvault-0.9.2/teamvault/static/bundled/underscore/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      663 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/underscore/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1117 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/underscore/LICENSE
--rw-r--r--   0 trehn     (1000) trehn     (1000)      253 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/underscore/bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)    18069 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/underscore/underscore-min.js
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.073886 teamvault-0.9.2/teamvault/static/bundled/zxcvbn/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      843 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/zxcvbn/.bower.json
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1078 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/zxcvbn/LICENSE.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)      629 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/zxcvbn/bower.json
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.073886 teamvault-0.9.2/teamvault/static/bundled/zxcvbn/dist/
--rw-r--r--   0 trehn     (1000) trehn     (1000)   821711 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/bundled/zxcvbn/dist/zxcvbn.js
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.073886 teamvault-0.9.2/teamvault/static/css/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1230 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/css/base.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4074 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/css/bootstrap-overrides.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1074 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/css/login.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)      763 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/static/css/typeaheadjs.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static_collected/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static_collected/bundled/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/dist/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.077220 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/dist/css/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    25682 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/dist/css/bootstrap-theme.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    25682 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/dist/css/bootstrap-theme.da9549a015c0.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    23411 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/dist/css/bootstrap-theme.min.2010fa9fb075.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    23411 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/dist/css/bootstrap-theme.min.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)   146011 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/dist/css/bootstrap.aefedc37294b.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)   145933 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)   121457 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)   121547 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/bootstrap/dist/css/bootstrap.min.eb2644c7646f.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static_collected/bundled/card/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.077220 teamvault-0.9.2/teamvault/static_collected/bundled/card/dist/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    24727 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/card/dist/card.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    24727 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/card/dist/card.ff5468b42eb8.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static_collected/bundled/font-awesome/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.080553 teamvault-0.9.2/teamvault/static_collected/bundled/font-awesome/css/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    37492 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/font-awesome/css/font-awesome.7d46203b9170.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    37414 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/font-awesome/css/font-awesome.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    31078 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/font-awesome/css/font-awesome.min.bf0c425cdb73.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    31000 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.080553 teamvault-0.9.2/teamvault/static_collected/bundled/jquery/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1095 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/jquery/LICENSE.75308107741f.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1095 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/jquery/LICENSE.txt
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static_collected/bundled/jquery/external/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.080553 teamvault-0.9.2/teamvault/static_collected/bundled/jquery/external/sizzle/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1605 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/jquery/external/sizzle/LICENSE.18d9b3a646e7.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1605 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/jquery/external/sizzle/LICENSE.txt
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.080553 teamvault-0.9.2/teamvault/static_collected/bundled/select2/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3347 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/select2/select2-bootstrap.0fe870dbba4c.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3347 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/select2/select2-bootstrap.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    19496 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/select2/select2.1af95fa49767.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    19223 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/select2/select2.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.080553 teamvault-0.9.2/teamvault/static_collected/bundled/select2-bootstrap/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    14948 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/select2-bootstrap/select2-bootstrap.9814432aefab.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    14948 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/select2-bootstrap/select2-bootstrap.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.083886 teamvault-0.9.2/teamvault/static_collected/bundled/zxcvbn/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1078 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/zxcvbn/LICENSE.a890445e0f8a.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1078 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/bundled/zxcvbn/LICENSE.txt
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.083886 teamvault-0.9.2/teamvault/static_collected/css/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1230 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/css/base.7477f9f40f4b.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1230 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/css/base.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4074 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/css/bootstrap-overrides.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4074 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/css/bootstrap-overrides.e93416adfc37.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1074 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/css/login.b8b9030d821b.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1074 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/css/login.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2753 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/css/secrets.62953799ac9d.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2753 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/css/secrets.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)      763 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/css/typeaheadjs.04969a09b6b8.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)      763 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/css/typeaheadjs.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static_collected/rest_framework/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.087219 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    23411 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/bootstrap-theme.min.66b84a04375e.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    23411 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/bootstrap-theme.min.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3398 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3385 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/bootstrap-tweaks.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)   121547 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/bootstrap.min.77017a69879a.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)   121457 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/bootstrap.min.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1131 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/default.8d5591a6aabc.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1131 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/default.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    21723 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)    21658 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/font-awesome-4.0.3.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)      817 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/prettify.a987f72342ee.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)      817 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/css/prettify.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.003891 teamvault-0.9.2/teamvault/static_collected/rest_framework/docs/
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.090552 teamvault-0.9.2/teamvault/static_collected/rest_framework/docs/css/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     6147 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/docs/css/base.3208b6cc4466.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     6147 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/docs/css/base.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1682 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/docs/css/highlight.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1682 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/docs/css/highlight.e0e4d973c6d7.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1307 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1307 2021-01-28 15:13:22.000000 teamvault-0.9.2/teamvault/static_collected/rest_framework/docs/css/jquery.json-view.min.css
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.093885 teamvault-0.9.2/teamvault/templates/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      538 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/templates/404_anon.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)      548 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/templates/404_loggedin.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1978 2021-01-28 09:22:36.000000 teamvault-0.9.2/teamvault/templates/base.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4873 2021-01-28 09:23:07.000000 teamvault-0.9.2/teamvault/templates/base_nav.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)      896 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/templates/pagination.html
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.093885 teamvault-0.9.2/teamvault/templates/rest_framework/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      279 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/templates/rest_framework/api.html
--rw-r--r--   0 trehn     (1000) trehn     (1000)      542 2021-01-28 14:49:48.000000 teamvault-0.9.2/teamvault/urls.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      882 2020-11-12 14:23:29.000000 teamvault-0.9.2/teamvault/utils.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      256 2019-10-23 08:34:39.000000 teamvault-0.9.2/teamvault/views.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      247 2021-01-28 10:52:37.000000 teamvault-0.9.2/teamvault/wsgi.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.007224 teamvault-0.9.2/teamvault.egg-info/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      742 2021-02-08 12:56:44.000000 teamvault-0.9.2/teamvault.egg-info/PKG-INFO
--rw-r--r--   0 trehn     (1000) trehn     (1000)    16730 2021-02-08 12:56:44.000000 teamvault-0.9.2/teamvault.egg-info/SOURCES.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)        1 2021-02-08 12:56:44.000000 teamvault-0.9.2/teamvault.egg-info/dependency_links.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)       50 2021-02-08 12:56:44.000000 teamvault-0.9.2/teamvault.egg-info/entry_points.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)        1 2020-11-13 08:31:25.000000 teamvault-0.9.2/teamvault.egg-info/not-zip-safe
--rw-r--r--   0 trehn     (1000) trehn     (1000)      929 2021-02-08 12:56:44.000000 teamvault-0.9.2/teamvault.egg-info/requires.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)       16 2021-02-08 12:56:44.000000 teamvault-0.9.2/teamvault.egg-info/top_level.txt
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.097219 teamvault-0.9.2/tests/
--rw-r--r--   0 trehn     (1000) trehn     (1000)        0 2019-10-23 08:34:39.000000 teamvault-0.9.2/tests/__init__.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-02-08 12:56:45.097219 teamvault-0.9.2/tests/teamvault/
--rw-r--r--   0 trehn     (1000) trehn     (1000)        0 2019-10-23 08:34:39.000000 teamvault-0.9.2/tests/teamvault/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      147 2019-10-23 08:34:39.000000 teamvault-0.9.2/tests/teamvault/cli_tests.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.645343 teamvault-1.0.0rc3/
+-rw-r--r--   0 mre       (1000) mre       (1000)     3609 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/CHANGELOG.md
+-rw-r--r--   0 mre       (1000) mre       (1000)    35392 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/LICENSE
+-rw-r--r--   0 mre       (1000) mre       (1000)      374 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/MANIFEST.in
+-rw-r--r--   0 mre       (1000) mre       (1000)    44508 2024-04-30 11:49:15.645343 teamvault-1.0.0rc3/PKG-INFO
+-rw-r--r--   0 mre       (1000) mre       (1000)     2182 2024-04-30 11:19:22.000000 teamvault-1.0.0rc3/README.md
+-rw-r--r--   0 mre       (1000) mre       (1000)     1800 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/pyproject.toml
+-rw-r--r--   0 mre       (1000) mre       (1000)       38 2024-04-30 11:49:15.645343 teamvault-1.0.0rc3/setup.cfg
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/
+-rw-r--r--   0 mre       (1000) mre       (1000)       46 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)       25 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/__version__.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/
+-rw-r--r--   0 mre       (1000) mre       (1000)        0 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/__init__.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/accounts/
+-rw-r--r--   0 mre       (1000) mre       (1000)      106 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1258 2024-04-15 09:53:21.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/auth.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      134 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/context_processors.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      440 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/forms.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/accounts/migrations/
+-rw-r--r--   0 mre       (1000) mre       (1000)      488 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/migrations/0001_initial.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1583 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/migrations/0002_add_user_settings.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      399 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/migrations/0003_usersettings_avatar.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      546 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/migrations/0004_alter_usersettings_hide_deleted_secrets.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      521 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/migrations/0005_rename_usersettings_userprofile.py
+-rw-r--r--   0 mre       (1000) mre       (1000)        0 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/migrations/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1169 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/models.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/accounts/templates/
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/accounts/templates/accounts/
+-rw-r--r--   0 mre       (1000) mre       (1000)     1053 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/templates/accounts/_avatar.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     2006 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/templates/accounts/login.html
+-rw-r--r--   0 mre       (1000) mre       (1000)      746 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/templates/accounts/logout.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     5780 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/templates/accounts/user_detail.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     2387 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/templates/accounts/user_list.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     1141 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/templates/accounts/user_settings.html
+-rw-r--r--   0 mre       (1000) mre       (1000)      994 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/urls.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     3405 2024-04-15 10:47:04.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/utils.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     4021 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/accounts/views.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/audit/
+-rw-r--r--   0 mre       (1000) mre       (1000)      100 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/audit/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      555 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/audit/auditlog.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      999 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/audit/filters.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/audit/migrations/
+-rw-r--r--   0 mre       (1000) mre       (1000)     1588 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/audit/migrations/0001_initial.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1686 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/audit/migrations/0002_auto_20170313_1544.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     2637 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/audit/migrations/0003_logentry_categories.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1489 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/audit/migrations/0004_alter_logentry_category.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     2236 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/audit/migrations/0005_alter_logentry_category.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1479 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/audit/migrations/0006_logentry_reason.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1587 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/audit/migrations/0007_alter_logentry_category.py
+-rw-r--r--   0 mre       (1000) mre       (1000)        0 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/audit/migrations/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     2688 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/audit/models.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/audit/templates/
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/audit/templates/audit/
+-rw-r--r--   0 mre       (1000) mre       (1000)     4169 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/audit/templates/audit/log.html
+-rw-r--r--   0 mre       (1000) mre       (1000)      152 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/audit/urls.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1338 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/audit/views.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/secrets/
+-rw-r--r--   0 mre       (1000) mre       (1000)      104 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/__init__.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/secrets/api/
+-rw-r--r--   0 mre       (1000) mre       (1000)        0 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/api/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     9269 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/api/serializers.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1045 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/api/urls.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     6093 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/api/views.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      106 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/context_processors.py
+-rw-r--r--   0 mre       (1000) mre       (1000)       43 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/exceptions.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      371 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/filters.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     5059 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/forms.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/secrets/management/
+-rw-r--r--   0 mre       (1000) mre       (1000)        0 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/management/__init__.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/apps/secrets/management/commands/
+-rw-r--r--   0 mre       (1000) mre       (1000)        0 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/management/commands/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      734 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/management/commands/update_search_index.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/
+-rw-r--r--   0 mre       (1000) mre       (1000)     4810 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0001_initial.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      450 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0002_secret_filename.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      690 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0003_auto_20150113_1915.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      333 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0004_unaccent_extension.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      454 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0005_secret_search_index.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      382 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0006_auto_20150124_1103.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      517 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0007_auto_20150205_1918.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      789 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0008_auto_20150322_0944.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1417 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0009_auto_20150322_0949.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      399 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0011_remove_secret_search_index.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      533 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0012_secret_search_index.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      885 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0013_auto_20161021_1411.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     2169 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0014_auto_20170313_1544.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      462 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0015_secretrevision_plaintext_data_sha256.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      766 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0016_auto_20180220_1053.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1308 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0017_auto_20180220_1115.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      502 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0018_auto_20180220_1244.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      578 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0019_secret_notify_on_access_request.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      752 2023-05-25 16:15:10.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0020_auto_20180220_1356.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      440 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0021_auto_20180220_1428.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      498 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0022_secret_last_changed.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      713 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0023_auto_20190822_1234.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      666 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0024_auto_20210824_1203.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      705 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0025_alter_secret_description_alter_secret_name.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     2817 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0026_allowed_groups_users_intermediate.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      682 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0027_sharedsecretdata_only_one_set.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      591 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0028_sharedsecretdata_grant_description_and_more.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      723 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0029_sharedsecretdata_granted_by.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      425 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0030_sharedsecretdata_granted_on.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     2506 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0031_rename_share_data_fields.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      706 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0032_alter_sharedsecretdata_granted_by.py
+-rw-r--r--   0 mre       (1000) mre       (1000)        0 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)    21633 2024-04-30 11:14:32.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/models.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     2600 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/tasks.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/
+-rw-r--r--   0 mre       (1000) mre       (1000)      338 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/opensearch.xml
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/addedit_content/
+-rw-r--r--   0 mre       (1000) mre       (1000)     4164 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/addedit_content/cc.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     2102 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/addedit_content/file.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     4114 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/addedit_content/password.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     1848 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/dashboard.html
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/detail_content/
+-rw-r--r--   0 mre       (1000) mre       (1000)     4044 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/detail_content/_js.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     1928 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/detail_content/_su_confirm_modal.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     7475 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/detail_content/cc.html
+-rw-r--r--   0 mre       (1000) mre       (1000)      950 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/detail_content/file.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     2710 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/detail_content/meta.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     5361 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/detail_content/password.html
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/search/
+-rw-r--r--   0 mre       (1000) mre       (1000)      684 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/search/_search_item.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     8688 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/secret_addedit.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     1256 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/secret_delete.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     6006 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/secret_detail.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     8683 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/secret_list.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     1428 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/secret_restore.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     1447 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/secret_row.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     8463 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/secret_search.html
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/share_content/
+-rw-r--r--   0 mre       (1000) mre       (1000)     5641 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/share_content/_share_list_entry.html
+-rw-r--r--   0 mre       (1000) mre       (1000)    10992 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/share_content/share_list_modal.html
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/secrets/templatetags/
+-rw-r--r--   0 mre       (1000) mre       (1000)        0 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templatetags/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1078 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/templatetags/smart_pagination.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/secrets/tests/
+-rw-r--r--   0 mre       (1000) mre       (1000)        0 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/tests/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1259 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/tests/test_model_consistency.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1602 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/urls.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1410 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/utils.py
+-rw-r--r--   0 mre       (1000) mre       (1000)    21149 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/apps/secrets/views.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/settings/
+-rw-r--r--   0 mre       (1000) mre       (1000)      924 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/settings/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)    17963 2024-04-15 09:53:33.000000 teamvault-1.0.0rc3/teamvault/apps/settings/config.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.635343 teamvault-1.0.0rc3/teamvault/apps/settings/migrations/
+-rw-r--r--   0 mre       (1000) mre       (1000)      630 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/settings/migrations/0001_initial.py
+-rw-r--r--   0 mre       (1000) mre       (1000)        0 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/apps/settings/migrations/__init__.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      856 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/settings/models.py
+-rw-r--r--   0 mre       (1000) mre       (1000)      501 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/apps/settings/webpack.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     3950 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/cli.py
+-rwxr-xr-x   0 mre       (1000) mre       (1000)      361 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/manage.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     1158 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/middleware.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     4378 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/settings.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.625343 teamvault-1.0.0rc3/teamvault/static/
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.645343 teamvault-1.0.0rc3/teamvault/static/bundled/
+-rw-r--r--   0 mre       (1000) mre       (1000)    52912 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/0e11b62db931f85340d4.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    52184 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/0ea53bd19b062bb4b1a0.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10532 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/1458587c0aa7cd06b82b.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    51784 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/1be936c894a0d2538aec.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10372 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/1df741eb9a4ccdba01d2.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10496 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/1ece20ed1ce14a31dc9e.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    25392 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/21cb8f55d8e0c5b89751.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)    36096 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/267b2500600d0f79e1dc.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)    39324 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/3343afa6b8c01e48a23b.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)    39148 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/349ed9fa39221b45ae9a.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)    10496 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/3555e897caceedb85c78.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    39224 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/36828c2aa518db3d9dfe.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)    10520 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/4404b6f14866b5181b22.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)   117852 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/455ea818179b4def0c43.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)   419720 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/45a265d0f07b31cde85f.ttf
+-rw-r--r--   0 mre       (1000) mre       (1000)    38100 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/45b1694298986e76152b.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)   156400 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/4d986b00ff9ca3828fbd.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)    10180 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/5165a96db616b820c773.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10180 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/575edee732e02309b47e.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    38964 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/5e8f879de58d6f900998.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)   209128 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/60127e352b7a11f7f1bc.ttf
+-rw-r--r--   0 mre       (1000) mre       (1000)   207972 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/6205fd00fb1b573e9f0f.ttf
+-rw-r--r--   0 mre       (1000) mre       (1000)    52764 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/62378484038222d8dcb8.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    39564 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/64d5f06ee726edd58ca3.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)    49300 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/6bec2374043867d07479.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10604 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/70e04c856f46aa529052.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    50708 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/740ce50b50dd0c553a92.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    39476 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/8236e953c7367362a568.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)   117372 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/8d3cabfc66809162fb4d.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)    10040 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/9432de654f2ae9e9bc21.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10432 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/9cfbb32450c2f97b3722.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10044 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/aa8b1b55c728cb4221da.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    68004 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/adc51aab4d771ab65f81.ttf
+-rw-r--r--   0 mre       (1000) mre       (1000)    52500 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/ae9c1f88ace17d23e8e6.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)   420332 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/bacd5de623fb563b961a.ttf
+-rw-r--r--   0 mre       (1000) mre       (1000)    10600 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/c0dcdaeaab8caa158cb9.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    52836 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/c5eb8fb453e49d29b817.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10436 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/c85b4172ef8cea3d563d.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10432 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/cd04c2ad00870c9ceebf.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10528 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/cda9c93f49237f11c766.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10432 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/e67a6d49530694caae42.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    10524 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/e8456c67c82fc38f40c6.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    25452 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/e931bc0d14f5bbb1da22.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)    10372 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/eb0d4c666d17c3ab1848.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)    67860 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/eb91f7b948a42799f678.ttf
+-rw-r--r--   0 mre       (1000) mre       (1000)    39136 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/f43b6ebf46ee6fba0555.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)    52352 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/f681eaa0ad0df351e7db.woff
+-rw-r--r--   0 mre       (1000) mre       (1000)   156496 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/fb8184add5a3101ad0a3.woff2
+-rw-r--r--   0 mre       (1000) mre       (1000)  2894510 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/main-28e48c6972dfda92c688.js
+-rw-r--r--   0 mre       (1000) mre       (1000)     1587 2024-04-30 11:24:53.000000 teamvault-1.0.0rc3/teamvault/static/bundled/main-28e48c6972dfda92c688.js.LICENSE.txt
+-rw-r--r--   0 mre       (1000) mre       (1000)  2896809 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/main-7b225262d27db5fe5581.js
+-rw-r--r--   0 mre       (1000) mre       (1000)     1587 2024-02-24 15:16:51.000000 teamvault-1.0.0rc3/teamvault/static/bundled/main-7b225262d27db5fe5581.js.LICENSE.txt
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.645343 teamvault-1.0.0rc3/teamvault/static/js/
+-rw-r--r--   0 mre       (1000) mre       (1000)     2158 2024-02-24 15:16:14.000000 teamvault-1.0.0rc3/teamvault/static/js/index.js
+-rw-r--r--   0 mre       (1000) mre       (1000)      525 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/static/js/utils.js
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.645343 teamvault-1.0.0rc3/teamvault/static/scss/
+-rw-r--r--   0 mre       (1000) mre       (1000)      901 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/static/scss/avatars.scss
+-rw-r--r--   0 mre       (1000) mre       (1000)     1619 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/static/scss/base.scss
+-rw-r--r--   0 mre       (1000) mre       (1000)      325 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/static/scss/fontawesome.scss
+-rw-r--r--   0 mre       (1000) mre       (1000)      421 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/static/scss/scrollbar.scss
+-rw-r--r--   0 mre       (1000) mre       (1000)     2310 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/static/scss/search.scss
+-rw-r--r--   0 mre       (1000) mre       (1000)     1830 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/static/scss/secrets.scss
+-rw-r--r--   0 mre       (1000) mre       (1000)      671 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/static/scss/select2.scss
+-rw-r--r--   0 mre       (1000) mre       (1000)      766 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/static/scss/theme.scss
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.645343 teamvault-1.0.0rc3/teamvault/templates/
+-rw-r--r--   0 mre       (1000) mre       (1000)      437 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/templates/404_anon.html
+-rw-r--r--   0 mre       (1000) mre       (1000)      538 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/templates/404_loggedin.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     2293 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/templates/base.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     6226 2024-04-15 09:03:50.000000 teamvault-1.0.0rc3/teamvault/templates/base_nav.html
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.645343 teamvault-1.0.0rc3/teamvault/templates/helpers/
+-rw-r--r--   0 mre       (1000) mre       (1000)     1754 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/templates/helpers/filter.html
+-rw-r--r--   0 mre       (1000) mre       (1000)      220 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/templates/helpers/filter_item.html
+-rw-r--r--   0 mre       (1000) mre       (1000)      328 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/templates/helpers/filter_row.html
+-rw-r--r--   0 mre       (1000) mre       (1000)     2143 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/templates/pagination.html
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.645343 teamvault-1.0.0rc3/teamvault/templates/rest_framework/
+-rw-r--r--   0 mre       (1000) mre       (1000)      279 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/templates/rest_framework/api.html
+-rw-r--r--   0 mre       (1000) mre       (1000)      563 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/urls.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     2064 2024-01-05 08:42:23.000000 teamvault-1.0.0rc3/teamvault/views.py
+-rw-r--r--   0 mre       (1000) mre       (1000)     5858 2024-04-30 11:49:13.000000 teamvault-1.0.0rc3/teamvault/webpack-stats.json
+-rw-r--r--   0 mre       (1000) mre       (1000)      247 2023-05-25 13:06:09.000000 teamvault-1.0.0rc3/teamvault/wsgi.py
+drwxr-xr-x   0 mre       (1000) mre       (1000)        0 2024-04-30 11:49:15.645343 teamvault-1.0.0rc3/teamvault.egg-info/
+-rw-r--r--   0 mre       (1000) mre       (1000)    44508 2024-04-30 11:49:15.000000 teamvault-1.0.0rc3/teamvault.egg-info/PKG-INFO
+-rw-r--r--   0 mre       (1000) mre       (1000)    10108 2024-04-30 11:49:15.000000 teamvault-1.0.0rc3/teamvault.egg-info/SOURCES.txt
+-rw-r--r--   0 mre       (1000) mre       (1000)        1 2024-04-30 11:49:15.000000 teamvault-1.0.0rc3/teamvault.egg-info/dependency_links.txt
+-rw-r--r--   0 mre       (1000) mre       (1000)       49 2024-04-30 11:49:15.000000 teamvault-1.0.0rc3/teamvault.egg-info/entry_points.txt
+-rw-r--r--   0 mre       (1000) mre       (1000)      319 2024-04-30 11:49:15.000000 teamvault-1.0.0rc3/teamvault.egg-info/requires.txt
+-rw-r--r--   0 mre       (1000) mre       (1000)       28 2024-04-30 11:49:15.000000 teamvault-1.0.0rc3/teamvault.egg-info/top_level.txt
```

### Comparing `teamvault-0.9.2/CHANGELOG.md` & `teamvault-1.0.0rc3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/LICENSE` & `teamvault-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/audit/migrations/0001_initial.py` & `teamvault-1.0.0rc3/teamvault/apps/audit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/audit/migrations/0002_auto_20170313_1544.py` & `teamvault-1.0.0rc3/teamvault/apps/audit/migrations/0002_auto_20170313_1544.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0001_initial.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0003_auto_20150113_1915.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0003_auto_20150113_1915.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0007_auto_20150205_1918.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0007_auto_20150205_1918.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0008_auto_20150322_0944.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0008_auto_20150322_0944.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0009_auto_20150322_0949.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0009_auto_20150322_0949.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0012_secret_search_index.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0012_secret_search_index.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0013_auto_20161021_1411.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0013_auto_20161021_1411.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0014_auto_20170313_1544.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0014_auto_20170313_1544.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0016_auto_20180220_1053.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0016_auto_20180220_1053.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0017_auto_20180220_1115.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0017_auto_20180220_1115.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0019_secret_notify_on_access_request.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0019_secret_notify_on_access_request.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0020_auto_20180220_1356.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0020_auto_20180220_1356.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/migrations/0023_auto_20190822_1234.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/migrations/0023_auto_20190822_1234.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/models.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from datetime import timedelta
 from hashlib import sha256
 from operator import itemgetter
-from random import sample
 
 from cryptography.fernet import Fernet
 from django.conf import settings
 from django.contrib.auth.models import Group, User
 from django.contrib.postgres.search import SearchVector, SearchVectorField
 from django.core.exceptions import PermissionDenied, ValidationError
 from django.db import models
+from django.db.models import BooleanField, Case, Max, Q, Value, When
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 from django.http import Http404
 from django.urls import reverse
 from django.utils.timezone import now
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from hashids import Hashids
 
-from ...utils import send_mail
-from ..audit.auditlog import log
-from ..audit.models import LogEntry
 from .exceptions import PermissionError
+from ..audit.auditlog import log
+from ..audit.models import AuditLogCategoryChoices, LogEntry
+
+
+class AccessPermissionTypes(models.IntegerChoices):
+    NOT_ALLOWED = 0
+    ALLOWED = 1
+    TEMPORARILY_ALLOWED = 2
+    SUPERUSER_ALLOWED = 3
 
 
 def validate_url(value):
     if "://" not in value or \
             value.startswith("javascript:") or \
             value.startswith("data:"):
         raise ValidationError(_("invalid URL"))
@@ -42,258 +48,33 @@
 
     def save(self, *args, **kwargs):
         if not self.pk:
             # need to save once to get a primary key, then once again to
             # save the hashid
             super(HashIDModel, self).save(*args, **kwargs)
         if not self.hashid:
-            # We cannot use the same salt for every model because
-            # 1. sequentially create lots of secrets
-            # 2. note the hashid of each secrets
-            # 3. you can now enumerate access requests by using the same
-            #    hashids
-            # it's not a huge deal, but let's avoid it anyway
             hasher = Hashids(
                 min_length=settings.HASHID_MIN_LENGTH,
                 salt=self.HASHID_NAMESPACE + settings.HASHID_SALT,
             )
             self.hashid = hasher.encode(self.pk)
         # we cannot force insert anymore because we might already have
         # created the object
         kwargs['force_insert'] = False
         return super(HashIDModel, self).save(*args, **kwargs)
 
 
-class AccessRequest(HashIDModel):
-    HASHID_NAMESPACE = "AccessRequest"
-
-    STATUS_PENDING = 1
-    STATUS_REJECTED = 2
-    STATUS_APPROVED = 3
-    STATUS_CHOICES = (
-        (STATUS_PENDING, _("pending")),
-        (STATUS_REJECTED, _("rejected")),
-        (STATUS_APPROVED, _("approved")),
-    )
-
-    closed = models.DateTimeField(
-        blank=True,
-        null=True,
-    )
-    closed_by = models.ForeignKey(
-        settings.AUTH_USER_MODEL,
-        models.PROTECT,
-        blank=True,
-        null=True,
-        related_name='access_requests_closed',
-    )
-    created = models.DateTimeField(auto_now_add=True)
-    reason_request = models.TextField(
-        blank=True,
-        null=True,
-    )
-    reason_rejected = models.TextField(
-        blank=True,
-        null=True,
-    )
-    requester = models.ForeignKey(
-        settings.AUTH_USER_MODEL,
-        models.PROTECT,
-        related_name='access_requests_created',
-    )
-    reviewers = models.ManyToManyField(
-        settings.AUTH_USER_MODEL,
-        related_name='access_requests_reviewed',
-    )
-    secret = models.ForeignKey(
-        'Secret',
-        models.PROTECT,
-        related_name='access_requests',
-    )
-    status = models.PositiveSmallIntegerField(
-        choices=STATUS_CHOICES,
-        default=STATUS_PENDING,
-    )
-
-    class Meta:
-        ordering = ('-created',)
-
-    def __repr__(self):
-        return "<AccessRequest {user}@'{name}' ({id})>".format(
-            id=self.hashid,
-            name=self.secret.name,
-            user=self.requester,
-        )
-
-    @classmethod
-    def get_all_readable_by_user(cls, user):
-        if user.is_superuser:
-            return cls.objects.all()
-        return (
-            cls.objects.filter(requester=user) |
-            cls.objects.filter(reviewers=user)
-        )
-
-    def approve(self, reviewer):
-        if self.status != self.STATUS_PENDING:
-            raise PermissionDenied(_("Can't approve closed access request"))
-
-        # make sure user is still allowed to handle secret, privileges might
-        # have been revoked since the access request was made
-        self.secret.check_access(reviewer)
-
-        log(
-            _("{reviewer} has approved access request #{access_request} for {requester}, "
-              "allowing access to '{secret}'").format(
-                access_request=self.id,
-                requester=self.requester,
-                reviewer=reviewer,
-                secret=self.secret.name,
-            ),
-            actor=reviewer,
-            secret=self.secret,
-            user=self.requester,
-        )
-
-        self.closed = now()
-        self.closed_by = reviewer
-        self.status = self.STATUS_APPROVED
-        self.save()
-
-        self.secret.allowed_users.add(self.requester)
-
-        other_reviewers = list(self.reviewers.all())
-        try:
-            other_reviewers.remove(reviewer)
-        except ValueError:
-            # review by other superuser
-            pass
-
-        send_mail(
-            other_reviewers + [self.requester],
-            _("[TeamVault] Access request for '{}' approved").format(self.secret.name),
-            "secrets/mail_access_request_approved",
-            context={
-                'approved_by': reviewer.username,
-                'base_url': settings.BASE_URL,
-                'secret_name': self.secret.name,
-                'secret_url': self.secret.get_absolute_url(),
-                'username': self.requester.username,
-            },
-            user_from=reviewer,
-        )
-
-    def assign_reviewers(self):
-        candidates = list(self.secret.notify_on_access_request.filter(is_active=True))
-        if len(candidates) < 3:
-            candidates += list(
-                self.secret.allowed_users.order_by('-last_login').filter(is_active=True)[:10]
-            )
-            for group in self.secret.allowed_groups.all():
-                candidates += list(group.user_set.order_by('-last_login').filter(is_active=True)[:3])
-        if len(candidates) < 3:
-            candidates += list(User.objects.filter(
-                is_active=True,
-                is_superuser=True,
-            ).order_by('-last_login')[:3])
-        candidates = set(candidates)
-        selected = sample(candidates, min(3, len(candidates)))
-        if not selected:
-            raise RuntimeError(_("unable to find reviewers for {}").format(self))
-        self.reviewers.set(selected)
-
-        send_mail(
-            self.reviewers.all(),
-            _("[TeamVault] Review access request for '{}'").format(self.secret.name),
-            "secrets/mail_access_request_review",
-            context={
-                'access_request_url': reverse(
-                    'secrets.access_request-detail',
-                    kwargs={'hashid': self.hashid},
-                ),
-                'base_url': settings.BASE_URL,
-                'secret_name': self.secret.name,
-                'secret_url': self.secret.get_absolute_url(),
-                'username': self.requester.username,
-            },
-            user_from=self.requester,
-        )
-
-    def reject(self, reviewer, reason=None):
-        if self.status != self.STATUS_PENDING:
-            raise PermissionDenied(_("Can't reject closed access request"))
-
-        # make sure user is still allowed to handle secret, privileges might
-        # have been revoked since the access request was made
-        self.secret.check_access(reviewer)
-
-        log(
-            _("{reviewer} has rejected access request #{access_request} for {requester}, "
-              "NOT allowing access to '{secret}'").format(
-                access_request=self.id,
-                requester=self.requester,
-                reviewer=reviewer,
-                secret=self.secret.name,
-            ),
-            actor=reviewer,
-            secret=self.secret,
-            user=self.requester,
-        )
-
-        self.closed = now()
-        self.closed_by = reviewer
-        self.reason_rejected = reason
-        self.status = self.STATUS_REJECTED
-        self.save()
-
-        other_reviewers = list(self.reviewers.all())
-        try:
-            other_reviewers.remove(reviewer)
-        except ValueError:
-            # review by other superuser
-            pass
-
-        send_mail(
-            other_reviewers + [self.requester],
-            _("[TeamVault] Access request for '{}' denied").format(self.secret.name),
-            "secrets/mail_access_request_denied",
-            context={
-                'base_url': settings.BASE_URL,
-                'denied_by': reviewer.username,
-                'reason': reason,
-                'secret_name': self.secret.name,
-                'secret_url': self.secret.get_absolute_url(),
-                'username': self.requester.username,
-            },
-            user_from=reviewer,
-        )
-
-    @property
-    def full_url(self):
-        return settings.BASE_URL.rstrip("/") + self.get_absolute_url()
-
-    def get_absolute_url(self):
-        return reverse('secrets.access_request-detail', args=[str(self.hashid)])
-
-    def is_readable_by_user(self, user):
-        return (
-            user == self.requester or
-            user in self.reviewers.all() or
-            user.is_superuser
-        )
-
-
 class Secret(HashIDModel):
     HASHID_NAMESPACE = "Secret"
 
-    ACCESS_POLICY_REQUEST = 1
+    ACCESS_POLICY_DISCOVERABLE = 1
     ACCESS_POLICY_ANY = 2
     ACCESS_POLICY_HIDDEN = 3
     ACCESS_POLICY_CHOICES = (
-        (ACCESS_POLICY_REQUEST, _("request")),
+        (ACCESS_POLICY_DISCOVERABLE, _("discoverable")),
         (ACCESS_POLICY_ANY, _("everyone")),
         (ACCESS_POLICY_HIDDEN, _("hidden")),
     )
     CONTENT_PASSWORD = 1
     CONTENT_CC = 2
     CONTENT_FILE = 3
     CONTENT_CHOICES = (
@@ -308,25 +89,15 @@
         (STATUS_OK, _("OK")),
         (STATUS_NEEDS_CHANGING, _("needs changing")),
         (STATUS_DELETED, _("deleted")),
     )
 
     access_policy = models.PositiveSmallIntegerField(
         choices=ACCESS_POLICY_CHOICES,
-        default=ACCESS_POLICY_REQUEST,
-    )
-    allowed_groups = models.ManyToManyField(
-        Group,
-        blank=True,
-        related_name='allowed_passwords',
-    )
-    allowed_users = models.ManyToManyField(
-        settings.AUTH_USER_MODEL,
-        blank=True,
-        related_name='allowed_passwords',
+        default=ACCESS_POLICY_DISCOVERABLE,
     )
     content_type = models.PositiveSmallIntegerField(
         choices=CONTENT_CHOICES,
         default=CONTENT_PASSWORD,
     )
     created = models.DateTimeField(auto_now_add=True)
     created_by = models.ForeignKey(
@@ -340,34 +111,42 @@
         blank=True,
         null=True,
         related_name='_password_current_revision',
     )
     description = models.TextField(
         blank=True,
         null=True,
+        help_text=_('Further information on the secret.'),
     )
     filename = models.CharField(
         blank=True,
         max_length=255,
         null=True,
     )
     last_changed = models.DateTimeField(
         auto_now_add=True,
     )
     last_read = models.DateTimeField(
         default=now,
     )
-    name = models.CharField(max_length=92)
+    name = models.CharField(max_length=92, help_text=_('Enter a unique name for the secret'))
     needs_changing_on_leave = models.BooleanField(
         default=True,
     )
-    notify_on_access_request = models.ManyToManyField(
+    shared_groups = models.ManyToManyField(
+        Group,
+        blank=True,
+        through='SharedSecretData',
+        through_fields=('secret', 'group'),
+    )
+    shared_users = models.ManyToManyField(
         settings.AUTH_USER_MODEL,
         blank=True,
-        related_name='notify_on_access_requests_for',
+        through='SharedSecretData',
+        through_fields=('secret', 'user'),
     )
     status = models.PositiveSmallIntegerField(
         choices=STATUS_CHOICES,
         default=STATUS_OK,
     )
     url = models.CharField(
         blank=True,
@@ -391,90 +170,114 @@
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return "<Secret '{name}' ({id})>".format(id=self.hashid, name=self.name)
 
-    def check_access(self, user):
+    def check_read_access(self, user):
+        if not self.is_visible_to_user(user):
+            raise Http404
+
+        readable = self.is_readable_by_user(user)
+        if not readable:
+            raise PermissionDenied()
+        return readable
+
+    def check_share_access(self, user):
         if not self.is_visible_to_user(user):
             raise Http404
-        elif not self.is_readable_by_user(user):
+
+        shareable = self.is_shareable_by_user(user)
+        if not shareable:
             raise PermissionDenied()
+        return shareable
 
     @property
     def full_url(self):
         return settings.BASE_URL.rstrip("/") + self.get_absolute_url()
 
     def get_absolute_url(self):
         return reverse('secrets.secret-detail', args=[str(self.hashid)])
 
     def get_data(self, user):
         if not self.current_revision:
             raise Http404
-        if not self.is_readable_by_user(user):
-            log(_(
-                    "{user} tried to access '{name}' without permission"
-                ).format(
-                    name=self.name,
-                    user=user.username,
-                ),
+
+        read_allowed = self.is_readable_by_user(user)
+        if not read_allowed:
+            log(
+                _("{user} tried to access '{name}' without permission").format(name=self.name, user=user.username),
                 actor=user,
-                level='warn',
+                category=AuditLogCategoryChoices.SECRET_PERMISSION_VIOLATION,
+                level='warning',
                 secret=self,
             )
             raise PermissionError(_(
                 "{user} not allowed access to '{name}' ({id})"
             ).format(
                 id=self.id,
                 name=self.name,
                 user=user.username,
             ))
-        f = Fernet(settings.TEAMVAULT_SECRET_KEY)
-        log(_(
-                "{user} read '{name}'"
-            ).format(
+
+        if read_allowed == AccessPermissionTypes.SUPERUSER_ALLOWED:
+            category = AuditLogCategoryChoices.SECRET_ELEVATED_SUPERUSER_READ
+            log_message = _("{user} used superuser privileges to read '{name}'")
+        else:
+            category = AuditLogCategoryChoices.SECRET_READ
+            log_message = _("{user} read '{name}'")
+
+        log(
+            log_message.format(
                 name=self.name,
                 user=user.username,
             ),
             actor=user,
+            category=category,
             level='info',
             secret=self,
             secret_revision=self.current_revision,
         )
         self.current_revision.accessed_by.add(user)
         self.current_revision.save()
         self.last_read = now()
         self.save()
 
+        f = Fernet(settings.TEAMVAULT_SECRET_KEY)
         plaintext_data = f.decrypt(self.current_revision.encrypted_data.tobytes())
         if self.content_type != Secret.CONTENT_FILE:
             plaintext_data = plaintext_data.decode('utf-8')
         return plaintext_data
 
     @classmethod
     def get_all_readable_by_user(cls, user):
-        if user.is_superuser:
+        if user.is_superuser and settings.ALLOW_SUPERUSER_READS:
             return cls.objects.all()
-        return (
-            cls.objects.filter(access_policy=cls.ACCESS_POLICY_ANY) |
-            cls.objects.filter(allowed_users=user) |
-            cls.objects.filter(allowed_groups__in=user.groups.all())
+
+        allowed_shares = SharedSecretData.objects.with_expiry_state().filter(
+            Q(user=user) | Q(group__user=user)
+        ).exclude(is_expired=True).values('secret__pk')
+        return cls.objects.filter(
+            Q(access_policy=cls.ACCESS_POLICY_ANY) | Q(pk__in=allowed_shares)
         ).exclude(status=cls.STATUS_DELETED).distinct()
 
     @classmethod
     def get_all_visible_to_user(cls, user, queryset=None):
         if queryset is None:
             queryset = cls.objects.all()
+
         if user.is_superuser:
             return queryset
-        return (
-            queryset.filter(access_policy__in=(cls.ACCESS_POLICY_ANY, cls.ACCESS_POLICY_REQUEST)) |
-            queryset.filter(allowed_users=user) |
-            queryset.filter(allowed_groups__in=user.groups.all())
+
+        allowed_shares = SharedSecretData.objects.with_expiry_state().filter(
+            Q(user=user) | Q(group__user=user)
+        ).exclude(is_expired=True).values('secret__pk')
+        return queryset.filter(
+            Q(access_policy__in=(cls.ACCESS_POLICY_ANY, cls.ACCESS_POLICY_DISCOVERABLE)) | Q(pk__in=allowed_shares)
         ).exclude(status=cls.STATUS_DELETED).distinct()
 
     @classmethod
     def get_most_used_for_user(cls, user, limit=5):
         since = now() - timedelta(days=90)
         accessed_secrets = LogEntry.objects.filter(
             actor=user,
@@ -488,72 +291,95 @@
             access_count=models.Count('secret'),
         )
         ordered_secrets = sorted(accessed_secrets, key=itemgetter('access_count'), reverse=True)
         return [cls.objects.get(id=item['secret']) for item in ordered_secrets[:limit]]
 
     @classmethod
     def get_most_recently_used_for_user(cls, user, limit=5):
-        secrets = []
         log_entries = LogEntry.objects.filter(
-            actor=user,
-            secret__isnull=False,
-        )
-        number_of_log_entries = log_entries.count()
-        offset = limit
-        while len(secrets) < limit and (offset < number_of_log_entries or offset == limit):
-            for log_entry in log_entries[:offset].select_related('secret'):
-                if log_entry.secret not in secrets and len(secrets) < limit:
-                    secrets.append(log_entry.secret)
-            offset += limit
-        return secrets
+            actor=user
+        ).values(
+            'secret'
+        ).annotate(
+            latest_time=Max('time')
+        ).order_by(
+            '-latest_time'
+        )[:limit]
+
+        ordered_secret_ids = [access['secret'] for access in log_entries]
+        unordered_secrets = Secret.objects.filter(id__in=ordered_secret_ids)
+        secret_map = {secret.id: secret for secret in unordered_secrets}
+        ordered_secrets = [secret_map[secret_id] for secret_id in ordered_secret_ids if secret_id in secret_map]
+        return ordered_secrets
 
     @classmethod
-    def get_search_results(cls, user, term, limit=None):
+    def get_search_results(cls, user, term, limit=None, substr_search=True):
         base_queryset = cls.get_all_visible_to_user(user)
         name_hits = base_queryset.filter(name__icontains=term)
         fulltext_hits = cls.get_all_visible_to_user(
             user,
             queryset=cls.objects.filter(search_index=term),
         )
-        substr_hits = base_queryset.filter(
-            models.Q(filename__icontains=term) |
-            models.Q(url__icontains=term) |
-            models.Q(username__icontains=term)
-        )
+
+        substr_hits = Secret.objects.none()
+        if substr_search:
+            substr_hits = base_queryset.filter(
+                models.Q(filename__icontains=term) |
+                models.Q(url__icontains=term) |
+                models.Q(username__icontains=term) |
+                models.Q(hashid__exact=term)
+            )
         if limit:
             name_hits = name_hits[:limit]
             fulltext_hits = fulltext_hits[:limit]
             substr_hits = substr_hits[:limit]
         # concatenate and remove duplicates
         result = (name_hits | fulltext_hits | substr_hits).distinct()
         if limit:
             return result[:limit]
         else:
             return result
 
     def is_readable_by_user(self, user):
-        return (
-            user.is_superuser or (
-                (
-                    self.access_policy == self.ACCESS_POLICY_ANY or
-                    user in self.allowed_users.all() or
-                    set(self.allowed_groups.all()).intersection(set(user.groups.all()))
-                ) and self.status != self.STATUS_DELETED
-            )
-        )
+        if self.status != self.STATUS_DELETED:
+            shares = self.share_data.with_expiry_state().filter(
+                Q(user=user) | Q(group__user=user)
+            ).exclude(is_expired=True)
+
+            if self.access_policy == self.ACCESS_POLICY_ANY or shares.filter(granted_until__isnull=True).exists():
+                return AccessPermissionTypes.ALLOWED
+
+            if shares.exists():
+                return AccessPermissionTypes.TEMPORARILY_ALLOWED
+
+        if user.is_superuser and settings.ALLOW_SUPERUSER_READS:
+            return AccessPermissionTypes.SUPERUSER_ALLOWED
+
+        return AccessPermissionTypes.NOT_ALLOWED
+
+    def is_shareable_by_user(self, user):
+        read_permission = self.is_readable_by_user(user)
+        if read_permission == AccessPermissionTypes.ALLOWED:
+            return AccessPermissionTypes.ALLOWED
+
+        if user.is_superuser:
+            return AccessPermissionTypes.SUPERUSER_ALLOWED
+        return AccessPermissionTypes.NOT_ALLOWED
 
     def is_visible_to_user(self, user):
-        return (
-            user.is_superuser or (
-                (
-                    self.access_policy in (self.ACCESS_POLICY_ANY, self.ACCESS_POLICY_REQUEST) or
+        if self.status != self.STATUS_DELETED:
+            if (
+                    self.access_policy in (self.ACCESS_POLICY_ANY, self.ACCESS_POLICY_DISCOVERABLE) or
                     self.is_readable_by_user(user)
-                ) and self.status != self.STATUS_DELETED
-            )
-       )
+            ):
+                return AccessPermissionTypes.ALLOWED
+
+        if user.is_superuser:
+            return AccessPermissionTypes.SUPERUSER_ALLOWED
+        return AccessPermissionTypes.NOT_ALLOWED
 
     def set_data(self, user, plaintext_data, skip_access_check=False):
         # skip_access_check is used when initially creating a secret
         # and makes it possible to create secrets you don't have access
         # to
         if not skip_access_check and not self.is_readable_by_user(user):
             raise PermissionError(_(
@@ -596,28 +422,69 @@
             previous_revision_id = _("none")
         self.current_revision = p
         self.last_changed = now()
         self.last_read = now()
         if self.status == self.STATUS_NEEDS_CHANGING:
             self.status = self.STATUS_OK
         self.save()
-        log(_(
-                "{user} set a new secret for '{name}' ({oldrev}->{newrev})"
-            ).format(
+        log(
+            _("{user} set a new secret for '{name}' ({oldrev}->{newrev})").format(
                 name=self.name,
                 newrev=self.current_revision.id,
                 oldrev=previous_revision_id,
                 user=user.username,
             ),
             actor=user,
+            category=AuditLogCategoryChoices.SECRET_CHANGED,
             level='info',
             secret=self,
             secret_revision=self.current_revision,
         )
 
+    def needs_changing(self):
+        return self.status == self.STATUS_NEEDS_CHANGING
+
+    def share(self, grant_description, granted_by, user=None, group=None, granted_until=None):
+        if (user and group) or (not user and not group):
+            raise ValueError('Specify either a user or a group!')
+
+        if not isinstance(granted_by, User):
+            raise ValueError('granted_by has to be a User object!')
+
+        permission = self.is_shareable_by_user(granted_by)
+        if not permission:
+            raise PermissionDenied()
+
+        share_obj = self.share_data.create(
+            grant_description=grant_description,
+            granted_by=granted_by,
+            granted_until=granted_until,
+            group=group,
+            user=user,
+        )
+        log(
+            _("{user} granted access to {shared_entity_type} '{name}' {time}").format(
+                shared_entity_type=share_obj.shared_entity_type,
+                name=share_obj.shared_entity_name,
+                user=granted_by.username,
+                time=_('until ') + share_obj.granted_until.isoformat() if share_obj.granted_until else _('permanently')
+            ),
+            actor=granted_by,
+            category=(
+                AuditLogCategoryChoices.SECRET_SUPERUSER_SHARED
+                if permission == AccessPermissionTypes.SUPERUSER_ALLOWED
+                else AuditLogCategoryChoices.SECRET_SHARED
+            ),
+            level='warning',
+            reason=grant_description,
+            secret=self,
+        )
+
+        return share_obj
+
 
 class SecretRevision(HashIDModel):
     HASHID_NAMESPACE = "SecretRevision"
 
     accessed_by = models.ManyToManyField(
         settings.AUTH_USER_MODEL,
     )
@@ -657,17 +524,130 @@
         return "<SecretRevision '{name}' ({id})>".format(id=self.hashid, name=self.secret.name)
 
     @property
     def is_current_revision(self):
         return self.secret.current_revision == self
 
 
+class SecretShareQuerySet(models.QuerySet):
+    # TODO: Rename to group_shares, user_shares
+    def groups(self):
+        return self.with_expiry_state().filter(group__isnull=False).order_by('group__name')
+
+    def users(self):
+        return self.with_expiry_state().filter(user__isnull=False).order_by('user__username')
+
+    def with_expiry_state(self):
+        return self.annotate(
+            is_expired=Case(
+                When(
+                    granted_until__lte=now(),
+                    then=Value(True)
+                ),
+                default=Value(False),
+                output_field=BooleanField()
+            )
+        )
+
+
+class SharedSecretData(models.Model):
+    objects = SecretShareQuerySet.as_manager()
+
+    group = models.ForeignKey(
+        Group,
+        on_delete=models.CASCADE,
+        null=True,
+        related_name='secret_share_data',
+    )
+
+    user = models.ForeignKey(
+        settings.AUTH_USER_MODEL,
+        on_delete=models.CASCADE,
+        null=True,
+        related_name='secret_share_data',
+    )
+
+    secret = models.ForeignKey(
+        'Secret',
+        on_delete=models.CASCADE,
+        related_name='share_data',
+    )
+
+    grant_description = models.TextField(
+        null=True
+    )
+
+    granted_by = models.ForeignKey(
+        settings.AUTH_USER_MODEL,
+        on_delete=models.PROTECT,
+        null=True,
+        related_name='+',
+    )
+
+    granted_on = models.DateTimeField(
+        auto_now_add=True,
+        null=True,
+    )
+
+    # Secrets are considered permanently shared if granted_until is not set
+    granted_until = models.DateTimeField(
+        blank=True,
+        null=True,
+    )
+
+    @property
+    def shared_entity(self):
+        return self.group if self.group else self.user
+
+    @property
+    def shared_entity_name(self):
+        return self.group.name if self.group else self.user.username
+
+    @property
+    def shared_entity_type(self):
+        return 'group' if self.group else 'user'
+
+    @property
+    def about_to_expire(self):
+        if not self.granted_until:
+            return False
+
+        if now() + timedelta(hours=8) >= self.granted_until:
+            return True
+
+    @property
+    def expiry_icon(self):
+        if not self.granted_until:
+            return 'success'
+
+        if self.about_to_expire:
+            time_left = self.granted_until - now()
+            if time_left <= timedelta(hours=8):
+                return 'danger'
+        return 'warning'
+
+    def __str__(self):
+        return f'SharedSecretData object ({self.secret.name}: {self.user.username if self.user else self.group.name})'
+
+    class Meta:
+        constraints = [
+            models.CheckConstraint(
+                check=(
+                        (Q(group__isnull=False) & Q(user__isnull=True)) |
+                        (Q(group__isnull=True) & Q(user__isnull=False))
+                ),
+                name='only_one_set'
+            ),
+        ]
+        unique_together = [('group', 'secret'), ('user', 'secret')]
+
+
 @receiver(post_save, sender=Secret)
 def update_search_index(sender, **kwargs):
     Secret.objects.filter(id=kwargs['instance'].id).update(
         search_index=(
-            SearchVector('name', weight='A') +
-            SearchVector('description', weight='B') +
-            SearchVector('username', weight='C') +
-            SearchVector('filename', weight='D')
+                SearchVector('name', weight='A') +
+                SearchVector('description', weight='B') +
+                SearchVector('username', weight='C') +
+                SearchVector('filename', weight='D')
         ),
     )
```

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/templates/secrets/secret_delete.html` & `teamvault-1.0.0rc3/teamvault/apps/secrets/templates/secrets/secret_delete.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-{% extends "base_nav.html" %}
+{% extends "base.html" %}
 {% load i18n %}
 {% load static %}
-{% block "title" %}{% trans "Confirm deletion" %}{% endblock %}
-{% block "content" %}
-<div class="container container-opaque">
-	<div class="row">
-		<div class="col-md-8 col-md-offset-2">
+{% block title %}{% trans "Confirm deletion" %}{% endblock %}
+{% block content %}
+	<div class="row justify-content-center">
+		<div class="col-8 col-lg-4">
 			<h1>
 				{% blocktrans with name=secret.name content_type=secret.get_content_type_display %}
 				Delete {{ content_type }} '{{ name }}'?
 				{% endblocktrans %}
 			</h1>
 			<hr>
 		</div>
 	</div>
-	<div class="row">
-		<div class="col-md-8 col-md-offset-2">
+	<div class="row justify-content-center">
+		<div class="col-8 col-lg-4">
 			<div class="alert alert-info" role="alert">
 				{% blocktrans %}
 				Passwords are never completely erased from the system. Administrators can undelete them. Regular users will not be able to see or access deleted passwords. If a password has been revealed to an unauthorized party, you should change it instead.
 				{% endblocktrans %}
 			</div>
 			<form role="form" method="POST" class="form-horizontal">
 				{% csrf_token %}
-				<a class="btn btn-default btn-lg pull-left" href="{{ secret.get_absolute_url }}"><i class="fa fa-angle-left"></i> &nbsp; {% trans "No, go back" %}</a>
-				<button type="submit" class="btn btn-danger btn-lg pull-right"><i class="fa fa-trash"></i> &nbsp; {% trans "Yes, delete" %}</button>
+				<a class="btn btn-light btn-lg fa-pull-left" href="{{ secret.get_absolute_url }}"><i class="fa fa-angle-left"></i> &nbsp; {% trans "No, go back" %}</a>
+				<button type="submit" class="btn btn-danger btn-lg fa-pull-right"><i class="fa fa-trash"></i> &nbsp; {% trans "Yes, delete" %}</button>
 			</form>
 		</div>
 	</div>
-</div>
 {% endblock %}
```

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/urls.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,71 @@
-from django.conf.urls import url
+from django.urls import path
 
 from . import views
 
 urlpatterns = (
-    url(
-        r'^$',
+    path(
+        '',
         views.dashboard,
         name='dashboard',
     ),
-    url(
-        r'^access_requests/$',
-        views.access_request_list,
-        name='secrets.access_request-list',
-    ),
-    url(
-        r'^access_requests/(?P<hashid>\w+)$',
-        views.access_request_detail,
-        name='secrets.access_request-detail',
-    ),
-    url(
-        r'^access_requests/(?P<hashid>\w+)/(?P<action>(allow|deny))$',
-        views.access_request_review,
-        name='secrets.access_request-review',
-    ),
-    url(
-        r'^opensearch.xml$',
+    path(
+        'opensearch.xml',
         views.opensearch,
         name='opensearch',
     ),
-    url(
-        r'^secrets/$',
+    path(
+        'secrets/',
         views.secret_list,
         name='secrets.secret-list',
     ),
-    url(
-        r'^secrets/(?P<hashid>\w+)$',
+    path(
+        'secrets/<str:hashid>/',
         views.secret_detail,
         name='secrets.secret-detail',
     ),
-    url(
-        r'^secrets/(?P<hashid>\w+)/delete$',
+    path(
+        'secrets/<str:hashid>/delete',
         views.secret_delete,
         name='secrets.secret-delete',
     ),
-    url(
-        r'^secrets/(?P<hashid>\w+)/download$',
+    path(
+        'secrets/<str:hashid>/download',
         views.secret_download,
         name='secrets.secret-download',
     ),
-    url(
-        r'^secrets/(?P<hashid>\w+)/edit$',
+    path(
+        'secrets/<str:hashid>/edit',
         views.secret_edit,
         name='secrets.secret-edit',
     ),
-    url(
-        r'^secrets/(?P<hashid>\w+)/request_access$',
-        views.access_request_create,
-        name='secrets.secret-request_access',
+    path(
+        'secrets/<str:hashid>/metadata',
+        views.secret_metadata,
+        name='secrets.secret-metadata',
     ),
-    url(
-        r'^secrets/(?P<hashid>\w+)/restore$',
+    path(
+        'secrets/<str:hashid>/restore',
         views.secret_restore,
         name='secrets.secret-restore',
     ),
-    url(
-        r'^secrets/add/(?P<content_type>\w+)$',
+    path(
+        'secrets/<str:hashid>/share',
+        views.secret_share_list,
+        name='secrets.secret-share',
+    ),
+    path(
+        'secrets/<str:hashid>/share/<int:share_id>/delete',
+        views.secret_share_delete,
+        name='secrets.secret-share-delete',
+    ),
+    path(
+        'secrets/add/<str:content_type>',
         views.secret_add,
         name='secrets.secret-add',
     ),
-    url(
-        r'^secrets/live-search$',
+    path(
+        'secrets/live-search',
         views.secret_search,
         name='secrets.secret-search',
     ),
 )
```

### Comparing `teamvault-0.9.2/teamvault/apps/secrets/views.py` & `teamvault-1.0.0rc3/teamvault/apps/secrets/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from json import dumps, loads
 from urllib.parse import quote, urlencode
 
 from django.conf import settings
+from django.contrib import messages
 from django.contrib.auth.decorators import login_required, user_passes_test
 from django.contrib.auth.models import Group, User
-from django.core.exceptions import PermissionDenied
-from django.http import HttpResponse, HttpResponseRedirect, Http404
-from django.shortcuts import get_object_or_404, render
+from django.core.exceptions import ObjectDoesNotExist, PermissionDenied
+from django.http import HttpResponse, HttpResponseRedirect, Http404, JsonResponse
+from django.shortcuts import get_object_or_404, render, redirect
+from django.template.defaultfilters import pluralize
 from django.urls import reverse
-from django.utils.translation import ugettext_lazy as _
+from django.utils.functional import cached_property
+from django.utils.translation import gettext_lazy as _
 from django.views.decorators.http import require_http_methods
 from django.views.generic import DetailView, ListView, TemplateView
 from django.views.generic.edit import CreateView, UpdateView
-import django_filters
+from django_htmx.http import trigger_client_event
 
+from .filters import SecretFilter
+from .forms import CCForm, FileForm, PasswordForm, SecretShareForm
+from .models import AccessPermissionTypes, Secret, SharedSecretData
+from ..accounts.models import UserProfile
 from ..audit.auditlog import log
-from .forms import CCForm, FileForm, PasswordForm
-from .models import AccessRequest, Secret
+from ..audit.models import AuditLogCategoryChoices
 
-ACCESS_STR_IDS = {
-    'ACCESS_POLICY_ANY': str(Secret.ACCESS_POLICY_ANY),
-    'ACCESS_POLICY_REQUEST': str(Secret.ACCESS_POLICY_REQUEST),
-    'ACCESS_POLICY_HIDDEN': str(Secret.ACCESS_POLICY_HIDDEN),
-}
 CONTENT_TYPE_FORMS = {
     'cc': CCForm,
     'file': FileForm,
     'password': PasswordForm,
 }
 CONTENT_TYPE_IDS = {
     'cc': Secret.CONTENT_CC,
@@ -38,162 +39,56 @@
 CONTENT_TYPE_NAMES = {
     'cc': _CONTENT_TYPES[Secret.CONTENT_CC],
     'file': _CONTENT_TYPES[Secret.CONTENT_FILE],
     'password': _CONTENT_TYPES[Secret.CONTENT_PASSWORD],
 }
 
 
-def _patch_post_data(POST, fields):
-    """
-    Select2 passes in selected values as CSV instead of as a real
-    multiple value field, so we need to split them before any validation
-    takes place.
-    """
-    POST = POST.copy()
-    for csv_field in fields:
-        if POST.getlist(csv_field) == ['']:
-            del POST[csv_field]
-        else:
-            POST.setlist(
-                csv_field,
-                POST.getlist(csv_field)[0].split(","),
-            )
-    return POST
-
-
-@login_required
-def access_request_create(request, hashid):
-    secret = Secret.objects.get(hashid=hashid)
-    if not secret.is_visible_to_user(request.user):
-        raise Http404
-    try:
-        AccessRequest.objects.get(
-            requester=request.user,
-            secret=secret,
-            status=AccessRequest.STATUS_PENDING,
-        )
-    except AccessRequest.DoesNotExist:
-        if request.method == 'POST' and not secret.is_readable_by_user(request.user):
-            access_request = AccessRequest()
-            access_request.reason_request = request.POST['reason']
-            access_request.requester = request.user
-            access_request.secret = secret
-            access_request.save()
-            access_request.assign_reviewers()
-    return HttpResponseRedirect(secret.get_absolute_url())
-
-
-@login_required
-@require_http_methods(["POST"])
-def access_request_review(request, hashid, action):
-    access_request = get_object_or_404(
-        AccessRequest,
-        hashid=hashid,
-        status=AccessRequest.STATUS_PENDING,
-    )
-    if not request.user.is_superuser and request.user not in access_request.reviewers.all():
-        raise PermissionDenied()
-
-    if action == 'allow':
-        access_request.approve(request.user)
-    else:
-        access_request.reject(request.user, reason=request.POST.get('reason', None))
-
-    return HttpResponseRedirect(reverse('secrets.access_request-list'))
-
-
-class AccessRequestDetail(DetailView):
-    context_object_name = 'access_request'
-    model = AccessRequest
-    slug_field = 'hashid'
-    slug_url_kwarg = 'hashid'
-    template_name = "secrets/accessrequest_detail.html"
-
-    def get_object(self):
-        if self.request.user.is_superuser:
-            return get_object_or_404(
-                AccessRequest,
-                hashid=self.kwargs['hashid'],
-                status=AccessRequest.STATUS_PENDING,
-            )
-        else:
-            return get_object_or_404(
-                AccessRequest,
-                hashid=self.kwargs['hashid'],
-                reviewers=self.request.user,
-                status=AccessRequest.STATUS_PENDING,
-            )
-access_request_detail = login_required(AccessRequestDetail.as_view())
-
-
-class AccessRequestList(ListView):
-    context_object_name = 'access_requests'
-    template_name = "secrets/accessrequests_list.html"
-
-    def get_context_data(self, **kwargs):
-        queryset = self.get_queryset()
-        context = super(AccessRequestList, self).get_context_data(**kwargs)
-        context['reviewable'] = queryset.exclude(requester=self.request.user)
-        context['pending_review'] = queryset.filter(requester=self.request.user)
-        return context
-
-    def get_queryset(self):
-        queryset = AccessRequest.get_all_readable_by_user(self.request.user)
-        return queryset.filter(status=AccessRequest.STATUS_PENDING)
-access_request_list = login_required(AccessRequestList.as_view())
-
-
 class Dashboard(TemplateView):
     template_name = "secrets/dashboard.html"
 
     def get_context_data(self, **kwargs):
         context = super(Dashboard, self).get_context_data(**kwargs)
         context['search_term'] = ""
         context['most_used_secrets'] = Secret.get_most_used_for_user(self.request.user)
         context['readable_secrets'] = Secret.get_all_readable_by_user(self.request.user)
         context['recently_used_secrets'] = Secret.get_most_recently_used_for_user(self.request.user)
         return context
+
+
 dashboard = login_required(Dashboard.as_view())
 
 
 class OpenSearch(TemplateView):
     content_type = "application/xml"
     template_name = "opensearch.xml"
 
     def get_context_data(self, **kwargs):
         context = super(OpenSearch, self).get_context_data(**kwargs)
         context['base_url'] = settings.BASE_URL
         return context
+
+
 opensearch = OpenSearch.as_view()
 
 
 class SecretAdd(CreateView):
     slug_field = 'hashid'
     slug_url_kwarg = 'hashid'
 
     def form_valid(self, form):
         secret = Secret()
         secret.content_type = CONTENT_TYPE_IDS[self.kwargs['content_type']]
         secret.created_by = self.request.user
 
-        for attr in ('access_policy', 'description', 'name', 'needs_changing_on_leave', 'url',
-                     'username'):
+        for attr in ('access_policy', 'description', 'name', 'needs_changing_on_leave', 'url', 'username'):
             if attr in form.cleaned_data:
                 setattr(secret, attr, form.cleaned_data[attr])
         secret.save()
 
-        for attr in ('notify_on_access_request',):
-            if form.cleaned_data[attr]:
-                getattr(secret, attr).add(self.request.user)
-            else:
-                getattr(secret, attr).remove(self.request.user)
-
-        for attr in ('allowed_groups', 'allowed_users'):
-            getattr(secret, attr).set(form.cleaned_data[attr])
-
         if secret.content_type == Secret.CONTENT_PASSWORD:
             plaintext_data = form.cleaned_data['password']
         elif secret.content_type == Secret.CONTENT_FILE:
             plaintext_data = form.cleaned_data['file'].read()
             secret.filename = form.cleaned_data['file'].name
             secret.save()
         elif secret.content_type == Secret.CONTENT_CC:
@@ -203,66 +98,81 @@
                 'expiration_month': str(form.cleaned_data['expiration_month']),
                 'expiration_year': str(form.cleaned_data['expiration_year']),
                 'security_code': str(form.cleaned_data['security_code']),
                 'password': form.cleaned_data['password'],
             })
         secret.set_data(self.request.user, plaintext_data, skip_access_check=True)
 
+        # Create share objects
+        secret.share_data.create(user=self.request.user)
+        if form.cleaned_data['access_policy'] != Secret.ACCESS_POLICY_ANY:
+            try:
+                secret.share_data.bulk_create(
+                    [
+                        SharedSecretData(
+                            grant_description=form.cleaned_data['grant_description'],
+                            granted_by=self.request.user,
+                            group=group,
+                            secret=secret,
+                        )
+                        for group in form.cleaned_data['shared_groups_on_create']
+                    ]
+                )
+            except UserProfile.DoesNotExist:
+                pass
         return HttpResponseRedirect(secret.get_absolute_url())
 
     def get_context_data(self, **kwargs):
         context = super(SecretAdd, self).get_context_data(**kwargs)
         try:
             context['pretty_content_type'] = CONTENT_TYPE_NAMES[self.kwargs['content_type']]
         except KeyError:
             raise Http404
-        context.update(ACCESS_STR_IDS)
         return context
 
+    def get_initial(self):
+        obj, _created = UserProfile.objects.get_or_create(user=self.request.user)
+        return {'shared_groups_on_create': obj.default_sharing_groups.all()}
+
     def get_form_class(self):
         return CONTENT_TYPE_FORMS[self.kwargs['content_type']]
 
+    def get_form(self, form_class=None):
+        form = super().get_form(form_class=form_class)
+        # handle files with sizes above FILE_UPLOAD_MAX_MEMORY_SIZE setting
+        if (
+                self.content_type == 'file'
+                and self.request.method == 'POST'
+                and not self.request.upload_handlers[0].activated
+        ):
+            form.add_error(
+                f'file', f'File size too big. Allowed file size: {settings.FILE_UPLOAD_MAX_MEMORY_SIZE} bytes'
+            )
+        return form
+
     def get_template_names(self):
-        return "secrets/secret_addedit_{}.html".format(self.kwargs['content_type'])
+        return "secrets/addedit_content/{}.html".format(self.kwargs['content_type'])
+
 
-    def post(self, request, *args, **kwargs):
-        request.POST = _patch_post_data(
-            request.POST,
-            (
-                'allowed_groups',
-                'allowed_users',
-            ),
-        )
-        return super(SecretAdd, self).post(request, *args, **kwargs)
 secret_add = login_required(SecretAdd.as_view())
 
 
 class SecretEdit(UpdateView):
     context_object_name = 'secret'
     slug_field = 'hashid'
     slug_url_kwarg = 'hashid'
 
     def form_valid(self, form):
         secret = self.object
 
-        for attr in ('access_policy', 'description', 'name', 'needs_changing_on_leave', 'url',
-                     'username'):
+        for attr in ('access_policy', 'description', 'name', 'needs_changing_on_leave', 'url', 'username'):
             if attr in form.cleaned_data:
                 setattr(secret, attr, form.cleaned_data[attr])
         secret.save()
 
-        for attr in ('notify_on_access_request',):
-            if form.cleaned_data[attr]:
-                getattr(secret, attr).add(self.request.user)
-            else:
-                getattr(secret, attr).remove(self.request.user)
-
-        for attr in ('allowed_groups', 'allowed_users'):
-            getattr(secret, attr).set(form.cleaned_data[attr])
-
         if secret.content_type == Secret.CONTENT_PASSWORD and form.cleaned_data['password']:
             plaintext_data = form.cleaned_data['password']
         elif secret.content_type == Secret.CONTENT_FILE and form.cleaned_data['file']:
             plaintext_data = form.cleaned_data['file'].read()
             secret.filename = form.cleaned_data['file'].name
             secret.save()
         elif secret.content_type == Secret.CONTENT_CC:
@@ -281,20 +191,32 @@
             secret.set_data(self.request.user, plaintext_data)
 
         return HttpResponseRedirect(secret.get_absolute_url())
 
     def get_context_data(self, **kwargs):
         context = super(SecretEdit, self).get_context_data(**kwargs)
         context['pretty_content_type'] = self.object.get_content_type_display()
-        context.update(ACCESS_STR_IDS)
         return context
 
     def get_form_class(self):
         return CONTENT_TYPE_FORMS[CONTENT_TYPE_IDENTIFIERS[self.object.content_type]]
 
+    def get_form(self, form_class=None):
+        form = super().get_form(form_class=form_class)
+        # handle files with sizes above FILE_UPLOAD_MAX_MEMORY_SIZE setting
+        if (
+                self.content_type == 'file'
+                and self.request.method == 'POST'
+                and not self.request.upload_handlers[0].activated
+        ):
+            form.add_error(
+                f'file', f'File size too big. Allowed file size: {settings.FILE_UPLOAD_MAX_MEMORY_SIZE} bytes'
+            )
+        return form
+
     def get_initial(self):
         if self.object.content_type == Secret.CONTENT_CC:
             data = loads(self.object.get_data(self.request.user))
             return {
                 'holder': data['holder'],
                 'number': data['number'],
                 'expiration_month': data['expiration_month'],
@@ -303,191 +225,339 @@
                 'password': data['password'],
             }
         else:
             return {}
 
     def get_object(self, queryset=None):
         secret = get_object_or_404(Secret, hashid=self.kwargs['hashid'])
-        secret.check_access(self.request.user)
+        secret.check_read_access(self.request.user)
         return secret
 
     def get_template_names(self):
-        return "secrets/secret_addedit_{}.html".format(CONTENT_TYPE_IDENTIFIERS[self.object.content_type])
+        return "secrets/addedit_content/{}.html".format(CONTENT_TYPE_IDENTIFIERS[self.object.content_type])
+
 
-    def post(self, request, *args, **kwargs):
-        request.POST = _patch_post_data(
-            request.POST,
-            (
-                'allowed_groups',
-                'allowed_users',
-            ),
-        )
-        return super(SecretEdit, self).post(request, *args, **kwargs)
 secret_edit = login_required(SecretEdit.as_view())
 
 
 @login_required
 def secret_delete(request, hashid):
     secret = get_object_or_404(Secret, hashid=hashid)
-    secret.check_access(request.user)
+    secret.check_read_access(request.user)
     if request.method == 'POST':
         log(_(
-                "{user} deleted '{name}' ({id}:{revision})"
-            ).format(
-                id=secret.id,
-                name=secret.name,
-                revision=secret.current_revision.id,
-                user=request.user.username,
-            ),
+            "{user} deleted '{name}' ({id}:{revision})"
+        ).format(
+            id=secret.id,
+            name=secret.name,
+            revision=secret.current_revision.id,
+            user=request.user.username,
+        ),
             actor=request.user,
+            category=AuditLogCategoryChoices.SECRET_CHANGED,
             level='info',
             secret=secret,
             secret_revision=secret.current_revision,
         )
         secret.status = Secret.STATUS_DELETED
         secret.save()
-        return HttpResponseRedirect(reverse('secrets.secret-list') + "?" + urlencode([("search", secret.name.encode('utf-8'))]))
+        messages.success(request, _('Successfully deleted secret'))
+        return HttpResponseRedirect(
+            reverse('secrets.secret-list') + "?" + urlencode([("search", secret.name.encode('utf-8'))]))
     else:
         return render(request, "secrets/secret_delete.html", {'secret': secret})
 
 
 @login_required
 @user_passes_test(lambda u: u.is_superuser)
 def secret_restore(request, hashid):
     secret = get_object_or_404(Secret, hashid=hashid)
-    secret.check_access(request.user)
+    secret.check_share_access(request.user)
     if request.method == 'POST':
         log(_(
-                "{user} restore '{name}' ({id}:{revision})"
-            ).format(
-                id=secret.id,
-                name=secret.name,
-                revision=secret.current_revision.id,
-                user=request.user.username,
-            ),
+            "{user} restored '{name}' ({id}:{revision})"
+        ).format(
+            id=secret.id,
+            name=secret.name,
+            revision=secret.current_revision.id,
+            user=request.user.username,
+        ),
             actor=request.user,
+            category=AuditLogCategoryChoices.SECRET_CHANGED,
             level='info',
             secret=secret,
             secret_revision=secret.current_revision,
         )
         secret.status = Secret.STATUS_OK
         secret.save()
-        return HttpResponseRedirect(reverse('secrets.secret-list') + "?" + urlencode([("search", secret.name.encode('utf-8'))]))
+        messages.success(request, _('Successfully restored secret'))
+        return redirect(secret.get_absolute_url())
     else:
         return render(request, "secrets/secret_restore.html", {'secret': secret})
 
 
 @login_required
 @require_http_methods(["GET"])
 def secret_download(request, hashid):
     secret = get_object_or_404(Secret, hashid=hashid)
     if secret.content_type != Secret.CONTENT_FILE:
         raise Http404
-    secret.check_access(request.user)
+    secret.check_read_access(request.user)
 
     response = HttpResponse(secret.get_data(request.user))
     response['Content-Disposition'] = \
         "attachment; filename*=UTF-8''{}".format(quote(secret.filename))
     response['Content-Type'] = "application/force-download"
     return response
 
 
 class SecretDetail(DetailView):
     context_object_name = 'secret'
     model = Secret
     slug_field = 'hashid'
     slug_url_kwarg = 'hashid'
-    template_name = "secrets/secret_detail.html"
 
     def get_context_data(self, **kwargs):
         context = super(SecretDetail, self).get_context_data(**kwargs)
         secret = self.get_object()
         context['content_type'] = CONTENT_TYPE_IDENTIFIERS[secret.content_type]
         context['readable'] = secret.is_readable_by_user(self.request.user)
+        context['shareable'] = secret.is_shareable_by_user(self.request.user)
         context['secret_url'] = reverse(
             'api.secret-revision_data',
             kwargs={'hashid': secret.current_revision.hashid},
         )
+
+        context['show_password_update_alert'] = False
         if context['readable']:
             context['placeholder'] = secret.current_revision.length * "•"
-        else:
-            try:
-                context['access_request'] = AccessRequest.objects.get(
-                    secret=secret,
-                    status=AccessRequest.STATUS_PENDING,
-                    requester=self.request.user,
-                )
-            except AccessRequest.DoesNotExist:
-                context['access_request'] = None
+            if context['readable'] == AccessPermissionTypes.SUPERUSER_ALLOWED:
+                context['su_access'] = True
+            if secret.status == Secret.STATUS_NEEDS_CHANGING and settings.PASSWORD_UPDATE_ALERT_ACTIVATED:
+                context['show_password_update_alert'] = True
         return context
 
-    def get_object(self):
+    def get_object(self, queryset=None):
         object = super(SecretDetail, self).get_object()
         if not object.is_visible_to_user(self.request.user):
             raise Http404
         return object
-secret_detail = login_required(SecretDetail.as_view())
 
+    def get_template_names(self):
+        content_type = CONTENT_TYPE_IDENTIFIERS[self.object.content_type]
+        return f'secrets/detail_content/{content_type}.html'
 
-class SecretFilter(django_filters.FilterSet):
-    order = django_filters.OrderingFilter(
-        choices=(
-            ('last_changed', _("Last changed")),
-            ('last_read', _("Last read")),
-        ),
-    )
 
-    class Meta:
-        model = Secret
-        fields = {
-            'last_changed': ['gt', 'gte', 'lt', 'lte'],
-            'last_read': ['gt', 'gte', 'lt', 'lte'],
-        }
+secret_detail = login_required(SecretDetail.as_view())
+
+
+@login_required
+@require_http_methods(["GET"])
+def secret_metadata(request, hashid):
+    secret = get_object_or_404(Secret, hashid=hashid)
+    share_data = secret.share_data.with_expiry_state().filter(is_expired=False)
+    context = {
+        'allowed_groups': share_data.groups(),
+        'allowed_users': share_data.users(),
+        'secret': secret,
+    }
+    return render(request, context=context, template_name='secrets/detail_content/meta.html')
 
 
 class SecretList(ListView):
     context_object_name = 'secrets'
+    filter = None
     paginate_by = 25
     template_name = "secrets/secret_list.html"
 
     def get_context_data(self, **kwargs):
         context = super(SecretList, self).get_context_data(**kwargs)
+        context['filter'] = self.filter
         context['readable_secrets'] = Secret.get_all_readable_by_user(self.request.user)
         return context
 
     def get_queryset(self):
         if "search" in self.request.GET:
             queryset = Secret.get_search_results(self.request.user, self.request.GET['search'])
         else:
             queryset = Secret.get_all_visible_to_user(self.request.user)
-        filtered = SecretFilter(self.request.GET, queryset)
-        return filtered.qs
+
+        try:
+            if '3' not in self.request.GET.get('status', []) and self.request.user.profile.hide_deleted_secrets:
+                queryset = queryset.exclude(status=Secret.STATUS_DELETED)
+        except ObjectDoesNotExist:
+            pass
+
+        self.filter = SecretFilter(self.request.GET, queryset)
+        return self.filter.qs
+
+
 secret_list = login_required(SecretList.as_view())
 
 
+class SecretShareList(CreateView):
+    form_class = SecretShareForm
+    slug_field = 'secret__hashid'
+    slug_url_kwarg = 'hashid'
+    template_name = 'secrets/share_content/share_list_modal.html'
+
+    @cached_property
+    def group_shares(self):
+        if not self.queryset:
+            self.queryset = self.get_queryset().with_expiry_state()
+        return self.queryset.groups()
+
+    @cached_property
+    def user_shares(self):
+        if not self.queryset:
+            self.queryset = self.get_queryset().with_expiry_state()
+        return self.queryset.users()
+
+    def get_queryset(self):
+        return SharedSecretData.objects.filter(
+            secret__hashid=self.kwargs[self.slug_url_kwarg]
+        ).prefetch_related('secret', 'user', 'group')
+
+    def get_context_data(self, *, object_list=None, **kwargs):
+        secret = get_object_or_404(Secret, hashid=self.kwargs[self.slug_url_kwarg])
+
+        context = {
+            'secret': secret,
+            'shareable': secret.is_shareable_by_user(self.request.user),
+            'shares': {
+                'groups': self.group_shares,
+                'users': self.user_shares,
+            },
+        }
+        return super().get_context_data(**context)
+
+    def form_valid(self, form):
+        secret = Secret.objects.get(hashid=self.kwargs[self.slug_url_kwarg])
+        permission = secret.is_shareable_by_user(self.request.user)
+        if not permission:
+            raise PermissionDenied()
+
+        form_obj = form.save(commit=False)
+        obj = secret.share(
+            grant_description=form_obj.grant_description,
+            granted_by=self.request.user,
+            granted_until=form_obj.granted_until,
+            group=form_obj.group,
+            user=form_obj.user,
+        )
+
+        messages.success(self.request, _('Shared secret with {}'.format(obj.shared_entity_name)))
+
+        # Clear cache
+        delattr(self, 'group_shares')
+        delattr(self, 'user_shares')
+
+        context = self.get_context_data()
+        context.update({
+            'form': self.get_form_class()(),  # create a new blank form
+            'show_object': {
+                'id': obj.shared_entity.id,
+                'type': 'group' if form.cleaned_data['group'] else 'user',
+            }
+        })
+        response = self.render_to_response(context=context)
+        trigger_client_event(response, 'refreshMetadata')
+        return response
+
+    def get_form_class(self):
+        form_class = super(SecretShareList, self).get_form_class()
+
+        # Exclude groups and users which the secret was already shared with
+        form_class.base_fields['group'].queryset = Group.objects.all().exclude(
+            name__in=self.group_shares.values_list('group__name', flat=True)
+        ).order_by('name')
+        form_class.base_fields['user'].queryset = User.objects.filter(is_active=True).order_by('username').exclude(
+            username__in=self.user_shares.values_list('user__username', flat=True)
+        ).order_by('username')
+        return form_class
+
+
+secret_share_list = login_required(SecretShareList.as_view())
+
+
+@login_required
+@require_http_methods(['DELETE'])
+def secret_share_delete(request, hashid, share_id):
+    share_data = get_object_or_404(SharedSecretData, secret__hashid=hashid, id=share_id)
+    permission = share_data.secret.is_shareable_by_user(request.user)
+    if not permission:
+        raise PermissionDenied()
+
+    secret = share_data.secret
+    entity_type = share_data.shared_entity_type
+    entity_name = share_data.shared_entity_name
+    share_data.delete()
+
+    messages.success(
+        request,
+        _('Successfully removed {} from allowed {}'.format(
+            share_data.shared_entity_name, pluralize(share_data.shared_entity_type)
+        ))
+    )
+    log(
+        _("{user} removed access of {shared_entity_type} '{name}'").format(
+            shared_entity_type=entity_type,
+            name=entity_name,
+            user=request.user.username,
+        ),
+        actor=request.user,
+        category=(
+            AuditLogCategoryChoices.SECRET_SUPERUSER_SHARE_REMOVED
+            if permission == AccessPermissionTypes.SUPERUSER_ALLOWED
+            else AuditLogCategoryChoices.SECRET_SHARE_REMOVED
+        ),
+        level='warning',
+        secret=secret,
+    )
+    response = HttpResponse(status=200)
+    trigger_client_event(response, 'refreshMetadata')
+    trigger_client_event(response, 'refreshShareData')
+    return response
+
+
 @login_required
 @require_http_methods(["GET"])
 def secret_search(request):
     search_term = request.GET['q']
-    search_result = []
-    filtered_secrets = list(Secret.get_search_results(request.user, search_term, limit=10))
+    search_limit = request.GET.get('limit', 15)
+    search_results = []
+    raw_results = Secret.get_search_results(request.user, search_term)
+    filtered_secrets = list(raw_results[:search_limit])
     unreadable_secrets = filtered_secrets[:]
     sorted_secrets = []
 
     # sort readable passwords to top...
     for secret in filtered_secrets:
+        metadata = ''
+        icon = "lock-open"
         if secret.is_readable_by_user(request.user):
-            sorted_secrets.append((secret, "unlock"))
+            if secret.content_type == secret.CONTENT_PASSWORD:
+                icon = "user"
+                metadata = getattr(secret, 'username')
+            elif secret.content_type == secret.CONTENT_FILE:
+                icon = "file"
+                metadata = getattr(secret, 'filename')
+            elif secret.content_type == secret.CONTENT_CC:
+                icon = "credit-card"
+                metadata = getattr(secret, 'description')
+            sorted_secrets.append((secret, icon, metadata))
             unreadable_secrets.remove(secret)
 
     # and others to the bottom
     for secret in unreadable_secrets:
-        sorted_secrets.append((secret, "lock"))
+        sorted_secrets.append((secret, "lock", ''))
 
-    for secret, icon in sorted_secrets:
-        search_result.append({
+    for secret, icon, metadata in sorted_secrets:
+        search_results.append({
+            'icon': icon,
+            'meta': metadata,
             'name': secret.name,
+            'locked': True if icon == 'lock' else False,
+            'hashid': secret.hashid,
             'url': reverse('secrets.secret-detail', kwargs={'hashid': secret.hashid}),
-            'icon': icon,
         })
-
-    return HttpResponse(dumps(search_result), content_type="application/json")
+    return JsonResponse({'count': raw_results.count(), 'results': search_results})
```

### Comparing `teamvault-0.9.2/teamvault/apps/settings/config.py` & `teamvault-1.0.0rc3/teamvault/apps/settings/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 from base64 import b64decode, b64encode
-from configparser import SafeConfigParser
+from configparser import ConfigParser
 from gettext import gettext as _
 from hashlib import sha1
 from os import environ, umask
 from os.path import exists, isfile
 from random import choice
 from string import ascii_letters, digits, punctuation
 from urllib.parse import urlparse
 
 from cryptography.fernet import Fernet
+from django.core.exceptions import ImproperlyConfigured
 from django.db.utils import ProgrammingError
 
 
+class UnconfiguredSettingsError(Exception):
+    def __str__(self):
+        return _(
+            "missing config file at {} (set env var TEAMVAULT_CONFIG_FILE to use a different path)"
+        ).format(environ['TEAMVAULT_CONFIG_FILE'])
+
+
 def configure_base_url(config, settings):
     settings.BASE_URL = config.get("teamvault", "base_url")
     settings.ALLOWED_HOSTS = [urlparse(settings.BASE_URL).hostname]
 
 
 def configure_database(config):
     """
@@ -56,27 +64,42 @@
     """
     return (
         int(get_from_config(config, "hashid", "min_length", "6")),
         b64decode(config.get("hashid", "salt").encode()).decode('utf-8'),
     )
 
 
+def configure_password_generator(config, settings):
+    settings.PASSWORD_LENGTH = int(get_from_config(config, "password_generator", "length", 16))
+    settings.PASSWORD_DIGITS = int(get_from_config(config, "password_generator", "digits", 2))
+    settings.PASSWORD_UPPER = int(get_from_config(config, "password_generator", "upper", 2))
+    settings.PASSWORD_LOWER = int(get_from_config(config, "password_generator", "lower", 2))
+    settings.PASSWORD_SPECIAL = int(get_from_config(config, "password_generator", "special", 2))
+
+    char_sum = settings.PASSWORD_SPECIAL + settings.PASSWORD_LOWER + settings.PASSWORD_UPPER + settings.PASSWORD_DIGITS
+
+    if char_sum > settings.PASSWORD_LENGTH:
+        raise ImproperlyConfigured(_(
+            'The sum of characters defined in password settings exceeds the value set in password_length setting'
+        ))
+
+
 def configure_google_auth(config, settings):
     if not config.has_section("auth_google"):
         settings.GOOGLE_AUTH_ENABLED = False
         return
 
     settings.GOOGLE_AUTH_ENABLED = True
 
     settings.AUTHENTICATION_BACKENDS.insert(
         0,
         'social_core.backends.google.GoogleOAuth2',
     )
 
-    settings.SOCIAL_AUTH_PIPELINE = (
+    settings.SOCIAL_AUTH_PIPELINE = [
         # Get the information we can about the user and return it in a simple
         # format to create the user instance later. In some cases the details are
         # already part of the auth response from the provider, but sometimes this
         # could hit a provider API.
         'social_core.pipeline.social_auth.social_details',
 
         # Get the social uid from whichever service we're authing thru. The uid is
@@ -92,38 +115,106 @@
         'social_core.pipeline.social_auth.social_user',
 
         # Associates the current social details with another user account with
         # a similar email address.
         'social_core.pipeline.social_auth.associate_by_email',
 
         # Create a user account if we haven't found one yet.
+        # Also see comment below for LDAP compatibility
         'social_core.pipeline.user.create_user',
 
         # Create the record that associates the social account with the user.
         'social_core.pipeline.social_auth.associate_user',
 
         # Populate the extra_data field in the social record with the values
         # specified by settings (and the default ones like access_token, etc).
         'social_core.pipeline.social_auth.load_extra_data',
 
         # Update the user record with any changed info from the auth service.
         'social_core.pipeline.user.user_details',
-
-        # Get groups from LDAP
-        'teamvault.apps.accounts.auth.populate_from_ldap',
-    )
+    ]
 
     settings.SOCIAL_AUTH_GOOGLE_OAUTH2_WHITELISTED_DOMAINS = [
         domain.strip() for domain in
         config.get("auth_google", "allowed_domains").split(",")
     ]
 
+    settings.GOOGLE_AUTH_AVATARS = get_from_config(config, "auth_google", "use_avatars", True)
+    if settings.GOOGLE_AUTH_AVATARS:
+        settings.SOCIAL_AUTH_PIPELINE.append('teamvault.apps.accounts.utils.save_google_avatar')
+    else:
+        settings.SOCIAL_AUTH_PIPELINE.append('teamvault.apps.accounts.utils.save_gravatar')
+
     settings.SOCIAL_AUTH_GOOGLE_OAUTH2_KEY = config.get("auth_google", "oauth2_key")
     settings.SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET = config.get("auth_google", "oauth2_secret")
 
+    # LDAP compatibility settings
+    if config.has_section("auth_ldap"):
+        settings.SOCIAL_AUTH_PIPELINE.append('teamvault.apps.accounts.auth.populate_from_ldap')
+
+        if get_from_config(config, "auth_google", "use_ldap_usernames", False):
+            # Social Auth tries to create users with usernames by stripping the domain part of their email address.
+            # This behaviour clashes when these usernames differ from the ones in a configured LDAP directory.
+            # We cannot use "SOCIAL_AUTH_CLEAN_USERNAME_FUNCTION" here, because Social Auth only provides the username
+            # of our chosen storage provider and not the full email address.
+            settings.SOCIAL_AUTH_PIPELINE.insert(
+                # Username fix has to happen before "social_core.pipeline.user.create_user".
+                settings.SOCIAL_AUTH_PIPELINE.index('social_core.pipeline.user.create_user'),
+                'teamvault.apps.accounts.auth.find_ldap_username_for_social_auth'
+            )
+
+
+def configure_huey(config):
+    # For now, all tasks use the same crontab value. They're all
+    # background maintenance task at the moment.
+    freq = get_from_config(config, "tasks", "scheduler_frequency", "daily")
+    if freq == "daily":
+        scheduler_frequency = {
+            'day': '*/1',
+            'hour': '0',
+            'minute': '0',
+        }
+    elif freq == "hourly":
+        scheduler_frequency = {
+            'hour': '*/1',
+            'minute': '0',
+        }
+    elif freq == "minutely":
+        scheduler_frequency = {
+            'minute': '*/1',
+        }
+    else:
+        raise RuntimeError(_(
+            "Unknown value {freq} for task.scheduler_frequency in {path}"
+        ).format(
+            freq=freq,
+            path=environ['TEAMVAULT_CONFIG_FILE'],
+        ))
+
+    revoke = get_from_config(
+        config,
+        "tasks",
+        "revoke_unused_shares_after_days",
+        None,
+    )
+    if not revoke is None:
+        try:
+            revoke = int(revoke)
+        except ValueError:
+            raise RuntimeError(_(
+                "task.revoke_unused_shares_after_days must be an integer in {path}"
+            ).format(
+                path=environ['TEAMVAULT_CONFIG_FILE'],
+            ))
+
+    return {
+        'revoke_unused_shares_after_days': revoke,
+        'scheduler_frequency': scheduler_frequency,
+    }
+
 
 def configure_ldap_auth(config, settings):
     if not config.has_section("auth_ldap"):
         settings.LDAP_AUTH_ENABLED = False
         return
 
     settings.LDAP_AUTH_ENABLED = True
@@ -197,15 +288,15 @@
         settings.AUTH_LDAP_CONNECTION_OPTIONS[OPT_X_TLS_NEWCTX] = 0
 
 
 def configure_logging(config):
     level = 'INFO'
 
     if get_from_config(config, "teamvault", "insecure_debug_mode", "no").lower() in \
-        ("1", "enabled", "true", "yes"):
+            ("1", "enabled", "true", "yes"):
         level = 'DEBUG'
 
     LOGGING = {
         'version': 1,
         'disable_existing_loggers': False,
         'formatters': {
             'console': {
@@ -218,15 +309,15 @@
                 'level': 'DEBUG',
                 'class': 'logging.StreamHandler',
             },
         },
         'loggers': {
             'django': {
                 'handlers': ['console'],
-                'level': level,
+                'level': 'INFO',
             },
             'django_auth_ldap': {
                 'handlers': ['console'],
                 'level': level,
             },
             'teamvault': {
                 'handlers': ['console'],
@@ -241,14 +332,21 @@
 def configure_max_file_size(config, settings):
     settings.TEAMVAULT_MAX_FILE_SIZE = int(
         get_from_config(config, "teamvault", "max_file_size", "5242880")
     )
     settings.FILE_UPLOAD_MAX_MEMORY_SIZE = settings.TEAMVAULT_MAX_FILE_SIZE
 
 
+def configure_password_update_alert(config, settings):
+    equivalent_true_values = ["1", "true", "enabled", "yes"]
+
+    password_update_alert_value = get_from_config(config, "teamvault", "password_update_alert_activated", False)
+    settings.PASSWORD_UPDATE_ALERT_ACTIVATED = str(password_update_alert_value).lower() in equivalent_true_values
+
+
 def configure_session(config):
     """
     Called directly from the Django settings module.
     """
     age = int(get_from_config(config, "teamvault", "session_cookie_age", "3600"))
     expire = get_from_config(config, "teamvault", "session_expire_at_browser_close", "True")
     secure = get_from_config(config, "teamvault", "session_cookie_secure", "False")
@@ -257,14 +355,20 @@
         age = 3600
     expire = expire.lower() in ("1", "enabled", "true", "yes")
     secure = secure.lower() in ("1", "enabled", "true", "yes")
 
     return age, expire, secure
 
 
+def configure_superuser_reads(config, settings):
+    settings.ALLOW_SUPERUSER_READS = False
+    if get_from_config(config, "teamvault", "allow_superuser_reads", "False").lower() in ("1", "enabled", "true", "yes"):
+        settings.ALLOW_SUPERUSER_READS = True
+
+
 def configure_teamvault_secret_key(config, settings):
     from .models import Setting
 
     key = config.get("teamvault", "fernet_key")
 
     try:
         checksum = Setting.get("fernet_key_hash", default=None)
@@ -283,14 +387,27 @@
                 hash=checksum,
                 path=environ['TEAMVAULT_CONFIG_FILE'],
             ))
 
     settings.TEAMVAULT_SECRET_KEY = key
 
 
+def configure_time_zone(config):
+    return get_from_config(config, "teamvault", "time_zone", "UTC")
+
+
+def configure_whitenoise(settings):
+    if not settings.DEBUG:
+        settings.STORAGES = {
+            'staticfiles': {
+                'BACKEND': 'whitenoise.storage.StaticFilesStorage'
+            }
+        }
+
+
 def create_default_config(filename):
     if exists(filename):
         raise RuntimeError("not overwriting existing path {}".format(filename))
     SECRET_KEY = "".join(choice(ascii_letters + digits + punctuation) for i in range(50))
     HASHID_SALT = "".join(choice(ascii_letters + digits + punctuation) for i in range(50))
     config = """
 [teamvault]
@@ -301,14 +418,23 @@
 # do not enable this in production
 insecure_debug_mode = disabled
 # file uploads larger than this number of bytes will have their connection reset
 max_file_size = 5242880
 session_cookie_age = 3600
 session_expire_at_browser_close = True
 session_cookie_secure = False
+time_zone = UTC
+# allow_superuser_reads = False
+
+#[password_generator]
+#length = 16
+#digits = 2
+#upper = 2
+#lower = 2
+#special = 2
 
 [django]
 # This key has been generated for you, there is no need to change it
 secret_key = {django_key}
 
 [database]
 host = localhost
@@ -339,14 +465,19 @@
 ##attr_last_name = sn
 #admin_group = cn=admins,ou=groups,dc=example,dc=com
 
 #[auth_google]
 #allowed_domains = example.com, another.example.com
 #oauth2_key = 123456789.apps.googleusercontent.com
 #oauth2_secret = ******************
+#use_avatars = True
+
+#[tasks]
+#scheduler_frequency = daily  # or hourly, minutely
+#revoke_unused_shares_after_days = 365  # task disabled if unset
     """.format(
         django_key=b64encode(SECRET_KEY.encode('utf-8')).decode('utf-8'),
         hashid_salt=b64encode(HASHID_SALT.encode('utf-8')).decode('utf-8'),
         teamvault_key=Fernet.generate_key().decode('utf-8'),
     )
     old_umask = umask(7)
     try:
@@ -354,27 +485,22 @@
             f.write(config.strip())
     finally:
         umask(old_umask)
 
 
 def get_config():
     if not isfile(environ['TEAMVAULT_CONFIG_FILE']):
-        raise RuntimeError(
-            _("missing config file at {} "
-              "(set env var TEAMVAULT_CONFIG_FILE to use a different path)").format(
-                environ['TEAMVAULT_CONFIG_FILE'],
-            )
-        )
+        raise UnconfiguredSettingsError()
 
     with open(environ['TEAMVAULT_CONFIG_FILE']) as f:
-        # SafeConfigParser.read() will not complain if it can't read the
+        # ConfigParser.read() will not complain if it can't read the
         # file, so we need to read it once ourselves to get a proper IOError
         f.read()
 
-    config = SafeConfigParser()
+    config = ConfigParser()
     config.read(environ['TEAMVAULT_CONFIG_FILE'])
     return config
 
 
 def get_from_config(config, section, option, default):
     if config.has_option(section, option):
         return config.get(section, option)
```

### Comparing `teamvault-0.9.2/teamvault/apps/settings/migrations/0001_initial.py` & `teamvault-1.0.0rc3/teamvault/apps/settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `teamvault-0.9.2/teamvault/apps/settings/models.py` & `teamvault-1.0.0rc3/teamvault/apps/settings/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class Setting(models.Model):
     key = models.CharField(
         max_length=64,
         unique=True,
     )
```

### Comparing `teamvault-0.9.2/teamvault/cli.py` & `teamvault-1.0.0rc3/teamvault/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,62 @@
-from argparse import ArgumentParser
+from argparse import ArgumentParser, REMAINDER
 from gettext import gettext as _
 from hashlib import sha1
 from os import environ, mkdir
 from shutil import rmtree
 from subprocess import Popen
 from sys import argv
 
-from django.core.management import execute_from_command_line
+import django
+from django.core.management import execute_from_command_line, get_commands
 
-from .apps.settings.config import create_default_config
-from . import VERSION_STRING
+from teamvault.__version__ import __version__
+from teamvault.apps.settings.config import create_default_config, UnconfiguredSettingsError
 
 
 def build_parser():
     parser = ArgumentParser(prog="teamvault")
     parser.add_argument(
         "--version",
         action='version',
-        version=VERSION_STRING,
+        version=__version__,
     )
     subparsers = parser.add_subparsers(
         title=_("subcommands"),
         help=_("use 'teamvault <subcommand> --help' for more info"),
     )
 
+    environ['DJANGO_SETTINGS_MODULE'] = 'teamvault.settings'
+    environ.setdefault("TEAMVAULT_CONFIG_FILE", "/etc/teamvault.cfg")
+
     # teamvault plumbing
+    unconfigured_settings = False
+    try:
+        django.setup()
+    except UnconfiguredSettingsError:
+        unconfigured_settings = True
+
+    commands = [k for k in get_commands()]
+    plumbing_help = f'One of: {",".join(commands)}'
+    if unconfigured_settings:
+        plumbing_help += " - To see all available commands, configure teamvault settings with \"teamvault setup\""
+
     parser_plumbing = subparsers.add_parser("plumbing")
-    parser_plumbing.add_argument('plumbing_command', nargs='+')
+    parser_plumbing.add_argument('plumbing_command', nargs=REMAINDER, help=plumbing_help)
     parser_plumbing.set_defaults(func=plumbing)
 
     # teamvault run
     parser_run = subparsers.add_parser("run")
     parser_run.add_argument('--bind', nargs='?', help='define bind, default is 127.0.0.1:8000')
     parser_run.set_defaults(func=run)
 
+    # teamvault run_huey
+    parser_run = subparsers.add_parser("run_huey")
+    parser_run.set_defaults(func=run_huey)
+
     # teamvault setup
     parser_setup = subparsers.add_parser("setup")
     parser_setup.set_defaults(func=setup)
 
     # teamvault upgrade
     parser_upgrade = subparsers.add_parser("upgrade")
     parser_upgrade.set_defaults(func=upgrade)
@@ -58,31 +77,34 @@
     if not hasattr(pargs, 'func'):
         parser.print_help()
         exit(2)
     pargs.func(pargs)
 
 
 def plumbing(pargs):
-    environ['DJANGO_SETTINGS_MODULE'] = 'teamvault.settings'
-    environ.setdefault("TEAMVAULT_CONFIG_FILE", "/etc/teamvault.cfg")
-    execute_from_command_line([""] + pargs.plumbing_command[0].split(" "))
+    execute_from_command_line([""] + pargs.plumbing_command)
 
 
 def run(pargs):
     cmd = "gunicorn --preload teamvault.wsgi:application"
     if pargs.bind:
         cmd += ' -b ' + pargs.bind
 
+    print("Now open http://localhost:8000")
     gunicorn = Popen(
         cmd,
         shell=True,
     )
     gunicorn.communicate()
 
 
+def run_huey(pargs):
+    execute_from_command_line(["", "run_huey"])
+
+
 def setup(pargs):
     environ.setdefault("TEAMVAULT_CONFIG_FILE", "/etc/teamvault.cfg")
     create_default_config(environ['TEAMVAULT_CONFIG_FILE'])
 
 
 def upgrade(pargs):
     environ['DJANGO_SETTINGS_MODULE'] = 'teamvault.settings'
```

### Comparing `teamvault-0.9.2/teamvault/settings.py` & `teamvault-1.0.0rc3/teamvault/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from os.path import dirname, join, realpath
 
+from huey import SqliteHuey
+
 from .apps.settings.config import (
     configure_database,
     configure_django_secret_key,
     configure_hashid,
+    configure_huey,
     configure_logging,
+    configure_password_generator,
     configure_session,
+    configure_time_zone,
     get_config,
+    get_from_config,
 )
 
 CONFIG = get_config()
 PROJECT_ROOT = realpath(dirname(__file__))
 
-### Django
+# Django
 
 AUTHENTICATION_BACKENDS = [
     'django.contrib.auth.backends.ModelBackend',
 ]
 
 DATABASES = configure_database(CONFIG)
 
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
+
 FILE_UPLOAD_HANDLERS = (
     "teamvault.apps.secrets.utils.CappedMemoryFileUploadHandler",
 )
 
 FIXTURE_DIRS = (
     join(PROJECT_ROOT, "fixtures"),
 )
@@ -31,21 +39,23 @@
 INSTALLED_APPS = [
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.humanize',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
-    'django_gravatar',
+    'django_bootstrap5',
+    'huey.contrib.djhuey',
     'rest_framework',
     'social_django',
     'teamvault.apps.accounts.AccountsConfig',
     'teamvault.apps.audit.AuditConfig',
     'teamvault.apps.secrets.SecretsConfig',
     'teamvault.apps.settings.SettingsConfig',
+    'webpack_loader',
 ]
 
 LANGUAGE_CODE = "en-us"
 
 LOCALE_PATHS = (PROJECT_ROOT + "/locale",)
 
 LOGIN_REDIRECT_URL = "/"
@@ -60,14 +70,15 @@
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.locale.LocaleMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
+    'teamvault.middleware.htmx_message_middleware',
 ]
 
 ROOT_URLCONF = "teamvault.urls"
 
 SECRET_KEY = configure_django_secret_key(CONFIG)
 
 SECURE_PROXY_SSL_HEADER = ("HTTP_X_FORWARDED_PROTO", "https")
@@ -81,59 +92,65 @@
 # remember this is hardcoded in the error page templates (e.g. 500.html)
 STATIC_URL = "/static/"
 
 STATICFILES_DIRS = (
     join(PROJECT_ROOT, "static"),
 )
 
-STATICFILES_STORAGE = 'whitenoise.storage.CompressedManifestStaticFilesStorage'
-
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [join(PROJECT_ROOT, "templates"),],
+        'DIRS': [join(PROJECT_ROOT, "templates"), ],
         'APP_DIRS': True,
         'OPTIONS': {
             'context_processors': [
                 'django.contrib.auth.context_processors.auth',
+                'django.contrib.messages.context_processors.messages',
                 'django.template.context_processors.csrf',
                 'django.template.context_processors.debug',
                 'django.template.context_processors.i18n',
                 'django.template.context_processors.media',
                 'django.template.context_processors.request',
                 'django.template.context_processors.static',
                 'teamvault.apps.accounts.context_processors.google_auth_enabled',
-                'teamvault.apps.secrets.context_processors.access_request_count',
                 'teamvault.apps.secrets.context_processors.version',
             ],
         },
     },
 ]
 
 TEST_RUNNER = 'django.test.runner.DiscoverRunner'
 
-TIME_ZONE = 'UTC'
+TIME_ZONE = configure_time_zone(CONFIG)
 
 USE_I18N = False
-USE_L10N = True
 USE_THOUSAND_SEPARATOR = False
 USE_TZ = True
 
-### Hashid
-
+# HashID
 HASHID_MIN_LENGTH, HASHID_SALT = configure_hashid(CONFIG)
 
-### REST Framework
-
+# Django REST Framework
 REST_FRAMEWORK = {
     'DEFAULT_MODEL_SERIALIZER_CLASS':
         'rest_framework.serializers.HyperlinkedModelSerializer',
     'DEFAULT_PAGINATION_CLASS': 'rest_framework.pagination.PageNumberPagination',
     'DEFAULT_PERMISSION_CLASSES': (
         'rest_framework.permissions.IsAuthenticated',
     ),
     'PAGE_SIZE': 25,
 }
 
-### Social Auth
+# Social Auth
+SOCIAL_AUTH_JSONFIELD_ENABLED = True
+
+# Django-Bootstrap5
+BOOTSTRAP5 = {
+    'horizontal_field_class': 'col-xl-8',
+    'horizontal_label_class': 'col-xl-2',
+    'required_css_class': 'required',
+    'success_css_class': 'is-valid',
+    'error_css_class': 'is-invalid',
+}
 
-SOCIAL_AUTH_POSTGRES_JSONFIELD = True
+HUEY = SqliteHuey('teamvault')
+HUEY_TASKS = configure_huey(CONFIG)
```

### Comparing `teamvault-0.9.2/teamvault/templates/404_loggedin.html` & `teamvault-1.0.0rc3/teamvault/templates/404_loggedin.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-{% extends "base_nav.html" %}
+{% extends "base.html" %}
 {% load static %}
 {% load i18n %}
-{% block "title" %}{% trans "Page not found" %}{% endblock %}
-{% block "nav_search" %}active{% endblock %}
-{% block "content" %}
+{% block title %}{% trans "Page not found" %}{% endblock %}
+{% block nav_search %}active{% endblock %}
+{% block content %}
 <div class="container">
 	<div class="row">
 		<div class="col-md-8 col-md-offset-2">
 			<h1>{% trans "404 - Page Not Found" %}</h1>
 			<br>
 			<p>{% trans "Sorry, the page you requested couldn't be found." %}</p>
 			<p>{% trans "If you expected a secret here, you may need to ask someone to grant you access." %}</p>
```

