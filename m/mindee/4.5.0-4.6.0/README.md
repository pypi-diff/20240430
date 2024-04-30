# Comparing `tmp/mindee-4.5.0.tar.gz` & `tmp/mindee-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindee-4.5.0.tar", last modified: Fri Mar 15 14:12:25 2024, max compression
+gzip compressed data, was "mindee-4.6.0.tar", last modified: Tue Apr 30 16:18:17 2024, max compression
```

## Comparing `mindee-4.5.0.tar` & `mindee-4.6.0.tar`

### file list

```diff
@@ -1,336 +1,336 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.128172 mindee-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-15 14:12:07.000000 mindee-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-03-15 14:12:25.128172 mindee-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-03-15 14:12:07.000000 mindee-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.084173 mindee-4.5.0/mindee/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.088173 mindee-4.5.0/mindee/error/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/error/geometry_error.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/error/mimetype_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/error/mindee_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/error/mindee_http_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.088173 mindee-4.5.0/mindee/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/geometry/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/geometry/minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/geometry/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/geometry/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/geometry/polygon_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/geometry/quadrilateral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.088173 mindee-4.5.0/mindee/input/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/input/page_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/input/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.092173 mindee-4.5.0/mindee/mindee_http/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/mindee_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/mindee_http/base_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/mindee_http/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/mindee_http/mindee_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/mindee_http/response_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.092173 mindee-4.5.0/mindee/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.092173 mindee-4.5.0/mindee/parsing/common/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/async_predict_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.092173 mindee-4.5.0/mindee/parsing/common/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/extras/cropper_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/extras/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/feedback_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.096173 mindee-4.5.0/mindee/parsing/common/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/ocr/mvision_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/ocr/ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/ocr/ocr_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/ocr/ocr_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/ocr/ocr_word.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/predict_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/product.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/string_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/common/summary_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.096173 mindee-4.5.0/mindee/parsing/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/custom/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/custom/line_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/custom/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.096173 mindee-4.5.0/mindee/parsing/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/generated/generated_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/generated/generated_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.096173 mindee-4.5.0/mindee/parsing/standard/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/company_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/payment_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/position.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/parsing/standard/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.096173 mindee-4.5.0/mindee/product/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.100173 mindee-4.5.0/mindee/product/barcode_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/barcode_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/barcode_reader/barcode_reader_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/barcode_reader/barcode_reader_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.100173 mindee-4.5.0/mindee/product/cropper/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/cropper/cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/cropper/cropper_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/cropper/cropper_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.100173 mindee-4.5.0/mindee/product/custom/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/custom/custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/custom/custom_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/custom/custom_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.100173 mindee-4.5.0/mindee/product/eu/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.100173 mindee-4.5.0/mindee/product/eu/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/eu/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/eu/driver_license/driver_license_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/eu/driver_license/driver_license_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/eu/driver_license/driver_license_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.100173 mindee-4.5.0/mindee/product/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/eu/license_plate/license_plate_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/eu/license_plate/license_plate_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.100173 mindee-4.5.0/mindee/product/financial_document/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/financial_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/financial_document/financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/financial_document/financial_document_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/financial_document/financial_document_v1_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.100173 mindee-4.5.0/mindee/product/fr/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.104173 mindee-4.5.0/mindee/product/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.104173 mindee-4.5.0/mindee/product/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/carte_grise/carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.104173 mindee-4.5.0/mindee/product/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.104173 mindee-4.5.0/mindee/product/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/id_card/id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/id_card/id_card_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/id_card/id_card_v1_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/id_card/id_card_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/id_card/id_card_v2_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/id_card/id_card_v2_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.104173 mindee-4.5.0/mindee/product/fr/petrol_receipt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/petrol_receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.108173 mindee-4.5.0/mindee/product/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/generated/generated_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/generated/generated_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/generated/generated_v1_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/generated/generated_v1_prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.108173 mindee-4.5.0/mindee/product/international_id/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/international_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/international_id/international_id_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/international_id/international_id_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/international_id/international_id_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/international_id/international_id_v2_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.108173 mindee-4.5.0/mindee/product/invoice/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/invoice/invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/invoice/invoice_v4_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/invoice/invoice_v4_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.108173 mindee-4.5.0/mindee/product/invoice_splitter/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/invoice_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/invoice_splitter/invoice_splitter_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.108173 mindee-4.5.0/mindee/product/material_certificate/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/material_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/material_certificate/material_certificate_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/material_certificate/material_certificate_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.108173 mindee-4.5.0/mindee/product/multi_receipts_detector/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/multi_receipts_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.112172 mindee-4.5.0/mindee/product/passport/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/passport/passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/passport/passport_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.112172 mindee-4.5.0/mindee/product/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/proof_of_address/proof_of_address_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/proof_of_address/proof_of_address_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.112172 mindee-4.5.0/mindee/product/receipt/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/receipt/receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/receipt/receipt_v4_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/receipt/receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/receipt/receipt_v5_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/receipt/receipt_v5_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.112172 mindee-4.5.0/mindee/product/resume/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/resume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/resume/resume_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/resume/resume_v1_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/resume/resume_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/resume/resume_v1_education.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/resume/resume_v1_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/resume/resume_v1_professional_experience.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/resume/resume_v1_social_networks_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.112172 mindee-4.5.0/mindee/product/us/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.112172 mindee-4.5.0/mindee/product/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/bank_check/bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/bank_check/bank_check_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/bank_check/bank_check_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.116172 mindee-4.5.0/mindee/product/us/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/driver_license/driver_license_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/driver_license/driver_license_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/driver_license/driver_license_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.116172 mindee-4.5.0/mindee/product/us/w9/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/w9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/w9/w9_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/w9/w9_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/product/us/w9/w9_v1_page.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/version
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-15 14:12:07.000000 mindee-4.5.0/mindee/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.128172 mindee-4.5.0/mindee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-03-15 14:12:25.000000 mindee-4.5.0/mindee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-03-15 14:12:25.000000 mindee-4.5.0/mindee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:12:25.000000 mindee-4.5.0/mindee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-15 14:12:25.000000 mindee-4.5.0/mindee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 14:12:10.000000 mindee-4.5.0/mindee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-15 14:12:25.000000 mindee-4.5.0/mindee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-15 14:12:25.000000 mindee-4.5.0/mindee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-15 14:12:07.000000 mindee-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-15 14:12:25.128172 mindee-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-15 14:12:07.000000 mindee-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.116172 mindee-4.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.116172 mindee-4.5.0/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/test_ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/test_payment_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/test_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/fields/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.116172 mindee-4.5.0/tests/product/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.116172 mindee-4.5.0/tests/product/barcode_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/barcode_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/barcode_reader/test_barcode_reader_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.120172 mindee-4.5.0/tests/product/cropper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/cropper/test_cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/cropper/test_cropper_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.120172 mindee-4.5.0/tests/product/eu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.120172 mindee-4.5.0/tests/product/eu/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/eu/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/eu/driver_license/test_driver_license_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.120172 mindee-4.5.0/tests/product/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/eu/license_plate/test_license_plate_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.120172 mindee-4.5.0/tests/product/fr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.120172 mindee-4.5.0/tests/product/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/bank_account_details/test_bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.120172 mindee-4.5.0/tests/product/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/carte_grise/test_carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.120172 mindee-4.5.0/tests/product/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/carte_vitale/test_carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.120172 mindee-4.5.0/tests/product/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/id_card/test_id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/id_card/test_id_card_v1_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/id_card/test_id_card_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/fr/id_card/test_id_card_v2_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.124172 mindee-4.5.0/tests/product/international_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/international_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/international_id/test_international_id_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/international_id/test_international_id_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.124172 mindee-4.5.0/tests/product/invoice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/invoice/test_invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/invoice/test_invoice_v4_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.124172 mindee-4.5.0/tests/product/material_certificate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/material_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/material_certificate/test_material_certificate_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.124172 mindee-4.5.0/tests/product/multi_receipts_detector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/multi_receipts_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.124172 mindee-4.5.0/tests/product/passport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/passport/test_passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/passport/test_passport_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.124172 mindee-4.5.0/tests/product/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/proof_of_address/test_proof_of_address_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.124172 mindee-4.5.0/tests/product/receipt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/receipt/test_receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/receipt/test_receipt_v4_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/receipt/test_receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/receipt/test_receipt_v5_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.124172 mindee-4.5.0/tests/product/resume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/resume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/resume/test_resume_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.124172 mindee-4.5.0/tests/product/us/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.124172 mindee-4.5.0/tests/product/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/us/bank_check/test_bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/us/bank_check/test_bank_check_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.128172 mindee-4.5.0/tests/product/us/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/us/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/us/driver_license/test_driver_license_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/us/driver_license/test_driver_license_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:25.128172 mindee-4.5.0/tests/product/us/w9/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/us/w9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/us/w9/test_w9_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/product/us/w9/test_w9_v1_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-15 14:12:07.000000 mindee-4.5.0/tests/test_pkg_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.244418 mindee-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 16:17:59.000000 mindee-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-30 16:18:17.244418 mindee-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-30 16:17:59.000000 mindee-4.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.204418 mindee-4.6.0/mindee/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.204418 mindee-4.6.0/mindee/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/error/geometry_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/error/mimetype_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/error/mindee_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/error/mindee_http_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.204418 mindee-4.6.0/mindee/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/polygon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/quadrilateral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.204418 mindee-4.6.0/mindee/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/input/page_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/input/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.208418 mindee-4.6.0/mindee/mindee_http/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/mindee_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/mindee_http/base_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/mindee_http/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/mindee_http/mindee_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/mindee_http/response_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.208418 mindee-4.6.0/mindee/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.208418 mindee-4.6.0/mindee/parsing/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/async_predict_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.208418 mindee-4.6.0/mindee/parsing/common/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/extras/cropper_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/extras/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/feedback_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.212418 mindee-4.6.0/mindee/parsing/common/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/mvision_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/ocr_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/ocr_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/ocr_word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/predict_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/string_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/summary_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.212418 mindee-4.6.0/mindee/parsing/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/custom/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/custom/line_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/custom/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.212418 mindee-4.6.0/mindee/parsing/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/generated/generated_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/generated/generated_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.212418 mindee-4.6.0/mindee/parsing/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/company_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.212418 mindee-4.6.0/mindee/product/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/barcode_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/barcode_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/barcode_reader/barcode_reader_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/barcode_reader/barcode_reader_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/cropper/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/cropper/cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/cropper/cropper_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/cropper/cropper_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/custom/custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/custom/custom_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/custom/custom_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/eu/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/eu/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/license_plate/license_plate_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/license_plate/license_plate_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/financial_document/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/financial_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/financial_document/financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/financial_document/financial_document_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/financial_document/financial_document_v1_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.220418 mindee-4.6.0/mindee/product/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.220418 mindee-4.6.0/mindee/product/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_grise/carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.220418 mindee-4.6.0/mindee/product/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.220418 mindee-4.6.0/mindee/product/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v1_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v2_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v2_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.220418 mindee-4.6.0/mindee/product/fr/petrol_receipt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/petrol_receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/generated/generated_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/generated/generated_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/generated/generated_v1_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/generated/generated_v1_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/international_id/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/international_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/international_id/international_id_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/international_id/international_id_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/international_id/international_id_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/international_id/international_id_v2_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice/invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice/invoice_v4_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice/invoice_v4_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/invoice_splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/material_certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/material_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/material_certificate/material_certificate_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/material_certificate/material_certificate_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/multi_receipts_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/multi_receipts_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/passport/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/passport/passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/passport/passport_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/proof_of_address/proof_of_address_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/proof_of_address/proof_of_address_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/receipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/receipt_v4_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/receipt_v5_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/receipt_v5_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/resume/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11736 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_education.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_professional_experience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_social_networks_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/us/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/us/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.232418 mindee-4.6.0/mindee/product/us/w9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/w9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/w9/w9_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/w9/w9_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/w9/w9_v1_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/version
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.244418 mindee-4.6.0/mindee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:18:03.000000 mindee-4.6.0/mindee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-30 16:17:59.000000 mindee-4.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-30 16:18:17.248418 mindee-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-30 16:17:59.000000 mindee-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.232418 mindee-4.6.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.232418 mindee-4.6.0/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.232418 mindee-4.6.0/tests/product/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.232418 mindee-4.6.0/tests/product/barcode_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/barcode_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/barcode_reader/test_barcode_reader_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/cropper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/cropper/test_cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/cropper/test_cropper_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/eu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/eu/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/driver_license/test_driver_license_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/license_plate/test_license_plate_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_grise/test_carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_vitale/test_carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/id_card/test_id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/id_card/test_id_card_v1_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/id_card/test_id_card_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/id_card/test_id_card_v2_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/international_id/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/international_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/international_id/test_international_id_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/international_id/test_international_id_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/invoice/test_invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/invoice/test_invoice_v4_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/material_certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/material_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/material_certificate/test_material_certificate_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/multi_receipts_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/multi_receipts_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/passport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/passport/test_passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/passport/test_passport_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/proof_of_address/test_proof_of_address_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/receipt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/receipt/test_receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/receipt/test_receipt_v4_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/receipt/test_receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/receipt/test_receipt_v5_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/resume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/resume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/resume/test_resume_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/us/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/bank_check/test_bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/bank_check/test_bank_check_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.244418 mindee-4.6.0/tests/product/us/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/driver_license/test_driver_license_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/driver_license/test_driver_license_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.244418 mindee-4.6.0/tests/product/us/w9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/w9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/w9/test_w9_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/w9/test_w9_v1_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/test_pkg_versions.py
```

### Comparing `mindee-4.5.0/LICENSE` & `mindee-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/PKG-INFO` & `mindee-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 4.5.0
+Version: 4.6.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: opensource@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-4.5.0/README.md` & `mindee-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/cli.py` & `mindee-4.6.0/mindee/cli.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/client.py` & `mindee-4.6.0/mindee/client.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/error/mindee_error.py` & `mindee-4.6.0/mindee/error/mindee_error.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/error/mindee_http_error.py` & `mindee-4.6.0/mindee/error/mindee_http_error.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/geometry/__init__.py` & `mindee-4.6.0/mindee/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/geometry/bbox.py` & `mindee-4.6.0/mindee/geometry/bbox.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/geometry/minmax.py` & `mindee-4.6.0/mindee/geometry/minmax.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/geometry/polygon.py` & `mindee-4.6.0/mindee/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/geometry/polygon_utils.py` & `mindee-4.6.0/mindee/geometry/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/geometry/quadrilateral.py` & `mindee-4.6.0/mindee/geometry/quadrilateral.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/input/page_options.py` & `mindee-4.6.0/mindee/input/page_options.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/input/sources.py` & `mindee-4.6.0/mindee/input/sources.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/mindee_http/endpoint.py` & `mindee-4.6.0/mindee/mindee_http/endpoint.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/mindee_http/mindee_api.py` & `mindee-4.6.0/mindee/mindee_http/mindee_api.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/mindee_http/response_validation.py` & `mindee-4.6.0/mindee/mindee_http/response_validation.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/__init__.py` & `mindee-4.6.0/mindee/parsing/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/api_request.py` & `mindee-4.6.0/mindee/parsing/common/api_request.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/api_response.py` & `mindee-4.6.0/mindee/parsing/common/api_response.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/async_predict_response.py` & `mindee-4.6.0/mindee/parsing/common/async_predict_response.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/document.py` & `mindee-4.6.0/mindee/parsing/common/document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/extras/cropper_extra.py` & `mindee-4.6.0/mindee/parsing/common/extras/cropper_extra.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/extras/extras.py` & `mindee-4.6.0/mindee/parsing/common/extras/extras.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/inference.py` & `mindee-4.6.0/mindee/parsing/common/inference.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/job.py` & `mindee-4.6.0/mindee/parsing/common/job.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/ocr/ocr_page.py` & `mindee-4.6.0/mindee/parsing/common/ocr/ocr_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/ocr/ocr_word.py` & `mindee-4.6.0/mindee/parsing/common/ocr/ocr_word.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/orientation.py` & `mindee-4.6.0/mindee/parsing/common/orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/page.py` & `mindee-4.6.0/mindee/parsing/common/page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/predict_response.py` & `mindee-4.6.0/mindee/parsing/common/predict_response.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/prediction.py` & `mindee-4.6.0/mindee/parsing/common/prediction.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/common/summary_helper.py` & `mindee-4.6.0/mindee/parsing/common/summary_helper.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/custom/line_items.py` & `mindee-4.6.0/mindee/parsing/custom/line_items.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/custom/list.py` & `mindee-4.6.0/mindee/parsing/custom/list.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/generated/generated_list.py` & `mindee-4.6.0/mindee/parsing/generated/generated_list.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/generated/generated_object.py` & `mindee-4.6.0/mindee/parsing/generated/generated_object.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/__init__.py` & `mindee-4.6.0/mindee/parsing/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/amount.py` & `mindee-4.6.0/mindee/parsing/standard/amount.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/base.py` & `mindee-4.6.0/mindee/parsing/standard/base.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/classification.py` & `mindee-4.6.0/mindee/parsing/standard/classification.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/company_registration.py` & `mindee-4.6.0/mindee/parsing/standard/company_registration.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/date.py` & `mindee-4.6.0/mindee/parsing/standard/date.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/locale.py` & `mindee-4.6.0/mindee/parsing/standard/locale.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/payment_details.py` & `mindee-4.6.0/mindee/parsing/standard/payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/position.py` & `mindee-4.6.0/mindee/parsing/standard/position.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/tax.py` & `mindee-4.6.0/mindee/parsing/standard/tax.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/parsing/standard/text.py` & `mindee-4.6.0/mindee/parsing/standard/text.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/__init__.py` & `mindee-4.6.0/mindee/product/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/barcode_reader/barcode_reader_v1.py` & `mindee-4.6.0/mindee/product/barcode_reader/barcode_reader_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.barcode_reader.barcode_reader_v1_document import (
     BarcodeReaderV1Document,
 )
 
 
 class BarcodeReaderV1(Inference):
