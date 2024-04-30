# Comparing `tmp/core-aws-1.0.2.tar.gz` & `tmp/core_aws-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-aws-1.0.2.tar", last modified: Sun Mar 31 15:51:50 2024, max compression
+gzip compressed data, was "core_aws-1.0.3.tar", last modified: Tue Apr 30 04:25:25 2024, max compression
```

## Comparing `core-aws-1.0.2.tar` & `core_aws-1.0.3.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.760999 core-aws-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1082 2024-03-31 15:51:35.000000 core-aws-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1660 2024-03-31 15:51:50.759999 core-aws-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      643 2024-03-31 15:51:35.000000 core-aws-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.749999 core-aws-1.0.2/core_aws/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.751999 core-aws-1.0.2/core_aws/ciphers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/ciphers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1325 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/ciphers/kms_cipher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.751999 core-aws-1.0.2/core_aws/etls/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/etls/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3718 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/etls/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3425 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/etls/bucket_based.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/etls/sqs_based.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.752999 core-aws-1.0.2/core_aws/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.752999 core-aws-1.0.2/core_aws/services/dynamo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/dynamo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7363 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/dynamo/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.753999 core-aws-1.0.2/core_aws/services/ecs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/ecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9608 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/ecs/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.753999 core-aws-1.0.2/core_aws/services/kinesis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/kinesis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6930 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/kinesis/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.754999 core-aws-1.0.2/core_aws/services/lambda_fcn/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/lambda_fcn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6884 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/lambda_fcn/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.755999 core-aws-1.0.2/core_aws/services/lambda_fcn/events/
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/lambda_fcn/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1322 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/lambda_fcn/events/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1592 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/lambda_fcn/events/kinesis_stream.py
--rw-rw-rw-   0 root         (0) root         (0)      741 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/lambda_fcn/events/sns_topic.py
--rw-rw-rw-   0 root         (0) root         (0)     1111 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/lambda_fcn/events/sqs_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.755999 core-aws-1.0.2/core_aws/services/s3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12416 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/s3/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.756999 core-aws-1.0.2/core_aws/services/sns/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/sns/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9830 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/sns/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.756999 core-aws-1.0.2/core_aws/services/sqs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/sqs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8069 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/sqs/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.757999 core-aws-1.0.2/core_aws/services/ssm/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/ssm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8846 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/services/ssm/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.757999 core-aws-1.0.2/core_aws/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6698 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/tests/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.759999 core-aws-1.0.2/core_aws/typing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/typing/client_context.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/typing/cognito_identity.py
--rw-rw-rw-   0 root         (0) root         (0)     2851 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/typing/lambda_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1149 2024-03-31 15:51:35.000000 core-aws-1.0.2/core_aws/typing/mobile_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:51:50.759999 core-aws-1.0.2/core_aws.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-03-31 15:51:50.000000 core-aws-1.0.2/core_aws.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1459 2024-03-31 15:51:50.000000 core-aws-1.0.2/core_aws.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 15:51:50.000000 core-aws-1.0.2/core_aws.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      140 2024-03-31 15:51:50.000000 core-aws-1.0.2/core_aws.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-31 15:51:50.000000 core-aws-1.0.2/core_aws.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1364 2024-03-31 15:51:35.000000 core-aws-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-31 15:51:50.760999 core-aws-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-03-31 15:51:35.000000 core-aws-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.407691 core_aws-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2024-04-30 04:25:10.000000 core_aws-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-04-30 04:25:25.407691 core_aws-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      643 2024-04-30 04:25:10.000000 core_aws-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.397691 core_aws-1.0.3/core_aws/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.398692 core_aws-1.0.3/core_aws/ciphers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/ciphers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/ciphers/kms_cipher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.399691 core_aws-1.0.3/core_aws/etls/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/etls/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/etls/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3425 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/etls/bucket_based.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/etls/sqs_based.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.400691 core_aws-1.0.3/core_aws/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.400691 core_aws-1.0.3/core_aws/services/cloud_formation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/cloud_formation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/cloud_formation/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.400691 core_aws-1.0.3/core_aws/services/dynamo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/dynamo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7363 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/dynamo/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.401691 core_aws-1.0.3/core_aws/services/ecs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/ecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9608 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/ecs/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.401691 core_aws-1.0.3/core_aws/services/kinesis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/kinesis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6930 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/kinesis/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.402691 core_aws-1.0.3/core_aws/services/lambda_fcn/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/lambda_fcn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6884 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/lambda_fcn/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.403691 core_aws-1.0.3/core_aws/services/lambda_fcn/events/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/lambda_fcn/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/lambda_fcn/events/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/lambda_fcn/events/kinesis_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)      741 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/lambda_fcn/events/sns_topic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/lambda_fcn/events/sqs_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.403691 core_aws-1.0.3/core_aws/services/s3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12416 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/s3/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.404691 core_aws-1.0.3/core_aws/services/sns/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/sns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9830 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/sns/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.404691 core_aws-1.0.3/core_aws/services/sqs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/sqs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8069 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/sqs/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.405691 core_aws-1.0.3/core_aws/services/ssm/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/ssm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8846 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/services/ssm/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.405691 core_aws-1.0.3/core_aws/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6698 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/tests/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.406691 core_aws-1.0.3/core_aws/typing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/typing/client_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/typing/cognito_identity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2851 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/typing/lambda_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2024-04-30 04:25:10.000000 core_aws-1.0.3/core_aws/typing/mobile_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 04:25:25.406691 core_aws-1.0.3/core_aws.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-04-30 04:25:25.000000 core_aws-1.0.3/core_aws.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1549 2024-04-30 04:25:25.000000 core_aws-1.0.3/core_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 04:25:25.000000 core_aws-1.0.3/core_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-30 04:25:25.000000 core_aws-1.0.3/core_aws.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-30 04:25:25.000000 core_aws-1.0.3/core_aws.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2024-04-30 04:25:10.000000 core_aws-1.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 04:25:25.407691 core_aws-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-30 04:25:10.000000 core_aws-1.0.3/setup.py
```

### Comparing `core-aws-1.0.2/LICENSE` & `core_aws-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/PKG-INFO` & `core_aws-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-aws
-Version: 1.0.2
+Version: 1.0.3
 Summary: This project/library contains common elements related to AWS services...
 Author-email: Alejandro Cora González <alek.cora.glez@gmail.com>
 Maintainer: Alejandro Cora González
 License: MIT
 Project-URL: Homepage, https://gitlab.com/bytecode-solutions/core/core-aws
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -17,16 +17,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: core-mixins==1.0.4
 Requires-Dist: core-ciphers==1.0.1
 Requires-Dist: core-tests==1.0.3
 Requires-Dist: core-etl==1.0.3
 Requires-Dist: aws-encryption-sdk==3.1.1
