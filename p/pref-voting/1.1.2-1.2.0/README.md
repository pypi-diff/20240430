# Comparing `tmp/pref_voting-1.1.2.tar.gz` & `tmp/pref_voting-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-1.1.2.tar", max compression
+gzip compressed data, was "pref_voting-1.2.0.tar", max compression
```

## Comparing `pref_voting-1.1.2.tar` & `pref_voting-1.2.0.tar`

### file list

```diff
@@ -1,74 +1,76 @@
--rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.1.2/LICENSE
--rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.1.2/README.md
--rw-r--r--   0        0        0       22 2024-04-28 20:46:28.226650 pref_voting-1.1.2/pref_voting/__init__.py
--rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.1.2/pref_voting/analysis.py
--rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.1.2/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.1.2/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.1.2/pref_voting/axioms.py
--rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-1.1.2/pref_voting/c1_methods.py
--rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-1.1.2/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-1.1.2/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.1.2/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.1.2/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.1.2/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.1.2/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.1.2/pref_voting/grade_methods.py
--rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.1.2/pref_voting/grade_profiles.py
--rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-1.1.2/pref_voting/helper.py
--rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.1.2/pref_voting/invariance_axioms.py
--rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.1.2/pref_voting/io/__init__.py
--rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.1.2/pref_voting/io/readers.py
--rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.1.2/pref_voting/io/writers.py
--rw-r--r--   0        0        0    90377 2024-04-28 20:39:24.446498 pref_voting-1.1.2/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.1.2/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.1.2/pref_voting/mappings.py
--rw-r--r--   0        0        0    72109 2024-04-28 20:01:53.768039 pref_voting-1.1.2/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.1.2/pref_voting/margin_based_methods_old.py
--rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.1.2/pref_voting/monotonicity_axioms.py
--rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-1.1.2/pref_voting/other_methods.py
--rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.1.2/pref_voting/prob_voting_method.py
--rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.1.2/pref_voting/probabilistic_methods.py
--rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-1.1.2/pref_voting/profiles.py
--rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.1.2/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.1.2/pref_voting/rankings.py
--rw-r--r--   0        0        0    21026 2024-04-09 02:00:24.744126 pref_voting-1.1.2/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.1.2/pref_voting/social_welfare_function.py
--rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.1.2/pref_voting/social_welfare_functions.py
--rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.1.2/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0    15790 2024-04-24 21:18:21.291486 pref_voting-1.1.2/pref_voting/strategic_axioms.py
--rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.1.2/pref_voting/tests/__init__.py
--rw-r--r--   0        0        0      745 2024-04-28 20:04:29.865701 pref_voting-1.1.2/pref_voting/tests/conftest.py
--rw-r--r--   0        0        0     5690 2024-04-28 20:01:53.768645 pref_voting-1.1.2/pref_voting/tests/test_c1_methods.py
--rw-r--r--   0        0        0     3092 2024-04-28 20:01:53.768816 pref_voting-1.1.2/pref_voting/tests/test_combined_methods.py
--rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.1.2/pref_voting/tests/test_generate_profiles.py
--rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.1.2/pref_voting/tests/test_generate_spatial_profile.py
--rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.1.2/pref_voting/tests/test_io.py
--rw-r--r--   0        0        0    11606 2024-04-28 20:41:27.682198 pref_voting-1.1.2/pref_voting/tests/test_iterative_methods.py
--rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.1.2/pref_voting/tests/test_majority_graph.py
--rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.1.2/pref_voting/tests/test_mapping.py
--rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.1.2/pref_voting/tests/test_margin_based_methods.py
--rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.1.2/pref_voting/tests/test_margin_graph.py
--rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.1.2/pref_voting/tests/test_other_methods.py
--rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.1.2/pref_voting/tests/test_prob_voting_method.py
--rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.1.2/pref_voting/tests/test_profile.py
--rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.1.2/pref_voting/tests/test_profile_with_ties.py
--rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.1.2/pref_voting/tests/test_ranking.py
--rw-r--r--   0        0        0     6234 2024-04-28 20:40:55.278187 pref_voting-1.1.2/pref_voting/tests/test_scoring_rules.py
--rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.1.2/pref_voting/tests/test_social_welfare_functions.py
--rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.1.2/pref_voting/tests/test_spatial_profile.py
--rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.1.2/pref_voting/tests/test_support_graph.py
--rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.1.2/pref_voting/tests/test_utility_function.py
--rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.1.2/pref_voting/tests/test_utility_functions.py
--rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.1.2/pref_voting/tests/test_voting_method.py
--rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.1.2/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.1.2/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.1.2/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.1.2/pref_voting/variable_candidate_axioms.py
--rw-r--r--   0        0        0    91126 2024-04-28 20:01:53.769602 pref_voting-1.1.2/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-1.1.2/pref_voting/voting_method.py
--rw-r--r--   0        0        0      863 2024-04-28 20:41:05.991631 pref_voting-1.1.2/pref_voting/voting_method_properties.py
--rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-1.1.2/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.1.2/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      760 2024-04-28 20:46:28.225281 pref_voting-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.1.2/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.2.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-30 01:55:59.429329 pref_voting-1.2.0/pref_voting/__init__.py
+-rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.2.0/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.2.0/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.2.0/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.2.0/pref_voting/axioms.py
+-rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-1.2.0/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-1.2.0/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    12827 2024-04-30 00:43:54.579498 pref_voting-1.2.0/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.2.0/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.2.0/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.2.0/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.2.0/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.2.0/pref_voting/grade_methods.py
+-rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.2.0/pref_voting/grade_profiles.py
+-rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-1.2.0/pref_voting/helper.py
+-rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.2.0/pref_voting/invariance_axioms.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.2.0/pref_voting/io/__init__.py
+-rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.2.0/pref_voting/io/readers.py
+-rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.2.0/pref_voting/io/writers.py
+-rw-r--r--   0        0        0    93528 2024-04-30 00:49:36.509648 pref_voting-1.2.0/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.2.0/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.2.0/pref_voting/mappings.py
+-rw-r--r--   0        0        0    72109 2024-04-28 20:01:53.768039 pref_voting-1.2.0/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.2.0/pref_voting/margin_based_methods_old.py
+-rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.2.0/pref_voting/monotonicity_axioms.py
+-rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-1.2.0/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.2.0/pref_voting/prob_voting_method.py
+-rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.2.0/pref_voting/probabilistic_methods.py
+-rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-1.2.0/pref_voting/profiles.py
+-rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.2.0/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.2.0/pref_voting/rankings.py
+-rw-r--r--   0        0        0    22528 2024-04-30 01:19:53.430327 pref_voting-1.2.0/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.2.0/pref_voting/social_welfare_function.py
+-rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.2.0/pref_voting/social_welfare_functions.py
+-rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.2.0/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0    15790 2024-04-30 00:43:41.503635 pref_voting-1.2.0/pref_voting/strategic_axioms.py
+-rw-r--r--   0        0        0     7833 2024-04-30 00:43:41.503770 pref_voting-1.2.0/pref_voting/swf_axioms.py
+-rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.2.0/pref_voting/tests/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-28 20:04:29.865701 pref_voting-1.2.0/pref_voting/tests/conftest.py
+-rw-r--r--   0        0        0     5690 2024-04-28 20:01:53.768645 pref_voting-1.2.0/pref_voting/tests/test_c1_methods.py
+-rw-r--r--   0        0        0     3092 2024-04-28 20:01:53.768816 pref_voting-1.2.0/pref_voting/tests/test_combined_methods.py
+-rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.2.0/pref_voting/tests/test_generate_profiles.py
+-rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.2.0/pref_voting/tests/test_generate_spatial_profile.py
+-rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.2.0/pref_voting/tests/test_io.py
+-rw-r--r--   0        0        0    11606 2024-04-28 20:41:27.682198 pref_voting-1.2.0/pref_voting/tests/test_iterative_methods.py
+-rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.2.0/pref_voting/tests/test_majority_graph.py
+-rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.2.0/pref_voting/tests/test_mapping.py
+-rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.2.0/pref_voting/tests/test_margin_based_methods.py
+-rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.2.0/pref_voting/tests/test_margin_graph.py
+-rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.2.0/pref_voting/tests/test_other_methods.py
+-rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.2.0/pref_voting/tests/test_prob_voting_method.py
+-rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.2.0/pref_voting/tests/test_profile.py
+-rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.2.0/pref_voting/tests/test_profile_with_ties.py
+-rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.2.0/pref_voting/tests/test_ranking.py
+-rw-r--r--   0        0        0     6234 2024-04-28 20:40:55.278187 pref_voting-1.2.0/pref_voting/tests/test_scoring_rules.py
+-rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.2.0/pref_voting/tests/test_social_welfare_functions.py
+-rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.2.0/pref_voting/tests/test_spatial_profile.py
+-rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.2.0/pref_voting/tests/test_support_graph.py
+-rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.2.0/pref_voting/tests/test_utility_function.py
+-rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.2.0/pref_voting/tests/test_utility_functions.py
+-rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.2.0/pref_voting/tests/test_voting_method.py
+-rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.2.0/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.2.0/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.2.0/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.2.0/pref_voting/variable_candidate_axioms.py
+-rw-r--r--   0        0        0    91126 2024-04-28 20:01:53.769602 pref_voting-1.2.0/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     6148 2024-04-30 01:20:56.462342 pref_voting-1.2.0/pref_voting/voting_method.py
+-rw-r--r--   0        0        0     1341 2024-04-30 00:59:45.610622 pref_voting-1.2.0/pref_voting/voting_method_properties.py
+-rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-1.2.0/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0     2563 2024-04-30 01:26:13.410155 pref_voting-1.2.0/pref_voting/voting_methods_registry.py
+-rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.2.0/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      760 2024-04-30 01:55:59.427023 pref_voting-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.2.0/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.2.0/PKG-INFO
```

### Comparing `pref_voting-1.1.2/LICENSE` & `pref_voting-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/README.md` & `pref_voting-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/analysis.py` & `pref_voting-1.2.0/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/axiom.py` & `pref_voting-1.2.0/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/c1_methods.py` & `pref_voting-1.2.0/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/combined_methods.py` & `pref_voting-1.2.0/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/dominance_axioms.py` & `pref_voting-1.2.0/pref_voting/dominance_axioms.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from pref_voting.axiom import Axiom
 from pref_voting.c1_methods import smith_set, schwartz_set
 from pref_voting.axiom_helpers import *
 
 
