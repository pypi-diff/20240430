# Comparing `tmp/drf_easily_saas-0.0.2.tar.gz` & `tmp/drf_easily_saas-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_easily_saas-0.0.2.tar", max compression
+gzip compressed data, was "drf_easily_saas-0.0.3.tar", max compression
```

## Comparing `drf_easily_saas-0.0.2.tar` & `drf_easily_saas-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,78 @@
--rw-r--r--   0        0        0     3293 2024-04-29 23:03:05.418285 drf_easily_saas-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_saas-0.0.2/drf_easily_saas/__init__.py
--rw-r--r--   0        0        0      202 2024-04-28 00:35:57.188145 drf_easily_saas-0.0.2/drf_easily_saas/admin.py
--rw-r--r--   0        0        0      385 2024-04-26 09:41:08.737105 drf_easily_saas-0.0.2/drf_easily_saas/app.py
--rw-r--r--   0        0        0        0 2024-04-25 08:46:00.373930 drf_easily_saas-0.0.2/drf_easily_saas/auth/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 11:47:52.771360 drf_easily_saas-0.0.2/drf_easily_saas/auth/firebase/__init__.py
--rw-r--r--   0        0        0     4307 2024-04-29 22:32:49.562607 drf_easily_saas-0.0.2/drf_easily_saas/auth/firebase/protect.py
--rw-r--r--   0        0        0     1010 2024-04-29 22:33:28.926860 drf_easily_saas-0.0.2/drf_easily_saas/auth/firebase/state_manager.py
--rw-r--r--   0        0        0        0 2024-04-28 13:00:51.390262 drf_easily_saas-0.0.2/drf_easily_saas/exceptions/__init__.py
--rw-r--r--   0        0        0      729 2024-04-28 13:12:31.045452 drf_easily_saas-0.0.2/drf_easily_saas/exceptions/base.py
--rw-r--r--   0        0        0     1360 2024-04-28 13:12:26.941420 drf_easily_saas-0.0.2/drf_easily_saas/exceptions/config.py
--rw-r--r--   0        0        0      350 2024-04-28 13:14:03.922181 drf_easily_saas-0.0.2/drf_easily_saas/exceptions/firebase.py
--rw-r--r--   0        0        0      673 2024-04-29 22:56:29.583740 drf_easily_saas-0.0.2/drf_easily_saas/exceptions/stripe.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_saas-0.0.2/drf_easily_saas/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_saas-0.0.2/drf_easily_saas/management/commands/__init__.py
--rw-r--r--   0        0        0     1911 2024-04-26 06:56:36.644489 drf_easily_saas-0.0.2/drf_easily_saas/management/commands/syncfirebaseusers.py
--rw-r--r--   0        0        0     2210 2024-04-25 08:58:35.026313 drf_easily_saas-0.0.2/drf_easily_saas/migrations/0001_initial.py
--rw-r--r--   0        0        0      641 2024-04-28 10:24:49.641296 drf_easily_saas-0.0.2/drf_easily_saas/migrations/0002_alter_subscription_options_and_more.py
--rw-r--r--   0        0        0      485 2024-04-28 10:25:24.197673 drf_easily_saas-0.0.2/drf_easily_saas/migrations/0003_alter_subscription_unique_together.py
--rw-r--r--   0        0        0        0 2024-04-25 08:37:58.179115 drf_easily_saas-0.0.2/drf_easily_saas/migrations/__init__.py
--rw-r--r--   0        0        0     1709 2024-04-29 22:43:04.290561 drf_easily_saas-0.0.2/drf_easily_saas/models.py
--rw-r--r--   0        0        0        0 2024-04-25 08:46:04.593982 drf_easily_saas-0.0.2/drf_easily_saas/payment/__init__.py
--rw-r--r--   0        0        0     8710 2024-04-29 23:18:41.352304 drf_easily_saas-0.0.2/drf_easily_saas/payment/manager.py
--rw-r--r--   0        0        0      263 2024-04-26 06:56:09.160156 drf_easily_saas-0.0.2/drf_easily_saas/payment/serializers.py
--rw-r--r--   0        0        0        0 2024-04-25 08:17:36.503667 drf_easily_saas-0.0.2/drf_easily_saas/payment/stripe/__init__.py
--rw-r--r--   0        0        0     1110 2024-04-25 08:17:36.507667 drf_easily_saas-0.0.2/drf_easily_saas/payment/stripe/serializers.py
--rw-r--r--   0        0        0      671 2024-04-26 09:47:15.905753 drf_easily_saas-0.0.2/drf_easily_saas/payment/stripe/urls.py
--rw-r--r--   0        0        0     3329 2024-04-29 22:34:19.799188 drf_easily_saas-0.0.2/drf_easily_saas/payment/stripe/views.py
--rw-r--r--   0        0        0      289 2024-04-26 10:54:18.688748 drf_easily_saas-0.0.2/drf_easily_saas/payment/urls.py
--rw-r--r--   0        0        0        0 2024-04-26 09:38:05.814726 drf_easily_saas-0.0.2/drf_easily_saas/schemas/__init__.py
--rw-r--r--   0        0        0     1648 2024-04-29 22:53:44.946681 drf_easily_saas-0.0.2/drf_easily_saas/schemas/claims.py
--rw-r--r--   0        0        0     2086 2024-04-28 14:54:43.947705 drf_easily_saas-0.0.2/drf_easily_saas/schemas/config.py
--rw-r--r--   0        0        0      627 2024-04-29 22:40:19.377500 drf_easily_saas-0.0.2/drf_easily_saas/schemas/constants.py
--rw-r--r--   0        0        0     3534 2024-04-28 21:47:18.360167 drf_easily_saas-0.0.2/drf_easily_saas/schemas/firebase.py
--rw-r--r--   0        0        0     5796 2024-04-28 21:48:02.052429 drf_easily_saas-0.0.2/drf_easily_saas/schemas/stripe.py
--rw-r--r--   0        0        0      461 2024-04-28 13:15:55.107103 drf_easily_saas-0.0.2/drf_easily_saas/schemas/utils.py
--rw-r--r--   0        0        0      808 2024-04-28 21:37:39.605450 drf_easily_saas-0.0.2/drf_easily_saas/settings.py
--rw-r--r--   0        0        0        0 2024-04-26 10:03:14.529552 drf_easily_saas-0.0.2/drf_easily_saas/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 10:03:31.689761 drf_easily_saas-0.0.2/drf_easily_saas/tests/user_stories/__init__.py
--rw-r--r--   0        0        0     2075 2024-04-29 12:28:35.269922 drf_easily_saas-0.0.2/drf_easily_saas/tests/user_stories/test_checkout.py
--rw-r--r--   0        0        0      265 2024-04-28 16:54:44.524990 drf_easily_saas-0.0.2/drf_easily_saas/urls.py
--rw-r--r--   0        0        0        0 2024-04-26 07:03:02.729014 drf_easily_saas-0.0.2/drf_easily_saas/utils/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-28 13:14:42.178492 drf_easily_saas-0.0.2/drf_easily_saas/utils/db.py
--rw-r--r--   0        0        0      525 2024-04-29 22:56:10.443616 drf_easily_saas-0.0.2/drf_easily_saas/utils/urls.py
--rw-r--r--   0        0        0      872 2024-04-29 23:34:11.238878 drf_easily_saas-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4410 1970-01-01 00:00:00.000000 drf_easily_saas-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3293 2024-04-30 09:05:16.884582 drf_easily_saas-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_saas-0.0.3/drf_easily_saas/__init__.py
+-rw-r--r--   0        0        0      202 2024-04-28 00:35:57.188145 drf_easily_saas-0.0.3/drf_easily_saas/admin.py
+-rw-r--r--   0        0        0      385 2024-04-26 09:41:08.737105 drf_easily_saas-0.0.3/drf_easily_saas/app.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:46:00.373930 drf_easily_saas-0.0.3/drf_easily_saas/auth/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-26 10:44:26.361923 drf_easily_saas-0.0.3/drf_easily_saas/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3364 2024-04-26 11:29:58.016132 drf_easily_saas-0.0.3/drf_easily_saas/auth/__pycache__/firebase.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-26 11:47:52.771360 drf_easily_saas-0.0.3/drf_easily_saas/auth/firebase/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-26 11:49:56.509112 drf_easily_saas-0.0.3/drf_easily_saas/auth/firebase/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3342 2024-04-29 22:32:49.654608 drf_easily_saas-0.0.3/drf_easily_saas/auth/firebase/__pycache__/protect.cpython-310.pyc
+-rw-r--r--   0        0        0      774 2024-04-30 09:05:03.488303 drf_easily_saas-0.0.3/drf_easily_saas/auth/firebase/__pycache__/state_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     4307 2024-04-29 22:32:49.562607 drf_easily_saas-0.0.3/drf_easily_saas/auth/firebase/protect.py
+-rw-r--r--   0        0        0        0 2024-04-28 13:00:51.390262 drf_easily_saas-0.0.3/drf_easily_saas/exceptions/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-28 13:08:55.671951 drf_easily_saas-0.0.3/drf_easily_saas/exceptions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1159 2024-04-28 13:13:10.973760 drf_easily_saas-0.0.3/drf_easily_saas/exceptions/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1863 2024-04-28 13:13:10.985760 drf_easily_saas-0.0.3/drf_easily_saas/exceptions/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0      792 2024-04-28 13:14:29.730390 drf_easily_saas-0.0.3/drf_easily_saas/exceptions/__pycache__/firebase.cpython-310.pyc
+-rw-r--r--   0        0        0     1204 2024-04-29 22:56:29.883741 drf_easily_saas-0.0.3/drf_easily_saas/exceptions/__pycache__/stripe.cpython-310.pyc
+-rw-r--r--   0        0        0      729 2024-04-28 13:12:31.045452 drf_easily_saas-0.0.3/drf_easily_saas/exceptions/base.py
+-rw-r--r--   0        0        0     1360 2024-04-28 13:12:26.941420 drf_easily_saas-0.0.3/drf_easily_saas/exceptions/config.py
+-rw-r--r--   0        0        0      350 2024-04-28 13:14:03.922181 drf_easily_saas-0.0.3/drf_easily_saas/exceptions/firebase.py
+-rw-r--r--   0        0        0      673 2024-04-29 22:56:29.583740 drf_easily_saas-0.0.3/drf_easily_saas/exceptions/stripe.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_saas-0.0.3/drf_easily_saas/management/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-25 22:16:19.080850 drf_easily_saas-0.0.3/drf_easily_saas/management/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_saas-0.0.3/drf_easily_saas/management/commands/__init__.py
+-rw-r--r--   0        0        0     1911 2024-04-26 06:56:36.644489 drf_easily_saas-0.0.3/drf_easily_saas/management/commands/syncfirebaseusers.py
+-rw-r--r--   0        0        0     2210 2024-04-25 08:58:35.026313 drf_easily_saas-0.0.3/drf_easily_saas/migrations/0001_initial.py
+-rw-r--r--   0        0        0      641 2024-04-28 10:24:49.641296 drf_easily_saas-0.0.3/drf_easily_saas/migrations/0002_alter_subscription_options_and_more.py
+-rw-r--r--   0        0        0      485 2024-04-28 10:25:24.197673 drf_easily_saas-0.0.3/drf_easily_saas/migrations/0003_alter_subscription_unique_together.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:37:58.179115 drf_easily_saas-0.0.3/drf_easily_saas/migrations/__init__.py
+-rw-r--r--   0        0        0     1633 2024-04-25 22:13:28.898879 drf_easily_saas-0.0.3/drf_easily_saas/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0        0        0      837 2024-04-28 10:24:55.241357 drf_easily_saas-0.0.3/drf_easily_saas/migrations/__pycache__/0002_alter_subscription_options_and_more.cpython-310.pyc
+-rw-r--r--   0        0        0      729 2024-04-28 10:25:27.237706 drf_easily_saas-0.0.3/drf_easily_saas/migrations/__pycache__/0003_alter_subscription_unique_together.cpython-310.pyc
+-rw-r--r--   0        0        0      187 2024-04-25 22:13:28.894879 drf_easily_saas-0.0.3/drf_easily_saas/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1709 2024-04-29 22:43:04.290561 drf_easily_saas-0.0.3/drf_easily_saas/models.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:46:04.593982 drf_easily_saas-0.0.3/drf_easily_saas/payment/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-25 22:11:12.017278 drf_easily_saas-0.0.3/drf_easily_saas/payment/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6849 2024-04-30 09:05:18.900624 drf_easily_saas-0.0.3/drf_easily_saas/payment/__pycache__/manager.cpython-310.pyc
+-rw-r--r--   0        0        0      722 2024-04-26 06:56:51.576669 drf_easily_saas-0.0.3/drf_easily_saas/payment/__pycache__/serializers.cpython-310.pyc
+-rw-r--r--   0        0        0      462 2024-04-26 10:54:19.396759 drf_easily_saas-0.0.3/drf_easily_saas/payment/__pycache__/urls.cpython-310.pyc
+-rw-r--r--   0        0        0     8728 2024-04-30 09:05:16.884582 drf_easily_saas-0.0.3/drf_easily_saas/payment/manager.py
+-rw-r--r--   0        0        0      263 2024-04-26 06:56:09.160156 drf_easily_saas-0.0.3/drf_easily_saas/payment/serializers.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:17:36.503667 drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-25 22:12:35.430256 drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1380 2024-04-25 22:13:28.850878 drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/__pycache__/serializers.cpython-310.pyc
+-rw-r--r--   0        0        0      565 2024-04-26 09:47:16.601761 drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/__pycache__/urls.cpython-310.pyc
+-rw-r--r--   0        0        0     2771 2024-04-30 09:05:18.896623 drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/__pycache__/views.cpython-310.pyc
+-rw-r--r--   0        0        0     1110 2024-04-25 08:17:36.507667 drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/serializers.py
+-rw-r--r--   0        0        0      671 2024-04-26 09:47:15.905753 drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/urls.py
+-rw-r--r--   0        0        0     3301 2024-04-30 09:05:16.884582 drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/views.py
+-rw-r--r--   0        0        0      289 2024-04-26 10:54:18.688748 drf_easily_saas-0.0.3/drf_easily_saas/payment/urls.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:38:05.814726 drf_easily_saas-0.0.3/drf_easily_saas/schemas/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-26 10:44:26.305922 drf_easily_saas-0.0.3/drf_easily_saas/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3959 2024-04-30 09:05:18.508616 drf_easily_saas-0.0.3/drf_easily_saas/schemas/__pycache__/claims.cpython-310.pyc
+-rw-r--r--   0        0        0     1943 2024-04-28 14:54:43.499699 drf_easily_saas-0.0.3/drf_easily_saas/schemas/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0      542 2024-04-29 22:40:20.097505 drf_easily_saas-0.0.3/drf_easily_saas/schemas/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     2930 2024-04-28 21:47:19.564174 drf_easily_saas-0.0.3/drf_easily_saas/schemas/__pycache__/firebase.cpython-310.pyc
+-rw-r--r--   0        0        0     5626 2024-04-28 21:48:02.868434 drf_easily_saas-0.0.3/drf_easily_saas/schemas/__pycache__/stripe.cpython-310.pyc
+-rw-r--r--   0        0        0      684 2024-04-28 13:15:56.383113 drf_easily_saas-0.0.3/drf_easily_saas/schemas/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     4181 2024-04-30 09:05:16.884582 drf_easily_saas-0.0.3/drf_easily_saas/schemas/claims.py
+-rw-r--r--   0        0        0     2086 2024-04-28 14:54:43.947705 drf_easily_saas-0.0.3/drf_easily_saas/schemas/config.py
+-rw-r--r--   0        0        0      627 2024-04-29 22:40:19.377500 drf_easily_saas-0.0.3/drf_easily_saas/schemas/constants.py
+-rw-r--r--   0        0        0     3534 2024-04-28 21:47:18.360167 drf_easily_saas-0.0.3/drf_easily_saas/schemas/firebase.py
+-rw-r--r--   0        0        0     5796 2024-04-28 21:48:02.052429 drf_easily_saas-0.0.3/drf_easily_saas/schemas/stripe.py
+-rw-r--r--   0        0        0      461 2024-04-28 13:15:55.107103 drf_easily_saas-0.0.3/drf_easily_saas/schemas/utils.py
+-rw-r--r--   0        0        0      808 2024-04-28 21:37:39.605450 drf_easily_saas-0.0.3/drf_easily_saas/settings.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:03:14.529552 drf_easily_saas-0.0.3/drf_easily_saas/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:03:31.689761 drf_easily_saas-0.0.3/drf_easily_saas/tests/user_stories/__init__.py
+-rw-r--r--   0        0        0     2075 2024-04-29 12:28:35.269922 drf_easily_saas-0.0.3/drf_easily_saas/tests/user_stories/test_checkout.py
+-rw-r--r--   0        0        0      265 2024-04-28 16:54:44.524990 drf_easily_saas-0.0.3/drf_easily_saas/urls.py
+-rw-r--r--   0        0        0        0 2024-04-26 07:03:02.729014 drf_easily_saas-0.0.3/drf_easily_saas/utils/__init__.py
+-rw-r--r--   0        0        0      182 2024-04-26 07:48:58.611013 drf_easily_saas-0.0.3/drf_easily_saas/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1503 2024-04-28 13:14:42.470495 drf_easily_saas-0.0.3/drf_easily_saas/utils/__pycache__/db.cpython-310.pyc
+-rw-r--r--   0        0        0      799 2024-04-29 22:56:11.475623 drf_easily_saas-0.0.3/drf_easily_saas/utils/__pycache__/urls.cpython-310.pyc
+-rw-r--r--   0        0        0     1233 2024-04-28 13:14:42.178492 drf_easily_saas-0.0.3/drf_easily_saas/utils/db.py
+-rw-r--r--   0        0        0      525 2024-04-29 22:56:10.443616 drf_easily_saas-0.0.3/drf_easily_saas/utils/urls.py
+-rw-r--r--   0        0        0      872 2024-04-30 09:05:54.397351 drf_easily_saas-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4410 1970-01-01 00:00:00.000000 drf_easily_saas-0.0.3/PKG-INFO
```

### Comparing `drf_easily_saas-0.0.2/README.md` & `drf_easily_saas-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - Upload the `.json` file into your Django project
 
 ## 2. Django configuration
 
 **Install authentication app in your project**
 
 ```bash
-pip install drf-easily-auth
+pip install drf-easily-saas
 ```
 
 ```bash
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
```

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/auth/firebase/protect.py` & `drf_easily_saas-0.0.3/drf_easily_saas/auth/firebase/protect.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/exceptions/base.py` & `drf_easily_saas-0.0.3/drf_easily_saas/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/exceptions/config.py` & `drf_easily_saas-0.0.3/drf_easily_saas/exceptions/config.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/exceptions/stripe.py` & `drf_easily_saas-0.0.3/drf_easily_saas/exceptions/stripe.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/management/commands/syncfirebaseusers.py` & `drf_easily_saas-0.0.3/drf_easily_saas/management/commands/syncfirebaseusers.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/migrations/0001_initial.py` & `drf_easily_saas-0.0.3/drf_easily_saas/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/migrations/0002_alter_subscription_options_and_more.py` & `drf_easily_saas-0.0.3/drf_easily_saas/migrations/0002_alter_subscription_options_and_more.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/models.py` & `drf_easily_saas-0.0.3/drf_easily_saas/models.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/payment/manager.py` & `drf_easily_saas-0.0.3/drf_easily_saas/payment/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from typing import Union, List, Dict, Any
 # Drf Easily Saas
 from drf_easily_saas.settings import AUTH_PROVIDER, PAYMENT_PROVIDER, STRIPE_CONFIG, STRIPE_SUBSCRIPTION_CONFIG, FRONTEND_URL
 
 # Drf Easily Saas exceptions
 from drf_easily_saas.exceptions.stripe import StripePaymentProcessingError
 from drf_easily_saas.schemas.stripe import StripeBaseSubscription
