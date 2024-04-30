# Comparing `tmp/django-paypal-2.0.tar.gz` & `tmp/django-paypal-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-paypal-2.0.tar", last modified: Fri Mar 25 21:26:18 2022, max compression
+gzip compressed data, was "django-paypal-2.1.tar", last modified: Tue Apr 30 19:52:33 2024, max compression
```

## Comparing `django-paypal-2.0.tar` & `django-paypal-2.1.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.469428 django-paypal-2.0/
--rw-r--r--   0 luke      (1000) luke      (1000)     1249 2022-03-25 21:23:33.000000 django-paypal-2.0/.pre-commit-config.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)     3400 2021-03-14 19:33:19.000000 django-paypal-2.0/CONTRIBUTING.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      220 2017-12-05 16:49:26.000000 django-paypal-2.0/CONTRIBUTORS.md
--rw-r--r--   0 luke      (1000) luke      (1000)     1063 2014-10-07 10:10:31.000000 django-paypal-2.0/LICENSE
--rw-r--r--   0 luke      (1000) luke      (1000)      379 2022-03-25 21:23:33.000000 django-paypal-2.0/MANIFEST.in
--rw-rw-rw-   0 luke      (1000) luke      (1000)     1266 2022-03-25 21:26:18.469428 django-paypal-2.0/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)     3213 2022-03-23 12:34:27.000000 django-paypal-2.0/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      580 2021-03-14 19:33:19.000000 django-paypal-2.0/RELEASE.rst
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.453428 django-paypal-2.0/django_paypal.egg-info/
--rw-r--r--   0 luke      (1000) luke      (1000)     1266 2022-03-25 21:26:18.000000 django-paypal-2.0/django_paypal.egg-info/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)     4178 2022-03-25 21:26:18.000000 django-paypal-2.0/django_paypal.egg-info/SOURCES.txt
--rw-r--r--   0 luke      (1000) luke      (1000)        1 2022-03-25 21:26:18.000000 django-paypal-2.0/django_paypal.egg-info/dependency_links.txt
--rw-r--r--   0 luke      (1000) luke      (1000)       41 2022-03-25 21:26:18.000000 django-paypal-2.0/django_paypal.egg-info/requires.txt
--rw-r--r--   0 luke      (1000) luke      (1000)        7 2022-03-25 21:26:18.000000 django-paypal-2.0/django_paypal.egg-info/top_level.txt
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.457428 django-paypal-2.0/docs/
--rw-r--r--   0 luke      (1000) luke      (1000)     5540 2016-09-09 08:36:11.000000 django-paypal-2.0/docs/Makefile
--rw-r--r--   0 luke      (1000) luke      (1000)     7693 2022-03-25 21:24:34.000000 django-paypal-2.0/docs/conf.py
--rw-r--r--   0 luke      (1000) luke      (1000)      553 2017-08-15 06:38:19.000000 django-paypal-2.0/docs/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1264 2018-11-28 07:05:03.000000 django-paypal-2.0/docs/install.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     5084 2016-09-09 08:36:11.000000 django-paypal-2.0/docs/make.bat
--rw-r--r--   0 luke      (1000) luke      (1000)     2023 2016-09-09 08:36:11.000000 django-paypal-2.0/docs/overview.rst
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.457428 django-paypal-2.0/docs/pro/
--rw-r--r--   0 luke      (1000) luke      (1000)     5711 2016-09-09 08:36:11.000000 django-paypal-2.0/docs/pro/detail.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     4093 2021-03-14 19:33:19.000000 django-paypal-2.0/docs/pro/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)    13239 2022-03-25 21:23:57.000000 django-paypal-2.0/docs/release_notes.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      500 2017-08-15 13:52:59.000000 django-paypal-2.0/docs/settings.rst
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.457428 django-paypal-2.0/docs/standard/
--rw-r--r--   0 luke      (1000) luke      (1000)     3832 2018-11-28 07:02:09.000000 django-paypal-2.0/docs/standard/encrypted_buttons.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      146 2016-09-09 08:36:11.000000 django-paypal-2.0/docs/standard/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     8562 2021-03-14 19:34:43.000000 django-paypal-2.0/docs/standard/ipn.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     3150 2021-03-14 19:33:19.000000 django-paypal-2.0/docs/standard/pdt.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1350 2021-03-14 18:08:06.000000 django-paypal-2.0/docs/standard/subscriptions.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1263 2021-03-14 18:08:06.000000 django-paypal-2.0/docs/standard/variables.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      950 2021-03-14 19:33:19.000000 django-paypal-2.0/docs/tests.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      371 2018-11-28 07:17:19.000000 django-paypal-2.0/docs/updatedb.rst
--rwxr-xr--   0 luke      (1000) luke      (1000)      964 2022-03-25 21:23:33.000000 django-paypal-2.0/manage.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.457428 django-paypal-2.0/paypal/
--rw-r--r--   0 luke      (1000) luke      (1000)       20 2022-03-25 21:24:15.000000 django-paypal-2.0/paypal/__init__.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.457428 django-paypal-2.0/paypal/pro/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2012-06-09 14:04:37.000000 django-paypal-2.0/paypal/pro/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)      397 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/admin.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2398 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/creditcard.py
--rw-r--r--   0 luke      (1000) luke      (1000)      203 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/exceptions.py
--rw-r--r--   0 luke      (1000) luke      (1000)    10898 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/fields.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2178 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/forms.py
--rw-r--r--   0 luke      (1000) luke      (1000)    12362 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/helpers.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.461428 django-paypal-2.0/paypal/pro/migrations/
--rw-r--r--   0 luke      (1000) luke      (1000)     3573 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/migrations/0001_initial.py
--rw-r--r--   0 luke      (1000) luke      (1000)      348 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/migrations/0002_auto_20141117_1647.py
--rw-r--r--   0 luke      (1000) luke      (1000)      398 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/migrations/0003_auto_20181128_1032.py
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2014-12-11 14:45:04.000000 django-paypal-2.0/paypal/pro/migrations/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5574 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/models.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.453428 django-paypal-2.0/paypal/pro/templates/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.461428 django-paypal-2.0/paypal/pro/templates/pro/
--rw-r--r--   0 luke      (1000) luke      (1000)      279 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/templates/pro/confirm.html
--rw-r--r--   0 luke      (1000) luke      (1000)      536 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/templates/pro/payment.html
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.461428 django-paypal-2.0/paypal/pro/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2018-11-28 07:02:09.000000 django-paypal-2.0/paypal/pro/tests/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)      745 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/tests/settings.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.461428 django-paypal-2.0/paypal/pro/tests/templates/
--rw-r--r--   0 luke      (1000) luke      (1000)      172 2016-09-09 08:36:11.000000 django-paypal-2.0/paypal/pro/tests/templates/confirmation.html
--rw-r--r--   0 luke      (1000) luke      (1000)      118 2016-09-09 08:36:11.000000 django-paypal-2.0/paypal/pro/tests/templates/payment.html
--rw-r--r--   0 luke      (1000) luke      (1000)     1833 2018-03-06 11:13:27.000000 django-paypal-2.0/paypal/pro/tests/test_doDirectPayment_authenticated_user.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)     1988 2016-10-06 11:57:10.000000 django-paypal-2.0/paypal/pro/tests/test_doDirectPayment_invalid.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)     1833 2016-10-06 11:57:18.000000 django-paypal-2.0/paypal/pro/tests/test_doDirectPayment_valid.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)     1833 2016-10-06 11:57:26.000000 django-paypal-2.0/paypal/pro/tests/test_doDirectPayment_valid_with_signal.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)     1565 2016-10-06 12:07:24.000000 django-paypal-2.0/paypal/pro/tests/test_get_redirect.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)    12023 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/tests/test_pro.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1616 2016-10-06 11:57:27.000000 django-paypal-2.0/paypal/pro/tests/test_setExpressCheckout.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)     1694 2016-10-06 12:07:25.000000 django-paypal-2.0/paypal/pro/tests/test_validate_confirm_form_error.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)     8415 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/pro/views.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.461428 django-paypal-2.0/paypal/standard/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2012-06-09 14:04:37.000000 django-paypal-2.0/paypal/standard/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1141 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/conf.py
--rw-r--r--   0 luke      (1000) luke      (1000)    11573 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/forms.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2778 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/helpers.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.465428 django-paypal-2.0/paypal/standard/ipn/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2012-06-09 14:04:37.000000 django-paypal-2.0/paypal/standard/ipn/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5049 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/admin.py
--rw-r--r--   0 luke      (1000) luke      (1000)      415 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/forms.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.465428 django-paypal-2.0/paypal/standard/ipn/migrations/
--rw-r--r--   0 luke      (1000) luke      (1000)    17161 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/migrations/0001_initial.py
--rw-r--r--   0 luke      (1000) luke      (1000)      381 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/migrations/0002_paypalipn_mp_id.py
--rw-r--r--   0 luke      (1000) luke      (1000)      356 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/migrations/0003_auto_20141117_1647.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5053 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/migrations/0004_auto_20150612_1826.py
--rw-r--r--   0 luke      (1000) luke      (1000)      531 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/migrations/0005_auto_20151217_0948.py
--rw-r--r--   0 luke      (1000) luke      (1000)      536 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/migrations/0006_auto_20160108_1112.py
--rw-r--r--   0 luke      (1000) luke      (1000)      896 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/migrations/0007_auto_20160219_1135.py
--rw-r--r--   0 luke      (1000) luke      (1000)      571 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/migrations/0008_auto_20181128_1032.py
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2014-10-03 14:10:18.000000 django-paypal-2.0/paypal/standard/ipn/migrations/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1123 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/models.py
--rw-r--r--   0 luke      (1000) luke      (1000)      516 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/signals.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.453428 django-paypal-2.0/paypal/standard/ipn/templates/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.465428 django-paypal-2.0/paypal/standard/ipn/templates/ipn/
--rw-r--r--   0 luke      (1000) luke      (1000)      287 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/templates/ipn/ipn.html
--rw-r--r--   0 luke      (1000) luke      (1000)     2171 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/templates/ipn/ipn_test.html
--rw-r--r--   0 luke      (1000) luke      (1000)       91 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/templates/ipn/paypal.html
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.465428 django-paypal-2.0/paypal/standard/ipn/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2018-11-28 07:02:09.000000 django-paypal-2.0/paypal/standard/ipn/tests/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1835 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/tests/test_admin.py
--rw-r--r--   0 luke      (1000) luke      (1000)      887 2018-11-28 07:02:09.000000 django-paypal-2.0/paypal/standard/ipn/tests/test_cert__do_not_use__private.pem
--rw-r--r--   0 luke      (1000) luke      (1000)      607 2018-11-28 07:02:09.000000 django-paypal-2.0/paypal/standard/ipn/tests/test_cert__do_not_use__public.pem
--rw-r--r--   0 luke      (1000) luke      (1000)     1334 2018-11-28 07:02:09.000000 django-paypal-2.0/paypal/standard/ipn/tests/test_cert_from_paypal__do_not_use.pem
--rw-r--r--   0 luke      (1000) luke      (1000)     6002 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/tests/test_forms.py
--rw-r--r--   0 luke      (1000) luke      (1000)    18201 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/tests/test_ipn.py
--rw-r--r--   0 luke      (1000) luke      (1000)      278 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/tests/test_urls.py
--rw-r--r--   0 luke      (1000) luke      (1000)      217 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/urls.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3814 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/ipn/views.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.465428 django-paypal-2.0/paypal/standard/migrations/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2014-10-07 10:14:36.000000 django-paypal-2.0/paypal/standard/migrations/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)    18939 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/models.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.465428 django-paypal-2.0/paypal/standard/pdt/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2012-06-09 14:04:37.000000 django-paypal-2.0/paypal/standard/pdt/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4085 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/admin.py
--rw-r--r--   0 luke      (1000) luke      (1000)      462 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/forms.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.469428 django-paypal-2.0/paypal/standard/pdt/migrations/
--rw-r--r--   0 luke      (1000) luke      (1000)    17756 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/migrations/0001_initial.py
--rw-r--r--   0 luke      (1000) luke      (1000)      381 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/migrations/0002_paypalpdt_mp_id.py
--rw-r--r--   0 luke      (1000) luke      (1000)      356 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/migrations/0003_auto_20141117_1647.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5053 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/migrations/0004_auto_20151029_1515.py
--rw-r--r--   0 luke      (1000) luke      (1000)      531 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/migrations/0005_auto_20151217_0948.py
--rw-r--r--   0 luke      (1000) luke      (1000)      536 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/migrations/0006_auto_20160108_1112.py
--rw-r--r--   0 luke      (1000) luke      (1000)      896 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/migrations/0007_auto_20160219_1137.py
--rw-r--r--   0 luke      (1000) luke      (1000)      571 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/migrations/0008_auto_20181128_1032.py
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2014-10-03 14:10:39.000000 django-paypal-2.0/paypal/standard/pdt/migrations/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3194 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/models.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.469428 django-paypal-2.0/paypal/standard/pdt/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2018-11-28 07:02:09.000000 django-paypal-2.0/paypal/standard/pdt/tests/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)      745 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/tests/settings.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.469428 django-paypal-2.0/paypal/standard/pdt/tests/templates/
--rw-r--r--   0 luke      (1000) luke      (1000)      122 2016-09-09 08:36:11.000000 django-paypal-2.0/paypal/standard/pdt/tests/templates/base.html
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2022-03-25 21:26:18.469428 django-paypal-2.0/paypal/standard/pdt/tests/templates/pdt/
--rwxr-xr--   0 luke      (1000) luke      (1000)      768 2016-09-09 08:36:11.000000 django-paypal-2.0/paypal/standard/pdt/tests/templates/pdt/pdt.html
--rw-r--r--   0 luke      (1000) luke      (1000)      738 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/tests/templates/pdt/test_pdt_response.html
--rw-r--r--   0 luke      (1000) luke      (1000)     5766 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/tests/test_pdt.py
--rw-r--r--   0 luke      (1000) luke      (1000)      714 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/tests/test_urls.py
--rw-r--r--   0 luke      (1000) luke      (1000)      217 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/urls.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1884 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/pdt/views.py
--rw-r--r--   0 luke      (1000) luke      (1000)      414 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/standard/widgets.py
--rw-r--r--   0 luke      (1000) luke      (1000)      543 2022-03-25 21:23:33.000000 django-paypal-2.0/paypal/utils.py
--rw-r--r--   0 luke      (1000) luke      (1000)      418 2022-03-25 21:23:33.000000 django-paypal-2.0/pyproject.toml
--rwxr-xr--   0 luke      (1000) luke      (1000)      326 2022-03-25 21:26:06.000000 django-paypal-2.0/release.sh
--rw-r--r--   0 luke      (1000) luke      (1000)       48 2021-12-13 21:44:06.000000 django-paypal-2.0/requirements-dev.txt
--rw-r--r--   0 luke      (1000) luke      (1000)      265 2022-03-23 12:34:27.000000 django-paypal-2.0/requirements-test.txt
--rwxr-xr--   0 luke      (1000) luke      (1000)     3638 2022-03-25 21:23:33.000000 django-paypal-2.0/runtests.py
--rw-r--r--   0 luke      (1000) luke      (1000)      168 2022-03-25 21:26:18.469428 django-paypal-2.0/setup.cfg
--rwxr-xr--   0 luke      (1000) luke      (1000)     1578 2022-03-25 21:24:24.000000 django-paypal-2.0/setup.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1116 2022-03-23 12:34:27.000000 django-paypal-2.0/tox.ini
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.867733 django-paypal-2.1/
+-rw-r--r--   0 luke      (1000) luke      (1000)      535 2024-04-30 19:48:34.000000 django-paypal-2.1/.pre-commit-config.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)     3436 2024-04-30 19:48:34.000000 django-paypal-2.1/CONTRIBUTING.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      220 2017-12-05 16:49:26.000000 django-paypal-2.1/CONTRIBUTORS.md
+-rw-r--r--   0 luke      (1000) luke      (1000)     1063 2014-10-07 10:10:31.000000 django-paypal-2.1/LICENSE
+-rw-r--r--   0 luke      (1000) luke      (1000)      379 2022-03-25 21:23:33.000000 django-paypal-2.1/MANIFEST.in
+-rw-r--r--   0 luke      (1000) luke      (1000)     1265 2024-04-30 19:52:33.867733 django-paypal-2.1/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)     3400 2024-04-30 19:30:27.000000 django-paypal-2.1/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      580 2021-03-14 19:33:19.000000 django-paypal-2.1/RELEASE.rst
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.867733 django-paypal-2.1/django_paypal.egg-info/
+-rw-r--r--   0 luke      (1000) luke      (1000)     1265 2024-04-30 19:52:33.000000 django-paypal-2.1/django_paypal.egg-info/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)     4178 2024-04-30 19:52:33.000000 django-paypal-2.1/django_paypal.egg-info/SOURCES.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)        1 2024-04-30 19:52:33.000000 django-paypal-2.1/django_paypal.egg-info/dependency_links.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)       41 2024-04-30 19:52:33.000000 django-paypal-2.1/django_paypal.egg-info/requires.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)        7 2024-04-30 19:52:33.000000 django-paypal-2.1/django_paypal.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.851733 django-paypal-2.1/docs/
+-rw-r--r--   0 luke      (1000) luke      (1000)     5540 2016-09-09 08:36:11.000000 django-paypal-2.1/docs/Makefile
+-rw-r--r--   0 luke      (1000) luke      (1000)     7693 2024-04-30 19:48:34.000000 django-paypal-2.1/docs/conf.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      553 2017-08-15 06:38:19.000000 django-paypal-2.1/docs/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1270 2024-04-30 19:48:34.000000 django-paypal-2.1/docs/install.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     5084 2016-09-09 08:36:11.000000 django-paypal-2.1/docs/make.bat
+-rw-r--r--   0 luke      (1000) luke      (1000)     2023 2016-09-09 08:36:11.000000 django-paypal-2.1/docs/overview.rst
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.851733 django-paypal-2.1/docs/pro/
+-rw-r--r--   0 luke      (1000) luke      (1000)     5711 2016-09-09 08:36:11.000000 django-paypal-2.1/docs/pro/detail.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     4093 2021-03-14 19:33:19.000000 django-paypal-2.1/docs/pro/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)    13508 2024-04-30 19:48:34.000000 django-paypal-2.1/docs/release_notes.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      502 2024-04-30 19:48:50.000000 django-paypal-2.1/docs/settings.rst
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.851733 django-paypal-2.1/docs/standard/
+-rw-r--r--   0 luke      (1000) luke      (1000)     3832 2018-11-28 07:02:09.000000 django-paypal-2.1/docs/standard/encrypted_buttons.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      146 2016-09-09 08:36:11.000000 django-paypal-2.1/docs/standard/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     8993 2024-02-10 20:03:32.000000 django-paypal-2.1/docs/standard/ipn.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     3150 2021-03-14 19:33:19.000000 django-paypal-2.1/docs/standard/pdt.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1350 2021-03-14 18:08:06.000000 django-paypal-2.1/docs/standard/subscriptions.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1263 2021-03-14 18:08:06.000000 django-paypal-2.1/docs/standard/variables.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      950 2021-03-14 19:33:19.000000 django-paypal-2.1/docs/tests.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      371 2018-11-28 07:17:19.000000 django-paypal-2.1/docs/updatedb.rst
+-rwxr-xr--   0 luke      (1000) luke      (1000)      964 2022-03-25 21:23:33.000000 django-paypal-2.1/manage.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.851733 django-paypal-2.1/paypal/
+-rw-r--r--   0 luke      (1000) luke      (1000)       20 2024-04-30 19:48:34.000000 django-paypal-2.1/paypal/__init__.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.855733 django-paypal-2.1/paypal/pro/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2012-06-09 14:04:37.000000 django-paypal-2.1/paypal/pro/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      397 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/admin.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2398 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/creditcard.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      203 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/exceptions.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    10898 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/fields.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2178 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/forms.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    12371 2024-04-30 19:48:34.000000 django-paypal-2.1/paypal/pro/helpers.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.855733 django-paypal-2.1/paypal/pro/migrations/
+-rw-r--r--   0 luke      (1000) luke      (1000)     3573 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/migrations/0001_initial.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      348 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/migrations/0002_auto_20141117_1647.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      398 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/migrations/0003_auto_20181128_1032.py
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2014-12-11 14:45:04.000000 django-paypal-2.1/paypal/pro/migrations/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5574 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/models.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.843733 django-paypal-2.1/paypal/pro/templates/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.855733 django-paypal-2.1/paypal/pro/templates/pro/
+-rw-r--r--   0 luke      (1000) luke      (1000)      279 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/templates/pro/confirm.html
+-rw-r--r--   0 luke      (1000) luke      (1000)      536 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/templates/pro/payment.html
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.859733 django-paypal-2.1/paypal/pro/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2018-11-28 07:02:09.000000 django-paypal-2.1/paypal/pro/tests/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      745 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/tests/settings.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.859733 django-paypal-2.1/paypal/pro/tests/templates/
+-rw-r--r--   0 luke      (1000) luke      (1000)      172 2016-09-09 08:36:11.000000 django-paypal-2.1/paypal/pro/tests/templates/confirmation.html
+-rw-r--r--   0 luke      (1000) luke      (1000)      118 2016-09-09 08:36:11.000000 django-paypal-2.1/paypal/pro/tests/templates/payment.html
+-rw-r--r--   0 luke      (1000) luke      (1000)     1833 2018-03-06 11:13:27.000000 django-paypal-2.1/paypal/pro/tests/test_doDirectPayment_authenticated_user.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)     1988 2016-10-06 11:57:10.000000 django-paypal-2.1/paypal/pro/tests/test_doDirectPayment_invalid.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)     1833 2016-10-06 11:57:18.000000 django-paypal-2.1/paypal/pro/tests/test_doDirectPayment_valid.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)     1833 2016-10-06 11:57:26.000000 django-paypal-2.1/paypal/pro/tests/test_doDirectPayment_valid_with_signal.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)     1565 2016-10-06 12:07:24.000000 django-paypal-2.1/paypal/pro/tests/test_get_redirect.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)    12023 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/tests/test_pro.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1616 2016-10-06 11:57:27.000000 django-paypal-2.1/paypal/pro/tests/test_setExpressCheckout.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)     1694 2016-10-06 12:07:25.000000 django-paypal-2.1/paypal/pro/tests/test_validate_confirm_form_error.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)     8415 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/pro/views.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.859733 django-paypal-2.1/paypal/standard/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2012-06-09 14:04:37.000000 django-paypal-2.1/paypal/standard/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1278 2024-02-10 20:03:32.000000 django-paypal-2.1/paypal/standard/conf.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    11557 2024-04-30 19:48:34.000000 django-paypal-2.1/paypal/standard/forms.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2778 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/helpers.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.859733 django-paypal-2.1/paypal/standard/ipn/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2012-06-09 14:04:37.000000 django-paypal-2.1/paypal/standard/ipn/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5049 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/admin.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      415 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/forms.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.863733 django-paypal-2.1/paypal/standard/ipn/migrations/
+-rw-r--r--   0 luke      (1000) luke      (1000)    17161 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/migrations/0001_initial.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      381 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/migrations/0002_paypalipn_mp_id.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      356 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/migrations/0003_auto_20141117_1647.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5053 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/migrations/0004_auto_20150612_1826.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      531 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/migrations/0005_auto_20151217_0948.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      536 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/migrations/0006_auto_20160108_1112.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      896 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/migrations/0007_auto_20160219_1135.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      571 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/migrations/0008_auto_20181128_1032.py
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2014-10-03 14:10:18.000000 django-paypal-2.1/paypal/standard/ipn/migrations/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1123 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/models.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      516 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/signals.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.843733 django-paypal-2.1/paypal/standard/ipn/templates/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.863733 django-paypal-2.1/paypal/standard/ipn/templates/ipn/
+-rw-r--r--   0 luke      (1000) luke      (1000)      287 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/templates/ipn/ipn.html
+-rw-r--r--   0 luke      (1000) luke      (1000)     2171 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/templates/ipn/ipn_test.html
+-rw-r--r--   0 luke      (1000) luke      (1000)       91 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/templates/ipn/paypal.html
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.863733 django-paypal-2.1/paypal/standard/ipn/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2018-11-28 07:02:09.000000 django-paypal-2.1/paypal/standard/ipn/tests/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1835 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/tests/test_admin.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      887 2018-11-28 07:02:09.000000 django-paypal-2.1/paypal/standard/ipn/tests/test_cert__do_not_use__private.pem
+-rw-r--r--   0 luke      (1000) luke      (1000)      607 2018-11-28 07:02:09.000000 django-paypal-2.1/paypal/standard/ipn/tests/test_cert__do_not_use__public.pem
+-rw-r--r--   0 luke      (1000) luke      (1000)     1334 2018-11-28 07:02:09.000000 django-paypal-2.1/paypal/standard/ipn/tests/test_cert_from_paypal__do_not_use.pem
+-rw-r--r--   0 luke      (1000) luke      (1000)     6002 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/tests/test_forms.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    18176 2024-04-30 19:48:34.000000 django-paypal-2.1/paypal/standard/ipn/tests/test_ipn.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      278 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/tests/test_urls.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      217 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/urls.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3814 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/ipn/views.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.863733 django-paypal-2.1/paypal/standard/migrations/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2014-10-07 10:14:36.000000 django-paypal-2.1/paypal/standard/migrations/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    18939 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/models.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.863733 django-paypal-2.1/paypal/standard/pdt/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2012-06-09 14:04:37.000000 django-paypal-2.1/paypal/standard/pdt/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4085 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/admin.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      462 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/forms.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.867733 django-paypal-2.1/paypal/standard/pdt/migrations/
+-rw-r--r--   0 luke      (1000) luke      (1000)    17756 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/migrations/0001_initial.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      381 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/migrations/0002_paypalpdt_mp_id.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      356 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/migrations/0003_auto_20141117_1647.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5053 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/migrations/0004_auto_20151029_1515.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      531 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/migrations/0005_auto_20151217_0948.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      536 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/migrations/0006_auto_20160108_1112.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      896 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/migrations/0007_auto_20160219_1137.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      571 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/migrations/0008_auto_20181128_1032.py
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2014-10-03 14:10:39.000000 django-paypal-2.1/paypal/standard/pdt/migrations/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3194 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/models.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.867733 django-paypal-2.1/paypal/standard/pdt/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2018-11-28 07:02:09.000000 django-paypal-2.1/paypal/standard/pdt/tests/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      745 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/tests/settings.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.867733 django-paypal-2.1/paypal/standard/pdt/tests/templates/
+-rw-r--r--   0 luke      (1000) luke      (1000)      122 2016-09-09 08:36:11.000000 django-paypal-2.1/paypal/standard/pdt/tests/templates/base.html
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-30 19:52:33.867733 django-paypal-2.1/paypal/standard/pdt/tests/templates/pdt/
+-rwxr-xr--   0 luke      (1000) luke      (1000)      768 2016-09-09 08:36:11.000000 django-paypal-2.1/paypal/standard/pdt/tests/templates/pdt/pdt.html
+-rw-r--r--   0 luke      (1000) luke      (1000)      738 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/tests/templates/pdt/test_pdt_response.html
+-rw-r--r--   0 luke      (1000) luke      (1000)     5766 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/tests/test_pdt.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      714 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/tests/test_urls.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      217 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/urls.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1884 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/pdt/views.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      414 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/standard/widgets.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      543 2022-03-25 21:23:33.000000 django-paypal-2.1/paypal/utils.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      621 2024-04-30 19:48:34.000000 django-paypal-2.1/pyproject.toml
+-rwxr-xr--   0 luke      (1000) luke      (1000)      326 2022-03-25 21:26:06.000000 django-paypal-2.1/release.sh
+-rw-r--r--   0 luke      (1000) luke      (1000)       30 2024-04-30 19:48:34.000000 django-paypal-2.1/requirements-dev.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)      265 2022-03-23 12:34:27.000000 django-paypal-2.1/requirements-test.txt
+-rwxr-xr--   0 luke      (1000) luke      (1000)     3638 2022-03-25 21:23:33.000000 django-paypal-2.1/runtests.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       38 2024-04-30 19:52:33.867733 django-paypal-2.1/setup.cfg
+-rwxr-xr--   0 luke      (1000) luke      (1000)     1529 2024-04-30 19:48:34.000000 django-paypal-2.1/setup.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      888 2024-04-30 19:48:34.000000 django-paypal-2.1/tox.ini
```

### Comparing `django-paypal-2.0/CONTRIBUTING.rst` & `django-paypal-2.1/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 
 2. Create a virtualenv, using one of the supported versions of Python.
 
 3. Run ``python setup.py develop``
 
 4. Install development tools::
 
