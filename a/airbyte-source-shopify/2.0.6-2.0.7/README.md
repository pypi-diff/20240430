# Comparing `tmp/airbyte_source_shopify-2.0.6.tar.gz` & `tmp/airbyte_source_shopify-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.0.6.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.0.7.tar", max compression
```

## Comparing `airbyte_source_shopify-2.0.6.tar` & `airbyte_source_shopify-2.0.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     4519 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/README.md
--rw-r--r--   0        0        0      796 2024-04-22 15:05:19.631510 airbyte_source_shopify-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/run.py
--rw-r--r--   0        0        0    16103 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     1272 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     1009 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     1109 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0      928 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0      610 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     1170 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     1488 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     1217 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      485 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0     5313 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0      736 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0      909 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    13381 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     5226 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    14757 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     1027 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0      536 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     1329 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0      911 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    17520 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0      728 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0    80187 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     1104 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     3891 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0      907 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     2336 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0     7060 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     1675 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     4059 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0      985 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0      951 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     3750 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/scopes.py
--rw-r--r--   0        0        0     1734 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    20743 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    56188 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6517 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     3629 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8540 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/spec.json
--rw-r--r--   0        0        0    37097 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11968 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/transform.py
--rw-r--r--   0        0        0    13944 2024-04-22 14:05:45.000000 airbyte_source_shopify-2.0.6/source_shopify/utils.py
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/README.md
+-rw-r--r--   0        0        0      800 2024-04-30 15:28:25.272251 airbyte_source_shopify-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/run.py
+-rw-r--r--   0        0        0    28417 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     2548 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     2135 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     2151 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0     1889 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0     1173 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     2162 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     3100 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     2628 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      986 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0    10233 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0     1621 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0     1775 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    24211 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     9939 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    23930 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     2042 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0     1114 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     2806 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0     1919 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0     1881 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0     1925 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0     1957 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0     2008 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0     1800 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0     1874 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0     1985 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0     1782 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0     1919 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0     2078 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0     1873 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0     1985 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    26296 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0     1549 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0   103922 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     2093 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     7004 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0     1760 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     4650 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0    13110 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     3598 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     8137 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0     2009 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0     2006 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     6603 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/scopes.py
+-rw-r--r--   0        0        0     1734 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    20743 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    56188 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6517 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     3629 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8540 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/spec.json
+-rw-r--r--   0        0        0    37097 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11968 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/transform.py
+-rw-r--r--   0        0        0    13944 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/utils.py
+-rw-r--r--   0        0        0     5305 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.7/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.0.6/README.md` & `airbyte_source_shopify-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/pyproject.toml` & `airbyte_source_shopify-2.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.6"
+version = "2.0.7"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_shopify" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.81.4"
 sgqlc = "==16.3"
 graphql-query = "^1.1.1"
 
 [tool.poetry.scripts]
 source-shopify = "source_shopify.run:run"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/__init__.py` & `airbyte_source_shopify-2.0.7/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/auth.py` & `airbyte_source_shopify-2.0.7/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.0.7/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_locations.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6917735042735043%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier for the metafield'}, 'created_at': "*

 * *                 "{'description': 'The date and time when the metafield was created'}, "*

 * *                 "'updated_at': {'description': 'The date and time when the metafield was last "*

 * *                 "updated'}, 'admin_graphql_api_id': {'description': 'The unique identifier for "*

 * *                 "the metafield in the Shopify GraphQL Admin API'}, 'shop_url': {'description': "*

 * *                 "'The URL of […]*

