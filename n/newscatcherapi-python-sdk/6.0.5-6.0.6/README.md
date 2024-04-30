# Comparing `tmp/newscatcherapi_python_sdk-6.0.5.tar.gz` & `tmp/newscatcherapi_python_sdk-6.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newscatcherapi_python_sdk-6.0.5.tar", max compression
+gzip compressed data, was "newscatcherapi_python_sdk-6.0.6.tar", max compression
```

## Comparing `newscatcherapi_python_sdk-6.0.5.tar` & `newscatcherapi_python_sdk-6.0.6.tar`

### file list

```diff
@@ -1,259 +1,239 @@
--rw-r--r--   0        0        0     1081 2024-04-25 19:58:24.285935 newscatcherapi_python_sdk-6.0.5/LICENSE
--rw-r--r--   0        0        0    77971 2024-04-25 20:02:27.020398 newscatcherapi_python_sdk-6.0.5/README.md
--rw-r--r--   0        0        0     1059 2024-04-25 20:02:27.020547 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/__init__.py
--rw-r--r--   0        0        0    77304 2024-04-25 20:02:27.020779 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/api_client.py
--rw-r--r--   0        0        0      663 2024-04-25 19:58:24.246592 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/api_response.py
--rw-r--r--   0        0        0      214 2024-04-25 19:58:24.246713 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/__init__.py
--rw-r--r--   0        0        0     1726 2024-04-25 20:02:27.020942 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/path_to_api.py
--rw-r--r--   0        0        0      248 2024-04-25 19:58:24.246991 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      197 2024-04-25 19:58:24.247093 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_authors.py
--rw-r--r--   0        0        0      223 2024-04-25 19:58:24.247196 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_latest_headlines.py
--rw-r--r--   0        0        0      194 2024-04-25 19:58:24.247290 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_search.py
--rw-r--r--   0        0        0      216 2024-04-25 19:58:24.247381 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_search_by_link.py
--rw-r--r--   0        0        0      268 2024-04-25 20:02:27.021036 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_search_duplicates_by_original_id.py
--rw-r--r--   0        0        0      217 2024-04-25 19:58:24.247682 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_search_similar.py
--rw-r--r--   0        0        0      197 2024-04-25 19:58:24.247771 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_sources.py
--rw-r--r--   0        0        0      212 2024-04-25 19:58:24.247858 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_subscription.py
--rw-r--r--   0        0        0     1622 2024-04-25 20:02:27.021176 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      581 2024-04-25 20:02:27.021334 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/__init__.py
--rw-r--r--   0        0        0      902 2024-04-25 19:58:24.248147 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/authors_api.py
--rw-r--r--   0        0        0      705 2024-04-25 19:58:24.248252 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/authors_api_raw.py
--rw-r--r--   0        0        0      961 2024-04-25 19:58:24.248403 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/latest_headlines_api.py
--rw-r--r--   0        0        0      731 2024-04-25 19:58:24.248544 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py
--rw-r--r--   0        0        0      895 2024-04-25 19:58:24.248659 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_api.py
--rw-r--r--   0        0        0      702 2024-04-25 19:58:24.248773 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_api_raw.py
--rw-r--r--   0        0        0     1061 2024-04-25 20:02:27.021453 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_duplicates_by_original_id_api.py
--rw-r--r--   0        0        0      776 2024-04-25 20:02:27.021592 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_duplicates_by_original_id_api_raw.py
--rw-r--r--   0        0        0      932 2024-04-25 19:58:24.249098 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_link_api.py
--rw-r--r--   0        0        0      722 2024-04-25 19:58:24.249203 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_link_api_raw.py
--rw-r--r--   0        0        0      947 2024-04-25 19:58:24.249303 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_similar_api.py
--rw-r--r--   0        0        0      725 2024-04-25 19:58:24.249436 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_similar_api_raw.py
--rw-r--r--   0        0        0      902 2024-04-25 19:58:24.249554 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/sources_api.py
--rw-r--r--   0        0        0      705 2024-04-25 19:58:24.249662 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/sources_api_raw.py
--rw-r--r--   0        0        0      937 2024-04-25 19:58:24.249876 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/subscription_api.py
--rw-r--r--   0        0        0      720 2024-04-25 19:58:24.249975 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/subscription_api_raw.py
--rw-r--r--   0        0        0     2352 2024-04-25 20:02:27.021756 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client.py
--rw-r--r--   0        0        0     2352 2024-04-25 20:02:27.021919 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client.pyi
--rw-r--r--   0        0        0      950 2024-04-25 19:58:24.250278 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client_custom.py
--rw-r--r--   0        0        0    18272 2024-04-25 20:02:27.022098 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/configuration.py
--rw-r--r--   0        0        0     7953 2024-04-25 19:58:24.250519 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/exceptions.py
--rw-r--r--   0        0        0     2274 2024-04-25 19:58:24.250625 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/exceptions_base.py
--rw-r--r--   0        0        0      355 2024-04-25 19:58:24.250761 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/__init__.py
--rw-r--r--   0        0        0     3784 2024-04-25 19:58:24.250862 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/additional_source_info.py
--rw-r--r--   0        0        0     3784 2024-04-25 19:58:24.250958 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/additional_source_info.pyi
--rw-r--r--   0        0        0    31500 2024-04-25 19:58:24.251067 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/author_search_request.py
--rw-r--r--   0        0        0    31184 2024-04-25 19:58:24.251196 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/author_search_request.pyi
--rw-r--r--   0        0        0     2575 2024-04-25 19:58:24.251304 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_get_response.py
--rw-r--r--   0        0        0     2575 2024-04-25 19:58:24.251406 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_get_response.pyi
--rw-r--r--   0        0        0     2577 2024-04-25 19:58:24.251515 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_post_response.py
--rw-r--r--   0        0        0     2577 2024-04-25 19:58:24.251616 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_post_response.pyi
--rw-r--r--   0        0        0     3926 2024-04-25 19:58:24.251719 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster.py
--rw-r--r--   0        0        0     3926 2024-04-25 19:58:24.251816 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster.pyi
--rw-r--r--   0        0        0     1483 2024-04-25 19:58:24.251924 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster_articles.py
--rw-r--r--   0        0        0     1483 2024-04-25 19:58:24.252144 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster_articles.pyi
--rw-r--r--   0        0        0     7607 2024-04-25 19:58:24.252273 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/clustering_search_response.py
--rw-r--r--   0        0        0     7607 2024-04-25 19:58:24.252422 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/clustering_search_response.pyi
--rw-r--r--   0        0        0    31387 2024-04-25 19:58:24.252555 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0    31387 2024-04-25 19:58:24.252697 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi
--rw-r--r--   0        0        0     7229 2024-04-25 19:58:24.252840 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     7229 2024-04-25 19:58:24.252968 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi
--rw-r--r--   0        0        0     6499 2024-04-25 19:58:24.253093 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0     6499 2024-04-25 19:58:24.253221 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi
--rw-r--r--   0        0        0     1561 2024-04-25 19:58:24.253332 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1561 2024-04-25 19:58:24.253442 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi
--rw-r--r--   0        0        0    33012 2024-04-25 19:58:24.253562 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0    33012 2024-04-25 19:58:24.253717 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi
--rw-r--r--   0        0        0     7228 2024-04-25 19:58:24.253853 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     7228 2024-04-25 19:58:24.253974 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi
--rw-r--r--   0        0        0     6499 2024-04-25 19:58:24.254093 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0     6499 2024-04-25 19:58:24.254215 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi
--rw-r--r--   0        0        0     1561 2024-04-25 19:58:24.254329 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1561 2024-04-25 19:58:24.254443 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi
--rw-r--r--   0        0        0     6437 2024-04-25 19:58:24.254566 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0     6437 2024-04-25 19:58:24.254682 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi
--rw-r--r--   0        0        0     1549 2024-04-25 19:58:24.254799 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1549 2024-04-25 19:58:24.254904 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi
--rw-r--r--   0        0        0     4257 2024-04-25 20:02:27.022250 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/duplicates_by_original_id_request.py
--rw-r--r--   0        0        0     4099 2024-04-25 20:02:27.022444 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/duplicates_by_original_id_request.pyi
--rw-r--r--   0        0        0     3525 2024-04-25 19:58:24.255225 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/http_validation_error.py
--rw-r--r--   0        0        0     3525 2024-04-25 19:58:24.255311 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/http_validation_error.pyi
--rw-r--r--   0        0        0     2429 2024-04-25 19:58:24.255401 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_get_response.py
--rw-r--r--   0        0        0     2429 2024-04-25 19:58:24.255492 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_get_response.pyi
--rw-r--r--   0        0        0     2431 2024-04-25 19:58:24.255581 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_post_response.py
--rw-r--r--   0        0        0     2431 2024-04-25 19:58:24.256025 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_post_response.pyi
--rw-r--r--   0        0        0    28271 2024-04-25 19:58:24.256168 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_request.py
--rw-r--r--   0        0        0    27955 2024-04-25 19:58:24.256293 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_request.pyi
--rw-r--r--   0        0        0     6273 2024-04-25 19:58:24.256415 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response.py
--rw-r--r--   0        0        0     6273 2024-04-25 19:58:24.256526 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response.pyi
--rw-r--r--   0        0        0     1515 2024-04-25 19:58:24.256621 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     1515 2024-04-25 19:58:24.256719 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response_articles.pyi
--rw-r--r--   0        0        0    32258 2024-04-25 19:58:24.256821 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/more_like_this_request.py
--rw-r--r--   0        0        0    31863 2024-04-25 19:58:24.256942 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/more_like_this_request.pyi
--rw-r--r--   0        0        0     2465 2024-04-25 19:58:24.257043 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_get_response.py
--rw-r--r--   0        0        0     2465 2024-04-25 19:58:24.257130 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_get_response.pyi
--rw-r--r--   0        0        0     2467 2024-04-25 19:58:24.257215 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_post_response.py
--rw-r--r--   0        0        0     2467 2024-04-25 19:58:24.257305 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_post_response.pyi
--rw-r--r--   0        0        0    37420 2024-04-25 20:02:27.022823 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_request.py
--rw-r--r--   0        0        0    37104 2024-04-25 20:02:27.022977 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_request.pyi
--rw-r--r--   0        0        0     2589 2024-04-25 19:58:24.257625 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_get_response.py
--rw-r--r--   0        0        0     2589 2024-04-25 19:58:24.257712 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_get_response.pyi
--rw-r--r--   0        0        0     2591 2024-04-25 19:58:24.257799 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_post_response.py
--rw-r--r--   0        0        0     2591 2024-04-25 19:58:24.257889 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_post_response.pyi
--rw-r--r--   0        0        0     4717 2024-04-25 19:58:24.257991 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_url_request.py
--rw-r--r--   0        0        0     4559 2024-04-25 19:58:24.258092 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_url_request.pyi
--rw-r--r--   0        0        0     2509 2024-04-25 20:02:27.023102 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_get_response.py
--rw-r--r--   0        0        0     2509 2024-04-25 20:02:27.023180 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_get_response.pyi
--rw-r--r--   0        0        0     2511 2024-04-25 20:02:27.023247 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_post_response.py
--rw-r--r--   0        0        0     2511 2024-04-25 20:02:27.023311 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_post_response.pyi
--rw-r--r--   0        0        0     4044 2024-04-25 19:58:24.258708 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/similar_document.py
--rw-r--r--   0        0        0     4044 2024-04-25 19:58:24.258802 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/similar_document.pyi
--rw-r--r--   0        0        0     4488 2024-04-25 19:58:24.258904 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_info.py
--rw-r--r--   0        0        0     4488 2024-04-25 19:58:24.259005 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_info.pyi
--rw-r--r--   0        0        0     3912 2024-04-25 19:58:24.259100 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response.py
--rw-r--r--   0        0        0     3912 2024-04-25 19:58:24.259191 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response.pyi
--rw-r--r--   0        0        0     3437 2024-04-25 19:58:24.259279 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response_sources.py
--rw-r--r--   0        0        0     3437 2024-04-25 19:58:24.259365 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response_sources.pyi
--rw-r--r--   0        0        0     6854 2024-04-25 19:58:24.259461 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/sources_request.py
--rw-r--r--   0        0        0     6854 2024-04-25 19:58:24.259556 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/sources_request.pyi
--rw-r--r--   0        0        0     5919 2024-04-25 19:58:24.259659 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/subscription_response.py
--rw-r--r--   0        0        0     5919 2024-04-25 19:58:24.259756 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/subscription_response.pyi
--rw-r--r--   0        0        0     3626 2024-04-25 19:58:24.259953 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error.py
--rw-r--r--   0        0        0     3626 2024-04-25 19:58:24.260036 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error.pyi
--rw-r--r--   0        0        0     3408 2024-04-25 19:58:24.260121 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error_loc.py
--rw-r--r--   0        0        0     3408 2024-04-25 19:58:24.260208 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error_loc.pyi
--rw-r--r--   0        0        0     4487 2024-04-25 20:02:27.023430 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/models/__init__.py
--rw-r--r--   0        0        0    25772 2024-04-25 20:02:27.023562 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/operation_parameter_map.py
--rw-r--r--   0        0        0      665 2024-04-25 20:02:27.024802 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/__init__.py
--rw-r--r--   0        0        0      323 2024-04-25 19:58:24.260619 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/__init__.py
--rw-r--r--   0        0        0    66916 2024-04-25 19:58:24.260746 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/get.py
--rw-r--r--   0        0        0    66607 2024-04-25 19:58:24.260889 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/get.pyi
--rw-r--r--   0        0        0    47473 2024-04-25 19:58:24.261010 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/post.py
--rw-r--r--   0        0        0    47336 2024-04-25 19:58:24.261131 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/post.pyi
--rw-r--r--   0        0        0      341 2024-04-25 19:58:24.261232 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/__init__.py
--rw-r--r--   0        0        0    66032 2024-04-25 19:58:24.261357 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/get.py
--rw-r--r--   0        0        0    65723 2024-04-25 19:58:24.261497 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/get.pyi
--rw-r--r--   0        0        0    49192 2024-04-25 19:58:24.262028 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/post.py
--rw-r--r--   0        0        0    49055 2024-04-25 19:58:24.262159 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/post.pyi
--rw-r--r--   0        0        0      321 2024-04-25 19:58:24.262271 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/__init__.py
--rw-r--r--   0        0        0    78572 2024-04-25 20:02:27.029088 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/get.py
--rw-r--r--   0        0        0    78263 2024-04-25 20:02:27.029366 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/get.pyi
--rw-r--r--   0        0        0    55220 2024-04-25 20:02:27.031116 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/post.py
--rw-r--r--   0        0        0    55083 2024-04-25 20:02:27.031311 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/post.pyi
--rw-r--r--   0        0        0      337 2024-04-25 19:58:24.262979 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/__init__.py
--rw-r--r--   0        0        0    19293 2024-04-25 19:58:24.263086 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/get.py
--rw-r--r--   0        0        0    19070 2024-04-25 19:58:24.263219 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/get.pyi
--rw-r--r--   0        0        0    17699 2024-04-25 19:58:24.263337 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/post.py
--rw-r--r--   0        0        0    17562 2024-04-25 19:58:24.263462 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/post.pyi
--rw-r--r--   0        0        0      373 2024-04-25 20:02:27.031417 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/__init__.py
--rw-r--r--   0        0        0    17623 2024-04-25 20:02:27.031489 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/get.py
--rw-r--r--   0        0        0    17400 2024-04-25 20:02:27.031596 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/get.pyi
--rw-r--r--   0        0        0    16697 2024-04-25 20:02:27.031674 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/post.py
--rw-r--r--   0        0        0    16560 2024-04-25 20:02:27.031764 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/post.pyi
--rw-r--r--   0        0        0      337 2024-04-25 19:58:24.264150 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/__init__.py
--rw-r--r--   0        0        0    67713 2024-04-25 19:58:24.264298 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/get.py
--rw-r--r--   0        0        0    67361 2024-04-25 19:58:24.264452 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/get.pyi
--rw-r--r--   0        0        0    47930 2024-04-25 19:58:24.264584 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/post.py
--rw-r--r--   0        0        0    47793 2024-04-25 19:58:24.264718 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/post.pyi
--rw-r--r--   0        0        0      323 2024-04-25 19:58:24.265433 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/__init__.py
--rw-r--r--   0        0        0    22889 2024-04-25 19:58:24.265541 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/get.py
--rw-r--r--   0        0        0    22752 2024-04-25 19:58:24.265659 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/get.pyi
--rw-r--r--   0        0        0    19936 2024-04-25 19:58:24.266109 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/post.py
--rw-r--r--   0        0        0    19799 2024-04-25 19:58:24.266226 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/post.pyi
--rw-r--r--   0        0        0      333 2024-04-25 19:58:24.266443 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/__init__.py
--rw-r--r--   0        0        0    12067 2024-04-25 19:58:24.266541 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/get.py
--rw-r--r--   0        0        0    11930 2024-04-25 19:58:24.266713 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/get.pyi
--rw-r--r--   0        0        0    12093 2024-04-25 19:58:24.266880 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/post.py
--rw-r--r--   0        0        0    11956 2024-04-25 19:58:24.267049 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/post.pyi
--rw-r--r--   0        0        0        0 2024-04-25 19:58:24.267202 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/__init__.py
--rw-r--r--   0        0        0      987 2024-04-25 19:58:24.267295 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/additional_source_info.py
--rw-r--r--   0        0        0     4726 2024-04-25 19:58:24.267392 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/author_search_request.py
--rw-r--r--   0        0        0     1061 2024-04-25 19:58:24.267483 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/authors_get_response.py
--rw-r--r--   0        0        0     1062 2024-04-25 19:58:24.267572 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/authors_post_response.py
--rw-r--r--   0        0        0      995 2024-04-25 19:58:24.267665 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/cluster.py
--rw-r--r--   0        0        0      665 2024-04-25 19:58:24.267758 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/cluster_articles.py
--rw-r--r--   0        0        0     1336 2024-04-25 19:58:24.267855 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/clustering_search_response.py
--rw-r--r--   0        0        0     3052 2024-04-25 19:58:24.267949 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0     1542 2024-04-25 19:58:24.268045 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     1436 2024-04-25 19:58:24.268136 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0      704 2024-04-25 19:58:24.268234 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     3239 2024-04-25 19:58:24.268436 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0     1543 2024-04-25 19:58:24.268716 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     1437 2024-04-25 19:58:24.269513 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0      704 2024-04-25 19:58:24.269778 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1411 2024-04-25 19:58:24.270012 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0      698 2024-04-25 19:58:24.270224 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0      979 2024-04-25 20:02:27.031870 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/duplicates_by_original_id_request.py
--rw-r--r--   0        0        0      937 2024-04-25 19:58:24.270419 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/http_validation_error.py
--rw-r--r--   0        0        0      907 2024-04-25 19:58:24.270513 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_get_response.py
--rw-r--r--   0        0        0      908 2024-04-25 19:58:24.270720 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_post_response.py
--rw-r--r--   0        0        0     4897 2024-04-25 19:58:24.270824 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_request.py
--rw-r--r--   0        0        0     1340 2024-04-25 19:58:24.271021 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_response.py
--rw-r--r--   0        0        0      681 2024-04-25 19:58:24.271117 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     4721 2024-04-25 19:58:24.271214 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/more_like_this_request.py
--rw-r--r--   0        0        0      952 2024-04-25 19:58:24.271301 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_get_response.py
--rw-r--r--   0        0        0      953 2024-04-25 19:58:24.271491 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_post_response.py
--rw-r--r--   0        0        0     5628 2024-04-25 20:02:27.032002 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_request.py
--rw-r--r--   0        0        0     1069 2024-04-25 19:58:24.271790 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_similar_get_response.py
--rw-r--r--   0        0        0     1070 2024-04-25 19:58:24.271903 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_similar_post_response.py
--rw-r--r--   0        0        0     1151 2024-04-25 19:58:24.272107 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_url_request.py
--rw-r--r--   0        0        0      974 2024-04-25 20:02:27.032073 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_get_response.py
--rw-r--r--   0        0        0      975 2024-04-25 20:02:27.032146 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_post_response.py
--rw-r--r--   0        0        0      937 2024-04-25 19:58:24.272469 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/similar_document.py
--rw-r--r--   0        0        0     1132 2024-04-25 19:58:24.272670 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_info.py
--rw-r--r--   0        0        0     1093 2024-04-25 19:58:24.272858 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_response.py
--rw-r--r--   0        0        0      760 2024-04-25 19:58:24.273047 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_response_sources.py
--rw-r--r--   0        0        0     1432 2024-04-25 19:58:24.273131 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/sources_request.py
--rw-r--r--   0        0        0     1216 2024-04-25 19:58:24.273320 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/subscription_response.py
--rw-r--r--   0        0        0      973 2024-04-25 19:58:24.273403 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/validation_error.py
--rw-r--r--   0        0        0      684 2024-04-25 19:58:24.273600 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/validation_error_loc.py
--rw-r--r--   0        0        0      913 2024-04-25 19:58:24.273689 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_after_hook.py
--rw-r--r--   0        0        0      971 2024-04-25 19:58:24.273776 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_before_hook.py
--rw-r--r--   0        0        0      936 2024-04-25 19:58:24.273966 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_before_url_hook.py
--rw-r--r--   0        0        0    11233 2024-04-25 19:58:24.274049 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/rest.py
--rw-r--r--   0        0        0    96391 2024-04-25 19:58:24.274266 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/schemas.py
--rw-r--r--   0        0        0        0 2024-04-25 19:58:24.274364 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/__init__.py
--rw-r--r--   0        0        0      842 2024-04-25 19:58:24.274454 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/additional_source_info.py
--rw-r--r--   0        0        0     2699 2024-04-25 19:58:24.274543 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/author_search_request.py
--rw-r--r--   0        0        0      992 2024-04-25 19:58:24.274627 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/authors_get_response.py
--rw-r--r--   0        0        0      993 2024-04-25 19:58:24.274715 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/authors_post_response.py
--rw-r--r--   0        0        0      862 2024-04-25 19:58:24.274797 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/cluster.py
--rw-r--r--   0        0        0      604 2024-04-25 19:58:24.274878 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/cluster_articles.py
--rw-r--r--   0        0        0     1106 2024-04-25 19:58:24.274961 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/clustering_search_response.py
--rw-r--r--   0        0        0     1778 2024-04-25 19:58:24.275053 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0     1341 2024-04-25 19:58:24.275143 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     1326 2024-04-25 19:58:24.275230 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0      643 2024-04-25 19:58:24.275320 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1903 2024-04-25 19:58:24.275568 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0     1342 2024-04-25 19:58:24.275659 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     1327 2024-04-25 19:58:24.275745 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0      643 2024-04-25 19:58:24.275835 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1277 2024-04-25 19:58:24.275922 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0      637 2024-04-25 19:58:24.276011 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0      880 2024-04-25 20:02:27.032216 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/duplicates_by_original_id_request.py
--rw-r--r--   0        0        0      889 2024-04-25 19:58:24.276181 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/http_validation_error.py
--rw-r--r--   0        0        0      838 2024-04-25 19:58:24.276265 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_get_response.py
--rw-r--r--   0        0        0      839 2024-04-25 19:58:24.276350 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_post_response.py
--rw-r--r--   0        0        0     2812 2024-04-25 19:58:24.276431 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_request.py
--rw-r--r--   0        0        0     1138 2024-04-25 19:58:24.276517 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_response.py
--rw-r--r--   0        0        0      620 2024-04-25 19:58:24.276603 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     2616 2024-04-25 19:58:24.276691 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/more_like_this_request.py
--rw-r--r--   0        0        0      883 2024-04-25 19:58:24.276776 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_get_response.py
--rw-r--r--   0        0        0      884 2024-04-25 19:58:24.276970 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_post_response.py
--rw-r--r--   0        0        0     3061 2024-04-25 20:02:27.032343 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_request.py
--rw-r--r--   0        0        0     1000 2024-04-25 19:58:24.277144 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_similar_get_response.py
--rw-r--r--   0        0        0     1001 2024-04-25 19:58:24.277224 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_similar_post_response.py
--rw-r--r--   0        0        0      957 2024-04-25 19:58:24.277306 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_url_request.py
--rw-r--r--   0        0        0      905 2024-04-25 20:02:27.032427 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/searchduplicatesbyoriginalid_get_response.py
--rw-r--r--   0        0        0      906 2024-04-25 20:02:27.032497 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/searchduplicatesbyoriginalid_post_response.py
--rw-r--r--   0        0        0      836 2024-04-25 19:58:24.277563 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/similar_document.py
--rw-r--r--   0        0        0      904 2024-04-25 19:58:24.277644 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_info.py
--rw-r--r--   0        0        0      994 2024-04-25 19:58:24.277730 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_response.py
--rw-r--r--   0        0        0      695 2024-04-25 19:58:24.277816 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_response_sources.py
--rw-r--r--   0        0        0      996 2024-04-25 19:58:24.277897 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/sources_request.py
--rw-r--r--   0        0        0      925 2024-04-25 19:58:24.277987 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/subscription_response.py
--rw-r--r--   0        0        0      892 2024-04-25 19:58:24.278071 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/validation_error.py
--rw-r--r--   0        0        0      623 2024-04-25 19:58:24.278162 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/validation_error_loc.py
--rw-r--r--   0        0        0      758 2024-04-25 19:58:24.278243 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type_util.py
--rw-r--r--   0        0        0     3177 2024-04-25 19:58:24.278323 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/validation_metadata.py
--rw-r--r--   0        0        0      791 2024-04-25 20:02:27.032728 newscatcherapi_python_sdk-6.0.5/pyproject.toml
--rw-r--r--   0        0        0    78988 1970-01-01 00:00:00.000000 newscatcherapi_python_sdk-6.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-30 18:56:21.581311 newscatcherapi_python_sdk-6.0.6/LICENSE
+-rw-r--r--   0        0        0    75708 2024-04-30 18:57:54.508766 newscatcherapi_python_sdk-6.0.6/README.md
+-rw-r--r--   0        0        0     1059 2024-04-30 18:57:54.509130 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/__init__.py
+-rw-r--r--   0        0        0    77304 2024-04-30 18:57:54.510352 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/api_client.py
+-rw-r--r--   0        0        0      663 2024-04-30 18:56:21.552108 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/api_response.py
+-rw-r--r--   0        0        0      214 2024-04-30 18:56:21.552209 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/__init__.py
+-rw-r--r--   0        0        0     1432 2024-04-30 18:57:54.510529 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      248 2024-04-30 18:56:21.552403 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-30 18:56:21.552494 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/paths/api_authors.py
+-rw-r--r--   0        0        0      223 2024-04-30 18:56:21.552586 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/paths/api_latest_headlines.py
+-rw-r--r--   0        0        0      194 2024-04-30 18:56:21.552679 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/paths/api_search.py
+-rw-r--r--   0        0        0      216 2024-04-30 18:56:21.552771 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/paths/api_search_by_link.py
+-rw-r--r--   0        0        0      217 2024-04-30 18:56:21.552857 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/paths/api_search_similar.py
+-rw-r--r--   0        0        0      197 2024-04-30 18:56:21.552983 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/paths/api_sources.py
+-rw-r--r--   0        0        0      212 2024-04-30 18:56:21.553123 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/paths/api_subscription.py
+-rw-r--r--   0        0        0     1339 2024-04-30 18:57:54.510640 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      507 2024-04-30 18:57:54.510764 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0      902 2024-04-30 18:56:21.553423 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/authors_api.py
+-rw-r--r--   0        0        0      705 2024-04-30 18:56:21.553521 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/authors_api_raw.py
+-rw-r--r--   0        0        0      961 2024-04-30 18:56:21.553609 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/latest_headlines_api.py
+-rw-r--r--   0        0        0      731 2024-04-30 18:56:21.553693 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py
+-rw-r--r--   0        0        0      895 2024-04-30 18:56:21.553778 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_api.py
+-rw-r--r--   0        0        0      702 2024-04-30 18:56:21.553862 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_api_raw.py
+-rw-r--r--   0        0        0      932 2024-04-30 18:56:21.553950 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_link_api.py
+-rw-r--r--   0        0        0      722 2024-04-30 18:56:21.554037 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_link_api_raw.py
+-rw-r--r--   0        0        0      947 2024-04-30 18:56:21.554126 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_similar_api.py
+-rw-r--r--   0        0        0      725 2024-04-30 18:56:21.554226 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_similar_api_raw.py
+-rw-r--r--   0        0        0      902 2024-04-30 18:56:21.554319 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/sources_api.py
+-rw-r--r--   0        0        0      705 2024-04-30 18:56:21.554429 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/sources_api_raw.py
+-rw-r--r--   0        0        0      937 2024-04-30 18:56:21.554534 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/subscription_api.py
+-rw-r--r--   0        0        0      720 2024-04-30 18:56:21.554634 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/subscription_api_raw.py
+-rw-r--r--   0        0        0     2114 2024-04-30 18:57:54.510883 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/client.py
+-rw-r--r--   0        0        0     2114 2024-04-30 18:57:54.511025 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/client.pyi
+-rw-r--r--   0        0        0      950 2024-04-30 18:56:21.554917 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/client_custom.py
+-rw-r--r--   0        0        0    18272 2024-04-30 18:57:54.511466 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/configuration.py
+-rw-r--r--   0        0        0     7953 2024-04-30 18:56:21.555199 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/exceptions.py
+-rw-r--r--   0        0        0     2274 2024-04-30 18:56:21.555284 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/exceptions_base.py
+-rw-r--r--   0        0        0      355 2024-04-30 18:56:21.555399 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/__init__.py
+-rw-r--r--   0        0        0     3784 2024-04-30 18:56:21.555488 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/additional_source_info.py
+-rw-r--r--   0        0        0     3784 2024-04-30 18:56:21.555624 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/additional_source_info.pyi
+-rw-r--r--   0        0        0    31500 2024-04-30 18:56:21.555723 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/author_search_request.py
+-rw-r--r--   0        0        0    31184 2024-04-30 18:56:21.555891 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/author_search_request.pyi
+-rw-r--r--   0        0        0     2575 2024-04-30 18:56:21.556006 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/authors_get_response.py
+-rw-r--r--   0        0        0     2575 2024-04-30 18:56:21.556108 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/authors_get_response.pyi
+-rw-r--r--   0        0        0     2577 2024-04-30 18:56:21.556199 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/authors_post_response.py
+-rw-r--r--   0        0        0     2577 2024-04-30 18:56:21.556288 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/authors_post_response.pyi
+-rw-r--r--   0        0        0     3926 2024-04-30 18:56:21.556374 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/cluster.py
+-rw-r--r--   0        0        0     3926 2024-04-30 18:56:21.556460 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/cluster.pyi
+-rw-r--r--   0        0        0     1483 2024-04-30 18:56:21.556545 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/cluster_articles.py
+-rw-r--r--   0        0        0     1483 2024-04-30 18:56:21.556629 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/cluster_articles.pyi
+-rw-r--r--   0        0        0     7607 2024-04-30 18:56:21.556745 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/clustering_search_response.py
+-rw-r--r--   0        0        0     7607 2024-04-30 18:56:21.556852 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/clustering_search_response.pyi
+-rw-r--r--   0        0        0    31387 2024-04-30 18:56:21.556960 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0    31387 2024-04-30 18:56:21.557073 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi
+-rw-r--r--   0        0        0     7229 2024-04-30 18:56:21.557200 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     7229 2024-04-30 18:56:21.557313 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi
+-rw-r--r--   0        0        0     6499 2024-04-30 18:56:21.557429 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0     6499 2024-04-30 18:56:21.557539 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi
+-rw-r--r--   0        0        0     1561 2024-04-30 18:56:21.557638 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1561 2024-04-30 18:56:21.557734 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi
+-rw-r--r--   0        0        0    33012 2024-04-30 18:56:21.557843 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0    33012 2024-04-30 18:56:21.557960 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi
+-rw-r--r--   0        0        0     7228 2024-04-30 18:56:21.558087 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     7228 2024-04-30 18:56:21.558198 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi
+-rw-r--r--   0        0        0     6499 2024-04-30 18:56:21.558301 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0     6499 2024-04-30 18:56:21.558408 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi
+-rw-r--r--   0        0        0     1561 2024-04-30 18:56:21.558504 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1561 2024-04-30 18:56:21.558603 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi
+-rw-r--r--   0        0        0     6437 2024-04-30 18:56:21.558722 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0     6437 2024-04-30 18:56:21.558831 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi
+-rw-r--r--   0        0        0     1549 2024-04-30 18:56:21.558932 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1549 2024-04-30 18:56:21.559022 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi
+-rw-r--r--   0        0        0     3525 2024-04-30 18:56:21.559103 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/http_validation_error.py
+-rw-r--r--   0        0        0     3525 2024-04-30 18:56:21.559185 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     2429 2024-04-30 18:56:21.559276 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_get_response.py
+-rw-r--r--   0        0        0     2429 2024-04-30 18:56:21.559363 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_get_response.pyi
+-rw-r--r--   0        0        0     2431 2024-04-30 18:56:21.559445 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     2431 2024-04-30 18:56:21.559529 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_post_response.pyi
+-rw-r--r--   0        0        0    28271 2024-04-30 18:56:21.559633 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_request.py
+-rw-r--r--   0        0        0    27955 2024-04-30 18:56:21.559798 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_request.pyi
+-rw-r--r--   0        0        0     6273 2024-04-30 18:56:21.559919 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_response.py
+-rw-r--r--   0        0        0     6273 2024-04-30 18:56:21.560024 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_response.pyi
+-rw-r--r--   0        0        0     1515 2024-04-30 18:56:21.560112 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     1515 2024-04-30 18:56:21.560200 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_response_articles.pyi
+-rw-r--r--   0        0        0    32258 2024-04-30 18:56:21.560295 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/more_like_this_request.py
+-rw-r--r--   0        0        0    31863 2024-04-30 18:56:21.560399 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/more_like_this_request.pyi
+-rw-r--r--   0        0        0     2465 2024-04-30 18:56:21.560498 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_get_response.py
+-rw-r--r--   0        0        0     2465 2024-04-30 18:56:21.560581 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_get_response.pyi
+-rw-r--r--   0        0        0     2467 2024-04-30 18:56:21.560660 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_post_response.py
+-rw-r--r--   0        0        0     2467 2024-04-30 18:56:21.560742 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_post_response.pyi
+-rw-r--r--   0        0        0    37420 2024-04-30 18:56:21.560849 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_request.py
+-rw-r--r--   0        0        0    37104 2024-04-30 18:56:21.560973 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_request.pyi
+-rw-r--r--   0        0        0     2589 2024-04-30 18:56:21.561082 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_similar_get_response.py
+-rw-r--r--   0        0        0     2589 2024-04-30 18:56:21.561171 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_similar_get_response.pyi
+-rw-r--r--   0        0        0     2591 2024-04-30 18:56:21.561256 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_similar_post_response.py
+-rw-r--r--   0        0        0     2591 2024-04-30 18:56:21.561342 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_similar_post_response.pyi
+-rw-r--r--   0        0        0     4717 2024-04-30 18:56:21.561448 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_url_request.py
+-rw-r--r--   0        0        0     4559 2024-04-30 18:56:21.561549 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_url_request.pyi
+-rw-r--r--   0        0        0     4044 2024-04-30 18:56:21.561637 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/similar_document.py
+-rw-r--r--   0        0        0     4044 2024-04-30 18:56:21.561718 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/similar_document.pyi
+-rw-r--r--   0        0        0     4488 2024-04-30 18:56:21.561821 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_info.py
+-rw-r--r--   0        0        0     4488 2024-04-30 18:56:21.561922 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_info.pyi
+-rw-r--r--   0        0        0     3912 2024-04-30 18:56:21.562013 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_response.py
+-rw-r--r--   0        0        0     3912 2024-04-30 18:56:21.562096 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_response.pyi
+-rw-r--r--   0        0        0     3437 2024-04-30 18:56:21.562340 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_response_sources.py
+-rw-r--r--   0        0        0     3437 2024-04-30 18:56:21.562428 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_response_sources.pyi
+-rw-r--r--   0        0        0     6854 2024-04-30 18:56:21.562534 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/sources_request.py
+-rw-r--r--   0        0        0     6854 2024-04-30 18:56:21.562635 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/sources_request.pyi
+-rw-r--r--   0        0        0     5919 2024-04-30 18:56:21.562736 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/subscription_response.py
+-rw-r--r--   0        0        0     5919 2024-04-30 18:56:21.562835 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/subscription_response.pyi
+-rw-r--r--   0        0        0     3626 2024-04-30 18:56:21.562923 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/validation_error.py
+-rw-r--r--   0        0        0     3626 2024-04-30 18:56:21.563006 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/validation_error.pyi
+-rw-r--r--   0        0        0     3408 2024-04-30 18:56:21.563087 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/validation_error_loc.py
+-rw-r--r--   0        0        0     3408 2024-04-30 18:56:21.563175 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/validation_error_loc.pyi
+-rw-r--r--   0        0        0     4137 2024-04-30 18:57:54.511641 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/models/__init__.py
+-rw-r--r--   0        0        0    25187 2024-04-30 18:57:54.512362 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/operation_parameter_map.py
+-rw-r--r--   0        0        0      582 2024-04-30 18:57:54.512514 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/__init__.py
+-rw-r--r--   0        0        0      323 2024-04-30 18:56:21.563600 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_authors/__init__.py
+-rw-r--r--   0        0        0    66916 2024-04-30 18:56:21.563726 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_authors/get.py
+-rw-r--r--   0        0        0    66607 2024-04-30 18:56:21.563861 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_authors/get.pyi
+-rw-r--r--   0        0        0    47473 2024-04-30 18:56:21.563979 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_authors/post.py
+-rw-r--r--   0        0        0    47336 2024-04-30 18:56:21.564096 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_authors/post.pyi
+-rw-r--r--   0        0        0      341 2024-04-30 18:56:21.564195 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_latest_headlines/__init__.py
+-rw-r--r--   0        0        0    66032 2024-04-30 18:56:21.564318 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_latest_headlines/get.py
+-rw-r--r--   0        0        0    65723 2024-04-30 18:56:21.564450 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_latest_headlines/get.pyi
+-rw-r--r--   0        0        0    49192 2024-04-30 18:56:21.564573 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_latest_headlines/post.py
+-rw-r--r--   0        0        0    49055 2024-04-30 18:56:21.564694 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_latest_headlines/post.pyi
+-rw-r--r--   0        0        0      321 2024-04-30 18:56:21.564793 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search/__init__.py
+-rw-r--r--   0        0        0    78572 2024-04-30 18:56:21.564919 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search/get.py
+-rw-r--r--   0        0        0    78263 2024-04-30 18:56:21.565059 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search/get.pyi
+-rw-r--r--   0        0        0    55220 2024-04-30 18:56:21.565185 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search/post.py
+-rw-r--r--   0        0        0    55083 2024-04-30 18:56:21.565318 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search/post.pyi
+-rw-r--r--   0        0        0      337 2024-04-30 18:56:21.565429 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_by_link/__init__.py
+-rw-r--r--   0        0        0    19293 2024-04-30 18:56:21.565532 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_by_link/get.py
+-rw-r--r--   0        0        0    19070 2024-04-30 18:56:21.565636 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_by_link/get.pyi
+-rw-r--r--   0        0        0    17699 2024-04-30 18:56:21.565741 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_by_link/post.py
+-rw-r--r--   0        0        0    17562 2024-04-30 18:56:21.565842 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_by_link/post.pyi
+-rw-r--r--   0        0        0      337 2024-04-30 18:56:21.565936 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_similar/__init__.py
+-rw-r--r--   0        0        0    67713 2024-04-30 18:56:21.566056 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_similar/get.py
+-rw-r--r--   0        0        0    67361 2024-04-30 18:56:21.566193 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_similar/get.pyi
+-rw-r--r--   0        0        0    47930 2024-04-30 18:56:21.566310 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_similar/post.py
+-rw-r--r--   0        0        0    47793 2024-04-30 18:56:21.566427 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_similar/post.pyi
+-rw-r--r--   0        0        0      323 2024-04-30 18:56:21.566522 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_sources/__init__.py
+-rw-r--r--   0        0        0    22889 2024-04-30 18:56:21.566618 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_sources/get.py
+-rw-r--r--   0        0        0    22752 2024-04-30 18:56:21.566723 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_sources/get.pyi
+-rw-r--r--   0        0        0    19936 2024-04-30 18:56:21.566824 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_sources/post.py
+-rw-r--r--   0        0        0    19799 2024-04-30 18:56:21.566942 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_sources/post.pyi
+-rw-r--r--   0        0        0      333 2024-04-30 18:56:21.567041 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_subscription/__init__.py
+-rw-r--r--   0        0        0    12067 2024-04-30 18:56:21.567126 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_subscription/get.py
+-rw-r--r--   0        0        0    11930 2024-04-30 18:56:21.567281 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_subscription/get.pyi
+-rw-r--r--   0        0        0    12093 2024-04-30 18:56:21.567418 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_subscription/post.py
+-rw-r--r--   0        0        0    11956 2024-04-30 18:56:21.567553 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_subscription/post.pyi
+-rw-r--r--   0        0        0        0 2024-04-30 18:56:21.567674 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-30 18:56:21.567764 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/additional_source_info.py
+-rw-r--r--   0        0        0     4726 2024-04-30 18:56:21.567866 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/author_search_request.py
+-rw-r--r--   0        0        0     1061 2024-04-30 18:56:21.567951 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/authors_get_response.py
+-rw-r--r--   0        0        0     1062 2024-04-30 18:56:21.568036 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/authors_post_response.py
+-rw-r--r--   0        0        0      995 2024-04-30 18:56:21.568123 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/cluster.py
+-rw-r--r--   0        0        0      665 2024-04-30 18:56:21.568214 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/cluster_articles.py
+-rw-r--r--   0        0        0     1336 2024-04-30 18:56:21.568297 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/clustering_search_response.py
+-rw-r--r--   0        0        0     3052 2024-04-30 18:56:21.568387 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0     1542 2024-04-30 18:56:21.568476 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     1436 2024-04-30 18:56:21.568559 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0      704 2024-04-30 18:56:21.568652 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     3239 2024-04-30 18:56:21.568738 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0     1543 2024-04-30 18:56:21.568825 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     1437 2024-04-30 18:56:21.568912 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0      704 2024-04-30 18:56:21.569008 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1411 2024-04-30 18:56:21.569100 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0      698 2024-04-30 18:56:21.569187 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0      937 2024-04-30 18:56:21.569275 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/http_validation_error.py
+-rw-r--r--   0        0        0      907 2024-04-30 18:56:21.569369 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/latest_headlines_get_response.py
+-rw-r--r--   0        0        0      908 2024-04-30 18:56:21.569452 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     4897 2024-04-30 18:56:21.569556 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/latest_headlines_request.py
+-rw-r--r--   0        0        0     1340 2024-04-30 18:56:21.569636 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/latest_headlines_response.py
+-rw-r--r--   0        0        0      681 2024-04-30 18:56:21.569727 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     4721 2024-04-30 18:56:21.569831 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/more_like_this_request.py
+-rw-r--r--   0        0        0      952 2024-04-30 18:56:21.569912 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_get_response.py
+-rw-r--r--   0        0        0      953 2024-04-30 18:56:21.569995 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_post_response.py
+-rw-r--r--   0        0        0     5628 2024-04-30 18:56:21.570097 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_request.py
+-rw-r--r--   0        0        0     1069 2024-04-30 18:56:21.570183 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_similar_get_response.py
+-rw-r--r--   0        0        0     1070 2024-04-30 18:56:21.570272 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_similar_post_response.py
+-rw-r--r--   0        0        0     1151 2024-04-30 18:56:21.570362 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_url_request.py
+-rw-r--r--   0        0        0      937 2024-04-30 18:56:21.570449 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/similar_document.py
+-rw-r--r--   0        0        0     1132 2024-04-30 18:56:21.570532 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/source_info.py
+-rw-r--r--   0        0        0     1093 2024-04-30 18:56:21.570618 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/source_response.py
+-rw-r--r--   0        0        0      760 2024-04-30 18:56:21.570701 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/source_response_sources.py
+-rw-r--r--   0        0        0     1432 2024-04-30 18:56:21.570793 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/sources_request.py
+-rw-r--r--   0        0        0     1216 2024-04-30 18:56:21.570882 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/subscription_response.py
+-rw-r--r--   0        0        0      973 2024-04-30 18:56:21.570968 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/validation_error.py
+-rw-r--r--   0        0        0      684 2024-04-30 18:56:21.571052 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/validation_error_loc.py
+-rw-r--r--   0        0        0      913 2024-04-30 18:56:21.571149 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/request_after_hook.py
+-rw-r--r--   0        0        0      971 2024-04-30 18:56:21.571246 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/request_before_hook.py
+-rw-r--r--   0        0        0      936 2024-04-30 18:56:21.571334 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/request_before_url_hook.py
+-rw-r--r--   0        0        0    11233 2024-04-30 18:56:21.571424 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/rest.py
+-rw-r--r--   0        0        0    96391 2024-04-30 18:56:21.571626 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:56:21.571728 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-30 18:56:21.571823 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/additional_source_info.py
+-rw-r--r--   0        0        0     2699 2024-04-30 18:56:21.571910 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/author_search_request.py
+-rw-r--r--   0        0        0      992 2024-04-30 18:56:21.571996 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/authors_get_response.py
+-rw-r--r--   0        0        0      993 2024-04-30 18:56:21.572084 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/authors_post_response.py
+-rw-r--r--   0        0        0      862 2024-04-30 18:56:21.572168 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/cluster.py
+-rw-r--r--   0        0        0      604 2024-04-30 18:56:21.572253 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/cluster_articles.py
+-rw-r--r--   0        0        0     1106 2024-04-30 18:56:21.572346 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/clustering_search_response.py
+-rw-r--r--   0        0        0     1778 2024-04-30 18:56:21.572437 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0     1341 2024-04-30 18:56:21.572528 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     1326 2024-04-30 18:56:21.572673 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0      643 2024-04-30 18:56:21.572828 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1903 2024-04-30 18:56:21.572937 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0     1342 2024-04-30 18:56:21.573039 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     1327 2024-04-30 18:56:21.573140 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0      643 2024-04-30 18:56:21.573242 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1277 2024-04-30 18:56:21.573345 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0      637 2024-04-30 18:56:21.573437 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0      889 2024-04-30 18:56:21.573529 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/http_validation_error.py
+-rw-r--r--   0        0        0      838 2024-04-30 18:56:21.573623 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/latest_headlines_get_response.py
+-rw-r--r--   0        0        0      839 2024-04-30 18:56:21.573713 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     2812 2024-04-30 18:56:21.573798 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/latest_headlines_request.py
+-rw-r--r--   0        0        0     1138 2024-04-30 18:56:21.573890 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/latest_headlines_response.py
+-rw-r--r--   0        0        0      620 2024-04-30 18:56:21.573990 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     2616 2024-04-30 18:56:21.574081 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/more_like_this_request.py
+-rw-r--r--   0        0        0      883 2024-04-30 18:56:21.574167 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_get_response.py
+-rw-r--r--   0        0        0      884 2024-04-30 18:56:21.574251 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_post_response.py
+-rw-r--r--   0        0        0     3061 2024-04-30 18:56:21.574338 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_request.py
+-rw-r--r--   0        0        0     1000 2024-04-30 18:56:21.574423 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_similar_get_response.py
+-rw-r--r--   0        0        0     1001 2024-04-30 18:56:21.574509 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_similar_post_response.py
+-rw-r--r--   0        0        0      957 2024-04-30 18:56:21.574596 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_url_request.py
+-rw-r--r--   0        0        0      836 2024-04-30 18:56:21.574690 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/similar_document.py
+-rw-r--r--   0        0        0      904 2024-04-30 18:56:21.574772 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/source_info.py
+-rw-r--r--   0        0        0      994 2024-04-30 18:56:21.574855 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/source_response.py
+-rw-r--r--   0        0        0      695 2024-04-30 18:56:21.574941 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/source_response_sources.py
+-rw-r--r--   0        0        0      996 2024-04-30 18:56:21.575032 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/sources_request.py
+-rw-r--r--   0        0        0      925 2024-04-30 18:56:21.575121 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/subscription_response.py
+-rw-r--r--   0        0        0      892 2024-04-30 18:56:21.575204 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/validation_error.py
+-rw-r--r--   0        0        0      623 2024-04-30 18:56:21.575284 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/validation_error_loc.py
+-rw-r--r--   0        0        0      758 2024-04-30 18:56:21.575373 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type_util.py
+-rw-r--r--   0        0        0     3177 2024-04-30 18:56:21.575461 newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/validation_metadata.py
+-rw-r--r--   0        0        0      791 2024-04-30 18:57:54.512971 newscatcherapi_python_sdk-6.0.6/pyproject.toml
+-rw-r--r--   0        0        0    76725 1970-01-01 00:00:00.000000 newscatcherapi_python_sdk-6.0.6/PKG-INFO
```

### Comparing `newscatcherapi_python_sdk-6.0.5/LICENSE` & `newscatcherapi_python_sdk-6.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/README.md` & `newscatcherapi_python_sdk-6.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,39 @@
+Metadata-Version: 2.1
+Name: newscatcherapi-python-sdk
+Version: 6.0.6
+Summary: Client for NewsCatcher-V3 Production API
+License: MIT
+Author: Maksym Sugonyaka
+Author-email: maksym@newscatcherapi.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: certifi (>=2023.7.22)
+Requires-Dist: cryptography (>=42.0.5,<43.0.0)
+Requires-Dist: frozendict (>=2.3.4,<3.0.0)
+Requires-Dist: pydantic (>=2.4.2,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
+Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
+Description-Content-Type: text/markdown
+
 # newscatcherapi-python-sdk<a id="newscatcherapi-python-sdk"></a>
 
 <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v6.0.5-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.5)