-Requires-Dist: boto3==1.34.74
-Requires-Dist: botocore==1.34.74
+Requires-Dist: boto3==1.34.94
+Requires-Dist: botocore==1.34.94
 Provides-Extra: test
 
 # core-aws
 _______________________________________________________________________________
 
 This project/library contains common elements related to AWS services...
```

### Comparing `core-aws-1.0.2/README.md` & `core_aws-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/ciphers/kms_cipher.py` & `core_aws-1.0.3/core_aws/ciphers/kms_cipher.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/etls/base.py` & `core_aws-1.0.3/core_aws/etls/base.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/etls/bucket_based.py` & `core_aws-1.0.3/core_aws/etls/bucket_based.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/etls/sqs_based.py` & `core_aws-1.0.3/core_aws/etls/sqs_based.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/dynamo/client.py` & `core_aws-1.0.3/core_aws/services/dynamo/client.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/ecs/client.py` & `core_aws-1.0.3/core_aws/services/ecs/client.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/kinesis/client.py` & `core_aws-1.0.3/core_aws/services/kinesis/client.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/lambda_fcn/decorators.py` & `core_aws-1.0.3/core_aws/services/lambda_fcn/decorators.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/lambda_fcn/events/base.py` & `core_aws-1.0.3/core_aws/services/lambda_fcn/events/base.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/lambda_fcn/events/kinesis_stream.py` & `core_aws-1.0.3/core_aws/services/lambda_fcn/events/kinesis_stream.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/lambda_fcn/events/sns_topic.py` & `core_aws-1.0.3/core_aws/services/lambda_fcn/events/sns_topic.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/lambda_fcn/events/sqs_queue.py` & `core_aws-1.0.3/core_aws/services/lambda_fcn/events/sqs_queue.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/s3/client.py` & `core_aws-1.0.3/core_aws/services/s3/client.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/sns/client.py` & `core_aws-1.0.3/core_aws/services/sns/client.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/sqs/client.py` & `core_aws-1.0.3/core_aws/services/sqs/client.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/services/ssm/client.py` & `core_aws-1.0.3/core_aws/services/ssm/client.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/tests/base.py` & `core_aws-1.0.3/core_aws/tests/base.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/typing/client_context.py` & `core_aws-1.0.3/core_aws/typing/client_context.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/typing/cognito_identity.py` & `core_aws-1.0.3/core_aws/typing/cognito_identity.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/typing/lambda_context.py` & `core_aws-1.0.3/core_aws/typing/lambda_context.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws/typing/mobile_client.py` & `core_aws-1.0.3/core_aws/typing/mobile_client.py`

 * *Files identical despite different names*

### Comparing `core-aws-1.0.2/core_aws.egg-info/PKG-INFO` & `core_aws-1.0.3/core_aws.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-aws
-Version: 1.0.2
+Version: 1.0.3
 Summary: This project/library contains common elements related to AWS services...
 Author-email: Alejandro Cora González <alek.cora.glez@gmail.com>
 Maintainer: Alejandro Cora González
 License: MIT
 Project-URL: Homepage, https://gitlab.com/bytecode-solutions/core/core-aws
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -17,16 +17,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: core-mixins==1.0.4
 Requires-Dist: core-ciphers==1.0.1
 Requires-Dist: core-tests==1.0.3
 Requires-Dist: core-etl==1.0.3
 Requires-Dist: aws-encryption-sdk==3.1.1
