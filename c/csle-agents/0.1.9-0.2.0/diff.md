# Comparing `tmp/csle_agents-0.1.9.tar.gz` & `tmp/csle_agents-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_agents-0.1.9.tar", last modified: Tue Mar 21 08:10:20 2023, max compression
+gzip compressed data, was "csle_agents-0.2.0.tar", last modified: Sun Apr 30 12:37:40 2023, max compression
```

## Comparing `csle_agents-0.1.9.tar` & `csle_agents-0.2.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/
--rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-03-21 08:10:20.905268 csle_agents-0.1.9/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     4154 2023-01-03 16:53:40.000000 csle_agents-0.1.9/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-02-11 20:28:41.000000 csle_agents-0.1.9/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1410 2023-03-21 08:10:20.905268 csle_agents-0.1.9/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_agents-0.1.9/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.893268 csle_agents-0.1.9/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.893268 csle_agents-0.1.9/src/csle_agents/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_agents-0.1.9/src/csle_agents/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.893268 csle_agents-0.1.9/src/csle_agents/agents/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/__init__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/base/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/base/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1854 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/base/base_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/bayes_opt/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/bayes_opt/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    27850 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/bayes_opt/bayes_opt_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/cross_entropy/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/cross_entropy/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    26825 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/differential_evolution/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/differential_evolution/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    31102 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/dqn/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/dqn/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    19026 2022-12-11 08:50:43.000000 csle_agents-0.1.9/src/csle_agents/agents/dqn/dqn_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/dynasec/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/dynasec/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    75221 2022-12-11 08:32:31.000000 csle_agents-0.1.9/src/csle_agents/agents/dynasec/dynasec_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/fp/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/fp/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18132 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/fp/fictitious_play_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/hsvi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/hsvi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    49186 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/hsvi/hsvi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/hsvi_os_posg/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/hsvi_os_posg/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    75141 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/kiefer_wolfowitz/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    29138 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/lp_nf/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/lp_nf/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18233 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/pi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/pi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17515 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/pi/pi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/ppo/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/ppo/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    23280 2023-03-17 07:49:22.000000 csle_agents-0.1.9/src/csle_agents/agents/ppo/ppo_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/q_learning/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/q_learning/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17233 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/q_learning/q_learning_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/random_search/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/random_search/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    26063 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/random_search/random_search_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/reinforce/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/reinforce/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    24982 2022-12-11 08:51:55.000000 csle_agents-0.1.9/src/csle_agents/agents/reinforce/reinforce_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/sarsa/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/sarsa/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17329 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/sarsa/sarsa_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/shapley_iteration/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/shapley_iteration/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15674 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/agents/sondik_vi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/sondik_vi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    22055 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/agents/t_fp/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/t_fp/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    41769 2022-12-11 08:32:31.000000 csle_agents-0.1.9/src/csle_agents/agents/t_fp/t_fp_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/agents/t_spsa/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/t_spsa/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    32591 2022-12-11 08:32:31.000000 csle_agents-0.1.9/src/csle_agents/agents/t_spsa/t_spsa_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/agents/vi/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/vi/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15759 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/vi/vi_agent.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/common/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/common/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5759 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/common/actor_critic_net.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4595 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/common/fnn_w_gaussian.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/common/fnn_w_linear.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3460 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/common/pruning.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10945 2023-03-06 21:38:13.000000 csle_agents-0.1.9/src/csle_agents/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/job_controllers/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/job_controllers/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2459 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/job_controllers/training_job_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.893268 csle_agents-0.1.9/src/csle_agents.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-03-21 08:10:20.000000 csle_agents-0.1.9/src/csle_agents.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     2852 2023-03-21 08:10:20.000000 csle_agents-0.1.9/src/csle_agents.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:10:20.000000 csle_agents-0.1.9/src/csle_agents.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:05.000000 csle_agents-0.1.9/src/csle_agents.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      371 2023-03-21 08:10:20.000000 csle_agents-0.1.9/src/csle_agents.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-03-21 08:10:20.000000 csle_agents-0.1.9/src/csle_agents.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.956838 csle_agents-0.2.0/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-04-30 12:37:40.956838 csle_agents-0.2.0/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4154 2023-03-28 14:03:22.000000 csle_agents-0.2.0/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-03-28 14:03:22.000000 csle_agents-0.2.0/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1410 2023-04-30 12:37:40.956838 csle_agents-0.2.0/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_agents-0.2.0/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/csle_agents/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_agents-0.2.0/src/csle_agents/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/csle_agents/agents/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/csle_agents/agents/base/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/base/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1854 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/base/base_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/csle_agents/agents/bayesian_optimization/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/bayesian_optimization/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28162 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/cross_entropy/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/cross_entropy/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    26946 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/differential_evolution/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/differential_evolution/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    31459 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/dqn/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/dqn/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19153 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/dqn/dqn_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/dynasec/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/dynasec/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    75392 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/dynasec/dynasec_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/fp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/fp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18259 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/fp/fictitious_play_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/hsvi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/hsvi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    49313 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/hsvi/hsvi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/hsvi_os_posg/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/hsvi_os_posg/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    75255 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/kiefer_wolfowitz/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    28849 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/lp_nf/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/lp_nf/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18360 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/pi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/pi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17642 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/pi/pi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.948838 csle_agents-0.2.0/src/csle_agents/agents/ppo/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/ppo/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    25515 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/ppo/ppo_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/q_learning/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/q_learning/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17360 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/q_learning/q_learning_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/random_search/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/random_search/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    26175 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/random_search/random_search_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/reinforce/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/reinforce/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    25109 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/reinforce/reinforce_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/sarsa/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/sarsa/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17456 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/sarsa/sarsa_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/shapley_iteration/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/shapley_iteration/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15788 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/sondik_vi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/sondik_vi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22182 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/t_fp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/t_fp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    41896 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/t_fp/t_fp_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/t_spsa/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/t_spsa/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    32105 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/t_spsa/t_spsa_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/agents/vi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/agents/vi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16358 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/agents/vi/vi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.952838 csle_agents-0.2.0/src/csle_agents/common/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/common/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5759 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/common/actor_critic_net.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4595 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/common/fnn_w_gaussian.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/common/fnn_w_linear.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3460 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/common/pruning.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.956838 csle_agents-0.2.0/src/csle_agents/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11221 2023-04-30 06:59:23.000000 csle_agents-0.2.0/src/csle_agents/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.956838 csle_agents-0.2.0/src/csle_agents/job_controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/job_controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2459 2023-03-28 14:03:22.000000 csle_agents-0.2.0/src/csle_agents/job_controllers/training_job_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:37:40.944838 csle_agents-0.2.0/src/csle_agents.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-04-30 12:37:40.000000 csle_agents-0.2.0/src/csle_agents.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2876 2023-04-30 12:37:40.000000 csle_agents-0.2.0/src/csle_agents.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:37:40.000000 csle_agents-0.2.0/src/csle_agents.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:05.000000 csle_agents-0.2.0/src/csle_agents.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      371 2023-04-30 12:37:40.000000 csle_agents-0.2.0/src/csle_agents.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-04-30 12:37:40.000000 csle_agents-0.2.0/src/csle_agents.egg-info/top_level.txt
```

### Comparing `csle_agents-0.1.9/PKG-INFO` & `csle_agents-0.2.0/src/csle_agents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: csle_agents
-Version: 0.1.9
+Name: csle-agents
+Version: 0.2.0
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.1.9/README.md` & `csle_agents-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.9/pyproject.toml` & `csle_agents-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.9/setup.cfg` & `csle_agents-0.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.1.9
-	csle-collector>=0.1.9
-	csle-attacker>=0.1.9
-	csle-defender>=0.1.9
-	csle-system-identification>=0.1.9
-	gym-csle-stopping-game>=0.1.9
-	stable-baselines3>=1.6.2
+	csle-common>=0.2.0
+	csle-collector>=0.2.0
+	csle-attacker>=0.2.0
+	csle-defender>=0.2.0
+	csle-system-identification>=0.2.0
+	gym-csle-stopping-game>=0.2.0
+	stable-baselines3>=1.8.0
 	pulp>=2.7.0
 	bayesian-optimization>=1.3.1
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/base/base_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/base/base_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/bayes_opt/bayes_opt_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from typing import Union, List, Dict, Optional
 import time
-import gym
+import gymnasium as gym
 import os
 import numpy as np
 from bayes_opt import BayesianOptimization
 from bayes_opt import UtilityFunction
 import gym_csle_stopping_game.constants.constants as env_constants
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
@@ -13,16 +13,19 @@
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
+from csle_common.dao.training.linear_threshold_stopping_policy import LinearThresholdStoppingPolicy
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
+from csle_common.util.general_util import GeneralUtil
+from csle_common.dao.training.policy_type import PolicyType
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
 class BayesOptAgent(BaseAgent):
     """
     Bayesian Optimization Agent
@@ -107,15 +110,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
@@ -134,15 +138,14 @@
             descr=descr, log_file_path=self.training_job.log_file_path)
         if self.save_to_metastore:
             exp_execution_id = MetastoreFacade.save_experiment_execution(self.exp_execution)
             self.exp_execution.id = exp_execution_id
 
         config = self.simulation_env_config.simulation_env_input_config
         if self.env is None:
-            print(f"MAKING GYM: {self.simulation_env_config.gym_env_name}")
             self.env = gym.make(self.simulation_env_config.gym_env_name, config=config)
         for seed in self.experiment_config.random_seeds:
             ExperimentUtil.set_seed(seed)
             exp_result = self.bayesian_optimization(exp_result=exp_result, seed=seed, training_job=self.training_job,
                                                     random_seeds=self.experiment_config.random_seeds)
 
             # Save latest trace
@@ -226,21 +229,15 @@
         else:
             if self.experiment_config.player_type == PlayerType.DEFENDER:
                 theta = BayesOptAgent.initial_theta(L=L)
             else:
                 theta = BayesOptAgent.initial_theta(L=2 * L)
 
         # Initial eval
-        policy = MultiThresholdStoppingPolicy(
-            theta=list(theta), simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.BAYESIAN_OPTIMIZATION)
+        policy = self.get_policy(theta=list(theta), L=L)
         avg_metrics = self.eval_theta(
             policy=policy,
             max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
         J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
         policy.avg_R = J
         exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
         exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(J)
@@ -272,61 +269,50 @@
                 f"Utility function: "
                 f"{self.experiment_config.hparams[agents_constants.BAYESIAN_OPTIMIZATION.UTILITY_FUNCTION].value} "
                 f"not recognized")
 
         for i in range(N):
             theta_candidate = optimizer.suggest(utility)
             theta = BayesOptAgent.get_theta_vector_from_param_dict(param_dict=theta_candidate)
-            candidate_policy = MultiThresholdStoppingPolicy(
-                theta=list(theta), simulation_name=self.simulation_env_config.name,
-                states=self.simulation_env_config.state_space_config.states,
-                player_type=self.experiment_config.player_type, L=L,
-                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                    self.experiment_config.player_idx].actions,
-                experiment_config=self.experiment_config, avg_R=-1,
-                agent_type=AgentType.BAYESIAN_OPTIMIZATION)
+            candidate_policy = self.get_policy(theta=list(theta), L=L)
             avg_metrics = self.eval_theta(
                 policy=candidate_policy,
                 max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
             J_candidate = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
             try:
                 optimizer.register(params=theta_candidate, target=J_candidate)
                 J = optimizer.max[agents_constants.BAYESIAN_OPTIMIZATION.TARGET]
             except Exception as e:
                 Logger.__call__().get_logger().info(
                     f"Exception, candidate:{theta_candidate}, exception: {str(e)}, {repr(e)}")
                 continue
 
             # Log average return
-            policy = MultiThresholdStoppingPolicy(
-                theta=list(BayesOptAgent.get_theta_vector_from_param_dict(
-                    optimizer.max[agents_constants.BAYESIAN_OPTIMIZATION.PARAMS])),
-                simulation_name=self.simulation_env_config.name,
-                states=self.simulation_env_config.state_space_config.states,
-                player_type=self.experiment_config.player_type, L=L,
-                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                    self.experiment_config.player_idx].actions,
-                experiment_config=self.experiment_config, avg_R=J,
-                agent_type=AgentType.BAYESIAN_OPTIMIZATION)
+            policy = self.get_policy(theta=list(BayesOptAgent.get_theta_vector_from_param_dict(
+                optimizer.max[agents_constants.BAYESIAN_OPTIMIZATION.PARAMS])), L=L)
             policy.avg_R = J
             running_avg_J = ExperimentUtil.running_average(
                 exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN],
                 self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value)
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(running_avg_J)
 
-            # Log thresholds
+            # Log thetas
             exp_result.all_metrics[seed][agents_constants.BAYESIAN_OPTIMIZATION.THETAS].append(
                 BayesOptAgent.round_vec(theta))
-            exp_result.all_metrics[seed][agents_constants.BAYESIAN_OPTIMIZATION.THRESHOLDS].append(
-                BayesOptAgent.round_vec(policy.thresholds()))
 
-            # Log stop distribution
-            for k, v in policy.stop_distributions().items():
-                exp_result.all_metrics[seed][k].append(v)
+            if self.experiment_config.hparams[agents_constants.BAYESIAN_OPTIMIZATION.POLICY_TYPE] \
+                    == PolicyType.MULTI_THRESHOLD:
+                # Log thresholds
+                exp_result.all_metrics[seed][agents_constants.BAYESIAN_OPTIMIZATION.THRESHOLDS].append(
+                    BayesOptAgent.round_vec(policy.thresholds()))
+
+                # Log stop distribution
+                for k, v in policy.stop_distributions().items():
+                    exp_result.all_metrics[seed][k].append(v)
 
             # Log intrusion lengths
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH].append(
                 round(avg_metrics[env_constants.ENV_METRICS.INTRUSION_LENGTH], 3))
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH].append(
                 ExperimentUtil.running_average(
                     exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH],
@@ -342,28 +328,31 @@
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON].append(
                 round(avg_metrics[env_constants.ENV_METRICS.TIME_HORIZON], 3))
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON].append(
                 ExperimentUtil.running_average(
                     exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON],
                     self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
             for l in range(1, self.experiment_config.hparams[agents_constants.BAYESIAN_OPTIMIZATION.L].value + 1):
-                exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
-                exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"].append(
-                    round(avg_metrics[env_constants.ENV_METRICS.STOP + f"_{l}"], 3))
-                exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_running_average_{l}"].append(
-                    ExperimentUtil.running_average(
-                        exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"],
-                        self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
+                if env_constants.ENV_METRICS.STOP + f"_{l}" in avg_metrics:
+                    exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
+                    exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"].append(
+                        round(avg_metrics[env_constants.ENV_METRICS.STOP + f"_{l}"], 3))
+                    exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_running_average_{l}"].append(
+                        ExperimentUtil.running_average(
+                            exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"],
+                            self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
 
             # Log baseline returns
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN].append(
                 round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN], 3))
-            exp_result.all_metrics[seed][
-                env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN].append(
-                round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN], 3))
+            if env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN in avg_metrics:
+                exp_result.all_metrics[seed][
+                    env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN].append(
+                    round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN],
+                          3))
 
             if i % self.experiment_config.log_every == 0 and i > 0:
                 # Update training job
                 total_iterations = len(random_seeds) * N
                 iterations_done = (random_seeds.index(seed)) * N + i
                 progress = round(iterations_done / total_iterations, 2)
                 training_job.progress_percentage = progress
@@ -385,56 +374,49 @@
 
                 Logger.__call__().get_logger().info(
                     f"[BAYES-OPT] i: {i}, J:{J}, "
                     f"J_avg_{self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value}:"
                     f"{running_avg_J}, "
                     f"opt_J:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN][-1]}, "
                     f"int_len:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH][-1]}, "
-                    f"sigmoid(theta):{policy.thresholds()}, progress: {round(progress*100,2)}%, "
-                    f"stop distributions:{policy.stop_distributions()}")
-
-        policy = MultiThresholdStoppingPolicy(
-            theta=list(theta), simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=J,
-            agent_type=AgentType.BAYESIAN_OPTIMIZATION)
+                    f"theta:{policy.theta}, progress: {round(progress*100,2)}%")
+        policy = self.get_policy(theta=list(theta), L=L)
         exp_result.policies[seed] = policy
         # Save policy
         if self.save_to_metastore:
             MetastoreFacade.save_multi_threshold_stopping_policy(multi_threshold_stopping_policy=policy)
         return exp_result
 
-    def eval_theta(self, policy: MultiThresholdStoppingPolicy, max_steps: int = 200) -> Dict[str, Union[float, int]]:
+    def eval_theta(self, policy: Union[MultiThresholdStoppingPolicy, LinearThresholdStoppingPolicy],
+                   max_steps: int = 200) -> Dict[str, Union[float, int]]:
         """
         Evaluates a given threshold policy by running monte-carlo simulations
 
         :param policy: the policy to evaluate
         :return: the average metrics of the evaluation
         """
         eval_batch_size = self.experiment_config.hparams[agents_constants.COMMON.EVAL_BATCH_SIZE].value
         metrics = {}
         for j in range(eval_batch_size):
             done = False
-            o = self.env.reset()
+            o, _ = self.env.reset()
             l = int(o[0])
             b1 = o[1]
             t = 1
             r = 0
             a = 0
             info = {}
             while not done and t <= max_steps:
                 Logger.__call__().get_logger().debug(f"t:{t}, a: {a}, b1:{b1}, r:{r}, l:{l}, info:{info}")
                 if self.experiment_config.player_type == PlayerType.ATTACKER:
                     policy.opponent_strategy = self.env.static_defender_strategy
                     a = policy.action(o=o)
                 else:
                     a = policy.action(o=o)
-                o, r, done, info = self.env.step(a)
+                o, r, done, _, info = self.env.step(a)
                 l = int(o[0])
                 b1 = o[1]
                 t += 1
             metrics = BayesOptAgent.update_metrics(metrics=metrics, info=info)
         avg_metrics = BayesOptAgent.compute_avg_metrics(metrics=metrics)
         return avg_metrics
 
@@ -498,7 +480,35 @@
         """
         Extracts the theta vector from the parameter dict
 
         :param param_dict: the parameter dict
         :return: the theta vector
         """
         return list(param_dict.values())
+
+    def get_policy(self, theta: List[float], L: int) \
+            -> Union[MultiThresholdStoppingPolicy, LinearThresholdStoppingPolicy]:
+        """
+        Utility method for getting the policy of a given parameter vector
+
+        :param theta: the parameter vector
+        :param L: the number of parameters
+        :return: the policy
+        """
+        if self.experiment_config.hparams[agents_constants.BAYESIAN_OPTIMIZATION.POLICY_TYPE] \
+                == PolicyType.MULTI_THRESHOLD:
+            policy = MultiThresholdStoppingPolicy(
+                theta=list(theta), simulation_name=self.simulation_env_config.name,
+                states=self.simulation_env_config.state_space_config.states,
+                player_type=self.experiment_config.player_type, L=L,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
+                agent_type=AgentType.BAYESIAN_OPTIMIZATION)
+        else:
+            policy = LinearThresholdStoppingPolicy(
+                theta=list(theta), simulation_name=self.simulation_env_config.name,
+                states=self.simulation_env_config.state_space_config.states,
+                player_type=self.experiment_config.player_type, L=L,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
+                agent_type=AgentType.BAYESIAN_OPTIMIZATION)
+        return policy
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import math
 from typing import Union, List, Dict, Optional
 import random
 import time
-import gym
+import gymnasium as gym
 import os
 import numpy as np
 from scipy import stats
 import gym_csle_stopping_game.constants.constants as env_constants
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
+from csle_common.dao.training.linear_threshold_stopping_policy import LinearThresholdStoppingPolicy
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
+from csle_common.dao.training.policy_type import PolicyType
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
 class CrossEntropyAgent(BaseAgent):
     """
     Cross-Entropy Agent
@@ -106,15 +109,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
@@ -219,21 +223,15 @@
         else:
             if self.experiment_config.player_type == PlayerType.DEFENDER:
                 theta = CrossEntropyAgent.initial_theta(L=L)
             else:
                 theta = CrossEntropyAgent.initial_theta(L=2 * L)
 
         # Initial eval
