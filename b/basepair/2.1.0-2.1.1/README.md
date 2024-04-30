# Comparing `tmp/basepair-2.1.0.tar.gz` & `tmp/basepair-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basepair-2.1.0.tar", last modified: Thu Mar 21 05:00:24 2024, max compression
+gzip compressed data, was "basepair-2.1.1.tar", last modified: Tue Apr 30 10:23:07 2024, max compression
```

## Comparing `basepair-2.1.0.tar` & `basepair-2.1.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.185653 basepair-2.1.0/
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1076 2024-03-03 12:37:15.000000 basepair-2.1.0/LICENSE
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1116 2024-03-03 12:37:15.000000 basepair-2.1.0/LICENSE.txt
--rw-r--r--   0 anshunarayan   (501) staff       (20)     2603 2024-03-21 05:00:24.185349 basepair-2.1.0/PKG-INFO
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1534 2024-03-03 12:37:15.000000 basepair-2.1.0/README.md
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.097439 basepair-2.1.0/basepair/
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1179 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)    58352 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/api.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.106466 basepair-2.1.0/basepair/helpers/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       95 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/helpers/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      201 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/helpers/eprint.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     5140 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/helpers/nice_print.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      448 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/helpers/set_filter.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.107530 basepair-2.1.0/basepair/infra/
--rw-r--r--   0 anshunarayan   (501) staff       (20)        0 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/__init__.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.108981 basepair-2.1.0/basepair/infra/configuration/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       27 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/configuration/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     2297 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/infra/configuration/parser.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.123897 basepair-2.1.0/basepair/infra/webapp/
--rw-r--r--   0 anshunarayan   (501) staff       (20)      358 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     8652 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/abstract.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1739 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/analysis.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      218 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/file.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      218 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/gene.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      228 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/genome.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      250 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/genome_file.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      218 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/host.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      318 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/instance.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      929 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/module.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      238 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/pipeline.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      233 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/project.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1989 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/sample.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      806 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/upload.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1391 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/infra/webapp/user.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.124787 basepair-2.1.0/basepair/modules/
--rw-r--r--   0 anshunarayan   (501) staff       (20)        0 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/__init__.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.126636 basepair-2.1.0/basepair/modules/alert/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       44 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/alert/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      565 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/alert/alert.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.129310 basepair-2.1.0/basepair/modules/alert/drivers/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       60 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/alert/drivers/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      578 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/alert/drivers/abstract.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1635 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/alert/drivers/opsgenie.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.145317 basepair-2.1.0/basepair/modules/aws/
--rw-r--r--   0 anshunarayan   (501) staff       (20)      391 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     4154 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/cw.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)    11274 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/ec2.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.146952 basepair-2.1.0/basepair/modules/aws/handler/
--rw-r--r--   0 anshunarayan   (501) staff       (20)        0 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/handler/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1218 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/handler/exception.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     4411 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/hos.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     3416 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/how.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)    10610 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/iam.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     5241 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/instance.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1241 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/mrktpl.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     5577 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/policy.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)    14739 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/s3.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     4880 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/service.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1851 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/sm.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     5843 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/sqs.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     2559 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/sts.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     6982 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/aws/swf.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.148646 basepair-2.1.0/basepair/modules/identity/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       52 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/identity/__init__.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.151824 basepair-2.1.0/basepair/modules/identity/drivers/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       65 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/identity/drivers/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1525 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/identity/drivers/abstract.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1929 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/identity/drivers/aws_iam.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1598 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/identity/drivers/local.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1736 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/identity/main.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.153277 basepair-2.1.0/basepair/modules/logger/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       47 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/logger/__init__.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.156689 basepair-2.1.0/basepair/modules/logger/drivers/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       59 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/logger/drivers/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      797 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/logger/drivers/abstract.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1585 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/logger/drivers/logbook.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1588 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/logger/drivers/rollbar.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      547 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/logger/logger.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.158359 basepair-2.1.0/basepair/modules/secrets/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       50 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/secrets/__init__.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.161725 basepair-2.1.0/basepair/modules/secrets/drivers/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       73 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/secrets/drivers/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      448 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/secrets/drivers/abstract.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      482 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/secrets/drivers/aws_sm.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      602 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/secrets/drivers/local.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      653 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/secrets/main.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.163295 basepair-2.1.0/basepair/modules/storage/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       78 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/storage/__init__.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.167456 basepair-2.1.0/basepair/modules/storage/drivers/
--rw-r--r--   0 anshunarayan   (501) staff       (20)       64 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/storage/drivers/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     2229 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/storage/drivers/abstract.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      777 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/storage/drivers/aws_hos.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     4072 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/storage/drivers/aws_s3.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      797 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/storage/drivers/minio.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     2591 2024-03-21 04:59:41.000000 basepair-2.1.0/basepair/modules/storage/main.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.172325 basepair-2.1.0/basepair/utils/
--rw-r--r--   0 anshunarayan   (501) staff       (20)        0 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/utils/__init__.py
--rwxr-xr-x   0 anshunarayan   (501) staff       (20)      929 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/utils/colors.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1211 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/utils/monitor.py
--rwxr-xr-x   0 anshunarayan   (501) staff       (20)     1894 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/utils/s3.py
--rwxr-xr-x   0 anshunarayan   (501) staff       (20)     4100 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/utils/sqs.py
--rwxr-xr-x   0 anshunarayan   (501) staff       (20)     4043 2024-03-03 12:37:15.000000 basepair-2.1.0/basepair/utils/swf.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.184299 basepair-2.1.0/basepair.egg-info/
--rw-r--r--   0 anshunarayan   (501) staff       (20)     2603 2024-03-21 05:00:23.000000 basepair-2.1.0/basepair.egg-info/PKG-INFO
--rw-r--r--   0 anshunarayan   (501) staff       (20)     3164 2024-03-21 05:00:23.000000 basepair-2.1.0/basepair.egg-info/SOURCES.txt
--rw-r--r--   0 anshunarayan   (501) staff       (20)        1 2024-03-21 05:00:23.000000 basepair-2.1.0/basepair.egg-info/dependency_links.txt
--rw-r--r--   0 anshunarayan   (501) staff       (20)       46 2024-03-21 05:00:23.000000 basepair-2.1.0/basepair.egg-info/requires.txt
--rw-r--r--   0 anshunarayan   (501) staff       (20)       13 2024-03-21 05:00:23.000000 basepair-2.1.0/basepair.egg-info/top_level.txt
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.174488 basepair-2.1.0/bin/
--rw-r--r--   0 anshunarayan   (501) staff       (20)        0 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/__init__.py
--rwxr-xr-x   0 anshunarayan   (501) staff       (20)     5003 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/basepair
--rw-r--r--   0 anshunarayan   (501) staff       (20)     5902 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/common_parser.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.180339 basepair-2.1.0/bin/datatypes/
--rw-r--r--   0 anshunarayan   (501) staff       (20)      233 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/datatypes/__init__.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     8664 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/datatypes/analysis.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1014 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/datatypes/file.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     1269 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/datatypes/genome.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     3216 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/datatypes/module.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     3162 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/datatypes/pipeline.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     2362 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/datatypes/project.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)     6741 2024-03-03 12:37:15.000000 basepair-2.1.0/bin/datatypes/sample.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)       79 2024-03-21 05:00:24.186825 basepair-2.1.0/setup.cfg
--rw-r--r--   0 anshunarayan   (501) staff       (20)     2283 2024-03-21 04:59:41.000000 basepair-2.1.0/setup.py
-drwxr-xr-x   0 anshunarayan   (501) staff       (20)        0 2024-03-21 05:00:24.183231 basepair-2.1.0/tests/
--rw-r--r--   0 anshunarayan   (501) staff       (20)    11164 2024-03-03 12:37:15.000000 basepair-2.1.0/tests/test_genes.py
--rw-r--r--   0 anshunarayan   (501) staff       (20)      402 2024-03-03 12:37:15.000000 basepair-2.1.0/tests/test_samples.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.831086 basepair-2.1.1/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1076 2024-03-20 11:43:33.000000 basepair-2.1.1/LICENSE
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1116 2024-03-20 11:43:33.000000 basepair-2.1.1/LICENSE.txt
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     2603 2024-04-30 10:23:07.831033 basepair-2.1.1/PKG-INFO
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1534 2024-03-20 11:43:33.000000 basepair-2.1.1/README.md
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.819597 basepair-2.1.1/basepair/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1179 2024-04-30 10:19:25.000000 basepair-2.1.1/basepair/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)    58352 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/api.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.820630 basepair-2.1.1/basepair/helpers/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       95 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/helpers/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      201 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/helpers/eprint.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     5140 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/helpers/nice_print.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      448 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/helpers/set_filter.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.820731 basepair-2.1.1/basepair/infra/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)        0 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/__init__.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.820954 basepair-2.1.1/basepair/infra/configuration/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       27 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/configuration/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     2297 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/infra/configuration/parser.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.822538 basepair-2.1.1/basepair/infra/webapp/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      358 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     8652 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/abstract.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1739 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/analysis.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      218 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/file.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      218 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/gene.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      228 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/genome.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      250 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/genome_file.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      218 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/host.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      318 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/instance.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      929 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/module.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      238 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/pipeline.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      233 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/project.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1989 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/sample.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      806 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/upload.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1391 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/infra/webapp/user.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.822636 basepair-2.1.1/basepair/modules/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)        0 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/__init__.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.822821 basepair-2.1.1/basepair/modules/alert/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       44 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/alert/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      565 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/alert/alert.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.823157 basepair-2.1.1/basepair/modules/alert/drivers/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       60 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/alert/drivers/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      578 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/alert/drivers/abstract.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1635 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/alert/drivers/opsgenie.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.825183 basepair-2.1.1/basepair/modules/aws/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      391 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     4154 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/cw.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)    11274 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/ec2.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.825434 basepair-2.1.1/basepair/modules/aws/handler/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)        0 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/handler/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1218 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/handler/exception.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     7495 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/aws/hos.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     3979 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/aws/how.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)    10610 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/iam.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     5241 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/instance.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1241 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/mrktpl.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     6303 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/aws/policy.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)    14818 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/aws/s3.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     4880 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/service.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1851 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/sm.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     5843 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/sqs.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     2559 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/sts.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     6982 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/aws/swf.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.825653 basepair-2.1.1/basepair/modules/identity/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       52 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/identity/__init__.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.826078 basepair-2.1.1/basepair/modules/identity/drivers/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       65 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/identity/drivers/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1525 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/identity/drivers/abstract.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1929 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/identity/drivers/aws_iam.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1598 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/identity/drivers/local.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1736 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/identity/main.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.826285 basepair-2.1.1/basepair/modules/logger/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       47 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/logger/__init__.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.826691 basepair-2.1.1/basepair/modules/logger/drivers/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       59 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/logger/drivers/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      797 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/logger/drivers/abstract.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1585 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/logger/drivers/logbook.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1588 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/logger/drivers/rollbar.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      547 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/logger/logger.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.826913 basepair-2.1.1/basepair/modules/secrets/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       50 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/secrets/__init__.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.827315 basepair-2.1.1/basepair/modules/secrets/drivers/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       73 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/secrets/drivers/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      448 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/secrets/drivers/abstract.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      482 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/secrets/drivers/aws_sm.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      602 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/secrets/drivers/local.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      653 2024-03-20 13:35:18.000000 basepair-2.1.1/basepair/modules/secrets/main.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.827518 basepair-2.1.1/basepair/modules/storage/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       78 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/storage/__init__.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.828025 basepair-2.1.1/basepair/modules/storage/drivers/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       64 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/storage/drivers/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     2253 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/storage/drivers/abstract.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     3763 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/storage/drivers/aws_hos.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     3845 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/storage/drivers/aws_s3.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      996 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/storage/drivers/minio.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     2466 2024-04-30 10:16:00.000000 basepair-2.1.1/basepair/modules/storage/main.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.828786 basepair-2.1.1/basepair/utils/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)        0 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/utils/__init__.py
+-rwxr-xr-x   0 amiaynarayan   (501) staff       (20)      929 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/utils/colors.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1211 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/utils/monitor.py
+-rwxr-xr-x   0 amiaynarayan   (501) staff       (20)     1894 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/utils/s3.py
+-rwxr-xr-x   0 amiaynarayan   (501) staff       (20)     4100 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/utils/sqs.py
+-rwxr-xr-x   0 amiaynarayan   (501) staff       (20)     4043 2024-03-20 11:43:33.000000 basepair-2.1.1/basepair/utils/swf.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.830843 basepair-2.1.1/basepair.egg-info/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     2603 2024-04-30 10:23:07.000000 basepair-2.1.1/basepair.egg-info/PKG-INFO
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     3164 2024-04-30 10:23:07.000000 basepair-2.1.1/basepair.egg-info/SOURCES.txt
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)        1 2024-04-30 10:23:07.000000 basepair-2.1.1/basepair.egg-info/dependency_links.txt
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       46 2024-04-30 10:23:07.000000 basepair-2.1.1/basepair.egg-info/requires.txt
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       13 2024-04-30 10:23:07.000000 basepair-2.1.1/basepair.egg-info/top_level.txt
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.829185 basepair-2.1.1/bin/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)        0 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/__init__.py
+-rwxr-xr-x   0 amiaynarayan   (501) staff       (20)     5003 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/basepair
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     5902 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/common_parser.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.830184 basepair-2.1.1/bin/datatypes/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      233 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/datatypes/__init__.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     8664 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/datatypes/analysis.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1014 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/datatypes/file.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     1269 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/datatypes/genome.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     3216 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/datatypes/module.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     3162 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/datatypes/pipeline.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     2362 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/datatypes/project.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     6741 2024-03-20 11:43:33.000000 basepair-2.1.1/bin/datatypes/sample.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)       79 2024-04-30 10:23:07.831259 basepair-2.1.1/setup.cfg
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)     2283 2024-03-20 13:35:18.000000 basepair-2.1.1/setup.py
+drwxr-xr-x   0 amiaynarayan   (501) staff       (20)        0 2024-04-30 10:23:07.830681 basepair-2.1.1/tests/
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)    11164 2024-03-20 11:43:33.000000 basepair-2.1.1/tests/test_genes.py
+-rw-r--r--   0 amiaynarayan   (501) staff       (20)      402 2024-03-20 11:43:33.000000 basepair-2.1.1/tests/test_samples.py
```

### Comparing `basepair-2.1.0/LICENSE` & `basepair-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/LICENSE.txt` & `basepair-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/PKG-INFO` & `basepair-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: basepair
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python client for Basepair's API
 Home-page: https://bitbucket.org/basepair/basepair