-def has_pareto_violation(edata, vm, verbose=False, strong_Pareto = False):
+def has_pareto_dominance_violation(edata, vm, verbose=False, strong_Pareto = False):
     """
     Returns True if some winner according to vm is Pareto dominated (there is a candidate that is unanimously preferred to the winner).
 
     If strong_Pareto is True, then a candidate A is dominated if there is a candidate B such that some voter prefers B to A and no voter prefers A to B.
     
     Args:
         edata (Profile, ProfileWithTies): the election data.
@@ -28,23 +28,24 @@
     """
 
     ws = vm(edata)
     for w in ws: 
         for c in edata.candidates: 
             if (strong_Pareto == False and edata.support(c,w)==edata.num_voters) or (strong_Pareto == True and edata.support(c,w)> 0 and edata.support(w,c)==0):
                 if verbose:  
+                    print(f"Pareto violation by {vm}:")
                     edata.display()
                     print(edata.description())
                     vm.display(edata)
-                    print(f"The winner {w} is Pareto dominated by {c}. ")
+                    print(f"The winner {w} is Pareto dominated by {c}.")
                     print()
                 return True
     return False
 
-def find_all_pareto_violations(edata, vm, verbose=False, strong_Pareto = False):
+def find_all_pareto_dominance_violations(edata, vm, verbose=False, strong_Pareto = False):
     """
     Returns all Pareto-dominated winners.
 
     If strong_Pareto is True, then a candidate A is dominated if there is a candidate B such that some voter prefers B to A and no voter prefers A to B.
     
     Args:
         edata (Profile, ProfileWithTies): the election data.
@@ -60,26 +61,27 @@
     pareto_dominated_winners = list()
     for w in ws: 
         for c in edata.candidates: 
             if (strong_Pareto == False and edata.support(c,w)==edata.num_voters) or (strong_Pareto == True and edata.support(c,w)> 0 and edata.support(w,c)==0):
                 pareto_dominated_winners.append((w, c))
     
     if len(pareto_dominated_winners) > 0 and verbose: 
+        print(f"Pareto violation by {vm}:")
         edata.display()
         print(edata.description())
         vm.display(edata)
         for w,c in pareto_dominated_winners:
-            print(f"The winner {w} is Pareto dominated by {c}. ")
+            print(f"The winner {w} is Pareto dominated by {c}.")
 
     return pareto_dominated_winners
 
-pareto = Axiom(
-    "Pareto Criterion",
-    has_violation = has_pareto_violation,
-    find_all_violations = find_all_pareto_violations, 
+pareto_dominance = Axiom(
+    "Pareto Dominance Criterion",
+    has_violation = has_pareto_dominance_violation,
+    find_all_violations = find_all_pareto_dominance_violations, 
 )
 
 def has_condorcet_winner_violation(edata, vm, verbose=False):
     """
     Returns True if there is a Condorcet winner in edata (a candidate that is majority preferred to every other candidate) that is not the unique winner according to vm.
     
     Args:
@@ -336,13 +338,13 @@
 schwartz = Axiom(
     "Schwartz",
     has_violation = has_schwartz_violation,
     find_all_violations = find_all_schwartz_violations, 
 )
 
 dominance_axioms = [
-    pareto, 
+    pareto_dominance, 
     condorcet_winner, 
     condorcet_loser,
     smith,
     schwartz
 ]
```

### Comparing `pref_voting-1.1.2/pref_voting/generate_profiles.py` & `pref_voting-1.2.0/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/generate_spatial_profiles.py` & `pref_voting-1.2.0/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/generate_utility_profiles.py` & `pref_voting-1.2.0/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-1.2.0/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/grade_methods.py` & `pref_voting-1.2.0/pref_voting/grade_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/grade_profiles.py` & `pref_voting-1.2.0/pref_voting/grade_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/helper.py` & `pref_voting-1.2.0/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/invariance_axioms.py` & `pref_voting-1.2.0/pref_voting/invariance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/io/readers.py` & `pref_voting-1.2.0/pref_voting/io/readers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/io/writers.py` & `pref_voting-1.2.0/pref_voting/io/writers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/iterative_methods.py` & `pref_voting-1.2.0/pref_voting/iterative_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,31 +7,80 @@
     Implementations of iterative voting methods.
 '''
 from pref_voting.voting_method import  *
 from pref_voting.voting_method import _num_rank_last, _num_rank_first
 from pref_voting.profiles import  _borda_score, _find_updated_profile
 from pref_voting.margin_based_methods import split_cycle, minimax_scores
 from pref_voting.c1_methods import top_cycle, gocha
-
+from pref_voting.rankings import Ranking
+from pref_voting.social_welfare_function import swf
 import copy
 from itertools import permutations, product
 import numpy as np
 
+def _instant_runoff_basic(profile,curr_cands = None):
+    "The basic implementation of instant runoff"
+    # need the total number of all candidates in a profile to check when all candidates have been removed   
+    num_cands = profile.num_cands 
+    
+    candidates = profile.candidates if curr_cands is None else curr_cands
+    cands_to_ignore = np.empty(0) if curr_cands is None else np.array([c for c in profile.candidates if c not in curr_cands])
+
+    strict_maj_size = profile.strict_maj_size()
+    
+    rs, rcounts = profile.rankings_counts # get all the ranking data
+
+    winners = [c for c in candidates 
+               if _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
+
+    while len(winners) == 0:
+        plurality_scores = {c: _num_rank_first(rs, rcounts, cands_to_ignore, c) for c in candidates 
+                            if  not isin(cands_to_ignore,c)}  
+        min_plurality_score = min(plurality_scores.values())
+        lowest_first_place_votes = np.array([c for c in plurality_scores.keys() 
+                                             if  plurality_scores[c] == min_plurality_score])
+
+        # remove cands with lowest plurality score
+        cands_to_ignore = np.concatenate((cands_to_ignore, lowest_first_place_votes), axis=None)
+        if len(cands_to_ignore) == num_cands: # removed all of the candidates 
+            winners = sorted(lowest_first_place_votes)
+        else:
+            winners = [c for c in candidates 
+                       if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
+     
+    return sorted(winners)
+
+def _instant_runoff_recursive(profile, curr_cands = None):
+    "A recursive implementation of instant runoff"
+    candidates = curr_cands if curr_cands is not None else profile.candidates
+    cands_to_ignore = np.array([c for c in profile.candidates if c not in candidates])
+    rs, rcounts = profile.rankings_counts # get all the ranking data
+    plurality_scores = {c: _num_rank_first(rs, rcounts, cands_to_ignore, c) for c in candidates if not isin(cands_to_ignore,c)}  
+    min_plurality_score = min(plurality_scores.values())
+    lowest_first_place_votes = np.array([c for c in plurality_scores.keys() 
+                                            if  plurality_scores[c] == min_plurality_score])
+
+    if len(lowest_first_place_votes) == len(candidates):
+        return sorted(lowest_first_place_votes)
+    
+    else:
+        return _instant_runoff_recursive(profile, [c for c in candidates if c not in lowest_first_place_votes])
+
 @vm(name = "Instant Runoff")
-def instant_runoff(profile, curr_cands = None):
+def instant_runoff(profile, curr_cands = None, algorithm = "basic"):
     """
-    If there is a majority winner then that candidate is the  winner.  If there is no majority winner, then remove all candidates that are ranked first by the fewest number of voters.  Continue removing candidates with the fewest number first-place votes until there is a candidate with a majority of first place votes.  
+    If there is a majority winner then that candidate is the winner. If there is no majority winner, then remove all candidates that are ranked first by the fewest number of voters. Continue removing candidates with the fewest number first-place votes until there is a candidate with a majority of first place votes.  
     
     .. important::
-        If there is  more than one candidate with the fewest number of first-place votes, then *all* such candidates are removed from the profile. 
+        If there is more than one candidate with the fewest number of first-place votes, then *all* such candidates are removed from the profile. 
     
-
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
+        algorithm (str, optiona): The algorithm to use.  Options are "basic" and "recursive".  The default is "basic".
 
     Returns: 
         A sorted list of candidates
 
     .. seealso::
 
         Instant Runoff is also known as "Ranked Choice", "Hare", and "Alternative Vote".
@@ -51,56 +100,66 @@
         instant_runoff.display(prof)
         ranked_choice.display(prof)
         alternative_vote.display(prof)
         hare.display(prof)
 
     """
 
-    # need the total number of all candidates in a profile to check when all candidates have been removed   
-    num_cands = profile.num_cands 
+    if algorithm == "basic":
+        return _instant_runoff_basic(profile, curr_cands = curr_cands)
     
-    candidates = profile.candidates if curr_cands is None else curr_cands
-    cands_to_ignore = np.empty(0) if curr_cands is None else np.array([c for c in profile.candidates if c not in curr_cands])
-
-    strict_maj_size = profile.strict_maj_size()
-    
-    rs, rcounts = profile.rankings_counts # get all the ranking data
+    elif algorithm == "recursive":
+        return _instant_runoff_recursive(profile, curr_cands = curr_cands)
     
-
-    winners = [c for c in candidates 
-               if _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
-
-    while len(winners) == 0:
-        plurality_scores = {c: _num_rank_first(rs, rcounts, cands_to_ignore, c) for c in candidates 
-                            if  not isin(cands_to_ignore,c)}  
-        min_plurality_score = min(plurality_scores.values())
-        lowest_first_place_votes = np.array([c for c in plurality_scores.keys() 
-                                             if  plurality_scores[c] == min_plurality_score])
-
-        # remove cands with lowest plurality score
-        cands_to_ignore = np.concatenate((cands_to_ignore, lowest_first_place_votes), axis=None)
-        if len(cands_to_ignore) == num_cands: # removed all of the candidates 
-            winners = sorted(lowest_first_place_votes)
-        else:
-            winners = [c for c in candidates 
-                       if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
-     
-    return sorted(winners)
+    else:
+        raise ValueError("Algorithm must be either 'basic' or 'recursive'.")
 
 # Create some aliases for instant runoff
 instant_runoff.set_name("Hare")
 hare = copy.deepcopy(instant_runoff)
 instant_runoff.set_name("Ranked Choice")
 ranked_choice = copy.deepcopy(instant_runoff)
 instant_runoff.set_name("Alternative Vote")
 alternative_vote = copy.deepcopy(instant_runoff)
 
 # reset the name Instant Runoff
 instant_runoff.set_name("Instant Runoff")
 
+@swf(name = "Instant Runoff Ranking")
+def instant_runoff_ranking(profile, curr_cands = None):
+    """Returns the reverse of the elimination order in the instant runoff voting process.
+
+    Args:
+        profile (Profile): An anonymous Profile of linear orders on a set of candidates
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
+
+    Returns:
+        A Ranking of the candidates.
+    """
+    
+    candidates = curr_cands if curr_cands is not None else profile.candidates
+    cands_to_ignore = np.array([c for c in profile.candidates if c not in candidates])
+    rs, rcounts = profile.rankings_counts # get all the ranking data
+    plurality_scores = {c: _num_rank_first(rs, rcounts, cands_to_ignore, c) for c in candidates if not isin(cands_to_ignore,c)}  
+    min_plurality_score = min(plurality_scores.values())
+    lowest_first_place_votes = np.array([c for c in plurality_scores.keys() 
+                                            if  plurality_scores[c] == min_plurality_score])
+    
+    if len(lowest_first_place_votes) == len(candidates):
+        full_tie = Ranking({c:0 for c in candidates})
+        return full_tie
+    
+    else:
+        rec_ranking = instant_runoff_ranking(profile, [c for c in candidates if c not in lowest_first_place_votes])
+        max_rank = max(rec_ranking.ranks)
+        rec_ranking_dict = rec_ranking.rmap
+        ranking = Ranking({c: rec_ranking_dict[c] if not isin(lowest_first_place_votes,c) else max_rank+1 for c in candidates})
+
+        return ranking
+
 @vm(name = "Instant Runoff TB")
 def instant_runoff_tb(profile, curr_cands = None, tie_breaker = None):
     """Instant Runoff (``instant_runoff``) with tie breaking:  If there is  more than one candidate with the fewest number of first-place votes, then remove the candidate with lowest in the tie_breaker ranking from the profile.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
```

### Comparing `pref_voting-1.1.2/pref_voting/maj_graph_ex1.png` & `pref_voting-1.2.0/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/mappings.py` & `pref_voting-1.2.0/pref_voting/mappings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/margin_based_methods.py` & `pref_voting-1.2.0/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/margin_based_methods_old.py` & `pref_voting-1.2.0/pref_voting/margin_based_methods_old.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/monotonicity_axioms.py` & `pref_voting-1.2.0/pref_voting/monotonicity_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/other_methods.py` & `pref_voting-1.2.0/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/prob_voting_method.py` & `pref_voting-1.2.0/pref_voting/prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/probabilistic_methods.py` & `pref_voting-1.2.0/pref_voting/probabilistic_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/profiles.py` & `pref_voting-1.2.0/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/profiles_with_ties.py` & `pref_voting-1.2.0/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/rankings.py` & `pref_voting-1.2.0/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/scoring_methods.py` & `pref_voting-1.2.0/pref_voting/scoring_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,25 @@
 '''
 from pref_voting.voting_method import  *
 from pref_voting.social_welfare_function import  *
 from pref_voting.profiles import Profile
 from pref_voting.rankings import Ranking, break_ties_alphabetically
 from pref_voting.voting_method import _num_rank_last 
 from pref_voting.profiles import _find_updated_profile, _num_rank