-        policy = MultiThresholdStoppingPolicy(
-            theta=list(theta), simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.CROSS_ENTROPY)
+        policy = self.get_policy(theta=list(theta), L=L)
         avg_metrics = self.eval_theta(
             policy=policy, max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
         J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
         policy.avg_R = J
         exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
         exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(J)
         exp_result.all_metrics[seed][agents_constants.CROSS_ENTROPY.THETAS].append(CrossEntropyAgent.round_vec(theta))
@@ -245,21 +243,15 @@
 
         # Hyperparameters
         N = self.experiment_config.hparams[agents_constants.CROSS_ENTROPY.N].value
         K = self.experiment_config.hparams[agents_constants.CROSS_ENTROPY.K].value
         lamb = self.experiment_config.hparams[agents_constants.CROSS_ENTROPY.LAMB].value
 
         # Initial eval
-        policy = MultiThresholdStoppingPolicy(
-            theta=list(theta), simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.CROSS_ENTROPY)
+        policy = self.get_policy(theta=list(theta), L=L)
         avg_metrics = self.eval_theta(
             policy=policy, max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
         J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
 
         means = []
         stds = []
         for l in range(L):
@@ -272,21 +264,15 @@
             for k in range(K):
                 theta_sample = norm_dist.rvs(1)
                 for i in range(len(theta_sample)):
                     if theta_sample[i] > 1:
                         theta_sample[i] = 0.99
                     if theta_sample[i] < 0:
                         theta_sample[i] = 0.01
-                policy = MultiThresholdStoppingPolicy(
-                    theta=list(theta_sample), simulation_name=self.simulation_env_config.name,
-                    states=self.simulation_env_config.state_space_config.states,
-                    player_type=self.experiment_config.player_type, L=L,
-                    actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                        self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-                    agent_type=AgentType.CROSS_ENTROPY)
+                policy = self.get_policy(theta=list(theta_sample), L=L)
                 avg_metrics = self.eval_theta(
                     policy=policy,
                     max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
                 J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
                 theta_samples_and_returns.append((theta_sample, J))
             sorted_samples = sorted(theta_samples_and_returns, key=lambda x: x[1], reverse=True)
             top_k_index = max(1, int(K * lamb))
@@ -380,53 +366,48 @@
                     f"J_avg_{self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value}:"
                     f"{running_avg_J}, "
                     f"opt_J:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN][-1]}, "
                     f"int_len:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH][-1]}, "
                     f"sigmoid(theta):{policy.thresholds()}, progress: {round(progress*100,2)}%, "
                     f"stop distributions:{policy.stop_distributions()}")
 
-        policy = MultiThresholdStoppingPolicy(
-            theta=list(theta), simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=J,
-            agent_type=AgentType.CROSS_ENTROPY)
+        policy = self.get_policy(theta=list(theta), L=L)
         exp_result.policies[seed] = policy
         # Save policy
         if self.save_to_metastore:
             MetastoreFacade.save_multi_threshold_stopping_policy(multi_threshold_stopping_policy=policy)
         return exp_result
 
-    def eval_theta(self, policy: MultiThresholdStoppingPolicy, max_steps: int = 200) -> Dict[str, Union[float, int]]:
+    def eval_theta(self, policy: Union[MultiThresholdStoppingPolicy, LinearThresholdStoppingPolicy],
+                   max_steps: int = 200) -> Dict[str, Union[float, int]]:
         """
         Evaluates a given threshold policy by running monte-carlo simulations
 
         :param policy: the policy to evaluate
         :return: the average metrics of the evaluation
         """
         eval_batch_size = self.experiment_config.hparams[agents_constants.COMMON.EVAL_BATCH_SIZE].value
         metrics = {}
         for j in range(eval_batch_size):
             done = False
-            o = self.env.reset()
+            o, _ = self.env.reset()
             l = int(o[0])
             b1 = o[1]
             t = 1
             r = 0
             a = 0
             info = {}
             while not done and t <= max_steps:
                 Logger.__call__().get_logger().debug(f"t:{t}, a: {a}, b1:{b1}, r:{r}, l:{l}, info:{info}")
                 if self.experiment_config.player_type == PlayerType.ATTACKER:
                     policy.opponent_strategy = self.env.static_defender_strategy
                     a = policy.action(o=o)
                 else:
                     a = policy.action(o=o)
-                o, r, done, info = self.env.step(a)
+                o, r, done, _, info = self.env.step(a)
                 l = int(o[0])
                 b1 = o[1]
                 t += 1
             metrics = CrossEntropyAgent.update_metrics(metrics=metrics, info=info)
         avg_metrics = CrossEntropyAgent.compute_avg_metrics(metrics=metrics)
         return avg_metrics
 
@@ -480,7 +461,35 @@
         """
         Rounds a vector to 3 decimals
 
         :param vec: the vector to round
         :return: the rounded vector
         """
         return list(map(lambda x: round(x, 3), vec))
+
+    def get_policy(self, theta: List[float], L: int) -> Union[LinearThresholdStoppingPolicy,
+                                                              MultiThresholdStoppingPolicy]:
+        """
+        Utility method for getting the policy of a given parameter vector
+
+        :param theta: the parameter vector
+        :param L: the number of parameters
+        :return: the policy
+        """
+        if self.experiment_config.hparams[agents_constants.CROSS_ENTROPY.POLICY_TYPE] \
+                == PolicyType.MULTI_THRESHOLD:
+            policy = MultiThresholdStoppingPolicy(
+                theta=theta, simulation_name=self.simulation_env_config.name,
+                states=self.simulation_env_config.state_space_config.states,
+                player_type=self.experiment_config.player_type, L=L,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
+                agent_type=AgentType.CROSS_ENTROPY)
+        else:
+            policy = LinearThresholdStoppingPolicy(
+                theta=theta, simulation_name=self.simulation_env_config.name,
+                states=self.simulation_env_config.state_space_config.states,
+                player_type=self.experiment_config.player_type, L=L,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
+                agent_type=AgentType.CROSS_ENTROPY)
+        return policy
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import math
 from typing import Union, List, Dict, Optional
 import random
 import time
-import gym
+import gymnasium as gym
 import os
 import numpy as np
 import gym_csle_stopping_game.constants.constants as env_constants
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
+from csle_common.dao.training.linear_threshold_stopping_policy import LinearThresholdStoppingPolicy
+from csle_common.dao.training.policy_type import PolicyType
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
 class DifferentialEvolutionAgent(BaseAgent):
     """
     Differential evolution agent
@@ -61,24 +64,26 @@
         exp_result.plot_metrics.append(agents_constants.COMMON.AVERAGE_RETURN)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_RETURN)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.INTRUSION_LENGTH)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.INTRUSION_START)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_START)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.TIME_HORIZON)
+        exp_result.plot_metrics.append(agents_constants.COMMON.RUNTIME)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN)
         for l in range(1, self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.L].value + 1):
             exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
             exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_running_average_{l}")
 
         descr = f"Training of policies with the differential evolution algorithm using " \
                 f"simulation:{self.simulation_env_config.name}"
         for seed in self.experiment_config.random_seeds:
+            self.start = time.time()
             exp_result.all_metrics[seed] = {}
             exp_result.all_metrics[seed][agents_constants.DIFFERENTIAL_EVOLUTION.THETAS] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.DIFFERENTIAL_EVOLUTION.THRESHOLDS] = []
             if self.experiment_config.player_type == PlayerType.DEFENDER:
                 for l in range(1, self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.L].value + 1):
@@ -89,14 +94,15 @@
                     for l in range(1,
                                    self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.L].value + 1):
                         exp_result.all_metrics[seed][agents_constants.DIFFERENTIAL_EVOLUTION.STOP_DISTRIBUTION_ATTACKER
                                                      + f"_l={l}_s={s.id}"] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_START] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH] = []
+            exp_result.all_metrics[seed][agents_constants.COMMON.RUNTIME] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_START] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = []
             exp_result.all_metrics[seed][
                 env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN] = []
             for l in range(1, self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.L].value + 1):
@@ -106,15 +112,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
@@ -222,35 +229,32 @@
         else:
             if self.experiment_config.player_type == PlayerType.DEFENDER:
                 theta = DifferentialEvolutionAgent.initial_theta(L=L)
             else:
                 theta = DifferentialEvolutionAgent.initial_theta(L=2 * L)
 
         # Initial eval
-        policy = MultiThresholdStoppingPolicy(
-            theta=list(theta), simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.DIFFERENTIAL_EVOLUTION)
+        policy = self.get_policy(theta=list(theta), L=L)
+        best_policy = policy
         avg_metrics = self.eval_theta(
             policy=policy,
             max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
         J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
         policy.avg_R = J
         exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
         exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(J)
         exp_result.all_metrics[seed][agents_constants.DIFFERENTIAL_EVOLUTION.THETAS].append(
             DifferentialEvolutionAgent.round_vec(theta))
+        time_elapsed_minutes = round((time.time() - self.start) / 60, 3)
+        exp_result.all_metrics[seed][agents_constants.COMMON.RUNTIME].append(time_elapsed_minutes)
 
         Logger.__call__().get_logger().info(
             f"[DIFFERENTIAL-EVOLUTION] i: {0}, J:{J}, "
             f"J_avg_{self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value}:"
-            f"{J}, sigmoid(theta):{policy.thresholds()}, progress: {0}%")
+            f"{J}, theta:{policy.theta}, runtime (m): {time_elapsed_minutes}, progress: {0}%")
 
         # Hyperparameters
         N = self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.N].value
         population_size = self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.POPULATION_SIZE].value
         mutate = self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.MUTATE].value
         recombination = self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.RECOMBINATION].value
         bounds = self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.BOUNDS].value
@@ -261,23 +265,15 @@
         for i in range(0, population_size):
             indv = []
             for j in range(len(bounds)):
                 indv.append(random.uniform(bounds[j][0], bounds[j][1]))
             population.append(indv)
 
         gen_sol = population[0]
-
-        candidate_policy = MultiThresholdStoppingPolicy(
-            theta=list(gen_sol), simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions,
-            experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.DIFFERENTIAL_EVOLUTION)
+        candidate_policy = self.get_policy(theta=list(gen_sol), L=L)
         avg_metrics = self.eval_theta(
             policy=candidate_policy,
             max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
         J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
         values.append(J)
 
         # cycle through each generation (step #2)
@@ -291,15 +287,15 @@
                 candidates = list(range(0, population_size))
                 candidates.remove(j)
                 random_index = random.sample(candidates, 3)
 
                 x_1 = population[random_index[0]]
                 x_2 = population[random_index[1]]
                 x_3 = population[random_index[2]]
-                x_t = population[j]     # target individual
+                x_t = population[j]  # target individual
 
                 # subtract x3 from x2, and create a new vector (x_diff)
                 x_diff = [x_2_i - x_3_i for x_2_i, x_3_i in zip(x_2, x_3)]
 
                 # multiply x_diff by the mutation factor (F) and add to x_1
                 v_donor = [x_1_i + mutate * x_diff_i for x_1_i, x_diff_i in zip(x_1, x_diff)]
                 # v_donor = self.ensure_bounds(v_donor, bounds)
@@ -312,76 +308,63 @@
                         v_trial.append(v_donor[k])
 
                     else:
                         v_trial.append(x_t[k])
                 v_trial = np.array(v_trial)
 
                 # GREEDY SELECTION STEP
-                candidate_policy = MultiThresholdStoppingPolicy(
-                    theta=list(v_trial), simulation_name=self.simulation_env_config.name,
-                    states=self.simulation_env_config.state_space_config.states,
-                    player_type=self.experiment_config.player_type, L=L,
-                    actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                        self.experiment_config.player_idx].actions,
-                    experiment_config=self.experiment_config, avg_R=-1,
-                    agent_type=AgentType.DIFFERENTIAL_EVOLUTION)
+                candidate_policy = self.get_policy(theta=list(v_trial), L=L)
                 avg_metrics = self.eval_theta(
                     policy=candidate_policy,
                     max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
                 score_trial = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
 
-                candidate_policy = MultiThresholdStoppingPolicy(
-                    theta=list(x_t), simulation_name=self.simulation_env_config.name,
-                    states=self.simulation_env_config.state_space_config.states,
-                    player_type=self.experiment_config.player_type, L=L,
-                    actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                        self.experiment_config.player_idx].actions,
-                    experiment_config=self.experiment_config, avg_R=-1,
-                    agent_type=AgentType.DIFFERENTIAL_EVOLUTION)
+                candidate_policy = self.get_policy(theta=list(x_t), L=L)
                 avg_metrics = self.eval_theta(
                     policy=candidate_policy,
                     max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
                 score_target = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
 
                 if score_trial > score_target:
                     population[j] = v_trial
                     gen_scores.append(score_trial)
                 else:
                     gen_scores.append(score_target)
 
-            gen_best = max(gen_scores)                                  # fitness of best individual
-            gen_sol = population[gen_scores.index(min(gen_scores))]     # solution of best individual
-            policy = MultiThresholdStoppingPolicy(
-                theta=gen_sol, simulation_name=self.simulation_env_config.name,
-                states=self.simulation_env_config.state_space_config.states,
-                player_type=self.experiment_config.player_type, L=L,
-                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                    self.experiment_config.player_idx].actions,
-                experiment_config=self.experiment_config, avg_R=-1,
-                agent_type=AgentType.DIFFERENTIAL_EVOLUTION)
+            gen_best = max(gen_scores)  # fitness of best individual
+            gen_sol = population[gen_scores.index(min(gen_scores))]  # solution of best individual
+            best_policy = self.get_policy(theta=list(gen_sol), L=L)
             values.append(gen_best)
             J = gen_best
 
             # Log average return
-            policy.avg_R = J
+            best_policy.avg_R = J
             running_avg_J = ExperimentUtil.running_average(
                 exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN],
                 self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value)
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(running_avg_J)
 
+            # log runtime
+            time_elapsed_minutes = round((time.time() - self.start) / 60, 3)
+            exp_result.all_metrics[seed][agents_constants.COMMON.RUNTIME].append(time_elapsed_minutes)
+
             # Log thresholds
             exp_result.all_metrics[seed][agents_constants.DIFFERENTIAL_EVOLUTION.THETAS].append(
                 DifferentialEvolutionAgent.round_vec(theta))
-            exp_result.all_metrics[seed][agents_constants.DIFFERENTIAL_EVOLUTION.THRESHOLDS].append(
-                DifferentialEvolutionAgent.round_vec(policy.thresholds()))
-
-            # Log stop distribution
-            for k, v in policy.stop_distributions().items():
-                exp_result.all_metrics[seed][k].append(v)
+            if self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.POLICY_TYPE] \
+                    == PolicyType.MULTI_THRESHOLD:
+                exp_result.all_metrics[seed][agents_constants.DIFFERENTIAL_EVOLUTION.THRESHOLDS].append(
+                    DifferentialEvolutionAgent.round_vec(best_policy.thresholds()))
+
+            if self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.POLICY_TYPE] \
+                    == PolicyType.MULTI_THRESHOLD:
+                # Log stop distribution
+                for k, v in best_policy.stop_distributions().items():
+                    exp_result.all_metrics[seed][k].append(v)
 
             # Log intrusion lengths
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH].append(
                 round(avg_metrics[env_constants.ENV_METRICS.INTRUSION_LENGTH], 3))
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH].append(
                 ExperimentUtil.running_average(
                     exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH],
@@ -396,29 +379,33 @@
                     self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON].append(
                 round(avg_metrics[env_constants.ENV_METRICS.TIME_HORIZON], 3))
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON].append(
                 ExperimentUtil.running_average(
                     exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON],
                     self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
-            for l in range(1, self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.L].value + 1):
-                exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
-                exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"].append(
-                    round(avg_metrics[env_constants.ENV_METRICS.STOP + f"_{l}"], 3))
-                exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_running_average_{l}"].append(
-                    ExperimentUtil.running_average(
-                        exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"],
-                        self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
+            if env_constants.ENV_METRICS.STOP + f"_{1}" in avg_metrics:
+                for l in range(1, self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.L].value + 1):
+                    exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
+                    exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"].append(
+                        round(avg_metrics[env_constants.ENV_METRICS.STOP + f"_{l}"], 3))
+                    exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_running_average_{l}"].append(
+                        ExperimentUtil.running_average(
+                            exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"],
+                            self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
 
             # Log baseline returns
-            exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN].append(
-                round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN], 3))
-            exp_result.all_metrics[seed][
-                env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN].append(
-                round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN], 3))
+            if env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN in avg_metrics:
+                exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN].append(
+                    round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN], 3))
+            if env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN in avg_metrics:
+                exp_result.all_metrics[seed][
+                    env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN].append(
+                    round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN],
+                          3))
 
             if i % self.experiment_config.log_every == 0 and i > 0:
                 # Update training job
                 total_iterations = len(random_seeds) * N
                 iterations_done = (random_seeds.index(seed)) * N + i
                 progress = round(iterations_done / total_iterations, 2)
                 training_job.progress_percentage = progress
@@ -434,62 +421,56 @@
                 ts = time.time()
                 self.exp_execution.timestamp = ts
                 self.exp_execution.result = exp_result
                 if self.save_to_metastore:
                     MetastoreFacade.update_experiment_execution(experiment_execution=self.exp_execution,
                                                                 id=self.exp_execution.id)
 
+                T_avg = exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON][-1]
                 Logger.__call__().get_logger().info(
                     f"[DIFFERENTIAL-EVOLUTION] i: {i}, J:{J}, "
                     f"J_avg_{self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value}:"
                     f"{running_avg_J}, "
                     f"opt_J:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN][-1]}, "
                     f"int_len:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH][-1]}, "
-                    f"sigmoid(theta):{policy.thresholds()}, progress: {round(progress*100,2)}%, "
-                    f"stop distributions:{policy.stop_distributions()}")
-
-        policy = MultiThresholdStoppingPolicy(
-            theta=list(theta), simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions,
-            experiment_config=self.experiment_config, avg_R=J, agent_type=AgentType.DIFFERENTIAL_EVOLUTION)
-        exp_result.policies[seed] = policy
+                    f"theta:{best_policy.theta}, T: {T_avg}, runtime (m): {time_elapsed_minutes}, "
+                    f"progress: {round(progress * 100, 2)}%")
+        exp_result.policies[seed] = best_policy
         # Save policy
         if self.save_to_metastore:
             MetastoreFacade.save_multi_threshold_stopping_policy(multi_threshold_stopping_policy=policy)
         return exp_result
 
-    def eval_theta(self, policy: MultiThresholdStoppingPolicy, max_steps: int = 200) -> Dict[str, Union[float, int]]:
+    def eval_theta(self, policy: Union[MultiThresholdStoppingPolicy, LinearThresholdStoppingPolicy],
+                   max_steps: int = 200) -> Dict[str, Union[float, int]]:
         """
         Evaluates a given threshold policy by running monte-carlo simulations
 
         :param policy: the policy to evaluate
         :return: the average metrics of the evaluation
         """
         eval_batch_size = self.experiment_config.hparams[agents_constants.COMMON.EVAL_BATCH_SIZE].value
         metrics = {}
         for j in range(eval_batch_size):
             done = False
-            o = self.env.reset()
+            o, _ = self.env.reset()
             l = int(o[0])
             b1 = o[1]
             t = 1
             r = 0
             a = 0
             info = {}
             while not done and t <= max_steps:
                 Logger.__call__().get_logger().debug(f"t:{t}, a: {a}, b1:{b1}, r:{r}, l:{l}, info:{info}")
                 if self.experiment_config.player_type == PlayerType.ATTACKER:
                     policy.opponent_strategy = self.env.static_defender_strategy
                     a = policy.action(o=o)
                 else:
                     a = policy.action(o=o)
-                o, r, done, info = self.env.step(a)
+                o, r, done, _, info = self.env.step(a)
                 l = int(o[0])
                 b1 = o[1]
                 t += 1
             metrics = DifferentialEvolutionAgent.update_metrics(metrics=metrics, info=info)
         avg_metrics = DifferentialEvolutionAgent.compute_avg_metrics(metrics=metrics)
         return avg_metrics
 
@@ -569,7 +550,35 @@
                 vec_new.append(bounds[i][1])
 
             # the variable is fine
             if bounds[i][0] <= vec[i] <= bounds[i][1]:
                 vec_new.append(vec[i])
 
         return vec_new
+
+    def get_policy(self, theta: List[float], L: int) -> Union[MultiThresholdStoppingPolicy,
+                                                              LinearThresholdStoppingPolicy]:
+        """
+        Utility method for getting the policy from a parameter vector
+
+        :param theta: the parameter vector
+        :param L: the number of parameters
+        :return: the policy
+        """
+        if self.experiment_config.hparams[agents_constants.DIFFERENTIAL_EVOLUTION.POLICY_TYPE] \
+                == PolicyType.MULTI_THRESHOLD:
+            policy = MultiThresholdStoppingPolicy(
+                theta=list(theta), simulation_name=self.simulation_env_config.name,
+                states=self.simulation_env_config.state_space_config.states,
+                player_type=self.experiment_config.player_type, L=L,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
+                agent_type=AgentType.DIFFERENTIAL_EVOLUTION)
+        else:
+            policy = LinearThresholdStoppingPolicy(
+                theta=list(theta), simulation_name=self.simulation_env_config.name,
+                states=self.simulation_env_config.state_space_config.states,
+                player_type=self.experiment_config.player_type, L=L,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
+                agent_type=AgentType.DIFFERENTIAL_EVOLUTION)
+        return policy
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/dqn/dqn_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/dqn/dqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union, List, Optional
 import time
-import gym
+import gymnasium as gym
 import os
 import numpy as np
 from stable_baselines3 import DQN
 from stable_baselines3.common.callbacks import BaseCallback
 from stable_baselines3.common.vec_env.vec_monitor import VecMonitor
 from stable_baselines3.common.vec_env.dummy_vec_env import DummyVecEnv
 from stable_baselines3.common.env_util import make_vec_env
@@ -19,14 +19,15 @@
 from csle_common.logging.log import Logger
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 from csle_common.dao.training.dqn_policy import DQNPolicy
 from csle_common.dao.simulation_config.state import State
 from csle_common.dao.simulation_config.action import Action
 from csle_common.dao.training.player_type import PlayerType
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
 class DQNAgent(BaseAgent):
     """
     A DQN agent using the implementation from OpenAI baselines
@@ -52,15 +53,16 @@
         # Setup training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
             self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
             MetastoreFacade.update_training_job(training_job=self.training_job, id=self.training_job.id)
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/dynasec/dynasec_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/dynasec/dynasec_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 from typing import List, Optional, Dict, Tuple
 import time
-import gym
+import gymnasium as gym
 import os
 import sys
 import numpy as np
 import threading
 import gym_csle_stopping_game.constants.constants as env_constants
 import csle_common.constants.constants as constants
 from csle_system_identification.emulator import Emulator
@@ -28,25 +28,26 @@
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 from csle_common.dao.system_identification.emulation_statistics import EmulationStatistics
 from csle_agents.agents.base.base_agent import BaseAgent
 from csle_common.dao.emulation_action.attacker.emulation_attacker_stopping_actions \
     import EmulationAttackerStoppingActions
 from csle_common.dao.emulation_action.defender.emulation_defender_stopping_actions \
     import EmulationDefenderStoppingActions
-import csle_agents.constants.constants as agents_constants
-from csle_system_identification.expectation_maximization.expectation_maximization_algorithm \
-    import ExpectationMaximizationAlgorithm
 from csle_common.dao.system_identification.gaussian_mixture_system_model import GaussianMixtureSystemModel
-from csle_agents.agents.t_spsa.t_spsa_agent import TSPSAAgent
-import csle_system_identification.constants.constants as system_identification_constants
 from csle_common.dao.system_identification.system_identification_config import SystemIdentificationConfig
 from csle_common.dao.training.policy import Policy
 from csle_common.util.read_emulation_statistics_util import ReadEmulationStatisticsUtil
 from csle_common.dao.emulation_config.static_emulation_attacker_type import StaticEmulationAttackerType
 from csle_common.dao.emulation_config.emulation_statistics_windowed import EmulationStatisticsWindowed
+from csle_common.util.general_util import GeneralUtil
+import csle_system_identification.constants.constants as system_identification_constants
+from csle_system_identification.expectation_maximization.expectation_maximization_algorithm \
+    import ExpectationMaximizationAlgorithm
+from csle_agents.agents.t_spsa.t_spsa_agent import TSPSAAgent
+import csle_agents.constants.constants as agents_constants
 
 
 class DataCollectorProcess(threading.Thread):
     """
     Process that interacts with an emulation execution to generate data
     """
 
@@ -87,15 +88,15 @@
             num_collected_steps=0, progress_percentage=0.0,
             attacker_sequence=attacker_sequence, defender_sequence=defender_sequence,
             pid=self.pid, descr=f"Data collection process in DynaSec with id: {self.worker_id}",
             repeat_times=10000, emulation_statistic_id=self.emulation_statistics_windowed.statistics_id,
             traces=[],
             num_sequences_completed=0, save_emulation_traces_every=1000000,
             num_cached_traces=emulation_traces_to_save_with_data_collection_job,
-            log_file_path=Logger.__call__().get_log_file_path())
+            log_file_path=Logger.__call__().get_log_file_path(), physical_host_ip=GeneralUtil.get_host_ip())
         self.job_id = MetastoreFacade.save_data_collection_job(
             data_collection_job=self.data_collection_job)
         self.data_collection_job.id = self.job_id
         self.emulation_traces = []
         self.statistics_id = self.emulation_statistics_windowed.statistics_id
         self.completed_episodes = 0
 
@@ -856,15 +857,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/fp/fictitious_play_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/fp/fictitious_play_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import math
 from typing import Union, List, Dict, Optional, Tuple
 import time
-import gym
+import gymnasium as gym
 import os
 import numpy as np
 import gym_csle_stopping_game.constants.constants as env_constants
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.dao.training.vector_policy import VectorPolicy
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
 class FictitiousPlayAgent(BaseAgent):
     """
     Fictitious Play Agent for Normal-form Games (Brown 1951)
@@ -86,15 +87,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=None, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/hsvi/hsvi_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/hsvi/hsvi_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import math
 from typing import List, Optional, Tuple
 import time
 import os
 import numpy as np
-import gym
+import gymnasium as gym
 import pulp
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.alpha_vectors_policy import AlphaVectorsPolicy
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 import csle_agents.common.pruning as pruning
 
 
 class HSVIAgent(BaseAgent):
     """
