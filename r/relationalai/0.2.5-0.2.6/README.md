# Comparing `tmp/relationalai-0.2.5.tar.gz` & `tmp/relationalai-0.2.6.tar.gz`

## Comparing `relationalai-0.2.5.tar` & `relationalai-0.2.6.tar`

### file list

```diff
@@ -1,449 +1,512 @@
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.5/README.md
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 relationalai-0.2.5/.github/actions/end-to-end/action.yml
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 relationalai-0.2.5/.github/workflows/end-to-end.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 relationalai-0.2.5/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/README.md
--rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/_old/quickstart.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/README.md
--rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/configuration/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Property.md
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/README.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/enter__.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/exit__.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/iter__.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/model.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Context/results.md
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/ContextSelect/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/ContextSelect/add.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/ContextSelect/call__.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/ContextSelect/getattribute__.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Instance/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Instance/persist.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Instance/set.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Instance/unpersist.md
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/InstanceProperty/README.md
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/InstanceProperty/or_.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/Type.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/found.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/name.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/not_found.md
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/ordered_choice.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/query.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/read.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/rule.md
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/scope.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Model/union.md
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/add__.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/enter__.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/eq__.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/exit__.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/ge__.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/getattribute__.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/gt__.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/le__.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/lt__.md
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/mul__.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/ne__.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/pow__.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/radd__.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/rmul__.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/rpow__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/rsub__.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/rtruediv__.md
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/sub__.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Producer/truediv__.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/README.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/add.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/call__.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/extend.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/model.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/name.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/Type/or__.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/PrimaryKey.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/Snowflake.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/Vars.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/alias.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/avg.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/count.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/max.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/min.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/rank_asc.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/rank_desc.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/aggregates/sum.md
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/README.md
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/README.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_degree.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/degree.md
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/indegree.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/infomap.md
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/is_connected.md
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/is_reachable.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/label_propagation.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/louvain.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/num_edges.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/num_nodes.md
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/outdegree.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/pagerank.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/reachable_from.md
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/README.md
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/add.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/call__.md
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/extend.md
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/set.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/to.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/Edge.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/Node.md
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/README.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/compute.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/fetch.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/id.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/model.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/undirected.md
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/visualize.md
--rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
--rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/README.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/concat.md
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/contains.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/ends_with.md
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/join.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/length.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/lowercase.md
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/replace.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/python/std/strings/uppercase.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/faq/README.md
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/faq/engines.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/cdc.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/custom_snowflake_connection.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/fraud.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/graph_algos.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/load_raw.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/nested.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/or_types.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/remote_load_csv.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/requirements.txt
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/simple_recursion.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/solver.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/weighted_graph_algos.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/README.md
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/articles_graph.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/articles_graph_with_nlp.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/pyproject.toml
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/utils.py
--rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/articles_graph/daily_articles/04_04_2024.json
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/data/transactions.csv
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/ev_penetration/ev_penetration.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/ev_penetration/ev_penetration_csv.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/ev_penetration/state_stats.csv
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/imdb/README.md
--rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/imdb/imdb.csv
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/imdb/imdb.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/rel/foo.rel
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/rel/solver.rel
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/social-money-network/SF_pagerank.ipynb
--rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/social-money-network/Simulation-and-SF-Upload.ipynb
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.5/examples/social-money-network/snowflake_pagerank.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/README.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/index.html
--rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/package-lock.json
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/package.json
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/tsconfig.json
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/vite.config.ts
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/.storybook/main.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/.storybook/preview-body.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/.storybook/preview-head.html
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/.storybook/preview.ts
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/App.styl
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/App.tsx
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/Selection.tsx
--rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/debugger_client.ts
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/index.css
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/index.tsx
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/logo.svg
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/util.styl
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/util.ts
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/ws.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/assets/favicon.png
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/EventList.styl
--rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/EventList.tsx
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/EventViewer.styl
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/EventViewer.tsx
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Sidebar.styl
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Sidebar.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.stories.tsx
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.styl
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.tsx
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/base.styl
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/base.tsx
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/index.tsx
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Accordion.stories.tsx
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Accordion.styl
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Accordion.tsx
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Button.styl
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Button.tsx
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Code.styl
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Code.tsx
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.stories.tsx
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.styl
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.tsx
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Field.stories.tsx
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Field.styl
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Field.tsx
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Icon.styl
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Icon.tsx
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.stories.tsx
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.styl
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.tsx
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.stories.tsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.styl
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.tsx
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/branch-improved.json
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/branch.json
--rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/fraud.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/index.ts
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/not_found.json
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/simple.json
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/fixtures/union.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/types/json.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/types/jsx.d.ts
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.5/frontend/debugger/src/types/mech.d.ts
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/__init__.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/emit.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/compiler.py
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/debugging.py
--rw-r--r--   0        0        0    45835 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/dsl.py
--rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/errors.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/metagen.py
--rw-r--r--   0        0        0    27896 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/rel.py
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/rel2.py
--rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/rel_emitter.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/rel_utils.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/analysis/mechanistic.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/client.py
--rw-r--r--   0        0        0    17970 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    36499 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/clients/types.py
--rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/loaders/loader.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/loaders/types.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/std/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/std/aggregates.py
--rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/std/graphs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/std/strings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    50224 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/debugger_server.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/tools/notes
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 relationalai-0.2.5/src/relationalai/util/snowflake_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/README.md
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/conftest.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_graph_visualize.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_snapshots.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/agg_ordering.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/bool.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/bottom.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/export.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/first.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/multi_valued.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/not_found.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/out_of_context.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/persist.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/smoke.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/strings.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/top.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/union.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/weighted_graphs.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/basics.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/centrality.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/community.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/connectivity.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/degree.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/link_prediction.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/end2end/test_cases/graphs/similarity.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/init-cli/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/init-cli/azure_basic.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/init-cli/common.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.5/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.5/.gitignore
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.5/docs/pypi/README.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.6/README.md
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/actions/benchmarks/action.yml
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/actions/end-to-end/action.yml
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/workflows/benchmarks.yml
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 relationalai-0.2.6/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/README.md
+-rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/getting_started.md
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/README.md
+-rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Instance/persist.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Instance/unpersist.md
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/floordiv__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/rfloordiv__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/extend.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_degree.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/diameter_range.md
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/distance.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_connected.md
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_reachable.md
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_triangle.md
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_edges.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_nodes.md
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_triangles.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/reachable_from.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/triangles.md
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/README.md
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/add.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/call__.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/extend.md
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/set.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/to.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/Edge.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/Node.md
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/README.md
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/abs.md
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/cbrt.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/ceil.md
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/floor.md
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/isclose.md
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/log.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/sign.md
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/sqrt.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/math/trunc_divide.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/README.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/concat.md
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/contains.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/ends_with.md
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/join.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/length.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/like.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/lowercase.md
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/regex_compile.md
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/regex_match.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/replace.md
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/split.md
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/split_part.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/python/std/strings/uppercase.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/faq/README.md
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/faq/engines.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/cdc.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/custom_snowflake_connection.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/fraud.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/requirements.txt
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/simple_recursion.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/simple_streamlit.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/README.md
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/articles_graph.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/articles_graph_with_nlp.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/pyproject.toml
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/utils.py
+-rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/articles_graph/daily_articles/04_04_2024.json
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/imdb/imdb.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/rel/foo.rel
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.6/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/index.html
+-rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/package.json
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/App.styl
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/Selection.tsx
+-rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/util.ts
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/assets/favicon.png
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/EventList.styl
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/EventList.tsx
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/EventViewer.styl
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/EventViewer.tsx
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Accordion.stories.tsx
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Accordion.styl
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Accordion.tsx
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Breadcrumbs.styl
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Breadcrumbs.tsx
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Button.styl
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Button.tsx
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Code.styl
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Code.tsx
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.stories.tsx
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.styl
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.tsx
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Field.stories.tsx
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Field.styl
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Field.tsx
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Icon.styl
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Icon.tsx
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.stories.tsx
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.styl
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.styl
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.tsx
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.6/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/emit.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/exec.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/compiler.py
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/debugging.py
+-rw-r--r--   0        0        0    46119 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    27989 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/rel.py
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/rel2.py
+-rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    18211 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0    37351 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/std/math.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/std/strings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    51586 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/tools/notes
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/util/keys.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/util/snowflake_logger.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relationalai-0.2.6/src/relationalai/util/tracing_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/conftest.py
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/util.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/benchmarks/conftest.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/benchmarks/test_tastybytes.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query0.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query2.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query3.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query4.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query5.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query6.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query7.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query8.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/math/query9.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/math.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/out_of_context.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/strings.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/union.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/basics.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/centrality.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/community.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/connectivity.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/degree.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/distance.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/link_prediction.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/similarity.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/end2end/test_cases/graphs/triangles.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/test_core.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/test_examples.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/basic/smoketest.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/found/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/execution/snapshots/test_examples/test_example/test/query0.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.6/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.6/docs/pypi/README.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.6/PKG-INFO
```

### Comparing `relationalai-0.2.5/README.md` & `relationalai-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/.github/actions/end-to-end/action.yml` & `relationalai-0.2.6/.github/actions/end-to-end/action.yml`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
   # Datadog
   datadog_api_key:
     required: false
     description: Datadog API key
   # Benchmark reporting
   sf_reporting_password:
     description: password for benchmark reporting
+    required: false
   
 
 runs:
   using: "composite"
   steps:
     - name: Set up Python
       uses: actions/setup-python@v4
@@ -56,29 +57,27 @@
       run: |
         python -m venv .venv
       shell: bash
 
     - name: Install dependencies
       run: |
         .venv/bin/python -m pip install --upgrade pip
-        .venv/bin/pip install pexpect
         .venv/bin/pip install .[dev]
       shell: bash
     
     - name: Setup Engine Name
       run: |
         echo "ENGINE_NAME=pyrel_test_$(openssl rand -hex 5)" >> $GITHUB_ENV
         echo "Setting up ENGINE_NAME..."
       shell: bash
 
     - name: Run Create Engine
       run: |
         echo "Using ENGINE_NAME: $ENGINE_NAME"
-        export PYTHONPATH=./tests/end2end:$PYTHONPATH
-        .venv/bin/python -c "from conftest import create_engine; create_engine('${{ env.ENGINE_NAME }}')"
+        .venv/bin/python -c "from tests.util import create_engine; create_engine('${{ env.ENGINE_NAME }}')"
 
       env: 
         RAI_CLIENT_ID: ${{ inputs.rai_client_id }}
         RAI_CLIENT_SECRET: ${{ inputs.rai_client_secret }}
         RAI_CLOUD_PROVIDER: ${{ inputs.rai_cloud_provider }}
         
         SF_TEST_ACCOUNT_NAME: ${{ inputs.sf_account }}
@@ -94,15 +93,22 @@
         DD_CIVISIBILITY_AGENTLESS_ENABLED: true
         DD_API_KEY: ${{ inputs.datadog_api_key }}
 
       shell: bash
     
     - name: Run Test
       run: |
-        .venv/bin/pytest -s tests/end2end --ddtrace --ddtrace-patch-all --cov=relationalai --cov-report lcov:coverage/lcov.info --cov-report html:coverage/html-report --cov-report term
+        .venv/bin/pytest -s \
+          tests/end2end \
+          --ddtrace \
+          --ddtrace-patch-all \
+          --cov=relationalai \
+          --cov-report lcov:coverage/lcov.info \
+          --cov-report html:coverage/html-report \
+          --cov-report term
       env:
         RAI_CLIENT_ID: ${{ inputs.rai_client_id }}
         RAI_CLIENT_SECRET: ${{ inputs.rai_client_secret }}
         RAI_CLOUD_PROVIDER: ${{ inputs.rai_cloud_provider }}
         
         SF_TEST_ACCOUNT_NAME: ${{ inputs.sf_account }}
         SF_TEST_WAREHOUSE_NAME: ${{ inputs.sf_warehouse }}
@@ -116,27 +122,27 @@
         SF_REPORTING_PASSWORD: ${{ inputs.sf_reporting_password }}
         SF_REPORTING_ACCOUNT: ndsoebe-rai_snowservices
         SF_REPORTING_WAREHOUSE: DATA_ANALYTICS_WH
         SF_REPORTING_DATABASE: PYREL_BENCHMARKING
         SF_REPORTING_SCHEMA: public
 
         ENGINE_NAME: ${{ env.ENGINE_NAME }}
+        ENABLE_TRACING_LOGGER: 'true'
 
         # datadog CI monitoring
         DD_SERVICE: pyrel-tests
         DD_ENV: ci
         DD_CIVISIBILITY_AGENTLESS_ENABLED: true
         DD_API_KEY: ${{ inputs.datadog_api_key }}
       shell: bash
     
     - name: Run Delete Engine
       if: always() && env.ENGINE_NAME != ''
       run: |
-          export PYTHONPATH=./tests/end2end:$PYTHONPATH
-          .venv/bin/python -c "from conftest import delete_engine; delete_engine('${{ env.ENGINE_NAME }}')"
+          .venv/bin/python -c "from tests.util import delete_engine; delete_engine('${{ env.ENGINE_NAME }}')"
       env: 
         RAI_CLIENT_ID: ${{ inputs.rai_client_id }}
         RAI_CLIENT_SECRET: ${{ inputs.rai_client_secret }}
         RAI_CLOUD_PROVIDER: ${{ inputs.rai_cloud_provider }}
         
         SF_TEST_ACCOUNT_NAME: ${{ inputs.sf_account }}
         SF_TEST_WAREHOUSE_NAME: ${{ inputs.sf_warehouse }}
@@ -146,8 +152,8 @@
         SF_TEST_ACCOUNT_PASSWORD: ${{ inputs.sf_password }}
 
         # datadog CI monitoring
         DD_SERVICE: pyrel-tests
         DD_ENV: ci
         DD_CIVISIBILITY_AGENTLESS_ENABLED: true
         DD_API_KEY: ${{ inputs.datadog_api_key }}
-      shell: bash
+      shell: bash
```

### Comparing `relationalai-0.2.5/.github/workflows/end-to-end.yml` & `relationalai-0.2.6/.github/workflows/benchmarks.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,36 @@
-name: Run End To End Tests
+name: Run Benchmarks
 
 on:
-  push:
-    branches: [main]
-  pull_request:
-    branches: [main]
-  workflow_call:
-    inputs:
-      username:
-        description: The username to run the tests against
-        type: string
-        default: team-prod-experience@relational.ai
-      account:
-        description: The account to run the tests against
-        type: string
-        default: ndsoebe-rai_integration_aws_uswest_1_consumer
-      warehouse:
-        description: The warehouse to run the tests against
-        type: string
-        default: int_env_wh
-      rai_app_name:
-        description: The name of the SPCS app to run the tests against
-        type: string
-        default: rai_int_app
-      compute_pool:
-        description: The compute pool to run the tests against
-        type: string
-        default: int_env_benchmark_compute_xs
-    secrets:
-      password:
-        description: The password to run the tests against
-        required: true
-      dd_api_key:
-        description: The Datadog API key
-        required: true
+  schedule:
+    - cron: '0 0 * * *'
+  workflow_dispatch:
 
 concurrency:
   group:
     ${{ github.workflow }}-${{ (github.ref_name == 'main' || github.event_name == 'workflow_dispatch')
     && github.run_id
     || github.ref }}
   cancel-in-progress: true 
 
 jobs:
-  test:
+  benchmark:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         include:
           - python-version: '3.12'
             cloud-provider: 'snowflake'
-          - python-version: '3.10'
-            cloud-provider: 'azure'
     steps:
 
     - uses: actions/checkout@v4
       name: Checkout repository
 
-    - uses: ./.github/actions/end-to-end
+    - uses: ./.github/actions/benchmarks
       with:
         python_version: ${{ matrix.python-version }}
         rai_cloud_provider: ${{ matrix.cloud-provider }}
         rai_client_id: ${{ secrets.RAI_CLIENT_ID }}
         rai_client_secret: ${{ secrets.RAI_CLIENT_SECRET }}
         sf_account: ndsoebe-rai_integration_aws_uswest_1_consumer
         sf_warehouse: int_env_wh
```

### Comparing `relationalai-0.2.5/.github/workflows/publish-to-pypi.yml` & `relationalai-0.2.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/.github/workflows/ruff.yml` & `relationalai-0.2.6/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/getting_started.md` & `relationalai-0.2.6/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.2.6/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/_old/metamodel.md` & `relationalai-0.2.6/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/_old/python_dsl.md` & `relationalai-0.2.6/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/_old/quickstart.md` & `relationalai-0.2.6/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/cli/README.md` & `relationalai-0.2.6/docs/api_reference/cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/configuration/README.md` & `relationalai-0.2.6/docs/api_reference/configuration/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Expression.md` & `relationalai-0.2.6/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Property.md` & `relationalai-0.2.6/docs/api_reference/python/Property.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/README.md` & `relationalai-0.2.6/docs/api_reference/python/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -37,22 +37,24 @@
   - [`Model.Type()`](./Model/Type.md)
   - [`Model.union()`](./Model/union.md)
 - [`Producer`](./Producer/README.md)
   - [`Producer.__add__()`](./Producer/add__.md)
   - [`Producer.__enter__()`](./Producer/enter__.md)
   - [`Producer.__eq__()`](./Producer/eq__.md)
   - [`Producer.__exit__()`](./Producer/exit__.md)
+  - [`Producer.__floordiv__()`](./Producer/floordiv__.md)
   - [`Producer.__ge__()`](./Producer/ge__.md)
   - [`Producer.__getattribute__()`](./Producer/getattribute__.md)
   - [`Producer.__gt__()`](./Producer/gt__.md)
   - [`Producer.__le__()`](./Producer/le__.md)
   - [`Producer.__lt__()`](./Producer/lt__.md)
   - [`Producer.__mul__()`](./Producer/mul__.md)
   - [`Producer.__ne__()`](./Producer/ne__.md)
   - [`Producer.__radd__()`](./Producer/radd__.md)
+  - [`Producer.__rfloordiv__()`](./Producer/rfloordiv__.md)
   - [`Producer.__rmul__()`](./Producer/rmul__.md)
   - [`Producer.__rsub__()`](./Producer/rsub__.md)
   - [`Producer.__rtruediv__()`](./Producer/rtruediv__.md)
   - [`Producer.__sub__()`](./Producer/sub__.md)
   - [`Producer.__truediv__()`](./Producer/truediv__.md)
 - [`Property`](./Property.md)
 - [`Type`](./Type/README.md)
@@ -88,36 +90,45 @@
   - [`graphs.Compute.adamic_adar()`](./std/graphs/Compute/adamic_adar.md)
   - [`graphs.Compute.avg_degree()`](./std/graphs/Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./std/graphs/Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./std/graphs/Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./std/graphs/Compute/betweeness_centrality.md)
   - [`graphs.Compute.cosine_similarity()`](./std/graphs/Compute/cosine_similarity.md)
   - [`graphs.Compute.common_neighbor()`](./std/graphs/Compute/common_neighbor.md)