-Download-URL: https://bitbucket.org/basepair/basepair/get/2.1.0.tar.gz
+Download-URL: https://bitbucket.org/basepair/basepair/get/2.1.1.tar.gz
 Author: Basepair
 Author-email: info@basepairtech.com
 Keywords: bioinformatics,ngs analysis,dna-seq,rna-seq,chip-seq,atac-seq
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
```

### Comparing `basepair-2.1.0/README.md` & `basepair-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/__init__.py` & `basepair-2.1.1/basepair/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Exposing infra webapp library
 from .infra.webapp import Analysis, File, Gene, Genome, GenomeFile, Host, Module, Pipeline, Project, Sample, Upload, User
 
 # Exposing the storage wrapper
 
 __title__ = 'basepair'
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 __copyright__ = 'Copyright [2017] - [2022] Basepair INC'
 
 
 JSON_URL = 'https://pypi.python.org/pypi/{}/json'.format(__title__)
 try:
     resp = requests.get(JSON_URL, timeout=1)
     if resp.status_code == 200:
```

### Comparing `basepair-2.1.0/basepair/api.py` & `basepair-2.1.1/basepair/api.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/helpers/nice_print.py` & `basepair-2.1.1/basepair/helpers/nice_print.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/infra/configuration/parser.py` & `basepair-2.1.1/basepair/infra/configuration/parser.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/infra/webapp/abstract.py` & `basepair-2.1.1/basepair/infra/webapp/abstract.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/infra/webapp/analysis.py` & `basepair-2.1.1/basepair/infra/webapp/analysis.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/infra/webapp/module.py` & `basepair-2.1.1/basepair/infra/webapp/module.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/infra/webapp/sample.py` & `basepair-2.1.1/basepair/infra/webapp/sample.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/infra/webapp/upload.py` & `basepair-2.1.1/basepair/infra/webapp/upload.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/infra/webapp/user.py` & `basepair-2.1.1/basepair/infra/webapp/user.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/alert/alert.py` & `basepair-2.1.1/basepair/modules/alert/alert.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/alert/drivers/abstract.py` & `basepair-2.1.1/basepair/modules/alert/drivers/abstract.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/alert/drivers/opsgenie.py` & `basepair-2.1.1/basepair/modules/alert/drivers/opsgenie.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/cw.py` & `basepair-2.1.1/basepair/modules/aws/cw.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/ec2.py` & `basepair-2.1.1/basepair/modules/aws/ec2.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/handler/exception.py` & `basepair-2.1.1/basepair/modules/aws/handler/exception.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/hos.py` & `basepair-2.1.1/basepair/modules/aws/how.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,152 +1,141 @@
-'''AWS HealthOmics Storage Wrappers'''
-
-# General imports
-import uuid
+'''AWS HealthOmics Workflow Wrapper'''
 
 # Libs imports
 from botocore.client import Config
 from botocore.exceptions import ClientError
 
 # Module imports
 from basepair.modules.aws.service import Service
 