```diff
@@ -1,118 +1,102 @@
 {
     "additionalProperties": true,
     "properties": {
         "admin_graphql_api_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "author": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "blog_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "body_html": {
+            "description": "The unique identifier for the metafield in the Shopify GraphQL Admin API",
             "type": [
                 "null",
                 "string"
             ]
         },
         "created_at": {
+            "description": "The date and time when the metafield was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "deleted_at": {
-            "format": "date-time",
+        "description": {
+            "description": "The description of the metafield",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "deleted_description": {
+        "id": {
+            "description": "The unique identifier for the metafield",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "deleted_message": {
+        "key": {
+            "description": "The key or name of the metafield",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "handle": {
+        "namespace": {
+            "description": "The namespace of the metafield",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "id": {
+        "owner_id": {
+            "description": "The unique identifier of the resource that owns the metafield",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "published_at": {
-            "format": "date-time",
+        "owner_resource": {
+            "description": "The type of resource that owns the metafield",
             "type": [
                 "null",
                 "string"
             ]
         },
         "shop_url": {
+            "description": "The URL of the shop where the metafield is associated",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "summary_html": {
+        "type": {
+            "description": "The type of the metafield value",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tags": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "template_suffix": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "title": {
+        "updated_at": {
+            "description": "The date and time when the metafield was last updated",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "value": {
+            "description": "The actual value of the metafield",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "user_id": {
+        "value_type": {
+            "description": "The data type of the metafield value",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "type": "object"
+    "type": [
+        "null",
+        "object"
+    ]
 }
```

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.0.7/source_shopify/schemas/disputes.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6708333333333334%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier of the dispute'}, 'order_id': "*

 * *                 "OrderedDict([('description', 'The identifier of the order associated with the "*

 * *                 "dispute'), ('type', ['null', 'integer'])]), 'type': OrderedDict([('description', "*

 * *                 "'The type of dispute (e.g., chargeback, refund request)'), ('type', ['null', "*

 * *                 "'string'])]), 'currency': OrderedDict([('description', 'The currency in which "*

 * *                 "the  […]*

