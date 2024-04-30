# Comparing `tmp/csle_agents-0.5.1.tar.gz` & `tmp/csle_agents-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_agents-0.5.1.tar", last modified: Tue Mar  5 17:30:46 2024, max compression
+gzip compressed data, was "csle_agents-0.5.2.tar", last modified: Tue Apr 30 10:50:15 2024, max compression
```

## Comparing `csle_agents-0.5.1.tar` & `csle_agents-0.5.2.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.947724 csle_agents-0.5.1/
--rw-r--r--   0 kim        (501) staff       (20)      643 2024-03-05 17:30:46.947787 csle_agents-0.5.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     4316 2024-02-13 12:24:16.000000 csle_agents-0.5.1/README.md
--rw-r--r--   0 kim        (501) staff       (20)      671 2023-08-15 10:44:03.000000 csle_agents-0.5.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     2134 2024-03-05 17:30:46.948050 csle_agents-0.5.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_agents-0.5.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.911465 csle_agents-0.5.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.915517 csle_agents-0.5.1/src/csle_agents/
--rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-03-05 17:30:08.000000 csle_agents-0.5.1/src/csle_agents/__version__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.916703 csle_agents-0.5.1/src/csle_agents/agents/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/__init__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.916966 csle_agents-0.5.1/src/csle_agents/agents/base/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/base/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2287 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/base/base_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.917381 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    30060 2023-10-09 08:04:01.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.918082 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    32040 2023-09-20 12:42:47.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bayes_opt_emukit_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.918935 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 16:45:09.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/__init__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.919585 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/acquisition/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 16:45:26.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/acquisition/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)      382 2023-09-14 15:13:37.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/acquisition/acquisition_function_type.py
--rw-r--r--   0 kim        (501) staff       (20)      194 2023-09-15 14:06:45.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/acquisition/acquisition_optimizer_type.py
--rw-r--r--   0 kim        (501) staff       (20)     7171 2023-09-20 12:41:16.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/bo_config.py
--rw-r--r--   0 kim        (501) staff       (20)     5574 2023-09-15 16:29:41.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/bo_results.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.919944 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/gp/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 16:45:33.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/gp/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2827 2023-09-15 16:30:32.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/gp/gp_config.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.920799 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-09-12 16:45:42.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2423 2023-09-20 12:38:03.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/kernel_config.py
--rw-r--r--   0 kim        (501) staff       (20)      122 2023-09-15 13:58:03.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/kernel_type.py
--rw-r--r--   0 kim        (501) staff       (20)     2632 2023-09-15 16:24:58.000000 csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/rbf_kernel_config.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.921157 csle_agents-0.5.1/src/csle_agents/agents/c51_clean/
--rw-r--r--   0 kim        (501) staff       (20)        0 2024-03-05 13:14:43.000000 csle_agents-0.5.1/src/csle_agents/agents/c51_clean/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    21449 2024-03-05 13:14:43.000000 csle_agents-0.5.1/src/csle_agents/agents/c51_clean/c51_clean_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.921422 csle_agents-0.5.1/src/csle_agents/agents/cma_es/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-10-09 08:04:01.000000 csle_agents-0.5.1/src/csle_agents/agents/cma_es/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    29811 2023-10-09 08:04:01.000000 csle_agents-0.5.1/src/csle_agents/agents/cma_es/cma_es_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.921730 csle_agents-0.5.1/src/csle_agents/agents/cross_entropy/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/cross_entropy/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    28917 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.922796 csle_agents-0.5.1/src/csle_agents/agents/dfsp_local/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/dfsp_local/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    39213 2023-08-17 07:27:45.000000 csle_agents-0.5.1/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py
--rw-r--r--   0 kim        (501) staff       (20)    40581 2023-08-17 07:24:15.000000 csle_agents-0.5.1/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.923328 csle_agents-0.5.1/src/csle_agents/agents/differential_evolution/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/differential_evolution/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    33146 2023-10-09 07:12:58.000000 csle_agents-0.5.1/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.924133 csle_agents-0.5.1/src/csle_agents/agents/dqn/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/dqn/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    20113 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/dqn/dqn_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.924417 csle_agents-0.5.1/src/csle_agents/agents/dqn_clean/
--rw-r--r--   0 kim        (501) staff       (20)        0 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/dqn_clean/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    20928 2024-03-05 13:14:43.000000 csle_agents-0.5.1/src/csle_agents/agents/dqn_clean/dqn_clean_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.924665 csle_agents-0.5.1/src/csle_agents/agents/dynasec/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/dynasec/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    76825 2023-08-17 07:44:55.000000 csle_agents-0.5.1/src/csle_agents/agents/dynasec/dynasec_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.925326 csle_agents-0.5.1/src/csle_agents/agents/fp/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/fp/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    18439 2023-08-17 08:04:48.000000 csle_agents-0.5.1/src/csle_agents/agents/fp/fictitious_play_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.925755 csle_agents-0.5.1/src/csle_agents/agents/hsvi/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/hsvi/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    51046 2023-08-17 09:45:48.000000 csle_agents-0.5.1/src/csle_agents/agents/hsvi/hsvi_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.926473 csle_agents-0.5.1/src/csle_agents/agents/hsvi_os_posg/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/hsvi_os_posg/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    77345 2023-08-17 09:48:38.000000 csle_agents-0.5.1/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.927097 csle_agents-0.5.1/src/csle_agents/agents/kiefer_wolfowitz/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    29247 2023-08-17 08:35:21.000000 csle_agents-0.5.1/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.927676 csle_agents-0.5.1/src/csle_agents/agents/lp_cmdp/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/lp_cmdp/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    21367 2023-09-20 12:38:03.000000 csle_agents-0.5.1/src/csle_agents/agents/lp_cmdp/linear_programming_cmdp_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.928217 csle_agents-0.5.1/src/csle_agents/agents/lp_nf/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/lp_nf/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    18607 2023-09-15 13:04:34.000000 csle_agents-0.5.1/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.928662 csle_agents-0.5.1/src/csle_agents/agents/nelder_mead/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-10-27 16:26:03.000000 csle_agents-0.5.1/src/csle_agents/agents/nelder_mead/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    33075 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/nelder_mead/nelder_mead_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.929334 csle_agents-0.5.1/src/csle_agents/agents/particle_swarm/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-10-27 16:26:03.000000 csle_agents-0.5.1/src/csle_agents/agents/particle_swarm/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    31697 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/particle_swarm/particle_swarm_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.929704 csle_agents-0.5.1/src/csle_agents/agents/pi/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/pi/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    18212 2023-08-17 08:39:44.000000 csle_agents-0.5.1/src/csle_agents/agents/pi/pi_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.931679 csle_agents-0.5.1/src/csle_agents/agents/pomcp/
--rw-r--r--   0 kim        (501) staff       (20)        0 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/pomcp/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2095 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/pomcp/action_node.py
--rw-r--r--   0 kim        (501) staff       (20)     2467 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/pomcp/belief_node.py
--rw-r--r--   0 kim        (501) staff       (20)     5180 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/pomcp/belief_tree.py
--rw-r--r--   0 kim        (501) staff       (20)     1543 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/pomcp/node.py
--rw-r--r--   0 kim        (501) staff       (20)    22874 2024-03-05 13:14:47.000000 csle_agents-0.5.1/src/csle_agents/agents/pomcp/pomcp.py
--rw-r--r--   0 kim        (501) staff       (20)      193 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/pomcp/pomcp_acquisition_function_type.py
--rw-r--r--   0 kim        (501) staff       (20)    21529 2024-03-05 13:14:47.000000 csle_agents-0.5.1/src/csle_agents/agents/pomcp/pomcp_agent.py
--rw-r--r--   0 kim        (501) staff       (20)     6725 2024-02-13 13:43:48.000000 csle_agents-0.5.1/src/csle_agents/agents/pomcp/pomcp_util.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.932056 csle_agents-0.5.1/src/csle_agents/agents/ppg_clean/
--rw-r--r--   0 kim        (501) staff       (20)        0 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/ppg_clean/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    27726 2024-03-05 16:52:27.000000 csle_agents-0.5.1/src/csle_agents/agents/ppg_clean/ppg_clean_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.932292 csle_agents-0.5.1/src/csle_agents/agents/ppo/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/ppo/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    26886 2024-03-05 13:14:43.000000 csle_agents-0.5.1/src/csle_agents/agents/ppo/ppo_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.932534 csle_agents-0.5.1/src/csle_agents/agents/ppo_clean/
--rw-r--r--   0 kim        (501) staff       (20)        0 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/ppo_clean/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    26839 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/ppo_clean/ppo_clean_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.932791 csle_agents-0.5.1/src/csle_agents/agents/q_learning/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/q_learning/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    19362 2024-02-13 12:24:16.000000 csle_agents-0.5.1/src/csle_agents/agents/q_learning/q_learning_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.933049 csle_agents-0.5.1/src/csle_agents/agents/random_search/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/random_search/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    28271 2023-10-09 07:12:58.000000 csle_agents-0.5.1/src/csle_agents/agents/random_search/random_search_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.933601 csle_agents-0.5.1/src/csle_agents/agents/reinforce/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/reinforce/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    25105 2023-08-17 09:44:21.000000 csle_agents-0.5.1/src/csle_agents/agents/reinforce/reinforce_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.934100 csle_agents-0.5.1/src/csle_agents/agents/sarsa/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/sarsa/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    18002 2023-08-17 09:48:09.000000 csle_agents-0.5.1/src/csle_agents/agents/sarsa/sarsa_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.934588 csle_agents-0.5.1/src/csle_agents/agents/shapley_iteration/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/shapley_iteration/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    15993 2023-08-17 09:38:38.000000 csle_agents-0.5.1/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.934997 csle_agents-0.5.1/src/csle_agents/agents/simulated_annealing/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/simulated_annealing/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    27300 2023-10-02 06:07:40.000000 csle_agents-0.5.1/src/csle_agents/agents/simulated_annealing/simulated_annealing_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.935505 csle_agents-0.5.1/src/csle_agents/agents/sondik_vi/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/sondik_vi/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    22621 2023-08-17 09:07:25.000000 csle_agents-0.5.1/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.935970 csle_agents-0.5.1/src/csle_agents/agents/t_fp/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/t_fp/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    42226 2023-09-20 12:50:04.000000 csle_agents-0.5.1/src/csle_agents/agents/t_fp/t_fp_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.936657 csle_agents-0.5.1/src/csle_agents/agents/t_spsa/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/t_spsa/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    34295 2023-10-09 07:12:58.000000 csle_agents-0.5.1/src/csle_agents/agents/t_spsa/t_spsa_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.937426 csle_agents-0.5.1/src/csle_agents/agents/vi/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/agents/vi/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    16821 2023-08-17 09:12:29.000000 csle_agents-0.5.1/src/csle_agents/agents/vi/vi_agent.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.939016 csle_agents-0.5.1/src/csle_agents/common/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/common/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     5998 2023-08-17 09:43:21.000000 csle_agents-0.5.1/src/csle_agents/common/actor_critic_net.py
--rw-r--r--   0 kim        (501) staff       (20)     4577 2023-08-17 09:37:02.000000 csle_agents-0.5.1/src/csle_agents/common/fnn_w_gaussian.py
--rw-r--r--   0 kim        (501) staff       (20)     3936 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/common/fnn_w_linear.py
--rw-r--r--   0 kim        (501) staff       (20)      149 2023-09-20 12:38:03.000000 csle_agents-0.5.1/src/csle_agents/common/objective_type.py
--rw-r--r--   0 kim        (501) staff       (20)     3551 2023-08-17 09:39:43.000000 csle_agents-0.5.1/src/csle_agents/common/pruning.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.939471 csle_agents-0.5.1/src/csle_agents/constants/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/constants/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    19997 2024-03-05 13:46:08.000000 csle_agents-0.5.1/src/csle_agents/constants/constants.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.939744 csle_agents-0.5.1/src/csle_agents/job_controllers/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_agents-0.5.1/src/csle_agents/job_controllers/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2526 2023-08-17 09:44:04.000000 csle_agents-0.5.1/src/csle_agents/job_controllers/training_job_manager.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.916485 csle_agents-0.5.1/src/csle_agents.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      643 2024-03-05 17:30:46.000000 csle_agents-0.5.1/src/csle_agents.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     6218 2024-03-05 17:30:46.000000 csle_agents-0.5.1/src/csle_agents.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-03-05 17:30:46.000000 csle_agents-0.5.1/src/csle_agents.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-09-28 06:32:56.000000 csle_agents-0.5.1/src/csle_agents.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      867 2024-03-05 17:30:46.000000 csle_agents-0.5.1/src/csle_agents.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       12 2024-03-05 17:30:46.000000 csle_agents-0.5.1/src/csle_agents.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-03-05 17:30:46.947521 csle_agents-0.5.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)    12324 2023-10-09 07:12:58.000000 csle_agents-0.5.1/tests/test_bayes_opt.py
--rw-r--r--   0 kim        (501) staff       (20)    15132 2023-09-20 12:42:47.000000 csle_agents-0.5.1/tests/test_bayes_opt_emukit.py
--rw-r--r--   0 kim        (501) staff       (20)    12912 2024-03-05 13:14:43.000000 csle_agents-0.5.1/tests/test_c51_clean.py
--rw-r--r--   0 kim        (501) staff       (20)    12459 2023-10-12 15:33:50.000000 csle_agents-0.5.1/tests/test_cma_es.py
--rw-r--r--   0 kim        (501) staff       (20)    11978 2023-09-20 12:46:10.000000 csle_agents-0.5.1/tests/test_cross_entropy.py
--rw-r--r--   0 kim        (501) staff       (20)    12456 2023-10-09 07:12:58.000000 csle_agents-0.5.1/tests/test_differential_evolution.py
--rw-r--r--   0 kim        (501) staff       (20)    11948 2023-08-17 09:51:02.000000 csle_agents-0.5.1/tests/test_dqn.py
--rw-r--r--   0 kim        (501) staff       (20)    14922 2024-02-13 12:24:16.000000 csle_agents-0.5.1/tests/test_dqn_clean.py
--rw-r--r--   0 kim        (501) staff       (20)     1059 2023-08-17 09:51:02.000000 csle_agents-0.5.1/tests/test_dynasec.py
--rw-r--r--   0 kim        (501) staff       (20)    10912 2023-08-17 09:53:52.000000 csle_agents-0.5.1/tests/test_fp.py
--rw-r--r--   0 kim        (501) staff       (20)    14199 2023-08-17 09:53:52.000000 csle_agents-0.5.1/tests/test_hsvi.py
--rw-r--r--   0 kim        (501) staff       (20)    10476 2023-08-17 09:55:47.000000 csle_agents-0.5.1/tests/test_hsvi_os_posg.py
--rw-r--r--   0 kim        (501) staff       (20)    11756 2023-08-17 09:53:52.000000 csle_agents-0.5.1/tests/test_kiefer_wolfowitz.py
--rw-r--r--   0 kim        (501) staff       (20)    33922 2023-09-20 12:38:03.000000 csle_agents-0.5.1/tests/test_lp_cmdp.py
--rw-r--r--   0 kim        (501) staff       (20)     5824 2023-08-17 09:53:52.000000 csle_agents-0.5.1/tests/test_lp_nf.py
--rw-r--r--   0 kim        (501) staff       (20)    14014 2024-02-13 12:24:16.000000 csle_agents-0.5.1/tests/test_nelder_mead.py
--rw-r--r--   0 kim        (501) staff       (20)    12373 2024-02-13 12:24:16.000000 csle_agents-0.5.1/tests/test_particle_swarm.py
--rw-r--r--   0 kim        (501) staff       (20)    11370 2023-08-17 09:53:52.000000 csle_agents-0.5.1/tests/test_pi.py
--rw-r--r--   0 kim        (501) staff       (20)    15365 2024-03-05 16:56:28.000000 csle_agents-0.5.1/tests/test_ppg_clean.py
--rw-r--r--   0 kim        (501) staff       (20)    11916 2024-02-13 12:24:16.000000 csle_agents-0.5.1/tests/test_ppo.py
--rw-r--r--   0 kim        (501) staff       (20)    13330 2024-02-13 12:24:16.000000 csle_agents-0.5.1/tests/test_ppo_clean.py
--rw-r--r--   0 kim        (501) staff       (20)    10465 2024-02-13 12:24:16.000000 csle_agents-0.5.1/tests/test_q_learning.py
--rw-r--r--   0 kim        (501) staff       (20)    11494 2023-10-09 07:12:58.000000 csle_agents-0.5.1/tests/test_random_search.py
--rw-r--r--   0 kim        (501) staff       (20)    10723 2023-08-17 09:53:52.000000 csle_agents-0.5.1/tests/test_reinforce.py
--rw-r--r--   0 kim        (501) staff       (20)    10187 2023-08-17 09:53:52.000000 csle_agents-0.5.1/tests/test_sarsa.py
--rw-r--r--   0 kim        (501) staff       (20)     9975 2023-08-17 09:53:52.000000 csle_agents-0.5.1/tests/test_shapley_iteration.py
--rw-r--r--   0 kim        (501) staff       (20)    12223 2023-10-09 07:12:58.000000 csle_agents-0.5.1/tests/test_simulated_annealing.py
--rw-r--r--   0 kim        (501) staff       (20)    13564 2023-08-17 09:53:52.000000 csle_agents-0.5.1/tests/test_sondik_vi.py
--rw-r--r--   0 kim        (501) staff       (20)     9785 2023-09-20 15:08:49.000000 csle_agents-0.5.1/tests/test_t_fp.py
--rw-r--r--   0 kim        (501) staff       (20)    11944 2023-09-20 12:48:14.000000 csle_agents-0.5.1/tests/test_t_spsa.py
--rw-r--r--   0 kim        (501) staff       (20)    11117 2023-08-17 09:54:32.000000 csle_agents-0.5.1/tests/test_vi.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.790837 csle_agents-0.5.2/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      643 2024-04-30 10:50:15.790837 csle_agents-0.5.2/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4316 2024-01-29 12:14:49.000000 csle_agents-0.5.2/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-08-08 14:54:06.000000 csle_agents-0.5.2/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2134 2024-04-30 10:50:15.790837 csle_agents-0.5.2/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_agents-0.5.2/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.754837 csle_agents-0.5.2/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.758837 csle_agents-0.5.2/src/csle_agents/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-09-16 09:55:37.000000 csle_agents-0.5.2/src/csle_agents/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 csle_agents-0.5.2/src/csle_agents/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.762837 csle_agents-0.5.2/src/csle_agents/agents/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.762837 csle_agents-0.5.2/src/csle_agents/agents/base/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/base/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2287 2024-01-29 12:14:49.000000 csle_agents-0.5.2/src/csle_agents/agents/base/base_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.762837 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    30060 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.762837 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    32040 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bayes_opt_emukit_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.762837 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.762837 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/acquisition/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/acquisition/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      382 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/acquisition/acquisition_function_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      194 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/acquisition/acquisition_optimizer_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7171 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/bo_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5574 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/bo_results.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.762837 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/gp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/gp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2827 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/gp/gp_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.766837 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2423 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/kernel_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      122 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/kernel_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2632 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/rbf_kernel_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.766837 csle_agents-0.5.2/src/csle_agents/agents/c51_clean/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/c51_clean/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    21449 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/c51_clean/c51_clean_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.766837 csle_agents-0.5.2/src/csle_agents/agents/cma_es/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/cma_es/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    29811 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/cma_es/cma_es_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.766837 csle_agents-0.5.2/src/csle_agents/agents/cross_entropy/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/cross_entropy/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28917 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.766837 csle_agents-0.5.2/src/csle_agents/agents/dfsp_local/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-05-03 08:18:28.000000 csle_agents-0.5.2/src/csle_agents/agents/dfsp_local/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    39213 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    40581 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.766837 csle_agents-0.5.2/src/csle_agents/agents/differential_evolution/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/differential_evolution/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    33146 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.766837 csle_agents-0.5.2/src/csle_agents/agents/dqn/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/dqn/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    20113 2024-01-29 12:14:49.000000 csle_agents-0.5.2/src/csle_agents/agents/dqn/dqn_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.766837 csle_agents-0.5.2/src/csle_agents/agents/dqn_clean/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/dqn_clean/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    20928 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/dqn_clean/dqn_clean_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.766837 csle_agents-0.5.2/src/csle_agents/agents/dynasec/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/dynasec/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    76825 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/dynasec/dynasec_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.770837 csle_agents-0.5.2/src/csle_agents/agents/fp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/fp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18439 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/fp/fictitious_play_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.770837 csle_agents-0.5.2/src/csle_agents/agents/hsvi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/hsvi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    51046 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/hsvi/hsvi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.770837 csle_agents-0.5.2/src/csle_agents/agents/hsvi_os_posg/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/hsvi_os_posg/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    77345 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.770837 csle_agents-0.5.2/src/csle_agents/agents/kiefer_wolfowitz/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    29247 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.770837 csle_agents-0.5.2/src/csle_agents/agents/lp_cmdp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/lp_cmdp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    21367 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/lp_cmdp/linear_programming_cmdp_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.770837 csle_agents-0.5.2/src/csle_agents/agents/lp_nf/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/lp_nf/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18607 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.770837 csle_agents-0.5.2/src/csle_agents/agents/nelder_mead/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/nelder_mead/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    33075 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/nelder_mead/nelder_mead_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.770837 csle_agents-0.5.2/src/csle_agents/agents/particle_swarm/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/particle_swarm/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    31697 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/particle_swarm/particle_swarm_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.774837 csle_agents-0.5.2/src/csle_agents/agents/pi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/pi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18212 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/pi/pi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.774837 csle_agents-0.5.2/src/csle_agents/agents/pomcp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 12:14:49.000000 csle_agents-0.5.2/src/csle_agents/agents/pomcp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2095 2024-01-29 12:14:49.000000 csle_agents-0.5.2/src/csle_agents/agents/pomcp/action_node.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2467 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/pomcp/belief_node.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5180 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/pomcp/belief_tree.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1543 2024-01-29 12:14:49.000000 csle_agents-0.5.2/src/csle_agents/agents/pomcp/node.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22874 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/pomcp/pomcp.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      193 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/pomcp/pomcp_acquisition_function_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    21529 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/pomcp/pomcp_agent.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6725 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/pomcp/pomcp_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.774837 csle_agents-0.5.2/src/csle_agents/agents/ppg_clean/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/ppg_clean/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    27726 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/ppg_clean/ppg_clean_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.774837 csle_agents-0.5.2/src/csle_agents/agents/ppo/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/ppo/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    26886 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/ppo/ppo_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.774837 csle_agents-0.5.2/src/csle_agents/agents/ppo_clean/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/ppo_clean/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    26839 2024-01-29 12:21:28.000000 csle_agents-0.5.2/src/csle_agents/agents/ppo_clean/ppo_clean_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.774837 csle_agents-0.5.2/src/csle_agents/agents/q_learning/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/q_learning/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19362 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/agents/q_learning/q_learning_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.774837 csle_agents-0.5.2/src/csle_agents/agents/random_search/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/random_search/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28271 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/random_search/random_search_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.774837 csle_agents-0.5.2/src/csle_agents/agents/reinforce/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/reinforce/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    25105 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/reinforce/reinforce_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.774837 csle_agents-0.5.2/src/csle_agents/agents/sarsa/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/sarsa/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18002 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/sarsa/sarsa_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.778837 csle_agents-0.5.2/src/csle_agents/agents/shapley_iteration/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/shapley_iteration/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15993 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.778837 csle_agents-0.5.2/src/csle_agents/agents/simulated_annealing/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/simulated_annealing/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    27300 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/simulated_annealing/simulated_annealing_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.778837 csle_agents-0.5.2/src/csle_agents/agents/sondik_vi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/sondik_vi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22621 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.778837 csle_agents-0.5.2/src/csle_agents/agents/t_fp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/t_fp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    42226 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/t_fp/t_fp_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.778837 csle_agents-0.5.2/src/csle_agents/agents/t_spsa/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/t_spsa/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    34295 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/t_spsa/t_spsa_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.778837 csle_agents-0.5.2/src/csle_agents/agents/vi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/agents/vi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16821 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/agents/vi/vi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.778837 csle_agents-0.5.2/src/csle_agents/common/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/common/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5998 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/common/actor_critic_net.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4577 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/common/fnn_w_gaussian.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/common/fnn_w_linear.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      149 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/common/objective_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3551 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/common/pruning.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.782837 csle_agents-0.5.2/src/csle_agents/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19997 2024-04-30 09:37:30.000000 csle_agents-0.5.2/src/csle_agents/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.782837 csle_agents-0.5.2/src/csle_agents/job_controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.5.2/src/csle_agents/job_controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2526 2024-01-29 11:24:00.000000 csle_agents-0.5.2/src/csle_agents/job_controllers/training_job_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.762837 csle_agents-0.5.2/src/csle_agents.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      643 2024-04-30 10:50:15.000000 csle_agents-0.5.2/src/csle_agents.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6218 2024-04-30 10:50:15.000000 csle_agents-0.5.2/src/csle_agents.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:50:15.000000 csle_agents-0.5.2/src/csle_agents.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:05.000000 csle_agents-0.5.2/src/csle_agents.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      867 2024-04-30 10:50:15.000000 csle_agents-0.5.2/src/csle_agents.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       12 2024-04-30 10:50:15.000000 csle_agents-0.5.2/src/csle_agents.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:15.790837 csle_agents-0.5.2/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12324 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_bayes_opt.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15132 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_bayes_opt_emukit.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12912 2024-04-30 09:37:30.000000 csle_agents-0.5.2/tests/test_c51_clean.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12459 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_cma_es.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11978 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_cross_entropy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12456 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_differential_evolution.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11948 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_dqn.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14922 2024-04-30 09:37:30.000000 csle_agents-0.5.2/tests/test_dqn_clean.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1059 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_dynasec.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10912 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_fp.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14199 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_hsvi.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10476 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_hsvi_os_posg.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11756 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_kiefer_wolfowitz.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    33922 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_lp_cmdp.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5824 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_lp_nf.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14014 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_nelder_mead.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12373 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_particle_swarm.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11370 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_pi.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15365 2024-04-30 09:37:30.000000 csle_agents-0.5.2/tests/test_ppg_clean.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11916 2024-01-29 12:14:49.000000 csle_agents-0.5.2/tests/test_ppo.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13330 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_ppo_clean.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10465 2024-01-29 12:14:49.000000 csle_agents-0.5.2/tests/test_q_learning.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11494 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_random_search.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10723 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_reinforce.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10187 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_sarsa.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9975 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_shapley_iteration.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12223 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_simulated_annealing.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13564 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_sondik_vi.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     9785 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_t_fp.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11944 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_t_spsa.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11117 2024-01-29 11:24:00.000000 csle_agents-0.5.2/tests/test_vi.py
```

### Comparing `csle_agents-0.5.1/PKG-INFO` & `csle_agents-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_agents
-Version: 0.5.1
+Version: 0.5.2
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.5.1/README.md` & `csle_agents-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/pyproject.toml` & `csle_agents-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/setup.cfg` & `csle_agents-0.5.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-base>=0.5.1
-	csle-common>=0.5.1
-	csle-collector>=0.5.1
-	csle-cluster>=0.5.1
-	csle-attacker>=0.5.1
-	csle-defender>=0.5.1
-	csle-system-identification>=0.5.1
-	gym-csle-stopping-game>=0.5.1
-	gym-csle-apt-game>=0.5.1
-	gym-csle-cyborg>=0.5.1
-	gym-csle-intrusion-response-game>=0.5.1
-	csle-tolerance>=0.5.1
+	csle-base>=0.5.2
+	csle-common>=0.5.2
+	csle-collector>=0.5.2
+	csle-cluster>=0.5.2
+	csle-attacker>=0.5.2
+	csle-defender>=0.5.2
+	csle-system-identification>=0.5.2
+	gym-csle-stopping-game>=0.5.2
+	gym-csle-apt-game>=0.5.2
+	gym-csle-cyborg>=0.5.2
+	gym-csle-intrusion-response-game>=0.5.2
+	csle-tolerance>=0.5.2
 	stable-baselines3>=2.0.0
 	pulp>=2.7.0
 	bayesian-optimization>=1.3.1
 	iteround>=1.0.4
 	emukit>=0.4.10
 	GPy>=1.10.0
 	numpy==1.23.5