-class HOS(Service):
-  '''Wrapper for Health Omics Storage services'''
+class HOW(Service):
+  '''Wrapper for Health Omics Workflow services'''
 
   def __init__(self, cfg):
-    super().__init__(cfg, 'HOS')
+    super().__init__(cfg, 'HOW')
     self.client = self.session.client(**{
       'config': Config(retries={'max_attempts': 0, 'mode': 'standard'}),
       'service_name': 'omics',
     })
-    self.sequence_store_id = cfg.get('sequence_store_id')
-    self.reference_store_id = cfg.get('reference_store_id')
-    self.role_arn = cfg.get('role_arn')
-
-  def get_export_job(self, job_id):
-    '''Get export job'''
-    try:
-      response = self.client.get_read_set_export_job(
-        id=job_id,
-        sequenceStoreId=self.sequence_store_id,
-      )
+
+  def create_workflow(self, params):
+    '''Create workflow'''
+    try:
+      response = self.client.create_workflow(**params)
     except ClientError as error:
       self.get_log_msg({
         'exception': error,
-        'msg': f'Not able to get HealthOmics export job information: {str(error)}.',
+        'msg': f'Not able to create HealthOmics workflow: {str(error)}.',
       })
       raise error
     return response
 
-  def get_read_set_import_job(self, job_id):
-    '''Get import job'''
+  def cancel_run(self, run_id):
+    '''Cancel run'''
     try:
-      response = self.client.get_read_set_import_job(
-        id=job_id,
-        sequenceStoreId=self.sequence_store_id,
-      )
+      response = self.client.cancel_run(id=run_id)
     except ClientError as error:
       self.get_log_msg({
         'exception': error,
-        'msg': f'Not able to get HealthOmics import job information: {str(error)}.',
+        'msg': f'Not able to cancel HealthOmics run: {str(error)}.',
       })
       raise error
     return response
 
-  def get_reference_import_job(self, job_id):
-    '''Get reference import job'''
+  def delete_run(self, run_id):
+    '''Delete run'''
     try:
-      response = self.client.get_reference_import_job(
-        id=job_id,
-        referenceStoreId=self.reference_store_id,
-      )
+      response = self.client.delete_run(id=run_id)
     except ClientError as error:
       self.get_log_msg({
         'exception': error,
-        'msg': f'Not able to get HealthOmics reference import job information: {str(error)}.',
+        'msg': f'Not able to delete HealthOmics run: {str(error)}.',
       })
       raise error
     return response
 
-  def list_read_sets(self, filters):
-    '''Get read sets list'''
+  def delete_workflow(self, params):
+    '''Delete workflow'''
     try:
-      response = self.client.list_read_sets(
-        sequenceStoreId=self.sequence_store_id,
-        filter=filters
-      )
+      response = self.client.delete_workflow(**params)
     except ClientError as error:
       self.get_log_msg({
         'exception': error,
-        'msg': f'Not able to list HealthOmics read sets: {str(error)}.',
+        'msg': f'Not able to delete HealthOmics workflow: {str(error)}.',
       })
       raise error
     return response
 
-  def delete_read_sets(self, read_set_ids):
-    '''Delete read sets'''
+  def get_run(self, params):
+    '''Get omics run'''
     try:
-      response = self.client.batch_delete_read_set(
-        sequenceStoreId=self.sequence_store_id,
-        ids=read_set_ids
-      )
+      return self.client.get_run(**params)
     except ClientError as error:
       self.get_log_msg({
-        'exception': error,
-        'msg': f'Not able to delete HealthOmics read sets: {str(error)}.',
+        'exception': str(error),
+        'msg': f'Not able to Get HealthOmics run id {params.get("id")}: {str(error)}.',
+      })
+      raise error
+  
+  def get_run_task(self, params):
+    '''Get omics run task'''
+    try:
+      return self.client.get_run_task(**params)
+    except ClientError as error:
+      self.get_log_msg({
+        'exception': str(error),
+        'msg': f'Not able to Get HealthOmics run task id {params.get("id")}: {str(error)}.',
       })
       raise error
-    return response
 