-     pip install tox isort flake8
+     pip install -r requirements-test.txt -r requirements-dev.txt
 
-5. Recommended: Install `pre-commit <https://pre-commit.com/>`_ and set up
+5. Strongly recommended: Install `pre-commit <https://pre-commit.com/>`_ and set up
    the hooks::
 
        pre-commit install
 
-   This will run flake8/isort automatically when you commit.
+   This will run linters automatically when you commit.
 
 Code quality
 ~~~~~~~~~~~~
 
 **isort** keeps imports in order. Run **tox -e isort-check** to check your
 imports, and **isort <PATHPATH>** to fix them. Use **# isort:skip** to
 get imports to be ignored by isort.
```

### Comparing `django-paypal-2.0/LICENSE` & `django-paypal-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/PKG-INFO` & `django-paypal-2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: django-paypal
-Version: 2.0
+Version: 2.1
 Summary: A pluggable Django application for integrating PayPal Payments Standard or Payments Pro
 Home-page: https://github.com/spookylukey/django-paypal
 Author: John Boxall
 Author-email: john@handimobility.ca
 Maintainer: Luke Plant
 Maintainer-email: L.Plant.98@cantab.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
+Requires-Dist: Django>=2.2
+Requires-Dist: requests>=2.5.3
+Requires-Dist: pytz>=2015.4
 
 A pluggable Django application for integrating PayPal Payments Standard or Payments Pro
 
 Home page: https://github.com/spookylukey/django-paypal
 
 Docs: https://django-paypal.readthedocs.org