+from drf_easily_saas.schemas.claims import FirebaseClaimsPayment
 
 # User methods and classes
 from drf_easily_saas.models import User, Subscription
-from drf_easily_saas.auth.firebase.state_manager import add_custom_claims
 
 
 # Ici je vais créer une classe qui va gérer les paiements avec Stripe et LemonSqueezy, 
 # aussi elle gérera la synchronisation des utilisateurs avec le provider d'authentification défini dans les settings.
 class PaymentManager:
     def __init__(self):
         self.payment_provider = PAYMENT_PROVIDER
@@ -38,14 +38,15 @@
     # Checkout session
     # -------------------------------------------- #
     def create_checkout_session(self, subscription_schema: dict) -> stripe.checkout.Session:
         """
         Create a checkout session with Stripe.
         """
         try:
+            # Validate the subscription schema for Stripe from define in settings.py in project
             subscription_schema_valid = StripeBaseSubscription(**subscription_schema)
             # Add user informations to metadata if not already present
             session = stripe.checkout.Session.create(**subscription_schema_valid.to_dict())
         except stripe.error.StripeError as e:
             raise StripePaymentProcessingError(str(e))
         return session
         
@@ -122,28 +123,32 @@
 
     def handle_checkout_session_completed(self, event_data) -> Union[Subscription, None]:
         session_ = event_data
         # Mets à jour le profile de l'utilisateur dans Firebase
         uid = session_['metadata']['uid']
         subscription_id = session_['subscription']
 
