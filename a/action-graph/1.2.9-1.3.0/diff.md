# Comparing `tmp/action-graph-1.2.9.tar.gz` & `tmp/action-graph-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action-graph-1.2.9.tar", last modified: Wed Jun 21 20:48:10 2023, max compression
+gzip compressed data, was "action-graph-1.3.0.tar", last modified: Fri Jun 23 21:32:13 2023, max compression
```

## Comparing `action-graph-1.2.9.tar` & `action-graph-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.2.9/LICENSE
--rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.2.9/README.md
--rw-r--r--   0        0        0      684 2023-06-21 20:46:34.412529 action-graph-1.2.9/action_graph/__init__.py
--rw-r--r--   0        0        0     3181 2023-06-05 00:52:07.725399 action-graph-1.2.9/action_graph/action.py
--rw-r--r--   0        0        0     9491 2023-06-16 02:52:33.411377 action-graph-1.2.9/action_graph/agent.py
--rw-r--r--   0        0        0     4691 2023-06-21 20:44:45.869031 action-graph-1.2.9/action_graph/planner.py
--rw-r--r--   0        0        0      832 2023-06-21 20:46:26.104567 action-graph-1.2.9/pyproject.toml
--rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.2.9/tests/01-redundant_precon_test.py
--rwxr-xr-x   0        0        0     1096 2023-06-16 14:35:32.753006 action-graph-1.2.9/tests/02-multi_feasible_test.py
--rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.2.9/tests/03-references_test.py
--rwxr-xr-x   0        0        0      917 2023-06-16 14:31:44.398052 action-graph-1.2.9/tests/04-loop_test.py
--rw-r--r--   0        0        0        0 2023-06-16 14:40:25.834530 action-graph-1.2.9/tests/__init__.py
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.3.0/README.md
+-rw-r--r--   0        0        0      684 2023-06-23 21:25:46.349305 action-graph-1.3.0/action_graph/__init__.py
+-rw-r--r--   0        0        0     3181 2023-06-05 00:52:07.725399 action-graph-1.3.0/action_graph/action.py
+-rw-r--r--   0        0        0    10818 2023-06-23 21:27:59.160761 action-graph-1.3.0/action_graph/agent.py
+-rw-r--r--   0        0        0     4708 2023-06-23 20:12:13.999379 action-graph-1.3.0/action_graph/planner.py
+-rw-r--r--   0        0        0      832 2023-06-23 21:26:03.705234 action-graph-1.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.3.0/tests/01-redundant_precon_test.py
+-rwxr-xr-x   0        0        0     1039 2023-06-23 21:15:35.619807 action-graph-1.3.0/tests/02-multi_feasible_test.py
+-rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.3.0/tests/03-references_test.py
+-rwxr-xr-x   0        0        0      909 2023-06-23 20:50:11.922048 action-graph-1.3.0/tests/04-loop_test.py
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.3.0/PKG-INFO
```

### Comparing `action-graph-1.2.9/LICENSE` & `action-graph-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.9/README.md` & `action-graph-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.9/action_graph/__init__.py` & `action-graph-1.3.0/action_graph/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 from action_graph.action import Action, ActionStatus, State
 from action_graph.agent import Agent
 
 name = 'action_graph'