-
-
```

### Comparing `django-paypal-2.0/README.rst` & `django-paypal-2.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 .. image:: https://badge.fury.io/py/django-paypal.svg
     :target: https://badge.fury.io/py/django-paypal
     :alt: Latest PyPI version
 
 Django PayPal is a pluggable application that integrates with PayPal Payments
 Standard and Payments Pro.
 
+Note that these are now very old payment methods that are increasingly badly
+supported by PayPal, and django-paypal does not have support for any payment
+methods using their newer APIs.
+
 See https://django-paypal.readthedocs.org/ for documentation.
 
 django-paypal supports:
 
 * Django 2.2 and later
 * Python 3.6 and later
```

### Comparing `django-paypal-2.0/RELEASE.rst` & `django-paypal-2.1/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/django_paypal.egg-info/PKG-INFO` & `django-paypal-2.1/django_paypal.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: django-paypal
-Version: 2.0
+Version: 2.1
 Summary: A pluggable Django application for integrating PayPal Payments Standard or Payments Pro
 Home-page: https://github.com/spookylukey/django-paypal
 Author: John Boxall
 Author-email: john@handimobility.ca
 Maintainer: Luke Plant
 Maintainer-email: L.Plant.98@cantab.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
+Requires-Dist: Django>=2.2
+Requires-Dist: requests>=2.5.3
+Requires-Dist: pytz>=2015.4
 
 A pluggable Django application for integrating PayPal Payments Standard or Payments Pro
 
 Home page: https://github.com/spookylukey/django-paypal
 
 Docs: https://django-paypal.readthedocs.org