```

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/base/base_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/base/base_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bayes_opt_emukit_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bayes_opt_emukit_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/bo_config.py` & `csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/bo_config.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/bo_results.py` & `csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/bo_results.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/gp/gp_config.py` & `csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/gp/gp_config.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/kernel_config.py` & `csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/kernel_config.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/rbf_kernel_config.py` & `csle_agents-0.5.2/src/csle_agents/agents/bayesian_optimization_emukit/bo/kernel/rbf_kernel_config.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/c51_clean/c51_clean_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/c51_clean/c51_clean_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/cma_es/cma_es_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/cma_es/cma_es_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/dfsp_local/dfsp_local_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/dfsp_local/dfsp_local_ppo_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/dqn/dqn_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/dqn/dqn_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/dqn_clean/dqn_clean_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/dqn_clean/dqn_clean_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/dynasec/dynasec_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/dynasec/dynasec_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/fp/fictitious_play_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/fp/fictitious_play_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/hsvi/hsvi_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/hsvi/hsvi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/lp_cmdp/linear_programming_cmdp_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/lp_cmdp/linear_programming_cmdp_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/nelder_mead/nelder_mead_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/nelder_mead/nelder_mead_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/particle_swarm/particle_swarm_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/particle_swarm/particle_swarm_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/pi/pi_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/pi/pi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/pomcp/action_node.py` & `csle_agents-0.5.2/src/csle_agents/agents/pomcp/action_node.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/pomcp/belief_node.py` & `csle_agents-0.5.2/src/csle_agents/agents/pomcp/belief_node.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/pomcp/belief_tree.py` & `csle_agents-0.5.2/src/csle_agents/agents/pomcp/belief_tree.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/pomcp/node.py` & `csle_agents-0.5.2/src/csle_agents/agents/pomcp/node.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/pomcp/pomcp.py` & `csle_agents-0.5.2/src/csle_agents/agents/pomcp/pomcp.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/pomcp/pomcp_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/pomcp/pomcp_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/pomcp/pomcp_util.py` & `csle_agents-0.5.2/src/csle_agents/agents/pomcp/pomcp_util.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/ppg_clean/ppg_clean_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/ppg_clean/ppg_clean_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/ppo/ppo_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/ppo/ppo_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/ppo_clean/ppo_clean_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/ppo_clean/ppo_clean_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/q_learning/q_learning_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/q_learning/q_learning_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/random_search/random_search_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/random_search/random_search_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/reinforce/reinforce_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/reinforce/reinforce_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/sarsa/sarsa_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/sarsa/sarsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/simulated_annealing/simulated_annealing_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/simulated_annealing/simulated_annealing_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/t_fp/t_fp_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/t_fp/t_fp_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/t_spsa/t_spsa_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/t_spsa/t_spsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/agents/vi/vi_agent.py` & `csle_agents-0.5.2/src/csle_agents/agents/vi/vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/common/actor_critic_net.py` & `csle_agents-0.5.2/src/csle_agents/common/actor_critic_net.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/common/fnn_w_gaussian.py` & `csle_agents-0.5.2/src/csle_agents/common/fnn_w_gaussian.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/common/fnn_w_linear.py` & `csle_agents-0.5.2/src/csle_agents/common/fnn_w_linear.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/common/pruning.py` & `csle_agents-0.5.2/src/csle_agents/common/pruning.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/constants/constants.py` & `csle_agents-0.5.2/src/csle_agents/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents/job_controllers/training_job_manager.py` & `csle_agents-0.5.2/src/csle_agents/job_controllers/training_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents.egg-info/PKG-INFO` & `csle_agents-0.5.2/src/csle_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-agents
-Version: 0.5.1
+Version: 0.5.2
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.5.1/src/csle_agents.egg-info/SOURCES.txt` & `csle_agents-0.5.2/src/csle_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/src/csle_agents.egg-info/requires.txt` & `csle_agents-0.5.2/src/csle_agents.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-csle-base>=0.5.1
-csle-common>=0.5.1
-csle-collector>=0.5.1
-csle-cluster>=0.5.1
-csle-attacker>=0.5.1
-csle-defender>=0.5.1
-csle-system-identification>=0.5.1
-gym-csle-stopping-game>=0.5.1
-gym-csle-apt-game>=0.5.1
-gym-csle-cyborg>=0.5.1
-gym-csle-intrusion-response-game>=0.5.1
-csle-tolerance>=0.5.1
+csle-base>=0.5.2
+csle-common>=0.5.2
+csle-collector>=0.5.2
+csle-cluster>=0.5.2
+csle-attacker>=0.5.2
+csle-defender>=0.5.2
+csle-system-identification>=0.5.2
+gym-csle-stopping-game>=0.5.2
+gym-csle-apt-game>=0.5.2
+gym-csle-cyborg>=0.5.2
+gym-csle-intrusion-response-game>=0.5.2
+csle-tolerance>=0.5.2
 stable-baselines3>=2.0.0
 pulp>=2.7.0
 bayesian-optimization>=1.3.1
 iteround>=1.0.4
 emukit>=0.4.10
 GPy>=1.10.0
 numpy==1.23.5
```