+from pref_voting.voting_method_properties import VotingMethodProperties, ElectionTypes
 
-@vm(name = "Plurality")
+pl_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=False,
+    pareto_dominance=False, 
+    )
+@vm(name = "Plurality", 
+    properties=pl_properties, 
+    input_types=[ElectionTypes.PROFILE, 
+                 ElectionTypes.TRUNCATED_LINEAR_PROFILE])
 def plurality(profile, curr_cands = None):
     """The **Plurality score** of a candidate :math:`c` is the number of voters that rank :math:`c` in first place. The Plurality winners are the candidates with the largest Plurality score in the ``profile`` restricted to ``curr_cands``.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -90,15 +99,22 @@
     p_ranking.normalize_ranks()
 
     if tie_breaking == "alphabetic":
         p_ranking = break_ties_alphabetically(p_ranking)
 
     return p_ranking
 
-@vm(name = "Borda")
+borda_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=True,
+    pareto_dominance=True, 
+    )
+@vm(name = "Borda",
+    properties=borda_properties,
+    input_types=[ElectionTypes.PROFILE])
 def borda(profile, curr_cands = None):
     r"""The **Borda score** of a candidate is calculated as follows: If there are :math:`m` candidates, then the Borda score of candidate :math:`c` is :math:`\sum_{r=1}^{m} (m - r) * Rank(c,r)` where :math:`Rank(c,r)` is the number of voters that rank candidate :math:`c` in position :math:`r`. The Borda winners are the candidates with the largest Borda score in the ``profile`` restricted to ``curr_cands``. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -167,15 +183,22 @@
     b_ranking.normalize_ranks()
 
     if tie_breaking == "alphabetic":
         b_ranking = break_ties_alphabetically(b_ranking)
 
     return b_ranking
 