+        # [Stripe] Add uid in customer metadata
+        customer = self._add_customer_metadata(session_['customer'], {'uid': uid})
+
         # [Stripe] ajoute les metadata à l'abonnement de l'utilisateur dans Stripe
         # Ajoute: uid
         subscription = self._add_subscribtion_meta(subscription_id, {'uid': uid})
 
         # [Firebase] Ajoute les custom claims au user dans Firebase
         # Cela aura pour effet de mettre à jour le token de l'utilisateur et de le deconnecter de toutes ses sessions
-        custom_claims = {   
-                'status': subscription['status'],
-                'subscription_id': subscription_id,
-                'plan_id': subscription['plan']['id'],
-                'customer_id': session_['customer']
-            }
-        if self._add_subscribtion_in_state(uid=uid, claims=custom_claims, subscription=subscription):
-            print('Subscription added to the database')
+        custom_claims = FirebaseClaimsPayment(
+            status=subscription.status,
+            customer_id=customer.id,
+            subscription_id=subscription_id,
+            plan_id=subscription.plan.id,
+            uid=uid
+        )
+
+        if custom_claims.update_state_token(custom_claims, subscription):
             return subscription
         else:
             print('Error adding subscription to the database')
             return None
 
     def handle_checkout_session_expired(self, session):
         print('Payment expired')