-
-
```

### Comparing `django-paypal-2.0/django_paypal.egg-info/SOURCES.txt` & `django-paypal-2.1/django_paypal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/Makefile` & `django-paypal-2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/conf.py` & `django-paypal-2.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 copyright = "2014"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "2.0"
+version = "2.1"
 # The full version, including alpha/beta/rc tags.
-release = "2.0"
+release = "2.1"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `django-paypal-2.0/docs/index.rst` & `django-paypal-2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/install.rst` & `django-paypal-2.1/docs/install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Install into a virtualenv using pip::
 
     pip install django-paypal
 
 
 Or using the latest version from GitHub::
 
-    pip install git://github.com/spookylukey/django-paypal.git#egg=django-paypal
+    pip install git+https://github.com/spookylukey/django-paypal.git#egg=django-paypal
 
 If you are using Django < 1.11, you should use django-paypal 0.5.x and refer to
 its documentation.
 
 You will also need to edit your ``settings.py``, but the specifics depend on
 whether you are using IPN/PDT/Pro.
```

### Comparing `django-paypal-2.0/docs/make.bat` & `django-paypal-2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/overview.rst` & `django-paypal-2.1/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/pro/detail.rst` & `django-paypal-2.1/docs/pro/detail.rst`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/pro/index.rst` & `django-paypal-2.1/docs/pro/index.rst`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/release_notes.rst` & `django-paypal-2.1/docs/release_notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 ===============
  Release notes
 ===============
 