@@ -75,15 +76,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=None, simulation_traces=[],
                 num_cached_traces=0,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.alpha_vectors_policy import AlphaVectorsPolicy
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 import csle_agents.common.pruning as pruning
 
 
 class HSVIOSPOSGAgent(BaseAgent):
     """
@@ -66,15 +67,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=None, simulation_traces=[],
                 num_cached_traces=0,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/random_search/random_search_agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 import math
 from typing import Union, List, Dict, Optional
 import time
-import gym
+import gymnasium as gym
 import os
 import numpy as np
 import gym_csle_stopping_game.constants.constants as env_constants
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
+from csle_common.dao.training.linear_threshold_stopping_policy import LinearThresholdStoppingPolicy
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
+from csle_common.util.general_util import GeneralUtil
+from csle_common.dao.training.policy_type import PolicyType
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
-class KieferWolfowitzAgent(BaseAgent):
+class RandomSearchAgent(BaseAgent):
     """
-    RL Agent implementing the Kiefer-Wolfowitz SA algorithm from the 50s
+    Random Search Agent
     """
 
     def __init__(self, simulation_env_config: SimulationEnvConfig,
                  emulation_env_config: Union[None, EmulationEnvConfig],
                  experiment_config: ExperimentConfig, env: Optional[gym.Env] = None,
                  training_job: Optional[TrainingJobConfig] = None, save_to_metastore: bool = True):
         """
-        Initializes the Kiefer-Wolfowitz agent
+        Initializes the Random Search Agent
 
         :param simulation_env_config: the simulation env config
         :param emulation_env_config: the emulation env config
         :param experiment_config: the experiment config
         :param env: (optional) the gym environment to use for simulation
         :param training_job: (optional) a training job configuration
         :param save_to_metastore: boolean flag that can be set to avoid saving results and progress to the metastore
         """
         super().__init__(simulation_env_config=simulation_env_config, emulation_env_config=emulation_env_config,
                          experiment_config=experiment_config)
-        assert experiment_config.agent_type == AgentType.KIEFER_WOLFOWITZ
+        assert experiment_config.agent_type == AgentType.RANDOM_SEARCH
         self.env = env
         self.training_job = training_job
         self.save_to_metastore = save_to_metastore
 
     def train(self) -> ExperimentExecution:
         """
-        Performs the policy training for the given random seeds using Kiefer-Wolfowitz
+        Performs the policy training for the given random seeds using random search
 
         :return: the training metrics and the trained policies
         """
         pid = os.getpid()
 
         # Initialize metrics
         exp_result = ExperimentResult()
@@ -63,56 +66,57 @@
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.INTRUSION_START)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_START)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.TIME_HORIZON)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN)
-        for l in range(1, self.experiment_config.hparams[agents_constants.KIEFER_WOLFOWITZ.L].value + 1):
+        for l in range(1, self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value + 1):
             exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
             exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_running_average_{l}")
 
-        descr = f"Training of policies with the Kiefer-Wolfowitz algorithm using " \
+        descr = f"Training of policies with the random search algorithm using " \
                 f"simulation:{self.simulation_env_config.name}"
         for seed in self.experiment_config.random_seeds:
             exp_result.all_metrics[seed] = {}
-            exp_result.all_metrics[seed][agents_constants.KIEFER_WOLFOWITZ.THETAS] = []
+            exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.THETAS] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN] = []
-            exp_result.all_metrics[seed][agents_constants.KIEFER_WOLFOWITZ.THRESHOLDS] = []
+            exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.THRESHOLDS] = []
             if self.experiment_config.player_type == PlayerType.DEFENDER:
-                for l in range(1, self.experiment_config.hparams[agents_constants.KIEFER_WOLFOWITZ.L].value + 1):
+                for l in range(1, self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value + 1):
                     exp_result.all_metrics[seed][
-                        agents_constants.KIEFER_WOLFOWITZ.STOP_DISTRIBUTION_DEFENDER + f"_l={l}"] = []
+                        agents_constants.RANDOM_SEARCH.STOP_DISTRIBUTION_DEFENDER + f"_l={l}"] = []
             else:
                 for s in self.simulation_env_config.state_space_config.states:
-                    for l in range(1, self.experiment_config.hparams[agents_constants.KIEFER_WOLFOWITZ.L].value + 1):
-                        exp_result.all_metrics[seed][agents_constants.KIEFER_WOLFOWITZ.STOP_DISTRIBUTION_ATTACKER
+                    for l in range(1, self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value + 1):
+                        exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.STOP_DISTRIBUTION_ATTACKER
                                                      + f"_l={l}_s={s.id}"] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_START] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_START] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = []
             exp_result.all_metrics[seed][
                 env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN] = []
-            for l in range(1, self.experiment_config.hparams[agents_constants.KIEFER_WOLFOWITZ.L].value + 1):
+            for l in range(1, self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value + 1):
                 exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"] = []
                 exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_running_average_{l}"] = []
 
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
@@ -121,28 +125,28 @@
 
         # Initialize execution result
         ts = time.time()
         emulation_name = None
         if self.emulation_env_config is not None:
             emulation_name = self.emulation_env_config.name
         simulation_name = self.simulation_env_config.name
-        self.exp_execution = ExperimentExecution(result=exp_result, config=self.experiment_config, timestamp=ts,
-                                                 emulation_name=emulation_name, simulation_name=simulation_name,
-                                                 descr=descr, log_file_path=self.training_job.log_file_path)
+        self.exp_execution = ExperimentExecution(
+            result=exp_result, config=self.experiment_config, timestamp=ts, emulation_name=emulation_name,
+            simulation_name=simulation_name, descr=descr, log_file_path=self.training_job.log_file_path)
         if self.save_to_metastore:
             exp_execution_id = MetastoreFacade.save_experiment_execution(self.exp_execution)
             self.exp_execution.id = exp_execution_id
 
         config = self.simulation_env_config.simulation_env_input_config
         if self.env is None:
             self.env = gym.make(self.simulation_env_config.gym_env_name, config=config)
         for seed in self.experiment_config.random_seeds:
             ExperimentUtil.set_seed(seed)
-            exp_result = self.kiefer_wolfowitz(exp_result=exp_result, seed=seed, training_job=self.training_job,
-                                               random_seeds=self.experiment_config.random_seeds)
+            exp_result = self.random_search(exp_result=exp_result, seed=seed, training_job=self.training_job,
+                                            random_seeds=self.experiment_config.random_seeds)
 
             # Save latest trace
             if self.save_to_metastore:
                 MetastoreFacade.save_simulation_trace(self.env.get_traces()[-1])
             self.env.reset_traces()
 
         # Calculate average and std metrics
@@ -190,111 +194,87 @@
                                                         id=self.exp_execution.id)
         return self.exp_execution
 
     def hparam_names(self) -> List[str]:
         """
         :return: a list with the hyperparameter names
         """
-        return [agents_constants.KIEFER_WOLFOWITZ.N, agents_constants.KIEFER_WOLFOWITZ.DELTA,
-                agents_constants.KIEFER_WOLFOWITZ.INITIAL_ALPHA,
-                agents_constants.KIEFER_WOLFOWITZ.L, agents_constants.KIEFER_WOLFOWITZ.THETA1,
+        return [agents_constants.RANDOM_SEARCH.N, agents_constants.RANDOM_SEARCH.DELTA,
+                agents_constants.RANDOM_SEARCH.L, agents_constants.RANDOM_SEARCH.THETA1,
                 agents_constants.COMMON.EVAL_BATCH_SIZE,
-                agents_constants.KIEFER_WOLFOWITZ.GRADIENT_BATCH_SIZE, agents_constants.COMMON.CONFIDENCE_INTERVAL,
+                agents_constants.COMMON.CONFIDENCE_INTERVAL,
                 agents_constants.COMMON.RUNNING_AVERAGE]
 
-    def kiefer_wolfowitz(self, exp_result: ExperimentResult, seed: int, training_job: TrainingJobConfig,
-                         random_seeds: List[int]) -> ExperimentResult:
+    def random_search(self, exp_result: ExperimentResult, seed: int,
+                      training_job: TrainingJobConfig, random_seeds: List[int]) -> ExperimentResult:
         """
-        Runs the Kiefer-Wolfowitz algorithm
+        Runs the random search algorithm
 
         :param exp_result: the experiment result object to store the result
         :param seed: the seed
         :param training_job: the training job config
         :param random_seeds: list of seeds
         :return: the updated experiment result and the trained policy
         """
-        L = self.experiment_config.hparams[agents_constants.KIEFER_WOLFOWITZ.L].value
-        if agents_constants.KIEFER_WOLFOWITZ.THETA1 in self.experiment_config.hparams:
-            theta = self.experiment_config.hparams[agents_constants.KIEFER_WOLFOWITZ.THETA1].value
+        L = self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value
+        if agents_constants.RANDOM_SEARCH.THETA1 in self.experiment_config.hparams:
+            theta = self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.THETA1].value
         else:
             if self.experiment_config.player_type == PlayerType.DEFENDER:
-                theta = KieferWolfowitzAgent.initial_theta(L=L)
+                theta = RandomSearchAgent.initial_theta(L=L)
             else:
-                theta = KieferWolfowitzAgent.initial_theta(L=2 * L)
+                theta = RandomSearchAgent.initial_theta(L=2 * L)
 
         # Initial eval
-        policy = MultiThresholdStoppingPolicy(
-            theta=theta, simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.KIEFER_WOLFOWITZ)
+        policy = self.get_policy(theta=list(theta), L=L)
         avg_metrics = self.eval_theta(
             policy=policy, max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
         J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
         policy.avg_R = J
         exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
         exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(J)
-        exp_result.all_metrics[seed][
-            agents_constants.KIEFER_WOLFOWITZ.THETAS].append(KieferWolfowitzAgent.round_vec(theta))
+        exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.THETAS].append(RandomSearchAgent.round_vec(theta))
 
         # Hyperparameters
-        N = self.experiment_config.hparams[agents_constants.KIEFER_WOLFOWITZ.N].value
-        delta = self.experiment_config.hparams[agents_constants.KIEFER_WOLFOWITZ.DELTA].value
-        initial_alpha = self.experiment_config.hparams[agents_constants.KIEFER_WOLFOWITZ.INITIAL_ALPHA].value
-        gradient_batch_size = self.experiment_config.hparams[
-            agents_constants.KIEFER_WOLFOWITZ.GRADIENT_BATCH_SIZE].value
+        N = self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.N].value
+        delta = self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.DELTA].value
 
-        for i in range(N):
-            # Step sizes and perturbation size
-            alpha = initial_alpha / (i + 1)
-
-            # Get estimated gradient
-            gk = self.batch_gradient(theta=theta, L=L, delta=delta, gradient_batch_size=gradient_batch_size)
-
-            # Adjust theta using SA
-            theta = list(np.array(theta) + alpha * np.array(gk))
+        # Initial eval
+        policy = self.get_policy(theta=list(theta), L=L)
+        avg_metrics = self.eval_theta(
+            policy=policy, max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
+        J_0 = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
 
-            # Constrain (Theorem 1.A, Hammar Stadler 2021)
-            if self.experiment_config.player_type == PlayerType.DEFENDER:
-                for l in range(L - 1):
-                    theta[l] = max(theta[l], theta[l + 1])
-            else:
-                if self.experiment_config.player_type == PlayerType.ATTACKER:
-                    for l in range(0, L - 1):
-                        theta[l] = min(theta[l], theta[l + 1])
-                    for l in range(L, 2 * L - 1):
-                        theta[l] = max(theta[l], theta[l + 1])
+        for i in range(N):
 
-            # Evaluate new theta
-            policy = MultiThresholdStoppingPolicy(
-                theta=theta, simulation_name=self.simulation_env_config.name,
-                states=self.simulation_env_config.state_space_config.states,
-                player_type=self.experiment_config.player_type, L=L,
-                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-                agent_type=AgentType.KIEFER_WOLFOWITZ)
+            theta_candidate = self.random_perturbation(delta=delta, theta=theta)
+            candidate_policy = self.get_policy(theta=list(theta_candidate), L=L)
             avg_metrics = self.eval_theta(
-                policy=policy, max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
+                policy=candidate_policy,
+                max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
+            J_candidate = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
+            if J_candidate > J_0:
+                theta = theta_candidate
+                J_0 = J_candidate
+                policy = candidate_policy
 
             # Log average return
-            J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
+            J = J_0
             policy.avg_R = J
             running_avg_J = ExperimentUtil.running_average(
                 exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN],
                 self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value)
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(running_avg_J)
 
             # Log thresholds
-            exp_result.all_metrics[seed][agents_constants.KIEFER_WOLFOWITZ.THETAS].append(
-                KieferWolfowitzAgent.round_vec(theta))
-            exp_result.all_metrics[seed][agents_constants.KIEFER_WOLFOWITZ.THRESHOLDS].append(
-                KieferWolfowitzAgent.round_vec(policy.thresholds()))
+            exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.THETAS].append(
+                RandomSearchAgent.round_vec(theta))
+            exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.THRESHOLDS].append(
+                RandomSearchAgent.round_vec(policy.thresholds()))
 
             # Log stop distribution
             for k, v in policy.stop_distributions().items():
                 exp_result.all_metrics[seed][k].append(v)
 
             # Log intrusion lengths
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH].append(
@@ -313,15 +293,15 @@
                     self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON].append(
                 round(avg_metrics[env_constants.ENV_METRICS.TIME_HORIZON], 3))
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON].append(
                 ExperimentUtil.running_average(
                     exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON],
                     self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
-            for l in range(1, self.experiment_config.hparams[agents_constants.KIEFER_WOLFOWITZ.L].value + 1):
+            for l in range(1, self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value + 1):
                 exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
                 exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"].append(
                     round(avg_metrics[env_constants.ENV_METRICS.STOP + f"_{l}"], 3))
                 exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_running_average_{l}"].append(
                     ExperimentUtil.running_average(
                         exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"],
                         self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
@@ -352,36 +332,30 @@
                 self.exp_execution.timestamp = ts
                 self.exp_execution.result = exp_result
                 if self.save_to_metastore:
                     MetastoreFacade.update_experiment_execution(experiment_execution=self.exp_execution,
                                                                 id=self.exp_execution.id)
 
                 Logger.__call__().get_logger().info(
-                    f"[Kiefer-Wolfowitz] i: {i}, J:{J}, "
+                    f"[RANDOM-SEARCH] i: {i}, J:{J}, "
                     f"J_avg_{self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value}:"
                     f"{running_avg_J}, "
                     f"opt_J:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN][-1]}, "
                     f"int_len:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH][-1]}, "
                     f"sigmoid(theta):{policy.thresholds()}, progress: {round(progress*100,2)}%, "
                     f"stop distributions:{policy.stop_distributions()}")
-
-        policy = MultiThresholdStoppingPolicy(
-            theta=theta, simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=J,
-            agent_type=AgentType.KIEFER_WOLFOWITZ)
+        policy = self.get_policy(theta=list(theta), L=L)
         exp_result.policies[seed] = policy
         # Save policy
         if self.save_to_metastore:
             MetastoreFacade.save_multi_threshold_stopping_policy(multi_threshold_stopping_policy=policy)
         return exp_result
 
-    def eval_theta(self, policy: MultiThresholdStoppingPolicy, max_steps: int = 200) -> Dict[str, Union[float, int]]:
+    def eval_theta(self, policy: Union[MultiThresholdStoppingPolicy, LinearThresholdStoppingPolicy],
+                   max_steps: int = 200) -> Dict[str, Union[float, int]]:
         """
         Evaluates a given threshold policy by running monte-carlo simulations
 
         :param policy: the policy to evaluate
         :return: the average metrics of the evaluation
         """
         eval_batch_size = self.experiment_config.hparams[agents_constants.COMMON.EVAL_BATCH_SIZE].value
@@ -402,18 +376,32 @@
                     a = policy.action(o=o)
                 else:
                     a = policy.action(o=o)
                 o, r, done, info = self.env.step(a)
                 l = int(o[0])
                 b1 = o[1]
                 t += 1
-            metrics = KieferWolfowitzAgent.update_metrics(metrics=metrics, info=info)
-        avg_metrics = KieferWolfowitzAgent.compute_avg_metrics(metrics=metrics)
+            metrics = RandomSearchAgent.update_metrics(metrics=metrics, info=info)
+        avg_metrics = RandomSearchAgent.compute_avg_metrics(metrics=metrics)
         return avg_metrics
 
+    def random_perturbation(self, delta: float, theta: np.ndarray) -> np.ndarray:
+        """
+        Performs a random perturbation to the theta vector
+
+        :param delta: the step size for the perturbation
+        :param theta: the current theta vector
+        :return: the perturbed theta vector
+        """
+        perturbed_theta = []
+        for l in range(len(theta)):
+            Delta = np.random.uniform(-delta, delta)
+            perturbed_theta.append(theta[l] + Delta)
+        return np.array(perturbed_theta)
+
     @staticmethod
     def update_metrics(metrics: Dict[str, List[Union[float, int]]], info: Dict[str, Union[float, int]]) \
             -> Dict[str, List[Union[float, int]]]:
         """
         Update a dict with aggregated metrics using new information from the environment
 
         :param metrics: the dict with the aggregated metrics
@@ -451,76 +439,44 @@
         """
         theta_1 = []
         for k in range(L):
             theta_1.append(np.random.uniform(-3, 3))
         theta_1 = np.array(theta_1)
         return theta_1
 
-    def batch_gradient(self, theta: List[float], delta: float, L: int, gradient_batch_size: int = 1):
-        """
-        Computes a batch of gradients and returns the average
-
-        :param theta: the current parameter vector
-        :param ck: the perturbation step size
-        :param L: the total number of stops for the defender
-        :param gradient_batch_size: the number of gradients to include in the batch
-        :return: the average of the batch of gradients
-        """
-        gradients = []
-        for i in range(gradient_batch_size):
-            gk_i = self.estimate_gk(theta=theta, delta=delta, L=L)
-            gradients.append(gk_i)
-        batch_gk = (np.matrix(gradients).sum(axis=0) * (1 / gradient_batch_size)).tolist()[0]
-        return batch_gk
-
-    def estimate_gk(self, theta: float, delta: List[float], L: int):
-        """
-        Estimate the gradient at iteration k of the Kiefer-Wolfowitz algorithm
-
-        :param theta: the current parameter vector
-        :param delta: the perturbation size
-        :param L: the total number of stops for the defender
-        :return: the estimated gradient
-        """
-        gradient = []
-        for l in range(1, L + 1):
-            perturbed_theta_1 = theta.copy()
-            perturbed_theta_2 = theta.copy()
-            theta_l = theta[l - 1]
-            perturbed_theta_1[l - 1] = theta_l + delta
-            perturbed_theta_2[l - 1] = theta_l - delta
-            # Calculate g_k(theta_k)
-            avg_metrics = self.eval_theta(MultiThresholdStoppingPolicy(
-                theta=perturbed_theta_1, simulation_name=self.simulation_env_config.name,
-                player_type=self.experiment_config.player_type,
-                states=self.simulation_env_config.state_space_config.states, L=L,
-                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-                agent_type=AgentType.KIEFER_WOLFOWITZ),
-                max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value
-            )
-            J_a = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
-            avg_metrics = self.eval_theta(MultiThresholdStoppingPolicy(
-                theta=perturbed_theta_2, simulation_name=self.simulation_env_config.name,
-                player_type=self.experiment_config.player_type,
-                states=self.simulation_env_config.state_space_config.states, L=L,
-                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-                agent_type=AgentType.KIEFER_WOLFOWITZ),
-                max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
-            J_b = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
-            numerator = J_a - J_b
-            denumerator = 2 * delta
-            g_l = numerator / denumerator
-            gradient.append(g_l)
-
-        return gradient
-
     @staticmethod
     def round_vec(vec) -> List[float]:
         """
         Rounds a vector to 3 decimals
 
         :param vec: the vector to round
         :return: the rounded vector
         """
         return list(map(lambda x: round(x, 3), vec))
+
+    def get_policy(self, theta: List[float], L: int) -> Union[MultiThresholdStoppingPolicy,
+                                                              LinearThresholdStoppingPolicy]:
+        """
+        Gets the policy of a given parameter vector
+
+        :param theta: the parameter vector
+        :param L: the number of parameters
+        :return: the policy
+        """
+        if self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.POLICY_TYPE] \
+                == PolicyType.MULTI_THRESHOLD:
+            policy = MultiThresholdStoppingPolicy(
+                theta=list(theta), simulation_name=self.simulation_env_config.name,
+                states=self.simulation_env_config.state_space_config.states,
+                player_type=self.experiment_config.player_type, L=L,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
+                agent_type=AgentType.RANDOM_SEARCH)
+        else:
+            policy = LinearThresholdStoppingPolicy(
+                theta=list(theta), simulation_name=self.simulation_env_config.name,
+                states=self.simulation_env_config.state_space_config.states,
+                player_type=self.experiment_config.player_type, L=L,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
+                agent_type=AgentType.RANDOM_SEARCH)
+        return policy
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from typing import Union, List, Dict, Optional, Tuple
 import time
-import gym
+import gymnasium as gym
 import os
 import numpy as np
 import pulp
 import gym_csle_stopping_game.constants.constants as env_constants
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
@@ -13,14 +13,15 @@
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.dao.training.vector_policy import VectorPolicy
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
 class LinearProgrammingNormalFormGameAgent(BaseAgent):
     """
     Linear programming agent for normal-form games
@@ -87,15 +88,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=None, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/pi/pi_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/pi/pi_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import math
 from typing import List, Optional, Tuple
 import time
 import os
 import numpy as np
-import gym
+import gymnasium as gym
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
-from csle_agents.agents.base.base_agent import BaseAgent
-import csle_agents.constants.constants as agents_constants
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.tabular_policy import TabularPolicy
+from csle_common.util.general_util import GeneralUtil
+from csle_agents.agents.base.base_agent import BaseAgent
+import csle_agents.constants.constants as agents_constants
 
 
 class PIAgent(BaseAgent):
     """
     Policy Iteration Agent
     """
 
@@ -66,15 +67,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=None, simulation_traces=[],
                 num_cached_traces=0,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/ppo/ppo_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/ppo/ppo_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Union, List, Optional
 import time
-import gym
+
+import gymnasium
+import gymnasium as gym
 import os
 import numpy as np
 import math
 from stable_baselines3 import PPO
 from stable_baselines3.common.vec_env.vec_monitor import VecMonitor
 from stable_baselines3.common.vec_env.dummy_vec_env import DummyVecEnv
 from stable_baselines3.common.env_util import make_vec_env
@@ -20,79 +22,103 @@
 from csle_common.logging.log import Logger
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 from csle_common.dao.training.ppo_policy import PPOPolicy
 from csle_common.dao.simulation_config.state import State
 from csle_common.dao.simulation_config.action import Action
 from csle_common.dao.training.player_type import PlayerType
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
 class PPOAgent(BaseAgent):
     """
     A PPO agent using the implementation from OpenAI baselines
     """
 
     def __init__(self, simulation_env_config: SimulationEnvConfig,
                  emulation_env_config: Union[None, EmulationEnvConfig], experiment_config: ExperimentConfig,
-                 training_job: Optional[TrainingJobConfig] = None):
+                 training_job: Optional[TrainingJobConfig] = None, save_to_metastore: bool = True):
+        """
+        Intializes the agent
+
+        :param simulation_env_config: the simulation environment configuration
+        :param emulation_env_config: the emulation environment configuration
+        :param experiment_config: the experiment configuration
+        :param training_job: the training job
+        :param save_to_metastore: boolean flag indicating whether the results should be saved to the metastore or not
+        """
         super(PPOAgent, self).__init__(simulation_env_config=simulation_env_config,
                                        emulation_env_config=emulation_env_config,
                                        experiment_config=experiment_config)
         assert experiment_config.agent_type == AgentType.PPO
         self.training_job = training_job