+[![PyPI](https://img.shields.io/badge/PyPI-v6.0.6-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.6)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/konfig-dev/newscatcher-sdks/tree/main/v3/python#readme)
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
 
 - [Requirements](#requirements)
@@ -26,27 +52,25 @@
   * [`newscatcher.search_link.post`](#newscatchersearch_linkpost)
   * [`newscatcher.search_similar.get`](#newscatchersearch_similarget)
   * [`newscatcher.search_similar.post`](#newscatchersearch_similarpost)
   * [`newscatcher.sources.get`](#newscatchersourcesget)
   * [`newscatcher.sources.post`](#newscatchersourcespost)
   * [`newscatcher.subscription.get`](#newscatchersubscriptionget)
   * [`newscatcher.subscription.post`](#newscatchersubscriptionpost)
-  * [`newscatcher.search_duplicates_by_original_id.get`](#newscatchersearch_duplicates_by_original_idget)
-  * [`newscatcher.search_duplicates_by_original_id.post`](#newscatchersearch_duplicates_by_original_idpost)
 
 <!-- tocstop -->
 
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install newscatcherapi-python-sdk==6.0.5
+pip install newscatcherapi-python-sdk==6.0.6
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from pprint import pprint
 from newscatcherapi_client import Newscatcher, ApiException
@@ -1693,81 +1717,11 @@
 
 `/api/subscription` `post`
 
 [🔙 **Back to Table of Contents**](#table-of-contents)
 
 ---
 
-### `newscatcher.search_duplicates_by_original_id.get`<a id="newscatchersearch_duplicates_by_original_idget"></a>
-
-This endpoint allows you to search for duplicate articles by original article id.
-
-#### 🛠️ Usage<a id="🛠️-usage"></a>
-
-```python
-get_response = newscatcher.search_duplicates_by_original_id.get(
-    original_article_id="original_article_id_example",
-    page=1,
-    page_size=100,
-)
-```
-
-#### ⚙️ Parameters<a id="⚙️-parameters"></a>
-
-##### original_article_id: `str`<a id="original_article_id-str"></a>
-
-##### page: `int`<a id="page-int"></a>
-
-##### page_size: `int`<a id="page_size-int"></a>
-
-#### 🔄 Return<a id="🔄-return"></a>
-
-[`SearchduplicatesbyoriginalidGetResponse`](./newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_get_response.py)
-
-#### 🌐 Endpoint<a id="🌐-endpoint"></a>
-
-`/api/search_duplicates_by_original_id` `get`
-
-[🔙 **Back to Table of Contents**](#table-of-contents)
-
----
-
-### `newscatcher.search_duplicates_by_original_id.post`<a id="newscatchersearch_duplicates_by_original_idpost"></a>
-
-This endpoint allows you to search for duplicate articles by original article id.
-
-#### 🛠️ Usage<a id="🛠️-usage"></a>
-
-```python
-post_response = newscatcher.search_duplicates_by_original_id.post(
-    original_article_id="string_example",
-    page=1,
-    page_size=100,
-)
-```
-
-#### ⚙️ Parameters<a id="⚙️-parameters"></a>
-
-##### original_article_id: `str`<a id="original_article_id-str"></a>
-
-##### page: `int`<a id="page-int"></a>
-
-##### page_size: `int`<a id="page_size-int"></a>
-
-#### ⚙️ Request Body<a id="⚙️-request-body"></a>
-
-[`DuplicatesByOriginalIdRequest`](./newscatcherapi_client/type/duplicates_by_original_id_request.py)
-#### 🔄 Return<a id="🔄-return"></a>
-
-[`SearchduplicatesbyoriginalidPostResponse`](./newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_post_response.py)
-
-#### 🌐 Endpoint<a id="🌐-endpoint"></a>
-
-`/api/search_duplicates_by_original_id` `post`
-
-[🔙 **Back to Table of Contents**](#table-of-contents)
-
----
-
 
 ## Author<a id="author"></a>
 This Python package is automatically generated by [Konfig](https://konfigthis.com)
+
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/__init__.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
     The version of the OpenAPI document: 3.2.16
     Contact: maksym@newscatcherapi.com
     Generated by: https://konfigthis.com
 """
 
-__version__ = "6.0.5"
+__version__ = "6.0.6"
 
 # import ApiClient
 from newscatcherapi_client.api_client import ApiClient
 
 # import Configuration
 from newscatcherapi_client.configuration import Configuration
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8 # flake8: noqa """ NewsCatcher-V3 Production API [https://
 uploads-ssl.webflow.com/6429857b17973b636c2195c5/
 646c6f1eb774ff2f2997bec5_newscatcher_.svg]
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
-konfigthis.com """ __version__ = "6.0.5" # import ApiClient from
+konfigthis.com """ __version__ = "6.0.6" # import ApiClient from
 newscatcherapi_client.api_client import ApiClient # import Configuration from
 newscatcherapi_client.configuration import Configuration # import exceptions
 from newscatcherapi_client.exceptions import OpenApiException from
 newscatcherapi_client.exceptions import ApiAttributeError from
 newscatcherapi_client.exceptions import ApiTypeError from
 newscatcherapi_client.exceptions import ApiValueError from
 newscatcherapi_client.exceptions import ApiKeyError from
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/api_client.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2984,15 +2984,15 @@
 0000ba70: 655d 203d 2068 6561 6465 725f 7661 6c75  e] = header_valu
 0000ba80: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
 0000ba90: 6f6f 6b69 6520 3d20 636f 6f6b 6965 0a20  ookie = cookie. 
 0000baa0: 2020 2020 2020 2023 2053 6574 2064 6566         # Set def
 0000bab0: 6175 6c74 2055 7365 722d 4167 656e 742e  ault User-Agent.
 0000bac0: 0a20 2020 2020 2020 2073 656c 662e 7573  .        self.us
 0000bad0: 6572 5f61 6765 6e74 203d 2027 4b6f 6e66  er_agent = 'Konf
-0000bae0: 6967 2f36 2e30 2e35 2f70 7974 686f 6e27  ig/6.0.5/python'
+0000bae0: 6967 2f36 2e30 2e36 2f70 7974 686f 6e27  ig/6.0.6/python'
 0000baf0: 0a0a 2020 2020 6465 6620 5f5f 656e 7465  ..    def __ente
 0000bb00: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
 0000bb10: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
 0000bb20: 2020 2020 6465 6620 5f5f 6578 6974 5f5f      def __exit__
 0000bb30: 2873 656c 662c 2065 7863 5f74 7970 652c  (self, exc_type,
 0000bb40: 2065 7863 5f76 616c 7565 2c20 7472 6163   exc_value, trac
 0000bb50: 6562 6163 6b29 3a0a 2020 2020 2020 2020  eback):.
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/api_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/api_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/path_to_api.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/path_to_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,35 +4,32 @@
 from newscatcherapi_client.apis.paths.api_search import ApiSearch
 from newscatcherapi_client.apis.paths.api_latest_headlines import ApiLatestHeadlines
 from newscatcherapi_client.apis.paths.api_authors import ApiAuthors
 from newscatcherapi_client.apis.paths.api_search_by_link import ApiSearchByLink
 from newscatcherapi_client.apis.paths.api_search_similar import ApiSearchSimilar
 from newscatcherapi_client.apis.paths.api_sources import ApiSources
 from newscatcherapi_client.apis.paths.api_subscription import ApiSubscription
-from newscatcherapi_client.apis.paths.api_search_duplicates_by_original_id import ApiSearchDuplicatesByOriginalId
 
 PathToApi = typing_extensions.TypedDict(
     'PathToApi',
     {
         PathValues.API_SEARCH: ApiSearch,
         PathValues.API_LATEST_HEADLINES: ApiLatestHeadlines,
         PathValues.API_AUTHORS: ApiAuthors,
         PathValues.API_SEARCH_BY_LINK: ApiSearchByLink,
         PathValues.API_SEARCH_SIMILAR: ApiSearchSimilar,
         PathValues.API_SOURCES: ApiSources,
         PathValues.API_SUBSCRIPTION: ApiSubscription,
-        PathValues.API_SEARCH_DUPLICATES_BY_ORIGINAL_ID: ApiSearchDuplicatesByOriginalId,
     }
 )
 
 path_to_api = PathToApi(
     {
         PathValues.API_SEARCH: ApiSearch,
         PathValues.API_LATEST_HEADLINES: ApiLatestHeadlines,
         PathValues.API_AUTHORS: ApiAuthors,
         PathValues.API_SEARCH_BY_LINK: ApiSearchByLink,
         PathValues.API_SEARCH_SIMILAR: ApiSearchSimilar,
         PathValues.API_SOURCES: ApiSources,
         PathValues.API_SUBSCRIPTION: ApiSubscription,
-        PathValues.API_SEARCH_DUPLICATES_BY_ORIGINAL_ID: ApiSearchDuplicatesByOriginalId,
     }
 )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tag_to_api.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tag_to_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,35 +4,32 @@
 from newscatcherapi_client.apis.tags.search_api import SearchApi
 from newscatcherapi_client.apis.tags.latest_headlines_api import LatestHeadlinesApi
 from newscatcherapi_client.apis.tags.authors_api import AuthorsApi
 from newscatcherapi_client.apis.tags.search_link_api import SearchLinkApi
 from newscatcherapi_client.apis.tags.search_similar_api import SearchSimilarApi
 from newscatcherapi_client.apis.tags.sources_api import SourcesApi
 from newscatcherapi_client.apis.tags.subscription_api import SubscriptionApi
-from newscatcherapi_client.apis.tags.search_duplicates_by_original_id_api import SearchDuplicatesByOriginalIdApi
 
 TagToApi = typing_extensions.TypedDict(
     'TagToApi',
     {
         TagValues.SEARCH: SearchApi,
         TagValues.LATEST_HEADLINES: LatestHeadlinesApi,
         TagValues.AUTHORS: AuthorsApi,
         TagValues.SEARCH_LINK: SearchLinkApi,
         TagValues.SEARCH_SIMILAR: SearchSimilarApi,
         TagValues.SOURCES: SourcesApi,
         TagValues.SUBSCRIPTION: SubscriptionApi,
-        TagValues.SEARCH_DUPLICATES_BY_ORIGINAL_ID: SearchDuplicatesByOriginalIdApi,
     }
 )
 
 tag_to_api = TagToApi(
     {
         TagValues.SEARCH: SearchApi,
         TagValues.LATEST_HEADLINES: LatestHeadlinesApi,
         TagValues.AUTHORS: AuthorsApi,
         TagValues.SEARCH_LINK: SearchLinkApi,
         TagValues.SEARCH_SIMILAR: SearchSimilarApi,
         TagValues.SOURCES: SourcesApi,
         TagValues.SUBSCRIPTION: SubscriptionApi,
-        TagValues.SEARCH_DUPLICATES_BY_ORIGINAL_ID: SearchDuplicatesByOriginalIdApi,
     }
 )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/authors_api.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/authors_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/authors_api_raw.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/authors_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/latest_headlines_api.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/latest_headlines_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_api.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_api_raw.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_duplicates_by_original_id_api.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_similar_api_raw.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,45 +23,24 @@
 00000160: 6374 3a20 6d61 6b73 796d 406e 6577 7363  ct: maksym@newsc
 00000170: 6174 6368 6572 6170 692e 636f 6d0a 2020  atcherapi.com.  
 00000180: 2020 4765 6e65 7261 7465 6420 6279 3a20    Generated by: 
 00000190: 6874 7470 733a 2f2f 6b6f 6e66 6967 7468  https://konfigth
 000001a0: 6973 2e63 6f6d 0a22 2222 0a0a 6672 6f6d  is.com."""..from
 000001b0: 206e 6577 7363 6174 6368 6572 6170 695f   newscatcherapi_
 000001c0: 636c 6965 6e74 2e70 6174 6873 2e61 7069  client.paths.api
-000001d0: 5f73 6561 7263 685f 6475 706c 6963 6174  _search_duplicat
-000001e0: 6573 5f62 795f 6f72 6967 696e 616c 5f69  es_by_original_i
-000001f0: 642e 6765 7420 696d 706f 7274 2047 6574  d.get import Get
-00000200: 0a66 726f 6d20 6e65 7773 6361 7463 6865  .from newscatche
-00000210: 7261 7069 5f63 6c69 656e 742e 7061 7468  rapi_client.path
-00000220: 732e 6170 695f 7365 6172 6368 5f64 7570  s.api_search_dup
-00000230: 6c69 6361 7465 735f 6279 5f6f 7269 6769  licates_by_origi
-00000240: 6e61 6c5f 6964 2e70 6f73 7420 696d 706f  nal_id.post impo
-00000250: 7274 2050 6f73 740a 6672 6f6d 206e 6577  rt Post.from new
-00000260: 7363 6174 6368 6572 6170 695f 636c 6965  scatcherapi_clie
-00000270: 6e74 2e61 7069 732e 7461 6773 2e73 6561  nt.apis.tags.sea
-00000280: 7263 685f 6475 706c 6963 6174 6573 5f62  rch_duplicates_b
-00000290: 795f 6f72 6967 696e 616c 5f69 645f 6170  y_original_id_ap
-000002a0: 695f 7261 7720 696d 706f 7274 2053 6561  i_raw import Sea
-000002b0: 7263 6844 7570 6c69 6361 7465 7342 794f  rchDuplicatesByO
-000002c0: 7269 6769 6e61 6c49 6441 7069 5261 770a  riginalIdApiRaw.
-000002d0: 0a0a 636c 6173 7320 5365 6172 6368 4475  ..class SearchDu
-000002e0: 706c 6963 6174 6573 4279 4f72 6967 696e  plicatesByOrigin
-000002f0: 616c 4964 4170 6928 0a20 2020 2047 6574  alIdApi(.    Get
-00000300: 2c0a 2020 2020 506f 7374 2c0a 293a 0a20  ,.    Post,.):. 
-00000310: 2020 2022 2222 4e4f 5445 3a0a 2020 2020     """NOTE:.    
-00000320: 5468 6973 2063 6c61 7373 2069 7320 6175  This class is au
-00000330: 746f 2067 656e 6572 6174 6564 2062 7920  to generated by 
-00000340: 4b6f 6e66 6967 2028 6874 7470 733a 2f2f  Konfig (https://
-00000350: 6b6f 6e66 6967 7468 6973 2e63 6f6d 290a  konfigthis.com).
-00000360: 2020 2020 2222 220a 2020 2020 7261 773a      """.    raw:
-00000370: 2053 6561 7263 6844 7570 6c69 6361 7465   SearchDuplicate
-00000380: 7342 794f 7269 6769 6e61 6c49 6441 7069  sByOriginalIdApi
-00000390: 5261 770a 0a20 2020 2064 6566 205f 5f69  Raw..    def __i
-000003a0: 6e69 745f 5f28 7365 6c66 2c20 6170 695f  nit__(self, api_
-000003b0: 636c 6965 6e74 3d4e 6f6e 6529 3a0a 2020  client=None):.  
-000003c0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-000003d0: 696e 6974 5f5f 2861 7069 5f63 6c69 656e  init__(api_clien
-000003e0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-000003f0: 7261 7720 3d20 5365 6172 6368 4475 706c  raw = SearchDupl
-00000400: 6963 6174 6573 4279 4f72 6967 696e 616c  icatesByOriginal
-00000410: 4964 4170 6952 6177 2861 7069 5f63 6c69  IdApiRaw(api_cli
-00000420: 656e 7429 0a                             ent).
+000001d0: 5f73 6561 7263 685f 7369 6d69 6c61 722e  _search_similar.
+000001e0: 6765 7420 696d 706f 7274 2047 6574 5261  get import GetRa
+000001f0: 770a 6672 6f6d 206e 6577 7363 6174 6368  w.from newscatch
+00000200: 6572 6170 695f 636c 6965 6e74 2e70 6174  erapi_client.pat
+00000210: 6873 2e61 7069 5f73 6561 7263 685f 7369  hs.api_search_si
+00000220: 6d69 6c61 722e 706f 7374 2069 6d70 6f72  milar.post impor
+00000230: 7420 506f 7374 5261 770a 0a0a 636c 6173  t PostRaw...clas
+00000240: 7320 5365 6172 6368 5369 6d69 6c61 7241  s SearchSimilarA
+00000250: 7069 5261 7728 0a20 2020 2047 6574 5261  piRaw(.    GetRa
+00000260: 772c 0a20 2020 2050 6f73 7452 6177 2c0a  w,.    PostRaw,.
+00000270: 293a 0a20 2020 2022 2222 4e4f 5445 3a0a  ):.    """NOTE:.
+00000280: 2020 2020 5468 6973 2063 6c61 7373 2069      This class i
+00000290: 7320 6175 746f 2067 656e 6572 6174 6564  s auto generated
+000002a0: 2062 7920 4b6f 6e66 6967 2028 6874 7470   by Konfig (http
+000002b0: 733a 2f2f 6b6f 6e66 6967 7468 6973 2e63  s://konfigthis.c
+000002c0: 6f6d 290a 2020 2020 2222 220a 2020 2020  om).    """.    
+000002d0: 7061 7373 0a                             pass.
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_duplicates_by_original_id_api_raw.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/subscription_api_raw.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
     The version of the OpenAPI document: 3.2.16
     Contact: maksym@newscatcherapi.com
     Generated by: https://konfigthis.com
 """
 
-from newscatcherapi_client.paths.api_search_duplicates_by_original_id.get import GetRaw
-from newscatcherapi_client.paths.api_search_duplicates_by_original_id.post import PostRaw
+from newscatcherapi_client.paths.api_subscription.get import GetRaw
+from newscatcherapi_client.paths.api_subscription.post import PostRaw
 
 
-class SearchDuplicatesByOriginalIdApiRaw(
+class SubscriptionApiRaw(
     GetRaw,
     PostRaw,
 ):
     """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
     pass
```

#### html2text {}

```diff
@@ -1,12 +1,10 @@
 # coding: utf-8 """ NewsCatcher-V3 Production API [https://uploads-
 ssl.webflow.com/6429857b17973b636c2195c5/
 646c6f1eb774ff2f2997bec5_newscatcher_.svg]
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
-konfigthis.com """ from
-newscatcherapi_client.paths.api_search_duplicates_by_original_id.get import
-GetRaw from
-newscatcherapi_client.paths.api_search_duplicates_by_original_id.post import
-PostRaw class SearchDuplicatesByOriginalIdApiRaw( GetRaw, PostRaw, ): """NOTE:
-This class is auto generated by Konfig (https://konfigthis.com) """ pass
+konfigthis.com """ from newscatcherapi_client.paths.api_subscription.get import
+GetRaw from newscatcherapi_client.paths.api_subscription.post import PostRaw
+class SubscriptionApiRaw( GetRaw, PostRaw, ): """NOTE: This class is auto
+generated by Konfig (https://konfigthis.com) """ pass
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_link_api.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_link_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_link_api_raw.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_link_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_similar_api.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/search_similar_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_similar_api_raw.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/sources_api_raw.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
     The version of the OpenAPI document: 3.2.16
     Contact: maksym@newscatcherapi.com
     Generated by: https://konfigthis.com
 """
 
-from newscatcherapi_client.paths.api_search_similar.get import GetRaw
-from newscatcherapi_client.paths.api_search_similar.post import PostRaw
+from newscatcherapi_client.paths.api_sources.get import GetRaw
+from newscatcherapi_client.paths.api_sources.post import PostRaw
 
 
-class SearchSimilarApiRaw(
+class SourcesApiRaw(
     GetRaw,
     PostRaw,
 ):
     """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
     pass
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8 """ NewsCatcher-V3 Production API [https://uploads-
 ssl.webflow.com/6429857b17973b636c2195c5/
 646c6f1eb774ff2f2997bec5_newscatcher_.svg]
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
-konfigthis.com """ from newscatcherapi_client.paths.api_search_similar.get
-import GetRaw from newscatcherapi_client.paths.api_search_similar.post import
-PostRaw class SearchSimilarApiRaw( GetRaw, PostRaw, ): """NOTE: This class is
-auto generated by Konfig (https://konfigthis.com) """ pass
+konfigthis.com """ from newscatcherapi_client.paths.api_sources.get import
+GetRaw from newscatcherapi_client.paths.api_sources.post import PostRaw class
+SourcesApiRaw( GetRaw, PostRaw, ): """NOTE: This class is auto generated by
+Konfig (https://konfigthis.com) """ pass
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/sources_api.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/sources_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/subscription_api.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/apis/tags/subscription_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from newscatcherapi_client.apis.tags.authors_api import AuthorsApi
 from newscatcherapi_client.apis.tags.latest_headlines_api import LatestHeadlinesApi
 from newscatcherapi_client.apis.tags.search_api import SearchApi
 from newscatcherapi_client.apis.tags.search_link_api import SearchLinkApi
 from newscatcherapi_client.apis.tags.search_similar_api import SearchSimilarApi
 from newscatcherapi_client.apis.tags.sources_api import SourcesApi
 from newscatcherapi_client.apis.tags.subscription_api import SubscriptionApi
-from newscatcherapi_client.apis.tags.search_duplicates_by_original_id_api import SearchDuplicatesByOriginalIdApi
 
 
 
 class Newscatcher(ClientCustom):
 
     def __init__(self, configuration: typing.Union[Configuration, None] = None, **kwargs):
         super().__init__(configuration, **kwargs)
@@ -39,8 +38,7 @@
         self.authors: AuthorsApi = AuthorsApi(api_client)
         self.latest_headlines: LatestHeadlinesApi = LatestHeadlinesApi(api_client)
         self.search: SearchApi = SearchApi(api_client)
         self.search_link: SearchLinkApi = SearchLinkApi(api_client)
         self.search_similar: SearchSimilarApi = SearchSimilarApi(api_client)
         self.sources: SourcesApi = SourcesApi(api_client)
         self.subscription: SubscriptionApi = SubscriptionApi(api_client)
-        self.search_duplicates_by_original_id: SearchDuplicatesByOriginalIdApi = SearchDuplicatesByOriginalIdApi(api_client)
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from newscatcherapi_client.apis.tags.authors_api import AuthorsApi
 from newscatcherapi_client.apis.tags.latest_headlines_api import LatestHeadlinesApi
 from newscatcherapi_client.apis.tags.search_api import SearchApi
 from newscatcherapi_client.apis.tags.search_link_api import SearchLinkApi
 from newscatcherapi_client.apis.tags.search_similar_api import SearchSimilarApi
 from newscatcherapi_client.apis.tags.sources_api import SourcesApi
 from newscatcherapi_client.apis.tags.subscription_api import SubscriptionApi
-from newscatcherapi_client.apis.tags.search_duplicates_by_original_id_api import SearchDuplicatesByOriginalIdApi
 
 
 
 class Newscatcher(ClientCustom):
 
     def __init__(self, configuration: typing.Union[Configuration, None] = None, **kwargs):
         super().__init__(configuration, **kwargs)
@@ -39,8 +38,7 @@
         self.authors: AuthorsApi = AuthorsApi(api_client)
         self.latest_headlines: LatestHeadlinesApi = LatestHeadlinesApi(api_client)
         self.search: SearchApi = SearchApi(api_client)
         self.search_link: SearchLinkApi = SearchLinkApi(api_client)
         self.search_similar: SearchSimilarApi = SearchSimilarApi(api_client)
         self.sources: SourcesApi = SourcesApi(api_client)
         self.subscription: SubscriptionApi = SubscriptionApi(api_client)
-        self.search_duplicates_by_original_id: SearchDuplicatesByOriginalIdApi = SearchDuplicatesByOriginalIdApi(api_client)
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client_custom.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/client_custom.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/configuration.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.2.16\n"\
-               "SDK Package Version: 6.0.5".\
+               "SDK Package Version: 6.0.6".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/exceptions.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/exceptions_base.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/additional_source_info.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/additional_source_info.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/author_search_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/author_search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/author_search_request.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/author_search_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_get_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/authors_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_post_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/authors_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/cluster.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster_articles.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/cluster_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/clustering_search_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/clustering_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/duplicates_by_original_id_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_url_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class DuplicatesByOriginalIdRequest(
+class SearchURLRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Duplicates by original article ID request DTO
+    Search URL Request DTO.
     """
 
 
     class MetaOapg:
-        required = {
-            "original_article_id",
-        }
         
         class properties:
-            original_article_id = schemas.StrSchema
+            ids = schemas.AnyTypeSchema
+            links = schemas.AnyTypeSchema
             
             
             class page(
                 schemas.IntSchema
             ):
             
             
@@ -56,65 +54,72 @@
                 schemas.IntSchema
             ):
             
             
                 class MetaOapg:
                     inclusive_minimum = 0
             __annotations__ = {
-                "original_article_id": original_article_id,
+                "ids": ids,
+                "links": links,
                 "page": page,
                 "page_size": page_size,
             }
     
-    original_article_id: MetaOapg.properties.original_article_id
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["ids"]) -> MetaOapg.properties.ids: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["original_article_id"]) -> MetaOapg.properties.original_article_id: ...
+    def __getitem__(self, name: typing_extensions.Literal["links"]) -> MetaOapg.properties.links: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["page_size"]) -> MetaOapg.properties.page_size: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["original_article_id", "page", "page_size", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["original_article_id"]) -> MetaOapg.properties.original_article_id: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["ids"]) -> typing.Union[MetaOapg.properties.ids, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["links"]) -> typing.Union[MetaOapg.properties.links, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["page"]) -> typing.Union[MetaOapg.properties.page, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["page_size"]) -> typing.Union[MetaOapg.properties.page_size, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["original_article_id", "page", "page_size", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        original_article_id: typing.Union[MetaOapg.properties.original_article_id, str, ],
+        ids: typing.Union[MetaOapg.properties.ids, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        links: typing.Union[MetaOapg.properties.links, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         page: typing.Union[MetaOapg.properties.page, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         page_size: typing.Union[MetaOapg.properties.page_size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DuplicatesByOriginalIdRequest':
+    ) -> 'SearchURLRequest':
         return super().__new__(
             cls,
             *args,
-            original_article_id=original_article_id,
+            ids=ids,
+            links=links,
             page=page,
             page_size=page_size,
             _configuration=_configuration,
             **kwargs,
         )
```

#### html2text {}

```diff
@@ -4,46 +4,51 @@
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
-newscatcherapi_client import schemas # noqa: F401 class
-DuplicatesByOriginalIdRequest( schemas.DictSchema ): """ This class is auto
-generated by Konfig (https://konfigthis.com) Duplicates by original article ID
-request DTO """ class MetaOapg: required = { "original_article_id", } class
-properties: original_article_id = schemas.StrSchema class page
+newscatcherapi_client import schemas # noqa: F401 class SearchURLRequest
+( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
+konfigthis.com) Search URL Request DTO. """ class MetaOapg: class properties:
+ids = schemas.AnyTypeSchema links = schemas.AnyTypeSchema class page
 ( schemas.IntSchema ): class MetaOapg: inclusive_minimum = 0 class page_size
 ( schemas.IntSchema ): class MetaOapg: inclusive_minimum = 0 __annotations__ =
-{ "original_article_id": original_article_id, "page": page, "page_size":
-page_size, } original_article_id: MetaOapg.properties.original_article_id
-@typing.overload def __getitem__(self, name: typing_extensions.Literal
-["original_article_id"]) -> MetaOapg.properties.original_article_id: ...
+{ "ids": ids, "links": links, "page": page, "page_size": page_size, }
+@typing.overload def __getitem__(self, name: typing_extensions.Literal["ids"])
+-> MetaOapg.properties.ids: ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["links"]) -> MetaOapg.properties.links: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal["page"])
 -> MetaOapg.properties.page: ... @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["page_size"]) -> MetaOapg.properties.page_size: ...
 @typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
-[typing_extensions.Literal["original_article_id", "page", "page_size", ],
-str]): # dict_instance[name] accessor return super().__getitem__(name)
-@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
-["original_article_id"]) -> MetaOapg.properties.original_article_id: ...
-@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
-["page"]) -> typing.Union[MetaOapg.properties.page, schemas.Unset]: ...
-@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
-["page_size"]) -> typing.Union[MetaOapg.properties.page_size, schemas.Unset]:
-... @typing.overload def get_item_oapg(self, name: str) -> typing.Union
+[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]): #
+dict_instance[name] accessor return super().__getitem__(name) @typing.overload
+def get_item_oapg(self, name: typing_extensions.Literal["ids"]) -> typing.Union
+[MetaOapg.properties.ids, schemas.Unset]: ... @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["links"]) -> typing.Union
+[MetaOapg.properties.links, schemas.Unset]: ... @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["page"]) -> typing.Union
+[MetaOapg.properties.page, schemas.Unset]: ... @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["page_size"]) -
+> typing.Union[MetaOapg.properties.page_size, schemas.Unset]: ...
+@typing.overload def get_item_oapg(self, name: str) -> typing.Union
 [schemas.UnsetAnyTypeSchema, schemas.Unset]: ... def get_item_oapg(self, name:
-typing.Union[typing_extensions.Literal["original_article_id", "page",
-"page_size", ], str]): return super().get_item_oapg(name) def __new__( cls,
-*args: typing.Union[dict, frozendict.frozendict, ], original_article_id:
-typing.Union[MetaOapg.properties.original_article_id, str, ], page:
-typing.Union[MetaOapg.properties.page, decimal.Decimal, int, schemas.Unset] =
-schemas.unset, page_size: typing.Union[MetaOapg.properties.page_size,
-decimal.Decimal, int, schemas.Unset] = schemas.unset, _configuration:
-typing.Optional[schemas.Configuration] = None, **kwargs: typing.Union
-[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime,
-uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes], ) -
-> 'DuplicatesByOriginalIdRequest': return super().__new__( cls, *args,
-original_article_id=original_article_id, page=page, page_size=page_size,
-_configuration=_configuration, **kwargs, )
+typing.Union[typing_extensions.Literal["ids", "links", "page", "page_size", ],
+str]): return super().get_item_oapg(name) def __new__( cls, *args: typing.Union
+[dict, frozendict.frozendict, ], ids: typing.Union[MetaOapg.properties.ids,
+dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
+schemas.Unset] = schemas.unset, links: typing.Union[MetaOapg.properties.links,
+dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
+schemas.Unset] = schemas.unset, page: typing.Union[MetaOapg.properties.page,
+decimal.Decimal, int, schemas.Unset] = schemas.unset, page_size: typing.Union
+[MetaOapg.properties.page_size, decimal.Decimal, int, schemas.Unset] =
+schemas.unset, _configuration: typing.Optional[schemas.Configuration] = None,
+**kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str,
+date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple,
+bytes], ) -> 'SearchURLRequest': return super().__new__( cls, *args, ids=ids,
+links=links, page=page, page_size=page_size, _configuration=_configuration,
+**kwargs, )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/duplicates_by_original_id_request.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_url_request.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -20,95 +20,100 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class DuplicatesByOriginalIdRequest(
+class SearchURLRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Duplicates by original article ID request DTO
+    Search URL Request DTO.
     """
 
 
     class MetaOapg:
-        required = {
-            "original_article_id",
-        }
         
         class properties:
-            original_article_id = schemas.StrSchema
+            ids = schemas.AnyTypeSchema
+            links = schemas.AnyTypeSchema
             
             
             class page(
                 schemas.IntSchema
             ):
                 pass
             
             
             class page_size(
                 schemas.IntSchema
             ):
                 pass
             __annotations__ = {
-                "original_article_id": original_article_id,
+                "ids": ids,
+                "links": links,
                 "page": page,
                 "page_size": page_size,
             }
     
-    original_article_id: MetaOapg.properties.original_article_id
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["ids"]) -> MetaOapg.properties.ids: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["original_article_id"]) -> MetaOapg.properties.original_article_id: ...
+    def __getitem__(self, name: typing_extensions.Literal["links"]) -> MetaOapg.properties.links: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["page_size"]) -> MetaOapg.properties.page_size: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["original_article_id", "page", "page_size", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["original_article_id"]) -> MetaOapg.properties.original_article_id: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["ids"]) -> typing.Union[MetaOapg.properties.ids, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["links"]) -> typing.Union[MetaOapg.properties.links, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["page"]) -> typing.Union[MetaOapg.properties.page, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["page_size"]) -> typing.Union[MetaOapg.properties.page_size, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["original_article_id", "page", "page_size", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        original_article_id: typing.Union[MetaOapg.properties.original_article_id, str, ],
+        ids: typing.Union[MetaOapg.properties.ids, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        links: typing.Union[MetaOapg.properties.links, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         page: typing.Union[MetaOapg.properties.page, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         page_size: typing.Union[MetaOapg.properties.page_size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DuplicatesByOriginalIdRequest':
+    ) -> 'SearchURLRequest':
         return super().__new__(
             cls,
             *args,
-            original_article_id=original_article_id,
+            ids=ids,
+            links=links,
             page=page,
             page_size=page_size,
             _configuration=_configuration,
             **kwargs,
         )
```

#### html2text {}

```diff
@@ -4,46 +4,51 @@
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
-newscatcherapi_client import schemas # noqa: F401 class
-DuplicatesByOriginalIdRequest( schemas.DictSchema ): """ This class is auto
-generated by Konfig (https://konfigthis.com) Duplicates by original article ID
-request DTO """ class MetaOapg: required = { "original_article_id", } class
-properties: original_article_id = schemas.StrSchema class page
+newscatcherapi_client import schemas # noqa: F401 class SearchURLRequest
+( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
+konfigthis.com) Search URL Request DTO. """ class MetaOapg: class properties:
+ids = schemas.AnyTypeSchema links = schemas.AnyTypeSchema class page
 ( schemas.IntSchema ): pass class page_size( schemas.IntSchema ): pass
-__annotations__ = { "original_article_id": original_article_id, "page": page,
-"page_size": page_size, } original_article_id:
-MetaOapg.properties.original_article_id @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["original_article_id"]) -
-> MetaOapg.properties.original_article_id: ... @typing.overload def __getitem__
+__annotations__ = { "ids": ids, "links": links, "page": page, "page_size":
+page_size, } @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["ids"]) -> MetaOapg.properties.ids: ...
+@typing.overload def __getitem__(self, name: typing_extensions.Literal
+["links"]) -> MetaOapg.properties.links: ... @typing.overload def __getitem__
 (self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page:
 ... @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["page_size"]) -> MetaOapg.properties.page_size: ... @typing.overload def
 __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__
-(self, name: typing.Union[typing_extensions.Literal["original_article_id",
-"page", "page_size", ], str]): # dict_instance[name] accessor return super
+(self, name: typing.Union[typing_extensions.Literal["ids", "links", "page",
+"page_size", ], str]): # dict_instance[name] accessor return super
 ().__getitem__(name) @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["original_article_id"]) -
-> MetaOapg.properties.original_article_id: ... @typing.overload def
-get_item_oapg(self, name: typing_extensions.Literal["page"]) -> typing.Union
-[MetaOapg.properties.page, schemas.Unset]: ... @typing.overload def
-get_item_oapg(self, name: typing_extensions.Literal["page_size"]) -
-> typing.Union[MetaOapg.properties.page_size, schemas.Unset]: ...
-@typing.overload def get_item_oapg(self, name: str) -> typing.Union
-[schemas.UnsetAnyTypeSchema, schemas.Unset]: ... def get_item_oapg(self, name:
-typing.Union[typing_extensions.Literal["original_article_id", "page",
-"page_size", ], str]): return super().get_item_oapg(name) def __new__( cls,
-*args: typing.Union[dict, frozendict.frozendict, ], original_article_id:
-typing.Union[MetaOapg.properties.original_article_id, str, ], page:
-typing.Union[MetaOapg.properties.page, decimal.Decimal, int, schemas.Unset] =
-schemas.unset, page_size: typing.Union[MetaOapg.properties.page_size,
-decimal.Decimal, int, schemas.Unset] = schemas.unset, _configuration:
-typing.Optional[schemas.Configuration] = None, **kwargs: typing.Union
-[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime,
-uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes], ) -
-> 'DuplicatesByOriginalIdRequest': return super().__new__( cls, *args,
-original_article_id=original_article_id, page=page, page_size=page_size,
-_configuration=_configuration, **kwargs, )
+typing_extensions.Literal["ids"]) -> typing.Union[MetaOapg.properties.ids,
+schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["links"]) -> typing.Union[MetaOapg.properties.links,
+schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["page"]) -> typing.Union[MetaOapg.properties.page,
+schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["page_size"]) -> typing.Union
+[MetaOapg.properties.page_size, schemas.Unset]: ... @typing.overload def
+get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema,
+schemas.Unset]: ... def get_item_oapg(self, name: typing.Union
+[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]):
+return super().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
+frozendict.frozendict, ], ids: typing.Union[MetaOapg.properties.ids, dict,
+frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
+schemas.Unset] = schemas.unset, links: typing.Union[MetaOapg.properties.links,
+dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
+schemas.Unset] = schemas.unset, page: typing.Union[MetaOapg.properties.page,
+decimal.Decimal, int, schemas.Unset] = schemas.unset, page_size: typing.Union
+[MetaOapg.properties.page_size, decimal.Decimal, int, schemas.Unset] =
+schemas.unset, _configuration: typing.Optional[schemas.Configuration] = None,
+**kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str,
+date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple,
+bytes], ) -> 'SearchURLRequest': return super().__new__( cls, *args, ids=ids,
+links=links, page=page, page_size=page_size, _configuration=_configuration,
+**kwargs, )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/http_validation_error.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_get_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_post_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_request.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/latest_headlines_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/more_like_this_request.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/more_like_this_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_get_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_post_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_request.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_get_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_similar_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_post_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/search_similar_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_url_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_info.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,106 +20,100 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class SearchURLRequest(
+class SourceInfo(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Search URL Request DTO.
+    "SourceInfo DTO class.
     """
 
 
     class MetaOapg:
+        required = {
+            "domain_url",
+        }
         
         class properties:
-            ids = schemas.AnyTypeSchema
-            links = schemas.AnyTypeSchema
-            
-            
-            class page(
-                schemas.IntSchema
-            ):
-            
-            
-                class MetaOapg:
-                    inclusive_minimum = 0
-            
-            
-            class page_size(
-                schemas.IntSchema
-            ):
-            
-            
-                class MetaOapg:
-                    inclusive_minimum = 0
+            domain_url = schemas.StrSchema
+            name_source = schemas.StrSchema
+            logo = schemas.StrSchema
+        
+            @staticmethod
+            def additional_info() -> typing.Type['AdditionalSourceInfo']:
+                return AdditionalSourceInfo
             __annotations__ = {
-                "ids": ids,
-                "links": links,
-                "page": page,
-                "page_size": page_size,
+                "domain_url": domain_url,
+                "name_source": name_source,
+                "logo": logo,
+                "additional_info": additional_info,
             }
     
+    domain_url: MetaOapg.properties.domain_url
+    
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["ids"]) -> MetaOapg.properties.ids: ...
+    def __getitem__(self, name: typing_extensions.Literal["domain_url"]) -> MetaOapg.properties.domain_url: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["links"]) -> MetaOapg.properties.links: ...
+    def __getitem__(self, name: typing_extensions.Literal["name_source"]) -> MetaOapg.properties.name_source: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
+    def __getitem__(self, name: typing_extensions.Literal["logo"]) -> MetaOapg.properties.logo: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["page_size"]) -> MetaOapg.properties.page_size: ...
+    def __getitem__(self, name: typing_extensions.Literal["additional_info"]) -> 'AdditionalSourceInfo': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["domain_url", "name_source", "logo", "additional_info", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["ids"]) -> typing.Union[MetaOapg.properties.ids, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["domain_url"]) -> MetaOapg.properties.domain_url: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["links"]) -> typing.Union[MetaOapg.properties.links, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name_source"]) -> typing.Union[MetaOapg.properties.name_source, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["page"]) -> typing.Union[MetaOapg.properties.page, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["logo"]) -> typing.Union[MetaOapg.properties.logo, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["page_size"]) -> typing.Union[MetaOapg.properties.page_size, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["additional_info"]) -> typing.Union['AdditionalSourceInfo', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["domain_url", "name_source", "logo", "additional_info", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        ids: typing.Union[MetaOapg.properties.ids, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        links: typing.Union[MetaOapg.properties.links, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        page: typing.Union[MetaOapg.properties.page, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        page_size: typing.Union[MetaOapg.properties.page_size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        domain_url: typing.Union[MetaOapg.properties.domain_url, str, ],
+        name_source: typing.Union[MetaOapg.properties.name_source, str, schemas.Unset] = schemas.unset,
+        logo: typing.Union[MetaOapg.properties.logo, str, schemas.Unset] = schemas.unset,
+        additional_info: typing.Union['AdditionalSourceInfo', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SearchURLRequest':
+    ) -> 'SourceInfo':
         return super().__new__(
             cls,
             *args,
-            ids=ids,
-            links=links,
-            page=page,
-            page_size=page_size,
+            domain_url=domain_url,
+            name_source=name_source,
+            logo=logo,
+            additional_info=additional_info,
             _configuration=_configuration,
             **kwargs,
         )
+
+from newscatcherapi_client.model.additional_source_info import AdditionalSourceInfo
```

#### html2text {}

```diff
@@ -4,51 +4,52 @@
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
-newscatcherapi_client import schemas # noqa: F401 class SearchURLRequest
+newscatcherapi_client import schemas # noqa: F401 class SourceInfo
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) Search URL Request DTO. """ class MetaOapg: class properties:
-ids = schemas.AnyTypeSchema links = schemas.AnyTypeSchema class page
-( schemas.IntSchema ): class MetaOapg: inclusive_minimum = 0 class page_size
-( schemas.IntSchema ): class MetaOapg: inclusive_minimum = 0 __annotations__ =
-{ "ids": ids, "links": links, "page": page, "page_size": page_size, }
-@typing.overload def __getitem__(self, name: typing_extensions.Literal["ids"])
--> MetaOapg.properties.ids: ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["links"]) -> MetaOapg.properties.links: ...
-@typing.overload def __getitem__(self, name: typing_extensions.Literal["page"])
--> MetaOapg.properties.page: ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["page_size"]) -> MetaOapg.properties.page_size: ...
+konfigthis.com) "SourceInfo DTO class. """ class MetaOapg: required =
+{ "domain_url", } class properties: domain_url = schemas.StrSchema name_source
+= schemas.StrSchema logo = schemas.StrSchema @staticmethod def additional_info
+() -> typing.Type['AdditionalSourceInfo']: return AdditionalSourceInfo
+__annotations__ = { "domain_url": domain_url, "name_source": name_source,
+"logo": logo, "additional_info": additional_info, } domain_url:
+MetaOapg.properties.domain_url @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["domain_url"]) -> MetaOapg.properties.domain_url: ...
+@typing.overload def __getitem__(self, name: typing_extensions.Literal
+["name_source"]) -> MetaOapg.properties.name_source: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["logo"]) -
+> MetaOapg.properties.logo: ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["additional_info"]) -> 'AdditionalSourceInfo': ...
 @typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