+Version 2.1 (2024-04-30)
+------------------------
+* Added easier method to customise the submit button via
+  ``get_html_submit_element``, thanks @fabiocaccamo
+* Added pay now button #266, thanks @ohidurbappy
+* Dropped support for Python 3.6
+* Fixed Django 5.0 support
+
 Version 2.0 (2022-03-25)
 ------------------------
 
 * Better fix for Django 4.0 form rendering, enabling custom subclasses to work.
 * Dropped support for old Python versions (< 3.6) and old Django versions (< 2.2)
 
 Version 1.1.2 (2021-12-13)
```

### Comparing `django-paypal-2.0/docs/standard/encrypted_buttons.rst` & `django-paypal-2.1/docs/standard/encrypted_buttons.rst`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/standard/ipn.rst` & `django-paypal-2.1/docs/standard/ipn.rst`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
    which sends all the data to PayPal. You simply need to call ``render``
    on the instance in your template to write out the HTML, which includes
    the ``<form>`` tag with the correct endpoint.
 
    ``views.py``:
 
    .. code-block:: python
+
        from django.urls import reverse
        from django.shortcuts import render
        from paypal.standard.forms import PayPalPaymentsForm
 
        def view_that_asks_for_money(request):
 
            # What you want the button to do.
@@ -64,15 +65,15 @@
            # Create the instance.
            form = PayPalPaymentsForm(initial=paypal_dict)
            context = {"form": form}
            return render(request, "payment.html", context)
 
 
    For a full list of variables that can be used in ``paypal_dict``, see
