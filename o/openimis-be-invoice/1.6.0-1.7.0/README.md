# Comparing `tmp/openimis-be-invoice-1.6.0.tar.gz` & `tmp/openimis_be_invoice-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-invoice-1.6.0.tar", last modified: Sat Dec 16 00:57:59 2023, max compression
+gzip compressed data, was "openimis_be_invoice-1.7.0.tar", last modified: Tue Apr 30 09:06:37 2024, max compression
```

## Comparing `openimis-be-invoice-1.6.0.tar` & `openimis_be_invoice-1.7.0.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.232884 openimis-be-invoice-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-16 00:57:59.232884 openimis-be-invoice-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.216884 openimis-be-invoice-1.6.0/invoice/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.216884 openimis-be-invoice-1.6.0/invoice/gql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.216884 openimis-be-invoice-1.6.0/invoice/gql/bill/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.216884 openimis-be-invoice-1.6.0/invoice/gql/bill_event/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill_event/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill_event/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.220884 openimis-be-invoice-1.6.0/invoice/gql/bill_item/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill_item/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill_item/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.220884 openimis-be-invoice-1.6.0/invoice/gql/bill_payment/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill_payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill_payment/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/bill_payment/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.220884 openimis-be-invoice-1.6.0/invoice/gql/detail_payment_invoice/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/detail_payment_invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/detail_payment_invoice/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/detail_payment_invoice/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/filter_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.220884 openimis-be-invoice-1.6.0/invoice/gql/gql_types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/gql_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/gql_types/bill_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/gql_types/invoice_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/gql_types/payment_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/input_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.220884 openimis-be-invoice-1.6.0/invoice/gql/invoice/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.220884 openimis-be-invoice-1.6.0/invoice/gql/invoice_event/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice_event/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice_event/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.220884 openimis-be-invoice-1.6.0/invoice/gql/invoice_line_item/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice_line_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice_line_item/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice_line_item/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.220884 openimis-be-invoice-1.6.0/invoice/gql/invoice_payment/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice_payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice_payment/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/invoice_payment/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.220884 openimis-be-invoice-1.6.0/invoice/gql/payment_invoice/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/payment_invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/payment_invoice/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/payment_invoice/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/gql/query_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.224884 openimis-be-invoice-1.6.0/invoice/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    57283 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0001_initial_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0002_auto_20211117_0904.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0003_auto_20211203_1053.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0004_invoice_bill_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0005_invoice_bill_roles_for_accountant.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0006_detailpaymentinvoice_historicaldetailpaymentinvoice_historicalpaymentinvoice_paymentinvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0007_auto_20220411_1053.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0008_auto_20220411_1358.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0009_auto_20220413_0824.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0010_auto_20230126_0903.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0011_auto_20230914_0805.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/0012_auto_20230921_0835.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    15353 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.224884 openimis-be-invoice-1.6.0/invoice/services/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/services/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/services/billLineItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/services/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/services/invoiceLineItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/services/invoicePayments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/services/paymentInvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.224884 openimis-be-invoice-1.6.0/invoice/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.228884 openimis-be-invoice-1.6.0/invoice/tests/gql/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/gql/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/gql/detail_payment_invoice_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/gql/invoice_event_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/gql/invoice_line_item_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/gql/invoice_payment_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/gql/invoice_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9245 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/gql/payment_invoice_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.228884 openimis-be-invoice-1.6.0/invoice/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/helpers/bill_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/helpers/bill_line_item_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/helpers/bill_payment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/helpers/default_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/helpers/invoice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/helpers/invoice_line_item_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/helpers/invoice_payment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/helpers/payment_invoice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.228884 openimis-be-invoice-1.6.0/invoice/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12998 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/services/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/services/invoiceLineItem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/services/invoicePayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/tests/services/paymentInvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.232884 openimis-be-invoice-1.6.0/invoice/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/validation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/validation/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/validation/billLineItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/validation/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/validation/invoiceLineItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/validation/invoicePayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/validation/paymentInvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/validation/paymentStatusValidation.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:49.000000 openimis-be-invoice-1.6.0/invoice/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:59.232884 openimis-be-invoice-1.6.0/openimis_be_invoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-16 00:57:59.000000 openimis-be-invoice-1.6.0/openimis_be_invoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2023-12-16 00:57:59.000000 openimis-be-invoice-1.6.0/openimis_be_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:59.000000 openimis-be-invoice-1.6.0/openimis_be_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-16 00:57:59.000000 openimis-be-invoice-1.6.0/openimis_be_invoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-16 00:57:59.000000 openimis-be-invoice-1.6.0/openimis_be_invoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:59.232884 openimis-be-invoice-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-12-16 00:57:58.000000 openimis-be-invoice-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.245438 openimis_be_invoice-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 09:06:37.245438 openimis_be_invoice-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.229438 openimis_be_invoice-1.7.0/invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.229438 openimis_be_invoice-1.7.0/invoice/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.229438 openimis_be_invoice-1.7.0/invoice/gql/bill/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.229438 openimis_be_invoice-1.7.0/invoice/gql/bill_event/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill_event/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill_event/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.233438 openimis_be_invoice-1.7.0/invoice/gql/bill_item/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill_item/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill_item/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.233438 openimis_be_invoice-1.7.0/invoice/gql/bill_payment/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill_payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill_payment/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/bill_payment/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.233438 openimis_be_invoice-1.7.0/invoice/gql/detail_payment_invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/detail_payment_invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/detail_payment_invoice/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/detail_payment_invoice/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/filter_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.233438 openimis_be_invoice-1.7.0/invoice/gql/gql_types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/gql_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/gql_types/bill_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/gql_types/invoice_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/gql_types/payment_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/input_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.233438 openimis_be_invoice-1.7.0/invoice/gql/invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.233438 openimis_be_invoice-1.7.0/invoice/gql/invoice_event/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice_event/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice_event/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.233438 openimis_be_invoice-1.7.0/invoice/gql/invoice_line_item/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice_line_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice_line_item/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice_line_item/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.237438 openimis_be_invoice-1.7.0/invoice/gql/invoice_payment/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice_payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice_payment/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/invoice_payment/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.237438 openimis_be_invoice-1.7.0/invoice/gql/payment_invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/payment_invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/payment_invoice/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/payment_invoice/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/gql/query_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.237438 openimis_be_invoice-1.7.0/invoice/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    57283 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0001_initial_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0002_auto_20211117_0904.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0003_auto_20211203_1053.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0004_invoice_bill_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0005_invoice_bill_roles_for_accountant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0006_detailpaymentinvoice_historicaldetailpaymentinvoice_historicalpaymentinvoice_paymentinvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0007_auto_20220411_1053.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0008_auto_20220411_1358.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0009_auto_20220413_0824.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0010_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0011_auto_20230914_0805.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0012_auto_20230921_0835.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46872 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/0013_alter_bill_code_ext_alter_bill_code_tp_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.241438 openimis_be_invoice-1.7.0/invoice/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/services/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/services/billLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/services/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/services/invoiceLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/services/invoicePayments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/services/paymentInvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.241438 openimis_be_invoice-1.7.0/invoice/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.241438 openimis_be_invoice-1.7.0/invoice/tests/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/gql/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/gql/detail_payment_invoice_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/gql/invoice_event_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/gql/invoice_line_item_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/gql/invoice_payment_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/gql/invoice_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/gql/payment_invoice_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.241438 openimis_be_invoice-1.7.0/invoice/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/helpers/bill_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/helpers/bill_line_item_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/helpers/bill_payment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/helpers/default_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/helpers/invoice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/helpers/invoice_line_item_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/helpers/invoice_payment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/helpers/payment_invoice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.245438 openimis_be_invoice-1.7.0/invoice/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13062 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/services/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/services/invoiceLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/services/invoicePayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/tests/services/paymentInvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.245438 openimis_be_invoice-1.7.0/invoice/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/validation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/validation/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/validation/billLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/validation/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/validation/invoiceLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/validation/invoicePayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/validation/paymentInvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/validation/paymentStatusValidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:28.000000 openimis_be_invoice-1.7.0/invoice/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:37.245438 openimis_be_invoice-1.7.0/openimis_be_invoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 09:06:37.000000 openimis_be_invoice-1.7.0/openimis_be_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-30 09:06:37.000000 openimis_be_invoice-1.7.0/openimis_be_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:37.000000 openimis_be_invoice-1.7.0/openimis_be_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 09:06:37.000000 openimis_be_invoice-1.7.0/openimis_be_invoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 09:06:37.000000 openimis_be_invoice-1.7.0/openimis_be_invoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:37.245438 openimis_be_invoice-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-30 09:06:36.000000 openimis_be_invoice-1.7.0/setup.py
```

### Comparing `openimis-be-invoice-1.6.0/LICENSE` & `openimis_be_invoice-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/PKG-INFO` & `openimis_be_invoice-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-invoice
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Invoice Payment reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-invoice-1.6.0/invoice/apps.py` & `openimis_be_invoice-1.7.0/invoice/apps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 import logging
 
 from django.apps import AppConfig