@@ -166,57 +171,56 @@
     def handle_customer_subscription_deleted(self, event_data):
         print('Subscription deleted')
         subscription = event_data
 
         # Mets à jour le profile de l'utilisateur dans Firebase
         uid = subscription['metadata']['uid']
         subscription_id = subscription['id']
+        
+        # [Firebase] Ajoute les custom claims au user dans Firebase
+        # Cela aura pour effet de mettre à jour le token de l'utilisateur et de le deconnecter de toutes ses sessions
+        custom_claims = FirebaseClaimsPayment(
+            status=subscription.status,
+            customer_id=subscription.customer,
+            subscription_id=subscription_id,
+            plan_id=subscription.plan.id,
+            uid=uid
+        )
 
-        custom_claims = {   
-                'status': subscription['status'],
-                'subscription_id': subscription_id,
-                'plan_id': subscription['plan']['id'],
-                'customer_id': subscription['customer']
-            }
-        if self._add_subscribtion_in_state(uid=uid, claims=custom_claims, subscription=subscription):
-            print('Subscription added to the database and custom claims added to the user')
+        if custom_claims.update_state_token(custom_claims, subscription):
             return subscription
         else:
-            print('Error adding subscription to the database')
+            print('Error adding subscription to the state')
             return None
 
     # -------------------------------------------- #
     # Private methods
     # -------------------------------------------- #