-   `PayPal HTML variables documentation <https://developer.paypal.com/webapps/developer/docs/classic/paypal-payments-standard/integration-guide/Appx_websitestandard_htmlvariables/>`_.
+   `PayPal HTML variables documentation <https://developer.paypal.com/api/nvp-soap/paypal-payments-standard/integration-guide/Appx-websitestandard-htmlvariables/>`_.
 
    .. note:: The names of these variables are not the same as the values
              returned on the IPN object.
 
    ``payment.html``:
 
    .. code-block:: html
@@ -82,14 +83,26 @@
        <!-- writes out the form tag automatically -->
        {{ form.render }}
 
    The image used for the button can be customized using the :doc:`/settings`, or
    by subclassing ``PayPalPaymentsForm`` and overriding the ``get_image``
    method.
 
+   **Submit button customisation**
+   The submit button used by the form is the standard PayPal payment button, but it's possible to customise it extending the form:
+
+   .. code-block:: python
+
+       from paypal.standard.forms import PayPalPaymentsForm
+
+       class CustomPayPalPaymentsForm(PayPalPaymentsForm):
+
+           def get_html_submit_element(self):
+               return """<button type="submit">Continue on PayPal website</button>"""
+
 4. When someone uses this button to buy something PayPal makes a HTTP POST to
    your "notify_url". PayPal calls this Instant Payment Notification (IPN).
    The view ``paypal.standard.ipn.views.ipn`` handles IPN processing. To set the
    correct ``notify_url`` add the following to your ``urls.py``:
 
    .. code-block:: python
```

### Comparing `django-paypal-2.0/docs/standard/pdt.rst` & `django-paypal-2.1/docs/standard/pdt.rst`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/standard/subscriptions.rst` & `django-paypal-2.1/docs/standard/subscriptions.rst`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/standard/variables.rst` & `django-paypal-2.1/docs/standard/variables.rst`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/docs/tests.rst` & `django-paypal-2.1/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/manage.py` & `django-paypal-2.1/manage.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/creditcard.py` & `django-paypal-2.1/paypal/pro/creditcard.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/fields.py` & `django-paypal-2.1/paypal/pro/fields.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/forms.py` & `django-paypal-2.1/paypal/pro/forms.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/helpers.py` & `django-paypal-2.1/paypal/pro/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 def paypaltime2datetime(s):
     """Convert a PayPal time string to a DateTime."""
     naive = datetime.datetime.strptime(s, PayPalNVP.TIMESTAMP_FORMAT)
     if not settings.USE_TZ:
         return naive
     else:
         # TIMESTAMP_FORMAT is UTC
-        return timezone.make_aware(naive, timezone.utc)
+        return timezone.make_aware(naive, timezone.timezone.utc)
 
 
 class PayPalError(TypeError):
     """Error thrown when something is wrong."""
 
 
 def express_endpoint():
```