+from core.utils import ConfigUtilMixin
 
 MODULE_NAME = 'invoice'
 
 DEFAULT_CONFIG = {
     "default_currency_code": "USD",
     "gql_invoice_search_perms": ["155101"],
     "gql_invoice_create_perms": ["155102"],
     "gql_invoice_update_perms": ["155103"],
     "gql_invoice_delete_perms": ["155104"],
-    "gql_invoice_amend_perms":  ["155109"],
+    "gql_invoice_amend_perms": ["155109"],
 
     "gql_invoice_payment_search_perms": ["155201"],
     "gql_invoice_payment_create_perms": ["155202"],
     "gql_invoice_payment_update_perms": ["155203"],
     "gql_invoice_payment_delete_perms": ["155204"],
     "gql_invoice_payment_refund_perms": ["155206"],
 
-    "gql_invoice_event_search_perms":             ["155301"],
-    "gql_invoice_event_create_perms":             ["155302"],
-    "gql_invoice_event_update_perms":             ["155303"],
-    "gql_invoice_event_delete_perms":             ["155304"],
-    "gql_invoice_event_create_message_perms":     ["155306"],
-    "gql_invoice_event_delete_my_message_perms":  ["155307"],
+    "gql_invoice_event_search_perms": ["155301"],
+    "gql_invoice_event_create_perms": ["155302"],
+    "gql_invoice_event_update_perms": ["155303"],
+    "gql_invoice_event_delete_perms": ["155304"],
+    "gql_invoice_event_create_message_perms": ["155306"],
+    "gql_invoice_event_delete_my_message_perms": ["155307"],
     "gql_invoice_event_delete_all_message_perms": ["155308"],
 
     "gql_bill_search_perms": ["156101"],
     "gql_bill_create_perms": ["156102"],
     "gql_bill_update_perms": ["156103"],
     "gql_bill_delete_perms": ["156104"],
-    "gql_bill_amend_perms":  ["156109"],
+    "gql_bill_amend_perms": ["156109"],
 
     "gql_bill_payment_search_perms": ["156201"],
     "gql_bill_payment_create_perms": ["156202"],
     "gql_bill_payment_update_perms": ["156203"],
     "gql_bill_payment_delete_perms": ["156204"],
     "gql_bill_payment_refund_perms": ["156206"],
 
-    "gql_bill_event_search_perms":             ["156301"],
-    "gql_bill_event_create_perms":             ["156302"],
-    "gql_bill_event_update_perms":             ["156303"],
-    "gql_bill_event_delete_perms":             ["156304"],
-    "gql_bill_event_create_message_perms":     ["156306"],
-    "gql_bill_event_delete_my_message_perms":  ["156307"],
+    "gql_bill_event_search_perms": ["156301"],
+    "gql_bill_event_create_perms": ["156302"],
+    "gql_bill_event_update_perms": ["156303"],
+    "gql_bill_event_delete_perms": ["156304"],
+    "gql_bill_event_create_message_perms": ["156306"],
+    "gql_bill_event_delete_my_message_perms": ["156307"],
     "gql_bill_event_delete_all_message_perms": ["156308"],
+
+    # Functions of type Callable[[QuerySet, User], QuerySet], to be used as custom user filters for bills and invoices
+    # To be specified as "module_name.submodule.function_name"
+    "bill_user_filter_function": None,
+    "invoice_user_filter_function": None,
 }
 
 logger = logging.getLogger(__name__)
 
 
-class InvoiceConfig(AppConfig):
+class InvoiceConfig(AppConfig, ConfigUtilMixin):
     name = MODULE_NAME
 
     default_currency_code = None
     gql_invoice_search_perms = None
     gql_invoice_create_perms = None
     gql_invoice_update_perms = None
     gql_invoice_delete_perms = None
@@ -85,16 +91,18 @@
     gql_bill_event_create_perms = None
     gql_bill_event_update_perms = None
     gql_bill_event_delete_perms = None
     gql_bill_event_create_message_perms = None
     gql_bill_event_delete_my_message_perms = None
     gql_bill_event_delete_all_message_perms = None
 
-    def __load_config(self, cfg):
-        for field in cfg:
-            if hasattr(InvoiceConfig, field):
-                setattr(InvoiceConfig, field, cfg[field])
+    bill_user_filter = None
+    invoice_user_filter = None
 
     def ready(self):
         from core.models import ModuleConfiguration
         cfg = ModuleConfiguration.get_or_default(MODULE_NAME, DEFAULT_CONFIG)
-        self.__load_config(cfg)
+        self._load_config_fields(cfg)
+        if cfg['bill_user_filter_function']:
+            self._load_config_function('bill_user_filter', cfg['bill_user_filter_function'])
+        if cfg['invoice_user_filter_function']:
+            self._load_config_function('invoice_user_filter', cfg['invoice_user_filter_function'])
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/bill/mutation.py` & `openimis_be_invoice-1.7.0/invoice/gql/bill/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/bill/query.py` & `openimis_be_invoice-1.7.0/invoice/gql/bill/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-import functools
-import logging
-import types
-
 import graphene
-import pandas as pd
 from django.contrib.auth.models import AnonymousUser
 from django.contrib.contenttypes.models import ContentType
 from django.db.models import Q
-from django.http import HttpResponse
 from pandas import DataFrame
 
 from core.gql.export_mixin import ExportableQueryMixin
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
 from invoice.gql.gql_types.bill_types import BillGQLType
@@ -22,22 +16,23 @@
 
 
 def patch_subjects(bills_df: DataFrame):
     subject_df = bills_df[['subject_type', 'subject_id']].drop_duplicates()
     bills_df['subject_class'] = 'undefined'
     for subject in subject_df['subject_type'].unique():
         model = ContentType.objects.get(id=subject).model_class()
-        entities_for_model = subject_df[subject_df['subject_type']==subject]['subject_id']
+        entities_for_model = subject_df[subject_df['subject_type'] == subject]['subject_id']
         if model == Policy:
-            subject_names = model.objects\
-                .filter(id__in=entities_for_model)\
+            subject_names = model.objects \
+                .filter(id__in=entities_for_model) \
                 .values('id', 'family__head_insuree__chf_id',
                         'family__head_insuree__last_name', 'family__head_insuree__other_names')
             names = {
-                str(x['id']): F"{x['family__head_insuree__other_names']} {x['family__head_insuree__last_name']} ({x['family__head_insuree__chf_id']})" for x in subject_names
+                str(x['id']): F"{x['family__head_insuree__other_names']} {x['family__head_insuree__last_name']} ({x['family__head_insuree__chf_id']})"
+                for x in subject_names
             }
             updated = bills_df['subject_type'] == subject
             bills_df.loc[updated, 'subject_id'] = bills_df[updated]['subject_id'].apply(lambda x: names[x])
         bills_df.loc[bills_df['subject_type'] == subject, 'subject_class'] = model.__name__
         bills_df['subject_type'] = bills_df.pop('subject_class')
     return bills_df
 
@@ -56,14 +51,15 @@
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String(),
     )
 
     def resolve_bill(self, info, **kwargs):
+        BillQueryMixin._check_permissions(info.context.user)
         filters = []
         filters += append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
@@ -71,15 +67,18 @@
         if subject_type:
             filters.append(Q(subject_type__model=subject_type))
 
         thirdparty_type = kwargs.get("thirdparty_type", None)
         if thirdparty_type:
             filters.append(Q(thirdparty_type__model=thirdparty_type))
 
-        BillQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(Bill.objects.filter(*filters).all(), info)
+        qs = Bill.objects.filter(*filters)
+        if InvoiceConfig.bill_user_filter:
+            qs = InvoiceConfig.bill_user_filter(qs, info.context.user)
+
+        return gql_optimizer.query(qs, info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 InvoiceConfig.gql_bill_search_perms):
             raise PermissionError("Unauthorized")
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/bill_event/mutation.py` & `openimis_be_invoice-1.7.0/invoice/gql/bill_event/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/bill_item/query.py` & `openimis_be_invoice-1.7.0/invoice/gql/bill_item/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,41 +2,47 @@
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
 from invoice.gql.gql_types.bill_types import BillItemGQLType
-from invoice.models import BillItem
+from invoice.models import BillItem, Bill
 import graphene_django_optimizer as gql_optimizer
 
 
 class BillItemQueryMixin:
     bill_item = OrderedDjangoFilterConnectionField(
         BillItemGQLType,
         orderBy=graphene.List(of_type=graphene.String),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String(),
     )
 
     def resolve_bill_item(self, info, **kwargs):
+        BillItemQueryMixin._check_permissions(info.context.user)
         filters = []
         filters += append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
         line_type = kwargs.get("line_type", None)
         if line_type:
             filters.append(Q(line_type__model=line_type))
 
-        BillItemQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(BillItem.objects.filter(*filters).all(), info)
+        bill_li_qs = BillItem.objects.filter(*filters)
+
+        if InvoiceConfig.bill_user_filter:
+            bill_qs = InvoiceConfig.bill_user_filter(Bill.objects.all(), info.context.user)
+            bill_li_qs = bill_li_qs.filter(bill__in=bill_qs)
+
+        return gql_optimizer.query(bill_li_qs, info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 InvoiceConfig.gql_bill_search_perms):
             raise PermissionError("Unauthorized")
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/bill_payment/mutation.py` & `openimis_be_invoice-1.7.0/invoice/gql/bill_payment/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/bill_payment/query.py` & `openimis_be_invoice-1.7.0/invoice/gql/bill_event/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import graphene
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
-from invoice.gql.gql_types.bill_types import BillPaymentGQLType
-from invoice.models import BillPayment
+from invoice.gql.gql_types.bill_types import BillEventGQLType
+from invoice.models import BillEvent, Bill
 import graphene_django_optimizer as gql_optimizer
 
 