-@vm(name = "Anti-Plurality")
+anti_plurality_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=False,
+    pareto_dominance=False, 
+    )
+@vm(name = "Anti-Plurality",
+    properties=anti_plurality_properties,
+    input_types=[ElectionTypes.PROFILE])
 def anti_plurality(profile, curr_cands = None):
     """The **Anti-Plurality score** of a candidate $c$ is the number of voters that rank $c$ in last place.  The Anti-Plurality winners are the candidates with the smallest Anti-Plurality score in the ``profile`` restricted to ``curr_cands``. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -243,15 +266,16 @@
 
     if tie_breaking == "alphabetic":
         ap_ranking = break_ties_alphabetically(ap_ranking)
 
     return ap_ranking
 
 
-@vm(name = "Scoring Rule")
+@vm(name = "Scoring Rule",
+    skip_registration=True,)
 def scoring_rule(profile, curr_cands = None, score = lambda num_cands, rank : 1 if rank == 1 else 0):
     """A general scoring rule.  Each voter assign a score to each candidate using the ``score`` function based on their submitted ranking (restricted to candidates in ``curr_cands``).   Returns that candidates with the greatest overall score in the profile restricted to ``curr_cands``. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
         score (function): A function that accepts two parameters ``num_cands`` (the number of candidates) and ``rank`` (a rank of a candidate) used to calculate the score of a candidate.   The default ``score`` function assigns 1 to a candidate ranked in first place, otherwise it assigns 0 to the candidate. 