### Comparing `django-paypal-2.0/paypal/pro/migrations/0001_initial.py` & `django-paypal-2.1/paypal/pro/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/models.py` & `django-paypal-2.1/paypal/pro/models.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/templates/pro/payment.html` & `django-paypal-2.1/paypal/pro/templates/pro/payment.html`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/tests/settings.py` & `django-paypal-2.1/paypal/pro/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/tests/test_doDirectPayment_authenticated_user.yaml` & `django-paypal-2.1/paypal/pro/tests/test_doDirectPayment_authenticated_user.yaml`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/tests/test_doDirectPayment_invalid.yaml` & `django-paypal-2.1/paypal/pro/tests/test_doDirectPayment_invalid.yaml`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/tests/test_doDirectPayment_valid.yaml` & `django-paypal-2.1/paypal/pro/tests/test_doDirectPayment_valid.yaml`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/tests/test_doDirectPayment_valid_with_signal.yaml` & `django-paypal-2.1/paypal/pro/tests/test_doDirectPayment_valid_with_signal.yaml`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/tests/test_get_redirect.yaml` & `django-paypal-2.1/paypal/pro/tests/test_get_redirect.yaml`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/tests/test_pro.py` & `django-paypal-2.1/paypal/pro/tests/test_pro.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/tests/test_setExpressCheckout.yaml` & `django-paypal-2.1/paypal/pro/tests/test_setExpressCheckout.yaml`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/tests/test_validate_confirm_form_error.yaml` & `django-paypal-2.1/paypal/pro/tests/test_validate_confirm_form_error.yaml`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/pro/views.py` & `django-paypal-2.1/paypal/pro/views.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/conf.py` & `django-paypal-2.1/paypal/standard/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     "https://www.paypal.com/en_US/i/btn/btn_subscribeCC_LG.gif",
 )
 DONATION_BUTTON_IMAGE = getattr(
     settings,
     "PAYPAL_DONATION_BUTTON_IMAGE",
     "https://www.paypal.com/en_US/i/btn/btn_donateCC_LG.gif",
 )
+PAY_BUTTON_IMAGE = getattr(
+    settings,
+    "PAYPAL_PAY_BUTTON_IMAGE",
+    "https://www.paypal.com/en_US/i/btn/btn_paynowCC_LG.gif",
+)
 
 
 # Paypal Encrypt Certificate
 PAYPAL_PRIVATE_CERT = getattr(settings, "PAYPAL_PRIVATE_CERT", None)
 PAYPAL_PUBLIC_CERT = getattr(settings, "PAYPAL_PUBLIC_CERT", None)
 PAYPAL_CERT = getattr(settings, "PAYPAL_CERT", None)
 PAYPAL_CERT_ID = getattr(settings, "PAYPAL_CERT_ID", None)
```

### Comparing `django-paypal-2.0/paypal/standard/forms.py` & `django-paypal-2.1/paypal/standard/forms.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 
 from paypal.standard.conf import (
     BUY_BUTTON_IMAGE,
     DONATION_BUTTON_IMAGE,
     LOGIN_URL,
+    PAY_BUTTON_IMAGE,
     PAYPAL_CERT,
     PAYPAL_CERT_ID,
     PAYPAL_PRIVATE_CERT,
     PAYPAL_PUBLIC_CERT,
     SANDBOX_LOGIN_URL,
     SUBSCRIPTION_BUTTON_IMAGE,
 )
@@ -84,15 +85,15 @@
                 code="invalid_date",
             )
 
         if zone_part in ["PDT", "PST"]:
             # PST/PDT is 'US/Pacific'
             dt = pytz.timezone("US/Pacific").localize(dt, is_dst=zone_part == "PDT")
             if not settings.USE_TZ:
-                dt = timezone.make_naive(dt, timezone=timezone.utc)
+                dt = timezone.make_naive(dt, timezone=timezone.timezone.utc)
         return dt
 
 
 # OK, fun days:
 # * Django 4.0 adds a `render` method to a base class, which earlier versions
 #   did not have, with a different signature to our `render()`, breaking everything.
 # * Doing `the_form.render` in a template has been the documented
@@ -145,14 +146,15 @@
         (1, "reattempt billing on Failure"),
         (0, "Do Not reattempt on failure"),
     )
 
     BUY = "buy"
     SUBSCRIBE = "subscribe"
     DONATE = "donate"