-__version__ = '1.2.9'
+__version__ = '1.3.0'
 __all__ = [
     'State',
     'Action',
     'ActionStatus',
     'ActionFailedException',
     'ActionAbortedException',
     'ActionTimedOutException',
```

### Comparing `action-graph-1.2.9/action_graph/action.py` & `action-graph-1.3.0/action_graph/action.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.9/action_graph/agent.py` & `action-graph-1.3.0/action_graph/agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python3
 
 import logging
 from time import sleep, time
-from typing import List
+from typing import Iterable, List
 
 from action_graph.action import (Action, ActionStatus, State,
                                  ActionTimedOutException, ActionAbortedException, ActionFailedException)
 from action_graph.planner import Planner, PlanningFailedException
 
 
 class Agent:
@@ -17,22 +17,24 @@
 
     def __init__(self, agent_name=None) -> None:
         if not agent_name:
             agent_name = self.__class__.__name__
         self.name = agent_name
         #
         self.state: State = {}
+        self.__actions: List[Action] = []
 
     def load_actions(self, actions: List[Action]):
         """
         Load actions list; refresh in case of any changes to the actions data.
 
         :param actions:List[Action]: List of actions.
         """
 
+        self.__actions = actions
         self.__planner.update_actions(actions)
 
     def update_state(self, state: State):
         """
         Updates system state with the incoming state.        
 
         :param state:State: New state
@@ -118,65 +120,85 @@
         """
         Creates a plan to satisfy the goal state; executes it action-by-action; re-evaluates the plan at each step;
 
         :param goal:State: Desired goal state
         :param verbose:bool: Print plan to console at each step, if True
         """
 
-        __actions_to_avoid: List[str] = []
+        blacklisted_actions: List[str] = []
 
         # state might have changed since the last step was executed
         while not self.is_goal_met(goal):
 
             try:
                 # (re)generate the plan
-                plan: List[Action] = self.__planner.generate_plan(goal, self.state, __actions_to_avoid)
+                plan: List[Action] = self.__planner.generate_plan(goal, self.state, blacklisted_actions)
                 if verbose:
                     self.print_plan_to_console(plan)
                 # execute one plan step at a time
-                __action = plan[0]
-                self.execute_action(__action)
+                first_action = plan[0]
+                self.execute_action(first_action)
+
+                # if the latest executed action has the same effect as any of the blacklisted actions,
+                # then it is prudent(?) to remove such a blacklisted action
+                ba: List[Action] = [a for a in self.__actions if str(a) in blacklisted_actions]
+                for action in ba:
+                    if set(first_action.effects.keys()) <= set(action.effects.keys()):
+                        blacklisted_actions.remove(str(action))
 
             except ActionFailedException as ex_fail:
                 logging.error(f"{ex_fail} / ATTEMPTING ALTERNATIVE PLAN")
-                __action_name = str(__action)
-                if __action_name not in __actions_to_avoid:
-                    __actions_to_avoid.append(__action_name)
+                __action_name = str(first_action)
+                if __action_name not in blacklisted_actions:
+                    blacklisted_actions.append(__action_name)
                 continue
 
             except Exception as _ex:
                 logging.error(f"{_ex}")
                 raise
 
         logging.info(f"EXECUTION SUCCEDED!")
 
-    def achieve_goal_interactive(self, goal: State):
+    def plan_and_execute(self, goal: State, verbose: bool = False) -> Iterable:
         """
         Creates a plan to satisfy the goal state; executes it action-by-action; re-evaluates the plan at each step;
 
         :param goal:State: Desired goal state
+        :param verbose:bool: if True, prints formatted plan to console at each step
         """
 
-        __actions_to_avoid: List[str] = []
+        blacklisted_actions: List[str] = []
 
         # state might have changed since the last step was executed
         while not self.is_goal_met(goal):
 
             try:
                 # (re)generate the plan
-                plan: List[Action] = self.__planner.generate_plan(goal, self.state, __actions_to_avoid)
-                yield plan
+                plan: List[Action] = self.__planner.generate_plan(goal, self.state, blacklisted_actions)
+                # print formatted plan to console
+                if verbose:
+                    self.print_plan_to_console(plan)
+
+                yield plan  # yields plan before execution
+
                 # execute one plan step at a time
-                self.execute_action(plan[0])
+                first_action = plan[0]
+                self.execute_action(first_action)
+                #
+                # if the latest executed action has the same effect as any of the blacklisted actions,
+                # then it is prudent(?) to remove such a blacklisted action
+                ba: List[Action] = [a for a in self.__actions if str(a) in blacklisted_actions]
+                for action in ba:
+                    if set(first_action.effects.keys()) <= set(action.effects.keys()):
+                        blacklisted_actions.remove(str(action))
 
             except ActionFailedException as ex_fail:
                 logging.error(f"{ex_fail} / ATTEMPTING ALTERNATIVE PLAN")
-                __action_name = str(plan[0])
-                if __action_name not in __actions_to_avoid:
-                    __actions_to_avoid.append(__action_name)
+                if str(first_action) not in blacklisted_actions:
+                    blacklisted_actions.append(str(first_action))
                 continue
 
             except Exception as _ex:
                 logging.error(f"{_ex}")
                 raise
 
         logging.info(f"EXECUTION SUCCEDED!")
```

### Comparing `action-graph-1.2.9/action_graph/planner.py` & `action-graph-1.3.0/action_graph/planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         :param target_state:State: Desired goal (target) state
         :param start_state:State: Current/start state of the system
         :return:List[Action]: List of actions updated with their expected outcomes (effects)
         """
 
         if len(target_state.items()) > 1:
-            raise PlanningFailedException('target_state should have a single state variable')
+            raise PlanningFailedException(f'target_state [{target_state}] should be a single state')
         tk, tv = list(target_state.items())[0]
         # in case target state value is a reference to another state variable
         if isinstance(tv, str) and tv[0] == '@':
             tv = self.__parse_references(tv, start_state)
         # check if the target state is already satisfied
         if (tk, tv) in list(start_state.items()):
             return []   # goal already met, move on
@@ -64,15 +64,15 @@
             action_path: List[Action] = []
             for pk, pv in action.preconditions.items():  # for each pre-condition ...
                 try:  # choose the shortest feasible path
                     if isinstance(pv, str) and pv[0] == '$':
                         pv = self.__parse_references(pv, action.effects)
                     action_path += self.generate_plan({pk: pv}, start_state, avoid_actions)  # merge the actions
                 except RecursionError:  # watch out for cyclic references
-                    raise PlanningFailedException(f'Found cyclic references!')
+                    raise PlanningFailedException(f'Found cyclic references! {pk}:{pv}')
             # include the current action;  remove duplicates; keep the order intact
             action_path = self.__make_unique(action_path + [action])
             #
             if not chosen_path:  # if no other path is available...
                 chosen_path = action_path  # use the current path
                 continue
             # if alternative paths exist, use the one with the lowest cost
```

### Comparing `action-graph-1.2.9/pyproject.toml` & `action-graph-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 authors = [
     { name = "Bharath Achyutha Rao", email = "bharath.rao@hotmail.com" },
 ]
 name = "action_graph"
-version = "1.2.9"
+version = "1.3.0"
 description = "Autonomous agent for task/action planning and execution"
 readme = "README.md"
 requires-python = ">=3.7,<4.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `action-graph-1.2.9/tests/01-redundant_precon_test.py` & `action-graph-1.3.0/tests/01-redundant_precon_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.9/tests/02-multi_feasible_test.py` & `action-graph-1.3.0/tests/03-references_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 #! /usr/bin/env python3
 
 from action_graph.action import Action
 from action_graph.agent import Agent
 
 
-class ActionA(Action):
+class Action5(Action):
+    effects = {"FINAL": True}
+    preconditions = {"FIRST": True, "FOURTH": "TESTSTATE"}
+
+
+class Action1(Action):
     effects = {"FIRST": True}
-    preconditions = {}
+    preconditions = {"FIRST": False}
 
 
-class ActionB1(Action):
-    effects = {"SECOND": True}
-    preconditions = {"FIRST": True}
+class Action4(Action):
+    effects = {"FOURTH": ...}
+    preconditions = {
+        "SECOND": "$FOURTH",
+        "THIRD": "$FOURTH",
+    }
 
 
-class ActionB2(Action):
-    effects = {"SECOND": True}
+class Action2(Action):
+    effects = {"SECOND": ...}
     preconditions = {}
-    cost = 1.5
 
 
-class ActionC(Action):
-    effects = {"THIRD": True}
-    preconditions = {"FIRST": True, "SECOND": True}
+class Action3(Action):
+    effects = {"THIRD": ...}
+    preconditions = {}
 
 
 def test():
-    world_state = {"FIRST": False, "SECOND": False, "THIRD": False}
-    goal_state = {"THIRD": True}
+    world_state = {"FINAL": False, "FIRST": False}
+    goal_state = {"FINAL": True}
 
     ai = Agent()
 
     actions = [a(ai) for a in Action.__subclasses__()]
     ai.load_actions(actions)
     ai.update_state(world_state)
     plan = ai.get_plan(goal_state)
 
-    expected_actions = ["ActionA", "ActionB2", "ActionC"]
-    expected_outcome = [{'FIRST': True}, {'SECOND': True}, {'THIRD': True}]
+    expected_actions = ["Action1", "Action2", "Action3", "Action4", "Action5"]
+    expected_outcome = [{'FIRST': True}, {'SECOND': 'TESTSTATE'}, {'THIRD': 'TESTSTATE'}, {'FOURTH': 'TESTSTATE'}, {'FINAL': True}]
 
     for ax, eax, eoc in zip(plan, expected_actions, expected_outcome):
         assert ax.__class__.__name__ == eax, f'Incorrect Action!'
         assert ax.effects == eoc, f'Incorrect Action Outcome!'
```

### Comparing `action-graph-1.2.9/tests/04-loop_test.py` & `action-graph-1.3.0/tests/04-loop_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,11 +20,11 @@
     world_state = {"fibonacci_sum": 0, "counter": 0}
     goal_state = {"counter": 10}
 
     ai = Agent()
     actions = [a(ai) for a in Action.__subclasses__()]
     ai.load_actions(actions)
     ai.update_state(world_state)
-    for plan in ai.achieve_goal_interactive(goal_state):
+    for plan in ai.plan_and_execute(goal_state):
         pass
 
     assert ai.state["fibonacci_sum"] == 55, f'Looping feature broken!'
```

### Comparing `action-graph-1.2.9/PKG-INFO` & `action-graph-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action_graph
-Version: 1.2.9
+Version: 1.3.0
 Summary: Autonomous agent for task/action planning and execution
 Author-email: Bharath Achyutha Rao <bharath.rao@hotmail.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Bug Tracker, https://github.com/bharathra/action_graph/issues
```