@@ -305,15 +329,22 @@
     """Create a scoring method using a given score function and name."""
 
     def _vm(profile, curr_cands = None):
         return scoring_rule(profile, curr_cands = curr_cands, score = score)
 
     return VotingMethod(_vm, name = name)
 
-@vm(name = "Dowdall")
+dowdal_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=False,
+    pareto_dominance=True, 
+    )
+@vm(name = "Dowdall",
+    properties=dowdal_properties,
+    input_types=[ElectionTypes.PROFILE])
 def dowdall(profile, curr_cands = None):
     """The first-ranked candidate gets 1 point, the second-ranked candidate gets 1/2 point, the third-ranked candidate gets 1/3 point, and so on.  The Dowdall winners are the candidates with the greatest overall score in the profile restricted to ``curr_cands``.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``.
 
@@ -323,15 +354,22 @@
     .. note::
         This system is used in Nauru. See, e.g., Jon Fraenkel & Bernard Grofman (2014), "The Borda Count and its real-world alternatives: Comparing scoring rules in Nauru and Slovenia," Australian Journal of Political Science, 49:2, 186-205, DOI: 10.1080/10361146.2014.900530.
     
     """
 
     return scoring_rule(profile, curr_cands = curr_cands, score = lambda num_cands, rank: 1 / rank)
 