-    """Inference prediction for Barcode Reader, API version 1."""
+    """Barcode Reader API version 1 inference prediction."""
 
     prediction: BarcodeReaderV1Document
     """Document-level prediction."""
     pages: List[Page[BarcodeReaderV1Document]]
     """Page-level prediction(s)."""
     endpoint_name = "barcode_reader"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/barcode_reader/barcode_reader_v1_document.py` & `mindee-4.6.0/mindee/product/barcode_reader/barcode_reader_v1_document.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import StringField
 
 
 class BarcodeReaderV1Document(Prediction):
-    """Document data for Barcode Reader, API version 1."""
+    """Barcode Reader API version 1.0 document data."""
 
     codes_1d: List[StringField]
     """List of decoded 1D barcodes."""
     codes_2d: List[StringField]
     """List of decoded 2D barcodes."""
 
     def __init__(
```

### Comparing `mindee-4.5.0/mindee/product/cropper/cropper_v1.py` & `mindee-4.6.0/mindee/product/cropper/cropper_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
-from mindee.product.cropper.cropper_v1_document import CropperV1Document
-from mindee.product.cropper.cropper_v1_page import CropperV1Page
+from mindee.product.cropper.cropper_v1_document import (
+    CropperV1Document,
+)
+from mindee.product.cropper.cropper_v1_page import (
+    CropperV1Page,
+)
 
 
 class CropperV1(Inference):
-    """Inference prediction for Cropper, API version 1."""
+    """Cropper API version 1 inference prediction."""
 
     prediction: CropperV1Document
     """Document-level prediction."""
     pages: List[Page[CropperV1Page]]
     """Page-level prediction(s)."""
     endpoint_name = "cropper"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/cropper/cropper_v1_page.py` & `mindee-4.6.0/mindee/product/cropper/cropper_v1_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import List, Optional
 
 from mindee.parsing.common import StringDict, clean_out_string
 from mindee.parsing.standard import PositionField
-from mindee.product.cropper.cropper_v1_document import CropperV1Document
+from mindee.product.cropper.cropper_v1_document import (
+    CropperV1Document,
+)
 
 
 class CropperV1Page(CropperV1Document):
-    """Page data for Cropper, API version 1."""
+    """Cropper API version 1.1 page data."""
 
     cropping: List[PositionField]
     """List of documents found in the image."""
 
     def __init__(
         self,
         raw_prediction: StringDict,
```

### Comparing `mindee-4.5.0/mindee/product/custom/custom_v1.py` & `mindee-4.6.0/mindee/product/custom/custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/custom/custom_v1_document.py` & `mindee-4.6.0/mindee/product/custom/custom_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/custom/custom_v1_page.py` & `mindee-4.6.0/mindee/product/custom/custom_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/eu/driver_license/driver_license_v1.py` & `mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.eu.driver_license.driver_license_v1_document import (
     DriverLicenseV1Document,
 )
-from mindee.product.eu.driver_license.driver_license_v1_page import DriverLicenseV1Page
+from mindee.product.eu.driver_license.driver_license_v1_page import (
+    DriverLicenseV1Page,
+)
 
 
 class DriverLicenseV1(Inference):
-    """Inference prediction for Driver License, API version 1."""
+    """Driver License API version 1 inference prediction."""
 
     prediction: DriverLicenseV1Document
     """Document-level prediction."""
     pages: List[Page[DriverLicenseV1Page]]
     """Page-level prediction(s)."""
     endpoint_name = "eu_driver_license"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/eu/driver_license/driver_license_v1_document.py` & `mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import DateField, StringField
 
 
 class DriverLicenseV1Document(Prediction):
-    """Document data for Driver License, API version 1."""
+    """Driver License API version 1.0 document data."""
 
     address: StringField
     """EU driver license holders address"""
     category: StringField
     """EU driver license holders categories"""
     country_code: StringField
     """Country code extracted as a string."""
```

### Comparing `mindee-4.5.0/mindee/product/eu/driver_license/driver_license_v1_page.py` & `mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1_page.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from mindee.parsing.standard import PositionField
 from mindee.product.eu.driver_license.driver_license_v1_document import (
     DriverLicenseV1Document,
 )
 
 
 class DriverLicenseV1Page(DriverLicenseV1Document):
-    """Page data for Driver License, API version 1."""
+    """Driver License API version 1.0 page data."""
 
     photo: PositionField
     """Has a photo of the EU driver license holder"""
     signature: PositionField
     """Has a signature of the EU driver license holder"""
 
     def __init__(
```

### Comparing `mindee-4.5.0/mindee/product/eu/license_plate/license_plate_v1.py` & `mindee-4.6.0/mindee/product/eu/license_plate/license_plate_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.eu.license_plate.license_plate_v1_document import (
     LicensePlateV1Document,
 )
 
 
 class LicensePlateV1(Inference):
-    """Inference prediction for License Plate, API version 1."""
+    """License Plate API version 1 inference prediction."""
 
     prediction: LicensePlateV1Document
     """Document-level prediction."""
     pages: List[Page[LicensePlateV1Document]]
     """Page-level prediction(s)."""
     endpoint_name = "license_plates"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/eu/license_plate/license_plate_v1_document.py` & `mindee-4.6.0/mindee/product/eu/license_plate/license_plate_v1_document.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import StringField
 
 
 class LicensePlateV1Document(Prediction):
-    """Document data for License Plate, API version 1."""
+    """License Plate API version 1.1 document data."""
 
     license_plates: List[StringField]
     """List of all license plates found in the image."""
 
     def __init__(
         self,
         raw_prediction: StringDict,
```

### Comparing `mindee-4.5.0/mindee/product/financial_document/financial_document_v1.py` & `mindee-4.6.0/mindee/product/financial_document/financial_document_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.financial_document.financial_document_v1_document import (
     FinancialDocumentV1Document,
 )
 
 
 class FinancialDocumentV1(Inference):
-    """Inference prediction for Financial Document, API version 1."""
+    """Financial Document API version 1 inference prediction."""
 
     prediction: FinancialDocumentV1Document
     """Document-level prediction."""
     pages: List[Page[FinancialDocumentV1Document]]
     """Page-level prediction(s)."""
     endpoint_name = "financial_document"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/financial_document/financial_document_v1_document.py` & `mindee-4.6.0/mindee/product/financial_document/financial_document_v1_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,26 @@
 )
 from mindee.product.financial_document.financial_document_v1_line_item import (
     FinancialDocumentV1LineItem,
 )
 
 
 class FinancialDocumentV1Document(Prediction):
-    """Document data for Financial Document, API version 1."""
+    """Financial Document API version 1.6 document data."""
 
+    billing_address: StringField
+    """The customer's address used for billing."""
     category: ClassificationField
     """The purchase category among predefined classes."""
     customer_address: StringField
     """The address of the customer."""
     customer_company_registrations: List[CompanyRegistrationField]
     """List of company registrations associated to the customer."""
+    customer_id: StringField
+    """The customer account number or identifier from the supplier."""
     customer_name: StringField
     """The name of the customer."""
     date: DateField
     """The date the purchase was made."""
     document_type: ClassificationField
     """One of: 'INVOICE', 'CREDIT NOTE', 'CREDIT CARD RECEIPT', 'EXPENSE RECEIPT'."""
     due_date: DateField
@@ -37,26 +41,32 @@
     """The invoice number or identifier."""
     line_items: List[FinancialDocumentV1LineItem]
     """List of line item details."""
     locale: LocaleField
     """The locale detected on the document."""
     reference_numbers: List[StringField]
     """List of Reference numbers, including PO number."""
+    shipping_address: StringField
+    """The customer's address used for shipping."""
     subcategory: ClassificationField
     """The purchase subcategory among predefined classes for transport and food."""
     supplier_address: StringField
     """The address of the supplier or merchant."""
     supplier_company_registrations: List[CompanyRegistrationField]
     """List of company registrations associated to the supplier."""
+    supplier_email: StringField
+    """The email of the supplier or merchant."""
     supplier_name: StringField
     """The name of the supplier or merchant."""
     supplier_payment_details: List[PaymentDetailsField]
     """List of payment details associated to the supplier."""
     supplier_phone_number: StringField
     """The phone number of the supplier or merchant."""
+    supplier_website: StringField
+    """The website URL of the supplier or merchant."""
     taxes: Taxes
     """List of tax lines information."""
     time: StringField
     """The time the purchase was made."""
     tip: AmountField
     """The total amount of tip and gratuity"""
     total_amount: AmountField
@@ -74,26 +84,34 @@
         """
         Financial Document document.
 
         :param raw_prediction: Raw prediction from HTTP response
         :param page_id: Page number for multi pages pdf input
         """
         super().__init__(raw_prediction, page_id)
+        self.billing_address = StringField(
+            raw_prediction["billing_address"],
+            page_id=page_id,
+        )
         self.category = ClassificationField(
             raw_prediction["category"],
             page_id=page_id,
         )
         self.customer_address = StringField(
             raw_prediction["customer_address"],
             page_id=page_id,
         )
         self.customer_company_registrations = [
             CompanyRegistrationField(prediction, page_id=page_id)
             for prediction in raw_prediction["customer_company_registrations"]
         ]
+        self.customer_id = StringField(
+            raw_prediction["customer_id"],
+            page_id=page_id,
+        )
         self.customer_name = StringField(
             raw_prediction["customer_name"],
             page_id=page_id,
         )
         self.date = DateField(
             raw_prediction["date"],
             page_id=page_id,
@@ -118,38 +136,50 @@
             raw_prediction["locale"],
             page_id=page_id,
         )
         self.reference_numbers = [
             StringField(prediction, page_id=page_id)
             for prediction in raw_prediction["reference_numbers"]
         ]
+        self.shipping_address = StringField(
+            raw_prediction["shipping_address"],
+            page_id=page_id,
+        )
         self.subcategory = ClassificationField(
             raw_prediction["subcategory"],
             page_id=page_id,
         )
         self.supplier_address = StringField(
             raw_prediction["supplier_address"],
             page_id=page_id,
         )
         self.supplier_company_registrations = [
             CompanyRegistrationField(prediction, page_id=page_id)
             for prediction in raw_prediction["supplier_company_registrations"]
         ]
+        self.supplier_email = StringField(
+            raw_prediction["supplier_email"],
+            page_id=page_id,
+        )
         self.supplier_name = StringField(
             raw_prediction["supplier_name"],
             page_id=page_id,
         )
         self.supplier_payment_details = [
             PaymentDetailsField(prediction, page_id=page_id)
             for prediction in raw_prediction["supplier_payment_details"]
         ]
         self.supplier_phone_number = StringField(
             raw_prediction["supplier_phone_number"],
             page_id=page_id,
         )
+        self.supplier_website = StringField(
+            raw_prediction["supplier_website"],
+            page_id=page_id,
+        )
         self.taxes = Taxes(raw_prediction["taxes"], page_id=page_id)
         self.time = StringField(
             raw_prediction["time"],
             page_id=page_id,
         )
         self.tip = AmountField(
             raw_prediction["tip"],
@@ -226,18 +256,23 @@
         out_str += f":Supplier Name: {self.supplier_name}\n"
         out_str += (
             f":Supplier Company Registrations: {supplier_company_registrations}\n"
         )
         out_str += f":Supplier Address: {self.supplier_address}\n"
         out_str += f":Supplier Phone Number: {self.supplier_phone_number}\n"
         out_str += f":Customer Name: {self.customer_name}\n"
+        out_str += f":Supplier Website: {self.supplier_website}\n"
+        out_str += f":Supplier Email: {self.supplier_email}\n"
         out_str += (
             f":Customer Company Registrations: {customer_company_registrations}\n"
         )
         out_str += f":Customer Address: {self.customer_address}\n"
+        out_str += f":Customer ID: {self.customer_id}\n"
+        out_str += f":Shipping Address: {self.shipping_address}\n"
+        out_str += f":Billing Address: {self.billing_address}\n"
         out_str += f":Document Type: {self.document_type}\n"
         out_str += f":Purchase Subcategory: {self.subcategory}\n"
         out_str += f":Purchase Category: {self.category}\n"
         out_str += f":Total Tax: {self.total_tax}\n"
         out_str += f":Tip and Gratuity: {self.tip}\n"
         out_str += f":Purchase Time: {self.time}\n"
         out_str += f":Line Items: {self._line_items_to_str()}\n"
```

### Comparing `mindee-4.5.0/mindee/product/financial_document/financial_document_v1_line_item.py` & `mindee-4.6.0/mindee/product/financial_document/financial_document_v1_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/fr/__init__.py` & `mindee-4.6.0/mindee/product/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py` & `mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.fr.bank_account_details.bank_account_details_v1_document import (
     BankAccountDetailsV1Document,
 )
 
 
 class BankAccountDetailsV1(Inference):
-    """Inference prediction for Bank Account Details, API version 1."""
+    """Bank Account Details API version 1 inference prediction."""
 
     prediction: BankAccountDetailsV1Document
     """Document-level prediction."""
     pages: List[Page[BankAccountDetailsV1Document]]
     """Page-level prediction(s)."""
     endpoint_name = "bank_account_details"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py` & `mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import StringField
 
 
 class BankAccountDetailsV1Document(Prediction):
-    """Document data for Bank Account Details, API version 1."""
+    """Bank Account Details API version 1.0 document data."""
 
     account_holder_name: StringField
     """The name of the account holder as seen on the document."""
     iban: StringField
     """The International Bank Account Number (IBAN)."""
     swift: StringField
     """The bank's SWIFT Business Identifier Code (BIC)."""
```

### Comparing `mindee-4.5.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py` & `mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.fr.bank_account_details.bank_account_details_v2_document import (
     BankAccountDetailsV2Document,
 )
 
 
 class BankAccountDetailsV2(Inference):
-    """Inference prediction for Bank Account Details, API version 2."""
+    """Bank Account Details API version 2 inference prediction."""
 
     prediction: BankAccountDetailsV2Document
     """Document-level prediction."""
     pages: List[Page[BankAccountDetailsV2Document]]
     """Page-level prediction(s)."""
     endpoint_name = "bank_account_details"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py` & `mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py` & `mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from mindee.parsing.standard import StringField
 from mindee.product.fr.bank_account_details.bank_account_details_v2_bban import (
     BankAccountDetailsV2Bban,
 )
 
 
 class BankAccountDetailsV2Document(Prediction):
-    """Document data for Bank Account Details, API version 2."""
+    """Bank Account Details API version 2.0 document data."""
 
     account_holders_names: StringField
     """Full extraction of the account holders names."""
     bban: BankAccountDetailsV2Bban
     """Full extraction of BBAN, including: branch code, bank code, account and key."""
     iban: StringField
     """Full extraction of the IBAN number."""
```

### Comparing `mindee-4.5.0/mindee/product/fr/carte_grise/carte_grise_v1.py` & `mindee-4.6.0/mindee/product/invoice/invoice_v4.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
-from mindee.product.fr.carte_grise.carte_grise_v1_document import CarteGriseV1Document
+from mindee.product.invoice.invoice_v4_document import (
+    InvoiceV4Document,
+)
 
 
-class CarteGriseV1(Inference):
-    """Inference prediction for Carte Grise, API version 1."""
+class InvoiceV4(Inference):
+    """Invoice API version 4 inference prediction."""
 
-    prediction: CarteGriseV1Document
+    prediction: InvoiceV4Document
     """Document-level prediction."""
-    pages: List[Page[CarteGriseV1Document]]
+    pages: List[Page[InvoiceV4Document]]
     """Page-level prediction(s)."""
-    endpoint_name = "carte_grise"
+    endpoint_name = "invoices"
     """Name of the endpoint."""
-    endpoint_version = "1"
+    endpoint_version = "4"
     """Version of the endpoint."""
 
     def __init__(self, raw_prediction: StringDict):
         """
-        Carte Grise v1 inference.
+        Invoice v4 inference.
 
         :param raw_prediction: Raw prediction from the HTTP response.
         """
         super().__init__(raw_prediction)
 
-        self.prediction = CarteGriseV1Document(raw_prediction["prediction"])
+        self.prediction = InvoiceV4Document(raw_prediction["prediction"])
         self.pages = []
         for page in raw_prediction["pages"]:
             try:
                 page_production = page["prediction"]
             except KeyError:
                 continue
             if page_production:
-                self.pages.append(Page(CarteGriseV1Document, page))
+                self.pages.append(Page(InvoiceV4Document, page))
```

### Comparing `mindee-4.5.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py` & `mindee-4.6.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import DateField, StringField
 
 
 class CarteGriseV1Document(Prediction):
-    """Document data for Carte Grise, API version 1."""
+    """Carte Grise API version 1.1 document data."""
 
     a: StringField
     """The vehicle's license plate number."""
     b: DateField
     """The vehicle's first release date."""
     c1: StringField
     """The vehicle owner's full name including maiden name."""
```

### Comparing `mindee-4.5.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py` & `mindee-4.6.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.fr.carte_vitale.carte_vitale_v1_document import (
     CarteVitaleV1Document,
 )
 
 
 class CarteVitaleV1(Inference):
-    """Inference prediction for Carte Vitale, API version 1."""
+    """Carte Vitale API version 1 inference prediction."""
 
     prediction: CarteVitaleV1Document
     """Document-level prediction."""
     pages: List[Page[CarteVitaleV1Document]]
     """Page-level prediction(s)."""
     endpoint_name = "carte_vitale"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py` & `mindee-4.6.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import DateField, StringField
 
 
 class CarteVitaleV1Document(Prediction):
-    """Document data for Carte Vitale, API version 1."""
+    """Carte Vitale API version 1.1 document data."""
 
     given_names: List[StringField]
     """The given name(s) of the card holder."""
     issuance_date: DateField
     """The date the card was issued."""
     social_security: StringField
     """The Social Security Number (Numéro de Sécurité Sociale) of the card holder"""
```

### Comparing `mindee-4.5.0/mindee/product/fr/id_card/id_card_v1.py` & `mindee-4.6.0/mindee/product/fr/id_card/id_card_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
-from mindee.product.fr.id_card.id_card_v1_document import IdCardV1Document
-from mindee.product.fr.id_card.id_card_v1_page import IdCardV1Page
+from mindee.product.fr.id_card.id_card_v1_document import (
+    IdCardV1Document,
+)
+from mindee.product.fr.id_card.id_card_v1_page import (
+    IdCardV1Page,
+)
 
 
 class IdCardV1(Inference):
-    """Inference prediction for Carte Nationale d'Identité, API version 1."""
+    """Carte Nationale d'Identité API version 1 inference prediction."""
 
     prediction: IdCardV1Document
     """Document-level prediction."""
     pages: List[Page[IdCardV1Page]]
     """Page-level prediction(s)."""
     endpoint_name = "idcard_fr"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/fr/id_card/id_card_v1_document.py` & `mindee-4.6.0/mindee/product/fr/id_card/id_card_v1_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import DateField, StringField
 
 
 class IdCardV1Document(Prediction):
-    """Document data for Carte Nationale d'Identité, API version 1."""
+    """Carte Nationale d'Identité API version 1.1 document data."""
 
     authority: StringField
     """The name of the issuing authority."""
     birth_date: DateField
     """The date of birth of the card holder."""
     birth_place: StringField
     """The place of birth of the card holder."""
```

### Comparing `mindee-4.5.0/mindee/product/fr/id_card/id_card_v1_page.py` & `mindee-4.6.0/mindee/product/fr/id_card/id_card_v1_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Optional
 
 from mindee.parsing.common import StringDict, clean_out_string
 from mindee.parsing.standard import ClassificationField
-from mindee.product.fr.id_card.id_card_v1_document import IdCardV1Document
+from mindee.product.fr.id_card.id_card_v1_document import (
+    IdCardV1Document,
+)
 
 
 class IdCardV1Page(IdCardV1Document):
-    """Page data for Carte Nationale d'Identité, API version 1."""
+    """Carte Nationale d'Identité API version 1.1 page data."""
 
     document_side: ClassificationField
     """The side of the document which is visible."""
 
     def __init__(
         self,
         raw_prediction: StringDict,
```

### Comparing `mindee-4.5.0/mindee/product/fr/id_card/id_card_v2.py` & `mindee-4.6.0/mindee/product/fr/id_card/id_card_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
-from mindee.product.fr.id_card.id_card_v2_document import IdCardV2Document
-from mindee.product.fr.id_card.id_card_v2_page import IdCardV2Page
+from mindee.product.fr.id_card.id_card_v2_document import (
+    IdCardV2Document,
+)
+from mindee.product.fr.id_card.id_card_v2_page import (
+    IdCardV2Page,
+)
 
 
 class IdCardV2(Inference):
-    """Inference prediction for Carte Nationale d'Identité, API version 2."""
+    """Carte Nationale d'Identité API version 2 inference prediction."""
 
     prediction: IdCardV2Document
     """Document-level prediction."""
     pages: List[Page[IdCardV2Page]]
     """Page-level prediction(s)."""
     endpoint_name = "idcard_fr"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/fr/id_card/id_card_v2_document.py` & `mindee-4.6.0/mindee/product/fr/id_card/id_card_v2_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import DateField, StringField
 
 
 class IdCardV2Document(Prediction):
-    """Document data for Carte Nationale d'Identité, API version 2."""
+    """Carte Nationale d'Identité API version 2.0 document data."""
 
     alternate_name: StringField
     """The alternate name of the card holder."""
     authority: StringField
     """The name of the issuing authority."""
     birth_date: DateField
     """The date of birth of the card holder."""
```

### Comparing `mindee-4.5.0/mindee/product/fr/id_card/id_card_v2_page.py` & `mindee-4.6.0/mindee/product/fr/id_card/id_card_v2_page.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Optional
 
 from mindee.parsing.common import StringDict, clean_out_string
 from mindee.parsing.standard import ClassificationField
-from mindee.product.fr.id_card.id_card_v2_document import IdCardV2Document
+from mindee.product.fr.id_card.id_card_v2_document import (
+    IdCardV2Document,
+)
 
 
 class IdCardV2Page(IdCardV2Document):
-    """Page data for Carte Nationale d'Identité, API version 2."""
+    """Carte Nationale d'Identité API version 2.0 page data."""
 
     document_side: ClassificationField
     """The sides of the document which are visible."""
     document_type: ClassificationField
     """The document type or format."""
 
     def __init__(
```

### Comparing `mindee-4.5.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py` & `mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py` & `mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py` & `mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py` & `mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/generated/generated_v1.py` & `mindee-4.6.0/mindee/product/generated/generated_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/generated/generated_v1_document.py` & `mindee-4.6.0/mindee/product/generated/generated_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/generated/generated_v1_page.py` & `mindee-4.6.0/mindee/product/generated/generated_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/generated/generated_v1_prediction.py` & `mindee-4.6.0/mindee/product/generated/generated_v1_prediction.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/international_id/international_id_v1.py` & `mindee-4.6.0/mindee/product/international_id/international_id_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/international_id/international_id_v1_document.py` & `mindee-4.6.0/mindee/product/international_id/international_id_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/international_id/international_id_v2.py` & `mindee-4.6.0/mindee/product/international_id/international_id_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.international_id.international_id_v2_document import (
     InternationalIdV2Document,
 )
 
 
 class InternationalIdV2(Inference):
-    """Inference prediction for International ID, API version 2."""
+    """International ID API version 2 inference prediction."""
 
     prediction: InternationalIdV2Document
     """Document-level prediction."""
     pages: List[Page[InternationalIdV2Document]]
     """Page-level prediction(s)."""
     endpoint_name = "international_id"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/international_id/international_id_v2_document.py` & `mindee-4.6.0/mindee/product/international_id/international_id_v2_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import ClassificationField, DateField, StringField
 
 
 class InternationalIdV2Document(Prediction):
-    """Document data for International ID, API version 2."""
+    """International ID API version 2.0 document data."""
 
     address: StringField
     """The physical address of the document holder."""
     birth_date: DateField
     """The date of birth of the document holder."""
     birth_place: StringField
     """The place of birth of the document holder."""
```

### Comparing `mindee-4.5.0/mindee/product/invoice/invoice_v4.py` & `mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
-from mindee.product.invoice.invoice_v4_document import InvoiceV4Document
+from mindee.product.us.bank_check.bank_check_v1_document import (
+    BankCheckV1Document,
+)
+from mindee.product.us.bank_check.bank_check_v1_page import (
+    BankCheckV1Page,
+)
 
 
-class InvoiceV4(Inference):
-    """Inference prediction for Invoice, API version 4."""
+class BankCheckV1(Inference):
+    """Bank Check API version 1 inference prediction."""
 
-    prediction: InvoiceV4Document
+    prediction: BankCheckV1Document
     """Document-level prediction."""
-    pages: List[Page[InvoiceV4Document]]
+    pages: List[Page[BankCheckV1Page]]
     """Page-level prediction(s)."""
-    endpoint_name = "invoices"
+    endpoint_name = "bank_check"
     """Name of the endpoint."""
-    endpoint_version = "4"
+    endpoint_version = "1"
     """Version of the endpoint."""
 
     def __init__(self, raw_prediction: StringDict):
         """
-        Invoice v4 inference.
+        Bank Check v1 inference.
 
         :param raw_prediction: Raw prediction from the HTTP response.
         """
         super().__init__(raw_prediction)
 
-        self.prediction = InvoiceV4Document(raw_prediction["prediction"])
+        self.prediction = BankCheckV1Document(raw_prediction["prediction"])
         self.pages = []
         for page in raw_prediction["pages"]:
             try:
                 page_production = page["prediction"]
             except KeyError:
                 continue
             if page_production:
-                self.pages.append(Page(InvoiceV4Document, page))
+                self.pages.append(Page(BankCheckV1Page, page))
```

### Comparing `mindee-4.5.0/mindee/product/invoice/invoice_v4_document.py` & `mindee-4.6.0/mindee/product/invoice/invoice_v4_document.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,24 @@
     StringField,
     Taxes,
 )
 from mindee.product.invoice.invoice_v4_line_item import InvoiceV4LineItem
 
 
 class InvoiceV4Document(Prediction):
-    """Document data for Invoice, API version 4."""
+    """Invoice API version 4.6 document data."""
 
     billing_address: StringField
     """The customer's address used for billing."""
     customer_address: StringField
     """The address of the customer."""
     customer_company_registrations: List[CompanyRegistrationField]
     """List of company registrations associated to the customer."""
+    customer_id: StringField
+    """The customer account number or identifier from the supplier."""
     customer_name: StringField
     """The name of the customer or client."""
     date: DateField
     """The date the purchase was made."""
     document_type: ClassificationField
     """One of: 'INVOICE', 'CREDIT NOTE'."""
     due_date: DateField
@@ -41,18 +43,24 @@
     """List of Reference numbers, including PO number."""
     shipping_address: StringField
     """Customer's delivery address."""
     supplier_address: StringField
     """The address of the supplier or merchant."""
     supplier_company_registrations: List[CompanyRegistrationField]
     """List of company registrations associated to the supplier."""
+    supplier_email: StringField
+    """The email of the supplier or merchant."""
     supplier_name: StringField
     """The name of the supplier or merchant."""
     supplier_payment_details: List[PaymentDetailsField]
     """List of payment details associated to the supplier."""
+    supplier_phone_number: StringField
+    """The phone number of the supplier or merchant."""
+    supplier_website: StringField
+    """The website URL of the supplier or merchant."""
     taxes: Taxes
     """List of tax line details."""
     total_amount: AmountField
     """The total amount paid: includes taxes, tips, fees, and other charges."""
     total_net: AmountField
     """The net amount paid: does not include taxes, fees, and discounts."""
     total_tax: AmountField
@@ -78,14 +86,18 @@
             raw_prediction["customer_address"],
             page_id=page_id,
         )
         self.customer_company_registrations = [
             CompanyRegistrationField(prediction, page_id=page_id)
             for prediction in raw_prediction["customer_company_registrations"]
         ]
+        self.customer_id = StringField(
+            raw_prediction["customer_id"],
+            page_id=page_id,
+        )
         self.customer_name = StringField(
             raw_prediction["customer_name"],
             page_id=page_id,
         )
         self.date = DateField(
             raw_prediction["date"],
             page_id=page_id,
@@ -122,22 +134,34 @@
             raw_prediction["supplier_address"],
             page_id=page_id,
         )
         self.supplier_company_registrations = [
             CompanyRegistrationField(prediction, page_id=page_id)
             for prediction in raw_prediction["supplier_company_registrations"]
         ]
+        self.supplier_email = StringField(
+            raw_prediction["supplier_email"],
+            page_id=page_id,
+        )
         self.supplier_name = StringField(
             raw_prediction["supplier_name"],
             page_id=page_id,
         )
         self.supplier_payment_details = [
             PaymentDetailsField(prediction, page_id=page_id)
             for prediction in raw_prediction["supplier_payment_details"]
         ]
+        self.supplier_phone_number = StringField(
+            raw_prediction["supplier_phone_number"],
+            page_id=page_id,
+        )
+        self.supplier_website = StringField(
+            raw_prediction["supplier_website"],
+            page_id=page_id,
+        )
         self.taxes = Taxes(raw_prediction["taxes"], page_id=page_id)
         self.total_amount = AmountField(
             raw_prediction["total_amount"],
             page_id=page_id,
         )
         self.total_net = AmountField(
             raw_prediction["total_net"],
@@ -205,17 +229,21 @@
         out_str += f":Taxes: {self.taxes}\n"
         out_str += f":Supplier Payment Details: {supplier_payment_details}\n"
         out_str += f":Supplier Name: {self.supplier_name}\n"
         out_str += (
             f":Supplier Company Registrations: {supplier_company_registrations}\n"
         )
         out_str += f":Supplier Address: {self.supplier_address}\n"
+        out_str += f":Supplier Phone Number: {self.supplier_phone_number}\n"
+        out_str += f":Supplier Website: {self.supplier_website}\n"
+        out_str += f":Supplier Email: {self.supplier_email}\n"
         out_str += f":Customer Name: {self.customer_name}\n"
         out_str += (
             f":Customer Company Registrations: {customer_company_registrations}\n"
         )
         out_str += f":Customer Address: {self.customer_address}\n"
+        out_str += f":Customer ID: {self.customer_id}\n"
         out_str += f":Shipping Address: {self.shipping_address}\n"
         out_str += f":Billing Address: {self.billing_address}\n"
         out_str += f":Document Type: {self.document_type}\n"
         out_str += f":Line Items: {self._line_items_to_str()}\n"
         return clean_out_string(out_str)
```

### Comparing `mindee-4.5.0/mindee/product/invoice/invoice_v4_line_item.py` & `mindee-4.6.0/mindee/product/invoice/invoice_v4_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/invoice_splitter/invoice_splitter_v1.py` & `mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py` & `mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py` & `mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/material_certificate/material_certificate_v1.py` & `mindee-4.6.0/mindee/product/material_certificate/material_certificate_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.material_certificate.material_certificate_v1_document import (
     MaterialCertificateV1Document,
 )
 
 
 class MaterialCertificateV1(Inference):
-    """Inference prediction for Material Certificate, API version 1."""
+    """Material Certificate API version 1 inference prediction."""
 
     prediction: MaterialCertificateV1Document
     """Document-level prediction."""
     pages: List[Page[MaterialCertificateV1Document]]
     """Page-level prediction(s)."""
     endpoint_name = "material_certificate"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/material_certificate/material_certificate_v1_document.py` & `mindee-4.6.0/mindee/product/material_certificate/material_certificate_v1_document.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import StringField
 
 
 class MaterialCertificateV1Document(Prediction):
-    """Document data for Material Certificate, API version 1."""
+    """Material Certificate API version 1.0 document data."""
 
     certificate_type: StringField
     """The type of certification."""
     heat_number: StringField
     """Heat Number is a unique identifier assigned to a batch of material produced in a manufacturing process."""
     norm: StringField
     """The international standard used for certification."""
```

### Comparing `mindee-4.5.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py` & `mindee-4.6.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.multi_receipts_detector.multi_receipts_detector_v1_document import (
     MultiReceiptsDetectorV1Document,
 )
 
 
 class MultiReceiptsDetectorV1(Inference):
-    """Inference prediction for Multi Receipts Detector, API version 1."""
+    """Multi Receipts Detector API version 1 inference prediction."""
 
     prediction: MultiReceiptsDetectorV1Document
     """Document-level prediction."""
     pages: List[Page[MultiReceiptsDetectorV1Document]]
     """Page-level prediction(s)."""
     endpoint_name = "multi_receipts_detector"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py` & `mindee-4.6.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import PositionField
 
 
 class MultiReceiptsDetectorV1Document(Prediction):
-    """Document data for Multi Receipts Detector, API version 1."""
+    """Multi Receipts Detector API version 1.0 document data."""
 
     receipts: List[PositionField]
     """Positions of the receipts on the document."""
 
     def __init__(
         self,
         raw_prediction: StringDict,
```

### Comparing `mindee-4.5.0/mindee/product/passport/passport_v1.py` & `mindee-4.6.0/mindee/product/passport/passport_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
-from mindee.product.passport.passport_v1_document import PassportV1Document
+from mindee.product.passport.passport_v1_document import (
+    PassportV1Document,
+)
 
 
 class PassportV1(Inference):
-    """Inference prediction for Passport, API version 1."""
+    """Passport API version 1 inference prediction."""
 
     prediction: PassportV1Document
     """Document-level prediction."""
     pages: List[Page[PassportV1Document]]
     """Page-level prediction(s)."""
     endpoint_name = "passport"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/passport/passport_v1_document.py` & `mindee-4.6.0/mindee/product/passport/passport_v1_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import DateField, StringField
 
 
 class PassportV1Document(Prediction):
-    """Document data for Passport, API version 1."""
+    """Passport API version 1.1 document data."""
 
     birth_date: DateField
     """The date of birth of the passport holder."""
     birth_place: StringField
     """The place of birth of the passport holder."""
     country: StringField
     """The country's 3 letter code (ISO 3166-1 alpha-3)."""
```

### Comparing `mindee-4.5.0/mindee/product/proof_of_address/proof_of_address_v1.py` & `mindee-4.6.0/mindee/product/proof_of_address/proof_of_address_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.proof_of_address.proof_of_address_v1_document import (
     ProofOfAddressV1Document,
 )
 
 
 class ProofOfAddressV1(Inference):
-    """Inference prediction for Proof of Address, API version 1."""
+    """Proof of Address API version 1 inference prediction."""
 
     prediction: ProofOfAddressV1Document
     """Document-level prediction."""
     pages: List[Page[ProofOfAddressV1Document]]
     """Page-level prediction(s)."""
     endpoint_name = "proof_of_address"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/proof_of_address/proof_of_address_v1_document.py` & `mindee-4.6.0/mindee/product/proof_of_address/proof_of_address_v1_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     DateField,
     LocaleField,
     StringField,
 )
 
 
 class ProofOfAddressV1Document(Prediction):
-    """Document data for Proof of Address, API version 1."""
+    """Proof of Address API version 1.1 document data."""
 
     date: DateField
     """The date the document was issued."""
     dates: List[DateField]
     """List of dates found on the document."""
     issuer_address: StringField
     """The address of the document's issuer."""
```

### Comparing `mindee-4.5.0/mindee/product/receipt/receipt_v4.py` & `mindee-4.6.0/mindee/product/receipt/receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/receipt/receipt_v4_document.py` & `mindee-4.6.0/mindee/product/receipt/receipt_v4_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/receipt/receipt_v5.py` & `mindee-4.6.0/mindee/product/receipt/receipt_v5.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
-from mindee.product.receipt.receipt_v5_document import ReceiptV5Document
+from mindee.product.receipt.receipt_v5_document import (
+    ReceiptV5Document,
+)
 
 
 class ReceiptV5(Inference):
-    """Inference prediction for Receipt, API version 5."""
+    """Receipt API version 5 inference prediction."""
 
     prediction: ReceiptV5Document
     """Document-level prediction."""
     pages: List[Page[ReceiptV5Document]]
     """Page-level prediction(s)."""
     endpoint_name = "expense_receipts"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/receipt/receipt_v5_document.py` & `mindee-4.6.0/mindee/product/receipt/receipt_v5_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     StringField,
     Taxes,
 )
 from mindee.product.receipt.receipt_v5_line_item import ReceiptV5LineItem
 
 
 class ReceiptV5Document(Prediction):
-    """Document data for Receipt, API version 5."""
+    """Receipt API version 5.1 document data."""
 
     category: ClassificationField
     """The purchase category among predefined classes."""
     date: DateField
     """The date the purchase was made."""
     document_type: ClassificationField
     """One of: 'CREDIT CARD RECEIPT', 'EXPENSE RECEIPT'."""
```

### Comparing `mindee-4.5.0/mindee/product/receipt/receipt_v5_line_item.py` & `mindee-4.6.0/mindee/product/receipt/receipt_v5_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/resume/__init__.py` & `mindee-4.6.0/mindee/product/resume/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/resume/resume_v1.py` & `mindee-4.6.0/mindee/product/resume/resume_v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
-from mindee.product.resume.resume_v1_document import ResumeV1Document
+from mindee.product.resume.resume_v1_document import (
+    ResumeV1Document,
+)
 
 
 class ResumeV1(Inference):
-    """Inference prediction for Resume, API version 1."""
+    """Resume API version 1 inference prediction."""
 
     prediction: ResumeV1Document
     """Document-level prediction."""
     pages: List[Page[ResumeV1Document]]
     """Page-level prediction(s)."""
     endpoint_name = "resume"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/resume/resume_v1_certificate.py` & `mindee-4.6.0/mindee/product/resume/resume_v1_certificate.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/resume/resume_v1_document.py` & `mindee-4.6.0/mindee/product/resume/resume_v1_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from mindee.product.resume.resume_v1_social_networks_url import (
     ResumeV1SocialNetworksUrl,
 )
 
 
 class ResumeV1Document(Prediction):
-    """Document data for Resume, API version 1."""
+    """Resume API version 1.0 document data."""
 
     address: StringField
     """The location information of the candidate, including city, state, and country."""
     certificates: List[ResumeV1Certificate]
     """The list of certificates obtained by the candidate."""
     document_language: StringField
     """The ISO 639 code of the language in which the document is written."""
```

### Comparing `mindee-4.5.0/mindee/product/resume/resume_v1_education.py` & `mindee-4.6.0/mindee/product/resume/resume_v1_education.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/resume/resume_v1_language.py` & `mindee-4.6.0/mindee/product/resume/resume_v1_language.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/resume/resume_v1_professional_experience.py` & `mindee-4.6.0/mindee/product/resume/resume_v1_professional_experience.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/resume/resume_v1_social_networks_url.py` & `mindee-4.6.0/mindee/product/resume/resume_v1_social_networks_url.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/us/__init__.py` & `mindee-4.6.0/mindee/product/us/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee/product/us/bank_check/bank_check_v1.py` & `mindee-4.6.0/mindee/product/us/w9/w9_v1.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
-from mindee.product.us.bank_check.bank_check_v1_document import BankCheckV1Document
-from mindee.product.us.bank_check.bank_check_v1_page import BankCheckV1Page
+from mindee.product.us.w9.w9_v1_document import (
+    W9V1Document,
+)
+from mindee.product.us.w9.w9_v1_page import (
+    W9V1Page,
+)
 
 
-class BankCheckV1(Inference):
-    """Inference prediction for Bank Check, API version 1."""
+class W9V1(Inference):
+    """W9 API version 1 inference prediction."""
 
-    prediction: BankCheckV1Document
+    prediction: W9V1Document
     """Document-level prediction."""
-    pages: List[Page[BankCheckV1Page]]
+    pages: List[Page[W9V1Page]]
     """Page-level prediction(s)."""
-    endpoint_name = "bank_check"
+    endpoint_name = "us_w9"
     """Name of the endpoint."""
     endpoint_version = "1"
     """Version of the endpoint."""
 
     def __init__(self, raw_prediction: StringDict):
         """
-        Bank Check v1 inference.
+        W9 v1 inference.
 
         :param raw_prediction: Raw prediction from the HTTP response.
         """
         super().__init__(raw_prediction)
 
-        self.prediction = BankCheckV1Document(raw_prediction["prediction"])
+        self.prediction = W9V1Document(raw_prediction["prediction"])
         self.pages = []
         for page in raw_prediction["pages"]:
             try:
                 page_production = page["prediction"]
             except KeyError:
                 continue
             if page_production:
-                self.pages.append(Page(BankCheckV1Page, page))
+                self.pages.append(Page(W9V1Page, page))
```

### Comparing `mindee-4.5.0/mindee/product/us/bank_check/bank_check_v1_document.py` & `mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1_document.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import AmountField, DateField, StringField
 
 
 class BankCheckV1Document(Prediction):
-    """Document data for Bank Check, API version 1."""
+    """Bank Check API version 1.1 document data."""
 
     account_number: StringField
     """The check payer's account number."""
     amount: AmountField
     """The amount of the check."""
     check_number: StringField
     """The issuer's check number."""
```

### Comparing `mindee-4.5.0/mindee/product/us/bank_check/bank_check_v1_page.py` & `mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import List, Optional
 
 from mindee.parsing.common import StringDict, clean_out_string
 from mindee.parsing.standard import PositionField
-from mindee.product.us.bank_check.bank_check_v1_document import BankCheckV1Document
+from mindee.product.us.bank_check.bank_check_v1_document import (
+    BankCheckV1Document,
+)
 
 
 class BankCheckV1Page(BankCheckV1Document):
-    """Page data for Bank Check, API version 1."""
+    """Bank Check API version 1.1 page data."""
 
     check_position: PositionField
     """The position of the check on the document."""
     signatures_positions: List[PositionField]
     """List of signature positions"""
 
     def __init__(
```

### Comparing `mindee-4.5.0/mindee/product/us/driver_license/driver_license_v1.py` & `mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
 from mindee.product.us.driver_license.driver_license_v1_document import (
     DriverLicenseV1Document,
 )
-from mindee.product.us.driver_license.driver_license_v1_page import DriverLicenseV1Page
+from mindee.product.us.driver_license.driver_license_v1_page import (
+    DriverLicenseV1Page,
+)
 
 
 class DriverLicenseV1(Inference):
-    """Inference prediction for Driver License, API version 1."""
+    """Driver License API version 1 inference prediction."""
 
     prediction: DriverLicenseV1Document
     """Document-level prediction."""
     pages: List[Page[DriverLicenseV1Page]]
     """Page-level prediction(s)."""
     endpoint_name = "us_driver_license"
     """Name of the endpoint."""
```

### Comparing `mindee-4.5.0/mindee/product/us/driver_license/driver_license_v1_document.py` & `mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from mindee.parsing.common import Prediction, StringDict, clean_out_string
 from mindee.parsing.standard import DateField, StringField
 
 
 class DriverLicenseV1Document(Prediction):
-    """Document data for Driver License, API version 1."""
+    """Driver License API version 1.1 document data."""
 
     address: StringField
     """US driver license holders address"""
     date_of_birth: DateField
     """US driver license holders date of birth"""
     dd_number: StringField
     """Document Discriminator Number of the US Driver License"""
```

### Comparing `mindee-4.5.0/mindee/product/us/driver_license/driver_license_v1_page.py` & `mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from mindee.parsing.standard import PositionField
 from mindee.product.us.driver_license.driver_license_v1_document import (
     DriverLicenseV1Document,
 )
 
 
 class DriverLicenseV1Page(DriverLicenseV1Document):
-    """Page data for Driver License, API version 1."""
+    """Driver License API version 1.1 page data."""
 
     photo: PositionField
     """Has a photo of the US driver license holder"""
     signature: PositionField
     """Has a signature of the US driver license holder"""
 
     def __init__(
```

### Comparing `mindee-4.5.0/mindee/product/us/w9/w9_v1.py` & `mindee-4.6.0/mindee/product/fr/carte_grise/carte_grise_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from typing import List
 
 from mindee.parsing.common import Inference, Page, StringDict
-from mindee.product.us.w9.w9_v1_document import W9V1Document
-from mindee.product.us.w9.w9_v1_page import W9V1Page
+from mindee.product.fr.carte_grise.carte_grise_v1_document import (
+    CarteGriseV1Document,
+)
 
 
-class W9V1(Inference):
-    """Inference prediction for W9, API version 1."""
+class CarteGriseV1(Inference):
+    """Carte Grise API version 1 inference prediction."""
 
-    prediction: W9V1Document
+    prediction: CarteGriseV1Document
     """Document-level prediction."""
-    pages: List[Page[W9V1Page]]
+    pages: List[Page[CarteGriseV1Document]]
     """Page-level prediction(s)."""
-    endpoint_name = "us_w9"
+    endpoint_name = "carte_grise"
     """Name of the endpoint."""
     endpoint_version = "1"
     """Version of the endpoint."""
 
     def __init__(self, raw_prediction: StringDict):
         """
-        W9 v1 inference.
+        Carte Grise v1 inference.
 
         :param raw_prediction: Raw prediction from the HTTP response.
         """
         super().__init__(raw_prediction)
 
-        self.prediction = W9V1Document(raw_prediction["prediction"])
+        self.prediction = CarteGriseV1Document(raw_prediction["prediction"])
         self.pages = []
         for page in raw_prediction["pages"]:
             try:
                 page_production = page["prediction"]
             except KeyError:
                 continue
             if page_production:
-                self.pages.append(Page(W9V1Page, page))
+                self.pages.append(Page(CarteGriseV1Document, page))
```

### Comparing `mindee-4.5.0/mindee/product/us/w9/w9_v1_page.py` & `mindee-4.6.0/mindee/product/us/w9/w9_v1_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Optional
 
 from mindee.parsing.common import StringDict, clean_out_string
 from mindee.parsing.standard import PositionField, StringField
-from mindee.product.us.w9.w9_v1_document import W9V1Document
+from mindee.product.us.w9.w9_v1_document import (
+    W9V1Document,
+)
 
 
 class W9V1Page(W9V1Document):
-    """Page data for W9, API version 1."""
+    """W9 API version 1.0 page data."""
 
     address: StringField
     """The street address (number, street, and apt. or suite no.) of the applicant."""
     business_name: StringField
     """The business name or disregarded entity name, if different from Name."""
     city_state_zip: StringField
     """The city, state, and ZIP code of the applicant."""
```

### Comparing `mindee-4.5.0/mindee/versions.py` & `mindee-4.6.0/mindee/versions.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/mindee.egg-info/PKG-INFO` & `mindee-4.6.0/mindee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 4.5.0
+Version: 4.6.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: opensource@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-4.5.0/mindee.egg-info/SOURCES.txt` & `mindee-4.6.0/mindee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/pyproject.toml` & `mindee-4.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/setup.cfg` & `mindee-4.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/fields/test_amount.py` & `mindee-4.6.0/tests/fields/test_amount.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/fields/test_date.py` & `mindee-4.6.0/tests/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/fields/test_field.py` & `mindee-4.6.0/tests/fields/test_field.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/fields/test_locale.py` & `mindee-4.6.0/tests/fields/test_locale.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/fields/test_orientation.py` & `mindee-4.6.0/tests/fields/test_orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/fields/test_payment_details.py` & `mindee-4.6.0/tests/fields/test_payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/fields/test_position.py` & `mindee-4.6.0/tests/fields/test_position.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/fields/test_tax.py` & `mindee-4.6.0/tests/fields/test_tax.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/fields/test_text.py` & `mindee-4.6.0/tests/fields/test_text.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/__init__.py` & `mindee-4.6.0/tests/product/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/barcode_reader/test_barcode_reader_v1.py` & `mindee-4.6.0/tests/product/cropper/test_cropper_v1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
-from mindee.product import BarcodeReaderV1
-from mindee.product.barcode_reader.barcode_reader_v1_document import (
-    BarcodeReaderV1Document,
+from mindee.product import CropperV1
+from mindee.product.cropper.cropper_v1_document import (
+    CropperV1Document,
+)
+from mindee.product.cropper.cropper_v1_page import (
+    CropperV1Page,
 )
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "cropper" / "response_v1"
+
+CropperV1DocumentType = Document[
+    CropperV1Document,
+    Page[CropperV1Page],
+]
+
 
 @pytest.fixture
-def complete_doc() -> Document[BarcodeReaderV1Document, Page[BarcodeReaderV1Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "barcode_reader" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(BarcodeReaderV1, json_data["document"])
+def complete_doc() -> CropperV1DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(CropperV1, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[BarcodeReaderV1Document, Page[BarcodeReaderV1Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "barcode_reader" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(BarcodeReaderV1, json_data["document"])
+def empty_doc() -> CropperV1DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(CropperV1, json_data["document"])
 
 
 @pytest.fixture
-def complete_page_0() -> Page[BarcodeReaderV1Document]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "barcode_reader" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(BarcodeReaderV1Document, json_data["document"]["inference"]["pages"][0])
-
-
-def test_complete_doc(
-    complete_doc: Document[BarcodeReaderV1Document, Page[BarcodeReaderV1Document]]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "barcode_reader" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def complete_page0() -> Page[CropperV1Page]:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    page0 = json_data["document"]["inference"]["pages"][0]
+    return Page(CropperV1Page, page0)
+
+
+def test_complete_doc(complete_doc: CropperV1DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(
-    empty_doc: Document[BarcodeReaderV1Document, Page[BarcodeReaderV1Document]]
-):
-    prediction = empty_doc.inference.prediction
-    assert len(prediction.codes_1d) == 0
-    assert len(prediction.codes_2d) == 0
+def test_empty_doc(empty_doc: CropperV1DocumentType):
+    prediction = empty_doc.inference.pages[0].prediction
+    assert len(prediction.cropping) == 0
+
+
+def test_complete_page0(complete_page0: Page[CropperV1Page]):
+    file_path = RESPONSE_DIR / "summary_page0.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
+    assert complete_page0.id == 0
+    assert str(complete_page0) == reference_str
```

### Comparing `mindee-4.5.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py` & `mindee-4.6.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/cropper/test_cropper_v1.py` & `mindee-4.6.0/tests/product/us/driver_license/test_driver_license_v1.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,82 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
-from mindee.product import CropperV1
-from mindee.product.cropper.cropper_v1_document import CropperV1Document
-from mindee.product.cropper.cropper_v1_page import CropperV1Page
+from mindee.product.us import DriverLicenseV1
+from mindee.product.us.driver_license.driver_license_v1_document import (
+    DriverLicenseV1Document,
+)
+from mindee.product.us.driver_license.driver_license_v1_page import (
+    DriverLicenseV1Page,
+)
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "us_driver_license" / "response_v1"
+
+DriverLicenseV1DocumentType = Document[
+    DriverLicenseV1Document,
+    Page[DriverLicenseV1Page],
+]
+
 
 @pytest.fixture
-def complete_doc() -> Document[CropperV1Document, Page[CropperV1Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "cropper" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(CropperV1, json_data["document"])
+def complete_doc() -> DriverLicenseV1DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(DriverLicenseV1, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[CropperV1Document, Page[CropperV1Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "cropper" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(CropperV1, json_data["document"])
+def empty_doc() -> DriverLicenseV1DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(DriverLicenseV1, json_data["document"])
 
 
 @pytest.fixture
-def complete_page_0() -> Page[CropperV1Page]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "cropper" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(CropperV1Page, json_data["document"]["inference"]["pages"][0])
-
-
-def test_complete_doc(complete_doc: Document[CropperV1Document, Page[CropperV1Page]]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "cropper" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
-    assert str(complete_doc) == reference_str
+def complete_page0() -> Page[DriverLicenseV1Page]:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    page0 = json_data["document"]["inference"]["pages"][0]
+    return Page(DriverLicenseV1Page, page0)
 
 
-def test_empty_doc(empty_doc: Document[CropperV1Document, Page[CropperV1Page]]):
-    prediction = empty_doc.inference.pages[0].prediction
-    assert len(prediction.cropping) == 0
+def test_complete_doc(complete_doc: DriverLicenseV1DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
+    assert str(complete_doc) == reference_str
 
 
-def test_complete_page_0(complete_page_0: Page[CropperV1Page]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "cropper" / "response_v1" / "summary_page0.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
-    assert complete_page_0.id == 0
-    assert str(complete_page_0) == reference_str
+def test_empty_doc(empty_doc: DriverLicenseV1DocumentType):
+    prediction = empty_doc.inference.prediction
+    assert prediction.state.value is None
+    assert prediction.driver_license_id.value is None
+    assert prediction.expiry_date.value is None
+    assert prediction.issued_date.value is None
+    assert prediction.last_name.value is None
+    assert prediction.first_name.value is None
+    assert prediction.address.value is None
+    assert prediction.date_of_birth.value is None
+    assert prediction.restrictions.value is None
+    assert prediction.endorsements.value is None
+    assert prediction.dl_class.value is None
+    assert prediction.sex.value is None
+    assert prediction.height.value is None
+    assert prediction.weight.value is None
+    assert prediction.hair_color.value is None
+    assert prediction.eye_color.value is None
+    assert prediction.dd_number.value is None
+
+
+def test_complete_page0(complete_page0: Page[DriverLicenseV1Page]):
+    file_path = RESPONSE_DIR / "summary_page0.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
+    assert complete_page0.id == 0
+    assert str(complete_page0) == reference_str
```

### Comparing `mindee-4.5.0/tests/product/cropper/test_cropper_v1_regression.py` & `mindee-4.6.0/tests/product/cropper/test_cropper_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/eu/driver_license/test_driver_license_v1.py` & `mindee-4.6.0/tests/product/eu/driver_license/test_driver_license_v1.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,65 +4,60 @@
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
 from mindee.product.eu import DriverLicenseV1
 from mindee.product.eu.driver_license.driver_license_v1_document import (
     DriverLicenseV1Document,
 )
-from mindee.product.eu.driver_license.driver_license_v1_page import DriverLicenseV1Page
+from mindee.product.eu.driver_license.driver_license_v1_page import (
+    DriverLicenseV1Page,
+)
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "eu_driver_license" / "response_v1"
+
+DriverLicenseV1DocumentType = Document[
+    DriverLicenseV1Document,
+    Page[DriverLicenseV1Page],
+]
+
 
 @pytest.fixture
-def complete_doc() -> Document[DriverLicenseV1Document, Page[DriverLicenseV1Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "eu_driver_license" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
+def complete_doc() -> DriverLicenseV1DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(DriverLicenseV1, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[DriverLicenseV1Document, Page[DriverLicenseV1Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "eu_driver_license" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
+def empty_doc() -> DriverLicenseV1DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(DriverLicenseV1, json_data["document"])
 
 
 @pytest.fixture
-def complete_page_0() -> Page[DriverLicenseV1Page]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "eu_driver_license" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(DriverLicenseV1Page, json_data["document"]["inference"]["pages"][0])
-
-
-def test_complete_doc(
-    complete_doc: Document[DriverLicenseV1Document, Page[DriverLicenseV1Page]]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "eu_driver_license" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def complete_page0() -> Page[DriverLicenseV1Page]:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    page0 = json_data["document"]["inference"]["pages"][0]
+    return Page(DriverLicenseV1Page, page0)
+
+
+def test_complete_doc(complete_doc: DriverLicenseV1DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(
-    empty_doc: Document[DriverLicenseV1Document, Page[DriverLicenseV1Page]]
-):
+def test_empty_doc(empty_doc: DriverLicenseV1DocumentType):
     prediction = empty_doc.inference.prediction
     assert prediction.country_code.value is None
     assert prediction.document_id.value is None
     assert prediction.category.value is None
     assert prediction.last_name.value is None
     assert prediction.first_name.value is None
     assert prediction.date_of_birth.value is None
@@ -70,15 +65,13 @@
     assert prediction.expiry_date.value is None
     assert prediction.issue_date.value is None
     assert prediction.issue_authority.value is None
     assert prediction.mrz.value is None
     assert prediction.address.value is None
 
 
-def test_complete_page_0(complete_page_0: Page[DriverLicenseV1Page]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "eu_driver_license" / "response_v1" / "summary_page0.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
-    assert complete_page_0.id == 0
-    assert str(complete_page_0) == reference_str
+def test_complete_page0(complete_page0: Page[DriverLicenseV1Page]):
+    file_path = RESPONSE_DIR / "summary_page0.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
+    assert complete_page0.id == 0
+    assert str(complete_page0) == reference_str
```

### Comparing `mindee-4.5.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py` & `mindee-4.6.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py` & `mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py` & `mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,72 +6,46 @@
 from mindee.parsing.common.page import Page
 from mindee.product.fr import BankAccountDetailsV2
 from mindee.product.fr.bank_account_details.bank_account_details_v2_document import (
     BankAccountDetailsV2Document,
 )
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "bank_account_details" / "response_v2"
+
+BankAccountDetailsV2DocumentType = Document[
+    BankAccountDetailsV2Document,
+    Page[BankAccountDetailsV2Document],
+]
+
 
 @pytest.fixture
-def complete_doc() -> (
-    Document[BankAccountDetailsV2Document, Page[BankAccountDetailsV2Document]]
-):
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "bank_account_details" / "response_v2" / "complete.json",
-            encoding="utf-8",
-        )
-    )
+def complete_doc() -> BankAccountDetailsV2DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(BankAccountDetailsV2, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> (
-    Document[BankAccountDetailsV2Document, Page[BankAccountDetailsV2Document]]
-):
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "bank_account_details" / "response_v2" / "empty.json",
-            encoding="utf-8",
-        )
-    )
+def empty_doc() -> BankAccountDetailsV2DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(BankAccountDetailsV2, json_data["document"])
 
 
-@pytest.fixture
-def complete_page_0() -> Page[BankAccountDetailsV2Document]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "bank_account_details" / "response_v2" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(
-        BankAccountDetailsV2Document, json_data["document"]["inference"]["pages"][0]
-    )
-
-
-def test_complete_doc(
-    complete_doc: Document[
-        BankAccountDetailsV2Document, Page[BankAccountDetailsV2Document]
-    ]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "bank_account_details" / "response_v2" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def test_complete_doc(complete_doc: BankAccountDetailsV2DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(
-    empty_doc: Document[
-        BankAccountDetailsV2Document, Page[BankAccountDetailsV2Document]
-    ]
-):
+def test_empty_doc(empty_doc: BankAccountDetailsV2DocumentType):
     prediction = empty_doc.inference.prediction
     assert prediction.account_holders_names.value is None
     assert prediction.bban.bban_bank_code is None
     assert prediction.bban.bban_branch_code is None
     assert prediction.bban.bban_key is None
     assert prediction.bban.bban_number is None
     assert prediction.iban.value is None
```

### Comparing `mindee-4.5.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py` & `mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py` & `mindee-4.6.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py` & `mindee-4.6.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/fr/id_card/test_id_card_v1.py` & `mindee-4.6.0/tests/product/international_id/test_international_id_v1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
-from mindee.product.fr import IdCardV1
-from mindee.product.fr.id_card.id_card_v1_document import IdCardV1Document
-from mindee.product.fr.id_card.id_card_v1_page import IdCardV1Page
+from mindee.product import InternationalIdV1
+from mindee.product.international_id.international_id_v1_document import (
+    InternationalIdV1Document,
+)
 from tests.product import PRODUCT_DATA_DIR
 
 
 @pytest.fixture
-def complete_doc() -> Document[IdCardV1Document, Page[IdCardV1Page]]:
+def complete_doc() -> (
+    Document[InternationalIdV1Document, Page[InternationalIdV1Document]]
+):
     json_data = json.load(
         open(
-            PRODUCT_DATA_DIR / "idcard_fr" / "response_v1" / "complete.json",
+            PRODUCT_DATA_DIR / "international_id" / "response_v1" / "complete.json",
             encoding="utf-8",
         )
     )
-    return Document(IdCardV1, json_data["document"])
+    return Document(InternationalIdV1, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[IdCardV1Document, Page[IdCardV1Page]]:
+def empty_doc() -> Document[InternationalIdV1Document, Page[InternationalIdV1Document]]:
     json_data = json.load(
         open(
-            PRODUCT_DATA_DIR / "idcard_fr" / "response_v1" / "empty.json",
+            PRODUCT_DATA_DIR / "international_id" / "response_v1" / "empty.json",
             encoding="utf-8",
         )
     )
-    return Document(IdCardV1, json_data["document"])
+    return Document(InternationalIdV1, json_data["document"])
 
 
 @pytest.fixture
-def complete_page_0() -> Page[IdCardV1Page]:
+def complete_page_0() -> Page[InternationalIdV1Document]:
     json_data = json.load(
         open(
-            PRODUCT_DATA_DIR / "idcard_fr" / "response_v1" / "complete.json",
+            PRODUCT_DATA_DIR / "international_id" / "response_v1" / "complete.json",
             encoding="utf-8",
         )
     )
-    return Page(IdCardV1Page, json_data["document"]["inference"]["pages"][0])
+    return Page(
+        InternationalIdV1Document, json_data["document"]["inference"]["pages"][0]
+    )
 
 
-def test_complete_doc(complete_doc: Document[IdCardV1Document, Page[IdCardV1Page]]):
+def test_complete_doc(
+    complete_doc: Document[InternationalIdV1Document, Page[InternationalIdV1Document]]
+):
     reference_str = open(
-        PRODUCT_DATA_DIR / "idcard_fr" / "response_v1" / "summary_full.rst",
+        PRODUCT_DATA_DIR / "international_id" / "response_v1" / "summary_full.rst",
         "r",
         encoding="utf-8",
     ).read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(empty_doc: Document[IdCardV1Document, Page[IdCardV1Page]]):
+def test_empty_doc(
+    empty_doc: Document[InternationalIdV1Document, Page[InternationalIdV1Document]]
+):
     prediction = empty_doc.inference.prediction
-    assert prediction.id_number.value is None
+    assert prediction.document_number.value is None
+    assert prediction.country_of_issue.value is None
+    assert len(prediction.surnames) == 0
     assert len(prediction.given_names) == 0
-    assert prediction.surname.value is None
+    assert prediction.sex.value is None
     assert prediction.birth_date.value is None
     assert prediction.birth_place.value is None
+    assert prediction.nationality.value is None
+    assert prediction.issue_date.value is None
     assert prediction.expiry_date.value is None
-    assert prediction.authority.value is None
-    assert prediction.gender.value is None
+    assert prediction.address.value is None
     assert prediction.mrz1.value is None
     assert prediction.mrz2.value is None
-
-
-def test_complete_page_0(complete_page_0: Page[IdCardV1Page]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "idcard_fr" / "response_v1" / "summary_page0.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
-    assert complete_page_0.id == 0
-    assert str(complete_page_0) == reference_str
+    assert prediction.mrz3.value is None
```

### Comparing `mindee-4.5.0/tests/product/fr/id_card/test_id_card_v1_regression.py` & `mindee-4.6.0/tests/product/fr/id_card/test_id_card_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/fr/id_card/test_id_card_v2.py` & `mindee-4.6.0/tests/product/fr/id_card/test_id_card_v1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,75 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
-from mindee.product.fr import IdCardV2
-from mindee.product.fr.id_card.id_card_v2_document import IdCardV2Document
-from mindee.product.fr.id_card.id_card_v2_page import IdCardV2Page
+from mindee.product.fr import IdCardV1
+from mindee.product.fr.id_card.id_card_v1_document import (
+    IdCardV1Document,
+)
+from mindee.product.fr.id_card.id_card_v1_page import (
+    IdCardV1Page,
+)
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "idcard_fr" / "response_v1"
+
+IdCardV1DocumentType = Document[
+    IdCardV1Document,
+    Page[IdCardV1Page],
+]
+
 
 @pytest.fixture
-def complete_doc() -> Document[IdCardV2Document, Page[IdCardV2Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "idcard_fr" / "response_v2" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(IdCardV2, json_data["document"])
+def complete_doc() -> IdCardV1DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(IdCardV1, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[IdCardV2Document, Page[IdCardV2Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "idcard_fr" / "response_v2" / "empty.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(IdCardV2, json_data["document"])
+def empty_doc() -> IdCardV1DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(IdCardV1, json_data["document"])
 
 
 @pytest.fixture
-def complete_page_0() -> Page[IdCardV2Page]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "idcard_fr" / "response_v2" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(IdCardV2Page, json_data["document"]["inference"]["pages"][0])
-
-
-def test_complete_doc(complete_doc: Document[IdCardV2Document, Page[IdCardV2Page]]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "idcard_fr" / "response_v2" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def complete_page0() -> Page[IdCardV1Page]:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    page0 = json_data["document"]["inference"]["pages"][0]
+    return Page(IdCardV1Page, page0)
+
+
+def test_complete_doc(complete_doc: IdCardV1DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(empty_doc: Document[IdCardV2Document, Page[IdCardV2Page]]):
+def test_empty_doc(empty_doc: IdCardV1DocumentType):
     prediction = empty_doc.inference.prediction
-    assert prediction.nationality.value is None
-    assert prediction.card_access_number.value is None
-    assert prediction.document_number.value is None
+    assert prediction.id_number.value is None
     assert len(prediction.given_names) == 0
     assert prediction.surname.value is None
-    assert prediction.alternate_name.value is None
     assert prediction.birth_date.value is None
     assert prediction.birth_place.value is None
-    assert prediction.gender.value is None
     assert prediction.expiry_date.value is None
+    assert prediction.authority.value is None
+    assert prediction.gender.value is None
     assert prediction.mrz1.value is None
     assert prediction.mrz2.value is None
-    assert prediction.mrz3.value is None
-    assert prediction.issue_date.value is None
-    assert prediction.authority.value is None
 
 
-def test_complete_page_0(complete_page_0: Page[IdCardV2Page]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "idcard_fr" / "response_v2" / "summary_page0.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
-    assert complete_page_0.id == 0
-    assert str(complete_page_0) == reference_str
+def test_complete_page0(complete_page0: Page[IdCardV1Page]):
+    file_path = RESPONSE_DIR / "summary_page0.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
+    assert complete_page0.id == 0
+    assert str(complete_page0) == reference_str
```

### Comparing `mindee-4.5.0/tests/product/fr/id_card/test_id_card_v2_regression.py` & `mindee-4.6.0/tests/product/fr/id_card/test_id_card_v2_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/international_id/test_international_id_v1.py` & `mindee-4.6.0/tests/product/us/w9/test_w9_v1.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,77 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
-from mindee.product import InternationalIdV1
-from mindee.product.international_id.international_id_v1_document import (
-    InternationalIdV1Document,
+from mindee.product.us import W9V1
+from mindee.product.us.w9.w9_v1_document import (
+    W9V1Document,
+)
+from mindee.product.us.w9.w9_v1_page import (
+    W9V1Page,
 )
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "us_w9" / "response_v1"
+
+W9V1DocumentType = Document[
+    W9V1Document,
+    Page[W9V1Page],
+]
+
 
 @pytest.fixture
-def complete_doc() -> (
-    Document[InternationalIdV1Document, Page[InternationalIdV1Document]]
-):
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "international_id" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(InternationalIdV1, json_data["document"])
+def complete_doc() -> W9V1DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(W9V1, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[InternationalIdV1Document, Page[InternationalIdV1Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "international_id" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(InternationalIdV1, json_data["document"])
+def empty_doc() -> W9V1DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(W9V1, json_data["document"])
 
 
 @pytest.fixture
-def complete_page_0() -> Page[InternationalIdV1Document]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "international_id" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(
-        InternationalIdV1Document, json_data["document"]["inference"]["pages"][0]
-    )
-
-
-def test_complete_doc(
-    complete_doc: Document[InternationalIdV1Document, Page[InternationalIdV1Document]]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "international_id" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def complete_page0() -> Page[W9V1Page]:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    page0 = json_data["document"]["inference"]["pages"][0]
+    return Page(W9V1Page, page0)
+
+
+def test_complete_doc(complete_doc: W9V1DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(
-    empty_doc: Document[InternationalIdV1Document, Page[InternationalIdV1Document]]
-):
-    prediction = empty_doc.inference.prediction
-    assert prediction.document_number.value is None
-    assert prediction.country_of_issue.value is None
-    assert len(prediction.surnames) == 0
-    assert len(prediction.given_names) == 0
-    assert prediction.sex.value is None
-    assert prediction.birth_date.value is None
-    assert prediction.birth_place.value is None
-    assert prediction.nationality.value is None
-    assert prediction.issue_date.value is None
-    assert prediction.expiry_date.value is None
+def test_empty_doc(empty_doc: W9V1DocumentType):
+    prediction = empty_doc.inference.pages[0].prediction
+    assert prediction.name.value is None
+    assert prediction.ssn.value is None
     assert prediction.address.value is None
-    assert prediction.mrz1.value is None
-    assert prediction.mrz2.value is None
-    assert prediction.mrz3.value is None
+    assert prediction.city_state_zip.value is None
+    assert prediction.business_name.value is None
+    assert prediction.ein.value is None
+    assert prediction.tax_classification.value is None
+    assert prediction.tax_classification_other_details.value is None
+    assert prediction.w9_revision_date.value is None
+    assert not prediction.signature_position.polygon
+    assert not prediction.signature_date_position.polygon
+    assert prediction.tax_classification_llc.value is None
+
+
+def test_complete_page0(complete_page0: Page[W9V1Page]):
+    file_path = RESPONSE_DIR / "summary_page0.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
+    assert complete_page0.id == 0
+    assert str(complete_page0) == reference_str
```

### Comparing `mindee-4.5.0/tests/product/international_id/test_international_id_v2.py` & `mindee-4.6.0/tests/product/international_id/test_international_id_v2.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,66 +6,46 @@
 from mindee.parsing.common.page import Page
 from mindee.product import InternationalIdV2
 from mindee.product.international_id.international_id_v2_document import (
     InternationalIdV2Document,
 )
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "international_id" / "response_v2"
+
+InternationalIdV2DocumentType = Document[
+    InternationalIdV2Document,
+    Page[InternationalIdV2Document],
+]
+
 
 @pytest.fixture
-def complete_doc() -> (
-    Document[InternationalIdV2Document, Page[InternationalIdV2Document]]
-):
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "international_id" / "response_v2" / "complete.json",
-            encoding="utf-8",
-        )
-    )
+def complete_doc() -> InternationalIdV2DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(InternationalIdV2, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[InternationalIdV2Document, Page[InternationalIdV2Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "international_id" / "response_v2" / "empty.json",
-            encoding="utf-8",
-        )
-    )
+def empty_doc() -> InternationalIdV2DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(InternationalIdV2, json_data["document"])
 
 
-@pytest.fixture
-def complete_page_0() -> Page[InternationalIdV2Document]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "international_id" / "response_v2" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(
-        InternationalIdV2Document, json_data["document"]["inference"]["pages"][0]
-    )
-
-
-def test_complete_doc(
-    complete_doc: Document[InternationalIdV2Document, Page[InternationalIdV2Document]]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "international_id" / "response_v2" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def test_complete_doc(complete_doc: InternationalIdV2DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(
-    empty_doc: Document[InternationalIdV2Document, Page[InternationalIdV2Document]]
-):
+def test_empty_doc(empty_doc: InternationalIdV2DocumentType):
     prediction = empty_doc.inference.prediction
     assert prediction.document_number.value is None
     assert len(prediction.surnames) == 0
     assert len(prediction.given_names) == 0
     assert prediction.sex.value is None
     assert prediction.birth_date.value is None
     assert prediction.birth_place.value is None
```

### Comparing `mindee-4.5.0/tests/product/invoice/test_invoice_v4.py` & `mindee-4.6.0/tests/product/invoice/test_invoice_v4.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,68 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
 from mindee.product import InvoiceV4
-from mindee.product.invoice.invoice_v4_document import InvoiceV4Document
+from mindee.product.invoice.invoice_v4_document import (
+    InvoiceV4Document,
+)
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "invoices" / "response_v4"
+
+InvoiceV4DocumentType = Document[
+    InvoiceV4Document,
+    Page[InvoiceV4Document],
+]
+
 
 @pytest.fixture
-def complete_doc() -> Document[InvoiceV4Document, Page[InvoiceV4Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "invoices" / "response_v4" / "complete.json",
-            encoding="utf-8",
-        )
-    )
+def complete_doc() -> InvoiceV4DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(InvoiceV4, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[InvoiceV4Document, Page[InvoiceV4Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "invoices" / "response_v4" / "empty.json",
-            encoding="utf-8",
-        )
-    )
+def empty_doc() -> InvoiceV4DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(InvoiceV4, json_data["document"])
 
 
-@pytest.fixture
-def complete_page_0() -> Page[InvoiceV4Document]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "invoices" / "response_v4" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(InvoiceV4Document, json_data["document"]["inference"]["pages"][0])
-
-
-def test_complete_doc(
-    complete_doc: Document[InvoiceV4Document, Page[InvoiceV4Document]]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "invoices" / "response_v4" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def test_complete_doc(complete_doc: InvoiceV4DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(empty_doc: Document[InvoiceV4Document, Page[InvoiceV4Document]]):
+def test_empty_doc(empty_doc: InvoiceV4DocumentType):
     prediction = empty_doc.inference.prediction
     assert prediction.locale.value is None
     assert prediction.invoice_number.value is None
     assert len(prediction.reference_numbers) == 0
     assert prediction.date.value is None
     assert prediction.due_date.value is None
     assert prediction.total_net.value is None
     assert prediction.total_amount.value is None
     assert prediction.total_tax.value is None
     assert len(prediction.taxes) == 0
     assert len(prediction.supplier_payment_details) == 0
     assert prediction.supplier_name.value is None
     assert len(prediction.supplier_company_registrations) == 0
     assert prediction.supplier_address.value is None
+    assert prediction.supplier_phone_number.value is None
+    assert prediction.supplier_website.value is None
+    assert prediction.supplier_email.value is None
     assert prediction.customer_name.value is None
     assert len(prediction.customer_company_registrations) == 0
     assert prediction.customer_address.value is None
+    assert prediction.customer_id.value is None
     assert prediction.shipping_address.value is None
     assert prediction.billing_address.value is None
     assert len(prediction.line_items) == 0
```

### Comparing `mindee-4.5.0/tests/product/invoice/test_invoice_v4_regression.py` & `mindee-4.6.0/tests/product/invoice/test_invoice_v4_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/material_certificate/test_material_certificate_v1.py` & `mindee-4.6.0/tests/product/material_certificate/test_material_certificate_v1.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,69 +6,43 @@
 from mindee.parsing.common.page import Page
 from mindee.product import MaterialCertificateV1
 from mindee.product.material_certificate.material_certificate_v1_document import (
     MaterialCertificateV1Document,
 )
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "material_certificate" / "response_v1"
+
+MaterialCertificateV1DocumentType = Document[
+    MaterialCertificateV1Document,
+    Page[MaterialCertificateV1Document],
+]
+
 
 @pytest.fixture
-def complete_doc() -> (
-    Document[MaterialCertificateV1Document, Page[MaterialCertificateV1Document]]
-):
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "material_certificate" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
+def complete_doc() -> MaterialCertificateV1DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(MaterialCertificateV1, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> (
-    Document[MaterialCertificateV1Document, Page[MaterialCertificateV1Document]]
-):
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "material_certificate" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
+def empty_doc() -> MaterialCertificateV1DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(MaterialCertificateV1, json_data["document"])
 
 
-@pytest.fixture
-def complete_page_0() -> Page[MaterialCertificateV1Document]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "material_certificate" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(
-        MaterialCertificateV1Document, json_data["document"]["inference"]["pages"][0]
-    )
-
-
-def test_complete_doc(
-    complete_doc: Document[
-        MaterialCertificateV1Document, Page[MaterialCertificateV1Document]
-    ]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "material_certificate" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def test_complete_doc(complete_doc: MaterialCertificateV1DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(
-    empty_doc: Document[
-        MaterialCertificateV1Document, Page[MaterialCertificateV1Document]
-    ]
-):
+def test_empty_doc(empty_doc: MaterialCertificateV1DocumentType):
     prediction = empty_doc.inference.prediction
     assert prediction.certificate_type.value is None
     assert prediction.norm.value is None
     assert prediction.heat_number.value is None
```

### Comparing `mindee-4.5.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py` & `mindee-4.6.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/passport/test_passport_v1.py` & `mindee-4.6.0/tests/product/passport/test_passport_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,51 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
 from mindee.product import PassportV1
-from mindee.product.passport.passport_v1_document import PassportV1Document
+from mindee.product.passport.passport_v1_document import (
+    PassportV1Document,
+)
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "passport" / "response_v1"
+
+PassportV1DocumentType = Document[
+    PassportV1Document,
+    Page[PassportV1Document],
+]
+
 
 @pytest.fixture
-def complete_doc() -> Document[PassportV1Document, Page[PassportV1Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "passport" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
+def complete_doc() -> PassportV1DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(PassportV1, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[PassportV1Document, Page[PassportV1Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "passport" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
+def empty_doc() -> PassportV1DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(PassportV1, json_data["document"])
 
 
-@pytest.fixture
-def complete_page_0() -> Page[PassportV1Document]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "passport" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(PassportV1Document, json_data["document"]["inference"]["pages"][0])
-
-
-def test_complete_doc(
-    complete_doc: Document[PassportV1Document, Page[PassportV1Document]]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "passport" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def test_complete_doc(complete_doc: PassportV1DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(empty_doc: Document[PassportV1Document, Page[PassportV1Document]]):
+def test_empty_doc(empty_doc: PassportV1DocumentType):
     prediction = empty_doc.inference.prediction
     assert prediction.country.value is None
     assert prediction.id_number.value is None
     assert len(prediction.given_names) == 0
     assert prediction.surname.value is None
     assert prediction.birth_date.value is None
     assert prediction.birth_place.value is None
```

### Comparing `mindee-4.5.0/tests/product/passport/test_passport_v1_regression.py` & `mindee-4.6.0/tests/product/passport/test_passport_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/proof_of_address/test_proof_of_address_v1.py` & `mindee-4.6.0/tests/product/proof_of_address/test_proof_of_address_v1.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,66 +6,46 @@
 from mindee.parsing.common.page import Page
 from mindee.product import ProofOfAddressV1
 from mindee.product.proof_of_address.proof_of_address_v1_document import (
     ProofOfAddressV1Document,
 )
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "proof_of_address" / "response_v1"
+
+ProofOfAddressV1DocumentType = Document[
+    ProofOfAddressV1Document,
+    Page[ProofOfAddressV1Document],
+]
+
 
 @pytest.fixture
-def complete_doc() -> (
-    Document[ProofOfAddressV1Document, Page[ProofOfAddressV1Document]]
-):
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "proof_of_address" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
+def complete_doc() -> ProofOfAddressV1DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(ProofOfAddressV1, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[ProofOfAddressV1Document, Page[ProofOfAddressV1Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "proof_of_address" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
+def empty_doc() -> ProofOfAddressV1DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(ProofOfAddressV1, json_data["document"])
 
 
-@pytest.fixture
-def complete_page_0() -> Page[ProofOfAddressV1Document]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "proof_of_address" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(
-        ProofOfAddressV1Document, json_data["document"]["inference"]["pages"][0]
-    )
-
-
-def test_complete_doc(
-    complete_doc: Document[ProofOfAddressV1Document, Page[ProofOfAddressV1Document]]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "proof_of_address" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def test_complete_doc(complete_doc: ProofOfAddressV1DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(
-    empty_doc: Document[ProofOfAddressV1Document, Page[ProofOfAddressV1Document]]
-):
+def test_empty_doc(empty_doc: ProofOfAddressV1DocumentType):
     prediction = empty_doc.inference.prediction
     assert prediction.locale.value is None
     assert prediction.issuer_name.value is None
     assert len(prediction.issuer_company_registration) == 0
     assert prediction.issuer_address.value is None
     assert prediction.recipient_name.value is None
     assert len(prediction.recipient_company_registration) == 0
```

### Comparing `mindee-4.5.0/tests/product/receipt/test_receipt_v4.py` & `mindee-4.6.0/tests/product/receipt/test_receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/receipt/test_receipt_v4_regression.py` & `mindee-4.6.0/tests/product/receipt/test_receipt_v4_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/receipt/test_receipt_v5_regression.py` & `mindee-4.6.0/tests/product/receipt/test_receipt_v5_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/resume/test_resume_v1.py` & `mindee-4.6.0/tests/product/fr/carte_grise/test_carte_grise_v1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,86 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
-from mindee.product import ResumeV1
-from mindee.product.resume.resume_v1_document import ResumeV1Document
+from mindee.product.fr import CarteGriseV1
+from mindee.product.fr.carte_grise.carte_grise_v1_document import (
+    CarteGriseV1Document,
+)
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "carte_grise" / "response_v1"
 
-@pytest.fixture
-def complete_doc() -> Document[ResumeV1Document, Page[ResumeV1Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "resume" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(ResumeV1, json_data["document"])
+CarteGriseV1DocumentType = Document[
+    CarteGriseV1Document,
+    Page[CarteGriseV1Document],
+]
 
 
 @pytest.fixture
-def empty_doc() -> Document[ResumeV1Document, Page[ResumeV1Document]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "resume" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(ResumeV1, json_data["document"])
+def complete_doc() -> CarteGriseV1DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(CarteGriseV1, json_data["document"])
 
 
 @pytest.fixture
-def complete_page_0() -> Page[ResumeV1Document]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "resume" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(ResumeV1Document, json_data["document"]["inference"]["pages"][0])
-
-
-def test_complete_doc(complete_doc: Document[ResumeV1Document, Page[ResumeV1Document]]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "resume" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def empty_doc() -> CarteGriseV1DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(CarteGriseV1, json_data["document"])
+
+
+def test_complete_doc(complete_doc: CarteGriseV1DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(empty_doc: Document[ResumeV1Document, Page[ResumeV1Document]]):
+def test_empty_doc(empty_doc: CarteGriseV1DocumentType):
     prediction = empty_doc.inference.prediction
-    assert prediction.document_language.value is None
-    assert len(prediction.given_names) == 0
-    assert len(prediction.surnames) == 0
-    assert prediction.nationality.value is None
-    assert prediction.email_address.value is None
-    assert prediction.phone_number.value is None
-    assert prediction.address.value is None
-    assert len(prediction.social_networks_urls) == 0
-    assert prediction.profession.value is None
-    assert prediction.job_applied.value is None
-    assert len(prediction.languages) == 0
-    assert len(prediction.hard_skills) == 0
-    assert len(prediction.soft_skills) == 0
-    assert len(prediction.education) == 0
-    assert len(prediction.professional_experiences) == 0
-    assert len(prediction.certificates) == 0
+    assert prediction.a.value is None
+    assert prediction.b.value is None
+    assert prediction.c1.value is None
+    assert prediction.c3.value is None
+    assert prediction.c41.value is None
+    assert prediction.c4a.value is None
+    assert prediction.d1.value is None
+    assert prediction.d3.value is None
+    assert prediction.e.value is None
+    assert prediction.f1.value is None
+    assert prediction.f2.value is None
+    assert prediction.f3.value is None
+    assert prediction.g.value is None
+    assert prediction.g1.value is None
+    assert prediction.i.value is None
+    assert prediction.j.value is None
+    assert prediction.j1.value is None
+    assert prediction.j2.value is None
+    assert prediction.j3.value is None
+    assert prediction.p1.value is None
+    assert prediction.p2.value is None
+    assert prediction.p3.value is None
+    assert prediction.p6.value is None
+    assert prediction.q.value is None
+    assert prediction.s1.value is None
+    assert prediction.s2.value is None
+    assert prediction.u1.value is None
+    assert prediction.u2.value is None
+    assert prediction.v7.value is None
+    assert prediction.x1.value is None
+    assert prediction.y1.value is None
+    assert prediction.y2.value is None
+    assert prediction.y3.value is None
+    assert prediction.y4.value is None
+    assert prediction.y5.value is None
+    assert prediction.y6.value is None
+    assert prediction.formula_number.value is None
+    assert prediction.owner_first_name.value is None
+    assert prediction.owner_surname.value is None
+    assert prediction.mrz1.value is None
+    assert prediction.mrz2.value is None
```

### Comparing `mindee-4.5.0/tests/product/us/bank_check/test_bank_check_v1.py` & `mindee-4.6.0/tests/product/us/bank_check/test_bank_check_v1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,71 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
 from mindee.product.us import BankCheckV1
-from mindee.product.us.bank_check.bank_check_v1_document import BankCheckV1Document
-from mindee.product.us.bank_check.bank_check_v1_page import BankCheckV1Page
+from mindee.product.us.bank_check.bank_check_v1_document import (
+    BankCheckV1Document,
+)
+from mindee.product.us.bank_check.bank_check_v1_page import (
+    BankCheckV1Page,
+)
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "bank_check" / "response_v1"
+
+BankCheckV1DocumentType = Document[
+    BankCheckV1Document,
+    Page[BankCheckV1Page],
+]
+
 
 @pytest.fixture
-def complete_doc() -> Document[BankCheckV1Document, Page[BankCheckV1Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "bank_check" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
+def complete_doc() -> BankCheckV1DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(BankCheckV1, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[BankCheckV1Document, Page[BankCheckV1Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "bank_check" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
+def empty_doc() -> BankCheckV1DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
     return Document(BankCheckV1, json_data["document"])
 
 
 @pytest.fixture
-def complete_page_0() -> Page[BankCheckV1Page]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "bank_check" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(BankCheckV1Page, json_data["document"]["inference"]["pages"][0])
-
-
-def test_complete_doc(
-    complete_doc: Document[BankCheckV1Document, Page[BankCheckV1Page]]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "bank_check" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def complete_page0() -> Page[BankCheckV1Page]:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    page0 = json_data["document"]["inference"]["pages"][0]
+    return Page(BankCheckV1Page, page0)
+
+
+def test_complete_doc(complete_doc: BankCheckV1DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(empty_doc: Document[BankCheckV1Document, Page[BankCheckV1Page]]):
+def test_empty_doc(empty_doc: BankCheckV1DocumentType):
     prediction = empty_doc.inference.prediction
     assert prediction.date.value is None
     assert prediction.amount.value is None
     assert len(prediction.payees) == 0
     assert prediction.routing_number.value is None
     assert prediction.account_number.value is None
     assert prediction.check_number.value is None
 
 
-def test_complete_page_0(complete_page_0: Page[BankCheckV1Page]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "bank_check" / "response_v1" / "summary_page0.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
-    assert complete_page_0.id == 0
-    assert str(complete_page_0) == reference_str
+def test_complete_page0(complete_page0: Page[BankCheckV1Page]):
+    file_path = RESPONSE_DIR / "summary_page0.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
+    assert complete_page0.id == 0
+    assert str(complete_page0) == reference_str
```

### Comparing `mindee-4.5.0/tests/product/us/bank_check/test_bank_check_v1_regression.py` & `mindee-4.6.0/tests/product/us/bank_check/test_bank_check_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/us/driver_license/test_driver_license_v1.py` & `mindee-4.6.0/tests/product/receipt/test_receipt_v5.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,58 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
-from mindee.product.us import DriverLicenseV1
-from mindee.product.us.driver_license.driver_license_v1_document import (
-    DriverLicenseV1Document,
+from mindee.product import ReceiptV5
+from mindee.product.receipt.receipt_v5_document import (
+    ReceiptV5Document,
 )
-from mindee.product.us.driver_license.driver_license_v1_page import DriverLicenseV1Page
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "expense_receipts" / "response_v5"
 
-@pytest.fixture
-def complete_doc() -> Document[DriverLicenseV1Document, Page[DriverLicenseV1Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "us_driver_license" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(DriverLicenseV1, json_data["document"])
+ReceiptV5DocumentType = Document[
+    ReceiptV5Document,
+    Page[ReceiptV5Document],
+]
 
 
 @pytest.fixture
-def empty_doc() -> Document[DriverLicenseV1Document, Page[DriverLicenseV1Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "us_driver_license" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(DriverLicenseV1, json_data["document"])
+def complete_doc() -> ReceiptV5DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(ReceiptV5, json_data["document"])
 
 
 @pytest.fixture
-def complete_page_0() -> Page[DriverLicenseV1Page]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "us_driver_license" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(DriverLicenseV1Page, json_data["document"]["inference"]["pages"][0])
-
-
-def test_complete_doc(
-    complete_doc: Document[DriverLicenseV1Document, Page[DriverLicenseV1Page]]
-):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "us_driver_license" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def empty_doc() -> ReceiptV5DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(ReceiptV5, json_data["document"])
+
+
+def test_complete_doc(complete_doc: ReceiptV5DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(
-    empty_doc: Document[DriverLicenseV1Document, Page[DriverLicenseV1Page]]
-):
+def test_empty_doc(empty_doc: ReceiptV5DocumentType):
     prediction = empty_doc.inference.prediction
-    assert prediction.state.value is None
-    assert prediction.driver_license_id.value is None
-    assert prediction.expiry_date.value is None
-    assert prediction.issued_date.value is None
-    assert prediction.last_name.value is None
-    assert prediction.first_name.value is None
-    assert prediction.address.value is None
-    assert prediction.date_of_birth.value is None
-    assert prediction.restrictions.value is None
-    assert prediction.endorsements.value is None
-    assert prediction.dl_class.value is None
-    assert prediction.sex.value is None
-    assert prediction.height.value is None
-    assert prediction.weight.value is None
-    assert prediction.hair_color.value is None
-    assert prediction.eye_color.value is None
-    assert prediction.dd_number.value is None
-
-
-def test_complete_page_0(complete_page_0: Page[DriverLicenseV1Page]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "us_driver_license" / "response_v1" / "summary_page0.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
-    assert complete_page_0.id == 0
-    assert str(complete_page_0) == reference_str
+    assert prediction.locale.value is None
+    assert prediction.date.value is None
+    assert prediction.time.value is None
+    assert prediction.total_amount.value is None
+    assert prediction.total_net.value is None
+    assert prediction.total_tax.value is None
+    assert prediction.tip.value is None
+    assert len(prediction.taxes) == 0
+    assert prediction.supplier_name.value is None
+    assert len(prediction.supplier_company_registrations) == 0
+    assert prediction.supplier_address.value is None
+    assert prediction.supplier_phone_number.value is None
+    assert len(prediction.line_items) == 0
```

### Comparing `mindee-4.5.0/tests/product/us/driver_license/test_driver_license_v1_regression.py` & `mindee-4.6.0/tests/product/us/driver_license/test_driver_license_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/product/us/w9/test_w9_v1.py` & `mindee-4.6.0/tests/product/fr/id_card/test_id_card_v2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,80 @@
 import json
 
 import pytest
 
 from mindee.parsing.common.document import Document
 from mindee.parsing.common.page import Page
-from mindee.product.us import W9V1
-from mindee.product.us.w9.w9_v1_document import W9V1Document
-from mindee.product.us.w9.w9_v1_page import W9V1Page
+from mindee.product.fr import IdCardV2
+from mindee.product.fr.id_card.id_card_v2_document import (
+    IdCardV2Document,
+)
+from mindee.product.fr.id_card.id_card_v2_page import (
+    IdCardV2Page,
+)
 from tests.product import PRODUCT_DATA_DIR
 
+RESPONSE_DIR = PRODUCT_DATA_DIR / "idcard_fr" / "response_v2"
+
+IdCardV2DocumentType = Document[
+    IdCardV2Document,
+    Page[IdCardV2Page],
+]
+
 
 @pytest.fixture
-def complete_doc() -> Document[W9V1Document, Page[W9V1Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "us_w9" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(W9V1, json_data["document"])
+def complete_doc() -> IdCardV2DocumentType:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(IdCardV2, json_data["document"])
 
 
 @pytest.fixture
-def empty_doc() -> Document[W9V1Document, Page[W9V1Page]]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "us_w9" / "response_v1" / "empty.json",
-            encoding="utf-8",
-        )
-    )
-    return Document(W9V1, json_data["document"])
+def empty_doc() -> IdCardV2DocumentType:
+    file_path = RESPONSE_DIR / "empty.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    return Document(IdCardV2, json_data["document"])
 
 
 @pytest.fixture
-def complete_page_0() -> Page[W9V1Page]:
-    json_data = json.load(
-        open(
-            PRODUCT_DATA_DIR / "us_w9" / "response_v1" / "complete.json",
-            encoding="utf-8",
-        )
-    )
-    return Page(W9V1Page, json_data["document"]["inference"]["pages"][0])
-
-
-def test_complete_doc(complete_doc: Document[W9V1Document, Page[W9V1Page]]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "us_w9" / "response_v1" / "summary_full.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
+def complete_page0() -> Page[IdCardV2Page]:
+    file_path = RESPONSE_DIR / "complete.json"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        json_data = json.load(open_file)
+    page0 = json_data["document"]["inference"]["pages"][0]
+    return Page(IdCardV2Page, page0)
+
+
+def test_complete_doc(complete_doc: IdCardV2DocumentType):
+    file_path = RESPONSE_DIR / "summary_full.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
     assert str(complete_doc) == reference_str
 
 
-def test_empty_doc(empty_doc: Document[W9V1Document, Page[W9V1Page]]):
-    prediction = empty_doc.inference.pages[0].prediction
-    assert prediction.name.value is None
-    assert prediction.ssn.value is None
-    assert prediction.address.value is None
-    assert prediction.city_state_zip.value is None
-    assert prediction.business_name.value is None
-    assert prediction.ein.value is None
-    assert prediction.tax_classification.value is None
-    assert prediction.tax_classification_other_details.value is None
-    assert prediction.w9_revision_date.value is None
-    assert not prediction.signature_position.polygon
-    assert not prediction.signature_date_position.polygon
-    assert prediction.tax_classification_llc.value is None
-
-
-def test_complete_page_0(complete_page_0: Page[W9V1Page]):
-    reference_str = open(
-        PRODUCT_DATA_DIR / "us_w9" / "response_v1" / "summary_page0.rst",
-        "r",
-        encoding="utf-8",
-    ).read()
-    assert complete_page_0.id == 0
-    assert str(complete_page_0) == reference_str
+def test_empty_doc(empty_doc: IdCardV2DocumentType):
+    prediction = empty_doc.inference.prediction
+    assert prediction.nationality.value is None
+    assert prediction.card_access_number.value is None
+    assert prediction.document_number.value is None
+    assert len(prediction.given_names) == 0
+    assert prediction.surname.value is None
+    assert prediction.alternate_name.value is None
+    assert prediction.birth_date.value is None
+    assert prediction.birth_place.value is None
+    assert prediction.gender.value is None
+    assert prediction.expiry_date.value is None
+    assert prediction.mrz1.value is None
+    assert prediction.mrz2.value is None
+    assert prediction.mrz3.value is None
+    assert prediction.issue_date.value is None
+    assert prediction.authority.value is None
+
+
+def test_complete_page0(complete_page0: Page[IdCardV2Page]):
+    file_path = RESPONSE_DIR / "summary_page0.rst"
+    with open(file_path, "r", encoding="utf-8") as open_file:
+        reference_str = open_file.read()
+    assert complete_page0.id == 0
+    assert str(complete_page0) == reference_str
```

### Comparing `mindee-4.5.0/tests/product/us/w9/test_w9_v1_regression.py` & `mindee-4.6.0/tests/product/us/w9/test_w9_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/test_cli.py` & `mindee-4.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/test_client.py` & `mindee-4.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/test_geometry.py` & `mindee-4.6.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/test_inputs.py` & `mindee-4.6.0/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `mindee-4.5.0/tests/test_pkg_versions.py` & `mindee-4.6.0/tests/test_pkg_versions.py`

 * *Files identical despite different names*