### Comparing `csle_agents-0.5.1/tests/test_bayes_opt.py` & `csle_agents-0.5.2/tests/test_bayes_opt.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_bayes_opt_emukit.py` & `csle_agents-0.5.2/tests/test_bayes_opt_emukit.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_c51_clean.py` & `csle_agents-0.5.2/tests/test_c51_clean.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_cma_es.py` & `csle_agents-0.5.2/tests/test_cma_es.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_cross_entropy.py` & `csle_agents-0.5.2/tests/test_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_differential_evolution.py` & `csle_agents-0.5.2/tests/test_differential_evolution.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_dqn.py` & `csle_agents-0.5.2/tests/test_dqn.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_dqn_clean.py` & `csle_agents-0.5.2/tests/test_dqn_clean.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_dynasec.py` & `csle_agents-0.5.2/tests/test_dynasec.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_fp.py` & `csle_agents-0.5.2/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_hsvi.py` & `csle_agents-0.5.2/tests/test_hsvi.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_hsvi_os_posg.py` & `csle_agents-0.5.2/tests/test_hsvi_os_posg.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_kiefer_wolfowitz.py` & `csle_agents-0.5.2/tests/test_kiefer_wolfowitz.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_lp_cmdp.py` & `csle_agents-0.5.2/tests/test_lp_cmdp.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_lp_nf.py` & `csle_agents-0.5.2/tests/test_lp_nf.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_nelder_mead.py` & `csle_agents-0.5.2/tests/test_nelder_mead.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_particle_swarm.py` & `csle_agents-0.5.2/tests/test_particle_swarm.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_pi.py` & `csle_agents-0.5.2/tests/test_pi.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_ppg_clean.py` & `csle_agents-0.5.2/tests/test_ppg_clean.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_ppo.py` & `csle_agents-0.5.2/tests/test_ppo.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_ppo_clean.py` & `csle_agents-0.5.2/tests/test_ppo_clean.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_q_learning.py` & `csle_agents-0.5.2/tests/test_q_learning.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_random_search.py` & `csle_agents-0.5.2/tests/test_random_search.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_reinforce.py` & `csle_agents-0.5.2/tests/test_reinforce.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_sarsa.py` & `csle_agents-0.5.2/tests/test_sarsa.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_shapley_iteration.py` & `csle_agents-0.5.2/tests/test_shapley_iteration.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_simulated_annealing.py` & `csle_agents-0.5.2/tests/test_simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_sondik_vi.py` & `csle_agents-0.5.2/tests/test_sondik_vi.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_t_fp.py` & `csle_agents-0.5.2/tests/test_t_fp.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_t_spsa.py` & `csle_agents-0.5.2/tests/test_t_spsa.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.5.1/tests/test_vi.py` & `csle_agents-0.5.2/tests/test_vi.py`

 * *Files identical despite different names*