-
+    # _ Subscription methods
     def _add_subscribtion_meta(self, subscription_id: int , metadata: dict) -> Union[stripe.Subscription, None]:
         subscription = stripe.Subscription.retrieve(subscription_id)
         subscription.metadata = metadata
         subscription.save()
         if subscription.metadata == metadata:
             return subscription
         return None
     
-    def _add_subscribtion_in_state(self, uid: str, claims: dict,  subscription: stripe.Subscription) -> Union[Subscription, None]:
-        # [Django] Ajoute l'abonnement à la base de données
-            user = User.objects.get(username=uid)
-            try:
-                add_custom_claims(uid, claims)
-                sub_table = Subscription.objects.update_or_create(
-                    user=user,
-                    provider='STRIPE',
-                    defaults={
-                        'subscription_id': subscription.id,
-                        'status': subscription.status,
-                        'plan_id': subscription.plan.id,
-                        'customer_id': subscription.customer,
-                    }
-                )
-                if sub_table:
-                    return sub_table
-                return None
-            except Exception as e:
-                print(e)
-                return None
-            
+    def _get_subscribtion_meta(self, subscription_id: int) -> Union[stripe.Subscription, None]:
+        subscription = stripe.Subscription.retrieve(subscription_id)
+        return subscription.metadata
+    
+    # _ Customer methods
+    def _add_customer_metadata(self, customer_id: int, metadata: dict) -> Union[stripe.Customer, None]:
+        customer = stripe.Customer.retrieve(customer_id)
+        customer.metadata = metadata
+        customer.save()
+        if customer.metadata == metadata:
+            return customer
+        return None
+    
+    def _get_customer_metadata(self, customer_id: int) -> Union[stripe.Customer, None]:
+        customer = stripe.Customer.retrieve(customer_id)
+        return customer.metadata
+
+    # _ Utils
     def _normalize_event_type(self, event_type: str) -> str:
         return event_type.replace('.', '_')
