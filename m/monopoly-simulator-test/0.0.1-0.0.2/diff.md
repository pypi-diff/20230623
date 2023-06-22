# Comparing `tmp/monopoly_simulator_test-0.0.1.tar.gz` & `tmp/monopoly_simulator_test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/monopoly_simulator_test-0.0.1.tar", last modified: Thu Jun 22 23:20:32 2023, max compression
+gzip compressed data, was "dist/monopoly_simulator_test-0.0.2.tar", last modified: Thu Jun 22 23:23:13 2023, max compression
```

## Comparing `monopoly_simulator_test-0.0.1.tar` & `monopoly_simulator_test-0.0.2.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 mchiu      (502) staff       (20)        0 2023-06-22 23:20:32.000000 monopoly_simulator_test-0.0.1/
--rw-r--r--   0 mchiu      (502) staff       (20)      281 2023-06-22 23:20:32.000000 monopoly_simulator_test-0.0.1/PKG-INFO
--rw-rw-r--   0 mchiu      (502) staff       (20)     3962 2022-05-29 19:01:10.000000 monopoly_simulator_test-0.0.1/README.md
-drwxr-xr-x   0 mchiu      (502) staff       (20)        0 2023-06-22 23:20:32.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/
--rw-rw-r--   0 mchiu      (502) staff       (20)        0 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/__init__.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    93000 2022-08-22 17:17:03.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/action_choices.py
--rw-rw-r--   0 mchiu      (502) staff       (20)     4132 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/agent.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    52515 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/agent_helper_functions.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    62820 2022-08-03 22:54:10.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/agent_helper_functions_v2.py
--rw-r--r--   0 mchiu      (502) staff       (20)    93157 2022-09-01 23:52:33.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/agent_helper_functions_v3.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    48196 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v1_2.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    62213 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    69238 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_action_novelty.py
--rw-r--r--   0 mchiu      (502) staff       (20)    45535 2022-10-28 19:10:12.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_cash_conservator.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    63926 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_interaction_accept_offer.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    63476 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_interaction_make_offer.py
--rw-r--r--   0 mchiu      (502) staff       (20)    64468 2022-08-31 18:52:59.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_railroad_chaser.py
--rw-r--r--   0 mchiu      (502) staff       (20)    64430 2022-09-01 18:26:51.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_sneaky_trader.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    63672 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_2.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    57599 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v4_1.py
--rw-r--r--   0 mchiu      (502) staff       (20)    51289 2022-08-31 23:25:50.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_others.py
--rw-r--r--   0 mchiu      (502) staff       (20)    61939 2022-05-08 02:36:24.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_ta2.py
--rw-r--r--   0 mchiu      (502) staff       (20)    62058 2023-05-03 19:56:29.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_wealthy.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    57489 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v5_1.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    12735 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/bank.py
--rw-rw-r--   0 mchiu      (502) staff       (20)     9140 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/card.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    44371 2022-08-22 17:42:07.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/card_utility_actions.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    15785 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/client_agent.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    19948 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/client_agent_serial.py
--rw-rw-r--   0 mchiu      (502) staff       (20)     3784 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/diagnostics.py
--rw-rw-r--   0 mchiu      (502) staff       (20)     1174 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/dice.py
--rw-r--r--   0 mchiu      (502) staff       (20)      411 2023-06-21 23:04:21.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/execute_phase3.py
--rw-rw-r--   0 mchiu      (502) staff       (20)      140 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/flag_config.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    34780 2022-09-06 19:55:00.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/gameplay.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    38357 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/gameplay_GUI.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    44172 2022-08-17 19:22:04.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/gameplay_socket.py
--rw-r--r--   0 mchiu      (502) staff       (20)    53209 2023-06-22 22:36:33.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/gameplay_socket_phase3.py
--rw-r--r--   0 mchiu      (502) staff       (20)    46023 2022-11-15 19:31:09.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/gameplay_socket_ta2.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    17190 2022-08-19 17:59:59.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/initialize_game_elements.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    25167 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/location.py
--rw-rw-r--   0 mchiu      (502) staff       (20)     7339 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/log_metrics.py
--rw-rw-r--   0 mchiu      (502) staff       (20)      662 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/logging_info.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    19355 2022-05-29 19:01:10.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/monopoly_game_schema_v1-2.json
--rw-rw-r--   0 mchiu      (502) staff       (20)    27643 2022-06-14 21:03:52.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_distributions_v2.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    74636 2022-06-14 06:54:08.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_distributions_v3.py
--rw-rw-r--   0 mchiu      (502) staff       (20)     1269 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_functions.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    84750 2022-05-29 18:43:24.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_functions_v2.py
--rw-rw-r--   0 mchiu      (502) staff       (20)   529178 2022-10-12 23:00:30.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_functions_v3.py
--rw-r--r--   0 mchiu      (502) staff       (20)     7978 2023-06-22 23:05:46.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_generation_phase3.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    21633 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_generator.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    46891 2023-04-20 01:11:04.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_generator_v2.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    44416 2023-04-20 19:51:24.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_generator_v3.py
--rw-r--r--   0 mchiu      (502) staff       (20)    20257 2022-10-27 17:37:53.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/phase3_novelty_config.json
--rw-rw-r--   0 mchiu      (502) staff       (20)    89356 2022-11-29 17:36:40.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/player.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    36160 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/read_write_current_state.py
--rw-rw-r--   0 mchiu      (502) staff       (20)     1155 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/scratchpad.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    17457 2023-05-03 20:01:02.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/serialization.py
--rw-rw-r--   0 mchiu      (502) staff       (20)     5370 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/server_agent.py
--rw-rw-r--   0 mchiu      (502) staff       (20)    13836 2022-10-12 20:10:57.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/server_agent_serial.py
--rw-r--r--   0 mchiu      (502) staff       (20)    11975 2023-05-03 20:30:04.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/test_harness_phase3.py
--rw-r--r--   0 mchiu      (502) staff       (20)    14203 2023-05-03 21:42:31.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/test_harness_phase3_goals.py
--rw-r--r--   0 mchiu      (502) staff       (20)    12856 2023-06-21 18:04:56.000000 monopoly_simulator_test-0.0.1/monopoly_simulator/test_harness_phase3_test.py
-drwxr-xr-x   0 mchiu      (502) staff       (20)        0 2023-06-22 23:20:32.000000 monopoly_simulator_test-0.0.1/monopoly_simulator_test.egg-info/
--rw-r--r--   0 mchiu      (502) staff       (20)      281 2023-06-22 23:20:32.000000 monopoly_simulator_test-0.0.1/monopoly_simulator_test.egg-info/PKG-INFO
--rw-r--r--   0 mchiu      (502) staff       (20)     2753 2023-06-22 23:20:32.000000 monopoly_simulator_test-0.0.1/monopoly_simulator_test.egg-info/SOURCES.txt
--rw-r--r--   0 mchiu      (502) staff       (20)        1 2023-06-22 23:20:32.000000 monopoly_simulator_test-0.0.1/monopoly_simulator_test.egg-info/dependency_links.txt
--rw-r--r--   0 mchiu      (502) staff       (20)       19 2023-06-22 23:20:32.000000 monopoly_simulator_test-0.0.1/monopoly_simulator_test.egg-info/top_level.txt
--rw-r--r--   0 mchiu      (502) staff       (20)       38 2023-06-22 23:20:32.000000 monopoly_simulator_test-0.0.1/setup.cfg
--rw-r--r--   0 mchiu      (502) staff       (20)      706 2023-06-22 23:20:23.000000 monopoly_simulator_test-0.0.1/setup.py
+drwxr-xr-x   0 mchiu      (502) staff       (20)        0 2023-06-22 23:23:13.000000 monopoly_simulator_test-0.0.2/
+-rw-r--r--   0 mchiu      (502) staff       (20)      281 2023-06-22 23:23:13.000000 monopoly_simulator_test-0.0.2/PKG-INFO
+-rw-rw-r--   0 mchiu      (502) staff       (20)     3962 2022-05-29 19:01:10.000000 monopoly_simulator_test-0.0.2/README.md
+drwxr-xr-x   0 mchiu      (502) staff       (20)        0 2023-06-22 23:23:13.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/
+-rw-rw-r--   0 mchiu      (502) staff       (20)        0 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/__init__.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    93000 2022-08-22 17:17:03.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/action_choices.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)     4132 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/agent.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    52515 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/agent_helper_functions.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    62820 2022-08-03 22:54:10.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/agent_helper_functions_v2.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    93157 2022-09-01 23:52:33.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/agent_helper_functions_v3.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    48196 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v1_2.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    62213 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    69238 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_action_novelty.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    45535 2022-10-28 19:10:12.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_cash_conservator.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    63926 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_interaction_accept_offer.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    63476 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_interaction_make_offer.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    64468 2022-08-31 18:52:59.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_railroad_chaser.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    64430 2022-09-01 18:26:51.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_sneaky_trader.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    63672 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_2.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    57599 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v4_1.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    51289 2022-08-31 23:25:50.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_others.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    61939 2022-05-08 02:36:24.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_ta2.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    62058 2023-05-03 19:56:29.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_wealthy.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    57489 2022-08-16 18:01:05.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v5_1.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    12735 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/bank.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)     9140 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/card.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    44371 2022-08-22 17:42:07.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/card_utility_actions.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    15785 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/client_agent.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    19948 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/client_agent_serial.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)     3784 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/diagnostics.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)     1174 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/dice.py
+-rw-r--r--   0 mchiu      (502) staff       (20)      411 2023-06-21 23:04:21.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/execute_phase3.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)      140 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/flag_config.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    34780 2022-09-06 19:55:00.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/gameplay.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    38357 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/gameplay_GUI.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    44172 2022-08-17 19:22:04.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/gameplay_socket.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    53209 2023-06-22 22:36:33.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/gameplay_socket_phase3.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    46023 2022-11-15 19:31:09.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/gameplay_socket_ta2.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    17190 2022-08-19 17:59:59.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/initialize_game_elements.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    25167 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/location.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)     7339 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/log_metrics.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)      662 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/logging_info.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    19355 2022-05-29 19:01:10.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/monopoly_game_schema_v1-2.json
+-rw-rw-r--   0 mchiu      (502) staff       (20)    27643 2022-06-14 21:03:52.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_distributions_v2.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    74636 2022-06-14 06:54:08.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_distributions_v3.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)     1269 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_functions.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    84750 2022-05-29 18:43:24.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_functions_v2.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)   529178 2022-10-12 23:00:30.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_functions_v3.py
+-rw-r--r--   0 mchiu      (502) staff       (20)     7978 2023-06-22 23:05:46.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_generation_phase3.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    21633 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_generator.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    46891 2023-04-20 01:11:04.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_generator_v2.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    44416 2023-04-20 19:51:24.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_generator_v3.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    20257 2022-10-27 17:37:53.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/phase3_novelty_config.json
+-rw-rw-r--   0 mchiu      (502) staff       (20)    89356 2022-11-29 17:36:40.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/player.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    36160 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/read_write_current_state.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)     1155 2022-05-31 17:40:56.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/scratchpad.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    17457 2023-05-03 20:01:02.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/serialization.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)     5370 2022-05-31 17:40:58.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/server_agent.py
+-rw-rw-r--   0 mchiu      (502) staff       (20)    13836 2022-10-12 20:10:57.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/server_agent_serial.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    11975 2023-05-03 20:30:04.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/test_harness_phase3.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    14203 2023-05-03 21:42:31.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/test_harness_phase3_goals.py
+-rw-r--r--   0 mchiu      (502) staff       (20)    12856 2023-06-21 18:04:56.000000 monopoly_simulator_test-0.0.2/monopoly_simulator/test_harness_phase3_test.py
+drwxr-xr-x   0 mchiu      (502) staff       (20)        0 2023-06-22 23:23:13.000000 monopoly_simulator_test-0.0.2/monopoly_simulator_test.egg-info/
+-rw-r--r--   0 mchiu      (502) staff       (20)      281 2023-06-22 23:23:13.000000 monopoly_simulator_test-0.0.2/monopoly_simulator_test.egg-info/PKG-INFO
+-rw-r--r--   0 mchiu      (502) staff       (20)     2799 2023-06-22 23:23:13.000000 monopoly_simulator_test-0.0.2/monopoly_simulator_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mchiu      (502) staff       (20)        1 2023-06-22 23:23:13.000000 monopoly_simulator_test-0.0.2/monopoly_simulator_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mchiu      (502) staff       (20)       17 2023-06-22 23:23:13.000000 monopoly_simulator_test-0.0.2/monopoly_simulator_test.egg-info/requires.txt
+-rw-r--r--   0 mchiu      (502) staff       (20)       19 2023-06-22 23:23:13.000000 monopoly_simulator_test-0.0.2/monopoly_simulator_test.egg-info/top_level.txt
+-rw-r--r--   0 mchiu      (502) staff       (20)       38 2023-06-22 23:23:13.000000 monopoly_simulator_test-0.0.2/setup.cfg
+-rw-r--r--   0 mchiu      (502) staff       (20)      754 2023-06-22 23:23:04.000000 monopoly_simulator_test-0.0.2/setup.py
```

### Comparing `monopoly_simulator_test-0.0.1/README.md` & `monopoly_simulator_test-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/action_choices.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/action_choices.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/agent.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/agent.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/agent_helper_functions.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/agent_helper_functions.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/agent_helper_functions_v2.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/agent_helper_functions_v2.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/agent_helper_functions_v3.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/agent_helper_functions_v3.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v1_2.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v1_2.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_action_novelty.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_action_novelty.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_cash_conservator.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_cash_conservator.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_interaction_accept_offer.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_interaction_accept_offer.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_interaction_make_offer.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_interaction_make_offer.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_railroad_chaser.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_railroad_chaser.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_1_sneaky_trader.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_1_sneaky_trader.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v3_2.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v3_2.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v4_1.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v4_1.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_others.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_others.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_ta2.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_ta2.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_wealthy.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v4_1_avoid_accept_trade_with_wealthy.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/background_agent_v5_1.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/background_agent_v5_1.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/bank.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/bank.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/card.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/card.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/card_utility_actions.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/card_utility_actions.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/client_agent.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/client_agent.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/client_agent_serial.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/client_agent_serial.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/diagnostics.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/diagnostics.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/dice.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/dice.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/gameplay.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/gameplay.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/gameplay_GUI.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/gameplay_GUI.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/gameplay_socket.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/gameplay_socket.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/gameplay_socket_phase3.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/gameplay_socket_phase3.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/gameplay_socket_ta2.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/gameplay_socket_ta2.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/initialize_game_elements.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/initialize_game_elements.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/location.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/location.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/log_metrics.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/log_metrics.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/logging_info.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/logging_info.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/monopoly_game_schema_v1-2.json` & `monopoly_simulator_test-0.0.2/monopoly_simulator/monopoly_game_schema_v1-2.json`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_distributions_v2.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_distributions_v2.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_distributions_v3.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_distributions_v3.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_functions.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_functions.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_functions_v2.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_functions_v2.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_functions_v3.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_functions_v3.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_generation_phase3.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_generation_phase3.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_generator.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_generator.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_generator_v2.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_generator_v2.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/novelty_generator_v3.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/novelty_generator_v3.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/phase3_novelty_config.json` & `monopoly_simulator_test-0.0.2/monopoly_simulator/phase3_novelty_config.json`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/player.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/player.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/read_write_current_state.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/read_write_current_state.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/scratchpad.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/scratchpad.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/serialization.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/serialization.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/server_agent.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/server_agent.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/server_agent_serial.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/server_agent_serial.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/test_harness_phase3.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/test_harness_phase3.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/test_harness_phase3_goals.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/test_harness_phase3_goals.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator/test_harness_phase3_test.py` & `monopoly_simulator_test-0.0.2/monopoly_simulator/test_harness_phase3_test.py`

 * *Files identical despite different names*

### Comparing `monopoly_simulator_test-0.0.1/monopoly_simulator_test.egg-info/SOURCES.txt` & `monopoly_simulator_test-0.0.2/monopoly_simulator_test.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,8 +57,9 @@
 monopoly_simulator/server_agent_serial.py
 monopoly_simulator/test_harness_phase3.py
 monopoly_simulator/test_harness_phase3_goals.py
 monopoly_simulator/test_harness_phase3_test.py
 monopoly_simulator_test.egg-info/PKG-INFO
 monopoly_simulator_test.egg-info/SOURCES.txt
 monopoly_simulator_test.egg-info/dependency_links.txt
+monopoly_simulator_test.egg-info/requires.txt
 monopoly_simulator_test.egg-info/top_level.txt
```

### Comparing `monopoly_simulator_test-0.0.1/setup.py` & `monopoly_simulator_test-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from distutils.core import setup
 import setuptools
 
 setup(name='monopoly_simulator_test',
-      version='0.0.1',
+      version='0.0.2',
       description='USC/ISI monopoly simulator',
       author='Min-Hsueh Chiu',
       author_email='minhsueh@isi.edu',
       url = "https://github.com/mayankkejriwal/GNOME-p3/tree/phase3_simulator_v1",
       #packages=['monopoly'],
       #package_dir={'monopoly': 'monopoly/monopoly_simulator'},
       #package_data={'monopoly': ['./*.json']},
       packages=setuptools.find_packages(),
       data_files=[
             ('', ['monopoly_simulator/monopoly_game_schema_v1-2.json']),
             ('', ['monopoly_simulator/phase3_novelty_config.json'])
       ],
-      include_package_data=True
+      include_package_data=True,
+      install_requires=['numpy', 'xlsxwriter']
      )
```