-[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]): #
-dict_instance[name] accessor return super().__getitem__(name) @typing.overload
-def get_item_oapg(self, name: typing_extensions.Literal["ids"]) -> typing.Union
-[MetaOapg.properties.ids, schemas.Unset]: ... @typing.overload def
-get_item_oapg(self, name: typing_extensions.Literal["links"]) -> typing.Union
-[MetaOapg.properties.links, schemas.Unset]: ... @typing.overload def
-get_item_oapg(self, name: typing_extensions.Literal["page"]) -> typing.Union
-[MetaOapg.properties.page, schemas.Unset]: ... @typing.overload def
-get_item_oapg(self, name: typing_extensions.Literal["page_size"]) -
-> typing.Union[MetaOapg.properties.page_size, schemas.Unset]: ...
-@typing.overload def get_item_oapg(self, name: str) -> typing.Union
-[schemas.UnsetAnyTypeSchema, schemas.Unset]: ... def get_item_oapg(self, name:
-typing.Union[typing_extensions.Literal["ids", "links", "page", "page_size", ],
-str]): return super().get_item_oapg(name) def __new__( cls, *args: typing.Union
-[dict, frozendict.frozendict, ], ids: typing.Union[MetaOapg.properties.ids,
-dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
-decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
-schemas.Unset] = schemas.unset, links: typing.Union[MetaOapg.properties.links,
-dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
-decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
-schemas.Unset] = schemas.unset, page: typing.Union[MetaOapg.properties.page,
-decimal.Decimal, int, schemas.Unset] = schemas.unset, page_size: typing.Union
-[MetaOapg.properties.page_size, decimal.Decimal, int, schemas.Unset] =
+[typing_extensions.Literal["domain_url", "name_source", "logo",
+"additional_info", ], str]): # dict_instance[name] accessor return super
+().__getitem__(name) @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["domain_url"]) -> MetaOapg.properties.domain_url: ...
+@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
+["name_source"]) -> typing.Union[MetaOapg.properties.name_source,
+schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["logo"]) -> typing.Union[MetaOapg.properties.logo,
+schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["additional_info"]) -> typing.Union
+['AdditionalSourceInfo', schemas.Unset]: ... @typing.overload def get_item_oapg
+(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+... def get_item_oapg(self, name: typing.Union[typing_extensions.Literal
+["domain_url", "name_source", "logo", "additional_info", ], str]): return super
+().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
+frozendict.frozendict, ], domain_url: typing.Union
+[MetaOapg.properties.domain_url, str, ], name_source: typing.Union
+[MetaOapg.properties.name_source, str, schemas.Unset] = schemas.unset, logo:
+typing.Union[MetaOapg.properties.logo, str, schemas.Unset] = schemas.unset,
+additional_info: typing.Union['AdditionalSourceInfo', schemas.Unset] =
 schemas.unset, _configuration: typing.Optional[schemas.Configuration] = None,
 **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str,
 date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple,
