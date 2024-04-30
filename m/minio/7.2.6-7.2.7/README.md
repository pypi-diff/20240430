# Comparing `tmp/minio-7.2.6.tar.gz` & `tmp/minio-7.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minio-7.2.6.tar", last modified: Thu Apr 25 20:46:42 2024, max compression
+gzip compressed data, was "minio-7.2.7.tar", last modified: Tue Apr 30 21:09:33 2024, max compression
```

## Comparing `minio-7.2.6.tar` & `minio-7.2.7.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.527246 minio-7.2.6/
--rw-r--r--   0 root         (0) root         (0)    11358 2024-04-25 20:44:59.000000 minio-7.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      235 2024-04-25 20:44:59.000000 minio-7.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      361 2024-04-25 20:44:59.000000 minio-7.2.6/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6443 2024-04-25 20:46:42.527246 minio-7.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5326 2024-04-25 20:44:59.000000 minio-7.2.6/README.md
--rw-r--r--   0 root         (0) root         (0)     9087 2024-04-25 20:44:59.000000 minio-7.2.6/README_zh_CN.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.507246 minio-7.2.6/docs/
--rw-r--r--   0 root         (0) root         (0)    63372 2024-04-25 20:44:59.000000 minio-7.2.6/docs/API.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.507246 minio-7.2.6/docs/zh_CN/
--rw-r--r--   0 root         (0) root         (0)    33853 2024-04-25 20:44:59.000000 minio-7.2.6/docs/zh_CN/API.md
--rw-r--r--   0 root         (0) root         (0)      688 2024-04-25 20:44:59.000000 minio-7.2.6/docs/zh_CN/CONTRIBUTING.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.519246 minio-7.2.6/examples/
--rw-r--r--   0 root         (0) root         (0)      930 2024-04-25 20:44:59.000000 minio-7.2.6/examples/bucket_exists.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-04-25 20:44:59.000000 minio-7.2.6/examples/compose_object.py
--rw-r--r--   0 root         (0) root         (0)     1733 2024-04-25 20:44:59.000000 minio-7.2.6/examples/copy_object.py
--rw-r--r--   0 root         (0) root         (0)      873 2024-04-25 20:44:59.000000 minio-7.2.6/examples/delete_bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)      872 2024-04-25 20:44:59.000000 minio-7.2.6/examples/delete_bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)      875 2024-04-25 20:44:59.000000 minio-7.2.6/examples/delete_bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)      869 2024-04-25 20:44:59.000000 minio-7.2.6/examples/delete_bucket_policy.py
--rw-r--r--   0 root         (0) root         (0)      874 2024-04-25 20:44:59.000000 minio-7.2.6/examples/delete_bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-04-25 20:44:59.000000 minio-7.2.6/examples/delete_bucket_tags.py
--rw-r--r--   0 root         (0) root         (0)      874 2024-04-25 20:44:59.000000 minio-7.2.6/examples/delete_object_lock_config.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-25 20:44:59.000000 minio-7.2.6/examples/delete_object_tags.py
--rw-r--r--   0 root         (0) root         (0)      887 2024-04-25 20:44:59.000000 minio-7.2.6/examples/disable_object_legal_hold.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-04-25 20:44:59.000000 minio-7.2.6/examples/enable_object_legal_hold.py
--rw-r--r--   0 root         (0) root         (0)     1288 2024-04-25 20:44:59.000000 minio-7.2.6/examples/fget_object.py
--rw-r--r--   0 root         (0) root         (0)     3561 2024-04-25 20:44:59.000000 minio-7.2.6/examples/fput_object.py
--rw-r--r--   0 root         (0) root         (0)      879 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)      881 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)      875 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_bucket_policy.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)      871 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_bucket_tags.py
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_object.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_object_lock_config.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_object_retention.py
--rw-r--r--   0 root         (0) root         (0)      884 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_object_tags.py
--rw-r--r--   0 root         (0) root         (0)     1600 2024-04-25 20:44:59.000000 minio-7.2.6/examples/get_presigned_url.py
--rw-r--r--   0 root         (0) root         (0)     1000 2024-04-25 20:44:59.000000 minio-7.2.6/examples/is_object_legal_hold_enabled.py
--rw-r--r--   0 root         (0) root         (0)      918 2024-04-25 20:44:59.000000 minio-7.2.6/examples/list_buckets.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-04-25 20:44:59.000000 minio-7.2.6/examples/list_objects.py
--rw-r--r--   0 root         (0) root         (0)     1026 2024-04-25 20:44:59.000000 minio-7.2.6/examples/listen_bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-25 20:44:59.000000 minio-7.2.6/examples/make_bucket.py
--rw-r--r--   0 root         (0) root         (0)     1635 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_assume_role_provider.py
--rw-r--r--   0 root         (0) root         (0)      897 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_aws_config_provider.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_certificate_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)     1274 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_chained_provider.py
--rw-r--r--   0 root         (0) root         (0)     1686 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_client_grants_provider.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_env_aws_provider.py
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_env_minio_provider.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_iam_aws_provider.py
--rw-r--r--   0 root         (0) root         (0)     1161 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_ldap_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)      925 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_minio_client_config_provider.py
--rw-r--r--   0 root         (0) root         (0)     2009 2024-04-25 20:44:59.000000 minio-7.2.6/examples/minio_with_web_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)     1222 2024-04-25 20:44:59.000000 minio-7.2.6/examples/presigned_get_object.py
--rw-r--r--   0 root         (0) root         (0)     1386 2024-04-25 20:44:59.000000 minio-7.2.6/examples/presigned_post_policy.py
--rw-r--r--   0 root         (0) root         (0)     1234 2024-04-25 20:44:59.000000 minio-7.2.6/examples/presigned_put_object.py
--rw-r--r--   0 root         (0) root         (0)     6203 2024-04-25 20:44:59.000000 minio-7.2.6/examples/progress.py
--rw-r--r--   0 root         (0) root         (0)     4036 2024-04-25 20:44:59.000000 minio-7.2.6/examples/put_object.py
--rw-r--r--   0 root         (0) root         (0)      852 2024-04-25 20:44:59.000000 minio-7.2.6/examples/remove_bucket.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-25 20:44:59.000000 minio-7.2.6/examples/remove_object.py
--rw-r--r--   0 root         (0) root         (0)     1490 2024-04-25 20:44:59.000000 minio-7.2.6/examples/remove_objects.py
--rw-r--r--   0 root         (0) root         (0)     1297 2024-04-25 20:44:59.000000 minio-7.2.6/examples/select_object_content.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-25 20:44:59.000000 minio-7.2.6/examples/set_bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)     1410 2024-04-25 20:44:59.000000 minio-7.2.6/examples/set_bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     1260 2024-04-25 20:44:59.000000 minio-7.2.6/examples/set_bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)     2252 2024-04-25 20:44:59.000000 minio-7.2.6/examples/set_bucket_policy.py
--rw-r--r--   0 root         (0) root         (0)     1650 2024-04-25 20:44:59.000000 minio-7.2.6/examples/set_bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)      992 2024-04-25 20:44:59.000000 minio-7.2.6/examples/set_bucket_tags.py
--rw-r--r--   0 root         (0) root         (0)      988 2024-04-25 20:44:59.000000 minio-7.2.6/examples/set_bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-25 20:44:59.000000 minio-7.2.6/examples/set_object_lock_config.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-04-25 20:44:59.000000 minio-7.2.6/examples/set_object_retention.py
--rw-r--r--   0 root         (0) root         (0)     1005 2024-04-25 20:44:59.000000 minio-7.2.6/examples/set_object_tags.py
--rw-r--r--   0 root         (0) root         (0)     1567 2024-04-25 20:44:59.000000 minio-7.2.6/examples/stat_object.py
--rw-r--r--   0 root         (0) root         (0)     1266 2024-04-25 20:44:59.000000 minio-7.2.6/examples/upload_snowball_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.519246 minio-7.2.6/minio/
--rw-r--r--   0 root         (0) root         (0)     1622 2024-04-25 20:44:59.000000 minio-7.2.6/minio/__init__.py
--rw-r--r--   0 root         (0) root         (0)   116808 2024-04-25 20:44:59.000000 minio-7.2.6/minio/api.py
--rw-r--r--   0 root         (0) root         (0)    18536 2024-04-25 20:44:59.000000 minio-7.2.6/minio/commonconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.523246 minio-7.2.6/minio/credentials/
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-25 20:44:59.000000 minio-7.2.6/minio/credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2266 2024-04-25 20:44:59.000000 minio-7.2.6/minio/credentials/credentials.py
--rw-r--r--   0 root         (0) root         (0)    23574 2024-04-25 20:44:59.000000 minio-7.2.6/minio/credentials/providers.py
--rw-r--r--   0 root         (0) root         (0)     7516 2024-04-25 20:44:59.000000 minio-7.2.6/minio/crypto.py
--rw-r--r--   0 root         (0) root         (0)    36127 2024-04-25 20:44:59.000000 minio-7.2.6/minio/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     5760 2024-04-25 20:44:59.000000 minio-7.2.6/minio/deleteobjects.py
--rw-r--r--   0 root         (0) root         (0)     5416 2024-04-25 20:44:59.000000 minio-7.2.6/minio/error.py
--rw-r--r--   0 root         (0) root         (0)    28543 2024-04-25 20:44:59.000000 minio-7.2.6/minio/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1629 2024-04-25 20:44:59.000000 minio-7.2.6/minio/legalhold.py
--rw-r--r--   0 root         (0) root         (0)    15285 2024-04-25 20:44:59.000000 minio-7.2.6/minio/lifecycleconfig.py
--rw-r--r--   0 root         (0) root         (0)    28934 2024-04-25 20:44:59.000000 minio-7.2.6/minio/minioadmin.py
--rw-r--r--   0 root         (0) root         (0)    12129 2024-04-25 20:44:59.000000 minio-7.2.6/minio/notificationconfig.py
--rw-r--r--   0 root         (0) root         (0)     3505 2024-04-25 20:44:59.000000 minio-7.2.6/minio/objectlockconfig.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:44:59.000000 minio-7.2.6/minio/py.typed
--rw-r--r--   0 root         (0) root         (0)    18618 2024-04-25 20:44:59.000000 minio-7.2.6/minio/replicationconfig.py
--rw-r--r--   0 root         (0) root         (0)     2542 2024-04-25 20:44:59.000000 minio-7.2.6/minio/retention.py
--rw-r--r--   0 root         (0) root         (0)    14433 2024-04-25 20:44:59.000000 minio-7.2.6/minio/select.py
--rw-r--r--   0 root         (0) root         (0)     9585 2024-04-25 20:44:59.000000 minio-7.2.6/minio/signer.py
--rw-r--r--   0 root         (0) root         (0)     3445 2024-04-25 20:44:59.000000 minio-7.2.6/minio/sse.py
--rw-r--r--   0 root         (0) root         (0)     3619 2024-04-25 20:44:59.000000 minio-7.2.6/minio/sseconfig.py
--rw-r--r--   0 root         (0) root         (0)     1747 2024-04-25 20:44:59.000000 minio-7.2.6/minio/tagging.py
--rw-r--r--   0 root         (0) root         (0)     3938 2024-04-25 20:44:59.000000 minio-7.2.6/minio/time.py
--rw-r--r--   0 root         (0) root         (0)     3604 2024-04-25 20:44:59.000000 minio-7.2.6/minio/versioningconfig.py
--rw-r--r--   0 root         (0) root         (0)     3879 2024-04-25 20:44:59.000000 minio-7.2.6/minio/xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.527246 minio-7.2.6/minio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6443 2024-04-25 20:46:41.000000 minio-7.2.6/minio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4183 2024-04-25 20:46:42.000000 minio-7.2.6/minio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:46:41.000000 minio-7.2.6/minio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2024-04-25 20:46:41.000000 minio-7.2.6/minio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-25 20:46:41.000000 minio-7.2.6/minio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 20:46:42.527246 minio-7.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2373 2024-04-25 20:44:59.000000 minio-7.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.523246 minio-7.2.6/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:44:59.000000 minio-7.2.6/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.523246 minio-7.2.6/tests/certs/
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-25 20:44:59.000000 minio-7.2.6/tests/certs/private.key
--rw-r--r--   0 root         (0) root         (0)      696 2024-04-25 20:44:59.000000 minio-7.2.6/tests/certs/public.crt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.523246 minio-7.2.6/tests/functional/
--rw-r--r--   0 root         (0) root         (0)      119 2024-04-25 20:44:59.000000 minio-7.2.6/tests/functional/play.min.io.kes.root.key
--rw-r--r--   0 root         (0) root         (0)    70066 2024-04-25 20:44:59.000000 minio-7.2.6/tests/functional/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:46:42.527246 minio-7.2.6/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      656 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2758 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/bucket_exist_test.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/config.json.sample
--rw-r--r--   0 root         (0) root         (0)     1662 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/copy_object_test.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/credentials.empty
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/credentials.sample
--rw-r--r--   0 root         (0) root         (0)     9162 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/credentials_test.py
--rw-r--r--   0 root         (0) root         (0)     1631 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/crypto_test.py
--rw-r--r--   0 root         (0) root         (0)     3612 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/get_bucket_policy_test.py
--rw-r--r--   0 root         (0) root         (0)     2101 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/get_object_test.py
--rw-r--r--   0 root         (0) root         (0)    68504 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/legelhold_test.py
--rw-r--r--   0 root         (0) root         (0)     3045 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/lifecycleconfig_test.py
--rw-r--r--   0 root         (0) root         (0)     3436 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/list_buckets_test.py
--rw-r--r--   0 root         (0) root         (0)     3713 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/list_objects_test.py
--rw-r--r--   0 root         (0) root         (0)     7280 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/list_objects_v1_test.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/make_bucket_test.py
--rw-r--r--   0 root         (0) root         (0)     2891 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/minio_mocks.py
--rw-r--r--   0 root         (0) root         (0)     5972 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/minio_test.py
--rw-r--r--   0 root         (0) root         (0)     2190 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/notificationconfig_test.py
--rw-r--r--   0 root         (0) root         (0)     1486 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/objectlockconfig_test.py
--rw-r--r--   0 root         (0) root         (0)     2014 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/presigned_get_object_test.py
--rw-r--r--   0 root         (0) root         (0)     1383 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/presigned_put_object_test.py
--rw-r--r--   0 root         (0) root         (0)     1595 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/put_object_test.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/remove_bucket_test.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/remove_object_test.py
--rw-r--r--   0 root         (0) root         (0)     3064 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/remove_objects_test.py
--rw-r--r--   0 root         (0) root         (0)     2548 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/replicationconfig_test.py
--rw-r--r--   0 root         (0) root         (0)     1498 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/retention_test.py
--rw-r--r--   0 root         (0) root         (0)     7856 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/sign_test.py
--rw-r--r--   0 root         (0) root         (0)     1572 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/sseconfig_test.py
--rw-r--r--   0 root         (0) root         (0)     2130 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/stat_object_test.py
--rw-r--r--   0 root         (0) root         (0)     1339 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/tagging_test.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/trace_test.py
--rw-r--r--   0 root         (0) root         (0)     1917 2024-04-25 20:44:59.000000 minio-7.2.6/tests/unit/versioningconfig_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.207041 minio-7.2.7/
+-rw-r--r--   0 root         (0) root         (0)    11358 2024-04-30 21:07:49.000000 minio-7.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      235 2024-04-30 21:07:49.000000 minio-7.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      361 2024-04-30 21:07:49.000000 minio-7.2.7/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6444 2024-04-30 21:09:33.207041 minio-7.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5326 2024-04-30 21:07:49.000000 minio-7.2.7/README.md
+-rw-r--r--   0 root         (0) root         (0)     9087 2024-04-30 21:07:49.000000 minio-7.2.7/README_zh_CN.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.175041 minio-7.2.7/docs/
+-rw-r--r--   0 root         (0) root         (0)    63372 2024-04-30 21:07:49.000000 minio-7.2.7/docs/API.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.175041 minio-7.2.7/docs/zh_CN/
+-rw-r--r--   0 root         (0) root         (0)    33853 2024-04-30 21:07:49.000000 minio-7.2.7/docs/zh_CN/API.md
+-rw-r--r--   0 root         (0) root         (0)      688 2024-04-30 21:07:49.000000 minio-7.2.7/docs/zh_CN/CONTRIBUTING.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.191041 minio-7.2.7/examples/
+-rw-r--r--   0 root         (0) root         (0)      930 2024-04-30 21:07:49.000000 minio-7.2.7/examples/bucket_exists.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-04-30 21:07:49.000000 minio-7.2.7/examples/compose_object.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2024-04-30 21:07:49.000000 minio-7.2.7/examples/copy_object.py
+-rw-r--r--   0 root         (0) root         (0)      873 2024-04-30 21:07:49.000000 minio-7.2.7/examples/delete_bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)      872 2024-04-30 21:07:49.000000 minio-7.2.7/examples/delete_bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-04-30 21:07:49.000000 minio-7.2.7/examples/delete_bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)      869 2024-04-30 21:07:49.000000 minio-7.2.7/examples/delete_bucket_policy.py
+-rw-r--r--   0 root         (0) root         (0)      874 2024-04-30 21:07:49.000000 minio-7.2.7/examples/delete_bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-04-30 21:07:49.000000 minio-7.2.7/examples/delete_bucket_tags.py
+-rw-r--r--   0 root         (0) root         (0)      874 2024-04-30 21:07:49.000000 minio-7.2.7/examples/delete_object_lock_config.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-30 21:07:49.000000 minio-7.2.7/examples/delete_object_tags.py
+-rw-r--r--   0 root         (0) root         (0)      887 2024-04-30 21:07:49.000000 minio-7.2.7/examples/disable_object_legal_hold.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-04-30 21:07:49.000000 minio-7.2.7/examples/enable_object_legal_hold.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2024-04-30 21:07:49.000000 minio-7.2.7/examples/fget_object.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2024-04-30 21:07:49.000000 minio-7.2.7/examples/fput_object.py
+-rw-r--r--   0 root         (0) root         (0)      879 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)      881 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_bucket_policy.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)      871 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_bucket_tags.py
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_object.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_object_lock_config.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_object_retention.py
+-rw-r--r--   0 root         (0) root         (0)      884 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_object_tags.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-04-30 21:07:49.000000 minio-7.2.7/examples/get_presigned_url.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2024-04-30 21:07:49.000000 minio-7.2.7/examples/is_object_legal_hold_enabled.py
+-rw-r--r--   0 root         (0) root         (0)      918 2024-04-30 21:07:49.000000 minio-7.2.7/examples/list_buckets.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-30 21:07:49.000000 minio-7.2.7/examples/list_objects.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2024-04-30 21:07:49.000000 minio-7.2.7/examples/listen_bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-30 21:07:49.000000 minio-7.2.7/examples/make_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_assume_role_provider.py
+-rw-r--r--   0 root         (0) root         (0)      897 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_aws_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_certificate_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_chained_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_client_grants_provider.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_env_aws_provider.py
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_env_minio_provider.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_iam_aws_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1161 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_ldap_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)      925 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_minio_client_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-04-30 21:07:49.000000 minio-7.2.7/examples/minio_with_web_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2024-04-30 21:07:49.000000 minio-7.2.7/examples/presigned_get_object.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-04-30 21:07:49.000000 minio-7.2.7/examples/presigned_post_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1234 2024-04-30 21:07:49.000000 minio-7.2.7/examples/presigned_put_object.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2024-04-30 21:07:49.000000 minio-7.2.7/examples/progress.py
+-rw-r--r--   0 root         (0) root         (0)     4036 2024-04-30 21:07:49.000000 minio-7.2.7/examples/put_object.py
+-rw-r--r--   0 root         (0) root         (0)      852 2024-04-30 21:07:49.000000 minio-7.2.7/examples/remove_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-30 21:07:49.000000 minio-7.2.7/examples/remove_object.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2024-04-30 21:07:49.000000 minio-7.2.7/examples/remove_objects.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-04-30 21:07:49.000000 minio-7.2.7/examples/select_object_content.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-30 21:07:49.000000 minio-7.2.7/examples/set_bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2024-04-30 21:07:49.000000 minio-7.2.7/examples/set_bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-04-30 21:07:49.000000 minio-7.2.7/examples/set_bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-30 21:07:49.000000 minio-7.2.7/examples/set_bucket_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-04-30 21:07:49.000000 minio-7.2.7/examples/set_bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)      992 2024-04-30 21:07:49.000000 minio-7.2.7/examples/set_bucket_tags.py
+-rw-r--r--   0 root         (0) root         (0)      988 2024-04-30 21:07:49.000000 minio-7.2.7/examples/set_bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-30 21:07:49.000000 minio-7.2.7/examples/set_object_lock_config.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-30 21:07:49.000000 minio-7.2.7/examples/set_object_retention.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-04-30 21:07:49.000000 minio-7.2.7/examples/set_object_tags.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-04-30 21:07:49.000000 minio-7.2.7/examples/stat_object.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-04-30 21:07:49.000000 minio-7.2.7/examples/upload_snowball_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.199041 minio-7.2.7/minio/
+-rw-r--r--   0 root         (0) root         (0)     1622 2024-04-30 21:07:49.000000 minio-7.2.7/minio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   116710 2024-04-30 21:07:49.000000 minio-7.2.7/minio/api.py
+-rw-r--r--   0 root         (0) root         (0)    18536 2024-04-30 21:07:49.000000 minio-7.2.7/minio/commonconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.199041 minio-7.2.7/minio/credentials/
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-30 21:07:49.000000 minio-7.2.7/minio/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-04-30 21:07:49.000000 minio-7.2.7/minio/credentials/credentials.py
+-rw-r--r--   0 root         (0) root         (0)    23574 2024-04-30 21:07:49.000000 minio-7.2.7/minio/credentials/providers.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2024-04-30 21:07:49.000000 minio-7.2.7/minio/crypto.py
+-rw-r--r--   0 root         (0) root         (0)    36127 2024-04-30 21:07:49.000000 minio-7.2.7/minio/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     5760 2024-04-30 21:07:49.000000 minio-7.2.7/minio/deleteobjects.py
+-rw-r--r--   0 root         (0) root         (0)     5416 2024-04-30 21:07:49.000000 minio-7.2.7/minio/error.py
+-rw-r--r--   0 root         (0) root         (0)    28543 2024-04-30 21:07:49.000000 minio-7.2.7/minio/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2024-04-30 21:07:49.000000 minio-7.2.7/minio/legalhold.py
+-rw-r--r--   0 root         (0) root         (0)    15285 2024-04-30 21:07:49.000000 minio-7.2.7/minio/lifecycleconfig.py
+-rw-r--r--   0 root         (0) root         (0)    28934 2024-04-30 21:07:49.000000 minio-7.2.7/minio/minioadmin.py
+-rw-r--r--   0 root         (0) root         (0)    12129 2024-04-30 21:07:49.000000 minio-7.2.7/minio/notificationconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2024-04-30 21:07:49.000000 minio-7.2.7/minio/objectlockconfig.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 21:07:49.000000 minio-7.2.7/minio/py.typed
+-rw-r--r--   0 root         (0) root         (0)    18618 2024-04-30 21:07:49.000000 minio-7.2.7/minio/replicationconfig.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2024-04-30 21:07:49.000000 minio-7.2.7/minio/retention.py
+-rw-r--r--   0 root         (0) root         (0)    14433 2024-04-30 21:07:49.000000 minio-7.2.7/minio/select.py
+-rw-r--r--   0 root         (0) root         (0)     9585 2024-04-30 21:07:49.000000 minio-7.2.7/minio/signer.py
+-rw-r--r--   0 root         (0) root         (0)     3445 2024-04-30 21:07:49.000000 minio-7.2.7/minio/sse.py
+-rw-r--r--   0 root         (0) root         (0)     3619 2024-04-30 21:07:49.000000 minio-7.2.7/minio/sseconfig.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-04-30 21:07:49.000000 minio-7.2.7/minio/tagging.py
+-rw-r--r--   0 root         (0) root         (0)     3938 2024-04-30 21:07:49.000000 minio-7.2.7/minio/time.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2024-04-30 21:07:49.000000 minio-7.2.7/minio/versioningconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3879 2024-04-30 21:07:49.000000 minio-7.2.7/minio/xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.207041 minio-7.2.7/minio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6444 2024-04-30 21:09:32.000000 minio-7.2.7/minio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4183 2024-04-30 21:09:33.000000 minio-7.2.7/minio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 21:09:32.000000 minio-7.2.7/minio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-04-30 21:09:32.000000 minio-7.2.7/minio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-30 21:09:32.000000 minio-7.2.7/minio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 21:09:33.207041 minio-7.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-30 21:07:49.000000 minio-7.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.199041 minio-7.2.7/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 21:07:49.000000 minio-7.2.7/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.199041 minio-7.2.7/tests/certs/
+-rw-r--r--   0 root         (0) root         (0)      241 2024-04-30 21:07:49.000000 minio-7.2.7/tests/certs/private.key
+-rw-r--r--   0 root         (0) root         (0)      696 2024-04-30 21:07:49.000000 minio-7.2.7/tests/certs/public.crt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.199041 minio-7.2.7/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-30 21:07:49.000000 minio-7.2.7/tests/functional/play.min.io.kes.root.key
+-rw-r--r--   0 root         (0) root         (0)    70066 2024-04-30 21:07:49.000000 minio-7.2.7/tests/functional/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:09:33.207041 minio-7.2.7/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      656 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/bucket_exist_test.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/config.json.sample
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/copy_object_test.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/credentials.empty
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/credentials.sample
+-rw-r--r--   0 root         (0) root         (0)     9162 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/credentials_test.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/crypto_test.py
+-rw-r--r--   0 root         (0) root         (0)     3612 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/get_bucket_policy_test.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/get_object_test.py
+-rw-r--r--   0 root         (0) root         (0)    68504 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/legelhold_test.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/lifecycleconfig_test.py
+-rw-r--r--   0 root         (0) root         (0)     3436 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/list_buckets_test.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/list_objects_test.py
+-rw-r--r--   0 root         (0) root         (0)     7280 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/list_objects_v1_test.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/make_bucket_test.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/minio_mocks.py
+-rw-r--r--   0 root         (0) root         (0)     5972 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/minio_test.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/notificationconfig_test.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/objectlockconfig_test.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/presigned_get_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/presigned_put_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/put_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/remove_bucket_test.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/remove_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/remove_objects_test.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/replicationconfig_test.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/retention_test.py
+-rw-r--r--   0 root         (0) root         (0)     7856 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/sign_test.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/sseconfig_test.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/stat_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/tagging_test.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/trace_test.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-04-30 21:07:49.000000 minio-7.2.7/tests/unit/versioningconfig_test.py
```

### Comparing `minio-7.2.6/LICENSE` & `minio-7.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/PKG-INFO` & `minio-7.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: minio
-Version: 7.2.6
+Version: 7.2.7
 Summary: MinIO Python SDK for Amazon S3 Compatible Cloud Storage
 Home-page: https://github.com/minio/minio-py
 Download-URL: https://github.com/minio/minio-py/releases
 Author: MinIO, Inc.
 Author-email: dev@min.io
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: certifi
 Requires-Dist: urllib3
 Requires-Dist: argon2-cffi