-  def start_export_job(self, destination, sources):
-    '''Start export job'''
+  def get_workflow(self, params):
+    '''Get omics workflow'''
     try:
-      client_token = str(uuid.uuid4())
-      response = self.client.start_read_set_export_job(
-        sequenceStoreId=self.sequence_store_id,
-        destination=destination,
-        roleArn=self.role_arn,
-        clientToken=client_token,
-        sources=sources
-      )
+      return self.client.get_workflow(**params)
     except ClientError as error:
       self.get_log_msg({
-        'exception': error,
-        'msg': f'Not able to start HealthOmics export job: {str(error)}.',
+        'exception': str(error),
+        'msg': f'Not able to get HealthOmics workflow: {str(error)}.',
+      })
+      raise error
+
+  def list_run_tasks(self, params):
+    '''Get omics run list'''
+    try:
+      tasks = []
+      while True:
+        response = self.client.list_run_tasks(**params)
+        next_token = response.get("nextToken")
+        tasks += response.get('items')
+        if next_token:
+          params["startingToken"] = next_token
+        else:
+          break
+      return tasks
+    except ClientError as error:
+      self.get_log_msg({
+        'exception':error,
+        'msg': f'Not able to Get HealthOmics run task list id {params.get("id")}: {str(error)}'
       })
       raise error
-    return response
 
-  def start_import_job(self, sources):
-    '''Start import job'''
+  def list_workflows(self, params):
+    '''List omics workflows'''
     try:
-      client_token = str(uuid.uuid4())
-      return self.client.start_read_set_import_job(
-        sequenceStoreId=self.sequence_store_id,
-        roleArn=self.role_arn,
-        clientToken=client_token,
-        sources=sources
-      )
+      return self.client.list_workflows(**params)
     except ClientError as error:
       self.get_log_msg({
         'exception': str(error),
-        'msg': f'Not able to start HealthOmics import job: {str(error)}.',
+        'msg': f'Not able to list HealthOmics workflows: {str(error)}.',
       })
       raise error
 
-  def start_reference_import_job(self, sources):
-    '''Start reference import job'''
+  def start_run(self, params):
+    '''Start omics workflow'''
     try:
-      client_token = str(uuid.uuid4())
-      return self.client.start_reference_import_job(
-        referenceStoreId=self.reference_store_id,
-        roleArn=self.role_arn,
-        clientToken=client_token,
-        sources=sources
-      )
+      return self.client.start_run(**params)
     except ClientError as error:
       self.get_log_msg({
         'exception': str(error),
-        'msg': f'Not able to start HealthOmics reference import job: {str(error)}.',
+        'msg': f'Not able to start HealthOmics workflow id {params.get("workflowId")}: {str(error)}.',
       })
       raise error
```

### Comparing `basepair-2.1.0/basepair/modules/aws/iam.py` & `basepair-2.1.1/basepair/modules/aws/iam.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/instance.py` & `basepair-2.1.1/basepair/modules/aws/instance.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/mrktpl.py` & `basepair-2.1.1/basepair/modules/aws/mrktpl.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/policy.py` & `basepair-2.1.1/basepair/modules/aws/policy.py`

 * *Files 25% similar despite different names*

```diff
@@ -81,44 +81,58 @@
         'Effect': 'Allow',
         'Resource': resource,
       }],
       'Version': '2012-10-17'
     }
 
   @staticmethod