-class BillPaymentQueryMixin:
-    bill_payment = OrderedDjangoFilterConnectionField(
-        BillPaymentGQLType,
+class BillEventQueryMixin:
+    bill_event = OrderedDjangoFilterConnectionField(
+        BillEventGQLType,
         orderBy=graphene.List(of_type=graphene.String),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String(),
     )
 
-    def resolve_bill_payment(self, info, **kwargs):
+    def resolve_bill_event(self, info, **kwargs):
+        BillEventQueryMixin._check_permissions(info.context.user)
         filters = []
         filters += append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
-        BillPaymentQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(BillPayment.objects.filter(*filters).all(), info)
+        bill_event_qs = BillEvent.objects.filter(*filters)
+
+        if InvoiceConfig.bill_user_filter:
+            bill_qs = InvoiceConfig.bill_user_filter(Bill.objects.all(), info.context.user)
+            bill_event_qs = bill_event_qs.filter(bill__in=bill_qs)
+
+        return gql_optimizer.query(bill_event_qs, info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
-                InvoiceConfig.gql_bill_payment_search_perms):
+                InvoiceConfig.gql_bill_event_search_perms):
             raise PermissionError("Unauthorized")
-
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/detail_payment_invoice/mutation.py` & `openimis_be_invoice-1.7.0/invoice/gql/detail_payment_invoice/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/detail_payment_invoice/query.py` & `openimis_be_invoice-1.7.0/invoice/gql/detail_payment_invoice/query.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/filter_mixin.py` & `openimis_be_invoice-1.7.0/invoice/gql/filter_mixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/gql_types/bill_types.py` & `openimis_be_invoice-1.7.0/invoice/gql/gql_types/invoice_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,164 +1,169 @@
 import graphene
 import json
-from django.contrib.contenttypes.models import ContentType
 from django.core.serializers.json import DjangoJSONEncoder
 from graphene_django import DjangoObjectType
 
 from core import prefix_filterset, ExtendedConnection
-from invoice.apps import InvoiceConfig
+from insuree.models import Insuree
 from invoice.gql.filter_mixin import GenericFilterGQLTypeMixin
-from invoice.models import Bill, \
-    BillItem, BillEvent, BillPayment
+from invoice.models import Invoice, InvoiceLineItem, InvoicePayment, InvoiceEvent, InvoiceMutation, \
+    InvoicePaymentMutation, InvoiceLineItemMutation, InvoiceEventMutation
 from invoice.utils import underscore_to_camel
-from location.models import Location
-from product.models import Product
-from django.core.exceptions import PermissionDenied
-from django.utils.translation import gettext as _
 
 
-class BillGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
-
+class InvoiceGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
+    subject = graphene.JSONString()
     subject_type = graphene.Int()