+        self.save_to_metastore = save_to_metastore
 
     def train(self) -> ExperimentExecution:
+        """
+        Runs the training process
+
+        :return: the results
+        """
         pid = os.getpid()
 
         # Setup experiment metrics
         exp_result = ExperimentResult()
         exp_result.plot_metrics.append(agents_constants.COMMON.AVERAGE_RETURN)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_RETURN)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON)
         exp_result.plot_metrics.append(agents_constants.COMMON.AVERAGE_TIME_HORIZON)
         exp_result.plot_metrics.append(agents_constants.COMMON.AVERAGE_UPPER_BOUND_RETURN)
         exp_result.plot_metrics.append(agents_constants.COMMON.AVERAGE_RANDOM_RETURN)
+        exp_result.plot_metrics.append(agents_constants.COMMON.AVERAGE_HEURISTIC_RETURN)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNTIME)
         descr = f"Training of policies with PPO using " \
                 f"simulation:{self.simulation_env_config.name}"
 
         # Setup training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
-            training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
+            training_job_id = -1
+            if self.save_to_metastore:
+                training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
             self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
-            MetastoreFacade.update_training_job(training_job=self.training_job, id=self.training_job.id)
+            if self.save_to_metastore:
+                MetastoreFacade.update_training_job(training_job=self.training_job, id=self.training_job.id)
 
         # Setup experiment execution
         ts = time.time()
         emulation_name = None
         if self.emulation_env_config is not None:
             emulation_name = self.emulation_env_config.name
         simulation_name = self.simulation_env_config.name
         self.exp_execution = ExperimentExecution(
             result=exp_result, config=self.experiment_config, timestamp=ts,
             emulation_name=emulation_name, simulation_name=simulation_name, descr=descr,
             log_file_path=self.training_job.log_file_path)
-        exp_execution_id = MetastoreFacade.save_experiment_execution(self.exp_execution)
+        exp_execution_id = -1
+        if self.save_to_metastore:
+            exp_execution_id = MetastoreFacade.save_experiment_execution(self.exp_execution)
         self.exp_execution.id = exp_execution_id
 
         # Setup gym environment
         config = self.simulation_env_config.simulation_env_input_config
-        orig_env = gym.make(self.simulation_env_config.gym_env_name, config=config)
+        orig_env = gymnasium.make(self.simulation_env_config.gym_env_name, config=config)
+        print(orig_env.observation_space)
         env = make_vec_env(env_id=self.simulation_env_config.gym_env_name,
                            n_envs=self.experiment_config.hparams[agents_constants.COMMON.NUM_PARALLEL_ENVS].value,
                            env_kwargs={"config": config}, vec_env_cls=DummyVecEnv)
         env = VecMonitor(env)
 
         # Training runs, one per seed
         for seed in self.experiment_config.random_seeds:
@@ -100,14 +126,15 @@
             exp_result.all_metrics[seed] = {}
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_TIME_HORIZON] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_UPPER_BOUND_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RANDOM_RETURN] = []
+            exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_HEURISTIC_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNTIME] = []
             ExperimentUtil.set_seed(seed)
 
             # Callback for logging training metrics
             cb = PPOTrainingCallback(
                 eval_every=self.experiment_config.hparams[agents_constants.COMMON.EVAL_EVERY].value,
                 eval_batch_size=self.experiment_config.hparams[agents_constants.COMMON.EVAL_BATCH_SIZE].value,
@@ -120,15 +147,15 @@
                     self.simulation_env_config.joint_action_space_config.action_spaces[
                         self.experiment_config.player_idx].actions),
                 save_every=self.experiment_config.hparams[agents_constants.COMMON.SAVE_EVERY].value,
                 save_dir=self.experiment_config.output_dir, exp_execution=self.exp_execution,
                 env=orig_env, experiment_config=self.experiment_config,
                 L=self.experiment_config.hparams[agents_constants.COMMON.L].value,
                 gym_env_name=self.simulation_env_config.gym_env_name,
-                start=self.start
+                start=self.start, save_to_metastore=self.save_to_metastore
             )
 
             # Create PPO Agent
             policy_kwargs = dict(
                 net_arch=[self.experiment_config.hparams[constants.NEURAL_NETWORKS.NUM_NEURONS_PER_HIDDEN_LAYER].value
                           ] * self.experiment_config.hparams[constants.NEURAL_NETWORKS.NUM_HIDDEN_LAYERS].value)
             model = PPO(
@@ -165,19 +192,21 @@
                 actions=self.simulation_env_config.joint_action_space_config.action_spaces[
                     self.experiment_config.player_idx].actions, player_type=self.experiment_config.player_type,
                 experiment_config=self.experiment_config,
                 avg_R=exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN][-1])
             exp_result.policies[seed] = policy
 
             # Save policy metadata
-            MetastoreFacade.save_ppo_policy(ppo_policy=policy)
-            os.chmod(save_path, 0o777)
+            if self.save_to_metastore:
+                MetastoreFacade.save_ppo_policy(ppo_policy=policy)
+                os.chmod(save_path, 0o777)
 
             # Save latest trace
-            MetastoreFacade.save_simulation_trace(orig_env.get_traces()[-1])
+            if self.save_to_metastore:
+                MetastoreFacade.save_simulation_trace(orig_env.get_traces()[-1])
             orig_env.reset_traces()
 
         # Calculate average and std metrics
         exp_result.avg_metrics = {}
         exp_result.std_metrics = {}
         for metric in exp_result.all_metrics[self.experiment_config.random_seeds[0]].keys():
             value_vectors = []
@@ -196,15 +225,15 @@
                 std_metrics.append(ExperimentUtil.mean_confidence_interval(
                     data=seed_values,
                     confidence=self.experiment_config.hparams[agents_constants.COMMON.CONFIDENCE_INTERVAL].value)[1])
             exp_result.avg_metrics[metric] = avg_metrics
             exp_result.std_metrics[metric] = std_metrics
 
         traces = orig_env.get_traces()
-        if len(traces) > 0:
+        if len(traces) > 0 and self.save_to_metastore:
             MetastoreFacade.save_simulation_trace(traces[-1])
         return self.exp_execution
 
     def hparam_names(self) -> List[str]:
         """
         :return: a list with the hyperparameter names
         """
@@ -227,15 +256,15 @@
 
     def __init__(self, exp_result: ExperimentResult, seed: int, random_seeds: List[int],
                  training_job: TrainingJobConfig, exp_execution: ExperimentExecution,
                  max_steps: int, simulation_name: str, start: float,
                  states: List[State], actions: List[Action], player_type: PlayerType,
                  env: gym.Env, experiment_config: ExperimentConfig, verbose=0,
                  eval_every: int = 100, eval_batch_size: int = 10, save_every: int = 10, save_dir: str = "",
-                 L: int = 3, gym_env_name: str = ""):
+                 L: int = 3, gym_env_name: str = "", save_to_metastore: bool = False):
         """
         Initializes the callback
 
         :param exp_result: the experiment result to populate
         :param seed: the random seed
         :param random_seeds: the list of all random seeds
         :param training_job: the training job
@@ -251,14 +280,15 @@
         :param save_every: how frequently to checkpoint the current model
         :param save_dir: the path to checkpoint models
         :param env: the training environment
         :param experiment_config: the experiment configuration
         :param L: num stops if a stopping environment
         :param gym_env_name: name of gym env
         :param start_time: the start time-stamp
+        :param save_to_metastore: boolean flag indicating whether the results should be saved to the metastore
         """
         super(PPOTrainingCallback, self).__init__(verbose)
         self.states = states
         self.simulation_name = simulation_name
         self.iter = 0
         self.eval_every = eval_every
         self.eval_batch_size = eval_batch_size
@@ -273,14 +303,15 @@
         self.save_every = save_every
         self.save_dir = save_dir
         self.env = env
         self.experiment_config = experiment_config
         self.L = L
         self.gym_env_name = gym_env_name
         self.start = start
+        self.save_to_metastore = save_to_metastore
 
     def _on_training_start(self) -> None:
         """
         This method is called before the first rollout starts.
         """
         pass
 
@@ -332,29 +363,30 @@
         if self.iter % self.eval_every == 0:
             if self.player_type == PlayerType.ATTACKER and "stopping" in self.simulation_name:
                 self.env.set_model(self.model)
             policy = PPOPolicy(
                 model=self.model, simulation_name=self.simulation_name, save_path=save_path,
                 states=self.states, player_type=self.player_type, actions=self.actions,
                 experiment_config=self.experiment_config, avg_R=-1)
-            o = self.env.reset()
+            o, _ = self.env.reset()
             max_horizon = self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value
             avg_rewards = []
             avg_horizons = []
             avg_upper_bounds = []
             avg_random_returns = []
+            avg_heuristic_returns = []
             info = {}
             for i in range(self.eval_batch_size):
-                o = self.env.reset()
+                o, _ = self.env.reset()
                 done = False
                 t = 0
                 cumulative_reward = 0
                 while not done and t <= max_horizon:
                     a = policy.action(o=o)
-                    o, r, done, info = self.env.step(a)
+                    o, r, done, _, info = self.env.step(a)
                     cumulative_reward += r * math.pow(
                         self.experiment_config.hparams[agents_constants.COMMON.GAMMA].value, t)
                     t += 1
                     Logger.__call__().get_logger().debug(f"t:{t}, a1:{a}, r:{r}, info:{info}, done:{done}")
                 avg_rewards.append(cumulative_reward)
                 if agents_constants.ENV_METRICS.TIME_HORIZON in info:
                     avg_horizons.append(info[agents_constants.ENV_METRICS.TIME_HORIZON])
@@ -364,29 +396,36 @@
                     avg_upper_bounds.append(info[agents_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN])
                 else:
                     avg_upper_bounds.append(-1)
                 if agents_constants.ENV_METRICS.AVERAGE_RANDOM_RETURN in info:
                     avg_random_returns.append(info[agents_constants.ENV_METRICS.AVERAGE_RANDOM_RETURN])
                 else:
                     avg_random_returns.append(-1)
+                if agents_constants.ENV_METRICS.AVERAGE_HEURISTIC_RETURN in info:
+                    avg_heuristic_returns.append(info[agents_constants.ENV_METRICS.AVERAGE_HEURISTIC_RETURN])
+                else:
+                    avg_heuristic_returns.append(-1)
 
                 avg_upper_bounds.append(info[agents_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN])
             avg_R = np.mean(avg_rewards)
             avg_T = np.mean(avg_horizons)
             avg_random_return = np.mean(avg_random_returns)
+            avg_heuristic_return = np.mean(avg_heuristic_returns)
             avg_upper_bound = np.mean(avg_upper_bounds)
             policy.avg_R = avg_R
-            time_elapsed_minutes = (time.time() - self.start) // 60
+            time_elapsed_minutes = round((time.time() - self.start) / 60, 3)
             self.exp_result.all_metrics[self.seed][agents_constants.COMMON.AVERAGE_RETURN].append(round(avg_R, 3))
             self.exp_result.all_metrics[self.seed][agents_constants.COMMON.AVERAGE_TIME_HORIZON].append(round(avg_T, 3))
             self.exp_result.all_metrics[self.seed][agents_constants.COMMON.AVERAGE_UPPER_BOUND_RETURN].append(
                 round(avg_upper_bound, 3))
             self.exp_result.all_metrics[self.seed][agents_constants.COMMON.RUNTIME].append(time_elapsed_minutes)
             self.exp_result.all_metrics[self.seed][agents_constants.COMMON.AVERAGE_RANDOM_RETURN].append(
                 round(avg_random_return, 3))
+            self.exp_result.all_metrics[self.seed][agents_constants.COMMON.AVERAGE_HEURISTIC_RETURN].append(
+                round(avg_heuristic_return, 3))
             running_avg_J = ExperimentUtil.running_average(
                 self.exp_result.all_metrics[self.seed][agents_constants.COMMON.AVERAGE_RETURN],
                 self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value)
             self.exp_result.all_metrics[self.seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(
                 round(running_avg_J, 3))
             running_avg_T = ExperimentUtil.running_average(
                 self.exp_result.all_metrics[self.seed][agents_constants.COMMON.AVERAGE_TIME_HORIZON],
@@ -395,31 +434,34 @@
                 round(running_avg_T, 3))
             Logger.__call__().get_logger().info(
                 f"[EVAL] Training iteration: {self.iter}, Avg R:{round(avg_R, 3)}, "
                 f"Running_avg_{self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value}_R: "
                 f"{round(running_avg_J, 3)}, Avg T:{round(avg_T, 3)}, "
                 f"Running_avg_{self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value}_T: "
                 f"{round(running_avg_T, 3)}, Avg pi*: {round(avg_upper_bound, 3)}, "
-                f"Avg random R:{round(avg_random_return, 3)}, time elapsed (min): {time_elapsed_minutes}")
+                f"Avg random R:{round(avg_random_return, 3)}, Avg heuristic R:{round(avg_heuristic_return, 3)}, "
+                f"time elapsed (min): {time_elapsed_minutes}")
 
             self.env.reset()
 
             # Update training job
             total_steps_done = len(self.random_seeds) * self.max_steps
             steps_done = (self.random_seeds.index(self.seed)) * self.max_steps + self.num_timesteps
             progress = round(steps_done / total_steps_done, 2)
             self.training_job.progress_percentage = progress
             self.training_job.experiment_result = self.exp_result
             if len(self.env.get_traces()) > 0:
                 self.training_job.simulation_traces.append(self.env.get_traces()[-1])
             if len(self.training_job.simulation_traces) > self.training_job.num_cached_traces:
                 self.training_job.simulation_traces = self.training_job.simulation_traces[1:]
-            MetastoreFacade.update_training_job(training_job=self.training_job, id=self.training_job.id)
+            if self.save_to_metastore:
+                MetastoreFacade.update_training_job(training_job=self.training_job, id=self.training_job.id)
 
             # Update execution
             ts = time.time()
             self.exp_execution.timestamp = ts
             self.exp_execution.result = self.exp_result
-            MetastoreFacade.update_experiment_execution(experiment_execution=self.exp_execution,
-                                                        id=self.exp_execution.id)
+            if self.save_to_metastore:
+                MetastoreFacade.update_experiment_execution(experiment_execution=self.exp_execution,
+                                                            id=self.exp_execution.id)
 
         self.iter += 1
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/q_learning/q_learning_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/q_learning/q_learning_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import math
 from typing import List, Optional, Tuple
 import time
 import os
 import numpy as np
-import gym
+import gymnasium as gym
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.tabular_policy import TabularPolicy
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
 class QLearningAgent(BaseAgent):
     """
     Q-learning Agent
@@ -67,15 +68,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=None, simulation_traces=[],
                 num_cached_traces=0,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/random_search/random_search_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/reinforce/reinforce_agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,108 @@
 import math
 from typing import Union, List, Dict, Optional
 import time
-import gym
+import gymnasium as gym
 import os
+import torch
 import numpy as np
 import gym_csle_stopping_game.constants.constants as env_constants
+import csle_common.constants.constants as constants
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
-from csle_common.dao.training.player_type import PlayerType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
-from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
+from csle_common.dao.training.fnn_with_softmax_policy import FNNWithSoftmaxPolicy
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
+from csle_common.models.fnn_w_softmax import FNNwithSoftmax
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
-class RandomSearchAgent(BaseAgent):
+class ReinforceAgent(BaseAgent):
     """
-    Random Search Agent
+    Reinforce Agent
     """
 
     def __init__(self, simulation_env_config: SimulationEnvConfig,
                  emulation_env_config: Union[None, EmulationEnvConfig],
                  experiment_config: ExperimentConfig, env: Optional[gym.Env] = None,
                  training_job: Optional[TrainingJobConfig] = None, save_to_metastore: bool = True):
         """
-        Initializes the Random Search Agent
+        Initializes the Reinforce Agent
 
         :param simulation_env_config: the simulation env config
         :param emulation_env_config: the emulation env config
         :param experiment_config: the experiment config
         :param env: (optional) the gym environment to use for simulation
         :param training_job: (optional) a training job configuration
         :param save_to_metastore: boolean flag that can be set to avoid saving results and progress to the metastore
         """
         super().__init__(simulation_env_config=simulation_env_config, emulation_env_config=emulation_env_config,
                          experiment_config=experiment_config)
-        assert experiment_config.agent_type == AgentType.RANDOM_SEARCH
+        assert experiment_config.agent_type == AgentType.REINFORCE
         self.env = env
         self.training_job = training_job
         self.save_to_metastore = save_to_metastore
+        self.machine_eps = np.finfo(np.float32).eps.item()
 
     def train(self) -> ExperimentExecution:
         """