-  def ho_run(ho_import_export_role_arn):
-    '''HO workflow policy template for starting and getting run'''
+  def hos_general_purpose(ho_region, reference_store_id, sequence_store_id):
+    '''HOS policy template for general purpose'''
     return {
-      "Version": "2012-10-17",
-      "Statement": [
+      'Statement': [
         {
-          "Sid": "VisualEditor0",
-          "Effect": "Allow",
-          "Action": [
-            "omics:GetRunTask",
-            "omics:GetWorkflow",
-            "omics:GetRun"
+          'Action': [
+            "omics:BatchDeleteReadSet",
+            "omics:DeleteReference",
+            "omics:GetReadSet",
+            "omics:GetReadSetExportJob",
+            "omics:GetReadSetImportJob",
+            "omics:GetReadSetMetadata",
+            "omics:GetReferenceImportJob",
+            "omics:GetReferenceMetadata",
+            "omics:ListReadSets",
+            "omics:ListReferences",
+            "omics:StartReadSetActivationJob",
+            "omics:StartReadSetExportJob",
+            "omics:StartReadSetImportJob",
+            "omics:StartReferenceImportJob",
           ],
-          "Resource": [
-            "arn:aws:omics:us-east-1:*:run/*",
-            "arn:aws:omics:us-east-1:*:task/*",
-            "arn:aws:omics:us-east-1:*:workflow/*"
+          'Effect': 'Allow',
+          'Resource': [
+            f"arn:aws:omics:{ho_region}:*:referenceStore/{reference_store_id}/*",
+            f"arn:aws:omics:{ho_region}:*:referenceStore/{reference_store_id}",
+            f"arn:aws:omics:{ho_region}:*:sequenceStore/{sequence_store_id}/*",
+            f"arn:aws:omics:{ho_region}:*:sequenceStore/{sequence_store_id}",
           ]
-        },
-        {
-          "Sid": "VisualEditor1",
-          "Effect": "Allow",
-          "Action": "omics:StartRun",
-          "Resource": "*"
-        },
-        {
-          "Sid": "VisualEditor2",
-          "Effect": "Allow",
-          "Action": "iam:PassRole",
-          "Resource": ho_import_export_role_arn
+        }, {
+          'Action': [
+            "s3:GetObject",
+            "s3:ListBucket"
+          ],
+          'Effect': 'Allow',
+          'Resource': ['*'],
+          'Condition': {
+            'StringLike': {
+              "s3:DataAccessPointArn": f"arn:aws:s3:{ho_region}:*"
+            }
+          }
+        }, {
+          'Action': ["kms:Decrypt"],
+          'Effect': 'Allow',
+          'Resource': [f"arn:aws:kms:{ho_region}:*:*"]
         }
       ]
     }
 
   @staticmethod
   def s3_general_purpose(bucket, reflib_buckets, user_id):
     '''S3 policy template for general purpose'''
```

### Comparing `basepair-2.1.0/basepair/modules/aws/s3.py` & `basepair-2.1.1/basepair/modules/aws/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,20 +182,21 @@
         'std_print': show_log,
       })
       if ExceptionHandler.is_throttled_error(exception=error):
         raise error
       response = int(error.response['Error']['Code']) != 404
     return response
 
-  def get_self_signed(self, key, expires_in=28800):
+  def get_self_signed(self, key, bucket=None, expires_in=28800):
     '''Generate self signed url for key'''
     try:
+      bucket = bucket or self.bucket
       return self.client.generate_presigned_url(
         'get_object',
-        Params={'Bucket': self.bucket, 'Key': key},
+        Params={'Bucket': bucket, 'Key': key},
         ExpiresIn=expires_in, # a week
       )
     except (ClientError, NoCredentialsError, Exception) as error: # pylint: disable=broad-except
       self.get_log_msg({
         'exception': error,
         'msg': f'Not able to self sign object key {key}.',
       })
@@ -204,14 +205,15 @@
     return None
 
   def get_storage_context(self):
     '''Method to return context for S3'''
     return {
       'storage_archival_enabled' : bool(self.cfg.get('restore_period', False)),
       'storage_bucket' : self.cfg.get('bucket'),
+      'storage_driver': 'aws_s3',
       'storage_region' : self.cfg.get('region'),
       'storage_sse_enabled' : 'True',
       'storage_url': f"https://s3.{self.cfg.get('region')}.amazonaws.com",
     }
 
   def get_status(self, key, bucket=None):
     '''Method to check the status of file restore process'''
```

### Comparing `basepair-2.1.0/basepair/modules/aws/service.py` & `basepair-2.1.1/basepair/modules/aws/service.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/sm.py` & `basepair-2.1.1/basepair/modules/aws/sm.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/sqs.py` & `basepair-2.1.1/basepair/modules/aws/sqs.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/sts.py` & `basepair-2.1.1/basepair/modules/aws/sts.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/aws/swf.py` & `basepair-2.1.1/basepair/modules/aws/swf.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/identity/drivers/abstract.py` & `basepair-2.1.1/basepair/modules/identity/drivers/abstract.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/identity/drivers/aws_iam.py` & `basepair-2.1.1/basepair/modules/identity/drivers/aws_iam.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/identity/drivers/local.py` & `basepair-2.1.1/basepair/modules/identity/drivers/local.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/identity/main.py` & `basepair-2.1.1/basepair/modules/identity/main.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/logger/drivers/abstract.py` & `basepair-2.1.1/basepair/modules/logger/drivers/abstract.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/logger/drivers/logbook.py` & `basepair-2.1.1/basepair/modules/logger/drivers/logbook.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/logger/drivers/rollbar.py` & `basepair-2.1.1/basepair/modules/logger/drivers/rollbar.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/logger/logger.py` & `basepair-2.1.1/basepair/modules/logger/logger.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/secrets/drivers/local.py` & `basepair-2.1.1/basepair/modules/secrets/drivers/local.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/secrets/main.py` & `basepair-2.1.1/basepair/modules/secrets/main.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/modules/storage/drivers/aws_s3.py` & `basepair-2.1.1/basepair/modules/storage/drivers/aws_s3.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,128 +1,116 @@
-'''Driver for AWS S3 compute'''
+"""Driver for AWS S3 compute"""
 
 # Libs import
 from basepair.modules.aws import S3
 
 # App import
 from .abstract import StorageAbstract
 
 FILE_NOT_FOUND = 'file_not_found'
 RESTORE_COMPLETE = 'restore_complete'
 RESTORE_ERROR = 'restore_error'
 RESTORE_IN_PROGRESS = 'restore_in_progress'
 RESTORE_NOT_REQUIRED = 'restore_not_required'
 RESTORE_NOT_STARTED = 'restore_not_started'
 
+
 class Driver(StorageAbstract):
-  '''AWS S3 Driver class'''
+    """AWS S3 Driver class"""
 
-  def __init__(self, cfg=None): # pylint: disable=super-init-not-called
-    '''Instance constructor'''
-    self.storage_settings = cfg.get('settings', {})
-    self.s3_service = S3({
-      'bucket': self.storage_settings.get('bucket'),
-      'credentials': cfg.get('credentials'),
-      'region': self.storage_settings.get('region'),
-      'endpoint_url': self.storage_settings.get('endpoint_url'),
-      'disable_sts': self.storage_settings.get('disable_sts', False),
-    })
-
-  def bulk_delete(self, uris):
-    '''Delete list of files by their uris'''
-    return self.s3_service.bulk_delete(uris)
-
-  def delete(self, uri):
-    '''Delete file from storage'''
-    key = S3.get_key_from_uri(uri)
-    return self.s3_service.delete(key)
-
-  def download(self, uri, callback=None, file=None):
-    '''Download file froms torage'''
-    bucket = S3.get_bucket_from_uri(uri)
-    key = S3.get_key_from_uri(uri)
-    if callback:
-      return self.s3_service.client.download_fileobj(
-        bucket,
-        key,
-        file,
-        Callback=callback,
-      )
-    return self.s3_service.download(key, file)
-
-  def get_body(self, uri):
-    '''Get file body'''
-    key = S3.get_key_from_uri(uri)
-    return self.s3_service.get_file_body(key)
-
-  def get_head(self, uri):
-    '''Get file head'''
-    key = S3.get_key_from_uri(uri)
-    return self.s3_service.get_object_head(key)
-
-  def get_lifecycle(self, bucket=None):
-    '''Get storage lifecycle'''
-    return self.s3_service.get_lifecycle(bucket)
-
-  def get_overall_status(self, uris):
-    '''Get overall sample files status'''
-    restore_statuses = [self.get_status(uri) for uri in uris]
-
-    # Check if all statuses are RESTORE_COMPLETE
-    if all(status == RESTORE_COMPLETE for status in restore_statuses):
-      return RESTORE_COMPLETE
-    # Find the first status
-    for state in [FILE_NOT_FOUND, RESTORE_IN_PROGRESS, RESTORE_ERROR, RESTORE_NOT_STARTED]:
-      if any(status == state for status in restore_statuses):
-        return state
-    # If no status found, return RESTORE_NOT_REQUIRED
-    return RESTORE_NOT_REQUIRED
-
-  def get_public_url(self, uri):
-    '''Get a public accessible url'''
-    key = S3.get_key_from_uri(uri)
-    return self.s3_service.get_self_signed(key)
-
-  def get_service(self):
-    return self.s3_service
-
-  def get_storage_context(self):
-    '''Get the storage context'''
-    return self.s3_service.get_storage_context()
-
-  def get_status(self, uri):
-    '''Get the file status'''
-    bucket = S3.get_bucket_from_uri(uri)
-    key = S3.get_key_from_uri(uri)
-    return self.s3_service.get_status(bucket=bucket, key=key)
-
-  def get_uri(self, key):
-    '''Get uri using key and storage settings'''
-    return f's3://{self.s3_service.bucket}/{key}'
-
-  def list(self, prefix, bucket=None):
-    return self.s3_service.list(prefix, bucket)
-
-  def restore_files_from_cold(self, uris, days):
-    '''Restore files from cold storage'''
-    for uri in uris:
-      status = self.get_status(uri)
-      if status == 'restore_not_started':
-        self.restore_from_cold(uri, days=days)
-
-  def restore_from_cold(self, uri, days):
-    '''Restore file from cold storage'''
-    key = S3.get_key_from_uri(uri)
-    return self.s3_service.start_restore(key, days)
-
-  def set_body(self, body, uri):
-    '''Set file body'''
-    key = S3.get_key_from_uri(uri)
-    return self.s3_service.set_file_body(body, key)
-
-  def set_lifecycle(self, **kwargs):
-    '''Set storage lifecycle'''
-    return self.s3_service.set_lifecycle(**kwargs)
-
-  def upload(self, file_name, full_path, **kwargs):
-    '''Upload file to storage'''
-    return self.s3_service.upload_file(file_name, full_path, **kwargs)
+    def __init__(self, cfg=None):
+        """Instance constructor"""
+        self.storage_settings = cfg.get('settings', {})
+        self.s3_service = S3({
+            'bucket': self.storage_settings.get('bucket'),
+            'credentials': cfg.get('credentials'),
+            'region': self.storage_settings.get('region'),
+            'restore_period': self.storage_settings.get('restore_period'),
+            'endpoint_url': self.storage_settings.get('endpoint_url'),
+            'disable_sts': self.storage_settings.get('disable_sts', False),
+        })
+
+    def bulk_delete(self, uris):
+        """Delete list of files by their uris"""
+        return self.s3_service.bulk_delete(uris)
+
+    def delete(self, uri):
+        """Delete file from storage"""
+        key = S3.get_key_from_uri(uri)
+        return self.s3_service.delete(key)
+
+    def download(self, uri, callback=None, file=None):
+        """Download file from storage"""
+        bucket = S3.get_bucket_from_uri(uri)
+        key = S3.get_key_from_uri(uri)
+        if callback:
+            return self.s3_service.client.download_fileobj(
+                bucket,
+                key,
+                file,
+                Callback=callback,
+            )
+        return self.s3_service.download(key, file)
+
+    def get_body(self, uri):
+        """Get file body"""
+        key = S3.get_key_from_uri(uri)
+        return self.s3_service.get_file_body(key)
+
+    def get_head(self, uri):
+        """Get file head"""
+        key = S3.get_key_from_uri(uri)
+        return self.s3_service.get_object_head(key)
+
+    def get_lifecycle(self, bucket=None):
+        """Get storage lifecycle"""
+        return self.s3_service.get_lifecycle(bucket)
+
+    def get_public_url(self, uri):
+        """Get a public accessible url"""
+        key = S3.get_key_from_uri(uri)
+        return self.s3_service.get_self_signed(key)
+
+    def get_service(self):
+        return self.s3_service
+
+    def get_storage_context(self):
+        """Get the storage context"""
+        return self.s3_service.get_storage_context()
+
+    def get_status(self, uri):
+        """Get the file status"""
+        bucket = S3.get_bucket_from_uri(uri)
+        key = S3.get_key_from_uri(uri)
+        return self.s3_service.get_status(bucket=bucket, key=key)
+
+    def get_uri(self, key):
+        """Get uri using key and storage settings"""
+        return f's3://{self.s3_service.bucket}/{key}'
+
+    def list(self, prefix, bucket=None):
+        return self.s3_service.list(prefix, bucket)
+
+    def restore_files_from_cold(self, uris, days):
+        """Restore files from cold storage"""
+        for uri in uris:
+            status = self.get_status(uri)
+            if status == 'restore_not_started':
+                self.restore_from_cold(uri, days=days)
+
+    def restore_from_cold(self, uri, days):
+        """Restore file from cold storage"""
+        key = S3.get_key_from_uri(uri)
+        return self.s3_service.start_restore(key, days)
+
+    def set_body(self, body, uri):
+        """Set file body"""
+        key = S3.get_key_from_uri(uri)
+        return self.s3_service.set_file_body(body, key)
+
+    def set_lifecycle(self, **kwargs):
+        """Set storage lifecycle"""
+        return self.s3_service.set_lifecycle(**kwargs)
+
+    def upload(self, file_name, full_path, **kwargs):
+        """Upload file to storage"""
+        return self.s3_service.upload_file(file_name, full_path, **kwargs)
```

### Comparing `basepair-2.1.0/basepair/modules/storage/drivers/minio.py` & `basepair-2.1.1/basepair/modules/storage/drivers/minio.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-'''Driver for AWS S3 compute'''
+"""Driver for AWS S3 compute"""
 
 # App import
 from .aws_s3 import Driver as S3Driver
 from .abstract import raise_no_implemented
 
-# constants
 
 class Driver(S3Driver):
-  '''Min IO Driver class'''
-
-  def __init__(self, cfg=None):
-    super().__init__(cfg)
-
-  def get_lifecycle(self, bucket=None):
-    raise_no_implemented("MinIO does not support lifecycle")
-
-  def get_storage_context(self):
-    '''Get the context for Minio'''
-    return {
-      **super().get_storage_context(),
-      'storage_url' : self.storage_settings.get('endpoint_url'),
-      'storage_sse_enabled' : 'False'
-    }
-
-  def restore_from_cold(self, uri, days):
-    raise_no_implemented("MinIO does not support restore from cold")
-
-  def set_lifecycle(self, **kwargs):
-    raise_no_implemented("MinIO does not support lifecycle")
+    """Min IO Driver class"""
+    def __init__(self, cfg=None):
+        super().__init__(cfg)
+
+    def get_lifecycle(self, bucket=None):
+        """Get storage lifecycle"""
+        raise_no_implemented("MinIO does not support lifecycle")
+
+    def get_storage_context(self):
+        """Get the context for Minio"""
+        return {
+            **super().get_storage_context(),
+            'storage_driver': 'minio',
+            'storage_url': self.storage_settings.get('endpoint_url'),
+            'storage_sse_enabled': 'False'
+        }
+
+    def restore_from_cold(self, uri, days):
+        """Restore file from cold storage"""
+        raise_no_implemented("MinIO does not support restore from cold")
+
+    def set_lifecycle(self, **kwargs):
+        """Set storage lifecycle"""
+        raise_no_implemented("MinIO does not support lifecycle")
```

### Comparing `basepair-2.1.0/basepair/utils/colors.py` & `basepair-2.1.1/basepair/utils/colors.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/utils/monitor.py` & `basepair-2.1.1/basepair/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/utils/s3.py` & `basepair-2.1.1/basepair/utils/s3.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/utils/sqs.py` & `basepair-2.1.1/basepair/utils/sqs.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair/utils/swf.py` & `basepair-2.1.1/basepair/utils/swf.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/basepair.egg-info/PKG-INFO` & `basepair-2.1.1/basepair.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: basepair
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python client for Basepair's API
 Home-page: https://bitbucket.org/basepair/basepair
-Download-URL: https://bitbucket.org/basepair/basepair/get/2.1.0.tar.gz
+Download-URL: https://bitbucket.org/basepair/basepair/get/2.1.1.tar.gz
 Author: Basepair
 Author-email: info@basepairtech.com
 Keywords: bioinformatics,ngs analysis,dna-seq,rna-seq,chip-seq,atac-seq
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
```

### Comparing `basepair-2.1.0/basepair.egg-info/SOURCES.txt` & `basepair-2.1.1/basepair.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/bin/basepair` & `basepair-2.1.1/bin/basepair`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/bin/common_parser.py` & `basepair-2.1.1/bin/common_parser.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/bin/datatypes/analysis.py` & `basepair-2.1.1/bin/datatypes/analysis.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/bin/datatypes/file.py` & `basepair-2.1.1/bin/datatypes/file.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/bin/datatypes/genome.py` & `basepair-2.1.1/bin/datatypes/genome.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/bin/datatypes/module.py` & `basepair-2.1.1/bin/datatypes/module.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/bin/datatypes/pipeline.py` & `basepair-2.1.1/bin/datatypes/pipeline.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/bin/datatypes/project.py` & `basepair-2.1.1/bin/datatypes/project.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/bin/datatypes/sample.py` & `basepair-2.1.1/bin/datatypes/sample.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/setup.py` & `basepair-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `basepair-2.1.0/tests/test_genes.py` & `basepair-2.1.1/tests/test_genes.py`

 * *Files identical despite different names*