```

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/payment/stripe/serializers.py` & `drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/payment/stripe/urls.py` & `drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/urls.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/payment/stripe/views.py` & `drf_easily_saas-0.0.3/drf_easily_saas/payment/stripe/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 # -------------------------------------------- #
 
 # -------------------------------------------- #
 # Checkout
 # -------------------------------------------- #
 class CheckoutView(APIView):
     serializer_class = CheckoutSerializer
-    permission_classes = []
     stripe_manager = StripeManager()
 
     @extend_schema(
         request=CheckoutSerializer,
         responses=CheckoutSessionSerializer
     )
     def post(self, request):
```

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/schemas/config.py` & `drf_easily_saas-0.0.3/drf_easily_saas/schemas/config.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/schemas/constants.py` & `drf_easily_saas-0.0.3/drf_easily_saas/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/schemas/firebase.py` & `drf_easily_saas-0.0.3/drf_easily_saas/schemas/firebase.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/schemas/stripe.py` & `drf_easily_saas-0.0.3/drf_easily_saas/schemas/stripe.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/settings.py` & `drf_easily_saas-0.0.3/drf_easily_saas/settings.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/tests/user_stories/test_checkout.py` & `drf_easily_saas-0.0.3/drf_easily_saas/tests/user_stories/test_checkout.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/utils/db.py` & `drf_easily_saas-0.0.3/drf_easily_saas/utils/db.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/drf_easily_saas/utils/urls.py` & `drf_easily_saas-0.0.3/drf_easily_saas/utils/urls.py`

 * *Files identical despite different names*

### Comparing `drf_easily_saas-0.0.2/pyproject.toml` & `drf_easily_saas-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf_easily_saas"
-version = "0.0.2"
+version = "0.0.3"
 description = "This package is complete tools for sass building"
 authors = ["Alexandre Meline <alexandre.meline.dev@gmail.com>"]
 readme = "README.md"
 keywords = [
     "Django",
     "Firebase",
     "Authentication",
```

### Comparing `drf_easily_saas-0.0.2/PKG-INFO` & `drf_easily_saas-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_easily_saas
-Version: 0.0.2
+Version: 0.0.3
 Summary: This package is complete tools for sass building
 Home-page: https://github.com/alexandre-meline/drf_easily_sass/
 Keywords: Django,Firebase,Authentication,User Synchronization,DRF,Python,User Management,Security,API,JSON Web Tokens,Payment,Stripe
 Author: Alexandre Meline
 Author-email: alexandre.meline.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 - Upload the `.json` file into your Django project
 
 ## 2. Django configuration
 
 **Install authentication app in your project**
 
 ```bash
-pip install drf-easily-auth
+pip install drf-easily-saas
 ```
 
 ```bash
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
```