-        Performs the policy training for the given random seeds using random search
+        Performs the policy training for the given random seeds using reinforce
 
         :return: the training metrics and the trained policies
         """
         pid = os.getpid()
 
         # Initialize metrics
         exp_result = ExperimentResult()
         exp_result.plot_metrics.append(agents_constants.COMMON.AVERAGE_RETURN)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_RETURN)
+        exp_result.plot_metrics.append(agents_constants.COMMON.POLICY_LOSSES)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.INTRUSION_LENGTH)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.INTRUSION_START)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_START)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.TIME_HORIZON)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN)
         exp_result.plot_metrics.append(env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN)
-        for l in range(1, self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value + 1):
-            exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
-            exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_running_average_{l}")
 
         descr = f"Training of policies with the random search algorithm using " \
                 f"simulation:{self.simulation_env_config.name}"
         for seed in self.experiment_config.random_seeds:
             exp_result.all_metrics[seed] = {}
-            exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.THETAS] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN] = []
-            exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.THRESHOLDS] = []
-            if self.experiment_config.player_type == PlayerType.DEFENDER:
-                for l in range(1, self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value + 1):
-                    exp_result.all_metrics[seed][
-                        agents_constants.RANDOM_SEARCH.STOP_DISTRIBUTION_DEFENDER + f"_l={l}"] = []
-            else:
-                for s in self.simulation_env_config.state_space_config.states:
-                    for l in range(1, self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value + 1):
-                        exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.STOP_DISTRIBUTION_ATTACKER
-                                                     + f"_l={l}_s={s.id}"] = []
+            exp_result.all_metrics[seed][agents_constants.COMMON.POLICY_LOSSES] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_START] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_START] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON] = []
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = []
             exp_result.all_metrics[seed][
                 env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN] = []
-            for l in range(1, self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value + 1):
-                exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"] = []
-                exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_running_average_{l}"] = []
 
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
@@ -121,28 +111,28 @@
 
         # Initialize execution result
         ts = time.time()
         emulation_name = None
         if self.emulation_env_config is not None:
             emulation_name = self.emulation_env_config.name
         simulation_name = self.simulation_env_config.name
-        self.exp_execution = ExperimentExecution(
-            result=exp_result, config=self.experiment_config, timestamp=ts, emulation_name=emulation_name,
-            simulation_name=simulation_name, descr=descr, log_file_path=self.training_job.log_file_path)
+        self.exp_execution = ExperimentExecution(result=exp_result, config=self.experiment_config, timestamp=ts,
+                                                 emulation_name=emulation_name, simulation_name=simulation_name,
+                                                 descr=descr, log_file_path=self.training_job.log_file_path)
         if self.save_to_metastore:
             exp_execution_id = MetastoreFacade.save_experiment_execution(self.exp_execution)
             self.exp_execution.id = exp_execution_id
 
         config = self.simulation_env_config.simulation_env_input_config
         if self.env is None:
             self.env = gym.make(self.simulation_env_config.gym_env_name, config=config)
         for seed in self.experiment_config.random_seeds:
             ExperimentUtil.set_seed(seed)
-            exp_result = self.random_search(exp_result=exp_result, seed=seed, training_job=self.training_job,
-                                            random_seeds=self.experiment_config.random_seeds)
+            exp_result = self.reinforce(exp_result=exp_result, seed=seed, training_job=self.training_job,
+                                        random_seeds=self.experiment_config.random_seeds)
 
             # Save latest trace
             if self.save_to_metastore:
                 MetastoreFacade.save_simulation_trace(self.env.get_traces()[-1])
             self.env.reset_traces()
 
         # Calculate average and std metrics
@@ -190,111 +180,129 @@
                                                         id=self.exp_execution.id)
         return self.exp_execution
 
     def hparam_names(self) -> List[str]:
         """
         :return: a list with the hyperparameter names
         """
-        return [agents_constants.RANDOM_SEARCH.N, agents_constants.RANDOM_SEARCH.DELTA,
-                agents_constants.RANDOM_SEARCH.L, agents_constants.RANDOM_SEARCH.THETA1,
-                agents_constants.COMMON.EVAL_BATCH_SIZE,
+        return [agents_constants.REINFORCE.N, agents_constants.COMMON.EVAL_BATCH_SIZE,
                 agents_constants.COMMON.CONFIDENCE_INTERVAL,
-                agents_constants.COMMON.RUNNING_AVERAGE]
+                agents_constants.COMMON.RUNNING_AVERAGE,
+                agents_constants.COMMON.LEARNING_RATE_DECAY_RATE, agents_constants.COMMON.LEARNING_RATE_EXP_DECAY,
+                constants.NEURAL_NETWORKS.NUM_HIDDEN_LAYERS, constants.NEURAL_NETWORKS.NUM_NEURONS_PER_HIDDEN_LAYER,
+                constants.NEURAL_NETWORKS.ACTIVATION_FUNCTION, agents_constants.COMMON.OPTIMIZER]
 
-    def random_search(self, exp_result: ExperimentResult, seed: int,
-                      training_job: TrainingJobConfig, random_seeds: List[int]) -> ExperimentResult:
+    def reinforce(self, exp_result: ExperimentResult, seed: int,
+                  training_job: TrainingJobConfig, random_seeds: List[int]) -> ExperimentResult:
         """
         Runs the random search algorithm
 
         :param exp_result: the experiment result object to store the result
         :param seed: the seed
         :param training_job: the training job config
         :param random_seeds: list of seeds
         :return: the updated experiment result and the trained policy
         """
-        L = self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value
-        if agents_constants.RANDOM_SEARCH.THETA1 in self.experiment_config.hparams:
-            theta = self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.THETA1].value
-        else:
-            if self.experiment_config.player_type == PlayerType.DEFENDER:
-                theta = RandomSearchAgent.initial_theta(L=L)
-            else:
-                theta = RandomSearchAgent.initial_theta(L=2 * L)
-
-        # Initial eval
-        policy = MultiThresholdStoppingPolicy(
-            theta=list(theta), simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.RANDOM_SEARCH)
-        avg_metrics = self.eval_theta(
-            policy=policy, max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
-        J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
-        policy.avg_R = J
-        exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
-        exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(J)
-        exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.THETAS].append(RandomSearchAgent.round_vec(theta))
-
         # Hyperparameters
-        N = self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.N].value
-        delta = self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.DELTA].value
+        N = self.experiment_config.hparams[agents_constants.REINFORCE.N].value
 
-        # Initial eval
-        policy = MultiThresholdStoppingPolicy(
-            theta=list(theta), simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.RANDOM_SEARCH)
-        avg_metrics = self.eval_theta(
-            policy=policy, max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
-        J_0 = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
+        # Setup policy network
+        policy_network = FNNwithSoftmax(
+            input_dim=self.env.observation_space.shape[0],
+            output_dim=self.env.action_space.n,
+            hidden_dim=self.experiment_config.hparams[constants.NEURAL_NETWORKS.NUM_NEURONS_PER_HIDDEN_LAYER].value,
+            num_hidden_layers=self.experiment_config.hparams[constants.NEURAL_NETWORKS.NUM_HIDDEN_LAYERS].value,
+            hidden_activation=self.experiment_config.hparams[constants.NEURAL_NETWORKS.ACTIVATION_FUNCTION].value
+        )
+
+        # Setup device
+        policy_network.to(torch.device(self.experiment_config.hparams[constants.NEURAL_NETWORKS.DEVICE].value))
+
+        # Setup optimizer
+        if self.experiment_config.hparams[agents_constants.COMMON.OPTIMIZER].value == agents_constants.COMMON.ADAM:
+            optimizer = torch.optim.Adam(
+                policy_network.parameters(),
+                lr=self.experiment_config.hparams[agents_constants.COMMON.LEARNING_RATE].value)
+        elif self.experiment_config.hparams[agents_constants.COMMON.OPTIMIZER].value == agents_constants.COMMON.SGD:
+            optimizer = torch.optim.SGD(
+                policy_network.parameters(),
+                lr=self.experiment_config.hparams[agents_constants.COMMON.LEARNING_RATE].value)
+        else:
+            raise ValueError(f"Optimizer: {self.experiment_config.hparams[agents_constants.COMMON.OPTIMIZER].value}"
+                             f" not recognized")
 
-        for i in range(N):
+        # Setup LR decay
+        # if self.experiment_config.hparams[agents_constants.COMMON.LEARNING_RATE_EXP_DECAY].value:
+        #     lr_decay = torch.optim.lr_scheduler.ExponentialLR(
+        #         optimizer=optimizer,
+        #         gamma=self.experiment_config.hparams[agents_constants.COMMON.LEARNING_RATE_DECAY_RATE].value)
 
-            theta_candidate = self.random_perturbation(delta=delta, theta=theta)
-            candidate_policy = MultiThresholdStoppingPolicy(
-                theta=list(theta_candidate), simulation_name=self.simulation_env_config.name,
+        for i in range(N):
+            rewards_batch = []
+            log_probs_batch = []
+            metrics = {}
+            ts = time.time()
+            save_path = f"{self.experiment_config.output_dir}/ppo_policy_seed_{seed}_{ts}.zip"
+            policy = FNNWithSoftmaxPolicy(
+                policy_network=policy_network, simulation_name=self.simulation_env_config.name,
+                save_path=save_path,
                 states=self.simulation_env_config.state_space_config.states,
-                player_type=self.experiment_config.player_type, L=L,
                 actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                    self.experiment_config.player_idx].actions,
-                experiment_config=self.experiment_config, avg_R=-1,
-                agent_type=AgentType.RANDOM_SEARCH)
-            avg_metrics = self.eval_theta(
-                policy=candidate_policy,
-                max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
-            J_candidate = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
-            if J_candidate > J_0:
-                theta = theta_candidate
-                J_0 = J_candidate
-                policy = candidate_policy
+                    self.experiment_config.player_idx].actions, player_type=self.experiment_config.player_type,
+                experiment_config=self.experiment_config,
+                avg_R=-1, input_dim=policy_network.input_dim, output_dim=policy_network.output_dim)
+            policy.save_policy_network()
+
+            # Run a batch of rollouts
+            for j in range(self.experiment_config.hparams[agents_constants.REINFORCE.GRADIENT_BATCH_SIZE].value):
+                cumulative_reward = 0.0
+                rewards = []
+                log_probs = []
+                done = False
+                o = self.env.reset()
+                while not done:
+                    # get action
+                    action, log_prob = policy.get_action_and_log_prob(state=o)
+
+                    # Take a step in the environment
+                    o_prime, reward, done, info = self.env.step(action)
+
+                    # Update metrics
+                    cumulative_reward += reward
+                    rewards.append(cumulative_reward)
+                    log_probs.append(log_prob)
+
+                    # Move to the next state
+                    o = o_prime
+
+                # Accumulate batch
+                rewards_batch.append(rewards)
+                log_probs_batch.append(log_probs)
+
+                metrics = ReinforceAgent.update_metrics(metrics=metrics, info=info)
+
+            avg_metrics = ReinforceAgent.compute_avg_metrics(metrics=metrics)
+
+            # Perform Batch Policy Gradient updates
+            loss = self.training_step(saved_rewards=rewards_batch, saved_log_probs=log_probs_batch,
+                                      policy_network=policy_network,
+                                      optimizer=optimizer,
+                                      gamma=self.experiment_config.hparams[agents_constants.COMMON.GAMMA].value)
+            loss = loss.item()
 
-            # Log average return
-            J = J_0
+            # Log metrics
+            J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
             policy.avg_R = J
+            exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
+            exp_result.all_metrics[seed][agents_constants.COMMON.POLICY_LOSSES].append(loss)
             running_avg_J = ExperimentUtil.running_average(
                 exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN],
                 self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value)
-            exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(running_avg_J)
 
-            # Log thresholds
-            exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.THETAS].append(
-                RandomSearchAgent.round_vec(theta))
-            exp_result.all_metrics[seed][agents_constants.RANDOM_SEARCH.THRESHOLDS].append(
-                RandomSearchAgent.round_vec(policy.thresholds()))
-
-            # Log stop distribution
-            for k, v in policy.stop_distributions().items():
-                exp_result.all_metrics[seed][k].append(v)
-
             # Log intrusion lengths
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH].append(
                 round(avg_metrics[env_constants.ENV_METRICS.INTRUSION_LENGTH], 3))
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH].append(
                 ExperimentUtil.running_average(
                     exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH],
                     self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
@@ -308,22 +316,14 @@
                     self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON].append(
                 round(avg_metrics[env_constants.ENV_METRICS.TIME_HORIZON], 3))
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON].append(
                 ExperimentUtil.running_average(
                     exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON],
                     self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
-            for l in range(1, self.experiment_config.hparams[agents_constants.RANDOM_SEARCH.L].value + 1):
-                exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
-                exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"].append(
-                    round(avg_metrics[env_constants.ENV_METRICS.STOP + f"_{l}"], 3))
-                exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_running_average_{l}"].append(
-                    ExperimentUtil.running_average(
-                        exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"],
-                        self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
 
             # Log baseline returns
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN].append(
                 round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN], 3))
             exp_result.all_metrics[seed][
                 env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN].append(
                 round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN], 3))
@@ -347,82 +347,40 @@
                 self.exp_execution.timestamp = ts
                 self.exp_execution.result = exp_result
                 if self.save_to_metastore:
                     MetastoreFacade.update_experiment_execution(experiment_execution=self.exp_execution,
                                                                 id=self.exp_execution.id)
 
                 Logger.__call__().get_logger().info(
-                    f"[RANDOM-SEARCH] i: {i}, J:{J}, "
+                    f"[REINFORCE] i: {i}, J:{J}, "
                     f"J_avg_{self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value}:"
                     f"{running_avg_J}, "
                     f"opt_J:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN][-1]}, "
                     f"int_len:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH][-1]}, "
-                    f"sigmoid(theta):{policy.thresholds()}, progress: {round(progress*100,2)}%, "
-                    f"stop distributions:{policy.stop_distributions()}")
+                    f"progress: {round(progress*100,2)}%")
 
-        policy = MultiThresholdStoppingPolicy(
-            theta=list(theta), simulation_name=self.simulation_env_config.name,
+        ts = time.time()
+        save_path = f"{self.experiment_config.output_dir}/ppo_policy_seed_{seed}_{ts}.zip"
+        policy = FNNWithSoftmaxPolicy(
+            policy_network=policy_network, simulation_name=self.simulation_env_config.name,
+            save_path=save_path,
             states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
             actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=J,
-            agent_type=AgentType.RANDOM_SEARCH)
+                self.experiment_config.player_idx].actions, player_type=self.experiment_config.player_type,
+            experiment_config=self.experiment_config,
+            avg_R=exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN][-1],
+            input_dim=policy_network.input_dim, output_dim=policy_network.output_dim)
+        policy.save_policy_network()
+
         exp_result.policies[seed] = policy
         # Save policy
         if self.save_to_metastore:
-            MetastoreFacade.save_multi_threshold_stopping_policy(multi_threshold_stopping_policy=policy)
+            MetastoreFacade.save_fnn_w_softmax_policy(fnn_w_softmax_policy=policy)
         return exp_result
 
-    def eval_theta(self, policy: MultiThresholdStoppingPolicy, max_steps: int = 200) -> Dict[str, Union[float, int]]:
-        """
-        Evaluates a given threshold policy by running monte-carlo simulations
-
-        :param policy: the policy to evaluate
-        :return: the average metrics of the evaluation
-        """
-        eval_batch_size = self.experiment_config.hparams[agents_constants.COMMON.EVAL_BATCH_SIZE].value
-        metrics = {}
-        for j in range(eval_batch_size):
-            done = False
-            o = self.env.reset()
-            l = int(o[0])
-            b1 = o[1]
-            t = 1
-            r = 0
-            a = 0
-            info = {}
-            while not done and t <= max_steps:
-                Logger.__call__().get_logger().debug(f"t:{t}, a: {a}, b1:{b1}, r:{r}, l:{l}, info:{info}")
-                if self.experiment_config.player_type == PlayerType.ATTACKER:
-                    policy.opponent_strategy = self.env.static_defender_strategy
-                    a = policy.action(o=o)
-                else:
-                    a = policy.action(o=o)
-                o, r, done, info = self.env.step(a)
-                l = int(o[0])
-                b1 = o[1]
-                t += 1
-            metrics = RandomSearchAgent.update_metrics(metrics=metrics, info=info)
-        avg_metrics = RandomSearchAgent.compute_avg_metrics(metrics=metrics)
-        return avg_metrics
-
-    def random_perturbation(self, delta: float, theta: np.ndarray) -> np.ndarray:
-        """
-        Performs a random perturbation to the theta vector
-
-        :param delta: the step size for the perturbation
-        :param theta: the current theta vector
-        :return: the perturbed theta vector
-        """
-        perturbed_theta = []
-        for l in range(len(theta)):
-            Delta = np.random.uniform(-delta, delta)
-            perturbed_theta.append(theta[l] + Delta)
-        return np.array(perturbed_theta)
-
     @staticmethod
     def update_metrics(metrics: Dict[str, List[Union[float, int]]], info: Dict[str, Union[float, int]]) \
             -> Dict[str, List[Union[float, int]]]:
         """
         Update a dict with aggregated metrics using new information from the environment
 
         :param metrics: the dict with the aggregated metrics
@@ -447,29 +405,71 @@
         avg_metrics = {}
         for k, v in metrics.items():
             avg = round(sum(v) / len(v), 2)
             avg_metrics[k] = avg
         return avg_metrics
 
     @staticmethod
-    def initial_theta(L: int) -> np.ndarray:
-        """
-        Initializes theta randomly
-
-        :param L: the dimension of theta
-        :return: the initialized theta vector
-        """
-        theta_1 = []
-        for k in range(L):
-            theta_1.append(np.random.uniform(-3, 3))
-        theta_1 = np.array(theta_1)
-        return theta_1
-
-    @staticmethod
     def round_vec(vec) -> List[float]:
         """
         Rounds a vector to 3 decimals
 
         :param vec: the vector to round
         :return: the rounded vector
         """
         return list(map(lambda x: round(x, 3), vec))
+
+    def training_step(self, saved_rewards: List[List[float]], saved_log_probs: List[List[torch.Tensor]],
+                      policy_network: FNNwithSoftmax, optimizer: torch.optim.Optimizer, gamma: float) -> torch.Tensor:
+        """
+        Performs a training step of the REINFORCE algorithm
+
+        :param saved_rewards: list of rewards encountered in the latest episode trajectory
+        :param saved_log_probs: list of log-action probabilities (log p(a|s)) encountered in the latest
+                                episode trajectory
+        :param policy_network: the policy network
+        :param optimizer: the optimizer for updating the weights
+        :param gamma: the discount factor
+        :return: loss
+        """
+        policy_loss = []
+        num_batches = len(saved_rewards)
+
+        for batch in range(num_batches):
+            R = 0
+            returns = []
+
+            # Create discounted returns. When episode is finished we can go back and compute the observed cumulative
+            # discounted reward by using the observed rewards
+            for r in saved_rewards[batch][::-1]:
+                R = r + gamma * R
+                returns.insert(0, R)
+            num_rewards = len(returns)
+
+            # convert list to torch tensor
+            returns = torch.tensor(returns)
+
+            # normalize
+            std = returns.std()
+            if num_rewards < 2:
+                std = 0
+            returns = (returns - returns.mean()) / (std + self.machine_eps)
+
+            # Compute PG "loss" which in reality is the expected reward, which we want to maximize with gradient ascent
+            for log_prob, R in zip(saved_log_probs[batch], returns):
+                # negative log prob since we are doing gradient descent (not ascent)
+                policy_loss.append(-log_prob * R)
+
+        # Compute gradient and update models
+        # reset gradients
+        optimizer.zero_grad()
+        # expected loss over the batch
+        policy_loss_total = torch.stack(policy_loss).sum()
+        policy_loss = policy_loss_total / num_batches
+        # perform backprop
+        policy_loss.backward()
+        # maybe clip gradient
+        if self.experiment_config.hparams[constants.NEURAL_NETWORKS.DEVICE].value:
+            torch.nn.utils.clip_grad_norm_(policy_network.parameters(), 1)
+        # gradient descent step
+        optimizer.step()
+        return policy_loss
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/reinforce/reinforce_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,106 +1,88 @@
 import math
-from typing import Union, List, Dict, Optional
+from typing import List, Optional, Tuple
 import time
-import gym
 import os
-import torch
 import numpy as np
-import gym_csle_stopping_game.constants.constants as env_constants
-import csle_common.constants.constants as constants
-from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
+import gymnasium as gym
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
-from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
-from csle_common.dao.training.fnn_with_softmax_policy import FNNWithSoftmaxPolicy
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
+from csle_common.dao.training.experiment_execution import ExperimentExecution
+from csle_common.dao.training.alpha_vectors_policy import AlphaVectorsPolicy
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
-from csle_common.models.fnn_w_softmax import FNNwithSoftmax
+from scipy.optimize import linprog
+from itertools import product
 
 
-class ReinforceAgent(BaseAgent):
+class SondikVIAgent(BaseAgent):
     """
-    Reinforce Agent
+    Sondik's value iteration for POMDPs (Sondik 1971)
     """
 
     def __init__(self, simulation_env_config: SimulationEnvConfig,
-                 emulation_env_config: Union[None, EmulationEnvConfig],
-                 experiment_config: ExperimentConfig, env: Optional[gym.Env] = None,
+                 experiment_config: ExperimentConfig,
                  training_job: Optional[TrainingJobConfig] = None, save_to_metastore: bool = True):
         """
-        Initializes the Reinforce Agent
+        Initializes the Sondik-VI agent
 
-        :param simulation_env_config: the simulation env config
-        :param emulation_env_config: the emulation env config
-        :param experiment_config: the experiment config
-        :param env: (optional) the gym environment to use for simulation
-        :param training_job: (optional) a training job configuration
-        :param save_to_metastore: boolean flag that can be set to avoid saving results and progress to the metastore
+        :param simulation_env_config: configuration of the simulation environment
+        :param experiment_config: the experiment configuration
+        :param training_job: an existing training job to use (optional)
+        :param save_to_metastore: boolean flag whether to save the execution to the metastore
         """
-        super().__init__(simulation_env_config=simulation_env_config, emulation_env_config=emulation_env_config,
+        super().__init__(simulation_env_config=simulation_env_config, emulation_env_config=None,
                          experiment_config=experiment_config)
-        assert experiment_config.agent_type == AgentType.REINFORCE
-        self.env = env
+        assert experiment_config.agent_type == AgentType.SONDIK_VALUE_ITERATION
         self.training_job = training_job
         self.save_to_metastore = save_to_metastore
-        self.machine_eps = np.finfo(np.float32).eps.item()
+        self.env = gym.make(self.simulation_env_config.gym_env_name,
+                            config=self.simulation_env_config.simulation_env_input_config)
 
     def train(self) -> ExperimentExecution:
         """
-        Performs the policy training for the given random seeds using reinforce
+        Runs the value iteration algorithm to compute V*
 
-        :return: the training metrics and the trained policies
+        :return: the results
         """
         pid = os.getpid()
 
         # Initialize metrics
         exp_result = ExperimentResult()
         exp_result.plot_metrics.append(agents_constants.COMMON.AVERAGE_RETURN)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_RETURN)
-        exp_result.plot_metrics.append(agents_constants.COMMON.POLICY_LOSSES)
-        exp_result.plot_metrics.append(env_constants.ENV_METRICS.INTRUSION_LENGTH)
-        exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH)
-        exp_result.plot_metrics.append(env_constants.ENV_METRICS.INTRUSION_START)
-        exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_START)
-        exp_result.plot_metrics.append(env_constants.ENV_METRICS.TIME_HORIZON)
-        exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON)
-        exp_result.plot_metrics.append(env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN)
-        exp_result.plot_metrics.append(env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN)
+        exp_result.plot_metrics.append(agents_constants.SONDIK_VI.INITIAL_BELIEF_VALUES)
+        exp_result.plot_metrics.append(agents_constants.SONDIK_VI.NUM_ALPHA_VECTORS)
 
-        descr = f"Training of policies with the random search algorithm using " \
+        descr = f"Computation of V* with the Sondik value algorithm using " \
                 f"simulation:{self.simulation_env_config.name}"
+
         for seed in self.experiment_config.random_seeds:
             exp_result.all_metrics[seed] = {}
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN] = []
-            exp_result.all_metrics[seed][agents_constants.COMMON.POLICY_LOSSES] = []
-            exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_START] = []
-            exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON] = []
-            exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH] = []
-            exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_START] = []
-            exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH] = []
-            exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON] = []
-            exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN] = []
-            exp_result.all_metrics[seed][
-                env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN] = []
+            exp_result.all_metrics[seed][agents_constants.SONDIK_VI.NUM_ALPHA_VECTORS] = []
+            exp_result.all_metrics[seed][agents_constants.SONDIK_VI.INITIAL_BELIEF_VALUES] = []
 
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
-                emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
-                num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                emulation_env_name=None, simulation_traces=[],
+                num_cached_traces=0,
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
@@ -116,26 +98,17 @@
         self.exp_execution = ExperimentExecution(result=exp_result, config=self.experiment_config, timestamp=ts,
                                                  emulation_name=emulation_name, simulation_name=simulation_name,
                                                  descr=descr, log_file_path=self.training_job.log_file_path)
         if self.save_to_metastore:
             exp_execution_id = MetastoreFacade.save_experiment_execution(self.exp_execution)
             self.exp_execution.id = exp_execution_id
 
-        config = self.simulation_env_config.simulation_env_input_config
-        if self.env is None:
-            self.env = gym.make(self.simulation_env_config.gym_env_name, config=config)
         for seed in self.experiment_config.random_seeds:
             ExperimentUtil.set_seed(seed)
-            exp_result = self.reinforce(exp_result=exp_result, seed=seed, training_job=self.training_job,
-                                        random_seeds=self.experiment_config.random_seeds)
-
-            # Save latest trace
-            if self.save_to_metastore:
-                MetastoreFacade.save_simulation_trace(self.env.get_traces()[-1])
-            self.env.reset_traces()
+            exp_result = self.sondik_vi_algorithm(exp_result=exp_result, seed=seed)
 
         # Calculate average and std metrics
         exp_result.avg_metrics = {}
         exp_result.std_metrics = {}
         for metric in exp_result.all_metrics[self.experiment_config.random_seeds[0]].keys():
             value_vectors = []
             for seed in self.experiment_config.random_seeds:
@@ -163,311 +136,303 @@
                         std_metrics.append(-1)
                 else:
                     avg_metrics.append(-1)
                     std_metrics.append(-1)
                 exp_result.avg_metrics[metric] = avg_metrics
                 exp_result.std_metrics[metric] = std_metrics
 
-        traces = self.env.get_traces()
-        if len(traces) > 0 and self.save_to_metastore:
-            MetastoreFacade.save_simulation_trace(traces[-1])
-        ts = time.time()
+                ts = time.time()
         self.exp_execution.timestamp = ts
         self.exp_execution.result = exp_result
+        self.training_job.experiment_result = exp_result
         if self.save_to_metastore:
             MetastoreFacade.update_experiment_execution(experiment_execution=self.exp_execution,
                                                         id=self.exp_execution.id)
+            MetastoreFacade.update_training_job(training_job=self.training_job, id=self.training_job.id)
         return self.exp_execution
 
     def hparam_names(self) -> List[str]:
         """
         :return: a list with the hyperparameter names
         """