```diff
@@ -1,124 +1,94 @@
 {
     "additionalProperties": true,
     "properties": {
-        "address1": {
+        "amount": {
+            "description": "The disputed amount in the currency specified",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "address2": {
+        "currency": {
+            "description": "The currency in which the dispute amount is represented",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "city": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "company": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "country": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "country_code": {
+        "evidence_due_by": {
+            "description": "The date by which evidence needs to be submitted for the dispute",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "country_name": {
+        "evidence_sent_on": {
+            "description": "The date when evidence was sent for the dispute",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "customer_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "default": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "first_name": {
+        "finalized_on": {
+            "description": "The date when the dispute was finalized",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "id": {
+            "description": "The unique identifier of the dispute",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "last_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "phone": {
+        "initiated_at": {
+            "description": "The date and time when the dispute was initiated",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "province": {
+        "network_reason_code": {
+            "description": "The reason code provided by the network for the dispute",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "province_code": {
+        "order_id": {
+            "description": "The identifier of the order associated with the dispute",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "shop_url": {
+        "reason": {
+            "description": "The reason provided for the dispute",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "status": {
+            "description": "The current status of the dispute",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "zip": {
+        "type": {
+            "description": "The type of dispute (e.g., chargeback, refund request)",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "type": [
-        "null",
-        "object"
-    ]
+    "type": "object"
 }
```

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.0.7/source_shopify/schemas/product_variants.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8461328976034858%*

 * *Differences: {"'properties'": "{'shop_url': {'description': 'The URL of the shop where the variant is listed'}, "*

 * *                 "'updated_at': {'description': 'The date and time when the variant was last "*

 * *                 "updated'}, 'admin_graphql_api_id': {'description': 'The unique identifier for "*

 * *                 "the variant used by the GraphQL Admin API'}, 'id': {'description': 'The unique "*

 * *                 "identifier for the variant'}, 'created_at': {'description': 'The date and time "*

 * *                 "wh […]*

```diff
@@ -1,448 +1,244 @@
 {
     "additionalProperties": true,
     "properties": {
-        "accepts_marketing": {
+        "admin_graphql_api_id": {
+            "description": "The unique identifier for the variant used by the GraphQL Admin API",
             "type": [
                 "null",
-                "boolean"
-            ]
-        },
-        "accepts_marketing_updated_at": {
-            "anyOf": [
-                {
-                    "format": "date-time",
-                    "type": "string"
-                },
-                {
-                    "type": "string"
-                },
-                {
-                    "type": "null"
-                }
+                "string"
             ]
         },
-        "addresses": {
-            "items": {
-                "properties": {
-                    "address1": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "address2": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "city": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "company": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "country": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "country_code": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "country_name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "customer_id": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    },
-                    "default": {
-                        "type": [
-                            "null",
-                            "boolean"
-                        ]
-                    },
-                    "first_name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "id": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    },
-                    "last_name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "phone": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "province": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "province_code": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "zip": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
+        "barcode": {
+            "description": "The barcode associated with the variant",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "admin_graphql_api_id": {
+        "compare_at_price": {
+            "description": "The original price of the variant before any discount",
             "type": [
                 "null",
                 "string"
             ]
         },
         "created_at": {
+            "description": "The date and time when the variant was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "currency": {
+        "fulfillment_service": {
+            "description": "The fulfillment service for the variant",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "default_address": {
-            "properties": {
-                "address1": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "address2": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "city": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "company": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "country": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "country_code": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "country_name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "customer_id": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "default": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "first_name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "id": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "last_name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "phone": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "province": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "province_code": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "zip": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "grams": {
+            "description": "The weight of the variant in grams",
             "type": [
                 "null",
-                "object"
+                "integer"
             ]
         },
-        "email": {
+        "id": {
+            "description": "The unique identifier for the variant",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "email_marketing_consent": {
-            "properties": {
-                "consent_updated_at": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "opt_in_level": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "state": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "image_id": {
+            "description": "The unique identifier for the image associated with the variant",
             "type": [
                 "null",
-                "object"
+                "integer"
             ]
         },
-        "first_name": {
+        "inventory_item_id": {
+            "description": "The unique identifier for the inventory item associated with the variant",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "id": {
+        "inventory_management": {
+            "description": "The method used to manage inventory for the variant",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "last_name": {
+        "inventory_policy": {
+            "description": "The inventory policy for the variant",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "last_order_id": {
+        "inventory_quantity": {
+            "description": "The current inventory quantity for the variant",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "last_order_name": {
+        "old_inventory_quantity": {
+            "description": "The previous inventory quantity for the variant",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "marketing_opt_in_level": {
+        "option1": {
+            "description": "The value for option 1 of the variant",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "multipass_identifier": {
+        "option2": {
+            "description": "The value for option 2 of the variant",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "note": {
+        "option3": {
+            "description": "The value for option 3 of the variant",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "orders_count": {
+        "position": {
+            "description": "The position of the variant in the product's list of variants",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "phone": {
+        "presentment_prices": {
+            "description": "The prices of the variant for presentation in different currencies",
+            "items": {
+                "properties": {
+                    "compare_at_price": {
+                        "description": "The original price of the variant in a different currency before any discount",
+                        "type": [
+                            "null",
+                            "number"
+                        ]
+                    },
+                    "price": {
+                        "description": "The price of the variant in a different currency",
+                        "properties": {
+                            "amount": {
+                                "description": "The amount of the price",
+                                "type": [
+                                    "null",
+                                    "number"
+                                ]
+                            },
+                            "currency_code": {
+                                "description": "The currency code of the price",
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "price": {
+            "description": "The price of the variant",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "shop_url": {
+        "product_id": {
+            "description": "The unique identifier for the product associated with the variant",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "sms_marketing_consent": {
-            "properties": {
-                "consent_collected_from": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "consent_updated_at": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "opt_in_level": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "state": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "requires_shipping": {
+            "description": "Indicates whether the variant requires shipping",
             "type": [
                 "null",
-                "object"
+                "boolean"
             ]
         },
-        "state": {
+        "shop_url": {
+            "description": "The URL of the shop where the variant is listed",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tags": {
+        "sku": {
+            "description": "The unique SKU (stock keeping unit) of the variant",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tax_exempt": {
+        "taxable": {
+            "description": "Indicates whether taxes are applied to the variant",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "tax_exemptions": {
+        "title": {
+            "description": "The title of the variant",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "total_spent": {
+        "updated_at": {
+            "description": "The date and time when the variant was last updated",
+            "format": "date-time",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "weight": {
+            "description": "The weight of the variant",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "verified_email": {
+        "weight_unit": {
+            "description": "The unit of measurement for the weight of the variant",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         }
     },
     "type": [
         "null",
         "object"
     ]
```

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_orders.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6899801587301587%*

 * *Differences: {"'properties'": "{'admin_graphql_api_id': {'description': 'The unique identifier for the "*

 * *                 "metafield in the Admin GraphQL API.'}, 'created_at': {'description': 'The date "*

 * *                 "and time when the metafield was created.'}, 'id': {'description': 'The unique "*

 * *                 "identifier for the metafield record.'}, 'updated_at': {'description': 'The date "*

 * *                 "and time when the metafield was last updated.'}, 'shop_url': {'description': "*

 * *                 "'The URL […]*

```diff
@@ -1,128 +1,102 @@
 {
     "additionalProperties": true,
     "properties": {
-        "active": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "address1": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "address2": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "admin_graphql_api_id": {
+            "description": "The unique identifier for the metafield in the Admin GraphQL API.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "city": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "country": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "country_code": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "country_name": {
+        "created_at": {
+            "description": "The date and time when the metafield was created.",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "created_at": {
-            "format": "date-time",
+        "description": {
+            "description": "Additional information or notes about the metafield.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "id": {
+            "description": "The unique identifier for the metafield record.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "legacy": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "localized_country_name": {
+        "key": {
+            "description": "The name that identifies the metafield.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "localized_province_name": {
+        "namespace": {
+            "description": "The area or group to which the metafield belongs.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "name": {
+        "owner_id": {
+            "description": "The unique identifier of the resource that owns the metafield.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "phone": {
+        "owner_resource": {
+            "description": "The type of resource that owns the metafield.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "province": {
+        "shop_url": {
+            "description": "The URL of the Shopify shop associated with the metafield.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "province_code": {
+        "type": {
+            "description": "The data type of the metafield value.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "shop_url": {
+        "updated_at": {
+            "description": "The date and time when the metafield was last updated.",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "value": {
+            "description": "The actual value of the metafield.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "zip": {
+        "value_type": {
+            "description": "The type of data stored in the metafield value.",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "type": "object"
+    "type": [
+        "null",
+        "object"
+    ]
 }
```

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.0.7/source_shopify/schemas/inventory_levels.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6979166666666666%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'string')], delete: [1]}, 'description': 'The "*

 * *                 "unique identifier for the inventory level.'}, 'updated_at': {'description': 'The "*

 * *                 "date and time when the inventory level was last updated.'}, "*

 * *                 "'admin_graphql_api_id': {'description': 'The unique identifier for the inventory "*

 * *                 "levels in GraphQL format.'}, 'shop_url': {'description': 'The URL of the shop "*

 * *                 "where the inventor […]*