+    PAY = "pay"
 
     # Default fields.
     cmd = forms.ChoiceField(widget=forms.HiddenInput(), initial=CMD_CHOICES[0][0])
     charset = forms.CharField(widget=forms.HiddenInput(), initial="utf-8")
     currency_code = forms.CharField(widget=forms.HiddenInput(), initial="USD")
     no_shipping = forms.ChoiceField(
         widget=forms.HiddenInput(),
@@ -187,52 +189,51 @@
     def get_login_url(self):
         "Returns the endpoint url for the form."
         if self.test_mode():
             return SANDBOX_LOGIN_URL
         else:
             return LOGIN_URL
 
+    def get_html(self):
+        return format_html(
+            """<form action="{0}" method="post">{1}{2}</form>""",
+            self.get_login_url(),
+            self.as_p(),
+            self.get_html_submit_element(),
+        )
+
+    def get_html_submit_element(self):
+        return format_html(
+            """<input type="image" src="{0}" name="submit" alt="Buy it Now" />""",
+            self.get_image(),
+        )
+
     if DJANGO_FORM_HAS_RENDER_METHOD:
 
         def render(self, *args, **kwargs):
             if not args and not kwargs:
                 # `form.render` usage from template
-                return format_html(
-                    """<form action="{0}" method="post">
-    {1}
-    <input type="image" src="{2}" name="submit" alt="Buy it Now" />
-</form>""",
-                    self.get_login_url(),
-                    self.as_p(),
-                    self.get_image(),
-                )
+                return self.get_html()
             else:
                 # Need to delegate to super. This provides
                 # support for `as_p` method and for `BoundField.label_tag`,
                 # and perhaps others.
                 return super().render(*args, **kwargs)
 
     else:
 
         def render(self):
-            return format_html(
-                """<form action="{0}" method="post">
-    {1}
-    <input type="image" src="{2}" name="submit" alt="Buy it Now" />
-</form>""",
-                self.get_login_url(),
-                self.as_p(),
-                self.get_image(),
-            )
+            return self.get_html()
 
     def get_image(self):
         return {
             self.SUBSCRIBE: SUBSCRIPTION_BUTTON_IMAGE,
             self.BUY: BUY_BUTTON_IMAGE,
             self.DONATE: DONATION_BUTTON_IMAGE,
+            self.PAY: PAY_BUTTON_IMAGE,
         }[self.button_type]
 
     def is_transaction(self):
         warn_untested()
         return not self.is_subscription()
 
     def is_donation(self):
```

### Comparing `django-paypal-2.0/paypal/standard/helpers.py` & `django-paypal-2.1/paypal/standard/helpers.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/admin.py` & `django-paypal-2.1/paypal/standard/ipn/admin.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/migrations/0001_initial.py` & `django-paypal-2.1/paypal/standard/ipn/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/migrations/0004_auto_20150612_1826.py` & `django-paypal-2.1/paypal/standard/ipn/migrations/0004_auto_20150612_1826.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/migrations/0005_auto_20151217_0948.py` & `django-paypal-2.1/paypal/standard/ipn/migrations/0005_auto_20151217_0948.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/migrations/0006_auto_20160108_1112.py` & `django-paypal-2.1/paypal/standard/ipn/migrations/0006_auto_20160108_1112.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/migrations/0007_auto_20160219_1135.py` & `django-paypal-2.1/paypal/standard/ipn/migrations/0007_auto_20160219_1135.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/migrations/0008_auto_20181128_1032.py` & `django-paypal-2.1/paypal/standard/ipn/migrations/0008_auto_20181128_1032.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/models.py` & `django-paypal-2.1/paypal/standard/ipn/models.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/signals.py` & `django-paypal-2.1/paypal/standard/ipn/signals.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/templates/ipn/ipn_test.html` & `django-paypal-2.1/paypal/standard/ipn/templates/ipn/ipn_test.html`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/tests/test_admin.py` & `django-paypal-2.1/paypal/standard/ipn/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/tests/test_cert__do_not_use__private.pem` & `django-paypal-2.1/paypal/standard/ipn/tests/test_cert__do_not_use__private.pem`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/tests/test_cert__do_not_use__public.pem` & `django-paypal-2.1/paypal/standard/ipn/tests/test_cert__do_not_use__public.pem`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/tests/test_cert_from_paypal__do_not_use.pem` & `django-paypal-2.1/paypal/standard/ipn/tests/test_cert_from_paypal__do_not_use.pem`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/tests/test_forms.py` & `django-paypal-2.1/paypal/standard/ipn/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/ipn/tests/test_ipn.py` & `django-paypal-2.1/paypal/standard/ipn/tests/test_ipn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import locale
 import unittest
-from datetime import datetime
+from datetime import datetime, timezone
 from decimal import Decimal
 from urllib.parse import urlencode
 
 from django.conf import settings
 from django.test import TestCase
 from django.test.utils import override_settings
-from django.utils import timezone
 
 from paypal.standard.ipn.models import PayPalIPN
 from paypal.standard.ipn.signals import invalid_ipn_received, valid_ipn_received
 from paypal.standard.ipn.views import CONTENT_TYPE_ERROR
 from paypal.standard.models import ST_PP_CANCELLED
 
 # Parameters are all bytestrings, so we can construct a bytestring
@@ -380,15 +379,14 @@
     def test_postback(self):
         # Incorrect signature means we will always get failure
         self.assertFlagged({}, "Invalid postback. (INVALID)")
 
 
 @override_settings(ROOT_URLCONF="paypal.standard.ipn.tests.test_urls")
 class IPNSimulatorTests(TestCase):
-
     # Some requests, as sent by the simulator.
 
     # The simulator itself has bugs. For example, it doesn't send the 'charset'
     # parameter, unlike in production. We could wait for PayPal to fix these
     # bugs... ha ha, only kidding! If developers want to use the simulator, we
     # need to deal with whatever it sends.
```

### Comparing `django-paypal-2.0/paypal/standard/ipn/views.py` & `django-paypal-2.1/paypal/standard/ipn/views.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/models.py` & `django-paypal-2.1/paypal/standard/models.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/admin.py` & `django-paypal-2.1/paypal/standard/pdt/admin.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/migrations/0001_initial.py` & `django-paypal-2.1/paypal/standard/pdt/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/migrations/0004_auto_20151029_1515.py` & `django-paypal-2.1/paypal/standard/pdt/migrations/0004_auto_20151029_1515.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/migrations/0005_auto_20151217_0948.py` & `django-paypal-2.1/paypal/standard/pdt/migrations/0005_auto_20151217_0948.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/migrations/0006_auto_20160108_1112.py` & `django-paypal-2.1/paypal/standard/pdt/migrations/0006_auto_20160108_1112.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/migrations/0007_auto_20160219_1137.py` & `django-paypal-2.1/paypal/standard/pdt/migrations/0007_auto_20160219_1137.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/migrations/0008_auto_20181128_1032.py` & `django-paypal-2.1/paypal/standard/pdt/migrations/0008_auto_20181128_1032.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/models.py` & `django-paypal-2.1/paypal/standard/pdt/models.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/tests/settings.py` & `django-paypal-2.1/paypal/standard/pdt/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/tests/templates/pdt/pdt.html` & `django-paypal-2.1/paypal/standard/pdt/tests/templates/pdt/pdt.html`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/tests/templates/pdt/test_pdt_response.html` & `django-paypal-2.1/paypal/standard/pdt/tests/templates/pdt/test_pdt_response.html`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/tests/test_pdt.py` & `django-paypal-2.1/paypal/standard/pdt/tests/test_pdt.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/tests/test_urls.py` & `django-paypal-2.1/paypal/standard/pdt/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/standard/pdt/views.py` & `django-paypal-2.1/paypal/standard/pdt/views.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/paypal/utils.py` & `django-paypal-2.1/paypal/utils.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/runtests.py` & `django-paypal-2.1/runtests.py`

 * *Files identical despite different names*

### Comparing `django-paypal-2.0/setup.py` & `django-paypal-2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 DESCRIPTION = "A pluggable Django application for integrating PayPal Payments Standard or Payments Pro"
 URL = "https://github.com/spookylukey/django-paypal"
 DOCS_URL = "https://django-paypal.readthedocs.org"
 
 setup(
     name="django-paypal",
-    version="2.0",
+    version="2.1",
     author="John Boxall",
     author_email="john@handimobility.ca",
     maintainer="Luke Plant",
     maintainer_email="L.Plant.98@cantab.net",
     url=URL,
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=[
         "Django>=2.2",
         "requests>=2.5.3",
         "pytz>=2015.4",
     ],
     description=DESCRIPTION,
     long_description=f"{DESCRIPTION}\n\nHome page: {URL}\n\nDocs: {DOCS_URL}\n",
@@ -38,14 +38,13 @@
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 4.0",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Topic :: Software Development",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
 )
```