-bytes], ) -> 'SearchURLRequest': return super().__new__( cls, *args, ids=ids,
-links=links, page=page, page_size=page_size, _configuration=_configuration,
-**kwargs, )
+bytes], ) -> 'SourceInfo': return super().__new__( cls, *args,
+domain_url=domain_url, name_source=name_source, logo=logo,
+additional_info=additional_info, _configuration=_configuration, **kwargs, )
+from newscatcherapi_client.model.additional_source_info import
+AdditionalSourceInfo
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_url_request.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,100 +20,94 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class SearchURLRequest(
+class SourceResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Search URL Request DTO.
+    SourceResponse DTO class.
     """
 
 
     class MetaOapg:
+        required = {
+            "sources",
+            "user_input",
+            "message",
+        }
         
         class properties:
-            ids = schemas.AnyTypeSchema
-            links = schemas.AnyTypeSchema
-            
-            
-            class page(
-                schemas.IntSchema
-            ):
-                pass
-            
-            
-            class page_size(
-                schemas.IntSchema
-            ):
-                pass
+            message = schemas.StrSchema
+        
+            @staticmethod
+            def sources() -> typing.Type['SourceResponseSources']:
+                return SourceResponseSources
+            user_input = schemas.DictSchema
             __annotations__ = {
-                "ids": ids,
-                "links": links,
-                "page": page,
-                "page_size": page_size,
+                "message": message,
+                "sources": sources,
+                "user_input": user_input,
             }
     
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["ids"]) -> MetaOapg.properties.ids: ...
+    sources: 'SourceResponseSources'
+    user_input: MetaOapg.properties.user_input
+    message: MetaOapg.properties.message
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["links"]) -> MetaOapg.properties.links: ...
+    def __getitem__(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
+    def __getitem__(self, name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["page_size"]) -> MetaOapg.properties.page_size: ...
+    def __getitem__(self, name: typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["message", "sources", "user_input", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["ids"]) -> typing.Union[MetaOapg.properties.ids, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["links"]) -> typing.Union[MetaOapg.properties.links, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["page"]) -> typing.Union[MetaOapg.properties.page, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["page_size"]) -> typing.Union[MetaOapg.properties.page_size, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["message", "sources", "user_input", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        ids: typing.Union[MetaOapg.properties.ids, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        links: typing.Union[MetaOapg.properties.links, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        page: typing.Union[MetaOapg.properties.page, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        page_size: typing.Union[MetaOapg.properties.page_size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        sources: 'SourceResponseSources',
+        user_input: typing.Union[MetaOapg.properties.user_input, dict, frozendict.frozendict, ],
+        message: typing.Union[MetaOapg.properties.message, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SearchURLRequest':
+    ) -> 'SourceResponse':
         return super().__new__(
             cls,
             *args,
-            ids=ids,
-            links=links,
-            page=page,
-            page_size=page_size,
+            sources=sources,
+            user_input=user_input,
+            message=message,
             _configuration=_configuration,
             **kwargs,
         )
+
+from newscatcherapi_client.model.source_response_sources import SourceResponseSources
```

#### html2text {}

```diff
@@ -4,51 +4,44 @@
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
-newscatcherapi_client import schemas # noqa: F401 class SearchURLRequest
+newscatcherapi_client import schemas # noqa: F401 class SourceResponse
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) Search URL Request DTO. """ class MetaOapg: class properties:
-ids = schemas.AnyTypeSchema links = schemas.AnyTypeSchema class page
-( schemas.IntSchema ): pass class page_size( schemas.IntSchema ): pass
-__annotations__ = { "ids": ids, "links": links, "page": page, "page_size":
-page_size, } @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["ids"]) -> MetaOapg.properties.ids: ...
+konfigthis.com) SourceResponse DTO class. """ class MetaOapg: required =
+{ "sources", "user_input", "message", } class properties: message =
+schemas.StrSchema @staticmethod def sources() -> typing.Type
+['SourceResponseSources']: return SourceResponseSources user_input =
+schemas.DictSchema __annotations__ = { "message": message, "sources": sources,
+"user_input": user_input, } sources: 'SourceResponseSources' user_input:
+MetaOapg.properties.user_input message: MetaOapg.properties.message
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["links"]) -> MetaOapg.properties.links: ... @typing.overload def __getitem__
-(self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page:
-... @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["page_size"]) -> MetaOapg.properties.page_size: ... @typing.overload def
-__getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__
-(self, name: typing.Union[typing_extensions.Literal["ids", "links", "page",
-"page_size", ], str]): # dict_instance[name] accessor return super
-().__getitem__(name) @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["ids"]) -> typing.Union[MetaOapg.properties.ids,
-schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["links"]) -> typing.Union[MetaOapg.properties.links,
-schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["page"]) -> typing.Union[MetaOapg.properties.page,
-schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["page_size"]) -> typing.Union
-[MetaOapg.properties.page_size, schemas.Unset]: ... @typing.overload def
+["message"]) -> MetaOapg.properties.message: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["sources"]) -
+> 'SourceResponseSources': ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
+@typing.overload def __getitem__(self, name: str) -
+> schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
+[typing_extensions.Literal["message", "sources", "user_input", ], str]): #
+dict_instance[name] accessor return super().__getitem__(name) @typing.overload
+def get_item_oapg(self, name: typing_extensions.Literal["message"]) -
+> MetaOapg.properties.message: ... @typing.overload def get_item_oapg(self,
+name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
+@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
+["user_input"]) -> MetaOapg.properties.user_input: ... @typing.overload def
 get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema,
 schemas.Unset]: ... def get_item_oapg(self, name: typing.Union
-[typing_extensions.Literal["ids", "links", "page", "page_size", ], str]):
-return super().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
-frozendict.frozendict, ], ids: typing.Union[MetaOapg.properties.ids, dict,
-frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
-decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
-schemas.Unset] = schemas.unset, links: typing.Union[MetaOapg.properties.links,
-dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
-decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
-schemas.Unset] = schemas.unset, page: typing.Union[MetaOapg.properties.page,
-decimal.Decimal, int, schemas.Unset] = schemas.unset, page_size: typing.Union
-[MetaOapg.properties.page_size, decimal.Decimal, int, schemas.Unset] =
-schemas.unset, _configuration: typing.Optional[schemas.Configuration] = None,
-**kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str,
-date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple,
-bytes], ) -> 'SearchURLRequest': return super().__new__( cls, *args, ids=ids,
-links=links, page=page, page_size=page_size, _configuration=_configuration,
-**kwargs, )
+[typing_extensions.Literal["message", "sources", "user_input", ], str]): return
+super().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
+frozendict.frozendict, ], sources: 'SourceResponseSources', user_input:
+typing.Union[MetaOapg.properties.user_input, dict, frozendict.frozendict, ],
+message: typing.Union[MetaOapg.properties.message, str, ], _configuration:
+typing.Optional[schemas.Configuration] = None, **kwargs: typing.Union
+[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime,
+uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes], ) -
+> 'SourceResponse': return super().__new__( cls, *args, sources=sources,
+user_input=user_input, message=message, _configuration=_configuration,
+**kwargs, ) from newscatcherapi_client.model.source_response_sources import
+SourceResponseSources
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_response_sources.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,48 +20,70 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class SearchduplicatesbyoriginalidGetResponse(
-    schemas.ComposedSchema,
+class SourceResponseSources(
+    schemas.ListSchema
 ):
-    """
+    """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
-        @classmethod
-        @functools.lru_cache()
-        def any_of(cls):
-            # we need this here to make our import statements work
-            # we must store _composed_schemas in here so the code is only run
-            # when we invoke this method. If we kept this at the class
-            # level we would get an error because the class level
-            # code would be run when this module is imported, and these composed
-            # classes don't exist yet because their module has not finished
-            # loading
-            return [
-                DtoResponsesSearchResponseSearchResponse,
-                ClusteringSearchResponse,
-            ]
-
+        
+        class items(
+            schemas.ComposedSchema,
+        ):
+        
+        
+            class MetaOapg:
+                any_of_1 = schemas.StrSchema
+                
+                @classmethod
+                @functools.lru_cache()
+                def any_of(cls):
+                    # we need this here to make our import statements work
+                    # we must store _composed_schemas in here so the code is only run
+                    # when we invoke this method. If we kept this at the class
+                    # level we would get an error because the class level
+                    # code would be run when this module is imported, and these composed
+                    # classes don't exist yet because their module has not finished
+                    # loading
+                    return [
+                        SourceInfo,
+                        cls.any_of_1,
+                    ]
+        
+        
+            def __new__(
+                cls,
+                *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                _configuration: typing.Optional[schemas.Configuration] = None,
+                **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+            ) -> 'items':
+                return super().__new__(
+                    cls,
+                    *args,
+                    _configuration=_configuration,
+                    **kwargs,
+                )
 
     def __new__(
         cls,
-        *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ]], typing.List[typing.Union[MetaOapg.items, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ]]],
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SearchduplicatesbyoriginalidGetResponse':
+    ) -> 'SourceResponseSources':
         return super().__new__(
             cls,
-            *args,
+            arg,
             _configuration=_configuration,
-            **kwargs,
         )
 
-from newscatcherapi_client.model.clustering_search_response import ClusteringSearchResponse
-from newscatcherapi_client.model.dto_responses_search_response_search_response import DtoResponsesSearchResponseSearchResponse
+    def __getitem__(self, i: int) -> MetaOapg.items:
+        return super().__getitem__(i)
+
+from newscatcherapi_client.model.source_info import SourceInfo
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_get_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_response_sources.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -20,48 +20,70 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class SearchduplicatesbyoriginalidGetResponse(
-    schemas.ComposedSchema,
+class SourceResponseSources(
+    schemas.ListSchema
 ):
-    """
+    """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
-        @classmethod
-        @functools.lru_cache()
-        def any_of(cls):
-            # we need this here to make our import statements work
-            # we must store _composed_schemas in here so the code is only run
-            # when we invoke this method. If we kept this at the class
-            # level we would get an error because the class level
-            # code would be run when this module is imported, and these composed
-            # classes don't exist yet because their module has not finished
-            # loading
-            return [
-                DtoResponsesSearchResponseSearchResponse,
-                ClusteringSearchResponse,
-            ]
-
+        
+        class items(
+            schemas.ComposedSchema,
+        ):
+        
+        
+            class MetaOapg:
+                any_of_1 = schemas.StrSchema
+                
+                @classmethod
+                @functools.lru_cache()
+                def any_of(cls):
+                    # we need this here to make our import statements work
+                    # we must store _composed_schemas in here so the code is only run
+                    # when we invoke this method. If we kept this at the class
+                    # level we would get an error because the class level
+                    # code would be run when this module is imported, and these composed
+                    # classes don't exist yet because their module has not finished
+                    # loading
+                    return [
+                        SourceInfo,
+                        cls.any_of_1,
+                    ]
+        
+        
+            def __new__(
+                cls,
+                *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                _configuration: typing.Optional[schemas.Configuration] = None,
+                **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+            ) -> 'items':
+                return super().__new__(
+                    cls,
+                    *args,
+                    _configuration=_configuration,
+                    **kwargs,
+                )
 
     def __new__(
         cls,
-        *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ]], typing.List[typing.Union[MetaOapg.items, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ]]],
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SearchduplicatesbyoriginalidGetResponse':
+    ) -> 'SourceResponseSources':
         return super().__new__(
             cls,
-            *args,
+            arg,
             _configuration=_configuration,
-            **kwargs,
         )
 
-from newscatcherapi_client.model.clustering_search_response import ClusteringSearchResponse
-from newscatcherapi_client.model.dto_responses_search_response_search_response import DtoResponsesSearchResponseSearchResponse
+    def __getitem__(self, i: int) -> MetaOapg.items:
+        return super().__getitem__(i)
+
+from newscatcherapi_client.model.source_info import SourceInfo
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/validation_error_loc.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,48 +20,69 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class SearchduplicatesbyoriginalidPostResponse(
-    schemas.ComposedSchema,
+class ValidationErrorLoc(
+    schemas.ListSchema
 ):
-    """
+    """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
-        @classmethod
-        @functools.lru_cache()
-        def any_of(cls):
-            # we need this here to make our import statements work
-            # we must store _composed_schemas in here so the code is only run
-            # when we invoke this method. If we kept this at the class
-            # level we would get an error because the class level
-            # code would be run when this module is imported, and these composed
-            # classes don't exist yet because their module has not finished
-            # loading
-            return [
-                DtoResponsesSearchResponseSearchResponse,
-                ClusteringSearchResponse,
-            ]
-
+        
+        class items(
+            schemas.ComposedSchema,
+        ):
+        
+        
+            class MetaOapg:
+                items = schemas.StrSchema
+                any_of_1 = schemas.IntSchema
+                
+                @classmethod
+                @functools.lru_cache()
+                def any_of(cls):
+                    # we need this here to make our import statements work
+                    # we must store _composed_schemas in here so the code is only run
+                    # when we invoke this method. If we kept this at the class
+                    # level we would get an error because the class level
+                    # code would be run when this module is imported, and these composed
+                    # classes don't exist yet because their module has not finished
+                    # loading
+                    return [
+                        cls.items,
+                        cls.any_of_1,
+                    ]
+        
+        
+            def __new__(
+                cls,
+                *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                _configuration: typing.Optional[schemas.Configuration] = None,
+                **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+            ) -> 'items':
+                return super().__new__(
+                    cls,
+                    *args,
+                    _configuration=_configuration,
+                    **kwargs,
+                )
 
     def __new__(
         cls,
-        *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ]], typing.List[typing.Union[MetaOapg.items, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ]]],
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SearchduplicatesbyoriginalidPostResponse':
+    ) -> 'ValidationErrorLoc':
         return super().__new__(
             cls,
-            *args,
+            arg,
             _configuration=_configuration,
-            **kwargs,
         )
 
-from newscatcherapi_client.model.clustering_search_response import ClusteringSearchResponse
-from newscatcherapi_client.model.dto_responses_search_response_search_response import DtoResponsesSearchResponseSearchResponse
+    def __getitem__(self, i: int) -> MetaOapg.items:
+        return super().__getitem__(i)
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_post_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/validation_error_loc.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -20,48 +20,69 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class SearchduplicatesbyoriginalidPostResponse(
-    schemas.ComposedSchema,
+class ValidationErrorLoc(
+    schemas.ListSchema
 ):
-    """
+    """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
-        @classmethod
-        @functools.lru_cache()
-        def any_of(cls):
-            # we need this here to make our import statements work
-            # we must store _composed_schemas in here so the code is only run
-            # when we invoke this method. If we kept this at the class
-            # level we would get an error because the class level
-            # code would be run when this module is imported, and these composed
-            # classes don't exist yet because their module has not finished
-            # loading
-            return [
-                DtoResponsesSearchResponseSearchResponse,
-                ClusteringSearchResponse,
-            ]
-
+        
+        class items(
+            schemas.ComposedSchema,
+        ):
+        
+        
+            class MetaOapg:
+                items = schemas.StrSchema
+                any_of_1 = schemas.IntSchema
+                
+                @classmethod
+                @functools.lru_cache()
+                def any_of(cls):
+                    # we need this here to make our import statements work
+                    # we must store _composed_schemas in here so the code is only run
+                    # when we invoke this method. If we kept this at the class
+                    # level we would get an error because the class level
+                    # code would be run when this module is imported, and these composed
+                    # classes don't exist yet because their module has not finished
+                    # loading
+                    return [
+                        cls.items,
+                        cls.any_of_1,
+                    ]
+        
+        
+            def __new__(
+                cls,
+                *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                _configuration: typing.Optional[schemas.Configuration] = None,
+                **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+            ) -> 'items':
+                return super().__new__(
+                    cls,
+                    *args,
+                    _configuration=_configuration,
+                    **kwargs,
+                )
 
     def __new__(
         cls,
-        *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ]], typing.List[typing.Union[MetaOapg.items, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ]]],
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SearchduplicatesbyoriginalidPostResponse':
+    ) -> 'ValidationErrorLoc':
         return super().__new__(
             cls,
-            *args,
+            arg,
             _configuration=_configuration,
-            **kwargs,
         )
 
-from newscatcherapi_client.model.clustering_search_response import ClusteringSearchResponse
-from newscatcherapi_client.model.dto_responses_search_response_search_response import DtoResponsesSearchResponseSearchResponse
+    def __getitem__(self, i: int) -> MetaOapg.items:
+        return super().__getitem__(i)
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/similar_document.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/similar_document.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/similar_document.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/similar_document.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_info.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_info.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_info.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/source_response.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -20,100 +20,94 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class SourceInfo(
+class SourceResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    "SourceInfo DTO class.
+    SourceResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
-            "domain_url",
+            "sources",
+            "user_input",
+            "message",
         }
         
         class properties:
-            domain_url = schemas.StrSchema
-            name_source = schemas.StrSchema
-            logo = schemas.StrSchema
+            message = schemas.StrSchema
         
             @staticmethod
-            def additional_info() -> typing.Type['AdditionalSourceInfo']:
-                return AdditionalSourceInfo
+            def sources() -> typing.Type['SourceResponseSources']:
+                return SourceResponseSources
+            user_input = schemas.DictSchema
             __annotations__ = {
-                "domain_url": domain_url,
-                "name_source": name_source,
-                "logo": logo,
-                "additional_info": additional_info,
+                "message": message,
+                "sources": sources,
+                "user_input": user_input,
             }
     
-    domain_url: MetaOapg.properties.domain_url
+    sources: 'SourceResponseSources'
+    user_input: MetaOapg.properties.user_input
+    message: MetaOapg.properties.message
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["domain_url"]) -> MetaOapg.properties.domain_url: ...
+    def __getitem__(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name_source"]) -> MetaOapg.properties.name_source: ...
+    def __getitem__(self, name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["logo"]) -> MetaOapg.properties.logo: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["additional_info"]) -> 'AdditionalSourceInfo': ...
+    def __getitem__(self, name: typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["domain_url", "name_source", "logo", "additional_info", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["message", "sources", "user_input", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["domain_url"]) -> MetaOapg.properties.domain_url: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name_source"]) -> typing.Union[MetaOapg.properties.name_source, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["logo"]) -> typing.Union[MetaOapg.properties.logo, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["additional_info"]) -> typing.Union['AdditionalSourceInfo', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["domain_url", "name_source", "logo", "additional_info", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["message", "sources", "user_input", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        domain_url: typing.Union[MetaOapg.properties.domain_url, str, ],
-        name_source: typing.Union[MetaOapg.properties.name_source, str, schemas.Unset] = schemas.unset,
-        logo: typing.Union[MetaOapg.properties.logo, str, schemas.Unset] = schemas.unset,
-        additional_info: typing.Union['AdditionalSourceInfo', schemas.Unset] = schemas.unset,
+        sources: 'SourceResponseSources',
+        user_input: typing.Union[MetaOapg.properties.user_input, dict, frozendict.frozendict, ],
+        message: typing.Union[MetaOapg.properties.message, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SourceInfo':
+    ) -> 'SourceResponse':
         return super().__new__(
             cls,
             *args,
-            domain_url=domain_url,
-            name_source=name_source,
-            logo=logo,
-            additional_info=additional_info,
+            sources=sources,
+            user_input=user_input,
+            message=message,
             _configuration=_configuration,
             **kwargs,
         )
 
-from newscatcherapi_client.model.additional_source_info import AdditionalSourceInfo
+from newscatcherapi_client.model.source_response_sources import SourceResponseSources
```

#### html2text {}

```diff
@@ -4,52 +4,44 @@
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
-newscatcherapi_client import schemas # noqa: F401 class SourceInfo
+newscatcherapi_client import schemas # noqa: F401 class SourceResponse
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) "SourceInfo DTO class. """ class MetaOapg: required =
-{ "domain_url", } class properties: domain_url = schemas.StrSchema name_source
-= schemas.StrSchema logo = schemas.StrSchema @staticmethod def additional_info
-() -> typing.Type['AdditionalSourceInfo']: return AdditionalSourceInfo
-__annotations__ = { "domain_url": domain_url, "name_source": name_source,
-"logo": logo, "additional_info": additional_info, } domain_url:
-MetaOapg.properties.domain_url @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["domain_url"]) -> MetaOapg.properties.domain_url: ...
+konfigthis.com) SourceResponse DTO class. """ class MetaOapg: required =
+{ "sources", "user_input", "message", } class properties: message =
+schemas.StrSchema @staticmethod def sources() -> typing.Type
+['SourceResponseSources']: return SourceResponseSources user_input =
+schemas.DictSchema __annotations__ = { "message": message, "sources": sources,
+"user_input": user_input, } sources: 'SourceResponseSources' user_input:
+MetaOapg.properties.user_input message: MetaOapg.properties.message
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["name_source"]) -> MetaOapg.properties.name_source: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["logo"]) -
-> MetaOapg.properties.logo: ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["additional_info"]) -> 'AdditionalSourceInfo': ...
+["message"]) -> MetaOapg.properties.message: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["sources"]) -
+> 'SourceResponseSources': ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
 @typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
-[typing_extensions.Literal["domain_url", "name_source", "logo",
-"additional_info", ], str]): # dict_instance[name] accessor return super
-().__getitem__(name) @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["domain_url"]) -> MetaOapg.properties.domain_url: ...
+[typing_extensions.Literal["message", "sources", "user_input", ], str]): #
+dict_instance[name] accessor return super().__getitem__(name) @typing.overload
+def get_item_oapg(self, name: typing_extensions.Literal["message"]) -
+> MetaOapg.properties.message: ... @typing.overload def get_item_oapg(self,
+name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
-["name_source"]) -> typing.Union[MetaOapg.properties.name_source,
-schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["logo"]) -> typing.Union[MetaOapg.properties.logo,
-schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["additional_info"]) -> typing.Union
-['AdditionalSourceInfo', schemas.Unset]: ... @typing.overload def get_item_oapg
-(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
-... def get_item_oapg(self, name: typing.Union[typing_extensions.Literal
-["domain_url", "name_source", "logo", "additional_info", ], str]): return super
-().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
-frozendict.frozendict, ], domain_url: typing.Union
-[MetaOapg.properties.domain_url, str, ], name_source: typing.Union
-[MetaOapg.properties.name_source, str, schemas.Unset] = schemas.unset, logo:
-typing.Union[MetaOapg.properties.logo, str, schemas.Unset] = schemas.unset,
-additional_info: typing.Union['AdditionalSourceInfo', schemas.Unset] =
-schemas.unset, _configuration: typing.Optional[schemas.Configuration] = None,
-**kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str,
-date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple,
-bytes], ) -> 'SourceInfo': return super().__new__( cls, *args,
-domain_url=domain_url, name_source=name_source, logo=logo,
-additional_info=additional_info, _configuration=_configuration, **kwargs, )
-from newscatcherapi_client.model.additional_source_info import
-AdditionalSourceInfo
+["user_input"]) -> MetaOapg.properties.user_input: ... @typing.overload def
+get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema,
+schemas.Unset]: ... def get_item_oapg(self, name: typing.Union
+[typing_extensions.Literal["message", "sources", "user_input", ], str]): return
+super().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
+frozendict.frozendict, ], sources: 'SourceResponseSources', user_input:
+typing.Union[MetaOapg.properties.user_input, dict, frozendict.frozendict, ],
+message: typing.Union[MetaOapg.properties.message, str, ], _configuration:
+typing.Optional[schemas.Configuration] = None, **kwargs: typing.Union
+[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime,
+uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes], ) -
+> 'SourceResponse': return super().__new__( cls, *args, sources=sources,
+user_input=user_input, message=message, _configuration=_configuration,
+**kwargs, ) from newscatcherapi_client.model.source_response_sources import
+SourceResponseSources
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/validation_error.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,94 +20,92 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class SourceResponse(
+class ValidationError(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
-
-    SourceResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
-            "sources",
-            "user_input",
-            "message",
+            "msg",
+            "loc",
+            "type",
         }
         
         class properties:
-            message = schemas.StrSchema
         
             @staticmethod
-            def sources() -> typing.Type['SourceResponseSources']:
-                return SourceResponseSources
-            user_input = schemas.DictSchema
+            def loc() -> typing.Type['ValidationErrorLoc']:
+                return ValidationErrorLoc
+            msg = schemas.StrSchema
+            type = schemas.StrSchema
             __annotations__ = {
-                "message": message,
-                "sources": sources,
-                "user_input": user_input,
+                "loc": loc,
+                "msg": msg,
+                "type": type,
             }
     
-    sources: 'SourceResponseSources'
-    user_input: MetaOapg.properties.user_input
-    message: MetaOapg.properties.message
+    msg: MetaOapg.properties.msg
+    loc: 'ValidationErrorLoc'
+    type: MetaOapg.properties.type
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
+    def __getitem__(self, name: typing_extensions.Literal["loc"]) -> 'ValidationErrorLoc': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
+    def __getitem__(self, name: typing_extensions.Literal["msg"]) -> MetaOapg.properties.msg: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
+    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["message", "sources", "user_input", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["loc", "msg", "type", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["loc"]) -> 'ValidationErrorLoc': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
+    def get_item_oapg(self, name: typing_extensions.Literal["msg"]) -> MetaOapg.properties.msg: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["message", "sources", "user_input", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["loc", "msg", "type", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        sources: 'SourceResponseSources',
-        user_input: typing.Union[MetaOapg.properties.user_input, dict, frozendict.frozendict, ],
-        message: typing.Union[MetaOapg.properties.message, str, ],
+        msg: typing.Union[MetaOapg.properties.msg, str, ],
+        loc: 'ValidationErrorLoc',
+        type: typing.Union[MetaOapg.properties.type, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SourceResponse':
+    ) -> 'ValidationError':
         return super().__new__(
             cls,
             *args,
-            sources=sources,
-            user_input=user_input,
-            message=message,
+            msg=msg,
+            loc=loc,
+            type=type,
             _configuration=_configuration,
             **kwargs,
         )
 
-from newscatcherapi_client.model.source_response_sources import SourceResponseSources
+from newscatcherapi_client.model.validation_error_loc import ValidationErrorLoc
```

#### html2text {}

```diff
@@ -4,44 +4,40 @@
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
-newscatcherapi_client import schemas # noqa: F401 class SourceResponse
+newscatcherapi_client import schemas # noqa: F401 class ValidationError
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) SourceResponse DTO class. """ class MetaOapg: required =
-{ "sources", "user_input", "message", } class properties: message =
-schemas.StrSchema @staticmethod def sources() -> typing.Type
-['SourceResponseSources']: return SourceResponseSources user_input =
-schemas.DictSchema __annotations__ = { "message": message, "sources": sources,
-"user_input": user_input, } sources: 'SourceResponseSources' user_input:
-MetaOapg.properties.user_input message: MetaOapg.properties.message
-@typing.overload def __getitem__(self, name: typing_extensions.Literal
-["message"]) -> MetaOapg.properties.message: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["sources"]) -
-> 'SourceResponseSources': ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
+konfigthis.com) """ class MetaOapg: required = { "msg", "loc", "type", } class
+properties: @staticmethod def loc() -> typing.Type['ValidationErrorLoc']:
+return ValidationErrorLoc msg = schemas.StrSchema type = schemas.StrSchema
+__annotations__ = { "loc": loc, "msg": msg, "type": type, } msg:
+MetaOapg.properties.msg loc: 'ValidationErrorLoc' type:
+MetaOapg.properties.type @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["loc"]) -> 'ValidationErrorLoc': ... @typing.overload
+def __getitem__(self, name: typing_extensions.Literal["msg"]) -
+> MetaOapg.properties.msg: ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
 @typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
-[typing_extensions.Literal["message", "sources", "user_input", ], str]): #
-dict_instance[name] accessor return super().__getitem__(name) @typing.overload
-def get_item_oapg(self, name: typing_extensions.Literal["message"]) -
-> MetaOapg.properties.message: ... @typing.overload def get_item_oapg(self,
-name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
+[typing_extensions.Literal["loc", "msg", "type", ], str]): # dict_instance
+[name] accessor return super().__getitem__(name) @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["loc"]) -
+> 'ValidationErrorLoc': ... @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["msg"]) -> MetaOapg.properties.msg: ...
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
-["user_input"]) -> MetaOapg.properties.user_input: ... @typing.overload def
-get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema,
-schemas.Unset]: ... def get_item_oapg(self, name: typing.Union
-[typing_extensions.Literal["message", "sources", "user_input", ], str]): return
-super().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
-frozendict.frozendict, ], sources: 'SourceResponseSources', user_input:
-typing.Union[MetaOapg.properties.user_input, dict, frozendict.frozendict, ],
-message: typing.Union[MetaOapg.properties.message, str, ], _configuration:
-typing.Optional[schemas.Configuration] = None, **kwargs: typing.Union
-[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime,
-uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes], ) -
-> 'SourceResponse': return super().__new__( cls, *args, sources=sources,
-user_input=user_input, message=message, _configuration=_configuration,
-**kwargs, ) from newscatcherapi_client.model.source_response_sources import
-SourceResponseSources
+["type"]) -> MetaOapg.properties.type: ... @typing.overload def get_item_oapg
+(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+... def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["loc",
+"msg", "type", ], str]): return super().get_item_oapg(name) def __new__( cls,
+*args: typing.Union[dict, frozendict.frozendict, ], msg: typing.Union
+[MetaOapg.properties.msg, str, ], loc: 'ValidationErrorLoc', type: typing.Union
+[MetaOapg.properties.type, str, ], _configuration: typing.Optional
+[schemas.Configuration] = None, **kwargs: typing.Union[schemas.AnyTypeSchema,
+dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, None, list, tuple, bytes], ) -> 'ValidationError': return
+super().__new__( cls, *args, msg=msg, loc=loc, type=type,
+_configuration=_configuration, **kwargs, ) from
+newscatcherapi_client.model.validation_error_loc import ValidationErrorLoc
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/validation_error.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -20,94 +20,92 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 
-class SourceResponse(
+class ValidationError(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
-
-    SourceResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
-            "sources",
-            "user_input",
-            "message",
+            "msg",
+            "loc",
+            "type",
         }
         
         class properties:
-            message = schemas.StrSchema
         
             @staticmethod
-            def sources() -> typing.Type['SourceResponseSources']:
-                return SourceResponseSources
-            user_input = schemas.DictSchema
+            def loc() -> typing.Type['ValidationErrorLoc']:
+                return ValidationErrorLoc
+            msg = schemas.StrSchema
+            type = schemas.StrSchema
             __annotations__ = {
-                "message": message,
-                "sources": sources,
-                "user_input": user_input,
+                "loc": loc,
+                "msg": msg,
+                "type": type,
             }
     
-    sources: 'SourceResponseSources'
-    user_input: MetaOapg.properties.user_input
-    message: MetaOapg.properties.message
+    msg: MetaOapg.properties.msg
+    loc: 'ValidationErrorLoc'
+    type: MetaOapg.properties.type
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
+    def __getitem__(self, name: typing_extensions.Literal["loc"]) -> 'ValidationErrorLoc': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
+    def __getitem__(self, name: typing_extensions.Literal["msg"]) -> MetaOapg.properties.msg: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
+    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["message", "sources", "user_input", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["loc", "msg", "type", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["loc"]) -> 'ValidationErrorLoc': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
+    def get_item_oapg(self, name: typing_extensions.Literal["msg"]) -> MetaOapg.properties.msg: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["message", "sources", "user_input", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["loc", "msg", "type", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        sources: 'SourceResponseSources',
-        user_input: typing.Union[MetaOapg.properties.user_input, dict, frozendict.frozendict, ],
-        message: typing.Union[MetaOapg.properties.message, str, ],
+        msg: typing.Union[MetaOapg.properties.msg, str, ],
+        loc: 'ValidationErrorLoc',
+        type: typing.Union[MetaOapg.properties.type, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SourceResponse':
+    ) -> 'ValidationError':
         return super().__new__(
             cls,
             *args,
-            sources=sources,
-            user_input=user_input,
-            message=message,
+            msg=msg,
+            loc=loc,
+            type=type,
             _configuration=_configuration,
             **kwargs,
         )
 
-from newscatcherapi_client.model.source_response_sources import SourceResponseSources
+from newscatcherapi_client.model.validation_error_loc import ValidationErrorLoc
```

#### html2text {}

```diff
@@ -4,44 +4,40 @@
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
-newscatcherapi_client import schemas # noqa: F401 class SourceResponse
+newscatcherapi_client import schemas # noqa: F401 class ValidationError
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) SourceResponse DTO class. """ class MetaOapg: required =
-{ "sources", "user_input", "message", } class properties: message =
-schemas.StrSchema @staticmethod def sources() -> typing.Type
-['SourceResponseSources']: return SourceResponseSources user_input =
-schemas.DictSchema __annotations__ = { "message": message, "sources": sources,
-"user_input": user_input, } sources: 'SourceResponseSources' user_input:
-MetaOapg.properties.user_input message: MetaOapg.properties.message
-@typing.overload def __getitem__(self, name: typing_extensions.Literal
-["message"]) -> MetaOapg.properties.message: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["sources"]) -
-> 'SourceResponseSources': ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
+konfigthis.com) """ class MetaOapg: required = { "msg", "loc", "type", } class
+properties: @staticmethod def loc() -> typing.Type['ValidationErrorLoc']:
+return ValidationErrorLoc msg = schemas.StrSchema type = schemas.StrSchema
+__annotations__ = { "loc": loc, "msg": msg, "type": type, } msg:
+MetaOapg.properties.msg loc: 'ValidationErrorLoc' type:
+MetaOapg.properties.type @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["loc"]) -> 'ValidationErrorLoc': ... @typing.overload
+def __getitem__(self, name: typing_extensions.Literal["msg"]) -
+> MetaOapg.properties.msg: ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
 @typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
-[typing_extensions.Literal["message", "sources", "user_input", ], str]): #
-dict_instance[name] accessor return super().__getitem__(name) @typing.overload
-def get_item_oapg(self, name: typing_extensions.Literal["message"]) -
-> MetaOapg.properties.message: ... @typing.overload def get_item_oapg(self,
-name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
+[typing_extensions.Literal["loc", "msg", "type", ], str]): # dict_instance
+[name] accessor return super().__getitem__(name) @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["loc"]) -
+> 'ValidationErrorLoc': ... @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["msg"]) -> MetaOapg.properties.msg: ...
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
-["user_input"]) -> MetaOapg.properties.user_input: ... @typing.overload def
-get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema,
-schemas.Unset]: ... def get_item_oapg(self, name: typing.Union
-[typing_extensions.Literal["message", "sources", "user_input", ], str]): return
-super().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
-frozendict.frozendict, ], sources: 'SourceResponseSources', user_input:
-typing.Union[MetaOapg.properties.user_input, dict, frozendict.frozendict, ],
-message: typing.Union[MetaOapg.properties.message, str, ], _configuration:
-typing.Optional[schemas.Configuration] = None, **kwargs: typing.Union
-[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime,
-uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes], ) -
-> 'SourceResponse': return super().__new__( cls, *args, sources=sources,
-user_input=user_input, message=message, _configuration=_configuration,
-**kwargs, ) from newscatcherapi_client.model.source_response_sources import
-SourceResponseSources
+["type"]) -> MetaOapg.properties.type: ... @typing.overload def get_item_oapg
+(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+... def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["loc",
+"msg", "type", ], str]): return super().get_item_oapg(name) def __new__( cls,
+*args: typing.Union[dict, frozendict.frozendict, ], msg: typing.Union
+[MetaOapg.properties.msg, str, ], loc: 'ValidationErrorLoc', type: typing.Union
+[MetaOapg.properties.type, str, ], _configuration: typing.Optional
+[schemas.Configuration] = None, **kwargs: typing.Union[schemas.AnyTypeSchema,
+dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, None, list, tuple, bytes], ) -> 'ValidationError': return
+super().__new__( cls, *args, msg=msg, loc=loc, type=type,
+_configuration=_configuration, **kwargs, ) from
+newscatcherapi_client.model.validation_error_loc import ValidationErrorLoc
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/sources_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/sources_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/sources_request.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/sources_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/subscription_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/subscription_response.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/model/subscription_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/models/__init__.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,27 @@
 from newscatcherapi_client.model.dto_responses_author_search_response_search_response_articles import DtoResponsesAuthorSearchResponseSearchResponseArticles
 from newscatcherapi_client.model.dto_responses_more_like_this_response_article_result import DtoResponsesMoreLikeThisResponseArticleResult
 from newscatcherapi_client.model.dto_responses_more_like_this_response_failed_search_response import DtoResponsesMoreLikeThisResponseFailedSearchResponse
 from newscatcherapi_client.model.dto_responses_more_like_this_response_search_response import DtoResponsesMoreLikeThisResponseSearchResponse
 from newscatcherapi_client.model.dto_responses_more_like_this_response_search_response_articles import DtoResponsesMoreLikeThisResponseSearchResponseArticles
 from newscatcherapi_client.model.dto_responses_search_response_search_response import DtoResponsesSearchResponseSearchResponse
 from newscatcherapi_client.model.dto_responses_search_response_search_response_articles import DtoResponsesSearchResponseSearchResponseArticles
-from newscatcherapi_client.model.duplicates_by_original_id_request import DuplicatesByOriginalIdRequest
 from newscatcherapi_client.model.http_validation_error import HTTPValidationError
 from newscatcherapi_client.model.latest_headlines_get_response import LatestHeadlinesGetResponse
 from newscatcherapi_client.model.latest_headlines_post_response import LatestHeadlinesPostResponse
 from newscatcherapi_client.model.latest_headlines_request import LatestHeadlinesRequest
 from newscatcherapi_client.model.latest_headlines_response import LatestHeadlinesResponse
 from newscatcherapi_client.model.latest_headlines_response_articles import LatestHeadlinesResponseArticles
 from newscatcherapi_client.model.more_like_this_request import MoreLikeThisRequest
 from newscatcherapi_client.model.search_get_response import SearchGetResponse
 from newscatcherapi_client.model.search_post_response import SearchPostResponse
 from newscatcherapi_client.model.search_request import SearchRequest
 from newscatcherapi_client.model.search_similar_get_response import SearchSimilarGetResponse
 from newscatcherapi_client.model.search_similar_post_response import SearchSimilarPostResponse
 from newscatcherapi_client.model.search_url_request import SearchURLRequest
-from newscatcherapi_client.model.searchduplicatesbyoriginalid_get_response import SearchduplicatesbyoriginalidGetResponse
-from newscatcherapi_client.model.searchduplicatesbyoriginalid_post_response import SearchduplicatesbyoriginalidPostResponse
 from newscatcherapi_client.model.similar_document import SimilarDocument
 from newscatcherapi_client.model.source_info import SourceInfo
 from newscatcherapi_client.model.source_response import SourceResponse
 from newscatcherapi_client.model.source_response_sources import SourceResponseSources
 from newscatcherapi_client.model.sources_request import SourcesRequest
 from newscatcherapi_client.model.subscription_response import SubscriptionResponse
 from newscatcherapi_client.model.validation_error import ValidationError
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/operation_parameter_map.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/operation_parameter_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -1119,34 +1119,8 @@
         'parameters': [
         ]
     },
     '/api/subscription-POST': {
         'parameters': [
         ]
     },
-    '/api/search_duplicates_by_original_id-GET': {
-        'parameters': [
-            {
-                'name': 'original_article_id'
-            },
-            {
-                'name': 'page'
-            },
-            {
-                'name': 'page_size'
-            },
-        ]
-    },
-    '/api/search_duplicates_by_original_id-POST': {
-        'parameters': [
-            {
-                'name': 'original_article_id'
-            },
-            {
-                'name': 'page'
-            },
-            {
-                'name': 'page_size'
-            },
-        ]
-    },
 };
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/__init__.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,8 +9,7 @@
     API_SEARCH = "/api/search"
     API_LATEST_HEADLINES = "/api/latest_headlines"
     API_AUTHORS = "/api/authors"
     API_SEARCH_BY_LINK = "/api/search_by_link"
     API_SEARCH_SIMILAR = "/api/search_similar"
     API_SOURCES = "/api/sources"
     API_SUBSCRIPTION = "/api/subscription"
-    API_SEARCH_DUPLICATES_BY_ORIGINAL_ID = "/api/search_duplicates_by_original_id"
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/get.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_authors/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/get.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_authors/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/post.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_authors/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/post.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_authors/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/get.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_latest_headlines/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/get.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_latest_headlines/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/post.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_latest_headlines/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/post.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_latest_headlines/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/get.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/get.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/post.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/post.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/get.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_by_link/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/get.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_by_link/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/post.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_by_link/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/post.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_by_link/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/get.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_sources/get.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,99 +29,122 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
+from newscatcherapi_client.model.source_response import SourceResponse as SourceResponseSchema
 from newscatcherapi_client.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from newscatcherapi_client.model.searchduplicatesbyoriginalid_get_response import SearchduplicatesbyoriginalidGetResponse as SearchduplicatesbyoriginalidGetResponseSchema
 
-from newscatcherapi_client.type.searchduplicatesbyoriginalid_get_response import SearchduplicatesbyoriginalidGetResponse
+from newscatcherapi_client.type.source_response import SourceResponse
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
 
 from ...api_client import Dictionary
-from newscatcherapi_client.pydantic.searchduplicatesbyoriginalid_get_response import SearchduplicatesbyoriginalidGetResponse as SearchduplicatesbyoriginalidGetResponsePydantic
+from newscatcherapi_client.pydantic.source_response import SourceResponse as SourceResponsePydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
 
 from . import path
 
 # Query params
-OriginalArticleIdSchema = schemas.StrSchema
-
-
-class PageSchema(
-    schemas.IntSchema
-):
-
-
-    class MetaOapg:
-        inclusive_minimum = 0
-
-
-class PageSizeSchema(
-    schemas.IntSchema
-):
-
-
-    class MetaOapg:
-        inclusive_minimum = 0
+LangSchema = schemas.StrSchema
+CountriesSchema = schemas.StrSchema
+PredefinedSourcesSchema = schemas.StrSchema
+IncludeAdditionalInfoSchema = schemas.BoolSchema
+FromRankSchema = schemas.IntSchema
+ToRankSchema = schemas.IntSchema
+SourceNameSchema = schemas.AnyTypeSchema
+SourceUrlSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
-        'original_article_id': typing.Union[OriginalArticleIdSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
-        'page': typing.Union[PageSchema, decimal.Decimal, int, ],
-        'page_size': typing.Union[PageSizeSchema, decimal.Decimal, int, ],
+        'lang': typing.Union[LangSchema, str, ],
+        'countries': typing.Union[CountriesSchema, str, ],
+        'predefined_sources': typing.Union[PredefinedSourcesSchema, str, ],
+        'include_additional_info': typing.Union[IncludeAdditionalInfoSchema, bool, ],
+        'from_rank': typing.Union[FromRankSchema, decimal.Decimal, int, ],
+        'to_rank': typing.Union[ToRankSchema, decimal.Decimal, int, ],
+        'source_name': typing.Union[SourceNameSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'source_url': typing.Union[SourceUrlSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_original_article_id = api_client.QueryParameter(
-    name="original_article_id",
+request_query_lang = api_client.QueryParameter(
+    name="lang",
+    style=api_client.ParameterStyle.FORM,
+    schema=LangSchema,
+    explode=True,
+)
+request_query_countries = api_client.QueryParameter(
+    name="countries",
+    style=api_client.ParameterStyle.FORM,
+    schema=CountriesSchema,
+    explode=True,
+)
+request_query_predefined_sources = api_client.QueryParameter(
+    name="predefined_sources",
+    style=api_client.ParameterStyle.FORM,
+    schema=PredefinedSourcesSchema,
+    explode=True,
+)
+request_query_include_additional_info = api_client.QueryParameter(
+    name="include_additional_info",
+    style=api_client.ParameterStyle.FORM,
+    schema=IncludeAdditionalInfoSchema,
+    explode=True,
+)
+request_query_from_rank = api_client.QueryParameter(
+    name="from_rank",
+    style=api_client.ParameterStyle.FORM,
+    schema=FromRankSchema,
+    explode=True,
+)
+request_query_to_rank = api_client.QueryParameter(
+    name="to_rank",
     style=api_client.ParameterStyle.FORM,
-    schema=OriginalArticleIdSchema,
-    required=True,
+    schema=ToRankSchema,
     explode=True,
 )
-request_query_page = api_client.QueryParameter(
-    name="page",
+request_query_source_name = api_client.QueryParameter(
+    name="source_name",
     style=api_client.ParameterStyle.FORM,
-    schema=PageSchema,
+    schema=SourceNameSchema,
     explode=True,
 )
-request_query_page_size = api_client.QueryParameter(
-    name="page_size",
+request_query_source_url = api_client.QueryParameter(
+    name="source_url",
     style=api_client.ParameterStyle.FORM,
-    schema=PageSizeSchema,
+    schema=SourceUrlSchema,
     explode=True,
 )
 _auth = [
     'apiKey',
 ]
-SchemaFor200ResponseBodyApplicationJson = SearchduplicatesbyoriginalidGetResponseSchema
+SchemaFor200ResponseBodyApplicationJson = SourceResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: SearchduplicatesbyoriginalidGetResponse
+    body: SourceResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: SearchduplicatesbyoriginalidGetResponse
+    body: SourceResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -158,26 +181,41 @@
 )
 
 
 class BaseApi(api_client.Api):
 
     def _get_mapped_args(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
+        lang: typing.Optional[str] = None,
+        countries: typing.Optional[str] = None,
+        predefined_sources: typing.Optional[str] = None,
+        include_additional_info: typing.Optional[bool] = None,
+        from_rank: typing.Optional[int] = None,
+        to_rank: typing.Optional[int] = None,
+        source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        source_url: typing.Optional[str] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
-        if original_article_id is not None:
-            _query_params["original_article_id"] = original_article_id
-        if page is not None:
-            _query_params["page"] = page
-        if page_size is not None:
-            _query_params["page_size"] = page_size
+        if lang is not None:
+            _query_params["lang"] = lang
+        if countries is not None:
+            _query_params["countries"] = countries
+        if predefined_sources is not None:
+            _query_params["predefined_sources"] = predefined_sources
+        if include_additional_info is not None:
+            _query_params["include_additional_info"] = include_additional_info
+        if from_rank is not None:
+            _query_params["from_rank"] = from_rank
+        if to_rank is not None:
+            _query_params["to_rank"] = to_rank
+        if source_name is not None:
+            _query_params["source_name"] = source_name
+        if source_url is not None:
+            _query_params["source_url"] = source_url
         args.query = _query_params
         return args
 
     async def _aget_oapg(
         self,
             query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
@@ -187,27 +225,32 @@
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        [Get] Search Duplicate Articles For Articles Request
+        [Get] Search For Sources Request
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
     
         prefix_separator_iterator = None
         for parameter in (
-            request_query_original_article_id,
-            request_query_page,
-            request_query_page_size,
+            request_query_lang,
+            request_query_countries,
+            request_query_predefined_sources,
+            request_query_include_additional_info,
+            request_query_from_rank,
+            request_query_to_rank,
+            request_query_source_name,
+            request_query_source_url,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -220,15 +263,15 @@
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
         method = 'get'.upper()
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/search_duplicates_by_original_id',
+            path_template='/api/sources',
             auth_settings=_auth,
             headers=_headers,
         )
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
             method=method,
@@ -301,27 +344,32 @@
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        [Get] Search Duplicate Articles For Articles Request
+        [Get] Search For Sources Request
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
     
         prefix_separator_iterator = None
         for parameter in (
-            request_query_original_article_id,
-            request_query_page,
-            request_query_page_size,
+            request_query_lang,
+            request_query_countries,
+            request_query_predefined_sources,
+            request_query_include_additional_info,
+            request_query_from_rank,
+            request_query_to_rank,
+            request_query_source_name,
+            request_query_source_url,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -334,15 +382,15 @@
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
         method = 'get'.upper()
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/search_duplicates_by_original_id',
+            path_template='/api/sources',
             auth_settings=_auth,
             headers=_headers,
         )
     
         response = self.api_client.call_api(
             resource_path=used_path,
             method=method,
@@ -377,124 +425,184 @@
 
 
 class GetRaw(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def aget(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
+        lang: typing.Optional[str] = None,
+        countries: typing.Optional[str] = None,
+        predefined_sources: typing.Optional[str] = None,
+        include_additional_info: typing.Optional[bool] = None,
+        from_rank: typing.Optional[int] = None,
+        to_rank: typing.Optional[int] = None,
+        source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        source_url: typing.Optional[str] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+            lang=lang,
+            countries=countries,
+            predefined_sources=predefined_sources,
+            include_additional_info=include_additional_info,
+            from_rank=from_rank,
+            to_rank=to_rank,
+            source_name=source_name,
+            source_url=source_url,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
+        lang: typing.Optional[str] = None,
+        countries: typing.Optional[str] = None,
+        predefined_sources: typing.Optional[str] = None,
+        include_additional_info: typing.Optional[bool] = None,
+        from_rank: typing.Optional[int] = None,
+        to_rank: typing.Optional[int] = None,
+        source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        source_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+            lang=lang,
+            countries=countries,
+            predefined_sources=predefined_sources,
+            include_additional_info=include_additional_info,
+            from_rank=from_rank,
+            to_rank=to_rank,
+            source_name=source_name,
+            source_url=source_url,
         )
         return self._get_oapg(
             query_params=args.query,
         )
 
 class Get(BaseApi):
 
     async def aget(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
+        lang: typing.Optional[str] = None,
+        countries: typing.Optional[str] = None,
+        predefined_sources: typing.Optional[str] = None,
+        include_additional_info: typing.Optional[bool] = None,
+        from_rank: typing.Optional[int] = None,
+        to_rank: typing.Optional[int] = None,
+        source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        source_url: typing.Optional[str] = None,
         validate: bool = False,
         **kwargs,
-    ) -> SearchduplicatesbyoriginalidGetResponsePydantic:
+    ) -> SourceResponsePydantic:
         raw_response = await self.raw.aget(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+            lang=lang,
+            countries=countries,
+            predefined_sources=predefined_sources,
+            include_additional_info=include_additional_info,
+            from_rank=from_rank,
+            to_rank=to_rank,
+            source_name=source_name,
+            source_url=source_url,
             **kwargs,
         )
         if validate:
-            return RootModel[SearchduplicatesbyoriginalidGetResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(SearchduplicatesbyoriginalidGetResponsePydantic, raw_response.body)
+            return SourceResponsePydantic(**raw_response.body)
+        return api_client.construct_model_instance(SourceResponsePydantic, raw_response.body)
     
     
     def get(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
+        lang: typing.Optional[str] = None,
+        countries: typing.Optional[str] = None,
+        predefined_sources: typing.Optional[str] = None,
+        include_additional_info: typing.Optional[bool] = None,
+        from_rank: typing.Optional[int] = None,
+        to_rank: typing.Optional[int] = None,
+        source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        source_url: typing.Optional[str] = None,
         validate: bool = False,
-    ) -> SearchduplicatesbyoriginalidGetResponsePydantic:
+    ) -> SourceResponsePydantic:
         raw_response = self.raw.get(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+            lang=lang,
+            countries=countries,
+            predefined_sources=predefined_sources,
+            include_additional_info=include_additional_info,
+            from_rank=from_rank,
+            to_rank=to_rank,
+            source_name=source_name,
+            source_url=source_url,
         )
         if validate:
-            return RootModel[SearchduplicatesbyoriginalidGetResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(SearchduplicatesbyoriginalidGetResponsePydantic, raw_response.body)
+            return SourceResponsePydantic(**raw_response.body)
+        return api_client.construct_model_instance(SourceResponsePydantic, raw_response.body)
 
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def aget(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
+        lang: typing.Optional[str] = None,
+        countries: typing.Optional[str] = None,
+        predefined_sources: typing.Optional[str] = None,
+        include_additional_info: typing.Optional[bool] = None,
+        from_rank: typing.Optional[int] = None,
+        to_rank: typing.Optional[int] = None,
+        source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        source_url: typing.Optional[str] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+            lang=lang,
+            countries=countries,
+            predefined_sources=predefined_sources,
+            include_additional_info=include_additional_info,
+            from_rank=from_rank,
+            to_rank=to_rank,
+            source_name=source_name,
+            source_url=source_url,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
+        lang: typing.Optional[str] = None,
+        countries: typing.Optional[str] = None,
+        predefined_sources: typing.Optional[str] = None,
+        include_additional_info: typing.Optional[bool] = None,
+        from_rank: typing.Optional[int] = None,
+        to_rank: typing.Optional[int] = None,
+        source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        source_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+            lang=lang,
+            countries=countries,
+            predefined_sources=predefined_sources,
+            include_additional_info=include_additional_info,
+            from_rank=from_rank,
+            to_rank=to_rank,
+            source_name=source_name,
+            source_url=source_url,
         )
         return self._get_oapg(
             query_params=args.query,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/get.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_subscription/get.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,88 +29,40 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
+from newscatcherapi_client.model.subscription_response import SubscriptionResponse as SubscriptionResponseSchema
 from newscatcherapi_client.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from newscatcherapi_client.model.searchduplicatesbyoriginalid_get_response import SearchduplicatesbyoriginalidGetResponse as SearchduplicatesbyoriginalidGetResponseSchema
 
-from newscatcherapi_client.type.searchduplicatesbyoriginalid_get_response import SearchduplicatesbyoriginalidGetResponse
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
+from newscatcherapi_client.type.subscription_response import SubscriptionResponse
 
 from ...api_client import Dictionary
-from newscatcherapi_client.pydantic.searchduplicatesbyoriginalid_get_response import SearchduplicatesbyoriginalidGetResponse as SearchduplicatesbyoriginalidGetResponsePydantic
+from newscatcherapi_client.pydantic.subscription_response import SubscriptionResponse as SubscriptionResponsePydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
 
-# Query params
-OriginalArticleIdSchema = schemas.StrSchema
+from . import path
 
-
-class PageSchema(
-    schemas.IntSchema
-):
-    pass
-
-
-class PageSizeSchema(
-    schemas.IntSchema
-):
-    pass
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-        'original_article_id': typing.Union[OriginalArticleIdSchema, str, ],
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-        'page': typing.Union[PageSchema, decimal.Decimal, int, ],
-        'page_size': typing.Union[PageSizeSchema, decimal.Decimal, int, ],
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_original_article_id = api_client.QueryParameter(
-    name="original_article_id",
-    style=api_client.ParameterStyle.FORM,
-    schema=OriginalArticleIdSchema,
-    required=True,
-    explode=True,
-)
-request_query_page = api_client.QueryParameter(
-    name="page",
-    style=api_client.ParameterStyle.FORM,
-    schema=PageSchema,
-    explode=True,
-)
-request_query_page_size = api_client.QueryParameter(
-    name="page_size",
-    style=api_client.ParameterStyle.FORM,
-    schema=PageSizeSchema,
-    explode=True,
-)
-SchemaFor200ResponseBodyApplicationJson = SearchduplicatesbyoriginalidGetResponseSchema
+_auth = [
+    'apiKey',
+]
+SchemaFor200ResponseBodyApplicationJson = SubscriptionResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: SearchduplicatesbyoriginalidGetResponse
+    body: SubscriptionResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: SearchduplicatesbyoriginalidGetResponse
+    body: SubscriptionResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -134,96 +86,71 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
     def _get_mapped_args(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
-        _query_params = {}
-        if original_article_id is not None:
-            _query_params["original_article_id"] = original_article_id
-        if page is not None:
-            _query_params["page"] = page
-        if page_size is not None:
-            _query_params["page_size"] = page_size
-        args.query = _query_params
         return args
 
     async def _aget_oapg(
         self,
-            query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        [Get] Search Duplicate Articles For Articles Request
+        [Get] Get My Plan Info
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
     
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_original_article_id,
-            request_query_page,
-            request_query_page_size,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
         method = 'get'.upper()
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/search_duplicates_by_original_id',
+            path_template='/api/subscription',
             auth_settings=_auth,
             headers=_headers,
         )
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
             method=method,
             headers=_headers,
             auth_settings=_auth,
-            prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
             **kwargs
         )
     
         if stream:
             if not 200 <= response.http_response.status <= 299:
                 body = (await response.http_response.content.read()).decode("utf-8")
@@ -276,68 +203,50 @@
         await response.session.close()
     
         return api_response
 
 
     def _get_oapg(
         self,
-            query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        [Get] Search Duplicate Articles For Articles Request
+        [Get] Get My Plan Info
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
     
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_original_article_id,
-            request_query_page,
-            request_query_page_size,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
         method = 'get'.upper()
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/search_duplicates_by_original_id',
+            path_template='/api/subscription',
             auth_settings=_auth,
             headers=_headers,
         )
     
         response = self.api_client.call_api(
             resource_path=used_path,
             method=method,
             headers=_headers,
             auth_settings=_auth,
-            prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                     response,
@@ -362,124 +271,84 @@
 
 
 class GetRaw(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def aget(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
         )
         return await self._aget_oapg(
-            query_params=args.query,
             **kwargs,
         )
     
     def get(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
         )
         return self._get_oapg(
-            query_params=args.query,
         )
 
 class Get(BaseApi):
 
     async def aget(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         validate: bool = False,
         **kwargs,
-    ) -> SearchduplicatesbyoriginalidGetResponsePydantic:
+    ) -> SubscriptionResponsePydantic:
         raw_response = await self.raw.aget(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
             **kwargs,
         )
         if validate:
-            return RootModel[SearchduplicatesbyoriginalidGetResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(SearchduplicatesbyoriginalidGetResponsePydantic, raw_response.body)
+            return SubscriptionResponsePydantic(**raw_response.body)
+        return api_client.construct_model_instance(SubscriptionResponsePydantic, raw_response.body)
     
     
     def get(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         validate: bool = False,
-    ) -> SearchduplicatesbyoriginalidGetResponsePydantic:
+    ) -> SubscriptionResponsePydantic:
         raw_response = self.raw.get(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
         )
         if validate:
-            return RootModel[SearchduplicatesbyoriginalidGetResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(SearchduplicatesbyoriginalidGetResponsePydantic, raw_response.body)
+            return SubscriptionResponsePydantic(**raw_response.body)
+        return api_client.construct_model_instance(SubscriptionResponsePydantic, raw_response.body)
 
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def aget(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
         )
         return await self._aget_oapg(
-            query_params=args.query,
             **kwargs,
         )
     
     def get(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
         )
         return self._get_oapg(
-            query_params=args.query,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/post.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_subscription/post.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,54 +29,40 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
-from newscatcherapi_client.model.searchduplicatesbyoriginalid_post_response import SearchduplicatesbyoriginalidPostResponse as SearchduplicatesbyoriginalidPostResponseSchema
+from newscatcherapi_client.model.subscription_response import SubscriptionResponse as SubscriptionResponseSchema
 from newscatcherapi_client.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from newscatcherapi_client.model.duplicates_by_original_id_request import DuplicatesByOriginalIdRequest as DuplicatesByOriginalIdRequestSchema
 
-from newscatcherapi_client.type.searchduplicatesbyoriginalid_post_response import SearchduplicatesbyoriginalidPostResponse
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
-from newscatcherapi_client.type.duplicates_by_original_id_request import DuplicatesByOriginalIdRequest
+from newscatcherapi_client.type.subscription_response import SubscriptionResponse
 
 from ...api_client import Dictionary
+from newscatcherapi_client.pydantic.subscription_response import SubscriptionResponse as SubscriptionResponsePydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
-from newscatcherapi_client.pydantic.searchduplicatesbyoriginalid_post_response import SearchduplicatesbyoriginalidPostResponse as SearchduplicatesbyoriginalidPostResponsePydantic
-from newscatcherapi_client.pydantic.duplicates_by_original_id_request import DuplicatesByOriginalIdRequest as DuplicatesByOriginalIdRequestPydantic
 
 from . import path
 
-# body param
-SchemaForRequestBodyApplicationJson = DuplicatesByOriginalIdRequestSchema
-
-
-request_body_duplicates_by_original_id_request = api_client.RequestBody(
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaForRequestBodyApplicationJson),
-    },
-    required=True,
-)
 _auth = [
     'apiKey',
 ]
-SchemaFor200ResponseBodyApplicationJson = SearchduplicatesbyoriginalidPostResponseSchema
+SchemaFor200ResponseBodyApplicationJson = SubscriptionResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: SearchduplicatesbyoriginalidPostResponse
+    body: SubscriptionResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: SearchduplicatesbyoriginalidPostResponse
+    body: SubscriptionResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -113,86 +99,57 @@
 )
 
 
 class BaseApi(api_client.Api):
 
     def _post_mapped_args(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
-        _body = {}
-        if original_article_id is not None:
-            _body["original_article_id"] = original_article_id
-        if page is not None:
-            _body["page"] = page
-        if page_size is not None:
-            _body["page_size"] = page_size
-        args.body = _body
         return args
 
     async def _apost_oapg(
         self,
-        body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        content_type: str = 'application/json',
         stream: bool = False,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        [Post] Search Duplicate Articles For Articles Request
+        [Post] Get My Plan Info
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
         method = 'post'.upper()
-        _headers.add('Content-Type', content_type)
-    
-        if body is schemas.unset:
-            raise exceptions.ApiValueError(
-                'The required body parameter has an invalid value of: unset. Set a valid value instead')
-        _fields = None
-        _body = None
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/search_duplicates_by_original_id',
-            body=body,
+            path_template='/api/subscription',
             auth_settings=_auth,
             headers=_headers,
         )
-        serialized_data = request_body_duplicates_by_original_id_request.serialize(body, content_type)
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-        elif 'body' in serialized_data:
-            _body = serialized_data['body']
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
             method=method,
             headers=_headers,
-            fields=_fields,
-            serialized_body=_body,
-            body=body,
             auth_settings=_auth,
             timeout=timeout,
             **kwargs
         )
     
         if stream:
             if not 200 <= response.http_response.status <= 299:
@@ -246,67 +203,49 @@
         await response.session.close()
     
         return api_response
 
 
     def _post_oapg(
         self,
-        body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        [Post] Search Duplicate Articles For Articles Request
+        [Post] Get My Plan Info
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
         method = 'post'.upper()
-        _headers.add('Content-Type', content_type)
-    
-        if body is schemas.unset:
-            raise exceptions.ApiValueError(
-                'The required body parameter has an invalid value of: unset. Set a valid value instead')
-        _fields = None
-        _body = None
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/search_duplicates_by_original_id',
-            body=body,
+            path_template='/api/subscription',
             auth_settings=_auth,
             headers=_headers,
         )
-        serialized_data = request_body_duplicates_by_original_id_request.serialize(body, content_type)
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-        elif 'body' in serialized_data:
-            _body = serialized_data['body']
     
         response = self.api_client.call_api(
             resource_path=used_path,
             method=method,
             headers=_headers,
-            fields=_fields,
-            serialized_body=_body,
-            body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
@@ -332,124 +271,84 @@
 
 
 class PostRaw(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def apost(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
         )
         return await self._apost_oapg(
-            body=args.body,
             **kwargs,
         )
     
     def post(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
         )
         return self._post_oapg(
-            body=args.body,
         )
 
 class Post(BaseApi):
 
     async def apost(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         validate: bool = False,
         **kwargs,
-    ) -> SearchduplicatesbyoriginalidPostResponsePydantic:
+    ) -> SubscriptionResponsePydantic:
         raw_response = await self.raw.apost(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
             **kwargs,
         )
         if validate:
-            return RootModel[SearchduplicatesbyoriginalidPostResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(SearchduplicatesbyoriginalidPostResponsePydantic, raw_response.body)
+            return SubscriptionResponsePydantic(**raw_response.body)
+        return api_client.construct_model_instance(SubscriptionResponsePydantic, raw_response.body)
     
     
     def post(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         validate: bool = False,
-    ) -> SearchduplicatesbyoriginalidPostResponsePydantic:
+    ) -> SubscriptionResponsePydantic:
         raw_response = self.raw.post(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
         )
         if validate:
-            return RootModel[SearchduplicatesbyoriginalidPostResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(SearchduplicatesbyoriginalidPostResponsePydantic, raw_response.body)
+            return SubscriptionResponsePydantic(**raw_response.body)
+        return api_client.construct_model_instance(SubscriptionResponsePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
         )
         return await self._apost_oapg(
-            body=args.body,
             **kwargs,
         )
     
     def post(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
         )
         return self._post_oapg(
-            body=args.body,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/post.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_subscription/get.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -29,49 +29,35 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
-from newscatcherapi_client.model.searchduplicatesbyoriginalid_post_response import SearchduplicatesbyoriginalidPostResponse as SearchduplicatesbyoriginalidPostResponseSchema
+from newscatcherapi_client.model.subscription_response import SubscriptionResponse as SubscriptionResponseSchema
 from newscatcherapi_client.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from newscatcherapi_client.model.duplicates_by_original_id_request import DuplicatesByOriginalIdRequest as DuplicatesByOriginalIdRequestSchema
 
-from newscatcherapi_client.type.searchduplicatesbyoriginalid_post_response import SearchduplicatesbyoriginalidPostResponse
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
-from newscatcherapi_client.type.duplicates_by_original_id_request import DuplicatesByOriginalIdRequest
+from newscatcherapi_client.type.subscription_response import SubscriptionResponse
 
 from ...api_client import Dictionary
+from newscatcherapi_client.pydantic.subscription_response import SubscriptionResponse as SubscriptionResponsePydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
-from newscatcherapi_client.pydantic.searchduplicatesbyoriginalid_post_response import SearchduplicatesbyoriginalidPostResponse as SearchduplicatesbyoriginalidPostResponsePydantic
-from newscatcherapi_client.pydantic.duplicates_by_original_id_request import DuplicatesByOriginalIdRequest as DuplicatesByOriginalIdRequestPydantic
 
-# body param
-SchemaForRequestBodyApplicationJson = DuplicatesByOriginalIdRequestSchema
-
-
-request_body_duplicates_by_original_id_request = api_client.RequestBody(
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaForRequestBodyApplicationJson),
-    },
-    required=True,
-)
-SchemaFor200ResponseBodyApplicationJson = SearchduplicatesbyoriginalidPostResponseSchema
+SchemaFor200ResponseBodyApplicationJson = SubscriptionResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: SearchduplicatesbyoriginalidPostResponse
+    body: SubscriptionResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: SearchduplicatesbyoriginalidPostResponse
+    body: SubscriptionResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -102,88 +88,59 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _post_mapped_args(
+    def _get_mapped_args(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
-        _body = {}
-        if original_article_id is not None:
-            _body["original_article_id"] = original_article_id
-        if page is not None:
-            _body["page"] = page
-        if page_size is not None:
-            _body["page_size"] = page_size
-        args.body = _body
         return args
 
-    async def _apost_oapg(
+    async def _aget_oapg(
         self,
-        body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        content_type: str = 'application/json',
         stream: bool = False,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        [Post] Search Duplicate Articles For Articles Request
+        [Get] Get My Plan Info
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-        method = 'post'.upper()
-        _headers.add('Content-Type', content_type)
-    
-        if body is schemas.unset:
-            raise exceptions.ApiValueError(
-                'The required body parameter has an invalid value of: unset. Set a valid value instead')
-        _fields = None
-        _body = None
+        method = 'get'.upper()
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/search_duplicates_by_original_id',
-            body=body,
+            path_template='/api/subscription',
             auth_settings=_auth,
             headers=_headers,
         )
-        serialized_data = request_body_duplicates_by_original_id_request.serialize(body, content_type)
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-        elif 'body' in serialized_data:
-            _body = serialized_data['body']
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
             method=method,
             headers=_headers,
-            fields=_fields,
-            serialized_body=_body,
-            body=body,
             auth_settings=_auth,
             timeout=timeout,
             **kwargs
         )
     
         if stream:
             if not 200 <= response.http_response.status <= 299:
@@ -235,69 +192,51 @@
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
 
-    def _post_oapg(
+    def _get_oapg(
         self,
-        body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        [Post] Search Duplicate Articles For Articles Request
+        [Get] Get My Plan Info
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-        method = 'post'.upper()
-        _headers.add('Content-Type', content_type)
-    
-        if body is schemas.unset:
-            raise exceptions.ApiValueError(
-                'The required body parameter has an invalid value of: unset. Set a valid value instead')
-        _fields = None
-        _body = None
+        method = 'get'.upper()
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/search_duplicates_by_original_id',
-            body=body,
+            path_template='/api/subscription',
             auth_settings=_auth,
             headers=_headers,
         )
-        serialized_data = request_body_duplicates_by_original_id_request.serialize(body, content_type)
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-        elif 'body' in serialized_data:
-            _body = serialized_data['body']
     
         response = self.api_client.call_api(
             resource_path=used_path,
             method=method,
             headers=_headers,
-            fields=_fields,
-            serialized_body=_body,
-            body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
@@ -318,129 +257,89 @@
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
 
-class PostRaw(BaseApi):
+class GetRaw(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def apost(
+    async def aget(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._post_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+        args = self._get_mapped_args(
         )
-        return await self._apost_oapg(
-            body=args.body,
+        return await self._aget_oapg(
             **kwargs,
         )
     
-    def post(
+    def get(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._post_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+        args = self._get_mapped_args(
         )
-        return self._post_oapg(
-            body=args.body,
+        return self._get_oapg(
         )
 
-class Post(BaseApi):
+class Get(BaseApi):
 
-    async def apost(
+    async def aget(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         validate: bool = False,
         **kwargs,
-    ) -> SearchduplicatesbyoriginalidPostResponsePydantic:
-        raw_response = await self.raw.apost(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+    ) -> SubscriptionResponsePydantic:
+        raw_response = await self.raw.aget(
             **kwargs,
         )
         if validate:
-            return RootModel[SearchduplicatesbyoriginalidPostResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(SearchduplicatesbyoriginalidPostResponsePydantic, raw_response.body)
+            return SubscriptionResponsePydantic(**raw_response.body)
+        return api_client.construct_model_instance(SubscriptionResponsePydantic, raw_response.body)
     
     
-    def post(
+    def get(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         validate: bool = False,
-    ) -> SearchduplicatesbyoriginalidPostResponsePydantic:
-        raw_response = self.raw.post(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+    ) -> SubscriptionResponsePydantic:
+        raw_response = self.raw.get(
         )
         if validate:
-            return RootModel[SearchduplicatesbyoriginalidPostResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(SearchduplicatesbyoriginalidPostResponsePydantic, raw_response.body)
+            return SubscriptionResponsePydantic(**raw_response.body)
+        return api_client.construct_model_instance(SubscriptionResponsePydantic, raw_response.body)
 
 
-class ApiForpost(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def apost(
+    async def aget(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._post_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+        args = self._get_mapped_args(
         )
-        return await self._apost_oapg(
-            body=args.body,
+        return await self._aget_oapg(
             **kwargs,
         )
     
-    def post(
+    def get(
         self,
-        original_article_id: str,
-        page: typing.Optional[int] = None,
-        page_size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._post_mapped_args(
-            original_article_id=original_article_id,
-            page=page,
-            page_size=page_size,
+        args = self._get_mapped_args(
         )
-        return self._post_oapg(
-            body=args.body,
+        return self._get_oapg(
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/get.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_similar/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/get.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_similar/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/post.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_similar/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/post.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_search_similar/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/get.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_sources/get.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,14 @@
 from newscatcherapi_client.type.source_response import SourceResponse
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
 
 from ...api_client import Dictionary
 from newscatcherapi_client.pydantic.source_response import SourceResponse as SourceResponsePydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
 
-from . import path
-
 # Query params
 LangSchema = schemas.StrSchema
 CountriesSchema = schemas.StrSchema
 PredefinedSourcesSchema = schemas.StrSchema
 IncludeAdditionalInfoSchema = schemas.BoolSchema
 FromRankSchema = schemas.IntSchema
 ToRankSchema = schemas.IntSchema
@@ -123,17 +121,14 @@
 )
 request_query_source_url = api_client.QueryParameter(
     name="source_url",
     style=api_client.ParameterStyle.FORM,
     schema=SourceUrlSchema,
     explode=True,
 )
-_auth = [
-    'apiKey',
-]
 SchemaFor200ResponseBodyApplicationJson = SourceResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: SourceResponse
 
@@ -168,18 +163,14 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/get.pyi` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_sources/post.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,104 +31,41 @@
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
 from newscatcherapi_client.model.source_response import SourceResponse as SourceResponseSchema
 from newscatcherapi_client.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from newscatcherapi_client.model.sources_request import SourcesRequest as SourcesRequestSchema
 
 from newscatcherapi_client.type.source_response import SourceResponse
+from newscatcherapi_client.type.sources_request import SourcesRequest
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
 
 from ...api_client import Dictionary
 from newscatcherapi_client.pydantic.source_response import SourceResponse as SourceResponsePydantic
+from newscatcherapi_client.pydantic.sources_request import SourcesRequest as SourcesRequestPydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
 
-# Query params
-LangSchema = schemas.StrSchema
-CountriesSchema = schemas.StrSchema
-PredefinedSourcesSchema = schemas.StrSchema
-IncludeAdditionalInfoSchema = schemas.BoolSchema
-FromRankSchema = schemas.IntSchema
-ToRankSchema = schemas.IntSchema
-SourceNameSchema = schemas.AnyTypeSchema
-SourceUrlSchema = schemas.StrSchema
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-        'lang': typing.Union[LangSchema, str, ],
-        'countries': typing.Union[CountriesSchema, str, ],
-        'predefined_sources': typing.Union[PredefinedSourcesSchema, str, ],
-        'include_additional_info': typing.Union[IncludeAdditionalInfoSchema, bool, ],
-        'from_rank': typing.Union[FromRankSchema, decimal.Decimal, int, ],
-        'to_rank': typing.Union[ToRankSchema, decimal.Decimal, int, ],
-        'source_name': typing.Union[SourceNameSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        'source_url': typing.Union[SourceUrlSchema, str, ],
-    },
-    total=False
-)
+from . import path
 
+# body param
+SchemaForRequestBodyApplicationJson = SourcesRequestSchema
 
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
 
-
-request_query_lang = api_client.QueryParameter(
-    name="lang",
-    style=api_client.ParameterStyle.FORM,
-    schema=LangSchema,
-    explode=True,
-)
-request_query_countries = api_client.QueryParameter(
-    name="countries",
-    style=api_client.ParameterStyle.FORM,
-    schema=CountriesSchema,
-    explode=True,
-)
-request_query_predefined_sources = api_client.QueryParameter(
-    name="predefined_sources",
-    style=api_client.ParameterStyle.FORM,
-    schema=PredefinedSourcesSchema,
-    explode=True,
-)
-request_query_include_additional_info = api_client.QueryParameter(
-    name="include_additional_info",
-    style=api_client.ParameterStyle.FORM,
-    schema=IncludeAdditionalInfoSchema,
-    explode=True,
-)
-request_query_from_rank = api_client.QueryParameter(
-    name="from_rank",
-    style=api_client.ParameterStyle.FORM,
-    schema=FromRankSchema,
-    explode=True,
-)
-request_query_to_rank = api_client.QueryParameter(
-    name="to_rank",
-    style=api_client.ParameterStyle.FORM,
-    schema=ToRankSchema,
-    explode=True,
-)
-request_query_source_name = api_client.QueryParameter(
-    name="source_name",
-    style=api_client.ParameterStyle.FORM,
-    schema=SourceNameSchema,
-    explode=True,
-)
-request_query_source_url = api_client.QueryParameter(
-    name="source_url",
-    style=api_client.ParameterStyle.FORM,
-    schema=SourceUrlSchema,
-    explode=True,
+request_body_sources_request = api_client.RequestBody(
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+    },
+    required=True,
 )
+_auth = [
+    'apiKey',
+]
 SchemaFor200ResponseBodyApplicationJson = SourceResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: SourceResponse
 
@@ -163,116 +100,115 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _get_mapped_args(
+    def _post_mapped_args(
         self,
         lang: typing.Optional[str] = None,
         countries: typing.Optional[str] = None,
         predefined_sources: typing.Optional[str] = None,
         include_additional_info: typing.Optional[bool] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_url: typing.Optional[str] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
-        _query_params = {}
+        _body = {}
         if lang is not None:
-            _query_params["lang"] = lang
+            _body["lang"] = lang
         if countries is not None:
-            _query_params["countries"] = countries
+            _body["countries"] = countries
         if predefined_sources is not None:
-            _query_params["predefined_sources"] = predefined_sources
+            _body["predefined_sources"] = predefined_sources
         if include_additional_info is not None:
-            _query_params["include_additional_info"] = include_additional_info
+            _body["include_additional_info"] = include_additional_info
         if from_rank is not None:
-            _query_params["from_rank"] = from_rank
+            _body["from_rank"] = from_rank
         if to_rank is not None:
-            _query_params["to_rank"] = to_rank
+            _body["to_rank"] = to_rank
         if source_name is not None:
-            _query_params["source_name"] = source_name
+            _body["source_name"] = source_name
         if source_url is not None:
-            _query_params["source_url"] = source_url
-        args.query = _query_params
+            _body["source_url"] = source_url
+        args.body = _body
         return args
 
-    async def _aget_oapg(
+    async def _apost_oapg(
         self,
-            query_params: typing.Optional[dict] = {},
+        body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json',
         stream: bool = False,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        [Get] Search For Sources Request
+        [Post] Search For Sources Request
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
     
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_lang,
-            request_query_countries,
-            request_query_predefined_sources,
-            request_query_include_additional_info,
-            request_query_from_rank,
-            request_query_to_rank,
-            request_query_source_name,
-            request_query_source_url,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-        method = 'get'.upper()
+        method = 'post'.upper()
+        _headers.add('Content-Type', content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
             path_template='/api/sources',
+            body=body,
             auth_settings=_auth,
             headers=_headers,
         )
+        serialized_data = request_body_sources_request.serialize(body, content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
             method=method,
             headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
             auth_settings=_auth,
-            prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
             **kwargs
         )
     
         if stream:
             if not 200 <= response.http_response.status <= 299:
                 body = (await response.http_response.content.read()).decode("utf-8")
@@ -323,75 +259,70 @@
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
 
-    def _get_oapg(
+    def _post_oapg(
         self,
-            query_params: typing.Optional[dict] = {},
+        body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        [Get] Search For Sources Request
+        [Post] Search For Sources Request
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
     
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_lang,
-            request_query_countries,
-            request_query_predefined_sources,
-            request_query_include_additional_info,
-            request_query_from_rank,
-            request_query_to_rank,
-            request_query_source_name,
-            request_query_source_url,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-        method = 'get'.upper()
+        method = 'post'.upper()
+        _headers.add('Content-Type', content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
             path_template='/api/sources',
+            body=body,
             auth_settings=_auth,
             headers=_headers,
         )
+        serialized_data = request_body_sources_request.serialize(body, content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
     
         response = self.api_client.call_api(
             resource_path=used_path,
             method=method,
             headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
             auth_settings=_auth,
-            prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                     response,
@@ -411,18 +342,18 @@
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
 
-class GetRaw(BaseApi):
+class PostRaw(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aget(
+    async def apost(
         self,
         lang: typing.Optional[str] = None,
         countries: typing.Optional[str] = None,
         predefined_sources: typing.Optional[str] = None,
         include_additional_info: typing.Optional[bool] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
@@ -430,73 +361,73 @@
         source_url: typing.Optional[str] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_mapped_args(
+        args = self._post_mapped_args(
             lang=lang,
             countries=countries,
             predefined_sources=predefined_sources,
             include_additional_info=include_additional_info,
             from_rank=from_rank,
             to_rank=to_rank,
             source_name=source_name,
             source_url=source_url,
         )
-        return await self._aget_oapg(
-            query_params=args.query,
+        return await self._apost_oapg(
+            body=args.body,
             **kwargs,
         )
     
-    def get(
+    def post(
         self,
         lang: typing.Optional[str] = None,
         countries: typing.Optional[str] = None,
         predefined_sources: typing.Optional[str] = None,
         include_additional_info: typing.Optional[bool] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_mapped_args(
+        args = self._post_mapped_args(
             lang=lang,
             countries=countries,
             predefined_sources=predefined_sources,
             include_additional_info=include_additional_info,
             from_rank=from_rank,
             to_rank=to_rank,
             source_name=source_name,
             source_url=source_url,
         )
-        return self._get_oapg(
-            query_params=args.query,
+        return self._post_oapg(
+            body=args.body,
         )
 
-class Get(BaseApi):
+class Post(BaseApi):
 
-    async def aget(
+    async def apost(
         self,
         lang: typing.Optional[str] = None,
         countries: typing.Optional[str] = None,
         predefined_sources: typing.Optional[str] = None,
         include_additional_info: typing.Optional[bool] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_url: typing.Optional[str] = None,
         validate: bool = False,
         **kwargs,
     ) -> SourceResponsePydantic:
-        raw_response = await self.raw.aget(
+        raw_response = await self.raw.apost(
             lang=lang,
             countries=countries,
             predefined_sources=predefined_sources,
             include_additional_info=include_additional_info,
             from_rank=from_rank,
             to_rank=to_rank,
             source_name=source_name,
@@ -504,45 +435,45 @@
             **kwargs,
         )
         if validate:
             return SourceResponsePydantic(**raw_response.body)
         return api_client.construct_model_instance(SourceResponsePydantic, raw_response.body)
     
     
-    def get(
+    def post(
         self,
         lang: typing.Optional[str] = None,
         countries: typing.Optional[str] = None,
         predefined_sources: typing.Optional[str] = None,
         include_additional_info: typing.Optional[bool] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_url: typing.Optional[str] = None,
         validate: bool = False,
     ) -> SourceResponsePydantic:
-        raw_response = self.raw.get(
+        raw_response = self.raw.post(
             lang=lang,
             countries=countries,
             predefined_sources=predefined_sources,
             include_additional_info=include_additional_info,
             from_rank=from_rank,
             to_rank=to_rank,
             source_name=source_name,
             source_url=source_url,
         )
         if validate:
             return SourceResponsePydantic(**raw_response.body)
         return api_client.construct_model_instance(SourceResponsePydantic, raw_response.body)
 
 
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def aget(
+    async def apost(
         self,
         lang: typing.Optional[str] = None,
         countries: typing.Optional[str] = None,
         predefined_sources: typing.Optional[str] = None,
         include_additional_info: typing.Optional[bool] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
@@ -550,50 +481,50 @@
         source_url: typing.Optional[str] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_mapped_args(
+        args = self._post_mapped_args(
             lang=lang,
             countries=countries,
             predefined_sources=predefined_sources,
             include_additional_info=include_additional_info,
             from_rank=from_rank,
             to_rank=to_rank,
             source_name=source_name,
             source_url=source_url,
         )
-        return await self._aget_oapg(
-            query_params=args.query,
+        return await self._apost_oapg(
+            body=args.body,
             **kwargs,
         )
     
-    def get(
+    def post(
         self,
         lang: typing.Optional[str] = None,
         countries: typing.Optional[str] = None,
         predefined_sources: typing.Optional[str] = None,
         include_additional_info: typing.Optional[bool] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_mapped_args(
+        args = self._post_mapped_args(
             lang=lang,
             countries=countries,
             predefined_sources=predefined_sources,
             include_additional_info=include_additional_info,
             from_rank=from_rank,
             to_rank=to_rank,
             source_name=source_name,
             source_url=source_url,
         )
-        return self._get_oapg(
-            query_params=args.query,
+        return self._post_oapg(
+            body=args.body,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/post.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_sources/post.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -42,30 +42,25 @@
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
 
 from ...api_client import Dictionary
 from newscatcherapi_client.pydantic.source_response import SourceResponse as SourceResponsePydantic
 from newscatcherapi_client.pydantic.sources_request import SourcesRequest as SourcesRequestPydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
 
-from . import path
-
 # body param
 SchemaForRequestBodyApplicationJson = SourcesRequestSchema
 
 
 request_body_sources_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'apiKey',
-]
 SchemaFor200ResponseBodyApplicationJson = SourceResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: SourceResponse
 
@@ -100,18 +95,14 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/get.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/paths/api_subscription/post.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -39,19 +39,14 @@
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
 from newscatcherapi_client.type.subscription_response import SubscriptionResponse
 
 from ...api_client import Dictionary
 from newscatcherapi_client.pydantic.subscription_response import SubscriptionResponse as SubscriptionResponsePydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
 
-from . import path
-
-_auth = [
-    'apiKey',
-]
 SchemaFor200ResponseBodyApplicationJson = SubscriptionResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: SubscriptionResponse
 
@@ -86,57 +81,53 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _get_mapped_args(
+    def _post_mapped_args(
         self,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         return args
 
-    async def _aget_oapg(
+    async def _apost_oapg(
         self,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        [Get] Get My Plan Info
+        [Post] Get My Plan Info
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-        method = 'get'.upper()
+        method = 'post'.upper()
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
             path_template='/api/subscription',
             auth_settings=_auth,
             headers=_headers,
@@ -201,38 +192,38 @@
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
 
-    def _get_oapg(
+    def _post_oapg(
         self,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        [Get] Get My Plan Info
+        [Post] Get My Plan Info
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-        method = 'get'.upper()
+        method = 'post'.upper()
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
             path_template='/api/subscription',
             auth_settings=_auth,
             headers=_headers,
@@ -266,89 +257,89 @@
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
 
-class GetRaw(BaseApi):
+class PostRaw(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aget(
+    async def apost(
         self,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_mapped_args(
+        args = self._post_mapped_args(
         )
-        return await self._aget_oapg(
+        return await self._apost_oapg(
             **kwargs,
         )
     
-    def get(
+    def post(
         self,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_mapped_args(
+        args = self._post_mapped_args(
         )
-        return self._get_oapg(
+        return self._post_oapg(
         )
 
-class Get(BaseApi):
+class Post(BaseApi):
 
-    async def aget(
+    async def apost(
         self,
         validate: bool = False,
         **kwargs,
     ) -> SubscriptionResponsePydantic:
-        raw_response = await self.raw.aget(
+        raw_response = await self.raw.apost(
             **kwargs,
         )
         if validate:
             return SubscriptionResponsePydantic(**raw_response.body)
         return api_client.construct_model_instance(SubscriptionResponsePydantic, raw_response.body)
     
     
-    def get(
+    def post(
         self,
         validate: bool = False,
     ) -> SubscriptionResponsePydantic:
-        raw_response = self.raw.get(
+        raw_response = self.raw.post(
         )
         if validate:
             return SubscriptionResponsePydantic(**raw_response.body)
         return api_client.construct_model_instance(SubscriptionResponsePydantic, raw_response.body)
 
 
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def aget(
+    async def apost(
         self,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_mapped_args(
+        args = self._post_mapped_args(
         )
-        return await self._aget_oapg(
+        return await self._apost_oapg(
             **kwargs,
         )
     
-    def get(
+    def post(
         self,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_mapped_args(
+        args = self._post_mapped_args(
         )
-        return self._get_oapg(
+        return self._post_oapg(
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/author_search_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/author_search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/cluster.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/latest_headlines_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_url_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/search_url_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_get_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,12 @@
     Generated by: https://konfigthis.com
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
-from pydantic import BaseModel, Field, RootModel, ConfigDict
 
-from newscatcherapi_client.pydantic.clustering_search_response import ClusteringSearchResponse
-from newscatcherapi_client.pydantic.dto_responses_search_response_search_response import DtoResponsesSearchResponseSearchResponse
+from newscatcherapi_client.type.clustering_search_response import ClusteringSearchResponse
+from newscatcherapi_client.type.dto_responses_search_response_search_response import DtoResponsesSearchResponseSearchResponse
 
-SearchduplicatesbyoriginalidGetResponse = typing.Union[DtoResponsesSearchResponseSearchResponse,ClusteringSearchResponse]
+SearchGetResponse = typing.Union[DtoResponsesSearchResponseSearchResponse,ClusteringSearchResponse]
```

#### html2text {}

```diff
@@ -2,14 +2,12 @@
 ssl.webflow.com/6429857b17973b636c2195c5/
 646c6f1eb774ff2f2997bec5_newscatcher_.svg]
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import datetime, date import typing from enum
 import Enum from typing_extensions import TypedDict, Literal, TYPE_CHECKING
-from pydantic import BaseModel, Field, RootModel, ConfigDict from
-newscatcherapi_client.pydantic.clustering_search_response import
+from newscatcherapi_client.type.clustering_search_response import
 ClusteringSearchResponse from
-newscatcherapi_client.pydantic.dto_responses_search_response_search_response
-import DtoResponsesSearchResponseSearchResponse
-SearchduplicatesbyoriginalidGetResponse = typing.Union
+newscatcherapi_client.type.dto_responses_search_response_search_response import
+DtoResponsesSearchResponseSearchResponse SearchGetResponse = typing.Union
 [DtoResponsesSearchResponseSearchResponse,ClusteringSearchResponse]
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/similar_document.py`

 * *Files 23% similar despite different names*

```diff
@@ -33,29 +33,27 @@
 00000200: 6578 7465 6e73 696f 6e73 2069 6d70 6f72  extensions impor
 00000210: 7420 5479 7065 6444 6963 742c 204c 6974  t TypedDict, Lit
 00000220: 6572 616c 2c20 5459 5045 5f43 4845 434b  eral, TYPE_CHECK
 00000230: 494e 470a 6672 6f6d 2070 7964 616e 7469  ING.from pydanti
 00000240: 6320 696d 706f 7274 2042 6173 654d 6f64  c import BaseMod
 00000250: 656c 2c20 4669 656c 642c 2052 6f6f 744d  el, Field, RootM
 00000260: 6f64 656c 2c20 436f 6e66 6967 4469 6374  odel, ConfigDict
-00000270: 0a0a 6672 6f6d 206e 6577 7363 6174 6368  ..from newscatch
-00000280: 6572 6170 695f 636c 6965 6e74 2e70 7964  erapi_client.pyd
-00000290: 616e 7469 632e 636c 7573 7465 7269 6e67  antic.clustering
-000002a0: 5f73 6561 7263 685f 7265 7370 6f6e 7365  _search_response
-000002b0: 2069 6d70 6f72 7420 436c 7573 7465 7269   import Clusteri
-000002c0: 6e67 5365 6172 6368 5265 7370 6f6e 7365  ngSearchResponse
-000002d0: 0a66 726f 6d20 6e65 7773 6361 7463 6865  .from newscatche
-000002e0: 7261 7069 5f63 6c69 656e 742e 7079 6461  rapi_client.pyda
-000002f0: 6e74 6963 2e64 746f 5f72 6573 706f 6e73  ntic.dto_respons
-00000300: 6573 5f73 6561 7263 685f 7265 7370 6f6e  es_search_respon
-00000310: 7365 5f73 6561 7263 685f 7265 7370 6f6e  se_search_respon
-00000320: 7365 2069 6d70 6f72 7420 4474 6f52 6573  se import DtoRes
-00000330: 706f 6e73 6573 5365 6172 6368 5265 7370  ponsesSearchResp
-00000340: 6f6e 7365 5365 6172 6368 5265 7370 6f6e  onseSearchRespon
-00000350: 7365 0a0a 5365 6172 6368 6475 706c 6963  se..Searchduplic
-00000360: 6174 6573 6279 6f72 6967 696e 616c 6964  atesbyoriginalid
-00000370: 506f 7374 5265 7370 6f6e 7365 203d 2074  PostResponse = t
-00000380: 7970 696e 672e 556e 696f 6e5b 4474 6f52  yping.Union[DtoR
-00000390: 6573 706f 6e73 6573 5365 6172 6368 5265  esponsesSearchRe
-000003a0: 7370 6f6e 7365 5365 6172 6368 5265 7370  sponseSearchResp
-000003b0: 6f6e 7365 2c43 6c75 7374 6572 696e 6753  onse,ClusteringS
-000003c0: 6561 7263 6852 6573 706f 6e73 655d 0a    earchResponse].
+00000270: 0a0a 0a63 6c61 7373 2053 696d 696c 6172  ...class Similar
+00000280: 446f 6375 6d65 6e74 2842 6173 654d 6f64  Document(BaseMod
+00000290: 656c 293a 0a20 2020 2074 6974 6c65 3a20  el):.    title: 
+000002a0: 7374 7220 3d20 4669 656c 6428 616c 6961  str = Field(alia
+000002b0: 733d 2774 6974 6c65 2729 0a0a 2020 2020  s='title')..    
+000002c0: 6964 3a20 7374 7220 3d20 4669 656c 6428  id: str = Field(
+000002d0: 616c 6961 733d 2769 6427 290a 0a20 2020  alias='id')..   
+000002e0: 2073 636f 7265 3a20 7479 7069 6e67 2e55   score: typing.U
+000002f0: 6e69 6f6e 5b69 6e74 2c20 666c 6f61 745d  nion[int, float]
+00000300: 203d 2046 6965 6c64 2861 6c69 6173 3d27   = Field(alias='
+00000310: 7363 6f72 6527 290a 0a20 2020 206c 696e  score')..    lin
+00000320: 6b3a 2073 7472 203d 2046 6965 6c64 2861  k: str = Field(a
+00000330: 6c69 6173 3d27 6c69 6e6b 2729 0a0a 2020  lias='link')..  
+00000340: 2020 6d6f 6465 6c5f 636f 6e66 6967 203d    model_config =
+00000350: 2043 6f6e 6669 6744 6963 7428 0a20 2020   ConfigDict(.   
+00000360: 2020 2020 2070 726f 7465 6374 6564 5f6e       protected_n
+00000370: 616d 6573 7061 6365 733d 2829 2c0a 2020  amespaces=(),.  
+00000380: 2020 2020 2020 6172 6269 7472 6172 795f        arbitrary_
+00000390: 7479 7065 735f 616c 6c6f 7765 643d 5472  types_allowed=Tr
+000003a0: 7565 0a20 2020 2029 0a                   ue.    ).
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/similar_document.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/source_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 from pydantic import BaseModel, Field, RootModel, ConfigDict
 
+from newscatcherapi_client.pydantic.source_response_sources import SourceResponseSources
 
-class SimilarDocument(BaseModel):
-    title: str = Field(alias='title')
+class SourceResponse(BaseModel):
+    message: str = Field(alias='message')
 
-    id: str = Field(alias='id')
+    sources: SourceResponseSources = Field(alias='sources')
 
-    score: typing.Union[int, float] = Field(alias='score')
-
-    link: str = Field(alias='link')
+    user_input: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(alias='user_input')
 
     model_config = ConfigDict(
         protected_namespaces=(),
         arbitrary_types_allowed=True
     )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_info.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/validation_error.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 from pydantic import BaseModel, Field, RootModel, ConfigDict
 
-from newscatcherapi_client.pydantic.source_response_sources import SourceResponseSources
+from newscatcherapi_client.pydantic.validation_error_loc import ValidationErrorLoc
 
-class SourceResponse(BaseModel):
-    message: str = Field(alias='message')
+class ValidationError(BaseModel):
+    loc: ValidationErrorLoc = Field(alias='loc')
 
-    sources: SourceResponseSources = Field(alias='sources')
+    msg: str = Field(alias='msg')
 
-    user_input: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(alias='user_input')
+    type: str = Field(alias='type')
 
     model_config = ConfigDict(
         protected_namespaces=(),
         arbitrary_types_allowed=True
     )
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/sources_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/sources_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/subscription_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/validation_error.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/sources_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,22 +10,31 @@
     Generated by: https://konfigthis.com
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
-from pydantic import BaseModel, Field, RootModel, ConfigDict
 
-from newscatcherapi_client.pydantic.validation_error_loc import ValidationErrorLoc
 
-class ValidationError(BaseModel):
-    loc: ValidationErrorLoc = Field(alias='loc')
+class RequiredSourcesRequest(TypedDict):
+    pass
 
-    msg: str = Field(alias='msg')
+class OptionalSourcesRequest(TypedDict, total=False):
+    lang: str
 
-    type: str = Field(alias='type')
+    countries: str
 
-    model_config = ConfigDict(
-        protected_namespaces=(),
-        arbitrary_types_allowed=True
-    )
+    predefined_sources: str
+
+    include_additional_info: bool
+
+    from_rank: int
+
+    to_rank: int
+
+    source_name: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
+
+    source_url: str
+
+class SourcesRequest(RequiredSourcesRequest, OptionalSourcesRequest):
+    pass
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/pydantic/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_after_hook.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_before_hook.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_before_url_hook.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/request_before_url_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/rest.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/schemas.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/schemas.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/author_search_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/author_search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/cluster.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/duplicates_by_original_id_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_url_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 
 
-class RequiredDuplicatesByOriginalIdRequest(TypedDict):
-    original_article_id: str
+class RequiredSearchURLRequest(TypedDict):
+    pass
+
+class OptionalSearchURLRequest(TypedDict, total=False):
+    ids: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
+
+    links: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
-class OptionalDuplicatesByOriginalIdRequest(TypedDict, total=False):
     page: int
 
     page_size: int
 
-class DuplicatesByOriginalIdRequest(RequiredDuplicatesByOriginalIdRequest, OptionalDuplicatesByOriginalIdRequest):
+class SearchURLRequest(RequiredSearchURLRequest, OptionalSearchURLRequest):
     pass
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/latest_headlines_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_post_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 
 from newscatcherapi_client.type.clustering_search_response import ClusteringSearchResponse
 from newscatcherapi_client.type.dto_responses_search_response_search_response import DtoResponsesSearchResponseSearchResponse
 
-SearchGetResponse = typing.Union[DtoResponsesSearchResponseSearchResponse,ClusteringSearchResponse]
+SearchPostResponse = typing.Union[DtoResponsesSearchResponseSearchResponse,ClusteringSearchResponse]
```

#### html2text {}

```diff
@@ -5,9 +5,9 @@
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import datetime, date import typing from enum
 import Enum from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 from newscatcherapi_client.type.clustering_search_response import
 ClusteringSearchResponse from
 newscatcherapi_client.type.dto_responses_search_response_search_response import
-DtoResponsesSearchResponseSearchResponse SearchGetResponse = typing.Union
+DtoResponsesSearchResponseSearchResponse SearchPostResponse = typing.Union
 [DtoResponsesSearchResponseSearchResponse,ClusteringSearchResponse]
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_post_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_similar_get_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 
-from newscatcherapi_client.type.clustering_search_response import ClusteringSearchResponse
-from newscatcherapi_client.type.dto_responses_search_response_search_response import DtoResponsesSearchResponseSearchResponse
+from newscatcherapi_client.type.dto_responses_more_like_this_response_failed_search_response import DtoResponsesMoreLikeThisResponseFailedSearchResponse
+from newscatcherapi_client.type.dto_responses_more_like_this_response_search_response import DtoResponsesMoreLikeThisResponseSearchResponse
 
-SearchPostResponse = typing.Union[DtoResponsesSearchResponseSearchResponse,ClusteringSearchResponse]
+SearchSimilarGetResponse = typing.Union[DtoResponsesMoreLikeThisResponseSearchResponse,DtoResponsesMoreLikeThisResponseFailedSearchResponse]
```

#### html2text {}

```diff
@@ -2,12 +2,14 @@
 ssl.webflow.com/6429857b17973b636c2195c5/
 646c6f1eb774ff2f2997bec5_newscatcher_.svg]
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import datetime, date import typing from enum
 import Enum from typing_extensions import TypedDict, Literal, TYPE_CHECKING
-from newscatcherapi_client.type.clustering_search_response import
-ClusteringSearchResponse from
-newscatcherapi_client.type.dto_responses_search_response_search_response import
-DtoResponsesSearchResponseSearchResponse SearchPostResponse = typing.Union
-[DtoResponsesSearchResponseSearchResponse,ClusteringSearchResponse]
+from
+newscatcherapi_client.type.dto_responses_more_like_this_response_failed_search_response
+import DtoResponsesMoreLikeThisResponseFailedSearchResponse from
+newscatcherapi_client.type.dto_responses_more_like_this_response_search_response
+import DtoResponsesMoreLikeThisResponseSearchResponse SearchSimilarGetResponse
+= typing.Union
+[DtoResponsesMoreLikeThisResponseSearchResponse,DtoResponsesMoreLikeThisResponseFailedSearchResponse]
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_request.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/search_similar_post_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 
 from newscatcherapi_client.type.dto_responses_more_like_this_response_failed_search_response import DtoResponsesMoreLikeThisResponseFailedSearchResponse
 from newscatcherapi_client.type.dto_responses_more_like_this_response_search_response import DtoResponsesMoreLikeThisResponseSearchResponse
 
-SearchSimilarGetResponse = typing.Union[DtoResponsesMoreLikeThisResponseSearchResponse,DtoResponsesMoreLikeThisResponseFailedSearchResponse]
+SearchSimilarPostResponse = typing.Union[DtoResponsesMoreLikeThisResponseSearchResponse,DtoResponsesMoreLikeThisResponseFailedSearchResponse]
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import datetime, date import typing from enum
 import Enum from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 from
 newscatcherapi_client.type.dto_responses_more_like_this_response_failed_search_response
 import DtoResponsesMoreLikeThisResponseFailedSearchResponse from
 newscatcherapi_client.type.dto_responses_more_like_this_response_search_response
-import DtoResponsesMoreLikeThisResponseSearchResponse SearchSimilarGetResponse
+import DtoResponsesMoreLikeThisResponseSearchResponse SearchSimilarPostResponse
 = typing.Union
 [DtoResponsesMoreLikeThisResponseSearchResponse,DtoResponsesMoreLikeThisResponseFailedSearchResponse]
```

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/similar_document.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/similar_document.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_info.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/source_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/subscription_response.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/validation_error.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type_util.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/type_util.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/validation_metadata.py` & `newscatcherapi_python_sdk-6.0.6/newscatcherapi_client/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.5/pyproject.toml` & `newscatcherapi_python_sdk-6.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "newscatcherapi-python-sdk"
-version = "6.0.5"
+version = "6.0.6"
 description = "Client for NewsCatcher-V3 Production API"
 authors = ["Maksym Sugonyaka <maksym@newscatcherapi.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "newscatcherapi_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `newscatcherapi_python_sdk-6.0.5/PKG-INFO` & `newscatcherapi_python_sdk-6.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,13 @@
-Metadata-Version: 2.1
-Name: newscatcherapi-python-sdk
-Version: 6.0.5
-Summary: Client for NewsCatcher-V3 Production API
-License: MIT
-Author: Maksym Sugonyaka
-Author-email: maksym@newscatcherapi.com
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: certifi (>=2023.7.22)
-Requires-Dist: cryptography (>=42.0.5,<43.0.0)
-Requires-Dist: frozendict (>=2.3.4,<3.0.0)
-Requires-Dist: pydantic (>=2.4.2,<3.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
-Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
-Description-Content-Type: text/markdown
-
 # newscatcherapi-python-sdk<a id="newscatcherapi-python-sdk"></a>
 
 <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v6.0.5-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.5)
+[![PyPI](https://img.shields.io/badge/PyPI-v6.0.6-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.6)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/konfig-dev/newscatcher-sdks/tree/main/v3/python#readme)
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
 
 - [Requirements](#requirements)
@@ -52,27 +26,25 @@
   * [`newscatcher.search_link.post`](#newscatchersearch_linkpost)
   * [`newscatcher.search_similar.get`](#newscatchersearch_similarget)
   * [`newscatcher.search_similar.post`](#newscatchersearch_similarpost)
   * [`newscatcher.sources.get`](#newscatchersourcesget)
   * [`newscatcher.sources.post`](#newscatchersourcespost)
   * [`newscatcher.subscription.get`](#newscatchersubscriptionget)
   * [`newscatcher.subscription.post`](#newscatchersubscriptionpost)
-  * [`newscatcher.search_duplicates_by_original_id.get`](#newscatchersearch_duplicates_by_original_idget)
-  * [`newscatcher.search_duplicates_by_original_id.post`](#newscatchersearch_duplicates_by_original_idpost)
 
 <!-- tocstop -->
 
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install newscatcherapi-python-sdk==6.0.5
+pip install newscatcherapi-python-sdk==6.0.6
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from pprint import pprint
 from newscatcherapi_client import Newscatcher, ApiException
@@ -1719,82 +1691,10 @@
 
 `/api/subscription` `post`
 
 [🔙 **Back to Table of Contents**](#table-of-contents)
 
 ---
 
-### `newscatcher.search_duplicates_by_original_id.get`<a id="newscatchersearch_duplicates_by_original_idget"></a>
-
-This endpoint allows you to search for duplicate articles by original article id.
-
-#### 🛠️ Usage<a id="🛠️-usage"></a>
-
-```python
-get_response = newscatcher.search_duplicates_by_original_id.get(
-    original_article_id="original_article_id_example",
-    page=1,
-    page_size=100,
-)
-```
-
-#### ⚙️ Parameters<a id="⚙️-parameters"></a>
-
-##### original_article_id: `str`<a id="original_article_id-str"></a>
-
-##### page: `int`<a id="page-int"></a>
-
-##### page_size: `int`<a id="page_size-int"></a>
-
-#### 🔄 Return<a id="🔄-return"></a>
-
-[`SearchduplicatesbyoriginalidGetResponse`](./newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_get_response.py)
-
-#### 🌐 Endpoint<a id="🌐-endpoint"></a>
-
-`/api/search_duplicates_by_original_id` `get`
-
-[🔙 **Back to Table of Contents**](#table-of-contents)
-
----
-
-### `newscatcher.search_duplicates_by_original_id.post`<a id="newscatchersearch_duplicates_by_original_idpost"></a>
-
-This endpoint allows you to search for duplicate articles by original article id.
-
-#### 🛠️ Usage<a id="🛠️-usage"></a>
-
-```python
-post_response = newscatcher.search_duplicates_by_original_id.post(
-    original_article_id="string_example",
-    page=1,
-    page_size=100,
-)
-```
-
-#### ⚙️ Parameters<a id="⚙️-parameters"></a>
-
-##### original_article_id: `str`<a id="original_article_id-str"></a>
-
-##### page: `int`<a id="page-int"></a>
-
-##### page_size: `int`<a id="page_size-int"></a>
-
-#### ⚙️ Request Body<a id="⚙️-request-body"></a>
-
-[`DuplicatesByOriginalIdRequest`](./newscatcherapi_client/type/duplicates_by_original_id_request.py)
-#### 🔄 Return<a id="🔄-return"></a>
-
-[`SearchduplicatesbyoriginalidPostResponse`](./newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_post_response.py)
-
-#### 🌐 Endpoint<a id="🌐-endpoint"></a>
-
-`/api/search_duplicates_by_original_id` `post`
-
-[🔙 **Back to Table of Contents**](#table-of-contents)
-
----
-
 
 ## Author<a id="author"></a>
 This Python package is automatically generated by [Konfig](https://konfigthis.com)
-
```