-  - [`graphs.Compute.degree()`](./std/graphs/Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./std/graphs/Compute/degree_centrality.md)
+  - [`graphs.Compute.degree()`](./std/graphs/Compute/degree.md)
+  - [`graphs.Compute.diameter_range()`](./std/graphs/Compute/diameter_range.md)
+  - [`graphs.Compute.distance()`](./std/graphs/Compute/distance.md)
   - [`graphs.Compute.eigenvector_centrality()`](./std/graphs/Compute/eigenvector_centrality.md)
   - [`graphs.Compute.num_edges()`](./std/graphs//Compute/num_edges.md)
   - [`graphs.Compute.indegree()`](./std/graphs/Compute/indegree.md)
   - [`graphs.Compute.is_connected()`](./std/graphs/Compute/is_connected.md)
   - [`graphs.Compute.is_reachable()`](./std/graphs/Compute/is_reachable.md)
+  - [`graphs.Compute.is_triangle()`](./std/graphs/Compute/is_triangle.md)
   - [`graphs.Compute.label_propagation()`](./std/graphs/Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./std/graphs/Compute/louvain.md)
   - [`graphs.Compute.max_degree()`](./std/graphs/Compute/max_degree.md)
   - [`graphs.Compute.max_indegree()`](./std/graphs/Compute/max_indegree.md)
   - [`graphs.Compute.max_outdegree()`](./std/graphs/Compute/max_outdegree.md)
   - [`graphs.Compute.min_degree()`](./std/graphs/Compute/min_degree.md)
   - [`graphs.Compute.min_indegree()`](./std/graphs/Compute/min_indegree.md)
   - [`graphs.Compute.min_outdegree()`](./std/graphs/Compute/min_outdegree.md)
+  - [`graphs.Compute.num_edges()`](./std/graphs/Compute/num_edges.md)
   - [`graphs.Compute.num_nodes()`](./std//graphs//Compute/num_nodes.md)
+  - [`graphs.Compute.num_triangles()`](./std/graphs/Compute/num_triangles.md)
   - [`graphs.Compute.outdegree()`](./std/graphs/Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./std/graphs/Compute/pagerank.md)
   - [`graphs.Compute.preferential_attachment()`](./std/graphs/Compute/preferential_attachment.md)
   - [`graphs.Compute.reachable_from()`](./std/graphs/Compute/reachable_from.md)
+  - [`graphs.Compute.triangles()`](./std/graphs/Compute/triangles.md)
   - [`graphs.Compute.weakly_connected_component()`](./std/graphs/Compute/weakly_connected_component.md)
+  - [`graphs.Compute.weighted_distance()`](./std/graphs/Compute/weighted_distance.md)
+  - [`graphs.Compute.weighted_cosine_similarity()`](./std/graphs/Compute/weighted_cosine_similarity.md)
   - [`graphs.Compute.weighted_degree_centrality()`](./std/graphs/Compute/weighted_degree_centrality.md)
+  - [`graphs.Compute.weighted_jaccard_similarity()`](./std/graphs/Compute/weighted_jaccard_similarity.md)
 - [`graphs.Edge`](./std/graphs/Edge/README.md)
   - [`graphs.Edge.add()`](./std/graphs/Edge/add.md)
   - [`graphs.Edge.extend()`](./std/graphs/Edge/extend.md)
 - [`graphs.EdgeInstance`](./std/graphs/EdgeInstance/README.md)
   - [`graphs.EdgeInstance.from_`](./std/graphs/EdgeInstance/from_.md)
   - [`graphs.EdgeInstance.to`](./std/graphs/EdgeInstance/to.md)
   - [`graphs.EdgeInstance.set()`](./std/graphs/EdgeInstance/set.md)
@@ -127,23 +138,40 @@
   - [`graphs.Graph.fetch()`](./std/graphs/Graph/fetch.md)
   - [`graphs.Graph.id`](./std/graphs/Graph/id.md)
   - [`graphs.Graph.model`](./std/graphs/Graph/model.md)
   - [`graphs.Graph.Node`](./std/graphs/Graph/Node.md)
   - [`graphs.Graph.undirected`](./std/graphs/Graph/undirected.md)
   - [`graphs.Graph.visualize()`](./std/graphs/Graph/visualize.md)
 
-## [`relationalai.std.strings`](./std/strings/README.md)
+### [`relationalai.std.math`](./std/math/README.md)
+
+- [`math.abs()`](./std/math/abs.md)
+- [`math.isclose()`](./std/math/isclose.md)
+- [`math.ceil()`](./std/math/ceil.md)
+- [`math.cbrt()`](./std/math/cbrt.md)
+- [`math.floor()`](./std/math/floor.md)
+- [`math.log()`](./std/math/log.md)
+- [`math.sign()`](./std/math/sign.md)
+- [`math.sqrt()`](./std/math/sqrt.md)
+- [`math.trunc_divide()`](./std/math/trunc_divide.md)
+
+### [`relationalai.std.strings`](./std/strings/README.md)
 
 - [`strings.concat()`](./std/strings/concat.md)
 - [`strings.contains()`](./std/strings/contains.md)
 - [`strings.ends_with()`](./std/strings/ends_with.md)
 - [`strings.join()`](./std/strings/join.md)
 - [`strings.length()`](./std/strings/length.md)
+- [`strings.like()`](./std/strings/like.md)
 - [`strings.lowercase()`](./std/strings/lowercase.md)
+- [`strings.regex_compile()`](./std/strings/regex_compile.md)
+- [`strings.regex_match()`](./std/strings/regex_match.md)
 - [`strings.replace()`](./std/strings/replace.md)
+- [`strings.split()`](./std/strings/split.md)
+- [`strings.split_part()`](./std/strings/split_part.md)
 - [`strings.uppercase()`](./std/strings/uppercase.md)
 
 ## [`relationalai.clients`](./clients/README.md)
 
 - [`clients.snowflake`](./clients/snowflake/README.md)
   - [`clients.snowflake.PrimaryKey`](./clients/snowflake/PrimaryKey.md)
   - [`clients.snowflake.Snowflake`](./clients/snowflake/Snowflake.md)
```

### Comparing `relationalai-0.2.5/docs/api_reference/python/Context/README.md` & `relationalai-0.2.6/docs/api_reference/python/Context/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Context/enter__.md` & `relationalai-0.2.6/docs/api_reference/python/Context/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Context/exit__.md` & `relationalai-0.2.6/docs/api_reference/python/Context/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Context/iter__.md` & `relationalai-0.2.6/docs/api_reference/python/Context/iter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Context/model.md` & `relationalai-0.2.6/docs/api_reference/python/Context/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Context/results.md` & `relationalai-0.2.6/docs/api_reference/python/Context/results.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/ContextSelect/README.md` & `relationalai-0.2.6/docs/api_reference/python/ContextSelect/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/ContextSelect/add.md` & `relationalai-0.2.6/docs/api_reference/python/ContextSelect/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/ContextSelect/call__.md` & `relationalai-0.2.6/docs/api_reference/python/ContextSelect/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/ContextSelect/getattribute__.md` & `relationalai-0.2.6/docs/api_reference/python/ContextSelect/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Instance/README.md` & `relationalai-0.2.6/docs/api_reference/python/Instance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Instance/persist.md` & `relationalai-0.2.6/docs/api_reference/python/Instance/persist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Instance/set.md` & `relationalai-0.2.6/docs/api_reference/python/Instance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Instance/unpersist.md` & `relationalai-0.2.6/docs/api_reference/python/Instance/unpersist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/InstanceProperty/README.md` & `relationalai-0.2.6/docs/api_reference/python/InstanceProperty/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/InstanceProperty/or_.md` & `relationalai-0.2.6/docs/api_reference/python/InstanceProperty/or_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Model/README.md` & `relationalai-0.2.6/docs/api_reference/python/Model/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Model/Type.md` & `relationalai-0.2.6/docs/api_reference/python/Model/Type.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Model/found.md` & `relationalai-0.2.6/docs/api_reference/python/Model/found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Model/not_found.md` & `relationalai-0.2.6/docs/api_reference/python/Model/not_found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Model/ordered_choice.md` & `relationalai-0.2.6/docs/api_reference/python/Model/ordered_choice.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Model/query.md` & `relationalai-0.2.6/docs/api_reference/python/Model/query.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Model/read.md` & `relationalai-0.2.6/docs/api_reference/python/Model/read.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Model/rule.md` & `relationalai-0.2.6/docs/api_reference/python/Model/rule.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Model/scope.md` & `relationalai-0.2.6/docs/api_reference/python/Model/scope.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Model/union.md` & `relationalai-0.2.6/docs/api_reference/python/Model/union.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/README.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 
 ## Methods
 
 - [`Producer.__add__()`](./add__.md)
 - [`Producer.__enter__()`](./enter__.md)
 - [`Producer.__eq__()`](./eq__.md)
 - [`Producer.__exit__()`](./exit__.md)
+- [`Producer.__floordiv__()`](./floordiv__.md)
 - [`Producer.__ge__()`](./ge__.md)
 - [`Producer.__getattribute__()`](./getattribute__.md)
 - [`Producer.__gt__()`](./gt__.md)
 - [`Producer.__le__()`](./le__.md)
 - [`Producer.__lt__()`](./lt__.md)
 - [`Producer.__mul__()`](./mul__.md)
 - [`Producer.__ne__()`](./ne__.md)
 - [`Producer.__pow__()`](./pow__.md),
 - [`Producer.__radd__()`](./radd__.md)
+- [`Producer.__rfloordiv__()`](./rfloordiv__.md)
 - [`Producer.__rmul__()`](./rmul__.md)
 - [`Producer.__rpow__()`](./rpow__.md),
 - [`Producer.__rsub__()`](./rsub__.md)
 - [`Producer.__rtruediv__()`](./rtruediv__.md)
 - [`Producer.__sub__()`](./sub__.md)
 - [`Producer.__truediv__()`](./truediv__.md)
```

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/add__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/add__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/enter__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/eq__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/eq__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/exit__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/ge__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/ge__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/getattribute__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/gt__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/gt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/le__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/le__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/lt__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/lt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/mul__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/mul__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/ne__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/ne__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/pow__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/pow__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/sub__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/sub__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Producer/truediv__.md` & `relationalai-0.2.6/docs/api_reference/python/Producer/truediv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Type/README.md` & `relationalai-0.2.6/docs/api_reference/python/Type/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Type/add.md` & `relationalai-0.2.6/docs/api_reference/python/Type/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Type/call__.md` & `relationalai-0.2.6/docs/api_reference/python/Type/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Type/extend.md` & `relationalai-0.2.6/docs/api_reference/python/Type/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/Type/or__.md` & `relationalai-0.2.6/docs/api_reference/python/Type/or__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/clients/README.md` & `relationalai-0.2.6/docs/api_reference/python/clients/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/PrimaryKey.md` & `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/PrimaryKey.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/README.md` & `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/Snowflake.md` & `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/Snowflake.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md` & `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md` & `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md` & `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md` & `relationalai-0.2.6/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/README.md` & `relationalai-0.2.6/docs/api_reference/python/std/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -22,36 +22,45 @@
   - [`graphs.Compute.avg_degree()`](./graphs/Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./graphs/Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./graphs/Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./graphs/Compute/betweeness_centrality.md)
   - [`graphs.Compute.common_neighbor()`](./graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.cosine_similarity()`](./graphs/Compute/cosine_similarity.md)
   - [`graphs.Compute.common_neighbor()`](./graphs/Compute/common_neighbor.md)
-  - [`graphs.Compute.degree()`](./graphs/Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./graphs/Compute/degree_centrality.md)
+  - [`graphs.Compute.degree()`](./graphs/Compute/degree.md)
+  - [`graphs.Compute.diameter_range()`](./graphs/Compute/diameter_range.md)
+  - [`graphs.Compute.distance()`](./graphs/Compute/distance.md)
   - [`graphs.Compute.eigenvector_centrality()`](./graphs/Compute/eigenvector_centrality.md)
   - [`graphs.Compute.is_connected()`](./graphs/Compute/is_connected.md)
   - [`graphs.Compute.is_reachable()`](./graphs/Compute/is_reachable.md)
+  - [`graphs.Compute.is_triangle()`](./graphs/Compute/is_triangle.md)
   - [`graphs.Compute.num_edges()`](./graphs/Compute/num_edges.md)
   - [`graphs.Compute.indegree()`](./graphs/Compute/indegree.md)
   - [`graphs.Compute.label_propagation()`](./graphs/Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./graphs/Compute/louvain.md)
   - [`graphs.Compute.max_degree()`](./graphs/Compute/max_degree.md)
   - [`graphs.Compute.max_indegree()`](./graphs/Compute/max_indegree.md)
   - [`graphs.Compute.max_outdegree()`](./graphs/Compute/max_outdegree.md)
   - [`graphs.Compute.min_degree()`](./graphs/Compute/min_degree.md)
   - [`graphs.Compute.min_indegree()`](./graphs/Compute/min_indegree.md)
   - [`graphs.Compute.min_outdegree()`](./graphs/Compute/min_outdegree.md)
+  - [`graphs.Compute.num_edges()`](./graphs/Compute/num_edges.md)
   - [`graphs.Compute.num_nodes()`](./graphs/Compute/num_nodes.md)
+  - [`graphs.Compute.num_triangles()`](./graphs/Compute/num_triangles.md)
   - [`graphs.Compute.outdegree()`](./graphs/Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./graphs/Compute/pagerank.md)
   - [`graphs.Compute.preferential_attachment()`](./graphs/Compute/preferential_attachment.md)
   - [`graphs.Compute.reachable_from()`](./graphs/Compute/reachable_from.md)
+  - [`graphs.Compute.triangles()`](./graphs/Compute/triangles.md)
   - [`graphs.Compute.weakly_connected_component()`](./graphs/Compute/weakly_connected_component.md)
+  - [`graphs.Compute.weighted_distance()`](./graphs/Compute/weighted_distance.md)
+  - [`graphs.Compute.weighted_cosine_similarity()`](./graphs/Compute/weighted_cosine_similarity.md)
   - [`graphs.Compute.weighted_degree_centrality()`](./graphs/Compute/weighted_degree_centrality.md)
+  - [`graphs.Compute.weighted_jaccard_similarity()`](./graphs/Compute/weighted_jaccard_similarity.md)
 - [`graphs.Edge`](./graphs/Edge/README.md)
   - [`graphs.Edge.__call__()`](./graphs/Edge/call__.md)
   - [`graphs.Edge.add()`](./graphs/Edge/add.md)
   - [`graphs.Edge.extend()`](./graphs/Edge/extend.md)
 - [`graphs.EdgeInstance`](./graphs/EdgeInstance/README.md)
   - [`graphs.EdgeInstance.from_`](./graphs/EdgeInstance/from_.md)
   - [`graphs.EdgeInstance.to`](./graphs/EdgeInstance/to.md)
@@ -61,18 +70,35 @@
   - [`graphs.Graph.Edge`](./graphs/Graph/Edge.md)
   - [`graphs.Graph.fetch()`](./graphs/Graph/fetch.md)
   - [`graphs.Graph.id`](./graphs/Graph/id.md)
   - [`graphs.Graph.model`](./graphs/Graph/model.md)
   - [`graphs.Graph.Node`](./graphs/Graph/Node.md)
   - [`graphs.Graph.undirected`](./graphs/Graph/undirected.md)
   - [`graphs.Graph.visualize()`](./graphs/Graph/visualize.md)
+  
+## [`relationalai.std.math`](./math/README.md)
+
+- [`math.abs()`](./math/abs.md)
+- [`math.isclose()`](./math/isclose.md)
+- [`math.ceil()`](./math/ceil.md)
+- [`math.cbrt()`](./math/cbrt.md)
+- [`math.floor()`](./math/floor.md)
+- [`math.log()`](./math/log.md)
+- [`math.sign()`](./math/sign.md)
+- [`math.sqrt()`](./math/sqrt.md)
+- [`math.trunc_divide()`](./math/trunc_divide.md)
 
 ## [`relationalai.std.strings`](./strings/README.md)
 
 - [`strings.concat()`](./strings/concat.md)
 - [`strings.contains()`](./strings/contains.md)
 - [`strings.ends_with()`](./strings/ends_with.md)
 - [`strings.join()`](./strings/join.md)
 - [`strings.length()`](./strings/length.md)
+- [`strings.like()`](./strings/like.md)
 - [`strings.lowercase()`](./strings/lowercase.md)
+- [`strings.regex_compile()`](./strings/regex_compile.md)
+- [`strings.regex_match()`](./strings/regex_match.md)
 - [`strings.replace()`](./strings/replace.md)
+- [`strings.split()`](./strings/split.md)
+- [`strings.split_part()`](./strings/split_part.md)
 - [`strings.uppercase()`](./strings/uppercase.md)
```

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/Vars.md` & `relationalai-0.2.6/docs/api_reference/python/std/Vars.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/alias.md` & `relationalai-0.2.6/docs/api_reference/python/std/alias.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/aggregates/README.md` & `relationalai-0.2.6/docs/api_reference/python/std/aggregates/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/aggregates/avg.md` & `relationalai-0.2.6/docs/api_reference/python/std/aggregates/avg.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/aggregates/count.md` & `relationalai-0.2.6/docs/api_reference/python/std/aggregates/count.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/aggregates/max.md` & `relationalai-0.2.6/docs/api_reference/python/std/aggregates/max.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/aggregates/min.md` & `relationalai-0.2.6/docs/api_reference/python/std/aggregates/min.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/aggregates/rank_asc.md` & `relationalai-0.2.6/docs/api_reference/python/std/aggregates/rank_asc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/aggregates/rank_desc.md` & `relationalai-0.2.6/docs/api_reference/python/std/aggregates/rank_desc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/aggregates/sum.md` & `relationalai-0.2.6/docs/api_reference/python/std/aggregates/sum.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/README.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -6,33 +6,44 @@
 - [`graphs.Compute`](./Compute/README.md)
   - [`graphs.Compute.avg_degree()`](./Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./Compute/betweeness_centrality.md)
   - [`graphs.Compute.common_neighbor()`](./Compute/common_neighbor.md)
   - [`graphs.Compute.cosine_similarity()`](./Compute/cosine_similarity.md)
-  - [`graphs.Compute.degree()`](./Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./Compute/degree_centrality.md)
+  - [`graphs.Compute.degree()`](./Compute/degree.md)
+  - [`graphs.Compute.diameter_range()`](./Compute/diameter_range.md)
+  - [`graphs.Compute.distance()`](./Compute/distance.md)
   - [`graphs.Compute.eigenvector_centrality()`](./Compute/eigenvector_centrality.md)
   - [`graph.Compute.indegree()`](./Compute/indegree.md)
   - [`graphs.Compute.is_connected()`](./Compute/is_connected.md)
   - [`graphs.Compute.is_reachable()`](./Compute/is_reachable.md)
+  - [`graphs.Compute.is_triangle()`](./Compute/is_triangle.md)
   - [`graphs.Compute.label_propagation()`](./Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./Compute/louvain.md)
   - [`graphs.Compute.max_degree()`](./Compute/max_degree.md)
   - [`graphs.Compute.max_indegree()`](./Compute/max_indegree.md)
   - [`graphs.Compute.max_outdegree()`](./Compute/max_outdegree.md)
   - [`graphs.Compute.min_degree()`](./Compute/min_degree.md)
   - [`graphs.Compute.min_indegree()`](./Compute/min_indegree.md)
   - [`graphs.Compute.min_outdegree()`](./Compute/min_outdegree.md)
+  - [`graphs.Compute.num_edges()`](./Compute/num_edges.md)
+  - [`graphs.Compute.num_nodes()`](./Compute/num_nodes.md)
+  - [`graphs.Compute.num_triangles()`](./Compute/num_triangles.md)
   - [`graphs.Compute.outdegree()`](./Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./Compute/pagerank.md)
   - [`graphs.Compute.preferential_attachment()`](./Compute/preferential_attachment.md)
   - [`graphs.Compute.reachable_from()`](./Compute/reachable_from.md
+  - [`graphs.Compute.triangles()`](./Compute/triangles.md)
   - [`graphs.Compute.weakly_connected_component()`](./Compute/weakly_connected_component.md)
+  - [`graphs.Compute.weighted_distance()`](./Compute/weighted_distance.md)
+  - [`graphs.Compute.weighted_cosine_similarity()`](./Compute/weighted_cosine_similarity.md)
+  - [`graphs.Compute.weighted_degree_centrality()`](./Compute/weighted_degree_centrality.md)
+  - [`graphs.Compute.weighted_jaccard_similarity()`](./Compute/weighted_jaccard_similarity.md)
 - [`graphs.Edge`](./Edge/README.md)
   - [`graphs.Edge.__call__()`](./Edge/call__.md)
   - [`graphs.Edge.add()`](./Edge/add.md)
   - [`graphs.Edge.extend()`](./Edge/extend.md)
 - [`graphs.EdgeInstance`](./EdgeInstance/README.md)
   - [`graphs.EdgeInstance.from_`](./EdgeInstance/from_.md)
   - [`graphs.EdgeInstance.to`](./EdgeInstance/to.md)
```

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/README.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,38 @@
 - [`Compute.avg_outdegree()`](./avg_outdegree.md)
 - [`Compute.betweeness_centrality()`](./betweeness_centrality.md)
 - [`Compute.common_neighbor()`](./common_neighbor.md)
 - [`Compute.cosine_similarity()`](./cosine_similarity.md)
 - [`Compute.degree()`](./degree.md)
 - [`Compute.degree_centrality()`](./degree_centrality.md)
 - [`Compute.eigenvector_centrality()`](./eigenvector_centrality.md)
+- [`Compute.indegree()`](./indegree.md)
 - [`Compute.is_connected()`](./is_connected.md)
 - [`Compute.is_reachable()`](./is_reachable.md)
-- [`Compute.num_edges()`](./num_edges.md)
-- [`Compute.indegree()`](./indegree.md)
+- [`Compute.is_triangle()`](./is_triangle.md)
 - [`Compute.label_propagation()`](./label_propagation.md)
 - [`Compute.louvain()`](./louvain.md)
 - [`Compute.max_degree()`](./max_degree.md)
 - [`Compute.max_indegree()`](./max_indegree.md)
 - [`Compute.max_outdegree()`](./max_outdegree.md)
 - [`Compute.min_degree()`](./min_degree.md)
 - [`Compute.min_indegree()`](./min_indegree.md)
 - [`Compute.min_outdegree()`](./min_outdegree.md)
+- [`Compute.num_edges()`](./num_edges.md)
 - [`Compute.num_nodes()`](./num_nodes.md)
+- [`Compute.num_triangles()`](./num_triangles.md)
 - [`Compute.outdegree()`](./outdegree.md)
 - [`Compute.pagerank()`](./pagerank.md)
 - [`Compute.preferential_attachment()`](./preferential_attachment.md)
 - [`Compute.reachable_from()`](./reachable_from.md)
+- [`Compute.triangles()`](./triangles.md)
 - [`Compute.weakly_connected_component()`](./weakly_connected_component.md)
+- [`Compute.weighted_cosine_similarity()`](./weighted_cosine_similarity.md)
 - [`Compute.weighted_degree_centrality()`](./weighted_degree_centrality.md)
+- [`Compute.weighted_jaccard_similarity()`](./weighted_jaccard_similarity.md)
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
```

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/adamic_adar.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/adamic_adar.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_degree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_indegree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/common_neighbor.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/common_neighbor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/degree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/degree_centrality.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/indegree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/infomap.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/infomap.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/is_connected.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_connected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/is_reachable.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/is_reachable.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/label_propagation.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/label_propagation.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/louvain.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/louvain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_degree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_indegree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/max_outdegree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/max_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_degree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_indegree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/min_outdegree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/min_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/num_edges.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_edges.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/num_nodes.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/num_nodes.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/outdegree.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/pagerank.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/pagerank.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/reachable_from.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/reachable_from.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/README.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/add.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/call__.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Edge/extend.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Edge/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/README.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/from_.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/from_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/set.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/EdgeInstance/to.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/EdgeInstance/to.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/Edge.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/Edge.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/Node.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/Node.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/README.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/compute.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/compute.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/fetch.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/fetch.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/id.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/id.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/model.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/undirected.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/undirected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/visualize.md` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/visualize.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png` & `relationalai-0.2.6/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/strings/concat.md` & `relationalai-0.2.6/docs/api_reference/python/std/strings/concat.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/strings/contains.md` & `relationalai-0.2.6/docs/api_reference/python/std/strings/contains.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # `relational.std.strings.contains()`
 
 ```python
-relationalai.std.strings.contains(string: Producer, substring: str | Producer) -> Expression
+relationalai.std.strings.contains(string: str | Producer, substring: str | Producer) -> Expression
 ```
 
-Constrains the `string` Producer to only values containing the substring `substring`.
+Adds a constraint to a [rule](../../Model/rule.md) or [query](../../Model/query.md) that
+`string` must contain the substring `substring`.
 
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `string` | [`Producer`](../../../Producer/README.md) | A producer that produces string values. |
+| `string` | [`Producer`](../../../Producer/README.md) | The string to check. |
 | `substring` | `str` or [`Producer`](../../../Producer/README.md) | The substring to check for. |
 
 ## Returns
 
 An [`Expression`](../../../Expression.md) object.
 
 ## Example
```

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/strings/ends_with.md` & `relationalai-0.2.6/docs/api_reference/python/std/strings/ends_with.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/strings/join.md` & `relationalai-0.2.6/docs/api_reference/python/std/strings/join.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/strings/length.md` & `relationalai-0.2.6/docs/api_reference/python/std/strings/length.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/strings/lowercase.md` & `relationalai-0.2.6/docs/api_reference/python/std/strings/lowercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/strings/replace.md` & `relationalai-0.2.6/docs/api_reference/python/std/strings/replace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/api_reference/python/std/strings/uppercase.md` & `relationalai-0.2.6/docs/api_reference/python/std/strings/uppercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/docs/faq/engines.md` & `relationalai-0.2.6/docs/faq/engines.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/README.md` & `relationalai-0.2.6/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/cdc.py` & `relationalai-0.2.6/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/custom_snowflake_connection.py` & `relationalai-0.2.6/examples/custom_snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/emit_playground.py` & `relationalai-0.2.6/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/found.py` & `relationalai-0.2.6/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/fraud.ipynb` & `relationalai-0.2.6/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/fraud.py` & `relationalai-0.2.6/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/graph_algos.py` & `relationalai-0.2.6/examples/graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/nested.py` & `relationalai-0.2.6/examples/nested.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/or_types.py` & `relationalai-0.2.6/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/remote_load_csv.py` & `relationalai-0.2.6/examples/remote_load_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/simple_recursion.py` & `relationalai-0.2.6/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/simple_streamlit.py` & `relationalai-0.2.6/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/solver.py` & `relationalai-0.2.6/examples/solver.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/weighted_graph_algos.py` & `relationalai-0.2.6/examples/weighted_graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/articles_graph/README.md` & `relationalai-0.2.6/examples/articles_graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/articles_graph/articles_graph.py` & `relationalai-0.2.6/examples/articles_graph/articles_graph.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/articles_graph/articles_graph_with_nlp.py` & `relationalai-0.2.6/examples/articles_graph/articles_graph_with_nlp.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/articles_graph/utils.py` & `relationalai-0.2.6/examples/articles_graph/utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/articles_graph/daily_articles/04_04_2024.json` & `relationalai-0.2.6/examples/articles_graph/daily_articles/04_04_2024.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/data/people.csv` & `relationalai-0.2.6/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/data/transactions.csv` & `relationalai-0.2.6/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/ev_penetration/ev_penetration.py` & `relationalai-0.2.6/examples/ev_penetration/ev_penetration.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/ev_penetration/ev_penetration_csv.py` & `relationalai-0.2.6/examples/ev_penetration/ev_penetration_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/ev_penetration/state_stats.csv` & `relationalai-0.2.6/examples/ev_penetration/state_stats.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/imdb/README.md` & `relationalai-0.2.6/examples/imdb/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/imdb/imdb.csv` & `relationalai-0.2.6/examples/imdb/imdb.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/imdb/imdb.py` & `relationalai-0.2.6/examples/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/rel/solver.rel` & `relationalai-0.2.6/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/social-money-network/SF_pagerank.ipynb` & `relationalai-0.2.6/examples/social-money-network/SF_pagerank.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/social-money-network/Simulation-and-SF-Upload.ipynb` & `relationalai-0.2.6/examples/social-money-network/Simulation-and-SF-Upload.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/examples/social-money-network/snowflake_pagerank.py` & `relationalai-0.2.6/examples/social-money-network/snowflake_pagerank.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/package-lock.json` & `relationalai-0.2.6/frontend/debugger/package-lock.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/package.json` & `relationalai-0.2.6/frontend/debugger/package.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/tsconfig.json` & `relationalai-0.2.6/frontend/debugger/tsconfig.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/vite.config.ts` & `relationalai-0.2.6/frontend/debugger/vite.config.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/.storybook/main.ts` & `relationalai-0.2.6/frontend/debugger/.storybook/main.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/App.styl` & `relationalai-0.2.6/frontend/debugger/src/App.styl`

 * *Files 24% similar despite different names*

```diff
@@ -54,31 +54,61 @@
   flex-direction: row;
   height: 100vh;
   overflow: hidden;
 
   & > .sidebar.left {
     flex: 0 0 auto;
 
-    & > .sidebar-content {
-      min-width: 200px;
-      max-width: unquote("min(450px, 30vw)");
+    .sidebar-content {
+      overflow-y: auto;
+      .os-windows & {
+        -ms-overflow-style: none;
+        scrollbar-width: none;
+        &::-webkit-scrollbar {
+          display: none;
+        }
+      }
+    }
 
-      & > .ui-collapsible-inner > .sidebar-inner > header {
+    .sidebar-inner {
+      min-width: 250px;
+      width: unquote("min(450px, 30vw)");
+
+      & > header {
         padding: 0 24px;
         padding-top: 24px;
         gap: 12px;
       }
     }
   }
 
   main {
     flex: 1 1 0;
     height: 100vh;
     min-width: 0;
     display: flex;
+    flex-direction: column;
+
+    & > .ui-breadcrumbs {
+      padding: 20px 60px;
+    }
+
+      scroll-container {
+        flex: 1 1 0;
+        overflow-y: auto;
+
+        scroll-inner {
+          min-height: 100%;
+          padding: 0 60px;
+          display: flex;
+          flex-direction: column;
+          align-items: center;
+          justify-content: center;
+        }
+      }
   }
 
   & > status-icon {
       position: absolute;
       top: 20px;
       right: 20px;
   }
```

### Comparing `relationalai-0.2.5/frontend/debugger/src/debugger_client.ts` & `relationalai-0.2.6/frontend/debugger/src/debugger_client.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import { Accessor, Setter, batch, createMemo, createSignal } from "solid-js";
-import { SetStoreFunction, createStore, produce } from "solid-js/store";
+import { SetStoreFunction, createStore, produce, unwrap } from "solid-js/store";
 import * as Mech from "./types/mech";
 import { create_ws } from "./ws";
 
 //------------------------------------------------------------------------------
 // Utils
 //------------------------------------------------------------------------------
 
@@ -16,29 +16,30 @@
 }
 
 export interface Placeholder {
     "event": "placeholder",
     selection_path: number[],
     span_type?: undefined,
     events?: undefined
+    parent?: undefined
 }
 
 export type Subject = Message.Event|Span|Placeholder;
 