-        return [agents_constants.REINFORCE.N, agents_constants.COMMON.EVAL_BATCH_SIZE,
-                agents_constants.COMMON.CONFIDENCE_INTERVAL,
-                agents_constants.COMMON.RUNNING_AVERAGE,
-                agents_constants.COMMON.LEARNING_RATE_DECAY_RATE, agents_constants.COMMON.LEARNING_RATE_EXP_DECAY,
-                constants.NEURAL_NETWORKS.NUM_HIDDEN_LAYERS, constants.NEURAL_NETWORKS.NUM_NEURONS_PER_HIDDEN_LAYER,
-                constants.NEURAL_NETWORKS.ACTIVATION_FUNCTION, agents_constants.COMMON.OPTIMIZER]
-
-    def reinforce(self, exp_result: ExperimentResult, seed: int,
-                  training_job: TrainingJobConfig, random_seeds: List[int]) -> ExperimentResult:
-        """
-        Runs the random search algorithm
-
-        :param exp_result: the experiment result object to store the result
-        :param seed: the seed
-        :param training_job: the training job config
-        :param random_seeds: list of seeds
-        :return: the updated experiment result and the trained policy
-        """
-        # Hyperparameters
-        N = self.experiment_config.hparams[agents_constants.REINFORCE.N].value
-
-        # Setup policy network
-        policy_network = FNNwithSoftmax(
-            input_dim=self.env.observation_space.shape[0],
-            output_dim=self.env.action_space.n,
-            hidden_dim=self.experiment_config.hparams[constants.NEURAL_NETWORKS.NUM_NEURONS_PER_HIDDEN_LAYER].value,
-            num_hidden_layers=self.experiment_config.hparams[constants.NEURAL_NETWORKS.NUM_HIDDEN_LAYERS].value,
-            hidden_activation=self.experiment_config.hparams[constants.NEURAL_NETWORKS.ACTIVATION_FUNCTION].value
-        )
-
-        # Setup device
-        policy_network.to(torch.device(self.experiment_config.hparams[constants.NEURAL_NETWORKS.DEVICE].value))
-
-        # Setup optimizer
-        if self.experiment_config.hparams[agents_constants.COMMON.OPTIMIZER].value == agents_constants.COMMON.ADAM:
-            optimizer = torch.optim.Adam(
-                policy_network.parameters(),
-                lr=self.experiment_config.hparams[agents_constants.COMMON.LEARNING_RATE].value)
-        elif self.experiment_config.hparams[agents_constants.COMMON.OPTIMIZER].value == agents_constants.COMMON.SGD:
-            optimizer = torch.optim.SGD(
-                policy_network.parameters(),
-                lr=self.experiment_config.hparams[agents_constants.COMMON.LEARNING_RATE].value)
-        else:
-            raise ValueError(f"Optimizer: {self.experiment_config.hparams[agents_constants.COMMON.OPTIMIZER].value}"
-                             f" not recognized")
-
-        # Setup LR decay
-        # if self.experiment_config.hparams[agents_constants.COMMON.LEARNING_RATE_EXP_DECAY].value:
-        #     lr_decay = torch.optim.lr_scheduler.ExponentialLR(
-        #         optimizer=optimizer,
-        #         gamma=self.experiment_config.hparams[agents_constants.COMMON.LEARNING_RATE_DECAY_RATE].value)
-
-        for i in range(N):
-            rewards_batch = []
-            log_probs_batch = []
-            metrics = {}
-            ts = time.time()
-            save_path = f"{self.experiment_config.output_dir}/ppo_policy_seed_{seed}_{ts}.zip"
-            policy = FNNWithSoftmaxPolicy(
-                policy_network=policy_network, simulation_name=self.simulation_env_config.name,
-                save_path=save_path,
-                states=self.simulation_env_config.state_space_config.states,
-                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                    self.experiment_config.player_idx].actions, player_type=self.experiment_config.player_type,
-                experiment_config=self.experiment_config,
-                avg_R=-1, input_dim=policy_network.input_dim, output_dim=policy_network.output_dim)
-            policy.save_policy_network()
-
-            # Run a batch of rollouts
-            for j in range(self.experiment_config.hparams[agents_constants.REINFORCE.GRADIENT_BATCH_SIZE].value):
-                cumulative_reward = 0.0
-                rewards = []
-                log_probs = []
-                done = False
-                o = self.env.reset()
-                while not done:
-                    # get action
-                    action, log_prob = policy.get_action_and_log_prob(state=o)
-
-                    # Take a step in the environment
-                    o_prime, reward, done, info = self.env.step(action)
-
-                    # Update metrics
-                    cumulative_reward += reward
-                    rewards.append(cumulative_reward)
-                    log_probs.append(log_prob)
-
-                    # Move to the next state
-                    o = o_prime
-
-                # Accumulate batch
-                rewards_batch.append(rewards)
-                log_probs_batch.append(log_probs)
-
-                metrics = ReinforceAgent.update_metrics(metrics=metrics, info=info)
-
-            avg_metrics = ReinforceAgent.compute_avg_metrics(metrics=metrics)
-
-            # Perform Batch Policy Gradient updates
-            loss = self.training_step(saved_rewards=rewards_batch, saved_log_probs=log_probs_batch,
-                                      policy_network=policy_network,
-                                      optimizer=optimizer,
-                                      gamma=self.experiment_config.hparams[agents_constants.COMMON.GAMMA].value)
-            loss = loss.item()
-
-            # Log metrics
-            J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
-            policy.avg_R = J
-            exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
-            exp_result.all_metrics[seed][agents_constants.COMMON.POLICY_LOSSES].append(loss)
-            running_avg_J = ExperimentUtil.running_average(
-                exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN],
-                self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value)
-            exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(running_avg_J)
-
-            # Log intrusion lengths
-            exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH].append(
-                round(avg_metrics[env_constants.ENV_METRICS.INTRUSION_LENGTH], 3))
-            exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH].append(
-                ExperimentUtil.running_average(
-                    exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH],
-                    self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
-
-            # Log stopping times
-            exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_START].append(
-                round(avg_metrics[env_constants.ENV_METRICS.INTRUSION_START], 3))
-            exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_START].append(
-                ExperimentUtil.running_average(
-                    exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_START],
-                    self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
-            exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON].append(
-                round(avg_metrics[env_constants.ENV_METRICS.TIME_HORIZON], 3))
-            exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON].append(
-                ExperimentUtil.running_average(
-                    exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON],
-                    self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
-
-            # Log baseline returns
-            exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN].append(
-                round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN], 3))
-            exp_result.all_metrics[seed][
-                env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN].append(
-                round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN], 3))
-
-            if i % self.experiment_config.log_every == 0 and i > 0:
-                # Update training job
-                total_iterations = len(random_seeds) * N
-                iterations_done = (random_seeds.index(seed)) * N + i
-                progress = round(iterations_done / total_iterations, 2)
-                training_job.progress_percentage = progress
-                training_job.experiment_result = exp_result
-                if len(self.env.get_traces()) > 0:
-                    training_job.simulation_traces.append(self.env.get_traces()[-1])
-                if len(training_job.simulation_traces) > training_job.num_cached_traces:
-                    training_job.simulation_traces = training_job.simulation_traces[1:]
-                if self.save_to_metastore:
-                    MetastoreFacade.update_training_job(training_job=training_job, id=training_job.id)
-
-                # Update execution
-                ts = time.time()
-                self.exp_execution.timestamp = ts
-                self.exp_execution.result = exp_result
-                if self.save_to_metastore:
-                    MetastoreFacade.update_experiment_execution(experiment_execution=self.exp_execution,
-                                                                id=self.exp_execution.id)
-
-                Logger.__call__().get_logger().info(
-                    f"[REINFORCE] i: {i}, J:{J}, "
-                    f"J_avg_{self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value}:"
-                    f"{running_avg_J}, "
-                    f"opt_J:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN][-1]}, "
-                    f"int_len:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH][-1]}, "
-                    f"progress: {round(progress*100,2)}%")
-
-        ts = time.time()
-        save_path = f"{self.experiment_config.output_dir}/ppo_policy_seed_{seed}_{ts}.zip"
-        policy = FNNWithSoftmaxPolicy(
-            policy_network=policy_network, simulation_name=self.simulation_env_config.name,
-            save_path=save_path,
-            states=self.simulation_env_config.state_space_config.states,
+        return [agents_constants.COMMON.EVAL_BATCH_SIZE, agents_constants.COMMON.CONFIDENCE_INTERVAL,
+                agents_constants.COMMON.RUNNING_AVERAGE, agents_constants.COMMON.GAMMA,
+                agents_constants.SONDIK_VI.TRANSITION_TENSOR,
+                agents_constants.SONDIK_VI.REWARD_TENSOR, agents_constants.SONDIK_VI.OBSERVATION_TENSOR,
+                agents_constants.SONDIK_VI.OBSERVATION_SPACE, agents_constants.SONDIK_VI.STATE_SPACE,
+                agents_constants.SONDIK_VI.USE_PRUNING, agents_constants.SONDIK_VI.PLANNING_HORIZON,
+                agents_constants.SONDIK_VI.INITIAL_BELIEF]
+
+    def sondik_vi_algorithm(self, exp_result: ExperimentResult, seed: int) -> ExperimentResult:
+        """
+        Runs
+
+        :param exp_result: the experiment result object
+        :param seed: the random seed
+        :return: the updated experiment result
+        """
+        discount_factor = self.experiment_config.hparams[agents_constants.COMMON.GAMMA].value
+        eval_batch_size = self.experiment_config.hparams[agents_constants.COMMON.EVAL_BATCH_SIZE].value
+        T = self.experiment_config.hparams[agents_constants.SONDIK_VI.TRANSITION_TENSOR].value
+        R = self.experiment_config.hparams[agents_constants.SONDIK_VI.REWARD_TENSOR].value
+        Z = self.experiment_config.hparams[agents_constants.SONDIK_VI.OBSERVATION_TENSOR].value
+        O = self.experiment_config.hparams[agents_constants.SONDIK_VI.OBSERVATION_SPACE].value
+        S = self.experiment_config.hparams[agents_constants.SONDIK_VI.STATE_SPACE].value
+        A = self.experiment_config.hparams[agents_constants.SONDIK_VI.ACTION_SPACE].value
+        b0 = self.experiment_config.hparams[agents_constants.SONDIK_VI.INITIAL_BELIEF].value
+        use_pruning = \
+            self.experiment_config.hparams[agents_constants.SONDIK_VI.USE_PRUNING].value
+        planning_horizon = self.experiment_config.hparams[agents_constants.SONDIK_VI.PLANNING_HORIZON].value
+        Logger.__call__().get_logger().info(f"Starting Sondik's value iteration,"
+                                            f"discount_factor: {discount_factor}, pruning: {use_pruning}, b0: {b0}")
+        alpha_vectors, num_alpha_vectors, initial_belief_values, avg_returns, running_avg_returns = \
+            self.sondik_vi(P=np.array(T), R=np.array(R), n_obs=len(O), n_states=len(S), Z=np.array(Z), n_actions=len(A),
+                           b0=b0, T=planning_horizon, gamma=discount_factor, eval_batch_size=eval_batch_size)
+        exp_result.all_metrics[seed][agents_constants.SONDIK_VI.INITIAL_BELIEF_VALUES] = initial_belief_values
+        exp_result.all_metrics[seed][agents_constants.SONDIK_VI.NUM_ALPHA_VECTORS] = num_alpha_vectors
+        exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN] = avg_returns
+        exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN] = running_avg_returns
+        alpha_vec_policy = AlphaVectorsPolicy(
+            player_type=self.experiment_config.player_type,
             actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, player_type=self.experiment_config.player_type,
-            experiment_config=self.experiment_config,
-            avg_R=exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN][-1],
-            input_dim=policy_network.input_dim, output_dim=policy_network.output_dim)
-        policy.save_policy_network()
-
-        exp_result.policies[seed] = policy
-        # Save policy
-        if self.save_to_metastore:
-            MetastoreFacade.save_fnn_w_softmax_policy(fnn_w_softmax_policy=policy)
+                self.experiment_config.player_idx].actions,
+            states=self.simulation_env_config.state_space_config.states,
+            alpha_vectors=alpha_vectors, agent_type=self.experiment_config.agent_type, avg_R=-1,
+            simulation_name=self.simulation_env_config.name, transition_tensor=T, reward_tensor=R)
+        exp_result.policies[seed] = alpha_vec_policy
         return exp_result
 
-    @staticmethod
-    def update_metrics(metrics: Dict[str, List[Union[float, int]]], info: Dict[str, Union[float, int]]) \
-            -> Dict[str, List[Union[float, int]]]:
+    def compute_all_conditional_plans_conditioned_on_a_t(self, n_alpha_vectors_t_plus_one, n_obs):
         """
-        Update a dict with aggregated metrics using new information from the environment
+        Compute the number of conditional plans conditioned on an action a. It produces all possible combinations of
+        (observation -> conditional_plan)
 
-        :param metrics: the dict with the aggregated metrics
-        :param info: the new information
-        :return: the updated dict
-        """
-        for k, v in info.items():
-            if k in metrics:
-                metrics[k].append(round(v, 3))
-            else:
-                metrics[k] = [v]
-        return metrics
-
-    @staticmethod
-    def compute_avg_metrics(metrics: Dict[str, List[Union[float, int]]]) -> Dict[str, Union[float, int]]:
-        """
-        Computes the average metrics of a dict with aggregated metrics
-
-        :param metrics: the dict with the aggregated metrics
-        :return: the average metrics
-        """
-        avg_metrics = {}
-        for k, v in metrics.items():
-            avg = round(sum(v) / len(v), 2)
-            avg_metrics[k] = avg
-        return avg_metrics
-
-    @staticmethod
-    def round_vec(vec) -> List[float]:
-        """
-        Rounds a vector to 3 decimals
-
-        :param vec: the vector to round
-        :return: the rounded vector
-        """
-        return list(map(lambda x: round(x, 3), vec))
+        :param n_alpha_vectors_t_plus_one: Number of alpha-vectors (number of conditional plans) for t+1
+        :param n_obs: Number of observations
+        :return: list of lists, where each list contains n_obs elements, and each element is in [0, n_alpha_vectors-1].
+
+        The number of conditional plans will be be n_alpha_vectors^n_obs elements.
+        The plan is of the form: (o^(1)_i, o^(2)_j, ..., o^(n_alpha_vectors_t_plus_one)_k)
+        where o^(1)_i means that if observation o_i is observed, conditional plan 1 should be followed,
+        o^(2)_j means that if observation o_j is observed, conditional plan 2 should be followed,
+        o^(n_alpha_vectors_t_plus_one)_k means that if observation o_k is observed, conditional plan
+        n_alpha_vectors_t_plus_one should be followed.
+        """
+        x = list(range(n_alpha_vectors_t_plus_one))
+        return [p for p in product(x, repeat=n_obs)]
+
+    def sondik_vi(self, P, Z, R, T, gamma, n_states, n_actions, n_obs, b0, eval_batch_size: int,
+                  use_pruning: bool = True) \
+            -> Tuple[List[float], List[float], List[float], List[float], List[float]]:
+        """
+
+        :param P: The transition probability matrix
+        :param Z: The observation probability matrix
+        :param R: The immediate rewards matrix
+        :param T: The planning horizon
+        :param gamma: The discount factor
+        :param n_states: The number of states
+        :param n_actions: The number of actions
+        :param n_obs: The number of observations
+        :param eval_batch_size: number of simulations to evaluate the policy induced by the alpha vectors
+                               at each iteration
+        :param b0: The initial belief
+        :return:
+        """
+        alepth_t_plus_1 = set()
+        zero_alpha_vec = (-1, tuple(np.zeros(n_states)))  # an alpha vector is associated with an action and
+        # a set of values
+        alepth_t_plus_1.add(zero_alpha_vec)
+        first = True
+        num_alpha_vectors = []
+        num_alpha_vectors.append(len(alepth_t_plus_1))
+        initial_values = []
+        average_returns = []
+        average_running_returns = []
+
+        # Backward induction
+        for t in range(T):
+            Logger.__call__().get_logger().info(
+                '[Value Iteration] planning horizon {}, |aleph|:{} ...'.format(t, len(alepth_t_plus_1)))
+
+            # New set of alpha vectors which will be constructed from the previous (backwards) set aleph_t+1.
+            aleph_t = set()
+
+            # Weight the alpha vectors in aleph_t by the transition probabilities alpha(s)*Z(s'|s,o)*P(s'|s,a)
+            # forall a,o,s,s'
+            # alpha'(s) = alpha(s)*Z(s'|s,o)*P(s'|s,a) forall a,o,s,s'
+            alpha_new = np.zeros(shape=(len(alepth_t_plus_1), n_actions, n_obs, n_states))
+            n_alpha_vectors = 0
+            for old_alpha_vec in alepth_t_plus_1:
+                for a in range(n_actions):
+                    for o in range(n_obs):
+                        for s in range(n_states):
+                            for s_prime in range(n_states):
+                                # Half of Sondik's one-pass DP backup, alpha'_(a,o)(s)=alpha(s')*Z(s'|s,o)*P(s'|s,a)
+                                # forall a,o,s,s'
+                                # note that alpha(s) is a representation of $V(s)$
+                                alpha_new[n_alpha_vectors][a][o][s] += \
+                                    np.array(old_alpha_vec[1][s_prime]) * Z[a][s_prime][o] * P[a][s][s_prime]
+                n_alpha_vectors += 1
+
+            # Compute the new alpha vectors by adding the discounted immediate rewards and the expected
+            # alpha vectors at time t+1
+            # There are in total |Gamma^(k+1)|=|A|*|Gamma^k|^(|Z|) number of conditional plans, which means that there
+            # is |Gamma^(k+1)|=|A|*|Gamma^k|^(|Z|) number of alpha vectors
+            for a in range(n_actions):
+
+                # |Gamma^k|^(|Z|) number of conditional plans conditioned on 'a'
+                conditional_plans_conditioned_on_a = self.compute_all_conditional_plans_conditioned_on_a_t(
+                    n_alpha_vectors, n_obs)
+
+                # Each conditional plan is of the form (o^(1)_i, o^(2)_j, ..., o^(n_alpha_vectors_t_plus_one)_k)
+                # where o^(p)_i means that if observation o_i is observed, conditional plan p should be followed
+                for conditional_plan_conditioned_on_a in conditional_plans_conditioned_on_a:
+                    for o in range(n_obs):
+                        conditional_plan_to_follow_when_observing_o = conditional_plan_conditioned_on_a[o]
+                        temp = np.zeros(n_states)
+                        for s in range(n_states):
+                            # Second half of Sondik's one-pass DP backup,
+                            # alpha_(a,o,beta)'(s) = gamma*(R(a,s) alpha_beta(s)*Z(s'|s,o)*P(s'|s,a) forall a,o,s,s')
+                            temp[s] = gamma * (R[a][s] +
+                                               alpha_new[conditional_plan_to_follow_when_observing_o][a][o][s])
+                        aleph_t.add((a, tuple(temp)))
+
+            alepth_t_plus_1.update(aleph_t)
+            num_alpha_vectors.append(len(alepth_t_plus_1))
+
+            if first:
+                # remove the dummy alpha vector
+                alepth_t_plus_1.remove(zero_alpha_vec)
+                first = False
+
+            if use_pruning:
+                alepth_t_plus_1 = self.prune(n_states, alepth_t_plus_1)  # remove dominated alpha vectors
+
+            # The optimal value function is implicitly represented by aleph^0. Note that aleph^0 is a much larger set of
+            # elements than the set of states. To compute the optimal value function V^*(b0) given an initial belief b0,
+            # compute
+            # V^*(b) = max_alpha b0*alpha for all alpha in aleph^0
+            max_v = -np.inf
+            for alpha in aleph_t:
+                v = np.dot(np.array(alpha[1]), b0)
+
+                if v > max_v:
+                    max_v = v
+            initial_values.append(max_v)
+            avg_R = -1
+            if len(average_returns) > 0:
+                avg_R = average_returns[-1]
+            alpha_vec_policy = AlphaVectorsPolicy(
+                player_type=self.experiment_config.player_type,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions,
+                states=self.simulation_env_config.state_space_config.states,
+                alpha_vectors=list(map(lambda x: x[1], list(aleph_t))), agent_type=self.experiment_config.agent_type,
+                avg_R=avg_R,
+                simulation_name=self.simulation_env_config.name, transition_tensor=P, reward_tensor=R)
+            avg_r = self.evaluate_policy(alpha_vec_policy, eval_batch_size=eval_batch_size)
+            average_returns.append(avg_r)
+            running_avg_J = ExperimentUtil.running_average(
+                average_returns, self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value)
+            average_running_returns.append(running_avg_J)
 
-    def training_step(self, saved_rewards: List[List[float]], saved_log_probs: List[List[torch.Tensor]],
-                      policy_network: FNNwithSoftmax, optimizer: torch.optim.Optimizer, gamma: float) -> torch.Tensor:
-        """
-        Performs a training step of the REINFORCE algorithm
+        return (list(map(lambda x: x[1], list(aleph_t))), num_alpha_vectors, initial_values, average_returns,
+                average_running_returns)
 
-        :param saved_rewards: list of rewards encountered in the latest episode trajectory
-        :param saved_log_probs: list of log-action probabilities (log p(a|s)) encountered in the latest
-                                episode trajectory
-        :param policy_network: the policy network
-        :param optimizer: the optimizer for updating the weights
-        :param gamma: the discount factor
-        :return: loss
+    def prune(self, n_states, aleph):
         """
-        policy_loss = []
-        num_batches = len(saved_rewards)
-
-        for batch in range(num_batches):
+        Remove dominated alpha-vectors using Lark's filtering algorithm
+        :param n_states
+        :return:
+        """
+        # parameters for linear program
+        delta = 0.0000000001
+        # equality constraints on the belief states
+        A_eq = np.array([np.append(np.ones(n_states), [0.])])
+        b_eq = np.array([1.])
+
+        # dirty set
+        F = aleph.copy()
+
+        # clean set
+        Q = set()
+
+        for i in range(n_states):
+            max_i = -np.inf
+            best = None
+            for av in F:
+                # av[1] = np.array(av[1])
+                if av[1][i] > max_i:
+                    max_i = av[1][i]
+                    best = av
+            if best is not None and len(F) > 0:
+                Q.update({best})
+                F.remove(best)
+        while F:
+            av_i = F.pop()  # get a reference to av_i
+            F.add(av_i)  # don't want to remove it yet from F
+            dominated = False
+            for av_j in Q:
+                c = np.append(np.zeros(n_states), [1.])
+                A_ub = np.array([np.append(-(np.array(av_i[1]) - np.array(av_j[1])), [-1.])])
+                b_ub = np.array([-delta])
+
+                res = linprog(c, A_eq=A_eq, b_eq=b_eq, A_ub=A_ub, b_ub=b_ub, bounds=(0, None))
+                if res.x[n_states] > 0.0:
+                    # this one is dominated
+                    dominated = True
+                    F.remove(av_i)
+                    break
+
+            if not dominated:
+                max_k = -np.inf
+                best = None
+                for av_k in F:
+                    b = res.x[0:2]
+                    v = np.dot(av_k.v, b)
+                    if v > max_k:
+                        max_k = v
+                        best = av_k
+                F.remove(best)
+                if not self.check_duplicate(Q, best):
+                    Q.update({best})
+        return Q
+
+    def check_duplicate(self, a, av):
+        """
+        Check whether alpha vector av is already in set a
+
+        :param a:
+        :param av:
+        :return:
+        """
+        for av_i in a:
+            if np.allclose(av_i[1], av.v):
+                return True
+            if av_i[1][0] == av[1][0] and av_i[1][1] > av[1][1]:
+                return True
+            if av_i[1][1] == av[1][1] and av_i[1][0] > av[1][0]:
+                return True
+
+    def evaluate_policy(self, policy: AlphaVectorsPolicy, eval_batch_size: int) -> float:
+        """
+        Evalutes a tabular policy
+
+        :param policy: the tabular policy to evaluate
+        :param eval_batch_size: the batch size
+        :return: None
+        """
+        returns = []
+        for i in range(eval_batch_size):
+            done = False
+            o = self.env.reset()
             R = 0
-            returns = []
-
-            # Create discounted returns. When episode is finished we can go back and compute the observed cumulative
-            # discounted reward by using the observed rewards
-            for r in saved_rewards[batch][::-1]:
-                R = r + gamma * R
-                returns.insert(0, R)
-            num_rewards = len(returns)
-
-            # convert list to torch tensor
-            returns = torch.tensor(returns)
-
-            # normalize
-            std = returns.std()
-            if num_rewards < 2:
-                std = 0
-            returns = (returns - returns.mean()) / (std + self.machine_eps)
-
-            # Compute PG "loss" which in reality is the expected reward, which we want to maximize with gradient ascent
-            for log_prob, R in zip(saved_log_probs[batch], returns):
-                # negative log prob since we are doing gradient descent (not ascent)
-                policy_loss.append(-log_prob * R)
-
-        # Compute gradient and update models
-        # reset gradients
-        optimizer.zero_grad()
-        # expected loss over the batch
-        policy_loss_total = torch.stack(policy_loss).sum()
-        policy_loss = policy_loss_total / num_batches
-        # perform backprop
-        policy_loss.backward()
-        # maybe clip gradient
-        if self.experiment_config.hparams[constants.NEURAL_NETWORKS.DEVICE].value:
-            torch.nn.utils.clip_grad_norm_(policy_network.parameters(), 1)
-        # gradient descent step
-        optimizer.step()
-        return policy_loss
+            while not done:
+                b1 = o[1]
+                b = [1 - b1, b1, 0]
+                a = policy.action(b)
+                o, r, done, info = self.env.step(a)
+                R += r
+            returns.append(R)
+        avg_return = np.mean(returns)
+        return float(avg_return)
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/sarsa/sarsa_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/sarsa/sarsa_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import List, Optional, Tuple, Union
 import math
 import time
 import os
 import numpy as np
