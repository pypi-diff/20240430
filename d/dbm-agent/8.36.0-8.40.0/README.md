# Comparing `tmp/dbm-agent-8.36.0.tar.gz` & `tmp/dbm-agent-8.40.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm-agent-8.36.0.tar", last modified: Fri Mar 29 03:17:17 2024, max compression
+gzip compressed data, was "dbm-agent-8.40.0.tar", last modified: Tue Apr 30 09:53:40 2024, max compression
```

## Comparing `dbm-agent-8.36.0.tar` & `dbm-agent-8.40.0.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.799689 dbm-agent-8.36.0/
--rw-r--r--   0 root         (0) root         (0)      626 2024-03-29 03:17:17.798689 dbm-agent-8.36.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7740 2023-07-21 12:27:33.000000 dbm-agent-8.36.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.776689 dbm-agent-8.36.0/bin/
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-30 12:35:14.000000 dbm-agent-8.36.0/bin/dbm-agent
--rw-r--r--   0 root         (0) root         (0)      322 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/bin/dbm-bt-conn-stack
--rw-r--r--   0 root         (0) root         (0)      887 2023-06-30 12:35:07.000000 dbm-agent-8.36.0/bin/dbma-cli-init
--rw-r--r--   0 root         (0) root         (0)     2671 2023-06-30 12:38:52.000000 dbm-agent-8.36.0/bin/dbma-cli-mysql
--rw-r--r--   0 root         (0) root         (0)     2321 2023-06-30 12:34:44.000000 dbm-agent-8.36.0/bin/dbma-cli-redis
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.777689 dbm-agent-8.36.0/dbm_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      626 2024-03-29 03:17:17.000000 dbm-agent-8.36.0/dbm_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2314 2024-03-29 03:17:17.000000 dbm-agent-8.36.0/dbm_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 03:17:17.000000 dbm-agent-8.36.0/dbm_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2024-03-29 03:17:17.000000 dbm-agent-8.36.0/dbm_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      252 2024-03-29 03:17:17.000000 dbm-agent-8.36.0/dbm_agent.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.777689 dbm-agent-8.36.0/dbma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.779689 dbm-agent-8.36.0/dbma/bil/
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/bil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/bil/cmdexecutor.py
--rw-r--r--   0 root         (0) root         (0)     3764 2023-05-27 07:30:34.000000 dbm-agent-8.36.0/dbma/bil/daemon.py
--rw-r--r--   0 root         (0) root         (0)     3959 2023-06-30 06:41:17.000000 dbm-agent-8.36.0/dbma/bil/fs.py
--rw-r--r--   0 root         (0) root         (0)      223 2023-05-27 07:30:39.000000 dbm-agent-8.36.0/dbma/bil/fun.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/bil/net.py
--rw-r--r--   0 root         (0) root         (0)     6795 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/bil/osuser.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/bil/sudos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.781689 dbm-agent-8.36.0/dbma/components/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.785689 dbm-agent-8.36.0/dbma/components/mysql/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/components/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2647 2023-05-29 11:59:15.000000 dbm-agent-8.36.0/dbma/components/mysql/asserts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.786689 dbm-agent-8.36.0/dbma/components/mysql/backends/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-18 14:11:07.000000 dbm-agent-8.36.0/dbma/components/mysql/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7758 2023-07-04 12:23:24.000000 dbm-agent-8.36.0/dbma/components/mysql/backends/clears.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.786689 dbm-agent-8.36.0/dbma/components/mysql/backups/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/components/mysql/backups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-27 07:26:51.000000 dbm-agent-8.36.0/dbma/components/mysql/backups/cloneplugin.py
--rw-r--r--   0 root         (0) root         (0)     9680 2024-03-28 14:58:25.000000 dbm-agent-8.36.0/dbma/components/mysql/commons.py
--rw-r--r--   0 root         (0) root         (0)    15760 2024-03-29 03:12:51.000000 dbm-agent-8.36.0/dbma/components/mysql/config.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-08-01 08:11:48.000000 dbm-agent-8.36.0/dbma/components/mysql/deploy.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-07-11 09:27:16.000000 dbm-agent-8.36.0/dbma/components/mysql/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14693 2023-07-18 06:49:24.000000 dbm-agent-8.36.0/dbma/components/mysql/install.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-05-27 07:26:20.000000 dbm-agent-8.36.0/dbma/components/mysql/instance.py
--rw-r--r--   0 root         (0) root         (0)     3994 2023-05-27 07:26:23.000000 dbm-agent-8.36.0/dbma/components/mysql/replica.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-05-27 07:26:29.000000 dbm-agent-8.36.0/dbma/components/mysql/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.787689 dbm-agent-8.36.0/dbma/components/mysql/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/components/mysql/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13668 2023-07-04 14:24:35.000000 dbm-agent-8.36.0/dbma/components/mysql/views/defaultsview.py
--rw-r--r--   0 root         (0) root         (0)     4373 2023-05-27 07:26:44.000000 dbm-agent-8.36.0/dbma/components/mysql/views/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.788689 dbm-agent-8.36.0/dbma/components/orchestrator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/components/orchestrator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-27 07:26:58.000000 dbm-agent-8.36.0/dbma/components/orchestrator/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-05-27 07:27:01.000000 dbm-agent-8.36.0/dbma/components/orchestrator/install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.790689 dbm-agent-8.36.0/dbma/components/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/components/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1623 2023-05-27 07:27:34.000000 dbm-agent-8.36.0/dbma/components/redis/commons.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-05-27 07:27:09.000000 dbm-agent-8.36.0/dbma/components/redis/config.py
--rw-r--r--   0 root         (0) root         (0)      548 2023-05-27 07:27:39.000000 dbm-agent-8.36.0/dbma/components/redis/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7269 2023-07-21 12:27:33.000000 dbm-agent-8.36.0/dbma/components/redis/install.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-05-27 07:27:52.000000 dbm-agent-8.36.0/dbma/components/redis/systemd.py
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-27 07:27:57.000000 dbm-agent-8.36.0/dbma/components/redis/uninstall.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.792689 dbm-agent-8.36.0/dbma/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.792689 dbm-agent-8.36.0/dbma/core/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/core/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-05-27 12:44:26.000000 dbm-agent-8.36.0/dbma/core/agent/init.py
--rw-r--r--   0 root         (0) root         (0)      115 2023-05-27 07:29:07.000000 dbm-agent-8.36.0/dbma/core/agent/upgrade.py
--rw-r--r--   0 root         (0) root         (0)     6064 2023-08-07 03:40:24.000000 dbm-agent-8.36.0/dbma/core/configs.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-27 07:28:18.000000 dbm-agent-8.36.0/dbma/core/exception.py
--rw-r--r--   0 root         (0) root         (0)     3785 2023-08-07 03:40:24.000000 dbm-agent-8.36.0/dbma/core/httpserver.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-05-27 07:28:34.000000 dbm-agent-8.36.0/dbma/core/messages.py
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-27 07:28:39.000000 dbm-agent-8.36.0/dbma/core/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.793689 dbm-agent-8.36.0/dbma/core/threads/
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/core/threads/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-05-27 07:28:57.000000 dbm-agent-8.36.0/dbma/core/threads/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.793689 dbm-agent-8.36.0/dbma/core/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/core/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/core/views/dbmagentview.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/core/views/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.775689 dbm-agent-8.36.0/dbma/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.798689 dbm-agent-8.36.0/dbma/static/cnfs/
--rw-r--r--   0 root         (0) root         (0)     1396 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/static/cnfs/auto-inseption-db.sql
--rw-r--r--   0 root         (0) root         (0)      514 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/static/cnfs/init-5.7.x.sql
--rw-r--r--   0 root         (0) root         (0)     1370 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/static/cnfs/init-8.0.x.sql
--rw-r--r--   0 root         (0) root         (0)     6681 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/static/cnfs/init-users.sql.jinja
--rw-r--r--   0 root         (0) root         (0)    10688 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/static/cnfs/mysql-5.7-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    10850 2024-03-28 11:54:36.000000 dbm-agent-8.36.0/dbma/static/cnfs/mysql-5.7.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    14664 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/static/cnfs/mysql-8.0-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    18775 2024-03-28 11:54:36.000000 dbm-agent-8.36.0/dbma/static/cnfs/mysql-8.0.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18774 2024-03-29 03:17:07.000000 dbm-agent-8.36.0/dbma/static/cnfs/mysql-8.3.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/static/cnfs/mysqld.service.jinja
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/static/cnfs/redis.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      710 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/static/cnfs/redisd.service.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 03:17:17.798689 dbm-agent-8.36.0/dbma/static/sql-scripts/
--rw-r--r--   0 root         (0) root         (0)     9468 2023-05-20 14:15:43.000000 dbm-agent-8.36.0/dbma/static/sql-scripts/常用SQL.md
--rw-r--r--   0 root         (0) root         (0)      344 2024-03-28 14:58:25.000000 dbm-agent-8.36.0/dbma/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-29 03:17:17.799689 dbm-agent-8.36.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1992 2023-06-21 06:55:16.000000 dbm-agent-8.36.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.446897 dbm-agent-8.40.0/
+-rw-r--r--   0 root         (0) root         (0)      626 2024-04-30 09:53:40.446897 dbm-agent-8.40.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8020 2024-03-29 12:44:37.000000 dbm-agent-8.40.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.435897 dbm-agent-8.40.0/bin/
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-30 12:35:14.000000 dbm-agent-8.40.0/bin/dbm-agent
+-rw-r--r--   0 root         (0) root         (0)      322 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/bin/dbm-bt-conn-stack
+-rw-r--r--   0 root         (0) root         (0)      887 2023-06-30 12:35:07.000000 dbm-agent-8.40.0/bin/dbma-cli-init
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-06-30 12:38:52.000000 dbm-agent-8.40.0/bin/dbma-cli-mysql
+-rw-r--r--   0 root         (0) root         (0)     2321 2023-06-30 12:34:44.000000 dbm-agent-8.40.0/bin/dbma-cli-redis
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.436897 dbm-agent-8.40.0/dbm_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      626 2024-04-30 09:53:40.000000 dbm-agent-8.40.0/dbm_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2351 2024-04-30 09:53:40.000000 dbm-agent-8.40.0/dbm_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 09:53:40.000000 dbm-agent-8.40.0/dbm_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-30 09:53:40.000000 dbm-agent-8.40.0/dbm_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-30 09:53:40.000000 dbm-agent-8.40.0/dbm_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.436897 dbm-agent-8.40.0/dbma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.438897 dbm-agent-8.40.0/dbma/bil/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/bil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/bil/cmdexecutor.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2023-05-27 07:30:34.000000 dbm-agent-8.40.0/dbma/bil/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-06-30 06:41:17.000000 dbm-agent-8.40.0/dbma/bil/fs.py
+-rw-r--r--   0 root         (0) root         (0)      223 2023-05-27 07:30:39.000000 dbm-agent-8.40.0/dbma/bil/fun.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/bil/net.py
+-rw-r--r--   0 root         (0) root         (0)     6795 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/bil/osuser.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/bil/sudos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.438897 dbm-agent-8.40.0/dbma/components/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.439897 dbm-agent-8.40.0/dbma/components/mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/components/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-05-29 11:59:15.000000 dbm-agent-8.40.0/dbma/components/mysql/asserts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.439897 dbm-agent-8.40.0/dbma/components/mysql/backends/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-18 14:11:07.000000 dbm-agent-8.40.0/dbma/components/mysql/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7758 2023-07-04 12:23:24.000000 dbm-agent-8.40.0/dbma/components/mysql/backends/clears.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.440897 dbm-agent-8.40.0/dbma/components/mysql/backups/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/components/mysql/backups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-27 07:26:51.000000 dbm-agent-8.40.0/dbma/components/mysql/backups/cloneplugin.py
+-rw-r--r--   0 root         (0) root         (0)     9680 2024-03-28 14:58:25.000000 dbm-agent-8.40.0/dbma/components/mysql/commons.py
+-rw-r--r--   0 root         (0) root         (0)    15760 2024-03-29 03:43:08.000000 dbm-agent-8.40.0/dbma/components/mysql/config.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-08-01 08:11:48.000000 dbm-agent-8.40.0/dbma/components/mysql/deploy.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-07-11 09:27:16.000000 dbm-agent-8.40.0/dbma/components/mysql/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14693 2023-07-18 06:49:24.000000 dbm-agent-8.40.0/dbma/components/mysql/install.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-05-27 07:26:20.000000 dbm-agent-8.40.0/dbma/components/mysql/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-05-27 07:26:23.000000 dbm-agent-8.40.0/dbma/components/mysql/replica.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-05-27 07:26:29.000000 dbm-agent-8.40.0/dbma/components/mysql/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.440897 dbm-agent-8.40.0/dbma/components/mysql/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/components/mysql/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13668 2023-07-04 14:24:35.000000 dbm-agent-8.40.0/dbma/components/mysql/views/defaultsview.py
+-rw-r--r--   0 root         (0) root         (0)     4373 2023-05-27 07:26:44.000000 dbm-agent-8.40.0/dbma/components/mysql/views/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.441897 dbm-agent-8.40.0/dbma/components/orchestrator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/components/orchestrator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-27 07:26:58.000000 dbm-agent-8.40.0/dbma/components/orchestrator/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-05-27 07:27:01.000000 dbm-agent-8.40.0/dbma/components/orchestrator/install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.442897 dbm-agent-8.40.0/dbma/components/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/components/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-05-27 07:27:34.000000 dbm-agent-8.40.0/dbma/components/redis/commons.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-05-27 07:27:09.000000 dbm-agent-8.40.0/dbma/components/redis/config.py
+-rw-r--r--   0 root         (0) root         (0)      548 2023-05-27 07:27:39.000000 dbm-agent-8.40.0/dbma/components/redis/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7269 2023-07-21 12:27:33.000000 dbm-agent-8.40.0/dbma/components/redis/install.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-05-27 07:27:52.000000 dbm-agent-8.40.0/dbma/components/redis/systemd.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-27 07:27:57.000000 dbm-agent-8.40.0/dbma/components/redis/uninstall.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.442897 dbm-agent-8.40.0/dbma/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.443897 dbm-agent-8.40.0/dbma/core/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/core/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-05-27 12:44:26.000000 dbm-agent-8.40.0/dbma/core/agent/init.py
+-rw-r--r--   0 root         (0) root         (0)      115 2023-05-27 07:29:07.000000 dbm-agent-8.40.0/dbma/core/agent/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)     6064 2023-08-07 03:40:24.000000 dbm-agent-8.40.0/dbma/core/configs.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-27 07:28:18.000000 dbm-agent-8.40.0/dbma/core/exception.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2023-08-07 03:40:24.000000 dbm-agent-8.40.0/dbma/core/httpserver.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-05-27 07:28:34.000000 dbm-agent-8.40.0/dbma/core/messages.py
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-27 07:28:39.000000 dbm-agent-8.40.0/dbma/core/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.443897 dbm-agent-8.40.0/dbma/core/threads/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/core/threads/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-05-27 07:28:57.000000 dbm-agent-8.40.0/dbma/core/threads/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.444897 dbm-agent-8.40.0/dbma/core/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/core/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/core/views/dbmagentview.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/core/views/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.434897 dbm-agent-8.40.0/dbma/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.446897 dbm-agent-8.40.0/dbma/static/cnfs/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/static/cnfs/auto-inseption-db.sql
+-rw-r--r--   0 root         (0) root         (0)      514 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/static/cnfs/init-5.7.x.sql
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/static/cnfs/init-8.0.x.sql
+-rw-r--r--   0 root         (0) root         (0)     6681 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/static/cnfs/init-users.sql.jinja
+-rw-r--r--   0 root         (0) root         (0)    10688 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/static/cnfs/mysql-5.7-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    10850 2024-03-28 11:54:36.000000 dbm-agent-8.40.0/dbma/static/cnfs/mysql-5.7.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    14665 2024-04-30 09:53:03.000000 dbm-agent-8.40.0/dbma/static/cnfs/mysql-8.0-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    18775 2024-03-29 03:43:08.000000 dbm-agent-8.40.0/dbma/static/cnfs/mysql-8.0.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18774 2024-03-29 03:43:08.000000 dbm-agent-8.40.0/dbma/static/cnfs/mysql-8.3.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18603 2024-04-30 09:49:35.000000 dbm-agent-8.40.0/dbma/static/cnfs/mysql-8.4.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/static/cnfs/mysqld.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/static/cnfs/redis.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/static/cnfs/redisd.service.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:53:40.446897 dbm-agent-8.40.0/dbma/static/sql-scripts/
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-05-20 14:15:43.000000 dbm-agent-8.40.0/dbma/static/sql-scripts/常用SQL.md
+-rw-r--r--   0 root         (0) root         (0)      344 2024-04-30 09:45:23.000000 dbm-agent-8.40.0/dbma/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 09:53:40.446897 dbm-agent-8.40.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-06-21 06:55:16.000000 dbm-agent-8.40.0/setup.py
```

### Comparing `dbm-agent-8.36.0/PKG-INFO` & `dbm-agent-8.40.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.36.0
+Version: 8.40.0
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.36.0/README.md` & `dbm-agent-8.40.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 - [安装-dbm-agent](#安装-dbm-agent)
 - [MySQL-功能列表](#MySQL-功能列表)
 - [Redis-功能列表](#Redis-功能列表)
 - [关闭-dbm-agent](#关闭-dbm-agent)
 - [规范](#规范)
 - [源码安装](#源码安装)
 - [官方微信公众平台](#官方微信公众平台)
+- [支持的MySQL版本](#支持的MySQL版本)
 
 
 ---
 
 ## dbm-愿景
   dbm 是一个软件套件，包含有 dbm-center 和 dbm-agent 两大组成部分；其中 dbm-center 可以看成一个 web 站点，DBA 通过它可以查看监控、告警、部署各种 MySQL|Redis 环境。
   dbm-agent 是 dbm-center 的助手，负责环境的部署、监控的采集与上报、数据库的备份与监控。总的来讲接活的 dbm-center 真正干活的是 dbm-agent。另外 dbm-agent 也集成了若干命令行工具，这使得它也可以单独使用。
@@ -194,8 +195,15 @@
 ```
 ---
 
 ## 官方微信公众平台 
 
 ![官方微信公众平台](imgs/mp-wechat.jpg)
 
+---
+
+## 支持的MySQL版本
+目前 MySQL 支持如下这些版本，子版本的话推荐使用最新版本；因为每一个新版本出来的时候都会用它来测试下，老版本就不会再测试了。
+ 1. 8.0.x
+ 2. 8.3.x
+
 ---
```

### Comparing `dbm-agent-8.36.0/bin/dbm-agent` & `dbm-agent-8.40.0/bin/dbm-agent`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/bin/dbma-cli-init` & `dbm-agent-8.40.0/bin/dbma-cli-init`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/bin/dbma-cli-mysql` & `dbm-agent-8.40.0/bin/dbma-cli-mysql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/bin/dbma-cli-redis` & `dbm-agent-8.40.0/bin/dbma-cli-redis`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbm_agent.egg-info/PKG-INFO` & `dbm-agent-8.40.0/dbm_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.36.0
+Version: 8.40.0
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.36.0/dbm_agent.egg-info/SOURCES.txt` & `dbm-agent-8.40.0/dbm_agent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -67,11 +67,12 @@
 dbma/static/cnfs/init-8.0.x.sql
 dbma/static/cnfs/init-users.sql.jinja
 dbma/static/cnfs/mysql-5.7-init-only.jinja
 dbma/static/cnfs/mysql-5.7.cnf.jinja
 dbma/static/cnfs/mysql-8.0-init-only.jinja
 dbma/static/cnfs/mysql-8.0.cnf.jinja
 dbma/static/cnfs/mysql-8.3.cnf.jinja
+dbma/static/cnfs/mysql-8.4.cnf.jinja
 dbma/static/cnfs/mysqld.service.jinja
 dbma/static/cnfs/redis.conf.jinja
 dbma/static/cnfs/redisd.service.jinja
 dbma/static/sql-scripts/常用SQL.md
```

### Comparing `dbm-agent-8.36.0/dbma/bil/daemon.py` & `dbm-agent-8.40.0/dbma/bil/daemon.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/bil/fs.py` & `dbm-agent-8.40.0/dbma/bil/fs.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/bil/net.py` & `dbm-agent-8.40.0/dbma/bil/net.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/bil/osuser.py` & `dbm-agent-8.40.0/dbma/bil/osuser.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/bil/sudos.py` & `dbm-agent-8.40.0/dbma/bil/sudos.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/asserts.py` & `dbm-agent-8.40.0/dbma/components/mysql/asserts.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/backends/clears.py` & `dbm-agent-8.40.0/dbma/components/mysql/backends/clears.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/backups/cloneplugin.py` & `dbm-agent-8.40.0/dbma/components/mysql/backups/cloneplugin.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/commons.py` & `dbm-agent-8.40.0/dbma/components/mysql/commons.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/config.py` & `dbm-agent-8.40.0/dbma/components/mysql/config.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/deploy.py` & `dbm-agent-8.40.0/dbma/components/mysql/deploy.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/exceptions.py` & `dbm-agent-8.40.0/dbma/components/mysql/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/install.py` & `dbm-agent-8.40.0/dbma/components/mysql/install.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/instance.py` & `dbm-agent-8.40.0/dbma/components/mysql/instance.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/replica.py` & `dbm-agent-8.40.0/dbma/components/mysql/replica.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/source.py` & `dbm-agent-8.40.0/dbma/components/mysql/source.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/views/defaultsview.py` & `dbm-agent-8.40.0/dbma/components/mysql/views/defaultsview.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/mysql/views/handlers.py` & `dbm-agent-8.40.0/dbma/components/mysql/views/handlers.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/orchestrator/install.py` & `dbm-agent-8.40.0/dbma/components/orchestrator/install.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/redis/commons.py` & `dbm-agent-8.40.0/dbma/components/redis/commons.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/redis/config.py` & `dbm-agent-8.40.0/dbma/components/redis/config.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/redis/exceptions.py` & `dbm-agent-8.40.0/dbma/components/redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/redis/install.py` & `dbm-agent-8.40.0/dbma/components/redis/install.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/components/redis/systemd.py` & `dbm-agent-8.40.0/dbma/components/redis/systemd.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/core/agent/init.py` & `dbm-agent-8.40.0/dbma/core/agent/init.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/core/configs.py` & `dbm-agent-8.40.0/dbma/core/configs.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/core/exception.py` & `dbm-agent-8.40.0/dbma/core/exception.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/core/httpserver.py` & `dbm-agent-8.40.0/dbma/core/httpserver.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/core/messages.py` & `dbm-agent-8.40.0/dbma/core/messages.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/core/threads/backends.py` & `dbm-agent-8.40.0/dbma/core/threads/backends.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/auto-inseption-db.sql` & `dbm-agent-8.40.0/dbma/static/cnfs/auto-inseption-db.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/init-5.7.x.sql` & `dbm-agent-8.40.0/dbma/static/cnfs/init-5.7.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/init-8.0.x.sql` & `dbm-agent-8.40.0/dbma/static/cnfs/init-8.0.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/init-users.sql.jinja` & `dbm-agent-8.40.0/dbma/static/cnfs/init-users.sql.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/mysql-5.7-init-only.jinja` & `dbm-agent-8.40.0/dbma/static/cnfs/mysql-5.7-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/mysql-5.7.cnf.jinja` & `dbm-agent-8.40.0/dbma/static/cnfs/mysql-5.7.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/mysql-8.0-init-only.jinja` & `dbm-agent-8.40.0/dbma/static/cnfs/mysql-8.0-init-only.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 binlog_row_image                           = {{binlog_row_image}}
 binlog_row_metadata                        = {{binlog_row_metadata}}
 binlog_rows_query_log_events               = {{binlog_rows_query_log_events}}
 binlog_stmt_cache_size                     = {{binlog_stmt_cache_size}}
 log_replica_updates                        = ON
 binlog_transaction_compression             = {{binlog_transaction_compression}}
 binlog_transaction_dependency_history_size = {{binlog_transaction_dependency_history_size}}
-binlog_transaction_dependency_tracking     = {{binlog_transaction_dependency_tracking}}
+#binlog_transaction_dependency_tracking     = {{binlog_transaction_dependency_tracking}}
 sync_binlog                                = {{sync_binlog}}
 binlog_cache_size                          = {{binlog_cache_size}}
 binlog_group_commit_sync_delay             = {{binlog_group_commit_sync_delay}}
 binlog_group_commit_sync_no_delay_count    = {{binlog_group_commit_sync_no_delay_count}}
 
 
 #### for gtid
```

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/mysql-8.0.cnf.jinja` & `dbm-agent-8.40.0/dbma/static/cnfs/mysql-8.0.cnf.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -293,12 +293,12 @@
 performance_schema_consumer_events_waits_current                        =ON  
 performance_schema_consumer_events_waits_history                        =ON  
 performance_schema_consumer_events_waits_history_long                   =OFF 
 performance-schema-instrument                                           ='memory/%=COUNTED'
 
 
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
-# base on mysql-8.0.34
+# base on mysql-8.0.36
 # generated by https://www.sqlpy.com at {{now}}
 # wechat: jianglegege
 # email: 1721900707@qq.com
 # -- ~ _ ~ --
```

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/mysql-8.3.cnf.jinja` & `dbm-agent-8.40.0/dbma/static/cnfs/mysql-8.3.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/redis.conf.jinja` & `dbm-agent-8.40.0/dbma/static/cnfs/redis.conf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/static/cnfs/redisd.service.jinja` & `dbm-agent-8.40.0/dbma/static/cnfs/redisd.service.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/dbma/static/sql-scripts/常用SQL.md` & `dbm-agent-8.40.0/dbma/static/sql-scripts/常用SQL.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.36.0/setup.py` & `dbm-agent-8.40.0/setup.py`

 * *Files identical despite different names*