-Requires-Dist: boto3==1.34.74
-Requires-Dist: botocore==1.34.74
+Requires-Dist: boto3==1.34.94
+Requires-Dist: botocore==1.34.94
 Provides-Extra: test
 
 # core-aws
 _______________________________________________________________________________
 
 This project/library contains common elements related to AWS services...
```

### Comparing `core-aws-1.0.2/core_aws.egg-info/SOURCES.txt` & `core_aws-1.0.3/core_aws.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 core_aws/ciphers/kms_cipher.py
 core_aws/etls/__init__.py
 core_aws/etls/base.py
 core_aws/etls/bucket_based.py
 core_aws/etls/sqs_based.py
 core_aws/services/__init__.py
 core_aws/services/base.py
+core_aws/services/cloud_formation/__init__.py
+core_aws/services/cloud_formation/client.py
 core_aws/services/dynamo/__init__.py
 core_aws/services/dynamo/client.py
 core_aws/services/ecs/__init__.py
 core_aws/services/ecs/client.py
 core_aws/services/kinesis/__init__.py
 core_aws/services/kinesis/client.py
 core_aws/services/lambda_fcn/__init__.py
```

### Comparing `core-aws-1.0.2/pyproject.toml` & `core_aws-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "core-aws"
 description = "This project/library contains common elements related to AWS services..."
-version = "1.0.2"
+version = "1.0.3"
 
 authors = [
     {name = "Alejandro Cora González", email = "alek.cora.glez@gmail.com"}
 ]
 
 maintainers = [
     {name = "Alejandro Cora González"}
@@ -36,16 +36,16 @@
 
 dependencies = [
     "core-mixins==1.0.4",
     "core-ciphers==1.0.1",
     "core-tests==1.0.3",
     "core-etl==1.0.3",
     "aws-encryption-sdk==3.1.1",
-    "boto3==1.34.74",
-    "botocore==1.34.74"
+    "boto3==1.34.94",
+    "botocore==1.34.94"
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/bytecode-solutions/core/core-aws"
 
 [project.optional-dependencies]
 test = []
```