```

### Comparing `minio-7.2.6/README.md` & `minio-7.2.7/README.md`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/README_zh_CN.md` & `minio-7.2.7/README_zh_CN.md`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/docs/API.md` & `minio-7.2.7/docs/API.md`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/docs/zh_CN/API.md` & `minio-7.2.7/docs/zh_CN/API.md`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/docs/zh_CN/CONTRIBUTING.md` & `minio-7.2.7/docs/zh_CN/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/bucket_exists.py` & `minio-7.2.7/examples/bucket_exists.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/compose_object.py` & `minio-7.2.7/examples/compose_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/copy_object.py` & `minio-7.2.7/examples/copy_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/delete_bucket_encryption.py` & `minio-7.2.7/examples/delete_bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/delete_bucket_lifecycle.py` & `minio-7.2.7/examples/delete_bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/delete_bucket_notification.py` & `minio-7.2.7/examples/delete_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/delete_bucket_policy.py` & `minio-7.2.7/examples/delete_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/delete_bucket_replication.py` & `minio-7.2.7/examples/delete_bucket_replication.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/delete_bucket_tags.py` & `minio-7.2.7/examples/delete_bucket_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/delete_object_lock_config.py` & `minio-7.2.7/examples/delete_object_lock_config.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/delete_object_tags.py` & `minio-7.2.7/examples/delete_object_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/disable_object_legal_hold.py` & `minio-7.2.7/examples/disable_object_legal_hold.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/enable_object_legal_hold.py` & `minio-7.2.7/examples/enable_object_legal_hold.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/fget_object.py` & `minio-7.2.7/examples/fget_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/fput_object.py` & `minio-7.2.7/examples/fput_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_bucket_encryption.py` & `minio-7.2.7/examples/get_bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_bucket_lifecycle.py` & `minio-7.2.7/examples/get_bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_bucket_notification.py` & `minio-7.2.7/examples/get_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_bucket_policy.py` & `minio-7.2.7/examples/get_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_bucket_replication.py` & `minio-7.2.7/examples/get_bucket_replication.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_bucket_tags.py` & `minio-7.2.7/examples/get_bucket_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_bucket_versioning.py` & `minio-7.2.7/examples/get_bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_object.py` & `minio-7.2.7/examples/get_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_object_lock_config.py` & `minio-7.2.7/examples/get_object_lock_config.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_object_retention.py` & `minio-7.2.7/examples/get_object_retention.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_object_tags.py` & `minio-7.2.7/examples/get_object_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/get_presigned_url.py` & `minio-7.2.7/examples/get_presigned_url.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/is_object_legal_hold_enabled.py` & `minio-7.2.7/examples/is_object_legal_hold_enabled.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/list_buckets.py` & `minio-7.2.7/examples/list_buckets.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/list_objects.py` & `minio-7.2.7/examples/list_objects.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/listen_bucket_notification.py` & `minio-7.2.7/examples/listen_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/make_bucket.py` & `minio-7.2.7/examples/make_bucket.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_assume_role_provider.py` & `minio-7.2.7/examples/minio_with_assume_role_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_aws_config_provider.py` & `minio-7.2.7/examples/minio_with_aws_config_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_certificate_identity_provider.py` & `minio-7.2.7/examples/minio_with_certificate_identity_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_chained_provider.py` & `minio-7.2.7/examples/minio_with_chained_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_client_grants_provider.py` & `minio-7.2.7/examples/minio_with_client_grants_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_env_aws_provider.py` & `minio-7.2.7/examples/minio_with_env_aws_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_env_minio_provider.py` & `minio-7.2.7/examples/minio_with_env_minio_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_iam_aws_provider.py` & `minio-7.2.7/examples/minio_with_iam_aws_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_ldap_identity_provider.py` & `minio-7.2.7/examples/minio_with_ldap_identity_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_minio_client_config_provider.py` & `minio-7.2.7/examples/minio_with_minio_client_config_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/minio_with_web_identity_provider.py` & `minio-7.2.7/examples/minio_with_web_identity_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/presigned_get_object.py` & `minio-7.2.7/examples/presigned_get_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/presigned_post_policy.py` & `minio-7.2.7/examples/presigned_post_policy.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/presigned_put_object.py` & `minio-7.2.7/examples/presigned_put_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/progress.py` & `minio-7.2.7/examples/progress.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/put_object.py` & `minio-7.2.7/examples/put_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/remove_bucket.py` & `minio-7.2.7/examples/remove_bucket.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/remove_object.py` & `minio-7.2.7/examples/remove_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/remove_objects.py` & `minio-7.2.7/examples/remove_objects.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/select_object_content.py` & `minio-7.2.7/examples/select_object_content.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/set_bucket_encryption.py` & `minio-7.2.7/examples/set_bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/set_bucket_lifecycle.py` & `minio-7.2.7/examples/set_bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/set_bucket_notification.py` & `minio-7.2.7/examples/set_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/set_bucket_policy.py` & `minio-7.2.7/examples/set_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/set_bucket_replication.py` & `minio-7.2.7/examples/set_bucket_replication.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/set_bucket_tags.py` & `minio-7.2.7/examples/set_bucket_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/set_bucket_versioning.py` & `minio-7.2.7/examples/set_bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/set_object_lock_config.py` & `minio-7.2.7/examples/set_object_lock_config.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/set_object_retention.py` & `minio-7.2.7/examples/set_object_retention.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/set_object_tags.py` & `minio-7.2.7/examples/set_object_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/stat_object.py` & `minio-7.2.7/examples/stat_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/examples/upload_snowball_objects.py` & `minio-7.2.7/examples/upload_snowball_objects.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/__init__.py` & `minio-7.2.7/minio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 :copyright: (C) 2015-2020 MinIO, Inc.
 :license: Apache 2.0, see LICENSE for more details.
 """
 
 __title__ = "minio-py"
 __author__ = "MinIO, Inc."
-__version__ = "7.2.6"
+__version__ = "7.2.7"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright 2015, 2016, 2017, 2018, 2019, 2020 MinIO, Inc."
 
 # pylint: disable=unused-import,useless-import-alias
 from .api import Minio as Minio
 from .error import InvalidResponseError as InvalidResponseError
 from .error import S3Error as S3Error
```

### Comparing `minio-7.2.6/minio/api.py` & `minio-7.2.7/minio/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1597,32 +1597,30 @@
                         part_number,
                         headers,
                     )
                     total_parts.append(Part(part_number, etag))
                     continue
                 while size > 0:
                     part_number += 1
-                    start_bytes = offset
-                    end_bytes = start_bytes + MAX_PART_SIZE
-                    if size < MAX_PART_SIZE:
-                        end_bytes = start_bytes + size
+                    length = size if size < MAX_PART_SIZE else MAX_PART_SIZE
+                    end_bytes = offset + length - 1
                     headers_copy = headers.copy()
                     headers_copy["x-amz-copy-source-range"] = (
-                        f"bytes={start_bytes}-{end_bytes}"
+                        f"bytes={offset}-{end_bytes}"
                     )
                     etag, _ = self._upload_part_copy(
                         bucket_name,
                         object_name,
                         upload_id,
                         part_number,
                         headers_copy,
                     )
                     total_parts.append(Part(part_number, etag))
-                    offset = start_bytes
-                    size -= end_bytes - start_bytes
+                    offset += length
+                    size -= length
             result = self._complete_multipart_upload(
                 bucket_name, object_name, upload_id, total_parts,
             )
             return ObjectWriteResult(
                 cast(str, result.bucket_name),
                 cast(str, result.object_name),
                 result.version_id,
```

### Comparing `minio-7.2.6/minio/commonconfig.py` & `minio-7.2.7/minio/commonconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/credentials/__init__.py` & `minio-7.2.7/minio/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/credentials/credentials.py` & `minio-7.2.7/minio/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/credentials/providers.py` & `minio-7.2.7/minio/credentials/providers.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/crypto.py` & `minio-7.2.7/minio/crypto.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/datatypes.py` & `minio-7.2.7/minio/datatypes.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/deleteobjects.py` & `minio-7.2.7/minio/deleteobjects.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/error.py` & `minio-7.2.7/minio/error.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/helpers.py` & `minio-7.2.7/minio/helpers.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/legalhold.py` & `minio-7.2.7/minio/legalhold.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/lifecycleconfig.py` & `minio-7.2.7/minio/lifecycleconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/minioadmin.py` & `minio-7.2.7/minio/minioadmin.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/notificationconfig.py` & `minio-7.2.7/minio/notificationconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/objectlockconfig.py` & `minio-7.2.7/minio/objectlockconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/replicationconfig.py` & `minio-7.2.7/minio/replicationconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/retention.py` & `minio-7.2.7/minio/retention.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/select.py` & `minio-7.2.7/minio/select.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/signer.py` & `minio-7.2.7/minio/signer.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/sse.py` & `minio-7.2.7/minio/sse.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/sseconfig.py` & `minio-7.2.7/minio/sseconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/tagging.py` & `minio-7.2.7/minio/tagging.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/time.py` & `minio-7.2.7/minio/time.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/versioningconfig.py` & `minio-7.2.7/minio/versioningconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio/xml.py` & `minio-7.2.7/minio/xml.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/minio.egg-info/PKG-INFO` & `minio-7.2.7/minio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: minio
-Version: 7.2.6
+Version: 7.2.7
 Summary: MinIO Python SDK for Amazon S3 Compatible Cloud Storage
 Home-page: https://github.com/minio/minio-py
 Download-URL: https://github.com/minio/minio-py/releases
 Author: MinIO, Inc.
 Author-email: dev@min.io
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: certifi
 Requires-Dist: urllib3
 Requires-Dist: argon2-cffi
```

### Comparing `minio-7.2.6/minio.egg-info/SOURCES.txt` & `minio-7.2.7/minio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/setup.py` & `minio-7.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,18 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     long_description=readme,
     package_data={"": ["LICENSE", "README.md"]},
     include_package_data=True,
 )
```

### Comparing `minio-7.2.6/tests/certs/public.crt` & `minio-7.2.7/tests/certs/public.crt`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/functional/tests.py` & `minio-7.2.7/tests/functional/tests.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/__init__.py` & `minio-7.2.7/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/bucket_exist_test.py` & `minio-7.2.7/tests/unit/bucket_exist_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/copy_object_test.py` & `minio-7.2.7/tests/unit/copy_object_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/credentials_test.py` & `minio-7.2.7/tests/unit/credentials_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/crypto_test.py` & `minio-7.2.7/tests/unit/crypto_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/get_bucket_policy_test.py` & `minio-7.2.7/tests/unit/get_bucket_policy_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/get_object_test.py` & `minio-7.2.7/tests/unit/get_object_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/helpers.py` & `minio-7.2.7/tests/unit/helpers.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/legelhold_test.py` & `minio-7.2.7/tests/unit/legelhold_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/lifecycleconfig_test.py` & `minio-7.2.7/tests/unit/lifecycleconfig_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/list_buckets_test.py` & `minio-7.2.7/tests/unit/list_buckets_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/list_objects_test.py` & `minio-7.2.7/tests/unit/list_objects_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/list_objects_v1_test.py` & `minio-7.2.7/tests/unit/list_objects_v1_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/make_bucket_test.py` & `minio-7.2.7/tests/unit/make_bucket_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/minio_mocks.py` & `minio-7.2.7/tests/unit/minio_mocks.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/minio_test.py` & `minio-7.2.7/tests/unit/minio_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/notificationconfig_test.py` & `minio-7.2.7/tests/unit/notificationconfig_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/objectlockconfig_test.py` & `minio-7.2.7/tests/unit/objectlockconfig_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/presigned_get_object_test.py` & `minio-7.2.7/tests/unit/presigned_get_object_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/presigned_put_object_test.py` & `minio-7.2.7/tests/unit/presigned_put_object_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/put_object_test.py` & `minio-7.2.7/tests/unit/put_object_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/remove_bucket_test.py` & `minio-7.2.7/tests/unit/remove_bucket_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/remove_object_test.py` & `minio-7.2.7/tests/unit/remove_object_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/remove_objects_test.py` & `minio-7.2.7/tests/unit/remove_objects_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/replicationconfig_test.py` & `minio-7.2.7/tests/unit/replicationconfig_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/retention_test.py` & `minio-7.2.7/tests/unit/retention_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/sign_test.py` & `minio-7.2.7/tests/unit/sign_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/sseconfig_test.py` & `minio-7.2.7/tests/unit/sseconfig_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/stat_object_test.py` & `minio-7.2.7/tests/unit/stat_object_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/tagging_test.py` & `minio-7.2.7/tests/unit/tagging_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/trace_test.py` & `minio-7.2.7/tests/unit/trace_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.2.6/tests/unit/versioningconfig_test.py` & `minio-7.2.7/tests/unit/versioningconfig_test.py`

 * *Files identical despite different names*