-@vm("Positive-Negative Voting")
+pos_neg_voting_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=False,
+    pareto_dominance=False, 
+    )
+@vm(name="Positive-Negative Voting",
+    properties=pos_neg_voting_properties,
+    input_types=[ElectionTypes.PROFILE])
 def positive_negative_voting(profile, curr_cands = None):
     """The **Positive-Negative Voting** method is a scoring rule where each voter assigns a score of 1 to their top-ranked candidate and a score of -1 to their bottom-ranked candidate.  See https://onlinelibrary.wiley.com/doi/10.1111/ecin.12929 for more information.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -424,15 +462,22 @@
 
     """
     
     return  {cand: -sum([len([_cand for _cand in profile.candidates if r.extended_strict_pref(_cand, cand)]) * c 
                     for r,c in zip(*profile.rankings_counts)]) for cand in profile.candidates}
 
 
-@vm(name="Borda")
+borda_prof_with_ties_properties = VotingMethodProperties(
+    condorcet_winner=None, 
+    condorcet_loser=None,
+    pareto_dominance=None, 
+    )
+@vm(name="Borda",
+    properties=borda_prof_with_ties_properties,
+    input_types=[ElectionTypes.TRUNCATED_LINEAR_PROFILE])
 def borda_for_profile_with_ties(
     profile, 
     curr_cands=None, 
     borda_scores=symmetric_borda_scores): 
     """
     Borda score for truncated linear orders using different ways of defining the Borda score for truncated linear
     orders.
```

### Comparing `pref_voting-1.1.2/pref_voting/social_welfare_function.py` & `pref_voting-1.2.0/pref_voting/social_welfare_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/spatial_profiles.py` & `pref_voting-1.2.0/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/strategic_axioms.py` & `pref_voting-1.2.0/pref_voting/strategic_axioms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     File: strategic_axioms.py
     Author: Wesley H. Holliday (wesholliday@berkeley.edu) and Eric Pacuit (epacuit@umd.edu)
-    Date: April 18, 2023
+    Date: April 18, 2024
     
     Strategic axioms 
 """
 
 from pref_voting.axiom import Axiom
 from pref_voting.axiom_helpers import *
 from itertools import permutations