-import gym
+import gymnasium as gym
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.tabular_policy import TabularPolicy
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
 class SARSAAgent(BaseAgent):
     """
     SARSA Agent
@@ -66,15 +67,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=None, simulation_traces=[],
                 num_cached_traces=0,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
-from csle_agents.agents.base.base_agent import BaseAgent
-import csle_agents.constants.constants as agents_constants
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.tabular_policy import TabularPolicy
+from csle_common.util.general_util import GeneralUtil
+from csle_agents.agents.base.base_agent import BaseAgent
+import csle_agents.constants.constants as agents_constants
 
 
 class ShapleyIterationAgent(BaseAgent):
     """
     Shapley Iteration Agent
     """
 
@@ -61,15 +62,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=None, simulation_traces=[],
                 num_cached_traces=0,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/vi/vi_agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import math
 from typing import List, Optional, Tuple
 import time
 import os
 import numpy as np
-import gym
+import gymnasium as gym
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
-from csle_common.dao.training.alpha_vectors_policy import AlphaVectorsPolicy
+from csle_common.dao.training.tabular_policy import TabularPolicy
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
-from scipy.optimize import linprog
-from itertools import product
 
 
-class SondikVIAgent(BaseAgent):
+class VIAgent(BaseAgent):
     """
-    Sondik's value iteration for POMDPs (Sondik 1971)
+    Value Iteration Agent
     """
 
     def __init__(self, simulation_env_config: SimulationEnvConfig,
                  experiment_config: ExperimentConfig,
                  training_job: Optional[TrainingJobConfig] = None, save_to_metastore: bool = True):
         """
-        Initializes the Sondik-VI agent
+        Initializes the value iteration agent
 
         :param simulation_env_config: configuration of the simulation environment
         :param experiment_config: the experiment configuration
         :param training_job: an existing training job to use (optional)
         :param save_to_metastore: boolean flag whether to save the execution to the metastore
         """
         super().__init__(simulation_env_config=simulation_env_config, emulation_env_config=None,
                          experiment_config=experiment_config)
-        assert experiment_config.agent_type == AgentType.SONDIK_VALUE_ITERATION
+        assert experiment_config.agent_type == AgentType.VALUE_ITERATION
         self.training_job = training_job
         self.save_to_metastore = save_to_metastore
         self.env = gym.make(self.simulation_env_config.gym_env_name,
                             config=self.simulation_env_config.simulation_env_input_config)
 
     def train(self) -> ExperimentExecution:
         """
@@ -52,35 +51,33 @@
         """
         pid = os.getpid()
 
         # Initialize metrics
         exp_result = ExperimentResult()
         exp_result.plot_metrics.append(agents_constants.COMMON.AVERAGE_RETURN)
         exp_result.plot_metrics.append(agents_constants.COMMON.RUNNING_AVERAGE_RETURN)
-        exp_result.plot_metrics.append(agents_constants.SONDIK_VI.INITIAL_BELIEF_VALUES)
-        exp_result.plot_metrics.append(agents_constants.SONDIK_VI.NUM_ALPHA_VECTORS)
+        exp_result.plot_metrics.append(agents_constants.VI.DELTA)
 
-        descr = f"Computation of V* with the Sondik value algorithm using " \
+        descr = f"Computation of V* with the Value Iteration algorithm using " \
                 f"simulation:{self.simulation_env_config.name}"
 
         for seed in self.experiment_config.random_seeds:
             exp_result.all_metrics[seed] = {}
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN] = []
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN] = []
-            exp_result.all_metrics[seed][agents_constants.SONDIK_VI.NUM_ALPHA_VECTORS] = []
-            exp_result.all_metrics[seed][agents_constants.SONDIK_VI.INITIAL_BELIEF_VALUES] = []
 
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=None, simulation_traces=[],
                 num_cached_traces=0,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
@@ -98,15 +95,15 @@
                                                  descr=descr, log_file_path=self.training_job.log_file_path)
         if self.save_to_metastore:
             exp_execution_id = MetastoreFacade.save_experiment_execution(self.exp_execution)
             self.exp_execution.id = exp_execution_id
 
         for seed in self.experiment_config.random_seeds:
             ExperimentUtil.set_seed(seed)
-            exp_result = self.sondik_vi_algorithm(exp_result=exp_result, seed=seed)
+            exp_result = self.value_iteration(exp_result=exp_result, seed=seed)
 
         # Calculate average and std metrics
         exp_result.avg_metrics = {}
         exp_result.std_metrics = {}
         for metric in exp_result.all_metrics[self.experiment_config.random_seeds[0]].keys():
             value_vectors = []
             for seed in self.experiment_config.random_seeds:
@@ -150,287 +147,174 @@
 
     def hparam_names(self) -> List[str]:
         """
         :return: a list with the hyperparameter names
         """
         return [agents_constants.COMMON.EVAL_BATCH_SIZE, agents_constants.COMMON.CONFIDENCE_INTERVAL,
                 agents_constants.COMMON.RUNNING_AVERAGE, agents_constants.COMMON.GAMMA,
-                agents_constants.SONDIK_VI.TRANSITION_TENSOR,
-                agents_constants.SONDIK_VI.REWARD_TENSOR, agents_constants.SONDIK_VI.OBSERVATION_TENSOR,
-                agents_constants.SONDIK_VI.OBSERVATION_SPACE, agents_constants.SONDIK_VI.STATE_SPACE,
-                agents_constants.SONDIK_VI.USE_PRUNING, agents_constants.SONDIK_VI.PLANNING_HORIZON,
-                agents_constants.SONDIK_VI.INITIAL_BELIEF]
+                agents_constants.VI.THETA, agents_constants.VI.TRANSITION_TENSOR,
+                agents_constants.VI.REWARD_TENSOR, agents_constants.VI.NUM_STATES, agents_constants.VI.NUM_ACTIONS]
 
-    def sondik_vi_algorithm(self, exp_result: ExperimentResult, seed: int) -> ExperimentResult:
+    def value_iteration(self, exp_result: ExperimentResult, seed: int) -> ExperimentResult:
         """
-        Runs
+        Runs the value iteration algorithm
 
         :param exp_result: the experiment result object
         :param seed: the random seed
         :return: the updated experiment result
         """
+        theta = self.experiment_config.hparams[agents_constants.VI.THETA].value
         discount_factor = self.experiment_config.hparams[agents_constants.COMMON.GAMMA].value
-        eval_batch_size = self.experiment_config.hparams[agents_constants.COMMON.EVAL_BATCH_SIZE].value
-        T = self.experiment_config.hparams[agents_constants.SONDIK_VI.TRANSITION_TENSOR].value
-        R = self.experiment_config.hparams[agents_constants.SONDIK_VI.REWARD_TENSOR].value
-        Z = self.experiment_config.hparams[agents_constants.SONDIK_VI.OBSERVATION_TENSOR].value
-        O = self.experiment_config.hparams[agents_constants.SONDIK_VI.OBSERVATION_SPACE].value
-        S = self.experiment_config.hparams[agents_constants.SONDIK_VI.STATE_SPACE].value
-        A = self.experiment_config.hparams[agents_constants.SONDIK_VI.ACTION_SPACE].value
-        b0 = self.experiment_config.hparams[agents_constants.SONDIK_VI.INITIAL_BELIEF].value
-        use_pruning = \
-            self.experiment_config.hparams[agents_constants.SONDIK_VI.USE_PRUNING].value
-        planning_horizon = self.experiment_config.hparams[agents_constants.SONDIK_VI.PLANNING_HORIZON].value
-        Logger.__call__().get_logger().info(f"Starting Sondik's value iteration,"
-                                            f"discount_factor: {discount_factor}, pruning: {use_pruning}, b0: {b0}")
-        alpha_vectors, num_alpha_vectors, initial_belief_values, avg_returns, running_avg_returns = \
-            self.sondik_vi(P=np.array(T), R=np.array(R), n_obs=len(O), n_states=len(S), Z=np.array(Z), n_actions=len(A),
-                           b0=b0, T=planning_horizon, gamma=discount_factor, eval_batch_size=eval_batch_size)
-        exp_result.all_metrics[seed][agents_constants.SONDIK_VI.INITIAL_BELIEF_VALUES] = initial_belief_values
-        exp_result.all_metrics[seed][agents_constants.SONDIK_VI.NUM_ALPHA_VECTORS] = num_alpha_vectors
+        num_states = self.experiment_config.hparams[agents_constants.VI.NUM_STATES].value
+        num_actions = self.experiment_config.hparams[agents_constants.VI.NUM_ACTIONS].value
+        T = self.experiment_config.hparams[agents_constants.VI.TRANSITION_TENSOR].value
+        R = self.experiment_config.hparams[agents_constants.VI.REWARD_TENSOR].value
+        Logger.__call__().get_logger().info(f"Starting the value iteration algorithm, theta:{theta}, "
+                                            f"num_states:{num_states}, discount_factor: {discount_factor}, "
+                                            f"num_actions: {num_actions}")
+        V, policy, deltas, avg_returns, running_avg_returns = self.vi(
+            T=np.array(T), num_states=num_states, num_actions=num_actions,
+            R=np.array(R), theta=theta, discount_factor=discount_factor)
+        exp_result.all_metrics[seed][agents_constants.VI.DELTA] = deltas
         exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN] = avg_returns
         exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN] = running_avg_returns
-        alpha_vec_policy = AlphaVectorsPolicy(
-            player_type=self.experiment_config.player_type,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions,
-            states=self.simulation_env_config.state_space_config.states,
-            alpha_vectors=alpha_vectors, agent_type=self.experiment_config.agent_type, avg_R=-1,
-            simulation_name=self.simulation_env_config.name, transition_tensor=T, reward_tensor=R)
-        exp_result.policies[seed] = alpha_vec_policy
+        lookup_table = list(policy)
+        for i in range(len(lookup_table)):
+            lookup_table[i] = list(lookup_table[i])
+        tabular_policy = TabularPolicy(player_type=self.experiment_config.player_type,
+                                       actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                                           self.experiment_config.player_idx].actions,
+                                       agent_type=self.experiment_config.agent_type, value_function=list(V),
+                                       lookup_table=lookup_table, simulation_name=self.simulation_env_config.name,
+                                       avg_R=avg_returns[-1])
+        exp_result.policies[seed] = tabular_policy
         return exp_result
 
-    def compute_all_conditional_plans_conditioned_on_a_t(self, n_alpha_vectors_t_plus_one, n_obs):
+    def one_step_lookahead(self, state, V, num_actions, num_states, T, discount_factor, R) \
+            -> np.ndarray:
         """
-        Compute the number of conditional plans conditioned on an action a. It produces all possible combinations of
-        (observation -> conditional_plan)
-
-        :param n_alpha_vectors_t_plus_one: Number of alpha-vectors (number of conditional plans) for t+1
-        :param n_obs: Number of observations
-        :return: list of lists, where each list contains n_obs elements, and each element is in [0, n_alpha_vectors-1].
-
-        The number of conditional plans will be be n_alpha_vectors^n_obs elements.
-        The plan is of the form: (o^(1)_i, o^(2)_j, ..., o^(n_alpha_vectors_t_plus_one)_k)
-        where o^(1)_i means that if observation o_i is observed, conditional plan 1 should be followed,
-        o^(2)_j means that if observation o_j is observed, conditional plan 2 should be followed,
-        o^(n_alpha_vectors_t_plus_one)_k means that if observation o_k is observed, conditional plan
-        n_alpha_vectors_t_plus_one should be followed.
-        """
-        x = list(range(n_alpha_vectors_t_plus_one))
-        return [p for p in product(x, repeat=n_obs)]
-
-    def sondik_vi(self, P, Z, R, T, gamma, n_states, n_actions, n_obs, b0, eval_batch_size: int,
-                  use_pruning: bool = True) \
-            -> Tuple[List[float], List[float], List[float], List[float], List[float]]:
-        """
-
-        :param P: The transition probability matrix
-        :param Z: The observation probability matrix
-        :param R: The immediate rewards matrix
-        :param T: The planning horizon
-        :param gamma: The discount factor
-        :param n_states: The number of states
-        :param n_actions: The number of actions
-        :param n_obs: The number of observations
-        :param eval_batch_size: number of simulations to evaluate the policy induced by the alpha vectors
-                               at each iteration
-        :param b0: The initial belief
-        :return:
-        """
-        alepth_t_plus_1 = set()
-        zero_alpha_vec = (-1, tuple(np.zeros(n_states)))  # an alpha vector is associated with an action and
-        # a set of values
-        alepth_t_plus_1.add(zero_alpha_vec)
-        first = True
-        num_alpha_vectors = []
-        num_alpha_vectors.append(len(alepth_t_plus_1))
-        initial_values = []
+        Performs a one-step lookahead for value iteration
+        :param state: the current state
+        :param V: the current value function
+        :param num_actions: the number of actions
+        :param num_states: the number of states
+        :param T: the transition kernel
+        :param discount_factor: the discount factor
+        :param R: the table with rewards
+        :param next_state_lookahead: the next state lookahead table
+        :return: an array with lookahead values
+        """
+        A = np.zeros(num_actions)
+        for a in range(num_actions):
+            reward = R[a][state]
+            for next_state in range(num_states):
+                prob = T[a][state][next_state]
+                A[a] += prob * (reward + discount_factor * V[next_state])
+        return A
+
+    def vi(self, T: np.ndarray, num_states: int, num_actions: int, R: np.ndarray,
+           theta=0.0001, discount_factor=1.0) -> Tuple[np.ndarray, np.ndarray, List, List, List]:
+        """
+        An implementation of the Value Iteration algorithm
+        :param T: the transition kernel T
+        :param num_states: the number of states
+        :param num_actions: the number of actions
+        :param state_to_id: the state-to-id lookup table
+        :param HP: the table with hack probabilities
+        :param R: the table with rewards
+        :param next_state_lookahead: the next-state-lookahead table
+        :param theta: convergence threshold
+        :param discount_factor: the discount factor
+        :return: (greedy policy, value function, deltas, average_returns)
+        """
+        deltas = []
         average_returns = []
-        average_running_returns = []
+        running_average_returns = []
+        V = np.zeros(num_states)
+        iteration = 0
+        while True:
+            # Stopping condition
+            delta = 0
+            # Update each state...
+            for s in range(num_states):
+                # Do a one-step lookahead to find the best action
+                A = self.one_step_lookahead(s, V, num_actions, num_states, T, discount_factor, R)
+                best_action_value = np.max(A)
+                # Calculate delta across all states seen so far
+                delta = max(delta, np.abs(best_action_value - V[s]))
+                # Update the value function. Ref: Sutton book eq. 4.10.
+                V[s] = best_action_value
+
+            deltas.append(delta)
+
+            avg_return = -1
+            if iteration % self.experiment_config.hparams[agents_constants.COMMON.EVAL_EVERY].value == 0:
+                policy = self.create_policy_from_value_function(num_states=num_states, num_actions=num_actions, V=V,
+                                                                T=T, discount_factor=discount_factor, R=R)
+                avg_return = self.evaluate_policy(policy=policy, eval_batch_size=self.experiment_config.hparams[
+                    agents_constants.COMMON.EVAL_BATCH_SIZE].value)
+                average_returns.append(avg_return)
+                running_avg_J = ExperimentUtil.running_average(
+                    average_returns,
+                    self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value)
+                running_average_returns.append(running_avg_J)
+
+            if iteration % self.experiment_config.log_every == 0 and iteration > 0:
+                Logger.__call__().get_logger().info(f"[VI] i:{iteration}, delta: {delta}, "
+                                                    f"theta: {theta}, avg_return: {avg_return}")
+            iteration += 1
+
+            # Check if we can stop
+            if delta < theta:
+                break
+
+        policy = self.create_policy_from_value_function(num_states=num_states, num_actions=num_actions, V=V, T=T,
+                                                        discount_factor=discount_factor, R=R)
+        return V, policy, deltas, average_returns, running_average_returns
 
-        # Backward induction
-        for t in range(T):
-            Logger.__call__().get_logger().info(
-                '[Value Iteration] planning horizon {}, |aleph|:{} ...'.format(t, len(alepth_t_plus_1)))
-
-            # New set of alpha vectors which will be constructed from the previous (backwards) set aleph_t+1.
-            aleph_t = set()
-
-            # Weight the alpha vectors in aleph_t by the transition probabilities alpha(s)*Z(s'|s,o)*P(s'|s,a)
-            # forall a,o,s,s'
-            # alpha'(s) = alpha(s)*Z(s'|s,o)*P(s'|s,a) forall a,o,s,s'
-            alpha_new = np.zeros(shape=(len(alepth_t_plus_1), n_actions, n_obs, n_states))
-            n_alpha_vectors = 0
-            for old_alpha_vec in alepth_t_plus_1:
-                for a in range(n_actions):
-                    for o in range(n_obs):
-                        for s in range(n_states):
-                            for s_prime in range(n_states):
-                                # Half of Sondik's one-pass DP backup, alpha'_(a,o)(s)=alpha(s')*Z(s'|s,o)*P(s'|s,a)
-                                # forall a,o,s,s'
-                                # note that alpha(s) is a representation of $V(s)$
-                                alpha_new[n_alpha_vectors][a][o][s] += \
-                                    np.array(old_alpha_vec[1][s_prime]) * Z[a][s_prime][o] * P[a][s][s_prime]
-                n_alpha_vectors += 1
-
-            # Compute the new alpha vectors by adding the discounted immediate rewards and the expected
-            # alpha vectors at time t+1
-            # There are in total |Gamma^(k+1)|=|A|*|Gamma^k|^(|Z|) number of conditional plans, which means that there
-            # is |Gamma^(k+1)|=|A|*|Gamma^k|^(|Z|) number of alpha vectors
-            for a in range(n_actions):
-
-                # |Gamma^k|^(|Z|) number of conditional plans conditioned on 'a'
-                conditional_plans_conditioned_on_a = self.compute_all_conditional_plans_conditioned_on_a_t(
-                    n_alpha_vectors, n_obs)
-
-                # Each conditional plan is of the form (o^(1)_i, o^(2)_j, ..., o^(n_alpha_vectors_t_plus_one)_k)
-                # where o^(p)_i means that if observation o_i is observed, conditional plan p should be followed
-                for conditional_plan_conditioned_on_a in conditional_plans_conditioned_on_a:
-                    for o in range(n_obs):
-                        conditional_plan_to_follow_when_observing_o = conditional_plan_conditioned_on_a[o]
-                        temp = np.zeros(n_states)
-                        for s in range(n_states):
-                            # Second half of Sondik's one-pass DP backup,
-                            # alpha_(a,o,beta)'(s) = gamma*(R(a,s) alpha_beta(s)*Z(s'|s,o)*P(s'|s,a) forall a,o,s,s')
-                            temp[s] = gamma * (R[a][s] +
-                                               alpha_new[conditional_plan_to_follow_when_observing_o][a][o][s])
-                        aleph_t.add((a, tuple(temp)))
-
-            alepth_t_plus_1.update(aleph_t)
-            num_alpha_vectors.append(len(alepth_t_plus_1))
-
-            if first:
-                # remove the dummy alpha vector
-                alepth_t_plus_1.remove(zero_alpha_vec)
-                first = False
-
-            if use_pruning:
-                alepth_t_plus_1 = self.prune(n_states, alepth_t_plus_1)  # remove dominated alpha vectors
-
-            # The optimal value function is implicitly represented by aleph^0. Note that aleph^0 is a much larger set of
-            # elements than the set of states. To compute the optimal value function V^*(b0) given an initial belief b0,
-            # compute
-            # V^*(b) = max_alpha b0*alpha for all alpha in aleph^0
-            max_v = -np.inf
-            for alpha in aleph_t:
-                v = np.dot(np.array(alpha[1]), b0)
-
-                if v > max_v:
-                    max_v = v
-            initial_values.append(max_v)
-            avg_R = -1
-            if len(average_returns) > 0:
-                avg_R = average_returns[-1]
-            alpha_vec_policy = AlphaVectorsPolicy(
-                player_type=self.experiment_config.player_type,
-                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                    self.experiment_config.player_idx].actions,
-                states=self.simulation_env_config.state_space_config.states,
-                alpha_vectors=list(map(lambda x: x[1], list(aleph_t))), agent_type=self.experiment_config.agent_type,
-                avg_R=avg_R,
-                simulation_name=self.simulation_env_config.name, transition_tensor=P, reward_tensor=R)
-            avg_r = self.evaluate_policy(alpha_vec_policy, eval_batch_size=eval_batch_size)
-            average_returns.append(avg_r)
-            running_avg_J = ExperimentUtil.running_average(
-                average_returns, self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value)
-            average_running_returns.append(running_avg_J)
-
-        return (list(map(lambda x: x[1], list(aleph_t))), num_alpha_vectors, initial_values, average_returns,
-                average_running_returns)
-
-    def prune(self, n_states, aleph):
-        """
-        Remove dominated alpha-vectors using Lark's filtering algorithm
-        :param n_states
-        :return:
-        """
-        # parameters for linear program
-        delta = 0.0000000001
-        # equality constraints on the belief states
-        A_eq = np.array([np.append(np.ones(n_states), [0.])])
-        b_eq = np.array([1.])
-
-        # dirty set
-        F = aleph.copy()
-
-        # clean set
-        Q = set()
-
-        for i in range(n_states):
-            max_i = -np.inf
-            best = None
-            for av in F:
-                # av[1] = np.array(av[1])
-                if av[1][i] > max_i:
-                    max_i = av[1][i]
-                    best = av
-            if best is not None and len(F) > 0:
-                Q.update({best})
-                F.remove(best)
-        while F:
-            av_i = F.pop()  # get a reference to av_i
-            F.add(av_i)  # don't want to remove it yet from F
-            dominated = False
-            for av_j in Q:
-                c = np.append(np.zeros(n_states), [1.])
-                A_ub = np.array([np.append(-(np.array(av_i[1]) - np.array(av_j[1])), [-1.])])
-                b_ub = np.array([-delta])
-
-                res = linprog(c, A_eq=A_eq, b_eq=b_eq, A_ub=A_ub, b_ub=b_ub, bounds=(0, None))
-                if res.x[n_states] > 0.0:
-                    # this one is dominated
-                    dominated = True
-                    F.remove(av_i)
-                    break
-
-            if not dominated:
-                max_k = -np.inf
-                best = None
-                for av_k in F:
-                    b = res.x[0:2]
-                    v = np.dot(av_k.v, b)
-                    if v > max_k:
-                        max_k = v
-                        best = av_k
-                F.remove(best)
-                if not self.check_duplicate(Q, best):
-                    Q.update({best})
-        return Q
-
-    def check_duplicate(self, a, av):
-        """
-        Check whether alpha vector av is already in set a
-
-        :param a:
-        :param av:
-        :return:
-        """
-        for av_i in a:
-            if np.allclose(av_i[1], av.v):
-                return True
-            if av_i[1][0] == av[1][0] and av_i[1][1] > av[1][1]:
-                return True
-            if av_i[1][1] == av[1][1] and av_i[1][0] > av[1][0]:
-                return True
-
-    def evaluate_policy(self, policy: AlphaVectorsPolicy, eval_batch_size: int) -> float:
+    def evaluate_policy(self, policy: np.ndarray, eval_batch_size: int) -> float:
         """
         Evalutes a tabular policy
 
         :param policy: the tabular policy to evaluate
         :param eval_batch_size: the batch size
         :return: None
         """
         returns = []
         for i in range(eval_batch_size):
             done = False