+    subject_type_name = graphene.String()
+    thirdparty = graphene.JSONString()
+    thirdparty_type = graphene.Int()
+    thirdparty_type_name = graphene.String()
+
     def resolve_subject_type(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.subject_type.id
+        if root.subject_type:
+            return root.subject_type.id
 
-    subject_type_name = graphene.String()
     def resolve_subject_type_name(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.subject_type.name
+        if root.subject_type:
+            return root.subject_type.name
 
-    thirdparty_type = graphene.Int()
     def resolve_thirdparty_type(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.thirdparty_type.id
+        if root.thirdparty_type:
+            return root.thirdparty_type.id
 
-    thirdparty_type_name = graphene.String()
     def resolve_thirdparty_type_name(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.thirdparty_type.name
+        if root.thirdparty_type:
+            return root.thirdparty_type.name
 
-    subject = graphene.JSONString()
     def resolve_subject(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        subject_object_dict = root.subject.__dict__
-        subject_object_dict.pop('_state')
-        subject_object_dict = {
-            underscore_to_camel(k): v for k, v in list(subject_object_dict.items())
-        }
-        if root.subject_type.name == "batch run":
-            location = Location.objects.filter(id=subject_object_dict['locationId'], validity_to__isnull=True)
-            location = location.values('code', 'name')
-            subject_object_dict['location'] = {
-                underscore_to_camel(k): v for k, v in location.first().items()
+        if root.subject:
+            subject_object_dict = root.subject.__dict__
+            subject_object_dict.pop('_state')
+            subject_object_dict = {
+                underscore_to_camel(k): v for k, v in list(subject_object_dict.items())
             }
-        subject_object_dict = json.dumps(subject_object_dict, cls=DjangoJSONEncoder)
-        return subject_object_dict
+            if root.subject_type.name == "family":
+                insuree = Insuree.objects.filter(id=subject_object_dict['headInsureeId'], validity_to__isnull=True)
+                insuree = insuree.values('id', 'chf_id', 'uuid', 'last_name', 'other_names')
+                subject_object_dict['headInsuree'] = {
+                    underscore_to_camel(k): v for k, v in insuree.first().items()
+                }
+            subject_object_dict = json.dumps(subject_object_dict, cls=DjangoJSONEncoder)
+            return subject_object_dict
 
-    thirdparty = graphene.JSONString()
     def resolve_thirdparty(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        thirdparty_object_dict = root.thirdparty.__dict__
-        thirdparty_object_dict.pop('_state')
-        thirdparty_object_dict = {
-            underscore_to_camel(k): v for k, v in list(thirdparty_object_dict.items())
-        }
-        thirdparty_object_dict = json.dumps(thirdparty_object_dict, cls=DjangoJSONEncoder)
-        return thirdparty_object_dict
+        if root.thirdparty:
+            thirdparty_object_dict = root.thirdparty.__dict__
+
+            thirdparty_object_dict.pop('_state')
+            thirdparty_object_dict = {
+                underscore_to_camel(k): v for k, v in list(thirdparty_object_dict.items())
+            }
+            thirdparty_object_dict = json.dumps(thirdparty_object_dict, cls=DjangoJSONEncoder)
+            return thirdparty_object_dict
 
     class Meta:
-        model = Bill
+        model = Invoice
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             **GenericFilterGQLTypeMixin.get_base_filters_invoice(),
-            "date_bill": ["exact", "lt", "lte", "gt", "gte"],
+            "date_invoice": ["exact", "lt", "lte", "gt", "gte"],
         }
 
         connection_class = ExtendedConnection
 
         @classmethod
         def get_queryset(cls, queryset, info):
-            return Bill.get_queryset(queryset, info)
+            return Invoice.get_queryset(queryset, info)
 
 
-class BillItemGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
-
+class InvoiceLineItemGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
+    line = graphene.JSONString()
     line_type = graphene.Int()
+    line_type_name = graphene.String()
+
     def resolve_line_type(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.line_type.id
+        if root.line_type:
+            return root.line_type.id
 
-    line_type_name = graphene.String()
     def resolve_line_type_name(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.line_type.name
+        if root.line_type:
+            return root.line_type.name
 
-    line = graphene.JSONString()
     def resolve_line(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_bill_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        line_object_dict = root.line.__dict__
-        line_object_dict.pop('_state')
-        key_values = list(line_object_dict.items())
-        line_object_dict.clear()
-        for k, v in key_values:
-            new_key = underscore_to_camel(k)
-            line_object_dict[new_key] = v
-        line_object_dict = json.dumps(line_object_dict, cls=DjangoJSONEncoder)
-        return line_object_dict
+        if root.line:
+            line_object_dict = root.line.__dict__
+            line_object_dict.pop('_state')
+            key_values = list(line_object_dict.items())
+            line_object_dict.clear()
+            for k, v in key_values:
+                new_key = underscore_to_camel(k)
+                line_object_dict[new_key] = v
+            line_object_dict = json.dumps(line_object_dict, cls=DjangoJSONEncoder)
+            return line_object_dict
 
     class Meta:
-        model = BillItem
+        model = InvoiceLineItem
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             **GenericFilterGQLTypeMixin.get_base_filters_invoice_line_item(),
-            **prefix_filterset("bill__", BillGQLType._meta.filter_fields),
+            **prefix_filterset("invoice__", InvoiceGQLType._meta.filter_fields),
         }
 
         connection_class = ExtendedConnection
 
         @classmethod
         def get_queryset(cls, queryset, info):
-            return BillItem.get_queryset(queryset, info)
-
+            return InvoiceLineItem.get_queryset(queryset, info)
 
-class BillPaymentGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
 
+class InvoicePaymentGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
     class Meta:
-        model = BillPayment
+        model = InvoicePayment
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             **GenericFilterGQLTypeMixin.get_base_filters_invoice_payment(),
-            **prefix_filterset("bill__", BillGQLType._meta.filter_fields),
+            **prefix_filterset("invoice__", InvoiceGQLType._meta.filter_fields),
         }
 
         connection_class = ExtendedConnection
 
         @classmethod
         def get_queryset(cls, queryset, info):
-            return BillPayment.get_queryset(queryset, info)
+            return InvoicePayment.get_queryset(queryset, info)
 
 
-class BillEventGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
-
+class InvoiceEventGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
     class Meta:
-        model = BillEvent
+        model = InvoiceEvent
         interfaces = (graphene.relay.Node,)
         filter_fields = {
-            **prefix_filterset("bill__", BillGQLType._meta.filter_fields),
             **GenericFilterGQLTypeMixin.get_base_filters_invoice_event(),
+            **prefix_filterset("invoice__", InvoiceGQLType._meta.filter_fields),
         }
 
         connection_class = ExtendedConnection
 
         @classmethod
         def get_queryset(cls, queryset, info):
-            return BillEvent.get_queryset(queryset, info)
+            return InvoiceEvent.get_queryset(queryset, info)
+
+
+class InvoiceMutationGQLType(DjangoObjectType):
+    class Meta:
+        model = InvoiceMutation
+
+
+class InvoicePaymentMutationGQLType(DjangoObjectType):
+    class Meta:
+        model = InvoicePaymentMutation
+
+
+class InvoiceLineItemMutationGQLType(DjangoObjectType):
+    class Meta:
+        model = InvoiceLineItemMutation
+
+
+class InvoiceEventMutationGQLType(DjangoObjectType):
+    class Meta:
+        model = InvoiceEventMutation
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/gql_types/invoice_types.py` & `openimis_be_invoice-1.7.0/invoice/tests/services/invoiceLineItem.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,182 +1,169 @@
-import graphene
-import json
-from django.core.serializers.json import DjangoJSONEncoder
-from graphene_django import DjangoObjectType
-
-from core import prefix_filterset, ExtendedConnection
-from insuree.models import Insuree
-from invoice.apps import InvoiceConfig
-from invoice.gql.filter_mixin import GenericFilterGQLTypeMixin
-from invoice.models import Invoice, InvoiceLineItem, InvoicePayment, InvoiceEvent, InvoiceMutation, \
-    InvoicePaymentMutation, InvoiceLineItemMutation, InvoiceEventMutation
-from invoice.utils import underscore_to_camel
-from django.core.exceptions import PermissionDenied
-from django.utils.translation import gettext as _
-
-
-class InvoiceGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
-
-    subject_type = graphene.Int()
-    def resolve_subject_type(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.subject_type.id
-
-    subject_type_name = graphene.String()
-    def resolve_subject_type_name(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.subject_type.name
-
-    thirdparty_type = graphene.Int()
-    def resolve_thirdparty_type(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.thirdparty_type.id
-
-    thirdparty_type_name = graphene.String()
-    def resolve_thirdparty_type_name(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.thirdparty_type.name
-
-    subject = graphene.JSONString()
-    def resolve_subject(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        subject_object_dict = root.subject.__dict__
-        subject_object_dict.pop('_state')
-        subject_object_dict = {
-            underscore_to_camel(k): v for k, v in list(subject_object_dict.items())
-        }
-        if root.subject_type.name == "family":
-            insuree = Insuree.objects.filter(id=subject_object_dict['headInsureeId'], validity_to__isnull=True)
-            insuree = insuree.values('id', 'chf_id', 'uuid', 'last_name', 'other_names')
-            subject_object_dict['headInsuree'] = {
-                underscore_to_camel(k): v for k, v in insuree.first().items()
+from django.db import transaction
+from policy.test_helpers import create_test_policy
+from product.test_helpers import create_test_product
+
+from core.forms import User
+from core.test_helpers import compare_dicts
+from django.test import TestCase
+
+from invoice.models import InvoiceLineItem
+from contract.tests.helpers import create_test_contract
+from policyholder.tests.helpers import create_test_policy_holder
+from insuree.test_helpers import create_test_insuree
+
+from invoice.services.invoiceLineItem import InvoiceLineItemService
+from invoice.tests.helpers import create_test_invoice
+
+
+class ServiceTestInvoiceLineItems(TestCase):
+    BASE_TEST_INVOICE_LINE_ITEM_PAYLOAD = {
+        'code': 'LineItem1',
+        # 'line_type': None,
+        # 'line_id': None,
+        # 'invoiceId': None,
+        'description': 'description_str',
+        'details': '{"test_int": 1, "test_txt": "some_str"}',
+        'ledger_account': 'account',
+        'quantity': 10,
+        'unit_price': 10.5,
+        'discount': 15.5,
+        'tax_rate': None,
+        'tax_analysis': {'lines': [{'code': 'c', 'label': 'l', 'base': '0.1', 'amount': '2.00'}], 'total': '2.0'},
+    }
+
+    BASE_TEST_UPDATE_LINE_ITEM_PAYLOAD = {
+        'code': 'LineItem2',
+        'description': 'description_str2',
+        'details': '{"test_int": 1, "test_txt": "some_str"}',
+        'ledger_account': 'account2',
+        'quantity': 12,
+        'unit_price': 10,
+        'discount': 20,
+        'tax_rate': None,
+        'tax_analysis': {'lines': [{'code': 'c', 'label': 'l', 'base': '0.1', 'amount': '1.00'}], 'total': '1.0'},
+    }
+
+    BASE_EXPECTED_CREATE_RESPONSE = {
+        "success": True,
+        "message": "Ok",
+        "detail": "",
+        "data": {
+            'code': 'LineItem1',
+            'line_type': None,
+            'line_id': None,
+            'invoice': None,
+            'amount_total': 91.5,
+            'amount_net': 89.5,
+            'description': 'description_str',
+            'details': {"test_int": 1, "test_txt": "some_str"},
+            'ledger_account': 'account',
+            'quantity': 10,
+            'unit_price': 10.5,
+            'discount': 15.5,
+            'tax_rate': None,
+            'tax_analysis': {'lines': [{'code': 'c', 'label': 'l', 'base': '0.1', 'amount': '2.00'}], 'total': '2.0'}
+        },
+    }
+
+    BASE_EXPECTED_UPDATE_RESPONSE = {
+        "success": True,
+        "message": "Ok",
+        "detail": "",
+        "data": {
+            'code': 'LineItem2',
+            'amount_total': 101.0,
+            'amount_net': 100.0,
+            'description': 'description_str2',
+            'details': {"test_int": 1, "test_txt": "some_str"},
+            'ledger_account': 'account2',
+            'quantity': 12,
+            'unit_price': 10.0,
+            'discount': 20.0,
+            'tax_analysis': {'lines': [{'code': 'c', 'label': 'l', 'base': '0.1', 'amount': '1.00'}], 'total': '1.0'},
+            'line_id': None,
+            'line_type': None
+        },
+    }
+
+    @classmethod
+    def setUpClass(cls):
+        super(ServiceTestInvoiceLineItems, cls).setUpClass()
+        if not User.objects.filter(username='admin_invoice').exists():
+            User.objects.create_superuser(username='admin_invoice', password='S\/pe®Pąßw0rd™')
+
+        cls.policy_holder = create_test_policy_holder()
+        cls.contract = create_test_contract(cls.policy_holder)
+        cls.user = User.objects.filter(username='admin').first()
+        cls.insuree = create_test_insuree(with_family=True)
+        cls.line_item_service = InvoiceLineItemService(cls.user)
+        cls.invoice = create_test_invoice(cls.contract, cls.insuree)
+        cls.product = create_test_product("TestC0d3", custom_props={"insurance_period": 12})
+        cls.policy = create_test_policy(
+            product=cls.product,
+            insuree=cls.insuree
+        )
+
+        cls.BASE_TEST_INVOICE_LINE_ITEM_PAYLOAD['line'] = cls.policy
+        cls.BASE_TEST_INVOICE_LINE_ITEM_PAYLOAD['invoice'] = cls.invoice
+
+    def test_line_items_create(self):
+        with transaction.atomic():
+            payload = self.BASE_TEST_INVOICE_LINE_ITEM_PAYLOAD.copy()
+            payload['invoice'] = self.invoice
+
+            expected_response = self.BASE_EXPECTED_CREATE_RESPONSE.copy()
+            expected_response['data']['invoice'] = str(self.invoice.pk)
+
+            response = self.line_item_service.create(payload)
+
+            truncated_output = response
+            truncated_output['data'] = {k: v for k, v in truncated_output['data'].items()
+                                        if k in expected_response['data'].keys()}
+
+            line_item = InvoiceLineItem.objects.filter(code=payload['code']).first()
+            expected_response['data']['line_type'] = line_item.line_type.id
+            expected_response['data']['line_id'] = self.policy.pk
+
+            self.assertTrue(compare_dicts(expected_response, response))
+            InvoiceLineItem.objects.filter(code=payload['code']).delete()
+
+    def test_line_items_update(self):
+        self.maxDiff = None
+        with transaction.atomic():
+            create_payload = self.BASE_TEST_INVOICE_LINE_ITEM_PAYLOAD.copy()
+            create_payload['invoice'] = self.invoice
+
+            expected_response = self.BASE_EXPECTED_UPDATE_RESPONSE.copy()
+            expected_response['data']['invoice'] = str(self.invoice.pk)
+
+            self.line_item_service.create(create_payload)
+
+            update_payload = self.BASE_TEST_UPDATE_LINE_ITEM_PAYLOAD.copy()
+            update_payload['id'] = InvoiceLineItem.objects.filter(code=create_payload['code']).first().id
+
+            response = self.line_item_service.update(update_payload)
+            truncated_output = response
+            truncated_output['data'] = {k: v for k, v in truncated_output['data'].items()
+                                        if k in expected_response['data'].keys()}
+
+            line_item = InvoiceLineItem.objects.filter(code=update_payload['code']).first()
+
+            expected_response['data']['line_type'] = line_item.line_type.id
+            expected_response['data']['line_id'] = str(self.policy.pk)
+
+            self.assertTrue(compare_dicts(expected_response, response))
+            InvoiceLineItem.objects.filter(code=update_payload['code']).delete()
+
+    def test_line_items_delete(self):
+        with transaction.atomic():
+            payload = self.BASE_TEST_INVOICE_LINE_ITEM_PAYLOAD.copy()
+            expected_response = {
+                "success": True,
+                "message": "Ok",
+                "detail": "",
             }
-        subject_object_dict = json.dumps(subject_object_dict, cls=DjangoJSONEncoder)
-        return subject_object_dict
 
-    thirdparty = graphene.JSONString()
-    def resolve_thirdparty(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        thirdparty_object_dict = root.thirdparty.__dict__
-        thirdparty_object_dict.pop('_state')
-        thirdparty_object_dict = {
-            underscore_to_camel(k): v for k, v in list(thirdparty_object_dict.items())
-        }
-        thirdparty_object_dict = json.dumps(thirdparty_object_dict, cls=DjangoJSONEncoder)
-        return thirdparty_object_dict
-
-    class Meta:
-        model = Invoice
-        interfaces = (graphene.relay.Node,)
-        filter_fields = {
-            **GenericFilterGQLTypeMixin.get_base_filters_invoice(),
-            "date_invoice": ["exact", "lt", "lte", "gt", "gte"],
-        }
-
-        connection_class = ExtendedConnection
-
-        @classmethod
-        def get_queryset(cls, queryset, info):
-            return Invoice.get_queryset(queryset, info)
-
-
-class InvoiceLineItemGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
-
-    line_type = graphene.Int()
-    def resolve_line_type(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.line_type.id
-
-    line_type_name = graphene.String()
-    def resolve_line_type_name(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        return root.line_type.name
-
-    line = graphene.JSONString()
-    def resolve_line(root, info):
-        if not info.context.user.has_perms(InvoiceConfig.gql_invoice_search_perms):
-            raise PermissionDenied(_("unauthorized"))
-        line_object_dict = root.line.__dict__
-        line_object_dict.pop('_state')
-        key_values = list(line_object_dict.items())
-        line_object_dict.clear()
-        for k, v in key_values:
-            new_key = underscore_to_camel(k)
-            line_object_dict[new_key] = v
-        line_object_dict = json.dumps(line_object_dict, cls=DjangoJSONEncoder)
-        return line_object_dict
-
-    class Meta:
-        model = InvoiceLineItem
-        interfaces = (graphene.relay.Node,)
-        filter_fields = {
-            **GenericFilterGQLTypeMixin.get_base_filters_invoice_line_item(),
-            **prefix_filterset("invoice__", InvoiceGQLType._meta.filter_fields),
-        }
-
-        connection_class = ExtendedConnection
-
-        @classmethod
-        def get_queryset(cls, queryset, info):
-            return InvoiceLineItem.get_queryset(queryset, info)
-
-
-class InvoicePaymentGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
-
-    class Meta:
-        model = InvoicePayment
-        interfaces = (graphene.relay.Node,)
-        filter_fields = {
-            **GenericFilterGQLTypeMixin.get_base_filters_invoice_payment(),
-            **prefix_filterset("invoice__", InvoiceGQLType._meta.filter_fields),
-        }
-
-        connection_class = ExtendedConnection
-
-        @classmethod
-        def get_queryset(cls, queryset, info):
-            return InvoicePayment.get_queryset(queryset, info)
-
-
-class InvoiceEventGQLType(DjangoObjectType, GenericFilterGQLTypeMixin):
-
-    class Meta:
-        model = InvoiceEvent
-        interfaces = (graphene.relay.Node,)
-        filter_fields = {
-            **GenericFilterGQLTypeMixin.get_base_filters_invoice_event(),
-            **prefix_filterset("invoice__", InvoiceGQLType._meta.filter_fields),
-        }
-
-        connection_class = ExtendedConnection
-
-        @classmethod
-        def get_queryset(cls, queryset, info):
-            return InvoiceEvent.get_queryset(queryset, info)
-
-
-class InvoiceMutationGQLType(DjangoObjectType):
-    class Meta:
-        model = InvoiceMutation
-
-
-class InvoicePaymentMutationGQLType(DjangoObjectType):
-    class Meta:
-        model = InvoicePaymentMutation
-
-
-class InvoiceLineItemMutationGQLType(DjangoObjectType):
-    class Meta:
-        model = InvoiceLineItemMutation
-
-
-class InvoiceEventMutationGQLType(DjangoObjectType):
-    class Meta:
-        model = InvoiceEventMutation
+            response = self.line_item_service.create(payload)
+            response = self.line_item_service.delete(response['data'])
+            self.assertDictEqual(expected_response, response)
+            InvoiceLineItem.objects.filter(code=payload['code']).delete()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/gql_types/payment_types.py` & `openimis_be_invoice-1.7.0/invoice/gql/gql_types/payment_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/input_types.py` & `openimis_be_invoice-1.7.0/invoice/gql/input_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/invoice/mutation.py` & `openimis_be_invoice-1.7.0/invoice/gql/invoice/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/invoice/query.py` & `openimis_be_invoice-1.7.0/invoice/gql/invoice/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String()
     )
 
     def resolve_invoice(self, info, **kwargs):
+        InvoiceQueryMixin._check_permissions(info.context.user)
         filters = []
         filters += append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
@@ -32,18 +33,18 @@
         if subject_type:
             filters.append(Q(subject_type__model=subject_type))
 
         thirdparty_type = kwargs.get("thirdparty_type", None)
         if thirdparty_type:
             filters.append(Q(thirdparty_type__model=thirdparty_type))
 
-        InvoiceQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(Invoice.objects.filter(*filters).all(), info)
+        qs = Invoice.objects.filter(*filters)
+        if InvoiceConfig.invoice_user_filter:
+            qs = InvoiceConfig.invoice_user_filter(qs, info.context.user)
+
+        return gql_optimizer.query(qs, info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 InvoiceConfig.gql_invoice_search_perms):
             raise PermissionError("Unauthorized")
-
-
-
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/invoice_event/mutation.py` & `openimis_be_invoice-1.7.0/invoice/gql/invoice_event/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/invoice_event/query.py` & `openimis_be_invoice-1.7.0/invoice/gql/invoice_event/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,39 +2,43 @@
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
 from invoice.gql.gql_types.invoice_types import InvoiceEventGQLType
-from invoice.models import InvoiceEvent
+from invoice.models import InvoiceEvent, Invoice
 import graphene_django_optimizer as gql_optimizer
 
 
 class InvoiceEventQueryMixin:
     invoice_event = OrderedDjangoFilterConnectionField(
         InvoiceEventGQLType,
         orderBy=graphene.List(of_type=graphene.String),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String(),
     )
 
     def resolve_invoice_event(self, info, **kwargs):
+        InvoiceEventQueryMixin._check_permissions(info.context.user)
         filters = []
         filters += append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
-        InvoiceEventQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(InvoiceEvent.objects.filter(*filters).all(), info)
+        invoice_event_qs = InvoiceEvent.objects.filter(*filters)
+
+        if InvoiceConfig.invoice_user_filter:
+            invoice_qs = InvoiceConfig.invoice_user_filter(Invoice.objects.all(), info.context.user)
+            invoice_event_qs = invoice_event_qs.filter(invoice__in=invoice_qs)
+
+        return gql_optimizer.query(invoice_event_qs, info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 InvoiceConfig.gql_invoice_event_search_perms):
             raise PermissionError("Unauthorized")
-
-
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/invoice_line_item/query.py` & `openimis_be_invoice-1.7.0/invoice/gql/invoice_line_item/query.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,41 +2,47 @@
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
 from invoice.gql.gql_types.invoice_types import InvoiceLineItemGQLType
-from invoice.models import InvoiceLineItem
+from invoice.models import InvoiceLineItem, Invoice
 import graphene_django_optimizer as gql_optimizer
 
 
 class InvoiceLineItemQueryMixin:
     invoice_line_item = OrderedDjangoFilterConnectionField(
         InvoiceLineItemGQLType,
         orderBy=graphene.List(of_type=graphene.String),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String(),
     )
 
     def resolve_invoice_line_item(self, info, **kwargs):
+        InvoiceLineItemQueryMixin._check_invoice_permissions(info.context.user)
         filters = []
         filters += append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
         line_type = kwargs.get("line_type", None)
         if line_type:
             filters.append(Q(line_type__model=line_type))
 
-        InvoiceLineItemQueryMixin._check_invoice_permissions(info.context.user)
-        return gql_optimizer.query(InvoiceLineItem.objects.filter(*filters).all(), info)
+        invoice_li_qs = InvoiceLineItem.objects.filter(*filters)
+
+        if InvoiceConfig.invoice_user_filter:
+            invoice_qs = InvoiceConfig.invoice_user_filter(Invoice.objects.all(), info.context.user)
+            invoice_li_qs = invoice_li_qs.filter(invoice__in=invoice_qs)
+
+        return gql_optimizer.query(invoice_li_qs, info)
 
     @staticmethod
     def _check_invoice_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 InvoiceConfig.gql_invoice_search_perms):
             raise PermissionError("Unauthorized")
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/invoice_payment/mutation.py` & `openimis_be_invoice-1.7.0/invoice/gql/invoice_payment/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/invoice_payment/query.py` & `openimis_be_invoice-1.7.0/invoice/gql/payment_invoice/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 import graphene
+import graphene_django_optimizer as gql_optimizer
+
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
-from invoice.gql.gql_types.invoice_types import InvoicePaymentGQLType
-from invoice.models import InvoicePayment
-import graphene_django_optimizer as gql_optimizer
+from invoice.gql.gql_types.payment_types import PaymentInvoiceGQLType
+from invoice.models import PaymentInvoice
 
 
-class InvoicePaymentQueryMixin:
-    invoice_payment = OrderedDjangoFilterConnectionField(
-        InvoicePaymentGQLType,
+class PaymentInvoiceQueryMixin:
+    payment_invoice = OrderedDjangoFilterConnectionField(
+        PaymentInvoiceGQLType,
         orderBy=graphene.List(of_type=graphene.String),
+        subjectIds=graphene.List(of_type=graphene.UUID),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String(),
     )
 
-    def resolve_invoice_payment(self, info, **kwargs):
+    def resolve_payment_invoice(self, info, **kwargs):
         filters = []
         filters += append_validity_filter(**kwargs)
 
+        query = PaymentInvoice.objects
+
+        subject_ids = kwargs.get('subjectIds', None)
+        if subject_ids:
+            query = query.filter(
+                invoice_payments__subject_id__in=subject_ids
+            ).distinct()
+
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
-        InvoicePaymentQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(InvoicePayment.objects.filter(*filters).all(), info)
+        PaymentInvoiceQueryMixin._check_permissions(info.context.user)
+        return gql_optimizer.query(query.filter(*filters).all(), info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 InvoiceConfig.gql_invoice_payment_search_perms):
             raise PermissionError("Unauthorized")
-
-
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/payment_invoice/mutation.py` & `openimis_be_invoice-1.7.0/invoice/gql/payment_invoice/mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/payment_invoice/query.py` & `openimis_be_invoice-1.7.0/invoice/gql/bill_payment/query.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 import graphene
-import graphene_django_optimizer as gql_optimizer
-
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from invoice.apps import InvoiceConfig
-from invoice.gql.gql_types.payment_types import PaymentInvoiceGQLType
-from invoice.models import PaymentInvoice
+from invoice.gql.gql_types.bill_types import BillPaymentGQLType
+from invoice.models import BillPayment, Bill
+import graphene_django_optimizer as gql_optimizer
 
 
-class PaymentInvoiceQueryMixin:
-    payment_invoice = OrderedDjangoFilterConnectionField(
-        PaymentInvoiceGQLType,
+class BillPaymentQueryMixin:
+    bill_payment = OrderedDjangoFilterConnectionField(
+        BillPaymentGQLType,
         orderBy=graphene.List(of_type=graphene.String),
-        subjectIds=graphene.List(of_type=graphene.UUID),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String(),
     )
 
-    def resolve_payment_invoice(self, info, **kwargs):
+    def resolve_bill_payment(self, info, **kwargs):
         filters = []
         filters += append_validity_filter(**kwargs)
 
-        query = PaymentInvoice.objects
-
-        subject_ids = kwargs.get('subjectIds', None)
-        if subject_ids:
-            query = query.filter(
-                invoice_payments__subject_id__in=subject_ids
-            ).distinct()
-
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
-        PaymentInvoiceQueryMixin._check_permissions(info.context.user)
-        return gql_optimizer.query(query.filter(*filters).all(), info)
+        bill_payment_qs = BillPayment.objects.filter(*filters)
+
+        if InvoiceConfig.bill_user_filter:
+            bill_qs = InvoiceConfig.bill_user_filter(Bill.objects.all(), info.context.user)
+            bill_payment_qs = bill_payment_qs.filter(bill__in=bill_qs)
+
+        return gql_optimizer.query(bill_payment_qs, info)
 
     @staticmethod
     def _check_permissions(user):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
-                InvoiceConfig.gql_invoice_payment_search_perms):
+                InvoiceConfig.gql_bill_payment_search_perms):
             raise PermissionError("Unauthorized")
```

### Comparing `openimis-be-invoice-1.6.0/invoice/gql/query_mixins.py` & `openimis_be_invoice-1.7.0/invoice/gql/query_mixins.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0001_initial_migration.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0001_initial_migration.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0002_auto_20211117_0904.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0002_auto_20211117_0904.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0003_auto_20211203_1053.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0003_auto_20211203_1053.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0004_invoice_bill_roles_for_admin.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0004_invoice_bill_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0005_invoice_bill_roles_for_accountant.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0005_invoice_bill_roles_for_accountant.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0006_detailpaymentinvoice_historicaldetailpaymentinvoice_historicalpaymentinvoice_paymentinvoice.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0006_detailpaymentinvoice_historicaldetailpaymentinvoice_historicalpaymentinvoice_paymentinvoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0007_auto_20220411_1053.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0007_auto_20220411_1053.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0008_auto_20220411_1358.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0008_auto_20220411_1358.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0009_auto_20220413_0824.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0009_auto_20220413_0824.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0010_auto_20230126_0903.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0010_auto_20230126_0903.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0011_auto_20230914_0805.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0011_auto_20230914_0805.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/migrations/0012_auto_20230921_0835.py` & `openimis_be_invoice-1.7.0/invoice/migrations/0012_auto_20230921_0835.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/mixins.py` & `openimis_be_invoice-1.7.0/invoice/mixins.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/models.py` & `openimis_be_invoice-1.7.0/invoice/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,73 +23,73 @@
         CANCELLED = 3, _('cancelled')
         DELETED = 4, _('deleted')
         SUSPENDED = 5, _('suspended')
         UNPAID = 6, _('unpaid')
         RECONCILIATED = 7, _('reconciliated')
 
     thirdparty_type = models.ForeignKey(ContentType, models.DO_NOTHING,
-                                          db_column='ThirdpartyType', null=True, unique=False)
-    thirdparty_id = models.CharField(db_column='ThirdpartyId', max_length=255, null=True)  # object is referenced by uuid
+                                          db_column='ThirdpartyType', blank=True, null=True, unique=False)
+    thirdparty_id = models.CharField(db_column='ThirdpartyId', max_length=255, blank=True, null=True)  # object is referenced by uuid
     thirdparty = GenericForeignKey('thirdparty_type', 'thirdparty_id')
 
-    code_tp = models.CharField(db_column='CodeTp', max_length=255, null=True)
+    code_tp = models.CharField(db_column='CodeTp', max_length=255, blank=True, null=True)
     code = models.CharField(db_column='Code', max_length=255, null=False)
-    code_ext = models.CharField(db_column='CodeExt', max_length=255, null=True)
+    code_ext = models.CharField(db_column='CodeExt', max_length=255, blank=True, null=True)
 
-    date_due = DateField(db_column='DateDue', null=True)
+    date_due = DateField(db_column='DateDue', blank=True, null=True)
 
-    date_payed = DateField(db_column='DatePayed', null=True)
+    date_payed = DateField(db_column='DatePayed', blank=True, null=True)
 
     amount_discount = models.DecimalField(
-        db_column='AmountDiscount', max_digits=18, decimal_places=2, null=True, default=0.0)
+        db_column='AmountDiscount', max_digits=18, decimal_places=2,  null=True, default=0.0)
     amount_net = models.DecimalField(
         db_column='AmountNet', max_digits=18, decimal_places=2, default=0.0)
     amount_total = models.DecimalField(
         db_column='AmountTotal', max_digits=18, decimal_places=2, default=0.0)
 
-    tax_analysis = models.JSONField(db_column='TaxAnalysis', null=True)
+    tax_analysis = models.JSONField(db_column='TaxAnalysis', blank=True, null=True)
 
     status = models.SmallIntegerField(
         db_column='Status', null=False, choices=Status.choices, default=Status.DRAFT)
 
     currency_tp_code = models.CharField(
         db_column='CurrencyTpCode', null=False, max_length=255, default=get_default_currency)
     currency_code = models.CharField(
         db_column='CurrencyCode', null=False, max_length=255, default=get_default_currency)
 
     note = models.TextField(db_column='Note', blank=True, null=True)
     terms = models.TextField(db_column='Terms', blank=True, null=True)
 
-    payment_reference = models.CharField(db_column='PaymentReference', max_length=255, null=True)
+    payment_reference = models.CharField(db_column='PaymentReference', max_length=255, blank=True, null=True)
 
     objects = GenericInvoiceManager()
 
     class Meta:
         abstract = True
 
 
 class GenericInvoiceLineItem(GenericInvoiceQuerysetMixin, HistoryBusinessModel):
     code = models.CharField(db_column='Code', max_length=255, null=False)
 
     description = models.TextField(db_column='Description', blank=True, null=True)
-    details = models.JSONField(db_column='Details', null=True)
+    details = models.JSONField(db_column='Details', blank=True, null=True)
 
-    ledger_account = models.CharField(db_column='LedgerAccount', max_length=255, null=True)
+    ledger_account = models.CharField(db_column='LedgerAccount', max_length=255, blank=True, null=True)
 
     quantity = models.IntegerField(db_column='Quantity', default=0.0)
     unit_price = models.DecimalField(db_column='UnitPrice', max_digits=18, decimal_places=2, default=0.0)
 
     discount = models.DecimalField(db_column='Discount', max_digits=18, decimal_places=2, default=0.0)
 
     deduction = models.DecimalField(db_column='Deduction', max_digits=18, decimal_places=2, default=0.0)
 
-    tax_rate = models.UUIDField(db_column="CalculationUUID", null=True)
-    tax_analysis = models.JSONField(db_column='TaxAnalysis', null=True)
+    tax_rate = models.UUIDField(db_column="CalculationUUID", blank=True, null=True)
+    tax_analysis = models.JSONField(db_column='TaxAnalysis',  blank=True, null=True)
 
-    amount_total = models.DecimalField(db_column='AmountTotal', max_digits=18, decimal_places=2, null=True)
+    amount_total = models.DecimalField(db_column='AmountTotal', max_digits=18, decimal_places=2, default=0.0)
     amount_net = models.DecimalField(db_column='AmountNet', max_digits=18, decimal_places=2, default=0.0)
 
     objects = GenericInvoiceManager()
 
     class Meta:
         abstract = True
 
@@ -97,29 +97,29 @@
 class GenericInvoicePayment(GenericInvoiceQuerysetMixin, HistoryModel):
     class PaymentStatus(models.IntegerChoices):
         REJECTED = 0, _('rejected')
         ACCEPTED = 1, _('accepted')
         REFUNDED = 2, _('refunded')
         CANCELLED = 3, _('cancelled')
 
-    code_tp = models.CharField(db_column='CodeTp', max_length=255, null=True)
-    code_ext = models.CharField(db_column='CodeExt', max_length=255, null=True)
-    code_receipt = models.CharField(db_column='CodeReceipt', max_length=255, null=True)
+    code_tp = models.CharField(db_column='CodeTp', max_length=255, blank=True, null=True)
+    code_ext = models.CharField(db_column='CodeExt', max_length=255, blank=True, null=True)
+    code_receipt = models.CharField(db_column='CodeReceipt', max_length=255, blank=True, null=True)
 
-    label = models.CharField(db_column='Label', max_length=255, null=True)
+    label = models.CharField(db_column='Label', max_length=255,  blank=True, null=True)
 
     status = models.SmallIntegerField(db_column='Status', null=False, choices=PaymentStatus.choices)
 
-    amount_payed = models.DecimalField(db_column='AmountPayed', max_digits=18, decimal_places=2, null=True)
-    fees = models.DecimalField(db_column='Fees', max_digits=18, decimal_places=2, null=True)
-    amount_received = models.DecimalField(db_column='AmountReceived', max_digits=18, decimal_places=2, null=True)
+    amount_payed = models.DecimalField(db_column='AmountPayed', max_digits=18, decimal_places=2,  blank=True, null=True)
+    fees = models.DecimalField(db_column='Fees', max_digits=18, decimal_places=2,  blank=True, null=True)
+    amount_received = models.DecimalField(db_column='AmountReceived', max_digits=18, decimal_places=2,  blank=True, null=True)
 
-    date_payment = DateField(db_column='DatePayment', null=True)
+    date_payment = DateField(db_column='DatePayment',  blank=True, null=True)
 
-    payment_origin = models.CharField(db_column='PaymentOrigin', max_length=255, null=True)
+    payment_origin = models.CharField(db_column='PaymentOrigin', max_length=255,  blank=True, null=True)
 
     objects = GenericInvoiceManager()
 
     class Meta:
         abstract = True
 
 
@@ -127,41 +127,41 @@
     class EventType(models.IntegerChoices):
         MESSAGE = 0, _('message')
         STATUS = 1, _('status')
         WARNING = 2, _('warning')
         PAYMENT = 3, _('payment')
         PAYMENT_ERROR = 4, _('payment_error')
 
-    message = models.CharField(db_column='Message', max_length=500, null=True)
+    message = models.CharField(db_column='Message', max_length=500,  blank=True, null=True)
     event_type = models.SmallIntegerField(
         db_column='Status', null=False, choices=EventType.choices, default=EventType.MESSAGE)
 
     objects = GenericInvoiceManager()
 
     class Meta:
         abstract = True
 
 
 class Invoice(GenericInvoice):
     subject_type = models.ForeignKey(ContentType, models.DO_NOTHING,
-                                        db_column='SubjectType', null=True, related_name='subject_type', unique=False)
-    subject_id = models.CharField(db_column='SubjectId', max_length=255, null=True)  # object is referenced by uuid
+                                        db_column='SubjectType',  blank=True, null=True, related_name='subject_type', unique=False)
+    subject_id = models.CharField(db_column='SubjectId', max_length=255,  blank=True, null=True)  # object is referenced by uuid
     subject = GenericForeignKey('subject_type', 'subject_id')
 
-    date_invoice = DateField(db_column='DateInvoice', default=date.today, null=True)
+    date_invoice = DateField(db_column='DateInvoice', default=date.today,  blank=True, null=True)
 
     class Meta:
         managed = True
         db_table = 'tblInvoice'
 
 
 class InvoiceLineItem(GenericInvoiceLineItem):
     line_type = models.ForeignKey(
-        ContentType, models.DO_NOTHING, db_column='LineType', null=True, related_name='line_type', unique=False)
-    line_id = models.CharField(db_column='LineId', max_length=255, null=True)  # object is referenced by uuid
+        ContentType, models.DO_NOTHING, db_column='LineType',  blank=True, null=True, related_name='line_type', unique=False)
+    line_id = models.CharField(db_column='LineId', max_length=255,  blank=True, null=True)  # object is referenced by uuid
     line = GenericForeignKey('line_type', 'line_id')
 
     invoice = models.ForeignKey(Invoice, models.DO_NOTHING, db_column='InvoiceId', related_name="line_items")
 
     class Meta:
         managed = True
         db_table = 'tblInvoiceLineItem'
@@ -181,30 +181,30 @@
     class Meta:
         managed = True
         db_table = 'tblInvoiceEvent'
 
 
 class Bill(GenericInvoice):
     subject_type = models.ForeignKey(ContentType, models.DO_NOTHING,
-                                        db_column='SubjectType', null=True, related_name='subject_type_bill',
+                                        db_column='SubjectType', null=True,blank=True, related_name='subject_type_bill',
                                      unique=False)
-    subject_id = models.CharField(db_column='SubjectId', max_length=255, null=True)  # object is referenced by uuid
+    subject_id = models.CharField(db_column='SubjectId', max_length=255, blank=True, null=True)  # object is referenced by uuid
     subject = GenericForeignKey('subject_type', 'subject_id')
 
-    date_bill = DateField(db_column='DateBill', default=date.today, null=True)
+    date_bill = DateField(db_column='DateBill', default=date.today,blank=True, null=True)
 
     class Meta:
         managed = True
         db_table = 'tblBill'
 
 
 class BillItem(GenericInvoiceLineItem):
     line_type = models.ForeignKey(
-        ContentType, models.DO_NOTHING, db_column='LineType', null=True, related_name='line_type_bill', unique=False)
-    line_id = models.CharField(db_column='LineId', max_length=255, null=True)  # object is referenced by uuid
+        ContentType, models.DO_NOTHING, db_column='LineType',  blank=True, null=True, related_name='line_type_bill', unique=False)
+    line_id = models.CharField(db_column='LineId', max_length=255,  blank=True, null=True)  # object is referenced by uuid
     line = GenericForeignKey('line_type', 'line_id')
 
     bill = models.ForeignKey(Bill, models.DO_NOTHING, db_column='BillId', related_name="line_items_bill")
 
     class Meta:
         managed = True
         db_table = 'tblBillLineItem'
@@ -302,32 +302,32 @@
 class PaymentInvoice(GenericInvoiceQuerysetMixin, HistoryModel):
     class ReconciliationStatus(models.IntegerChoices):
         NOT_RECONCILIATED = 0, _('not reconciliated')
         RECONCILIATED = 1, _('reconciliated')
         REFUNDED = 2, _('refunded')
         CANCELLED = 3, _('cancelled')
 
-    code_tp = models.CharField(db_column='CodeTp', max_length=255, null=True)
-    code_ext = models.CharField(db_column='CodeExt', max_length=255, null=True)
-    code_receipt = models.CharField(db_column='CodeReceipt', max_length=255, null=True)
+    code_tp = models.CharField(db_column='CodeTp', max_length=255,  blank=True, null=True)
+    code_ext = models.CharField(db_column='CodeExt', max_length=255,  blank=True, null=True)
+    code_receipt = models.CharField(db_column='CodeReceipt', max_length=255,  blank=True, null=True)
 
-    label = models.CharField(db_column='Label', max_length=255, null=True)
+    label = models.CharField(db_column='Label', max_length=255,  blank=True, null=True)
 
     reconciliation_status = models.SmallIntegerField(db_column='ReconciliationStatus', null=False,
                                                      choices=ReconciliationStatus.choices)
 
-    fees = models.DecimalField(db_column='Fees', max_digits=18, decimal_places=2, null=True)
-    amount_received = models.DecimalField(db_column='AmountReceived', max_digits=18, decimal_places=2, null=True)
+    fees = models.DecimalField(db_column='Fees', max_digits=18, decimal_places=2,  blank=True, null=True)
+    amount_received = models.DecimalField(db_column='AmountReceived', max_digits=18, decimal_places=2,  blank=True, null=True)
 
-    date_payment = DateField(db_column='DatePayment', null=True)
+    date_payment = DateField(db_column='DatePayment',  blank=True, null=True)
 
-    payment_origin = models.CharField(db_column='PaymentOrigin', max_length=255, null=True)
+    payment_origin = models.CharField(db_column='PaymentOrigin', max_length=255,  blank=True, null=True)
 
     payer_ref = models.CharField(db_column='PayerRef', max_length=255)
-    payer_name = models.CharField(db_column='PayerName', max_length=255, null=True)
+    payer_name = models.CharField(db_column='PayerName', max_length=255,  blank=True, null=True)
 
     objects = GenericInvoiceManager()
 
     class Meta:
         managed = True
         db_table = "tblPaymentInvoice"
 
@@ -339,24 +339,24 @@
         REFUNDED = 2, _('refunded')
         CANCELLED = 3, _('cancelled')
 
     payment = models.ForeignKey(PaymentInvoice, models.DO_NOTHING,
                                 db_column='PaymentUUID', related_name="invoice_payments")
 
     subject_type = models.ForeignKey(ContentType, models.DO_NOTHING, db_column='SubjectType',
-                                     related_name='subject_type_payment', null=True, unique=False)
-    subject_id = models.CharField(db_column='SubjectId', max_length=255, null=True)
+                                     related_name='subject_type_payment',  blank=True, null=True, unique=False)
+    subject_id = models.CharField(db_column='SubjectId', max_length=255,  blank=True, null=True)
     subject = GenericForeignKey('subject_type', 'subject_id')
 
     status = models.SmallIntegerField(db_column='Status', null=False, choices=DetailPaymentStatus.choices)
-    fees = models.DecimalField(db_column='Fees', max_digits=18, decimal_places=2, null=True)
-    amount = models.DecimalField(db_column='Amount', max_digits=18, decimal_places=2, null=True)
+    fees = models.DecimalField(db_column='Fees', max_digits=18, decimal_places=2,  blank=True, null=True)
+    amount = models.DecimalField(db_column='Amount', max_digits=18, decimal_places=2,  blank=True, null=True)
 
-    reconcilation_id = models.CharField(db_column='ReconcilationId', max_length=255, null=True)
-    reconcilation_date = models.DateField(db_column='ReconcilationDate', null=True)
+    reconcilation_id = models.CharField(db_column='ReconcilationId', max_length=255,  blank=True, null=True)
+    reconcilation_date = models.DateField(db_column='ReconcilationDate',  blank=True, null=True)
 
     objects = GenericInvoiceManager()
 
     class Meta:
         managed = True
         db_table = "tblDetailPaymentInvoice"
```

### Comparing `openimis-be-invoice-1.6.0/invoice/schema.py` & `openimis_be_invoice-1.7.0/invoice/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/services/bill.py` & `openimis_be_invoice-1.7.0/invoice/services/bill.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import decimal
 from typing import Union, List
 
 from invoice.models import Bill, BillItem
 from core.services import BaseService
 from invoice.services.billLineItem import BillLineItemService
 from core.services.utils import get_generic_type
 from invoice.validation.bill import BillModelValidation, BillItemStatus
 from core.signals import *
 
 
 class BillService(BaseService):
-
     OBJECT_TYPE = Bill
 
     def __init__(self, user, validation_class: BillModelValidation = BillModelValidation):
         super().__init__(user, validation_class)
         self.validation_class = validation_class
 
     def _base_payload_adjust(self, bill_data):
@@ -51,25 +51,27 @@
             bill_line_items = convert_results['bill_data_line']
             bill_service = BillService(user=user)
             bill_line_item_service = BillLineItemService(user=user)
             result_bill = bill_service.create(convert_results['bill_data'])
             if result_bill["success"] is True:
                 bill_update = {
                     "id": result_bill["data"]["id"],
-                    "amount_net": 0,
-                    "amount_total": 0,
-                    "amount_discount": 0
+                    "amount_net": decimal.Decimal(0),
+                    "amount_total": decimal.Decimal(0),
+                    "amount_discount": decimal.Decimal(0),
                 }
                 for bill_line_item in bill_line_items:
                     bill_line_item["bill_id"] = result_bill["data"]["id"]
                     result_bill_line = bill_line_item_service.create(bill_line_item)
                     if result_bill_line["success"] is True:
-                        bill_update["amount_net"] += float(result_bill_line["data"]["amount_net"])
-                        bill_update["amount_total"] += float(result_bill_line["data"]["amount_total"])
-                        bill_update["amount_discount"] += 0 if result_bill_line["data"]["discount"] else result_bill_line["data"]["discount"]
+                        bill_update["amount_net"] += decimal.Decimal(result_bill_line["data"]["amount_net"])
+                        bill_update["amount_total"] += decimal.Decimal(result_bill_line["data"]["amount_total"])
+                        bill_update["amount_discount"] += decimal.Decimal(0) \
+                            if not result_bill_line["data"]["discount"] \
+                            else decimal.Decimal(result_bill_line["data"]["discount"])
                 generated_bill = bill_service.update(bill_update)
                 return generated_bill
 
     def _evaluate_generic_types(self, bill_data):
         if 'subject_type' in bill_data.keys():
             bill_data['subject_type'] = get_generic_type(bill_data['subject_type'])
```

### Comparing `openimis-be-invoice-1.6.0/invoice/services/billLineItem.py` & `openimis_be_invoice-1.7.0/invoice/services/billLineItem.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/services/invoice.py` & `openimis_be_invoice-1.7.0/invoice/services/invoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/services/invoiceLineItem.py` & `openimis_be_invoice-1.7.0/invoice/services/invoiceLineItem.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/services/invoicePayments.py` & `openimis_be_invoice-1.7.0/invoice/services/invoicePayments.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/services/paymentInvoice.py` & `openimis_be_invoice-1.7.0/invoice/services/paymentInvoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/signals.py` & `openimis_be_invoice-1.7.0/invoice/signals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/gql/base.py` & `openimis_be_invoice-1.7.0/invoice/tests/gql/base.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/gql/detail_payment_invoice_schema.py` & `openimis_be_invoice-1.7.0/invoice/tests/gql/detail_payment_invoice_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/gql/invoice_event_schema.py` & `openimis_be_invoice-1.7.0/invoice/tests/gql/invoice_event_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/gql/invoice_line_item_schema.py` & `openimis_be_invoice-1.7.0/invoice/tests/gql/invoice_line_item_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/gql/invoice_payment_schema.py` & `openimis_be_invoice-1.7.0/invoice/tests/gql/invoice_payment_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/gql/invoice_schema.py` & `openimis_be_invoice-1.7.0/invoice/tests/gql/invoice_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/gql/payment_invoice_schema.py` & `openimis_be_invoice-1.7.0/invoice/tests/gql/payment_invoice_schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/helpers/__init__.py` & `openimis_be_invoice-1.7.0/invoice/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/helpers/bill_helpers.py` & `openimis_be_invoice-1.7.0/invoice/tests/helpers/bill_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/helpers/bill_line_item_helpers.py` & `openimis_be_invoice-1.7.0/invoice/tests/helpers/bill_line_item_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/helpers/bill_payment_helpers.py` & `openimis_be_invoice-1.7.0/invoice/tests/helpers/bill_payment_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/helpers/default_test_data.py` & `openimis_be_invoice-1.7.0/invoice/tests/helpers/default_test_data.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/helpers/invoice_helpers.py` & `openimis_be_invoice-1.7.0/invoice/tests/helpers/invoice_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/helpers/invoice_line_item_helpers.py` & `openimis_be_invoice-1.7.0/invoice/tests/helpers/invoice_line_item_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/helpers/invoice_payment_helpers.py` & `openimis_be_invoice-1.7.0/invoice/tests/helpers/invoice_payment_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/helpers/payment_invoice_helpers.py` & `openimis_be_invoice-1.7.0/invoice/tests/helpers/payment_invoice_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/helpers.py` & `openimis_be_invoice-1.7.0/invoice/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/services/invoice.py` & `openimis_be_invoice-1.7.0/invoice/tests/services/invoice.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import date, datetime, timedelta
 
 from django.db import transaction
 from django.test import TestCase
 
 from contract.tests.helpers import create_test_contract
 from core.forms import User
+from core.test_helpers import compare_dicts
 from insuree.test_helpers import create_test_insuree
 from invoice.models import Invoice, InvoiceLineItem, InvoicePayment
 from invoice.services import InvoiceService
 from invoice.tests.helpers import create_test_invoice_line_item
 from invoice.validation import TaxAnalysisFormatValidationMixin, InvoiceItemStatus
 from policy.test_helpers import create_test_policy
 from policyholder.tests.helpers import create_test_policy_holder
@@ -149,15 +150,15 @@
             truncated_output['data'] = {k: v for k, v in truncated_output['data'].items()
                                         if k in expected_response['data'].keys()}
 
             invoice = Invoice.objects.filter(code=payload['code']).first()
             expected_response['data']['subject_type'] = invoice.subject_type.id
             expected_response['data']['thirdparty_type'] = invoice.thirdparty_type.id
 
-            self.assertDictEqual(expected_response, response)
+            self.assertTrue(compare_dicts(expected_response, response))
             Invoice.objects.filter(code=payload['code']).delete()
 
     def test_invoice_update(self):
         with transaction.atomic():
             create_payload = self.BASE_TEST_INVOICE_PAYLOAD.copy()
             update_payload = self.BASE_TEST_UPDATE_INVOICE_PAYLOAD.copy()
             expected_response = self.BASE_EXPECTED_UPDATE_RESPONSE.copy()
@@ -171,15 +172,15 @@
             truncated_output = response
             truncated_output['data'] = {k: v for k, v in truncated_output['data'].items()
                                         if k in expected_response['data'].keys()}
 
             invoice = Invoice.objects.filter(code=update_payload['code']).first()
 
             expected_response['data']['thirdparty_type'] = invoice.thirdparty_type.id
-            self.assertDictEqual(expected_response, response)
+            self.assertTrue(compare_dicts(expected_response, response))
 
             Invoice.objects.filter(code=update_payload['code']).delete()
 
     def test_invoice_delete(self):
         with transaction.atomic():
             payload = self.BASE_TEST_INVOICE_PAYLOAD.copy()
             expected_response = {
```

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/services/invoicePayment.py` & `openimis_be_invoice-1.7.0/invoice/tests/services/invoicePayment.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/tests/services/paymentInvoice.py` & `openimis_be_invoice-1.7.0/invoice/tests/services/paymentInvoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/utils.py` & `openimis_be_invoice-1.7.0/invoice/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/validation/base.py` & `openimis_be_invoice-1.7.0/invoice/validation/base.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/validation/bill.py` & `openimis_be_invoice-1.7.0/invoice/validation/bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/validation/invoice.py` & `openimis_be_invoice-1.7.0/invoice/validation/invoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/validation/invoicePayment.py` & `openimis_be_invoice-1.7.0/invoice/validation/invoicePayment.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/validation/paymentInvoice.py` & `openimis_be_invoice-1.7.0/invoice/validation/paymentInvoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/invoice/validation/paymentStatusValidation.py` & `openimis_be_invoice-1.7.0/invoice/validation/paymentStatusValidation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-invoice-1.6.0/openimis_be_invoice.egg-info/PKG-INFO` & `openimis_be_invoice-1.7.0/openimis_be_invoice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-invoice
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Invoice Payment reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-invoice-1.6.0/openimis_be_invoice.egg-info/SOURCES.txt` & `openimis_be_invoice-1.7.0/openimis_be_invoice.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 invoice/migrations/0006_detailpaymentinvoice_historicaldetailpaymentinvoice_historicalpaymentinvoice_paymentinvoice.py
 invoice/migrations/0007_auto_20220411_1053.py
 invoice/migrations/0008_auto_20220411_1358.py
 invoice/migrations/0009_auto_20220413_0824.py
 invoice/migrations/0010_auto_20230126_0903.py
 invoice/migrations/0011_auto_20230914_0805.py
 invoice/migrations/0012_auto_20230921_0835.py
+invoice/migrations/0013_alter_bill_code_ext_alter_bill_code_tp_and_more.py
 invoice/migrations/__init__.py
 invoice/services/__init__.py
 invoice/services/bill.py
 invoice/services/billLineItem.py
 invoice/services/invoice.py
 invoice/services/invoiceLineItem.py
 invoice/services/invoicePayments.py
```

### Comparing `openimis-be-invoice-1.6.0/setup.py` & `openimis_be_invoice-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-invoice',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Invoice Payment reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