```diff
@@ -1,89 +1,56 @@
 {
     "additionalProperties": true,
     "properties": {
         "admin_graphql_api_id": {
+            "description": "The unique identifier for the inventory levels in GraphQL format.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "created_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "description": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "id": {
+        "available": {
+            "description": "The quantity of items available for sale in the inventory.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "key": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "namespace": {
+        "id": {
+            "description": "The unique identifier for the inventory level.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "owner_id": {
+        "inventory_item_id": {
+            "description": "The unique identifier for the associated inventory item.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "owner_resource": {
+        "location_id": {
+            "description": "The unique identifier for the location related to the inventory level.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
         "shop_url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "type": {
+            "description": "The URL of the shop where the inventory belongs.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "updated_at": {
+            "description": "The date and time when the inventory level was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "value": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "value_type": {
-            "type": [
-                "null",
-                "string"
-            ]
         }
     },
-    "type": [
-        "null",
-        "object"
-    ]
+    "type": "object"
 }
```

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.0.7/source_shopify/schemas/collects.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.38058035714285715%*

 * *Differences: {"'additionalProperties'": 'True',*

 * * "'properties'": "{'id': {'type': ['null', 'integer'], 'description': 'The unique identifier for "*

 * *                 "the collect.'}, 'shop_url': {'type': ['null', 'string'], 'description': 'The URL "*

 * *                 "of the shop associated with the collect.'}, 'collection_id': "*

 * *                 "OrderedDict([('description', 'The unique identifier for the collection.'), "*

 * *                 "('type', ['null', 'integer'])]), 'created_at': OrderedDict([('description', 'The "*

 * * […]*

```diff
@@ -1,101 +1,64 @@
 {
-    "$schema": "http://json-schema.org/schema#",
+    "additionalProperties": true,
     "properties": {
-        "createdAt": {
-            "type": "string"
-        },
-        "description": {
-            "type": "string"
-        },
-        "descriptionHtml": {
-            "type": "string"
+        "collection_id": {
+            "description": "The unique identifier for the collection.",
+            "type": [
+                "null",
+                "integer"
+            ]
         },
-        "handle": {
-            "type": "string"
+        "created_at": {
+            "description": "The date and time when the collect was created.",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
         },
         "id": {
-            "type": "string"
-        },
-        "isGiftCard": {
-            "type": "boolean"
-        },
-        "legacyResourceId": {
-            "type": "string"
+            "description": "The unique identifier for the collect.",
+            "type": [
+                "null",
+                "integer"
+            ]
         },
-        "mediaCount": {
-            "type": "integer"
+        "position": {
+            "description": "The position of the product in the collection.",
+            "type": [
+                "null",
+                "integer"
+            ]
         },
-        "onlineStorePreviewUrl": {
-            "type": "string"
+        "product_id": {
+            "description": "The unique identifier of the product.",
+            "type": [
+                "null",
+                "integer"
+            ]
         },
-        "onlineStoreUrl": {
+        "shop_url": {
+            "description": "The URL of the shop associated with the collect.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "options": {
-            "items": {
-                "properties": {
-                    "id": {
-                        "type": "string"
-                    },
-                    "name": {
-                        "type": "string"
-                    },
-                    "position": {
-                        "type": "integer"
-                    },
-                    "values": {
-                        "items": {
-                            "type": "string"
-                        },
-                        "type": "array"
-                    }
-                },
-                "type": "object"
-            },
-            "type": "array"
-        },
-        "productType": {
-            "type": "string"
-        },
-        "publishedAt": {
+        "sort_value": {
+            "description": "The value used to sort the products in the collection.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "shop_url": {
-            "type": "string"
-        },
-        "status": {
-            "type": "string"
-        },
-        "tags": {
-            "items": {
-                "type": "string"
-            },
-            "type": "array"
-        },
-        "title": {
-            "type": "string"
-        },
-        "totalInventory": {
-            "type": "integer"
-        },
-        "totalVariants": {
-            "type": "integer"
-        },
-        "tracksInventory": {
-            "type": "boolean"
-        },
-        "updatedAt": {
-            "type": "string"
-        },
-        "vendor": {
-            "type": "string"
+        "updated_at": {
+            "description": "The date and time when the collect was last updated.",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/scopes.py` & `airbyte_source_shopify-2.0.7/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/job.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/query.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/record.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/source.py` & `airbyte_source_shopify-2.0.7/source_shopify/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/spec.json` & `airbyte_source_shopify-2.0.7/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.0.7/source_shopify/streams/base_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.0.7/source_shopify/streams/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/transform.py` & `airbyte_source_shopify-2.0.7/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/source_shopify/utils.py` & `airbyte_source_shopify-2.0.7/source_shopify/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.6/PKG-INFO` & `airbyte_source_shopify-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.0.6
+Version: 2.0.7
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.81.4)
 Requires-Dist: graphql-query (>=1.1.1,<2.0.0)
 Requires-Dist: sgqlc (==16.3)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/shopify
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Shopify source connector
```