-            o = self.env.reset()
+            s, _ = self.env.reset()
             R = 0
             while not done:
-                b1 = o[1]
-                b = [1 - b1, b1, 0]
-                a = policy.action(b)
-                o, r, done, info = self.env.step(a)
+                if self.simulation_env_config.gym_env_name == "csle-intrusion-response-game-local-pomdp-defender-v1":
+                    a = np.random.choice(np.arange(0, len(policy[int(s[0])])), p=policy[int(s[0])])
+                    s, r, done, _, info = self.env.step(a)
+                    done = True
+                else:
+                    s, r, done, _, info = self.env.step(policy)
                 R += r
             returns.append(R)
         avg_return = np.mean(returns)
         return float(avg_return)
+
+    def create_policy_from_value_function(self, num_states: int, num_actions: int, V: np.ndarray, T: np.ndarray,
+                                          discount_factor: float, R: np.ndarray) -> np.ndarray:
+        """
+        Creates a tabular policy from a value function
+
+        :param num_states: the number of states
+        :param num_actions: the number of actions
+        :param V: the value function
+        :param T: the transition operator
+        :param discount_factor: the discount factor
+        :param R: the reward function
+        :return: the tabular policy
+        """
+        # Create a deterministic policy using the optimal value function
+        policy = np.zeros([num_states, num_actions])
+        for s in range(num_states):
+            # One step lookahead to find the best action for this state
+            A = self.one_step_lookahead(s, V, num_actions, num_states, T, discount_factor, R)
+            best_action = np.argmax(A)
+            # Always take the best action
+            policy[s, best_action] = 1.0
+        return policy
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/t_fp/t_fp_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/t_fp/t_fp_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union, List, Dict, Tuple, Optional
 import time
-import gym
+import gymnasium as gym
 import os
 import math
 import numpy as np
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
@@ -15,14 +15,15 @@
 from csle_common.logging.log import Logger
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
 from csle_common.dao.training.mixed_multi_threshold_stopping_policy import MixedMultiThresholdStoppingPolicy
 from csle_common.dao.training.policy import Policy
 import csle_common.constants.constants as constants
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 from csle_agents.agents.t_spsa.t_spsa_agent import TSPSAAgent
 import csle_agents.constants.constants as agents_constants
 import gym_csle_stopping_game.constants.constants as env_constants
 
 
 class TFPAgent(BaseAgent):
@@ -125,15 +126,16 @@
 
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 experiment_result=exp_result, progress_percentage=0, pid=pid,
                 emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
             self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
             MetastoreFacade.update_training_job(training_job=self.training_job, id=self.training_job.id)
```

### Comparing `csle_agents-0.1.9/src/csle_agents/agents/t_spsa/t_spsa_agent.py` & `csle_agents-0.2.0/src/csle_agents/agents/t_spsa/t_spsa_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import math
 from typing import Union, List, Dict, Optional
 import random
 import time
-import gym
+import gymnasium as gym
 import os
 import numpy as np
 import gym_csle_stopping_game.constants.constants as env_constants
 from csle_common.dao.emulation_config.emulation_env_config import EmulationEnvConfig
 from csle_common.dao.simulation_config.simulation_env_config import SimulationEnvConfig
 from csle_common.dao.training.experiment_config import ExperimentConfig
 from csle_common.dao.training.experiment_execution import ExperimentExecution
 from csle_common.dao.training.experiment_result import ExperimentResult
 from csle_common.dao.training.agent_type import AgentType
 from csle_common.dao.training.player_type import PlayerType
 from csle_common.util.experiment_util import ExperimentUtil
 from csle_common.logging.log import Logger
 from csle_common.dao.training.multi_threshold_stopping_policy import MultiThresholdStoppingPolicy
+from csle_common.dao.training.linear_threshold_stopping_policy import LinearThresholdStoppingPolicy
+from csle_common.dao.training.policy_type import PolicyType
 from csle_common.metastore.metastore_facade import MetastoreFacade
 from csle_common.dao.jobs.training_job_config import TrainingJobConfig
 import csle_common.constants.constants as constants
+from csle_common.util.general_util import GeneralUtil
 from csle_agents.agents.base.base_agent import BaseAgent
 import csle_agents.constants.constants as agents_constants
 
 
 class TSPSAAgent(BaseAgent):
     """
     RL Agent implementing the T-SPSA algorithm from
@@ -115,15 +118,16 @@
         # Initialize training job
         if self.training_job is None:
             self.training_job = TrainingJobConfig(
                 simulation_env_name=self.simulation_env_config.name, experiment_config=self.experiment_config,
                 progress_percentage=0, pid=pid, experiment_result=exp_result,
                 emulation_env_name=self.emulation_env_config.name, simulation_traces=[],
                 num_cached_traces=agents_constants.COMMON.NUM_CACHED_SIMULATION_TRACES,
-                log_file_path=Logger.__call__().get_log_file_path(), descr=descr)
+                log_file_path=Logger.__call__().get_log_file_path(), descr=descr,
+                physical_host_ip=GeneralUtil.get_host_ip())
             if self.save_to_metastore:
                 training_job_id = MetastoreFacade.save_training_job(training_job=self.training_job)
                 self.training_job.id = training_job_id
         else:
             self.training_job.pid = pid
             self.training_job.progress_percentage = 0
             self.training_job.experiment_result = exp_result
@@ -229,21 +233,15 @@
         else:
             if self.experiment_config.player_type == PlayerType.DEFENDER:
                 theta = TSPSAAgent.initial_theta(L=L)
             else:
                 theta = TSPSAAgent.initial_theta(L=2 * L)
 
         # Initial eval
-        policy = MultiThresholdStoppingPolicy(
-            theta=theta, simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.T_SPSA)
+        policy = self.get_policy(theta=theta, L=L)
         avg_metrics = self.eval_theta(
             policy=policy, max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
         J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
         policy.avg_R = J
         exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
         exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(J)
         exp_result.all_metrics[seed][constants.T_SPSA.THETAS].append(TSPSAAgent.round_vec(theta))
@@ -276,41 +274,36 @@
                 if self.experiment_config.player_type == PlayerType.ATTACKER:
                     for l in range(0, L - 1):
                         theta[l] = min(theta[l], theta[l + 1])
                     for l in range(L, 2 * L - 1):
                         theta[l] = max(theta[l], theta[l + 1])
 
             # Evaluate new theta
-            policy = MultiThresholdStoppingPolicy(
-                theta=theta, simulation_name=self.simulation_env_config.name,
-                states=self.simulation_env_config.state_space_config.states,
-                player_type=self.experiment_config.player_type, L=L,
-                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-                agent_type=AgentType.T_SPSA)
+            policy = self.get_policy(theta=theta, L=L)
             avg_metrics = self.eval_theta(
                 policy=policy, max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
 
             # Log average return
             J = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
             policy.avg_R = J
             running_avg_J = ExperimentUtil.running_average(
                 exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN],
                 self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value)
             exp_result.all_metrics[seed][agents_constants.COMMON.AVERAGE_RETURN].append(J)
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_RETURN].append(running_avg_J)
 
-            # Log thresholds
             exp_result.all_metrics[seed][constants.T_SPSA.THETAS].append(TSPSAAgent.round_vec(theta))
-            exp_result.all_metrics[seed][constants.T_SPSA.THRESHOLDS].append(
-                TSPSAAgent.round_vec(policy.thresholds()))
-
-            # Log stop distribution
-            for k, v in policy.stop_distributions().items():
-                exp_result.all_metrics[seed][k].append(v)
+            if self.experiment_config.hparams[constants.T_SPSA.POLICY_TYPE] == PolicyType.MULTI_THRESHOLD:
+                # Log thresholds
+                exp_result.all_metrics[seed][constants.T_SPSA.THRESHOLDS].append(
+                    TSPSAAgent.round_vec(policy.thresholds()))
+
+                # Log stop distribution
+                for k, v in policy.stop_distributions().items():
+                    exp_result.all_metrics[seed][k].append(v)
 
             # Log intrusion lengths
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH].append(
                 round(avg_metrics[env_constants.ENV_METRICS.INTRUSION_LENGTH], 3))
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_INTRUSION_LENGTH].append(
                 ExperimentUtil.running_average(
                     exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH],
@@ -342,29 +335,33 @@
                     self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON].append(
                 round(avg_metrics[env_constants.ENV_METRICS.TIME_HORIZON], 3))
             exp_result.all_metrics[seed][agents_constants.COMMON.RUNNING_AVERAGE_TIME_HORIZON].append(
                 ExperimentUtil.running_average(
                     exp_result.all_metrics[seed][env_constants.ENV_METRICS.TIME_HORIZON],
                     self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
+
             for l in range(1, self.experiment_config.hparams[constants.T_SPSA.L].value + 1):
-                exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
-                exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"].append(
-                    round(avg_metrics[env_constants.ENV_METRICS.STOP + f"_{l}"], 3))
-                exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_running_average_{l}"].append(
-                    ExperimentUtil.running_average(
-                        exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"],
-                        self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
+                if env_constants.ENV_METRICS.STOP + f"_{l}" in avg_metrics:
+                    exp_result.plot_metrics.append(env_constants.ENV_METRICS.STOP + f"_{l}")
+                    exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"].append(
+                        round(avg_metrics[env_constants.ENV_METRICS.STOP + f"_{l}"], 3))
+                    exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_running_average_{l}"].append(
+                        ExperimentUtil.running_average(
+                            exp_result.all_metrics[seed][env_constants.ENV_METRICS.STOP + f"_{l}"],
+                            self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value))
 
             # Log baseline returns
             exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN].append(
                 round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN], 3))
-            exp_result.all_metrics[seed][
-                env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN].append(
-                round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN], 3))
+            if env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN in avg_metrics:
+                exp_result.all_metrics[seed][
+                    env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN].append(
+                    round(avg_metrics[env_constants.ENV_METRICS.AVERAGE_DEFENDER_BASELINE_STOP_ON_FIRST_ALERT_RETURN],
+                          3))
 
             if i % self.experiment_config.log_every == 0:
                 # Update training job
                 total_iterations = len(random_seeds) * N
                 iterations_done = (random_seeds.index(seed)) * N + i
                 progress = round(iterations_done / total_iterations, 2)
                 training_job.progress_percentage = progress
@@ -379,69 +376,56 @@
                 # Update execution
                 ts = time.time()
                 self.exp_execution.timestamp = ts
                 self.exp_execution.result = exp_result
                 if self.save_to_metastore:
                     MetastoreFacade.update_experiment_execution(experiment_execution=self.exp_execution,
                                                                 id=self.exp_execution.id)
-
-                intrusion_prediction_distance = \
-                    exp_result.all_metrics[seed][env_constants.ENV_METRICS.WEIGHTED_INTRUSION_PREDICTION_DISTANCE][-1]
                 Logger.__call__().get_logger().info(
                     f"[T-SPSA] i: {i}, J:{J}, "
                     f"J_avg_{self.experiment_config.hparams[agents_constants.COMMON.RUNNING_AVERAGE].value}:"
                     f"{running_avg_J}, "
                     f"opt_J:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.AVERAGE_UPPER_BOUND_RETURN][-1]}, "
                     f"int_len:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_LENGTH][-1]}, "
-                    f"w_dist: {intrusion_prediction_distance},"
-                    f"spc:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.START_POINT_CORRECT][-1]}, "
-                    f"stop_1:{exp_result.all_metrics[seed]['stop_1'][-1]}, "
-                    f"int_start:{exp_result.all_metrics[seed][env_constants.ENV_METRICS.INTRUSION_START][-1]}, "
-                    f"sigmoid(theta):{policy.thresholds()}, progress: {round(progress*100,2)}%, "
-                    f"stop distributions:{policy.stop_distributions()}")
-
-        policy = MultiThresholdStoppingPolicy(
-            theta=theta, simulation_name=self.simulation_env_config.name,
-            states=self.simulation_env_config.state_space_config.states,
-            player_type=self.experiment_config.player_type, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=J,
-            agent_type=AgentType.T_SPSA)
+                    f"theta:{policy.theta}, progress: {round(progress * 100, 2)}%")
+
+        policy = self.get_policy(theta=theta, L=L)
         exp_result.policies[seed] = policy
         # Save policy
         if self.save_to_metastore:
             MetastoreFacade.save_multi_threshold_stopping_policy(multi_threshold_stopping_policy=policy)
         return exp_result
 
-    def eval_theta(self, policy: MultiThresholdStoppingPolicy, max_steps: int = 200) -> Dict[str, Union[float, int]]:
+    def eval_theta(self, policy: Union[MultiThresholdStoppingPolicy, LinearThresholdStoppingPolicy],
+                   max_steps: int = 200) -> Dict[str, Union[float, int]]:
         """
         Evaluates a given threshold policy by running monte-carlo simulations
 
         :param policy: the policy to evaluate
         :return: the average metrics of the evaluation
         """
         eval_batch_size = self.experiment_config.hparams[agents_constants.COMMON.EVAL_BATCH_SIZE].value
         metrics = {}
         for j in range(eval_batch_size):
             done = False
-            o = self.env.reset()
+            o, _ = self.env.reset()
             l = int(o[0])
             b1 = o[1]
             t = 1
             r = 0
             a = 0
             info = {}
             while not done and t <= max_steps:
-                Logger.__call__().get_logger().debug(f"t:{t}, a: {a}, b1:{b1}, r:{r}, l:{l}, info:{info}")
+                Logger.__call__().get_logger().debug(f"t:{t}, a:{a}, b1:{b1}, r:{r}, l:{l}, info:{info}")
                 if self.experiment_config.player_type == PlayerType.ATTACKER:
                     policy.opponent_strategy = self.env.static_defender_strategy
                     a = policy.action(o=o)
                 else:
                     a = policy.action(o=o)
-                o, r, done, info = self.env.step(a)
+                o, r, done, _, info = self.env.step(a)
                 l = int(o[0])
                 b1 = o[1]
                 t += 1
             metrics = TSPSAAgent.update_metrics(metrics=metrics, info=info)
         avg_metrics = TSPSAAgent.compute_avg_metrics(metrics=metrics)
         return avg_metrics
 
@@ -559,30 +543,23 @@
         """
         # Get the two perturbed values of theta
         # list comprehensions like this are quite nice
         ta = [t + ck * dk for t, dk in zip(theta, deltak)]
         tb = [t - ck * dk for t, dk in zip(theta, deltak)]
 
         # Calculate g_k(theta_k)
-        avg_metrics = self.eval_theta(MultiThresholdStoppingPolicy(
-            theta=ta, simulation_name=self.simulation_env_config.name,
-            player_type=self.experiment_config.player_type,
-            states=self.simulation_env_config.state_space_config.states, L=L,
-            actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.T_SPSA),
+        policy_1 = self.get_policy(theta=ta, L=L)
+        avg_metrics = self.eval_theta(
+            policy_1,
             max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value
         )
         J_a = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
-        avg_metrics = self.eval_theta(MultiThresholdStoppingPolicy(
-            theta=tb, simulation_name=self.simulation_env_config.name,
-            player_type=self.experiment_config.player_type, states=self.simulation_env_config.state_space_config.states,
-            L=L, actions=self.simulation_env_config.joint_action_space_config.action_spaces[
-                self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
-            agent_type=AgentType.T_SPSA),
+        policy_2 = self.get_policy(theta=tb, L=L)
+        avg_metrics = self.eval_theta(
+            policy_2,
             max_steps=self.experiment_config.hparams[agents_constants.COMMON.MAX_ENV_STEPS].value)
         J_b = round(avg_metrics[env_constants.ENV_METRICS.RETURN], 3)
         gk = [(J_a - J_b) / (2 * ck * dk) for dk in deltak]
 
         return gk
 
     @staticmethod
@@ -590,7 +567,34 @@
         """
         Rounds a vector to 3 decimals
 
         :param vec: the vector to round
         :return: the rounded vector
         """
         return list(map(lambda x: round(x, 3), vec))
+
+    def get_policy(self, theta: List[float], L: int) -> Union[MultiThresholdStoppingPolicy,
+                                                              LinearThresholdStoppingPolicy]:
+        """
+        Gets the policy from a parameter vector
+
+        :param theta: the parameter vector
+        :param L: the number of parameters
+        :return: the policy object
+        """
+        if self.experiment_config.hparams[constants.T_SPSA.POLICY_TYPE] == PolicyType.MULTI_THRESHOLD:
+            policy = MultiThresholdStoppingPolicy(
+                theta=theta, simulation_name=self.simulation_env_config.name,
+                states=self.simulation_env_config.state_space_config.states,
+                player_type=self.experiment_config.player_type, L=L,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
+                agent_type=AgentType.T_SPSA)
+        else:
+            policy = LinearThresholdStoppingPolicy(
+                theta=theta, simulation_name=self.simulation_env_config.name,
+                states=self.simulation_env_config.state_space_config.states,
+                player_type=self.experiment_config.player_type, L=L,
+                actions=self.simulation_env_config.joint_action_space_config.action_spaces[
+                    self.experiment_config.player_idx].actions, experiment_config=self.experiment_config, avg_R=-1,
+                agent_type=AgentType.T_SPSA)
+        return policy
```

### Comparing `csle_agents-0.1.9/src/csle_agents/common/actor_critic_net.py` & `csle_agents-0.2.0/src/csle_agents/common/actor_critic_net.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.9/src/csle_agents/common/fnn_w_gaussian.py` & `csle_agents-0.2.0/src/csle_agents/common/fnn_w_gaussian.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.9/src/csle_agents/common/fnn_w_linear.py` & `csle_agents-0.2.0/src/csle_agents/common/fnn_w_linear.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.9/src/csle_agents/common/pruning.py` & `csle_agents-0.2.0/src/csle_agents/common/pruning.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.9/src/csle_agents/constants/constants.py` & `csle_agents-0.2.0/src/csle_agents/constants/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         "csle-stopping-game-pomdp-defender-v1"
     ]
     RUNNING_AVERAGE_INTRUSION_LENGTH = "running_average_intrusion_length"
     RUNNING_AVERAGE_INTRUSION_START = "running_average_intrusion_start"
     AVERAGE_TIME_HORIZON = "average_time_horizon"
     AVERAGE_UPPER_BOUND_RETURN = "average_upper_bound_return"
     AVERAGE_RANDOM_RETURN = "average_random_return"
+    AVERAGE_HEURISTIC_RETURN = "average_heuristic_return"
     RUNNING_AVERAGE_TIME_HORIZON = "running_average_time_horizon"
     NUM_PARALLEL_ENVS = "num_parallel_envs"
     OPTIMIZER = "optimizer"
     ADAM = "Adam"
     SGD = "SGD"
     LEARNING_RATE_EXP_DECAY = "learning_rate_exp_decay"
     LEARNING_RATE_DECAY_RATE = "learning_rate_decay_rate"
@@ -168,14 +169,15 @@
     N = "N"
     THETA1 = "theta1"
     THETAS = "thetas"
     THRESHOLDS = "thresholds"
     STOP_DISTRIBUTION_ATTACKER = "stop_distribution_attacker"
     STOP_DISTRIBUTION_DEFENDER = "stop_distribution_defender"
     DELTA = "delta"
+    POLICY_TYPE = "policy_type"
 
 
 class BAYESIAN_OPTIMIZATION:
     """
     String constants related to Bayesian Optimization
     """
     L = "L"
@@ -188,22 +190,24 @@
     STOP_DISTRIBUTION_DEFENDER = "stop_distribution_defender"
     UTILITY_FUNCTION = "utility_function"
     UCB_KAPPA = "ucb_kappa"
     UCB_XI = "ucb_xi"
     UCB = "ucb"
     TARGET = "target"
     PARAMS = "params"
+    POLICY_TYPE = "policy_type"
 
 
 class DIFFERENTIAL_EVOLUTION:
     """
     String constants related to differential evolution
     """
     L = "L"
     N = "N"
+    POLICY_TYPE = "policy_type"
     THETA1 = "theta1"
     THETAS = "thetas"
     THRESHOLDS = "thresholds"
     STOP_DISTRIBUTION_ATTACKER = "stop_distribution_attacker"
     STOP_DISTRIBUTION_DEFENDER = "stop_distribution_defender"
     POPULATION_SIZE = "population_size"
     MUTATE = "mutate"
@@ -220,14 +224,15 @@
     K = "K"
     LAMB = "lamb"
     THETA1 = "theta1"
     THETAS = "thetas"
     THRESHOLDS = "thresholds"
     STOP_DISTRIBUTION_ATTACKER = "stop_distribution_attacker"
     STOP_DISTRIBUTION_DEFENDER = "stop_distribution_defender"
+    POLICY_TYPE = "policy_type"
 
 
 class KIEFER_WOLFOWITZ:
     """
     String constants related to Kiefer-Wolfowitz
     """
     N = "N"
@@ -236,14 +241,15 @@
     THETAS = "thetas"
     THRESHOLDS = "thresholds"
     GRADIENT_BATCH_SIZE = "gradient_batch_size"
     STOP_DISTRIBUTION_ATTACKER = "stop_distribution_attacker"
     STOP_DISTRIBUTION_DEFENDER = "stop_distribution_defender"
     INITIAL_ALPHA = "initial_alpha"
     DELTA = "delta"
+    POLICY_TYPE = "policy_type"
 
 
 class Q_LEARNING:
     """
     String constants related to Q-learning
     """
     N = "N"
@@ -366,7 +372,8 @@
     STATE = "s"
     DEFENDER_ACTION = "a1"
     ATTACKER_ACTION = "a2"
     OBSERVATION = "o"
     TIME_STEP = "t"
     AVERAGE_UPPER_BOUND_RETURN = "average_upper_bound_return"
     AVERAGE_RANDOM_RETURN = "average_random_return"
+    AVERAGE_HEURISTIC_RETURN = "average_heuristic_return"
```

### Comparing `csle_agents-0.1.9/src/csle_agents/job_controllers/training_job_manager.py` & `csle_agents-0.2.0/src/csle_agents/job_controllers/training_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.9/src/csle_agents.egg-info/PKG-INFO` & `csle_agents-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: csle-agents
-Version: 0.1.9
+Name: csle_agents
+Version: 0.2.0
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.1.9/src/csle_agents.egg-info/SOURCES.txt` & `csle_agents-0.2.0/src/csle_agents.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 src/csle_agents.egg-info/dependency_links.txt
 src/csle_agents.egg-info/not-zip-safe
 src/csle_agents.egg-info/requires.txt
 src/csle_agents.egg-info/top_level.txt
 src/csle_agents/agents/__init__.py
 src/csle_agents/agents/base/__init__.py
 src/csle_agents/agents/base/base_agent.py
-src/csle_agents/agents/bayes_opt/__init__.py
-src/csle_agents/agents/bayes_opt/bayes_opt_agent.py
+src/csle_agents/agents/bayesian_optimization/__init__.py
+src/csle_agents/agents/bayesian_optimization/bayes_opt_agent.py
 src/csle_agents/agents/cross_entropy/__init__.py
 src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
 src/csle_agents/agents/differential_evolution/__init__.py
 src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
 src/csle_agents/agents/dqn/__init__.py
 src/csle_agents/agents/dqn/dqn_agent.py
 src/csle_agents/agents/dynasec/__init__.py
```