-
 //------------------------------------------------------------------------------
 // Messages
 //------------------------------------------------------------------------------
 
 export namespace Message {
     export interface Base {
         event: string,
         selection_path: number[],
         span_type?: undefined,
         events?: undefined,
+        parent?: Span;
         [key: string]: unknown
     }
     
     export interface SpanStart extends Base {
         event: "span_start";
         span: {
             type: string;
@@ -56,14 +57,15 @@
     }
 
     export interface Time extends Base {
         event: "time",
         type: string,
         elapsed: number,
         results?: ResultData
+        code?: string
     }
     export function is_time(span: any): span is Message.Time {
         return span?.event === "time";
     }
 
     export interface Error extends Base {
         event: "error",
@@ -75,15 +77,16 @@
 
     export interface Compilation extends Base {
         event: "compilation",
         source: Source,
         passes: Pass[],
         emitted: string,
         emit_time: number,
-        mech?: Mech.Machine
+        mech?: Mech.Machine,
+        task?: string
     }
     export function is_compilation(span: any): span is Message.Compilation {
         return span?.event === "compilation";
     }
 
     export type Event = Time | Error | Compilation;
 
@@ -112,14 +115,15 @@
 //------------------------------------------------------------------------------
 // Spans
 //------------------------------------------------------------------------------
 
 export namespace Span {
     export interface Base {
         event: "span",
+        parent?: Span,
         span_type: string,
         start_time: Date,
         end_time?: Date,
         elapsed?: number,
         selection_path: number[],
 
         events: (Span | Message.Event)[],
@@ -246,14 +250,15 @@
                 end_time: undefined,
                 span_type,
                 event: "span",
                 selection_path: this.path.slice(),
                 run: span_type === "program" ? ++this.run_counter : undefined,
                 events: []
             };
+            Object.defineProperty(sub, "parent", {value: unwrap(parent), enumerable: false, configurable: true, writable: true});
             parent.events.push(sub)
         }));
     }
 
     protected handle_span_end(msg: Message.SpanEnd) {
         this.set_root(produce((root) => {
             let start = get_in(root, this.path);
@@ -270,21 +275,21 @@
     }
 
     protected handle_event(msg: Message.Event) {
         this.set_root(produce((root) => {
             let span = get_in(root, this.path);
             if(!span || !Span.is_span(span)) throw new Error();
             msg.selection_path = [...this.path, span.events.length],
+            Object.defineProperty(msg, "parent", {value: unwrap(span), enumerable: false, configurable: true, writable: true});
             span.events.push(msg);
         }));
     }
 
     protected handle_message = (msg: Message) => {
         batch(() => {
-            console.log('msg', msg);
             if(msg.event === "span_start") this.handle_span_start(msg)
             else if(msg.event === "span_end") this.handle_span_end(msg)
             else this.handle_event(msg);
 
             this.set_messages((prev) => {
                 prev.push(msg);
                 return prev;
```

### Comparing `relationalai-0.2.5/frontend/debugger/src/logo.svg` & `relationalai-0.2.6/frontend/debugger/src/logo.svg`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/util.styl` & `relationalai-0.2.6/frontend/debugger/src/util.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/util.ts` & `relationalai-0.2.6/frontend/debugger/src/util.ts`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,22 @@
     if(list.length < prefix.length) return false;
     for(let ix = 0; ix < prefix.length; ix += 1) {
         if(list[ix] !== prefix[ix]) return false;
     }
     return true;
 }
 
+export function omit<T extends object, K extends keyof T>(v: T, ...keys: K[]): Omit<T, K> {
+    const copy = {...v};
+    for(const key of keys) {
+        delete copy[key];
+    }
+    return copy;
+}
+
 function fallback_copy_text_to_clipboard(text: string): Promise<void> {
     var textArea = document.createElement('textarea');
     textArea.value = text;
 
     // Avoid scrolling to bottom
     textArea.style.top = '0';
     textArea.style.left = '0';
```

### Comparing `relationalai-0.2.5/frontend/debugger/src/assets/favicon.png` & `relationalai-0.2.6/frontend/debugger/src/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/EventList.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/EventList.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import { Message, Span, client, type Subject } from "@src/debugger_client"
-import { Component, For, Show, useContext, type JSXElement } from "solid-js"
+import { Component, For, Show, children, createEffect, createSignal, untrack, useContext, type JSXElement } from "solid-js"
 import { Collapsible } from "./ui/Collapsible";
 import { EventListSelection } from "@src/Selection";
 import { Dynamic } from "solid-js/web";
 import { CodeBlock } from "./ui/Code";
 import "./EventList.styl";
 import { fmt, prefix_of } from "@src/util";
 import { Icon } from "./ui/Icon";
@@ -26,45 +26,66 @@
     )
 }
 
 export function EventListItem(props: EventListItemProps) {
     const component = (() => {
         const event = props.event;
         if (Span.is_program(event)) return EventItemProgram;
-        if (Span.is_block(event)) return EventItemBlock;
+        // if (Span.is_block(event)) return EventItemBlock;
         else if (Span.is_span(event)) return EventItemUnknownSpan;
         else if (Message.is_compilation(event)) return EventItemCompilation;
         else if (Message.is_time(event)) return EventItemTime;
         else return EventItemUnknown;
 
     }) as () => Component<EventListItemProps>;
 
     return (
-        <Dynamic component={component()} event={props.event} onclick={props.onclick} />
+        <Dynamic component={component()} event={props.event} selects={props.selects} />
     )
 }
 
 //------------------------------------------------------------------------------
 // Base components for event list items
 //------------------------------------------------------------------------------
 
 export interface EventListItemProps<T extends Subject = Subject> {
     event: T,
-    onclick?: (event: Subject) => any
+    selects?: Subject
 }
 
 interface EventListBranchProps<T extends Span = Span> extends EventListItemProps<T> {
     class?: string;
     children?: JSXElement;
     open?: boolean;
 }
 export function EventListBranch<T extends Span>(props: EventListBranchProps<T>) {
     const klass = () => `event-list-item branch ${props.event.event} ${props.event.span_type || ""} ${props.class || ""}`;
+
+    const selection = useContext(EventListSelection);
+    const contains_selection = () => selection.selected().some((subject) => {
+        const subject_path = subject.selection_path;
+        const span_path = props.event.selection_path;
+        if(subject_path.length < span_path.length) return false;
+        for(let ix = 0; ix < span_path.length; ix += 1) {
+            if(subject_path[ix] !== span_path[ix]) return false;
+        }
+        return true;
+    });
+
+    const [open, set_open] = createSignal(contains_selection());
+
+    createEffect(() => {
+        let should_be_open = contains_selection();
+        if (untrack(() => open()) !== should_be_open) {
+            set_open(should_be_open);
+        }
+    });
+
     return (
-        <Collapsible side="top" defaultOpen={props.open} class={klass()}>
+        <Collapsible side="top" open={open()} onOpenChange={set_open} class={klass()}>
             <Collapsible.Trigger as="header">
                 <Collapsible.TriggerIcon />
                 {props.children}
             </Collapsible.Trigger>
             <Collapsible.Content>
                 <EventList sub events={props.event.events} />
             </Collapsible.Content>
@@ -74,19 +95,17 @@
 
 interface EventListLeafProps<T extends Subject = Subject> extends EventListItemProps<T> {
     class?: string;
     children?: JSXElement;
 }
 export function EventListLeaf(props: EventListLeafProps<Subject>) {
     const selection = useContext(EventListSelection);
-    const klass = () => `event-list-item leaf ${props.event.event} ${props.event.span_type || ""} ${props.class || ""}`;
-    const onclick = () => {
-        if(props.onclick) props.onclick(props.event);
-        else selection?.select?.(props.event);
-    }
+    const is_selected = () => selection.is_selected(props.selects ?? props.event);
+    const klass = () => `event-list-item leaf ${props.event.event} ${props.event.span_type || ""} ${props.class || ""} ${is_selected() ? "selected" : ""}`;
+    const onclick = () => selection?.select?.(props.selects ?? props.event);
     return (
         <div class={klass()} onclick={onclick}>
             {props.children}
         </div>
     );
 }
 
@@ -111,78 +130,71 @@
                     {fmt.time.s(props.event.elapsed!)}
                 </Show>
             </span>
         </EventListBranch>
     )
 }
 
-export function EventItemBlock(props: EventListItemProps<Span.Block>) {
-    const selection = useContext(EventListSelection);
-    return (
-        <For each={props.event.events}>
-            {(event) => <EventListItem event={event} onclick={() => selection?.select(props.event)} />}
-        </For>
-    )
-}
-
-
 export function EventItemCompilation(props: EventListItemProps<Message.Compilation>) {
     let source = () => props.event?.source;
 
     return (
         <Show when={source()?.block}>
-            <EventListLeaf event={props.event} class="block naked" onclick={props.onclick}>
+            <EventListLeaf event={props.event} class="block naked" selects={props.selects}>
                 <header>
                     <span style="flex: 1" />
                     <span class="event-detail">
-                        <span class="file">{source()?.file}:</span>
+                        <span class="file">{source()?.file}</span>
+                        <span class="sep">:</span>
                         <span class="line">{source()?.line}</span>
                     </span>
                 </header>
                 <CodeBlock lang="python" dense no_copy>
                     {source()?.block}
                 </CodeBlock>
             </EventListLeaf>
         </Show>
     )
 }
 
 export function EventItemTime(props: EventListItemProps<Message.Time>) {
     return (
-        <EventListLeaf event={props.event} onclick={props.onclick}>
+        <EventListLeaf event={props.event} selects={props.selects}>
             <span class="event-label">
                 {props.event.type}
             </span>
             <span style="flex: 1" />
             <span class="event-detail">
                 {fmt.time.ms(props.event.elapsed * 1000)}
             </span>
         </EventListLeaf>
     )
 }
 
 export function EventItemUnknownSpan(props: EventListItemProps<Span>) {
-    return (
+    const selection = useContext(EventListSelection);
+    const is_selected = () => selection.is_selected(props.selects ?? props.event);
+    const klass = () => `event-list-item branch unknown ${is_selected() ? "selected" : ""}`;
+    const content = children(() => (
         <For each={props.event.events}>
-            {(event) => <EventListItem event={event} onclick={props.onclick} />}
+            {(event) => <EventListItem event={event} selects={props.selects} />}
         </For>
+    ));
+    return (
+        <Show when={content.toArray()?.filter((v) => v).length}>
+            <div class={klass()}>
+                {content()}
+            </div>
+        </Show>
     )
-
-    // return (
-    //     <EventListBranch event={props.event} class="unknown naked" open>
-    //         <span>
-    //             {props.event.span_type}
-    //         </span>
-    //     </EventListBranch>
-    // )
 }
 
 export function EventItemUnknown(props: EventListItemProps<Message.Event>) {
     return (
-        <EventListLeaf event={props.event} class="unknown" onclick={props.onclick}>
+        <EventListLeaf event={props.event} class="unknown" selects={props.selects}>
             <span>
                 {props.event.event}
             </span>
             <span>
                 {Message.is_time(props.event) ? props.event.type : undefined}
             </span>
         </EventListLeaf>
```

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Sidebar.styl` & `relationalai-0.2.6/frontend/debugger/src/components/Sidebar.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Sidebar.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/ScopeProvider.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/ScopeProvider.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -79,15 +79,17 @@
         this.used_names.add(name);
     }
 
     name(value: Mech.Value): string {
         let key = value?.id ?? value;
         if (!this.names.has(key)) {
             if (typeof value !== "object") return value;
-            throw new Error(`No name for variable ${value.id} is in scope!`);
+            // throw new Error(`No name for variable ${value.id} is in scope!`);
+            console.error(`No name for variable ${value.id} is in scope!`);
+            return `var${value.id}`;
         }
         return this.names.get(key)!;
     }
 
     named_after(value: Mech.Value, name: string) {
         let key = value?.id ?? value;
         // console.log("named after?", key, this.base_names.get(key), name);
```

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.stories.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.styl` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/index.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/base.styl` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/base.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/base.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/base.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/Schematic/nodes/index.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/Schematic/nodes/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Accordion.stories.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Accordion.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Accordion.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Accordion.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Button.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Button.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Code.styl` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Code.styl`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,19 @@
   position: relative;
 
   background: var(--code-block-bg, transparent);
   border: 1px solid var(--code-block-border, transparent);
   border-radius: 4px;
   box-shadow: inset 0 1px 5px var(--code-block-shadow);
 
+  &, & > code {
+    white-space: pre-wrap;
+    word-wrap: break-word;
+  }
+
   &.dense {
     padding: 4px 6px;
     font-size: 14px;
   }
 
   & > .code-controls {
     opacity: 0.1;
```

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Code.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Code.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,41 @@
-import { JSXElement, Ref, Show, createEffect, splitProps } from "solid-js";
+import { JSXElement, Ref, Show, children, createEffect, splitProps } from "solid-js";
 import "prismjs/themes/prism.css";
 import "prismjs/plugins/line-numbers/prism-line-numbers.css";
 import "prismjs/plugins/line-highlight/prism-line-highlight.css";
 import "prismjs/plugins/toolbar/prism-toolbar.css";
 import Prism from "prismjs";
 import { Button } from "./Button";
 import { Icon } from "./Icon";
 import "./Code.styl";
 import { copy_text_to_clipboard } from "@src/util";
 
-Prism.languages.rel = {
-    'comment': /\/\/.*/,
-    'keyword': /\b(def|module|from)\b/,
-    'operator': /=/,
-    'function': /[a-z_]\w*(?=\[)/,
-    // ... other patterns
-};
+Prism.languages.rel = Prism.languages.python;
 
 export interface CodeProps {
     ref?: Ref<HTMLElement>;
     class?: string,
-    children: JSXElement,
+    children: string|undefined,
     lang?: string
 }
 export function Code(props: CodeProps) {
     let ref!:HTMLElement;
     createEffect(() => {
-        props.children;
+        ref.textContent = props.children ?? ""; // prism doing its thing breaks solid updating the value itself.
         Prism.highlightElement(ref);
     });
 
     const lang_class = () => props.lang ? `language-${props.lang}` : "";
     const set_ref = (elem: HTMLElement) => {
         ref = elem;
         typeof props.ref === "function" ? props.ref(elem) : props.ref = elem;
     };
 
     return (
-        <code ref={set_ref} class={`ui-code ${lang_class()} ${props.class || ""}`}>
-            {props.children}
-        </code>
+        <code ref={set_ref} class={`ui-code ${lang_class()} ${props.class || ""}`} textContent={props.children} />
     )
 }
 
 
 export interface CodeBlockProps extends Omit<CodeProps, "ref"> {
     ref?: Ref<HTMLPreElement>;
     no_copy?: boolean,
```

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.stories.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.styl` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Collapsible.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Collapsible.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Field.stories.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Field.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Field.styl` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Field.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Field.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Field.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Icon.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Icon.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.stories.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.styl` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Modal.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Modal.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.stories.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.styl` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/components/ui/Tooltip.tsx` & `relationalai-0.2.6/frontend/debugger/src/components/ui/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/fixtures/branch-improved.json` & `relationalai-0.2.6/frontend/debugger/src/fixtures/branch-improved.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/fixtures/branch.json` & `relationalai-0.2.6/frontend/debugger/src/fixtures/branch.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/fixtures/fraud.json` & `relationalai-0.2.6/frontend/debugger/src/fixtures/fraud.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/fixtures/not_found.json` & `relationalai-0.2.6/frontend/debugger/src/fixtures/not_found.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/fixtures/simple.json` & `relationalai-0.2.6/frontend/debugger/src/fixtures/simple.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/fixtures/union.json` & `relationalai-0.2.6/frontend/debugger/src/fixtures/union.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/frontend/debugger/src/types/mech.d.ts` & `relationalai-0.2.6/frontend/debugger/src/types/mech.d.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/README.md` & `relationalai-0.2.6/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/emit.py` & `relationalai-0.2.6/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/exec.py` & `relationalai-0.2.6/src/gentest/exec.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 import rich
 from rich.syntax import Syntax
 
 from relationalai.clients.test import Document, Query
 from relationalai import clients, debugging
+from relationalai.errors import RelQueryError
 from gentest.util import PROJECT_DIR
 from gentest.validate.roundtrip import exec_and_run_callback
 
 AzureClient = clients.azure.Client
 SnowflakeClient = clients.snowflake.Client
 AzureProxyClient = clients.test.proxy_client(AzureClient)
 SnowflakeProxyClient = clients.test.proxy_client(SnowflakeClient)
@@ -36,14 +37,17 @@
         with proxy_clients():
             # @TODO: Consider suppressing stdout
             doc: Document = exec_and_run_callback(code, None, ns=ns)
             for block in doc.blocks:
                 if isinstance(block, Query):
                     try:
                         snapshot.assert_match(str(block.result), f"query{block.ix}.txt")
+                    except RelQueryError as err:
+                        err.pprint()
+                        raise err from None
                     except AssertionError as err:
                         header, info, _, *body = str(err).splitlines()
                         with io.StringIO() as buf:
                             console = rich.console.Console(file=buf, force_terminal=True)
                             console.print(header)
                             console.print(info)
```

### Comparing `relationalai-0.2.5/src/gentest/fixtures.py` & `relationalai-0.2.6/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/patch.py` & `relationalai-0.2.6/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/util.py` & `relationalai-0.2.6/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/cli/__main__.py` & `relationalai-0.2.6/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/cli/collect_failures.py` & `relationalai-0.2.6/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/cli/collect_tests.py` & `relationalai-0.2.6/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/cli/repro.py` & `relationalai-0.2.6/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/cli/watch.py` & `relationalai-0.2.6/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/gen/action.py` & `relationalai-0.2.6/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/gen/context.py` & `relationalai-0.2.6/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/gen/document.py` & `relationalai-0.2.6/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/gen/group_limited.py` & `relationalai-0.2.6/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/gen/ir.py` & `relationalai-0.2.6/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/gen/scope.py` & `relationalai-0.2.6/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/gen/task.py` & `relationalai-0.2.6/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/gen/test.py` & `relationalai-0.2.6/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/harness/database.py` & `relationalai-0.2.6/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/validate/diff.py` & `relationalai-0.2.6/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/validate/errors.py` & `relationalai-0.2.6/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/validate/mapping.py` & `relationalai-0.2.6/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/gentest/validate/roundtrip.py` & `relationalai-0.2.6/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/__init__.py` & `relationalai-0.2.6/src/relationalai/__init__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/compiler.py` & `relationalai-0.2.6/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/debugging.py` & `relationalai-0.2.6/src/relationalai/debugging.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/dsl.py` & `relationalai-0.2.6/src/relationalai/dsl.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,19 @@
     def __rsub__(self, other):
         return self._wrapped_op(Builtins.minus, other, self)
 
     def __truediv__(self, other):
         return self._wrapped_op(Builtins.div, self, other)
     def __rtruediv__(self, other):
         return self._wrapped_op(Builtins.div, other, self)
+    
+    def __floordiv__(self, other):
+        return self._wrapped_op(Builtins.floor_div, self, other)
+    def __rfloordiv__(self, other):
+        return self._wrapped_op(Builtins.floor_div, other, self)
 
     def __pow__(self, other):
         return self._wrapped_op(Builtins.pow, self, other)
     def __rpow__(self, other):
         return self._wrapped_op(Builtins.pow, other, self)
 
     def __mod__(self, other):
@@ -264,29 +269,30 @@
 
         graph = self._context.graph
         graph._action(build.return_([item, *[kwargs[k] for k in self._props.keys()]]))
 
 class Context():
     def __init__(self, graph:'Graph', *args, behavior=Behavior.Query, op=None,
                  exec_type=TaskExecType.Rule, dynamic=False, name="None",
-                 inputs=None, outputs=None, engine=None):
+                 inputs=None, outputs=None, engine=None, tag=None):
         self._id = next_id()
         self.results = DataFrame()
         self.graph = graph
         self._task = Task(behavior=behavior)
         self._op = op
         self._args = list(args)
         self._exec_type = exec_type
         self._select_len = None
         self._rel = None
         self._dynamic = dynamic
         self._name = name
         self._inputs = inputs
         self._outputs = outputs
         self._engine= engine
+        self._tag = tag # for benchmark reporting
 
     def __enter__(self):
         debugging.set_source(self._task, dynamic=self._dynamic)
         self.graph._push(self)
         return ContextSelect(self)
 
     def __exit__(self, *args):
@@ -1130,15 +1136,15 @@
     def _remove_action(self, action):
         self._stack.items.remove(action)
 
     def _exec(self, context:Context, task):
         if context._exec_type == TaskExecType.Rule:
             self._client.install(f"rule{len(self._executed)}", context._task)
         elif context._exec_type == TaskExecType.Query:
-            context.results = self._client.query(context._task)
+            context.results = self._client.query(context._task, tag=context._tag)
         elif context._exec_type == TaskExecType.Procedure:
             self._client.export_udf(context._name, context._inputs, context._outputs, context._task, context._engine)
         self._executed.append(context)
 
     #--------------------------------------------------
     # Property handling
     #--------------------------------------------------
```

### Comparing `relationalai-0.2.5/src/relationalai/errors.py` & `relationalai-0.2.6/src/relationalai/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/metagen.py` & `relationalai-0.2.6/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/metamodel.py` & `relationalai-0.2.6/src/relationalai/metamodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,14 +413,16 @@
         self.eq = binary_op("=")
         self.neq = binary_op("!=")
 
         self.plus = binary_op("+", True)
         self.minus = binary_op("-", True)
         self.mult = binary_op("*", True)
         self.div = binary_op("/", True)
+        self.floor_div = binary_op("floor_divide", True)
+        self.floor_div.parents = []
 
         self.pow = binary_op("^", True)
         self.mod = binary_op("modulo", True)
         self.mod.parents = []
 
         self.count = aggregate("count")
         self.sum = aggregate("sum")
```

### Comparing `relationalai-0.2.5/src/relationalai/rel.py` & `relationalai-0.2.6/src/relationalai/rel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/rel2.py` & `relationalai-0.2.6/src/relationalai/rel2.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/rel_emitter.py` & `relationalai-0.2.6/src/relationalai/rel_emitter.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/rel_utils.py` & `relationalai-0.2.6/src/relationalai/rel_utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/analysis/mechanistic.py` & `relationalai-0.2.6/src/relationalai/analysis/mechanistic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/analysis/whynot.py` & `relationalai-0.2.6/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/clients/azure.py` & `relationalai-0.2.6/src/relationalai/clients/azure.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/clients/client.py` & `relationalai-0.2.6/src/relationalai/clients/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,19 +288,19 @@
 
     def install_raw(self, code:str, name:str="pyrel_batch_0"):
         if not name:
             name = "pyrel_batch_0"
         self.compiler.compile(dsl.build.raw_task(code))
         self._install_batch.append(name, code)
 
-    def query(self, task:m.Task, rentrant=False, readonly=True, raw_results=False, inputs={}) -> DataFrame|Any:
+    def query(self, task:m.Task, rentrant=False, readonly=True, raw_results=False, inputs={}, tag=None) -> DataFrame|Any:
         if self._install_batch.is_dirty():
             self._install_batch_flush()
 
-        with debugging.span("query", model=self._database, task=task) as end_span:
+        with debugging.span("query", model=self._database, task=task, tag=tag) as end_span:
             code = self.compiler.compile(task)
             if task.has_persist():
                 readonly = False
             if self.dry_run:
                 return DataFrame()
 
             start = time.perf_counter()
```

### Comparing `relationalai-0.2.5/src/relationalai/clients/config.py` & `relationalai-0.2.6/src/relationalai/clients/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,19 +188,25 @@
     if file.endswith(".toml"):
         try:
             cf = ConfigFile(file, toml.load(file))
             cf.apply_keymap()
             return cf
         except toml.TomlDecodeError as e:
             raise Exception(f"Error parsing {file}: {e}")
-    config = configparser.ConfigParser()
-    config.read(file)
-    cf = ConfigFile(file, {k: v for k, v in config.items() if k != "DEFAULT"}, format="ini")
-    cf.apply_keymap()
-    return cf
+    else:
+        try:
+            config = configparser.ConfigParser()
+            config.read(file)
+            cf = ConfigFile(file, {k: v for k, v in config.items() if k != "DEFAULT"}, format="ini")
+            cf.apply_keymap()
+            return cf
+        except Exception:
+            # silently ignore parsing errors for INI files because
+            # they are inessential to the flow
+            return ConfigFile(cfg={})
 
 def _get_full_config(profile:str|None=None) -> tuple[Dict[str,Any], str|None]:
     """
     Returns a dictionary representing the props to be used for the currently active profile. Incorporates the following rules:
     1. The `snowflake_connection` key fills in the properties from the Snowflake connections.toml file.
     2. Profiles with the same name are merged in order of appearance, with earlier profiles taking precedence.
     3. The profile indicated by the `active_profile` key is merged into other top-level properties.
```

### Comparing `relationalai-0.2.5/src/relationalai/clients/snowflake.py` & `relationalai-0.2.6/src/relationalai/clients/snowflake.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from ..clients.types import AvailableModel, Import, ImportSource, ImportSourceTable
 from ..clients.config import Config
 from ..clients.client import Client, ResourceProvider
 from .. import dsl, rel, metamodel as m
 from ..errors import Errors, RAIException
 from .. import std
 import re
+from concurrent.futures import ThreadPoolExecutor
 
 #--------------------------------------------------
 # Constants
 #--------------------------------------------------
 
 USE_EXEC_ASYNC = True
 VALID_POOL_STATUS = ["ACTIVE", "IDLE", "SUSPENDED"]
@@ -155,25 +156,27 @@
         return [{"name":name, "size":size, "state":state}
                 for (name, size, state) in results.fetchall()]
 
     def get_engine(self, name:str):
         results = self._exec(f"select NAME, SIZE, STATUS from {APP_NAME}.api.engines WHERE NAME='{name}'")
         if not results:
             return None
-        return [{"name":name, "size":size, "state":state}
-                for (name, size, state) in results.fetchall()][0]
+        engine = results.fetchone()
+        if not engine:
+            return None
+        return {"name": engine[0], "size": engine[1], "state": engine[2]}
 
     def create_engine(self, name:str, size:str, pool:str = ""):
         if not pool:
             raise ValueError("Pool is required")
         try:
             with debugging.span("create_engine", name=name, size=size, pool=pool):
                 self._exec(f"call {APP_NAME}.api.create_engine('{name}', '{pool}', '{size}');")
         except Exception as e:
-            raise Exception(f"Failed to create engine {name} using pool {pool} and size {size}") from e
+            raise Exception(f"Failed to create engine {name} using pool {pool} and size {size}: {e}") from e
 
     def delete_engine(self, name:str):
         self._exec(f"call {APP_NAME}.api.delete_engine('{name}');")
 
     def suspend_engine(self, name:str):
         raise Exception("Not implemented")
 
@@ -427,27 +430,51 @@
     def _list_exec_async_artifacts(self, txn_id: str) -> Dict[str, str]:
         """Grab the list of artifacts produced in the transaction and the URLs to retrieve their contents."""
         with debugging.span("list_results"):
             response = self._exec(f"CALL {APP_NAME}.api.list_transaction_outputs('{txn_id}');")
             assert response, f"No results from list_transaction_outputs('{txn_id}')"
             return {name: url for name, url in response}
 
-    def _fetch_exec_async_artifacts(self, artifact_urls: Dict[str, str]) -> Dict[str, Any]:
-        """Grab the contents of the given artifacts from SF."""
+    def _fetch_data(self, session, name_url):
+        name, url = name_url
+        response = session.get(url)
+        response.raise_for_status()  # Throw if something goes wrong
+        if name.endswith(".json"):
+            return name, response.json()
+        else:
+            return name, response.content
+
+    def _fetch_exec_async_artifacts(
+        self, artifact_urls: Dict[str, str]
+    ) -> Dict[str, Any]:
+        """Grab the contents of the given artifacts from SF in parallel using threads."""
         contents = {}
-        with debugging.span("fetch_results"):
-            with requests.Session() as session:
-                for name, url in artifact_urls.items():
-                    with debugging.span("fetch_result", name=name):
-                        response = session.get(url)
-                    response.raise_for_status() # throw if something goes wrong.
-                    if name.endswith(".json"):
-                        contents[name] = response.json()
-                    else:
-                        contents[name] = response.content
+
+        with requests.Session() as session:
+            # Define _fetch_data inside the session context to close over 'session'
+            def _fetch_data(name_url):
+                name, url = name_url
+                response = session.get(url)
+                response.raise_for_status()  # Throw if something goes wrong
+                if name.endswith(".json"):
+                    return name, response.json()
+                else:
+                    return name, response.content
+
+            # Create a list of tuples for the map function
+            name_url_pairs = list(artifact_urls.items())
+
+            # Create ThreadPoolExecutor to handle requests in parallel
+            with ThreadPoolExecutor(max_workers=5) as executor:
+                # Map fetch across all URLs using the executor
+                results = executor.map(_fetch_data, name_url_pairs)
+
+                # Populate contents dictionary
+                for name, data in results:
+                    contents[name] = data
 
         return contents
 
     def _parse_exec_async_results(self, arrow_files: List[Tuple[str, bytes]]):
         """Mimics the logic in _parse_arrow_results of railib/api.py#L303 without requiring a wrapping multipart form."""
         results = []
 
@@ -455,22 +482,52 @@
             with pa.ipc.open_stream(file_content) as reader:
                 schema = reader.schema
                 batches = [batch for batch in reader]
                 table = pa.Table.from_batches(batches=batches, schema=schema)
                 results.append({"relationId": file_name, "table": table})
 
         return results
+    
+    def _download_results(self, artifact_urls, txn_id):
+        with debugging.span("download_results"):
+            # Fetch artifacts
+            artifacts = self._fetch_exec_async_artifacts(artifact_urls)
+
+            # Parse metadata from the artifacts
+            meta = _parse_metadata_proto(artifacts["metadata.proto"])
+            meta_json = artifacts["metadata.json"]
+
+            # Use the metadata to map arrow files to the relations they contain
+            arrow_files_to_relations = {}
+            for ix, relation in enumerate(meta.relations):
+                arrow_file = relation.file_name
+                relation_id = meta_json[ix]["relationId"]
+                arrow_files_to_relations[arrow_file] = relation_id
+
+            # Hydrate the arrow files into tables
+            results = self._parse_exec_async_results([
+                (arrow_files_to_relations[name], content) for name, content in artifacts.items() if name.endswith(".arrow")
+            ])
+
+            # Create and return the response
+            rsp = TransactionAsyncResponse()
+            rsp.transaction = {"id": txn_id, "state": "COMPLETED", "response_format_version": None}
+            rsp.metadata = meta
+            rsp.problems = artifacts.get("problems.json")  # Safely access possible missing keys
+            rsp.results = results
+            return rsp
+
 
     def _exec_async_raw(self, database:str, engine:str, raw_code:str, readonly=True, inputs={}):
         with debugging.span("transaction") as txn_span:
             if inputs:
                 raise Exception("Inputs aren't currently supported using exec_async in SPCS.")
 
             with debugging.span("create"):
-                response = self._exec(f"CALL {APP_NAME}.api.exec_async('{database}','{engine}','{raw_code}', {readonly});")
+                response = self._exec(f"CALL {APP_NAME}.api.exec_async('{database}','{engine}', %s, {readonly});", raw_code)
                 if not response:
                     raise Exception("No results from exec_async")
 
             # Grab the txn_id from the response
             txn_id, status = next(iter(response))
             txn_span["txn_id"] = txn_id
             # Wait for completion or failure
@@ -480,40 +537,16 @@
                     poll_with_specified_overhead(lambda: self._check_exec_async_status(txn_id), 0.2)
 
             self._pending_transactions.remove(txn_id)
 
             with debugging.span("fetch"):
                 # List the result artifacts (and the URLs to retrieve them)
                 artifact_urls = self._list_exec_async_artifacts(txn_id)
-                # Actually retrieve them
-                artifacts = self._fetch_exec_async_artifacts(artifact_urls)
-
-                meta = _parse_metadata_proto(artifacts["metadata.proto"])
-                meta_json = artifacts["metadata.json"]
-
-                # We use the metadata to map arrow files to the relations they contain data for.
-                # In Azure, this is provided sideband via response headers.
-                arrow_files_to_relations = {}
-                for ix, relation in enumerate(cast(Any, meta).relations):
-
-                    arrow_file = relation.file_name
-                    relation_id = meta_json[ix]["relationId"]
-                    arrow_files_to_relations[arrow_file] = relation_id
-
-                # Hydrate the arrow files into tables
-                results = self._parse_exec_async_results([(arrow_files_to_relations[name], content) for name, content in artifacts.items() if name.endswith(".arrow")])
-
-                rsp = TransactionAsyncResponse()
-                # @FIXME: Hardcoding the `state` feels somewhat unsafe, but we can't have gotten here in the code otherwise.
-                # @FIXME: Missing `response_format_version`, which isn't obviously present anywhere in the results.
-                rsp.transaction = {"id": txn_id, "state": "COMPLETED", "response_format_version": None}
-                rsp.metadata = meta
-                rsp.problems = artifacts["problems.json"]
-                rsp.results = results
-                return rsp
+                
+                return self._download_results(artifact_urls, txn_id)
 
     # Copied directly from azure.py
     def _has_errors(self, results):
         if len(results.problems):
             for problem in results.problems:
                 if problem['is_error'] or problem['is_exception']:
                     return True
```

### Comparing `relationalai-0.2.5/src/relationalai/clients/test.py` & `relationalai-0.2.6/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/clients/types.py` & `relationalai-0.2.6/src/relationalai/clients/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/loaders/csv.py` & `relationalai-0.2.6/src/relationalai/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/loaders/loader.py` & `relationalai-0.2.6/src/relationalai/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/loaders/types.py` & `relationalai-0.2.6/src/relationalai/loaders/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/std/aggregates.py` & `relationalai-0.2.6/src/relationalai/std/aggregates.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/std/graphs.py` & `relationalai-0.2.6/src/relationalai/std/graphs.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,14 +93,30 @@
     # --------------------------------------------------
 
     def num_nodes(self):
         return self._lib.num_nodes(self._graph)
 
     def num_edges(self):
         return self._lib.num_edges(self._graph)
+    
+    # --------------------------------------------------
+    # Distance
+    # --------------------------------------------------
+    
+    def distance(self, node1, node2):
+        return self._lib.distance(self._graph, node1, node2)
+    
+    def weighted_distance(self, node1, node2):
+        return self._lib.weighted_distance(self._graph, node1, node2)
+    
+    def diameter_range(self):
+        min, max = Vars(2)
+        self._lib.diameter_range(self._graph, "min", min)
+        self._lib.diameter_range(self._graph, "max", max)
+        return (min, max)
 
     # --------------------------------------------------
     # Connectivity
     # --------------------------------------------------
 
     def is_connected(self):
         model = self._graph.model
@@ -122,14 +138,51 @@
                 self._lib.transitive_closure(self._graph, node1, node2)
                 v.add(True)
             with model.scope():
                 v.add(False)
         return v
 
     # --------------------------------------------------
+    # Triangles
+    # --------------------------------------------------
+
+    def num_triangles(self, node=None):
+        if node is None:
+            return self._lib.num_triangles(self._graph)
+        return self._lib.triangle_count(self._graph, node)
+
+    def is_triangle(self, node1, node2, node3):
+        model = dsl.get_graph()
+        with model.ordered_choice() as v:
+            with model.scope():
+                self._lib.triangle(self._graph, node1, node2, node3)
+                v.add(True)
+            with model.scope():
+                v.add(False)
+        return v
+
+    def triangles(self, node=None):
+        # If no node is provided, return all triangles in the graph,
+        # unique up to ordering of the nodes.
+        if node is None:
+            x, y, z = Vars(3)
+            self._lib.unique_triangle(self._graph, x, y, z)
+            return (x, y, z)
+        # If a node is provided, return all triangles that include that node,
+        # unique up to order of the nodes.
+        x, y = Vars(2)
+        model = dsl.get_graph()
+        with model.union(dynamic=True) as t:
+            for (a, b, c) in ([node, x, y], [x, node, y], [x, y, node]):
+                with model.scope():
+                    self._lib.unique_triangle(self._graph, a, b, c)
+                    t.add(node, a=a, b=b, c=c)
+        return (t.a, t.b, t.c)
+
+    # --------------------------------------------------
     # Link Prediction
     # --------------------------------------------------
 
     def adamic_adar(self, node1, node2):
         return self._lib.adamic_adar(self._graph, node1, node2)
 
     def preferential_attachment(self, node1, node2):
@@ -143,17 +196,25 @@
     # --------------------------------------------------
 
     def cosine_similarity(self, node1, node2):
         if not self._graph.undirected:
             invalid_param("graph", "must be undirected")
         return self._lib.cosine_similarity(self._graph, node1, node2)
 
+    def weighted_cosine_similarity(self, node1, node2):
+        if not self._graph.undirected:
+            invalid_param("graph", "must be undirected")
+        return self._lib.weighted_cosine_similarity(self._graph, node1, node2)
+
     def jaccard_similarity(self, node1, node2):
         return self._lib.jaccard_similarity(self._graph, node1, node2)
 
+    def weighted_jaccard_similarity(self, node1, node2):
+        return self._lib.weighted_jaccard_similarity(self._graph, node1, node2)
+
     # --------------------------------------------------
     # Centrality
     # --------------------------------------------------
 
     def pagerank(self, node, damping_factor=0.85, tolerance=1e-6, max_iter=20):
         between("damping_factor", damping_factor, 0, 1)
         positive("tolerance", tolerance)
```

### Comparing `relationalai-0.2.5/src/relationalai/tools/cli.py` & `relationalai-0.2.6/src/relationalai/tools/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from .cli_controls import divider, Spinner
 from . import cli_controls as controls
 
 #--------------------------------------------------
 # Constants
 #--------------------------------------------------
 
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 ENGINE_SIZES = ["XS", "S", "M", "L", "XL"]
 PROFILE = None
 
 SNOWFLAKE = "Snowflake"
 AZURE = "Azure (Beta)"
 
 AZURE_ENVS = {
@@ -229,15 +230,15 @@
             cur[key_parts[-1]] = val
         return options
 
 #--------------------------------------------------
 # Main group
 #--------------------------------------------------
 
-@click.group(cls=RichGroup)
+@click.group(cls=RichGroup, context_settings=CONTEXT_SETTINGS)
 @click.option("--profile", help="Which config profile to use")
 def cli(profile):
     global PROFILE
     PROFILE = profile
 
 #--------------------------------------------------
 # Init
@@ -278,20 +279,22 @@
     """Inverse of os.path.expanduser"""
     home_dir = os.path.expanduser('~')
     if path.startswith(home_dir):
         return '~' + path[len(home_dir):]
     return path
 
 def account_from_url(account_or_url:str):
-    regex = r"https://app.snowflake.com/([^/]+)/([^/]+)/.*"
+    regex = r"https://app.snowflake.com/([^/]+)/([^/]+)/?.*"
     match = re.match(regex, account_or_url)
     if match:
         org = match.group(1)
         account = match.group(2)
         return f"{org}-{account}"
+    elif "app.snowflake.com" in account_or_url or "https://" in account_or_url:
+        raise ValueError("URL not of the form https://app.snowflake.com/[org]/[account]")
     else:
         return account_or_url
 
 def snowflake_flow(cfg:config.Config):
     pyrel_config = check_original_config_flow(cfg, "snowflake")
     if not pyrel_config:
         check_snowflake_connections_flow(cfg)
@@ -546,16 +549,17 @@
         profile = controls.fuzzy("Select a profile:", profiles)
         divider()
     else:
         if profile not in profiles:
             rich.print(f"[yellow]Profile '{profile}' not found")
             divider()
             sys.exit(1)
-    cfg.profile = profile
-    cfg.save()
+    cfg.original_toml["active_profile"] = profile
+    with open(CONFIG_FILE, "w") as f:
+        f.write(cfg.original_toml.as_string())
     rich.print(f"[green]✓ Switched to profile '{profile}'")
     divider()
 
 #--------------------------------------------------
 # Explain config
 #--------------------------------------------------
 
@@ -634,15 +638,14 @@
             sys.exit(1)
     rich.print("[green]✓ Connection successful!")
 
 #--------------------------------------------------
 # Version
 #--------------------------------------------------
 
-
 def latest_version(package_name):
     """Get the current version of a package on PyPI."""
     url = f"https://pypi.org/pypi/{package_name}/json"
     response = requests.get(url)
     if response.status_code == 200:
         data = response.json()
         version = data['info']['version']
@@ -664,31 +667,31 @@
 
     divider()
     print_version("RelationalAI", __version__, latest_version("relationalai"))
     print_version("Rai-sdk", railib_version, latest_version("rai-sdk"))
     print_version("Python", sys.version.split()[0])
 
     try:
-        cfg = get_config(CONFIG_FILE)
+        cfg = get_config()
         if not cfg.file_path:
             table.add_row("[bold]App", "No configuration file found. To create one, run: [green]rai init")
         else:
-            platform = cfg.get("platform")
+            platform = cfg.get("platform", None)
             if platform == "snowflake":
                 # print()
                 with Spinner("Checking app version"):
                     try:
                         app_version = get_resource_provider().get_version()
                     except Exception as e:
                         rich.print(f"\n\n[yellow]Error fetching app version: {e}")
                         exit(1)
                 print_version("App", app_version)
 
     except Exception as e:
-        rich.print(f"[yellow]Error fetching platform: {e}")
+        rich.print(f"[yellow]Error checking app version: {e}")
         divider()
         exit(1)
 
     rich.print(table)
     divider()
 
 #--------------------------------------------------
@@ -724,14 +727,44 @@
             table.add_row(engine.get("name"), engine.get("size"), engine.get("state"))
         rich.print(table)
     else:
         rich.print("[yellow]No engines found")
 
     divider()
 
+@cli.command(name="engines:get", help="Get engine details")
+@click.option("--name", help="Name of the engine")
+def engines_get(name):
+    divider(flush=True)
+    ensure_config()
+
+    if not name:
+        name = controls.text("Engine name:", validator=ENGINE_NAME_REGEX.match, invalid_message=ENGINE_NAME_ERROR)
+        rich.print("")
+
+    with Spinner("Fetching engine"):
+        try:
+            engine = get_resource_provider().get_engine(name)
+        except Exception as e:
+            rich.print(f"\n\n[yellow]Error fetching engine: {e}")
+            divider(flush=True)
+            exit(1)
+
+    if engine:
+        table = Table(show_header=True, border_style="dim", header_style="bold", box=rich_box.SIMPLE_HEAD)
+        table.add_column("Name")
+        table.add_column("Size")
+        table.add_column("State")
+        table.add_row(engine.get("name"), engine.get("size"), engine.get("state"))
+        rich.print(table)
+    else:
+        rich.print("[yellow]Engine not found")
+
+    divider()
+
 #--------------------------------------------------
 # Engine create
 #--------------------------------------------------
 
 @cli.command(name="engines:create", help="Create a new engine")
 @click.option("--name", help="Name of the engine")
 @click.option("--size", type=click.Choice(ENGINE_SIZES, case_sensitive=False), help="Size of the engine")
@@ -1270,15 +1303,15 @@
         table.add_column("Schema")
         table.add_column("State")
         table.add_column("Created")
         table.add_column("Duration", justify="right")
 
         added = 0
         for txn in transactions:
-            if not all_users and txn.get("created_by").lower() != config.get("user", "").lower():
+            if not all_users and txn.get("created_by", "").lower() != config.get("user", "").lower():
                 continue
             if added >= limit:
                 break
 
             match txn.get("state", "").lower():
                 case "aborted":
                     style = "red"
```

### Comparing `relationalai-0.2.5/src/relationalai/tools/cli_controls.py` & `relationalai-0.2.6/src/relationalai/tools/cli_controls.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/tools/debugger.py` & `relationalai-0.2.6/src/relationalai/tools/debugger.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,52 +85,52 @@
 
 @ui.refreshable
 def my_stuff():
     total_time = 0
     with ui.column():
 
         for (ix, obj) in enumerate(current_json_objects):
-            if 'span' in obj['event']:
-                continue
+            me = None
 
             if obj['event'] == "compilation":
                 me = code(obj["source"]["block"] or obj["emitted"])
                 total_time += obj["emit_time"]
                 for p in obj['passes']:
                     total_time += p['elapsed']
             elif obj['event'] == "time":
                 total_time += obj['elapsed']
                 with ui.row() as me:
                     me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
                     ui.label(f"{obj['type']}")
                     ui.label(format_time(obj['elapsed']))
                     if obj.get('results'):
                         ui.label(f"{obj['results']['count']}")
-            elif obj['event'] == "transaction":
+            elif obj['event'] == "span_start" and obj['span']['type'] == "wait":
                 with ui.row() as me:
                     me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
-                    ui.label(f"{obj['event']}")
-                    ui.label(obj["txn_id"])
+                    ui.label("transaction")
+                    ui.label(obj["span"]["attrs"]["txn_id"])
             elif obj.get('type'):
                 total_time += obj.get('elapsed', 0)
                 with ui.row() as me:
                     me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
                     ui.label(f"{obj['type']}")
                     ui.label(format_time(obj.get('elapsed', 0)))
                     if obj.get('results'):
                         ui.label(f"{obj['results']['count']}")
-            else:
+            elif 'span' not in obj['event']:
                 with ui.row() as me:
                     me.style("padding: 5px 10px; border: 1px solid #544; border-radius: 5px; background:#322;")
                     ui.label(f"{obj['event']}")
 
-            me.classes("w-full")
-            me.on("click", lambda ix=ix: set_item(ix))
-            if ix != active_ix:
-                me.style('opacity: 0.5')
+            if me:
+                me.classes("w-full")
+                me.on("click", lambda ix=ix: set_item(ix))
+                if ix != active_ix:
+                    me.style('opacity: 0.5')
         with ui.row() as me:
             me.style("padding: 5px 10px; border: 1px solid #445; border-radius: 5px; background:#223; opacity: 0.5;")
             me.classes("w-full")
             if total_time > 1:
                 ui.label(f"Total time: {total_time:.1f}s")
             else:
                 ui.label(f"Total time: {total_time * 1000:.0f}ms")
```

### Comparing `relationalai-0.2.5/src/relationalai/tools/debugger_server.py` & `relationalai-0.2.6/src/relationalai/tools/debugger_server.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/tools/dev.py` & `relationalai-0.2.6/src/relationalai/tools/dev.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/src/relationalai/util/snowflake_logger.py` & `relationalai-0.2.6/src/relationalai/util/snowflake_logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import threading
 import time
 
 import logging
 import traceback
 import uuid
 
-from relationalai.debugging import Span
+from relationalai.util.keys import get_key
 
 # Don't insert these as attrs since they get their own columns
 FILTER_ATTRS = {
     "event",
     "span",
     "id",
     "parent_id",
@@ -19,14 +19,20 @@
     "start_timestamp",
     "end_time",
     "end_timestamp",
     "elapsed",
 }
 
 class SnowflakeLogger(logging.Handler):
+    """
+    This is a logging handler that inserts spans directly into a Snowflake table.
+
+    It uses a queue and a worker thread to buffer spans and then insert them in batches.
+    """
+    
     def __init__(self, snowflake_conn, sleep_interval_s=2):
         super().__init__()
         self.trace_id = uuid.uuid4()
         self.snowflake_conn = snowflake_conn
         self.queue = queue.Queue()
         self.is_shut_down = False
         self.sleep_interval_s = sleep_interval_s
@@ -70,19 +76,25 @@
     
         for event in batch:
             if event["event"] == "span_start":
                 span = event["span"]
                 self.open_spans[str(span.id)] = span
             elif event["event"] == "span_end":
                 span = self.open_spans.pop(event["id"])
+                # assemble attributes
                 filtered_attrs = {}
                 for k, v in span.attrs.items():
                     if k not in FILTER_ATTRS:
                         filtered_attrs[k] = v
+                for k, v in event["end_attrs"].items():
+                    if k not in FILTER_ATTRS:
+                        filtered_attrs[k] = v
+                # get key
                 span_key = get_key(span)
+                # add to batch
                 inserts.append({
                     "id": str(span.id),
                     "parent_id": None if span.parent is None else str(span.parent.id),
                     "trace_id": str(self.trace_id),
                     "key": str(span_key) if span_key is not None else None,
                     "type": span.type,
                     "start_ts": span.start_timestamp,
@@ -102,23 +114,9 @@
     
     def shut_down(self):
         self.is_shut_down = True
         print('snowflake logger: waiting to shut down...')
         self.worker_thread.join()
         print('snowflake logger: shut down')
 
-# === helpers ===
-
-SPAN_KEYS = {
-    'test': 'name',
-    'run': 'idx',
-}
-
-def get_key(span: 'Span'):
-    type = span.type
-    if type in SPAN_KEYS:
-        key = SPAN_KEYS[type]
-        return span.attrs[key]
-    return None
-
 def default_serialize(obj):
     return '<skipped>'
```

### Comparing `relationalai-0.2.5/tests/conftest.py` & `relationalai-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/README.md` & `relationalai-0.2.6/tests/end2end/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/conftest.py` & `relationalai-0.2.6/tests/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,44 @@
-import os
 import random
+import os
 
-import pytest
 import snowflake.connector
 
 import relationalai as rai
-from relationalai.clients import config as cfg
+from relationalai import debugging
 from relationalai.debugging import logger
+from relationalai.clients import config as cfg
 from relationalai.util.snowflake_logger import SnowflakeLogger
 
+def engine_config_fixture():
+    # Check for an externally provided engine name
+    # It is used in GitHub Actions to run tests against a specific engine
+    engine_name = os.getenv("ENGINE_NAME")
+    if engine_name:
+        # If engine name was provided, just yield the config
+        config = make_config(engine_name)
+        yield config
+        return
+
+    # If there's a local config file, use it, including
+    # the engine specified there.
+    config = cfg.Config()
+    if config.file_path is not None:
+        yield config
+        return
+
+    # Otherwise, create a new engine and delete it afterwards.
+    random_number = random.randint(1000000000, 9999999999)
+    engine_name = f"pyrel_test_{random_number}"
+    create_engine(engine_name)
+
+    yield make_config(engine_name)
+
+    delete_engine(engine_name)
+
 def create_engine(engine_name: str):
     config = make_config(engine_name)
 
     sf_compute_pool = os.getenv("SF_TEST_COMPUTE_POOL", config.get("compute_pool", ""))
 
     provider = rai.Resources(config=config)
     print(f"Creating engine {engine_name}")
@@ -23,44 +49,14 @@
 def delete_engine(engine_name: str):
     print(f"Deleting engine {engine_name}")
     config = make_config(engine_name)
     provider = rai.Resources(config=config)
     provider.delete_engine(engine_name)
     print(f"Engine {engine_name} deleted")
 
-
-@pytest.fixture(scope="session")
-def engine_config():
-    # Check for an externally provided engine name
-    # It is used in GitHub Actions to run tests against a specific engine
-    engine_name = os.getenv("ENGINE_NAME")
-    if engine_name:
-        config = make_config(engine_name)
-    else:
-        # If there's a local config file, use it, including
-        # the engine specified there.
-        config = cfg.Config()
-        if config.file_path is not None:
-            yield config
-            return
-
-        # Otherwise, create a new engine and delete it afterwards.
-        random_number = random.randint(1000000000, 9999999999)
-        engine_name = f"pyrel_test_{random_number}"
-        create_engine(engine_name)
-
-        yield config
-
-        delete_engine(engine_name)
-        return
-
-    # If engine name was provided, just yield the config
-    yield config
-
-
 def make_config(engine_name: str) -> cfg.Config:
     cloud_provider = os.getenv("RAI_CLOUD_PROVIDER")
 
     match cloud_provider:
         case None:
             raise ValueError("RAI_CLOUD_PROVIDER must be set")
         case "azure":
@@ -107,30 +103,48 @@
                     "engine": engine_name,
                     "compute_pool": sf_compute_pool,
                 }
             )
         case _:
             raise ValueError(f"Unsupported cloud provider: {cloud_provider}")
 
-# Attach Snowflake logger; shutting down that the end of the session
-
-SNOWFLAKE_LOGGER = None
+def snowflake_logger_fixture():
+    if not os.getenv("SF_REPORTING_PASSWORD"):
+        print('benchmarking logger disabled since config env vars not present')
+        yield
+        return
 
-if os.getenv("SF_REPORTING_USER") is not None:
     conn = snowflake.connector.connect(
         user=os.getenv("SF_REPORTING_USER"),
         password=os.getenv("SF_REPORTING_PASSWORD"),
         account=os.getenv("SF_REPORTING_ACCOUNT"),
         role=os.getenv("SF_REPORTING_ROLE"),
         warehouse=os.getenv("SF_REPORTING_WAREHOUSE"),
         database=os.getenv("SF_REPORTING_DATABASE"),
         schema=os.getenv("SF_REPORTING_SCHEMA"),
     )
-    SNOWFLAKE_LOGGER = SnowflakeLogger(conn)
-    logger.addHandler(SNOWFLAKE_LOGGER)
-else:
-    print('benchmarking logger disabled since config env vars not present')
-
-
-def pytest_sessionfinish(session, exitstatus):
-    if SNOWFLAKE_LOGGER:
-        SNOWFLAKE_LOGGER.shut_down()
+    snowflake_logger = SnowflakeLogger(conn)
+    logger.addHandler(snowflake_logger)
+    yield
+    snowflake_logger.shut_down()
+
+def root_span_fixture():
+    git_info = get_git_info()
+    attrs = {
+        **git_info,
+        "cloud_provider": os.getenv("RAI_CLOUD_PROVIDER"),
+    }
+    with debugging.span("test_session", **attrs):
+        yield
+
+def get_git_info():
+    if os.getenv("GITHUB_REF_NAME") is not None:
+        return {
+            'commit': os.getenv("GITHUB_SHA"),
+            'branch': os.getenv("GITHUB_REF_NAME"),
+        }
+    else:
+        # shell out to get the info
+        return {
+            'commit': 'local',
+            'branch': 'local',
+        }
```

### Comparing `relationalai-0.2.5/tests/end2end/test_graph_visualize.py` & `relationalai-0.2.6/tests/end2end/test_graph_visualize.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_snapshots.py` & `relationalai-0.2.6/tests/end2end/test_snapshots.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
 @pytest.mark.parametrize(
     "file_path", test_case_files, ids=lambda path: path_to_slug(path, test_case_dir)
 )
 def test_snapshots(file_path: Path, snapshot, engine_config: cfg.Config):
     test_name = file_path.stem
     provider = rai.Resources(config=engine_config)
-    cloud_provider_str = engine_config.get("platform", "snowflake")
-    with debugging.span("test", name=test_name, cloud_provider=cloud_provider_str):
+    with debugging.span("test", name=test_name):
         for i in range(1):
             with debugging.span("run", idx=i):
                 db_name = randomize(test_name)
                 validate_query_results(
                     file_path,
                     snapshot,
                     {
```

### Comparing `relationalai-0.2.5/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt` & `relationalai-0.2.6/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/bool.py` & `relationalai-0.2.6/tests/end2end/test_cases/bool.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/bottom.py` & `relationalai-0.2.6/tests/end2end/test_cases/bottom.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/export.py` & `relationalai-0.2.6/tests/end2end/test_cases/export.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/multi_valued.py` & `relationalai-0.2.6/tests/end2end/test_cases/multi_valued.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/not_found.py` & `relationalai-0.2.6/tests/end2end/test_cases/not_found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/out_of_context.py` & `relationalai-0.2.6/tests/end2end/test_cases/out_of_context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/persist.py` & `relationalai-0.2.6/tests/end2end/test_cases/persist.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/smoke.py` & `relationalai-0.2.6/tests/end2end/test_cases/smoke.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/strings.py` & `relationalai-0.2.6/tests/end2end/test_cases/strings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,114 @@
 import relationalai as rai
 from relationalai import std
 
 
-model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
+model = rai.Model(name=globals().get("name", "test_strings"), config=globals().get("config"))
 Person = model.Type("Person")
+LikePattern = model.Type("LikePattern")
 
 with model.rule():
     Person.add(first="John", last="Coltrane")
     Person.add(first="Miles", last="Davis")
+    Person.add(name="Herbie Hancock")
+    # Used in the `like` test, which relies on there being exactly one LikePattern instance.
+    LikePattern.add(pattern="Mi%")
 
 # Check that 'length' works.
-with model.query() as select:
+with model.query(tag="length") as select:
     p = Person()
     f_length = std.strings.length(p.last)
     v_length = std.strings.length("Four")
     select(p, p.last, f_length, v_length)
 
 # Check that 'contains' works.
-with model.query() as select:
+with model.query(tag="contains") as select:
     p = Person()
     with model.union() as u:
         with model.scope():
             std.strings.contains(p.last, "trane")
             u.add(p)
         with model.scope():
             std.strings.contains("SMiles", p.first)
             u.add(p)
     select(p, p.first, p.last)
 
 # Check that 'ends_with' works.
-with model.query() as select:
+with model.query(tag="ends_with") as select:
     p = Person()
     with model.union() as u:
         with model.scope():
             std.strings.ends_with(p.last, "trane")
             u.add(p)
         with model.scope():
             std.strings.ends_with("SMiles", p.first)
             u.add(p)
     select(u, u.first, u.last)
 
 # Check that 'lowercase' and 'uppercase' work.
-with model.query() as select:
+with model.query(tag="lowercase") as select:
     p = Person()
     lower = std.strings.lowercase(p.first)
     upper = std.strings.uppercase(p.first)
     select(p, p.first, lower, upper)
 
 # Check that 'join' works.
-with model.query() as select:
+with model.query(tag="join") as select:
     p = Person()
     name = std.strings.join([p.first, p.last], " ")
     name2 = std.strings.join(["FIRST", p.last], " ")
     name3 = std.strings.join([p.first, "LAST"], " ")
     sep = std.Vars(1)
     sep == ""
     name4 = std.strings.join(["FIRST", "LAST"], sep)
     select(p, p.first, p.last, name, name2, name3, name4)
 
 # Check that concat works:
-with model.query() as select:
+with model.query(tag="concat") as select:
     p = Person()
     first_name = std.strings.concat(p.first, "")
     last_name = std.strings.concat("", p.last)
     full_name = std.strings.concat(p.first, p.last)
     new_name = std.strings.concat("HEY", "YOU")
     select(p, first_name, last_name, full_name, new_name)
 
 # Check that replace works.
-with model.query() as select:
+with model.query(tag="replace") as select:
     p = Person(first="John", last="Coltrane")
     s = Person(first="Miles", last="Davis").first
     new1 = std.strings.replace(p.first, old="ohn", new="ohnny")
     new2 = std.strings.replace(p.first, old="ohn", new=s)
     new3 = std.strings.replace(p.first, old=p.first, new=s)
     select(p, p.first, new1, new2, new3)
+
+# Check that 'like' works.
+with model.query(tag="like") as select:
+    p = Person()
+    with model.union() as u:
+        with model.scope():
+            std.strings.like(p.last, "Col%")
+            u.add(p)
+        with model.scope():
+            pattern = LikePattern()
+            std.strings.like(p.first, pattern.pattern)
+            u.add(p)
+    select(u, u.first, u.last)
+
+# Check that 'regex_match' and 'regex_compile' work.
+with model.query(tag="regex_match_and_compile") as select:
+    p = Person()
+    pattern = std.strings.regex_compile(r"Col.*")
+    std.strings.regex_match(p.last, pattern)
+    select(p, p.first, p.last)
+
+# Check that 'split' work
+with model.query(tag="split") as select:
+    p = Person()
+    ix, part = std.strings.split(p.name, " ")
+    select(ix, part)
+
+# Check that 'split_part' works.
+with model.query(tag="split_part") as select:
+    p = Person()
+    first = std.strings.split_part(p.name, " ", 0)
+    last = std.strings.split_part(p.name, " ", 1)
+    select(p, p.name, first, last)
```

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/top.py` & `relationalai-0.2.6/tests/end2end/test_cases/top.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/union.py` & `relationalai-0.2.6/tests/end2end/test_cases/union.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/weighted_graphs.py` & `relationalai-0.2.6/tests/end2end/test_cases/weighted_graphs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/graphs/basics.py` & `relationalai-0.2.6/tests/end2end/test_cases/graphs/basics.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 graph = std.graphs.Graph(model)
 
 with model.rule():
     r = Relationship()
     graph.Edge.add(r.from_, r.to)
 
 for algo_name in ALGOS:
-    with model.query() as select:
+    with model.query(tag=algo_name) as select:
         o = Object()
         # NOTE: This only works for unary relations.
         algo = getattr(graph.compute, algo_name)()
         select(algo)
```

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/graphs/centrality.py` & `relationalai-0.2.6/tests/end2end/test_cases/graphs/centrality.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 undirected_graph = std.graphs.Graph(model, undirected=True)
 
 with model.rule():
     r = Relationship()
     undirected_graph.Edge.add(r.from_, r.to)
 
 for algo_name in UNWEIGHTED_ALGOS:
-    with model.query() as select:
+    with model.query(tag=algo_name) as select:
         o = Object()
         algo = getattr(undirected_graph.compute, algo_name)(o)
         select(o, algo)
 
 weighted_graph = std.graphs.Graph(model, undirected=True, weighted=True)
 
 with model.rule():
     r = Relationship()
     weighted_graph.Edge.add(r.from_, r.to, weight=r.weight)
 
 for algo_name in WEIGHTED_ALGOS:
-    with model.query() as select:
+    with model.query(tag=algo_name) as select:
         o = Object()
         algo = getattr(weighted_graph.compute, algo_name)(o)
         select(o, algo)
```

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/graphs/community.py` & `relationalai-0.2.6/tests/end2end/test_cases/graphs/community.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,11 +24,11 @@
 graph.Node.extend(Object)
 
 with model.rule():
     r = Relationship()
     graph.Edge.add(r.from_, r.to)
 
 for algo_name in ALGOS:
-    with model.query() as select:
+    with model.query(tag=algo_name) as select:
         o = Object()
         algo = getattr(graph.compute, algo_name)(o)
         select(o, algo)
```

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/graphs/connectivity.py` & `relationalai-0.2.6/tests/end2end/test_cases/graphs/connectivity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/graphs/degree.py` & `relationalai-0.2.6/tests/end2end/test_cases/graphs/degree.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/end2end/test_cases/graphs/link_prediction.py` & `relationalai-0.2.6/tests/end2end/test_cases/graphs/link_prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 Node.extend(Object)
 
 with model.rule():
     r = LinkPrediction()
     Edge.add(r.from_, r.to)
 
 for algo_name in ALGOS:
-    with model.query() as select:
+    with model.query(tag=algo_name) as select:
         o1 = Object(id=1)
         o2 = Object(id=2)
         o3 = Object(id=3)
         o4 = Object(id=4)
         algo1 = getattr(graph.compute, algo_name)(o1, o3)
         algo2 = getattr(graph.compute, algo_name)(o2, o4)
         select(o1, o3, algo1)
```

### Comparing `relationalai-0.2.5/tests/init-cli/azure_basic.py` & `relationalai-0.2.6/tests/init-cli/azure_basic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/init-cli/common.py` & `relationalai-0.2.6/tests/init-cli/common.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/roundtrip/test_document.py` & `relationalai-0.2.6/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/tests/roundtrip/test_task.py` & `relationalai-0.2.6/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.5/pyproject.toml` & `relationalai-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'relationalai'
-version = '0.2.5'
+version = '0.2.6'
 description = 'RelationalAI Library and CLI'
 readme="docs/pypi/README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
```

### Comparing `relationalai-0.2.5/PKG-INFO` & `relationalai-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: relationalai
-Version: 0.2.5
+Version: 0.2.6
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
 Requires-Dist: gravis
```