```

### Comparing `pref_voting-1.1.2/pref_voting/tests/conftest.py` & `pref_voting-1.2.0/pref_voting/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_c1_methods.py` & `pref_voting-1.2.0/pref_voting/tests/test_c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_combined_methods.py` & `pref_voting-1.2.0/pref_voting/tests/test_combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_generate_profiles.py` & `pref_voting-1.2.0/pref_voting/tests/test_generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_generate_spatial_profile.py` & `pref_voting-1.2.0/pref_voting/tests/test_generate_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_io.py` & `pref_voting-1.2.0/pref_voting/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_iterative_methods.py` & `pref_voting-1.2.0/pref_voting/tests/test_iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_majority_graph.py` & `pref_voting-1.2.0/pref_voting/tests/test_majority_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_mapping.py` & `pref_voting-1.2.0/pref_voting/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_margin_based_methods.py` & `pref_voting-1.2.0/pref_voting/tests/test_margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_margin_graph.py` & `pref_voting-1.2.0/pref_voting/tests/test_margin_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_other_methods.py` & `pref_voting-1.2.0/pref_voting/tests/test_other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_prob_voting_method.py` & `pref_voting-1.2.0/pref_voting/tests/test_prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_profile.py` & `pref_voting-1.2.0/pref_voting/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_profile_with_ties.py` & `pref_voting-1.2.0/pref_voting/tests/test_profile_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_ranking.py` & `pref_voting-1.2.0/pref_voting/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_scoring_rules.py` & `pref_voting-1.2.0/pref_voting/tests/test_scoring_rules.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_social_welfare_functions.py` & `pref_voting-1.2.0/pref_voting/tests/test_social_welfare_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_spatial_profile.py` & `pref_voting-1.2.0/pref_voting/tests/test_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_support_graph.py` & `pref_voting-1.2.0/pref_voting/tests/test_support_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_utility_function.py` & `pref_voting-1.2.0/pref_voting/tests/test_utility_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_utility_functions.py` & `pref_voting-1.2.0/pref_voting/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/tests/test_voting_method.py` & `pref_voting-1.2.0/pref_voting/tests/test_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/utility_functions.py` & `pref_voting-1.2.0/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/utility_methods.py` & `pref_voting-1.2.0/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/utility_profiles.py` & `pref_voting-1.2.0/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/variable_candidate_axioms.py` & `pref_voting-1.2.0/pref_voting/variable_candidate_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/variable_voter_axioms.py` & `pref_voting-1.2.0/pref_voting/variable_voter_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pref_voting/voting_method.py` & `pref_voting-1.2.0/pref_voting/voting_method.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,20 +15,30 @@
 class VotingMethod(object): 
     """
     A class to add functionality to voting methods. 
 
     Args:
         vm (function): An implementation of a voting method. The function should accept a Profile, ProfileWithTies, MajorityGraph, and/or MarginGraph, and a keyword parameter ``curr_cands`` to find the winner after restricting to ``curr_cands``. 
         name (string): The Human-readable name of the voting method.
+        properties (VotingMethodProperties): The properties of the voting method.
+        input_types (list): The types of input that the voting method can accept.
 
     """
-    def __init__(self, vm, name = None): 
+    def __init__(self, 
+                 vm, 
+                 name=None, 
+                 properties=None, 
+                 input_types=None, 
+                 skip_registration=False): 
         
         self.vm = vm
         self.name = name
+        self.properties = properties
+        self.input_types = input_types
+        self.skip_registration = skip_registration
         functools.update_wrapper(self, vm)   
 
     def __call__(self, edata, curr_cands = None, **kwargs):
 
         if (curr_cands is not None and len(curr_cands) == 0) or len(edata.candidates) == 0: 
             return []
         return self.vm(edata, curr_cands = curr_cands, **kwargs)
@@ -68,20 +78,20 @@
         """Set the name of the voting method."""
 
         self.name = new_name
 
     def __str__(self): 
         return f"{self.name}"
 
-def vm(name = None):
+def vm(name=None, properties=None, input_types=None, skip_registration=False):
     """
     A decorator used when creating a voting method. 
     """
     def wrapper(f):
-        return VotingMethod(f, name=name)
+        return VotingMethod(f, name=name, properties=properties, input_types=input_types, skip_registration=skip_registration)
     return wrapper
 
 @jit(nopython=True, fastmath=True)
 def isin(arr, val):
     """compiled function testing if the value val is in the array arr
     """
```

### Comparing `pref_voting-1.1.2/pref_voting/weighted_majority_graphs.py` & `pref_voting-1.2.0/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.2/pyproject.toml` & `pref_voting-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "1.1.2"
+version = "1.2.0"
 description = "pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-1.1.2/setup.py` & `pref_voting-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prefsampling>=0.1.16,<0.2.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '1.1.2',
+    'version': '1.2.0',
     'description': 'pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.',
     'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n\n## Documentation\n\nOnline documentation is available at [https://pref-voting.readthedocs.io](https://pref-voting.readthedocs.io).\n\n## Example Usage\n\nA profile (of linear orders over the candidates) is created by initializing a `Profile` class object.  Simply provide a list of rankings (each ranking is a tuple of numbers) and a list giving the number of voters with each ranking:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [\n    (0, 1, 2, 3), \n    (2, 3, 1, 0), \n    (3, 1, 2, 0), \n    (1, 2, 0, 3), \n    (1, 3, 2, 0)]\n\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function `generate_profile` is used to generate a profile for a given number of candidates and voters:  \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\nTo use one of the many voting methods, import the function from `pref_voting.voting_methods` and apply it to the profile: \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\nfrom pref_voting.voting_methods import *\n\nprof = generate_profile(3, 4)\nsplit_cycle(prof) # returns the sorted list of winning candidates\nsplit_cycle.display(prof) # display the winning candidates\n\n```\n\n## Questions?\n\nFeel free to [send an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
```

### Comparing `pref_voting-1.1.2/PKG-INFO` & `pref_voting-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 1.1.2
+Version: 1.2.0
 Summary: pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

