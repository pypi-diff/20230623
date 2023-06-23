# Comparing `tmp/replay_trajectory_classification-1.3.8.tar.gz` & `tmp/replay_trajectory_classification-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replay_trajectory_classification-1.3.8.tar", last modified: Wed Dec  7 17:26:41 2022, max compression
+gzip compressed data, was "replay_trajectory_classification-1.3.9.tar", last modified: Mon Feb 20 02:05:06 2023, max compression
```

## Comparing `replay_trajectory_classification-1.3.8.tar` & `replay_trajectory_classification-1.3.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2022-12-07 17:26:41.920217 replay_trajectory_classification-1.3.8/
--rw-r--r--   0 edeno      (501) staff       (20)     1071 2019-03-15 14:05:27.000000 replay_trajectory_classification-1.3.8/LICENSE
--rw-r--r--   0 edeno      (501) staff       (20)      292 2022-12-07 17:26:41.919979 replay_trajectory_classification-1.3.8/PKG-INFO
--rw-r--r--   0 edeno      (501) staff       (20)     5835 2022-12-06 19:43:52.000000 replay_trajectory_classification-1.3.8/README.md
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2022-12-07 17:26:41.916481 replay_trajectory_classification-1.3.8/replay_trajectory_classification/
--rw-r--r--   0 edeno      (501) staff       (20)     1038 2022-12-07 17:26:20.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/__init__.py
--rw-r--r--   0 edeno      (501) staff       (20)    37003 2022-12-07 16:53:59.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/classifier.py
--rw-r--r--   0 edeno      (501) staff       (20)     8197 2022-12-07 16:54:35.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/clusterless_simulation.py
--rw-r--r--   0 edeno      (501) staff       (20)    10051 2022-12-07 17:01:30.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/continuous_state_transitions.py
--rw-r--r--   0 edeno      (501) staff       (20)    15945 2022-12-07 16:55:17.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/core.py
--rw-r--r--   0 edeno      (501) staff       (20)    16541 2022-12-07 16:55:39.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/decoder.py
--rw-r--r--   0 edeno      (501) staff       (20)     4369 2022-12-07 16:56:10.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/discrete_state_transitions.py
--rw-r--r--   0 edeno      (501) staff       (20)    30141 2022-12-07 17:02:21.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/environments.py
--rw-r--r--   0 edeno      (501) staff       (20)     1793 2022-12-07 17:01:08.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/initial_conditions.py
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2022-12-07 17:26:41.919789 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/
--rw-r--r--   0 edeno      (501) staff       (20)     2472 2022-09-29 22:46:14.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/__init__.py
--rw-r--r--   0 edeno      (501) staff       (20)     7849 2022-09-29 22:46:14.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/calcium_likelihood.py
--rw-r--r--   0 edeno      (501) staff       (20)     2290 2022-09-29 22:46:14.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/diffusion.py
--rw-r--r--   0 edeno      (501) staff       (20)    15765 2022-10-07 15:01:47.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood.py
--rw-r--r--   0 edeno      (501) staff       (20)    17934 2022-10-07 15:01:47.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood_gpu.py
--rw-r--r--   0 edeno      (501) staff       (20)    16202 2022-10-07 15:01:47.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer.py
--rw-r--r--   0 edeno      (501) staff       (20)    18402 2022-10-07 15:01:47.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer_gpu.py
--rw-r--r--   0 edeno      (501) staff       (20)    19912 2022-10-07 15:01:47.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer_gpu_log.py
--rw-r--r--   0 edeno      (501) staff       (20)     3674 2022-10-01 17:57:03.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood_track_graph.py
--rw-r--r--   0 edeno      (501) staff       (20)     7474 2022-09-29 22:46:14.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/spiking_likelihood_glm.py
--rw-r--r--   0 edeno      (501) staff       (20)     9788 2022-10-30 16:30:07.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/spiking_likelihood_kde.py
--rw-r--r--   0 edeno      (501) staff       (20)    11313 2022-10-30 16:30:07.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/spiking_likelihood_kde_gpu.py
--rw-r--r--   0 edeno      (501) staff       (20)      298 2022-12-07 17:02:58.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/observation_model.py
--rw-r--r--   0 edeno      (501) staff       (20)     6205 2022-12-07 17:03:40.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/simulate.py
--rw-r--r--   0 edeno      (501) staff       (20)     7730 2022-12-07 17:04:07.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/sorted_spikes_simulation.py
--rw-r--r--   0 edeno      (501) staff       (20)    10259 2022-12-07 17:04:18.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification/standard_decoder.py
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2022-12-07 17:26:41.917147 replay_trajectory_classification-1.3.8/replay_trajectory_classification.egg-info/
--rw-r--r--   0 edeno      (501) staff       (20)      292 2022-12-07 17:26:41.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification.egg-info/PKG-INFO
--rw-r--r--   0 edeno      (501) staff       (20)     1851 2022-12-07 17:26:41.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification.egg-info/SOURCES.txt
--rw-r--r--   0 edeno      (501) staff       (20)        1 2022-12-07 17:26:41.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification.egg-info/dependency_links.txt
--rw-r--r--   0 edeno      (501) staff       (20)      157 2022-12-07 17:26:41.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification.egg-info/requires.txt
--rw-r--r--   0 edeno      (501) staff       (20)       33 2022-12-07 17:26:41.000000 replay_trajectory_classification-1.3.8/replay_trajectory_classification.egg-info/top_level.txt
--rw-r--r--   0 edeno      (501) staff       (20)       38 2022-12-07 17:26:41.920277 replay_trajectory_classification-1.3.8/setup.cfg
--rw-r--r--   0 edeno      (501) staff       (20)     1329 2022-12-07 17:18:13.000000 replay_trajectory_classification-1.3.8/setup.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-02-20 02:05:06.103158 replay_trajectory_classification-1.3.9/
+-rw-r--r--   0 edeno      (501) staff       (20)     1071 2019-03-15 14:05:27.000000 replay_trajectory_classification-1.3.9/LICENSE
+-rw-r--r--   0 edeno      (501) staff       (20)      292 2023-02-20 02:05:06.102940 replay_trajectory_classification-1.3.9/PKG-INFO
+-rw-r--r--   0 edeno      (501) staff       (20)     5835 2022-12-06 19:43:52.000000 replay_trajectory_classification-1.3.9/README.md
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-02-20 02:05:06.099121 replay_trajectory_classification-1.3.9/replay_trajectory_classification/
+-rw-r--r--   0 edeno      (501) staff       (20)     1038 2023-02-20 01:46:34.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/__init__.py
+-rw-r--r--   0 edeno      (501) staff       (20)    49644 2023-02-20 01:39:15.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/classifier.py
+-rw-r--r--   0 edeno      (501) staff       (20)    12825 2022-12-12 15:51:50.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/clusterless_simulation.py
+-rw-r--r--   0 edeno      (501) staff       (20)    13794 2022-12-08 19:45:42.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/continuous_state_transitions.py
+-rw-r--r--   0 edeno      (501) staff       (20)    17550 2023-02-20 01:39:15.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/core.py
+-rw-r--r--   0 edeno      (501) staff       (20)    23259 2023-02-20 01:39:14.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/decoder.py
+-rw-r--r--   0 edeno      (501) staff       (20)     4818 2023-02-20 01:39:15.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/discrete_state_transitions.py
+-rw-r--r--   0 edeno      (501) staff       (20)    32877 2022-12-09 02:36:41.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/environments.py
+-rw-r--r--   0 edeno      (501) staff       (20)     2660 2022-12-08 19:41:20.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/initial_conditions.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-02-20 02:05:06.102710 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/
+-rw-r--r--   0 edeno      (501) staff       (20)     2669 2022-12-08 21:21:22.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/__init__.py
+-rw-r--r--   0 edeno      (501) staff       (20)     8387 2022-12-09 01:53:18.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/calcium_likelihood.py
+-rw-r--r--   0 edeno      (501) staff       (20)     2574 2022-12-09 01:55:17.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/diffusion.py
+-rw-r--r--   0 edeno      (501) staff       (20)    16688 2023-02-20 01:39:15.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood.py
+-rw-r--r--   0 edeno      (501) staff       (20)    19158 2023-02-20 01:39:15.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood_gpu.py
+-rw-r--r--   0 edeno      (501) staff       (20)    17137 2023-02-20 01:39:15.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer.py
+-rw-r--r--   0 edeno      (501) staff       (20)    19370 2023-02-20 01:39:15.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer_gpu.py
+-rw-r--r--   0 edeno      (501) staff       (20)    19912 2023-02-20 01:39:15.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer_gpu_log.py
+-rw-r--r--   0 edeno      (501) staff       (20)     3674 2022-10-01 17:57:03.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood_track_graph.py
+-rw-r--r--   0 edeno      (501) staff       (20)     8067 2023-02-20 01:39:15.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/spiking_likelihood_glm.py
+-rw-r--r--   0 edeno      (501) staff       (20)    10615 2023-02-20 01:39:15.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/spiking_likelihood_kde.py
+-rw-r--r--   0 edeno      (501) staff       (20)    12225 2023-02-20 01:49:08.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/spiking_likelihood_kde_gpu.py
+-rw-r--r--   0 edeno      (501) staff       (20)      407 2022-12-08 19:41:57.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/observation_model.py
+-rw-r--r--   0 edeno      (501) staff       (20)     6863 2022-12-12 16:01:42.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/simulate.py
+-rw-r--r--   0 edeno      (501) staff       (20)    12245 2022-12-12 15:48:12.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/sorted_spikes_simulation.py
+-rw-r--r--   0 edeno      (501) staff       (20)    10259 2022-12-07 17:04:18.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification/standard_decoder.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-02-20 02:05:06.100021 replay_trajectory_classification-1.3.9/replay_trajectory_classification.egg-info/
+-rw-r--r--   0 edeno      (501) staff       (20)      292 2023-02-20 02:05:06.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification.egg-info/PKG-INFO
+-rw-r--r--   0 edeno      (501) staff       (20)     1851 2023-02-20 02:05:06.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification.egg-info/SOURCES.txt
+-rw-r--r--   0 edeno      (501) staff       (20)        1 2023-02-20 02:05:06.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification.egg-info/dependency_links.txt
+-rw-r--r--   0 edeno      (501) staff       (20)      157 2023-02-20 02:05:06.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification.egg-info/requires.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       33 2023-02-20 02:05:06.000000 replay_trajectory_classification-1.3.9/replay_trajectory_classification.egg-info/top_level.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       38 2023-02-20 02:05:06.103207 replay_trajectory_classification-1.3.9/setup.cfg
+-rw-r--r--   0 edeno      (501) staff       (20)     1329 2022-12-09 15:34:32.000000 replay_trajectory_classification-1.3.9/setup.py
```

### Comparing `replay_trajectory_classification-1.3.8/LICENSE` & `replay_trajectory_classification-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `replay_trajectory_classification-1.3.8/README.md` & `replay_trajectory_classification-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/__init__.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     make_actual_vs_linearized_position_movie,
     make_track_graph,
     plot_graph_as_1D,
     plot_track_graph,
 )
 
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/classifier.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/classifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """State space models that classify trajectories as well as decode the
 trajectory from population spiking
 """
 from copy import deepcopy
 from logging import getLogger
+from typing import Optional, Union
 
 import joblib
+import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 import sklearn
 import xarray as xr
+from sklearn.base import BaseEstimator
+
 from replay_trajectory_classification.continuous_state_transitions import (
     EmpiricalMovement,
     RandomWalk,
+    RandomWalkDirection1,
+    RandomWalkDirection2,
     Uniform,
 )
 from replay_trajectory_classification.core import (
     _acausal_classify,
     _acausal_classify_gpu,
     _causal_classify,
     _causal_classify_gpu,
@@ -24,24 +30,29 @@
     check_converged,
     get_centers,
     mask,
     scaled_likelihood,
 )
 from replay_trajectory_classification.discrete_state_transitions import (
     DiagonalDiscrete,
+    RandomDiscrete,
+    UniformDiscrete,
+    UserDefinedDiscrete,
     estimate_discrete_state_transition,
 )
 from replay_trajectory_classification.environments import Environment
-from replay_trajectory_classification.initial_conditions import UniformInitialConditions
+from replay_trajectory_classification.initial_conditions import (
+    UniformInitialConditions,
+    UniformOneEnvironmentInitialConditions,
+)
 from replay_trajectory_classification.likelihoods import (
     _SORTED_SPIKES_ALGORITHMS,
     _ClUSTERLESS_ALGORITHMS,
 )
 from replay_trajectory_classification.observation_model import ObservationModel
-from sklearn.base import BaseEstimator
 
 logger = getLogger(__name__)
 
 sklearn.set_config(print_changed_only=False)
 
 _DEFAULT_CLUSTERLESS_MODEL_KWARGS = {
     "mark_std": 24.0,
@@ -56,51 +67,82 @@
 
 _DEFAULT_CONTINUOUS_TRANSITIONS = [[RandomWalk(), Uniform()], [Uniform(), Uniform()]]
 
 _DEFAULT_ENVIRONMENT = Environment(environment_name="")
 
 
 class _ClassifierBase(BaseEstimator):
+    """Base class for classifier objects."""
+
     def __init__(
         self,
-        environments=_DEFAULT_ENVIRONMENT,
-        observation_models=None,
-        continuous_transition_types=_DEFAULT_CONTINUOUS_TRANSITIONS,
-        discrete_transition_type=DiagonalDiscrete(0.968),
-        initial_conditions_type=UniformInitialConditions(),
-        infer_track_interior=True,
+        environments: list[Environment] = _DEFAULT_ENVIRONMENT,
+        observation_models: Optional[ObservationModel] = None,
+        continuous_transition_types: list[
+            list[
+                Union[
+                    EmpiricalMovement,
+                    RandomWalk,
+                    RandomWalkDirection1,
+                    RandomWalkDirection2,
+                    Uniform,
+                ]
+            ]
+        ] = _DEFAULT_CONTINUOUS_TRANSITIONS,
+        discrete_transition_type: Union[
+            DiagonalDiscrete,
+            RandomDiscrete,
+            UniformDiscrete,
+            UserDefinedDiscrete,
+        ] = DiagonalDiscrete(0.968),
+        initial_conditions_type: Union[
+            UniformInitialConditions, UniformOneEnvironmentInitialConditions
+        ] = UniformInitialConditions(),
+        infer_track_interior: bool = True,
     ):
         if isinstance(environments, Environment):
             environments = (environments,)
         if observation_models is None:
             n_states = len(continuous_transition_types)
             env_name = environments[0].environment_name
             observation_models = (ObservationModel(env_name),) * n_states
         self.environments = environments
         self.observation_models = observation_models
         self.continuous_transition_types = continuous_transition_types
         self.discrete_transition_type = discrete_transition_type
         self.initial_conditions_type = initial_conditions_type
         self.infer_track_interior = infer_track_interior
 
-    def fit_environments(self, position, environment_labels=None):
+    def fit_environments(
+        self, position: np.ndarray, environment_labels: Optional[np.ndarray] = None
+    ) -> None:
+        """Fits the Environment class on the position data to get information about the spatial environment.
+
+        Parameters
+        ----------
+        position : np.ndarray, shape (n_time, n_position_dims)
+        environment_labels : np.ndarray, optional, shape (n_time,)
+            Labels for each time points about which environment it corresponds to, by default None
+
+        """
         for environment in self.environments:
             if environment_labels is None:
                 is_environment = np.ones((position.shape[0],), dtype=bool)
             else:
                 is_environment = environment_labels == environment.environment_name
             environment.fit_place_grid(
                 position[is_environment], infer_track_interior=self.infer_track_interior
             )
 
         self.max_pos_bins_ = np.max(
             [env.place_bin_centers_.shape[0] for env in self.environments]
         )
 
     def fit_initial_conditions(self):
+        """Constructs the initial probability for the state and each spatial bin."""
         logger.info("Fitting initial conditions...")
         environment_names_to_state = [
             obs.environment_name for obs in self.observation_models
         ]
         n_states = len(self.observation_models)
         initial_conditions = self.initial_conditions_type.make_initial_conditions(
             self.environments, environment_names_to_state
@@ -110,20 +152,47 @@
             (n_states, self.max_pos_bins_, 1), dtype=np.float64
         )
         for state_ind, ic in enumerate(initial_conditions):
             self.initial_conditions_[state_ind, : ic.shape[0]] = ic[..., np.newaxis]
 
     def fit_continuous_state_transition(
         self,
-        continuous_transition_types=_DEFAULT_CONTINUOUS_TRANSITIONS,
-        position=None,
-        is_training=None,
-        encoding_group_labels=None,
-        environment_labels=None,
-    ):
+        continuous_transition_types: list[
+            list[
+                Union[
+                    EmpiricalMovement,
+                    RandomWalk,
+                    RandomWalkDirection1,
+                    RandomWalkDirection2,
+                    Uniform,
+                ]
+            ]
+        ] = _DEFAULT_CONTINUOUS_TRANSITIONS,
+        position: Optional[np.ndarray] = None,
+        is_training: Optional[np.ndarray] = None,
+        encoding_group_labels: Optional[np.ndarray] = None,
+        environment_labels: Optional[np.ndarray] = None,
+    ) -> None:
+        """Constructs the transition matrices for the continuous states.
+
+        Parameters
+        ----------
+        continuous_transition_types : list of list of transition matrix instances, optional
+            Types of transition models, by default _DEFAULT_CONTINUOUS_TRANSITIONS
+        position : np.ndarray, optional
+            Position of the animal in the environment, by default None
+        is_training : np.ndarray, optional
+            Boolean array that determines what data to train the place fields on, by default None
+        encoding_group_labels : np.ndarray, shape (n_time,), optional
+            If place fields should correspond to each state, label each time point with the group name
+            For example, Some points could correspond to inbound trajectories and some outbound, by default None
+        environment_labels : np.ndarray, shape (n_time,), optional
+            If there are multiple environments, label each time point with the environment name, by default None
+
+        """
         logger.info("Fitting continuous state transition...")
 
         if is_training is None:
             n_time = position.shape[0]
             is_training = np.ones((n_time,), dtype=bool)
 
         if encoding_group_labels is None:
@@ -161,29 +230,45 @@
         for row_ind, row in enumerate(continuous_state_transition):
             for column_ind, st in enumerate(row):
                 self.continuous_state_transition_[
                     row_ind, column_ind, : st.shape[0], : st.shape[1]
                 ] = st
 
     def fit_discrete_state_transition(self):
+        """Constructs the transition matrix for the discrete states."""
         logger.info("Fitting discrete state transition")
         n_states = len(self.continuous_transition_types)
         self.discrete_state_transition_ = (
             self.discrete_transition_type.make_state_transition(n_states)
         )
 
     def plot_discrete_state_transition(
         self,
-        state_names=None,
-        cmap="Oranges",
-        ax=None,
-        convert_to_seconds=False,
-        sampling_frequency=1,
-    ):
+        state_names: Optional[list[str]] = None,
+        cmap: str = "Oranges",
+        ax: Optional[matplotlib.axes.Axes] = None,
+        convert_to_seconds: bool = False,
+        sampling_frequency: int = 1,
+    ) -> None:
+        """Plot heatmap of discrete transition matrix.
+
+        Parameters
+        ----------
+        state_names : list[str], optional
+            Names corresponding to each discrete state, by default None
+        cmap : str, optional
+            matplotlib colormap, by default "Oranges"
+        ax : matplotlib.axes.Axes, optional
+            Plotting axis, by default plots to current axis
+        convert_to_seconds : bool, optional
+            Convert the probabilities of state to expected duration of state, by default False
+        sampling_frequency : int, optional
+            Number of samples per second, by default 1
 
+        """
         if ax is None:
             ax = plt.gca()
 
         if state_names is None:
             state_names = [
                 f"state {ind + 1}"
                 for ind in range(self.discrete_state_transition_.shape[0])
@@ -214,24 +299,51 @@
         )
         ax.set_ylabel("Previous State", fontsize=12)
         ax.set_xlabel("Current State", fontsize=12)
         ax.set_title("Discrete State Transition", fontsize=16)
 
     def estimate_parameters(
         self,
-        fit_args,
-        predict_args,
-        tolerance=1e-4,
-        max_iter=10,
-        verbose=True,
-        store_likelihood=True,
-        estimate_initial_conditions=True,
-        estimate_discrete_transition=True,
-    ):
+        fit_args: dict,
+        predict_args: dict,
+        tolerance: float = 1e-4,
+        max_iter: int = 10,
+        verbose: bool = True,
+        store_likelihood: bool = True,
+        estimate_initial_conditions: bool = True,
+        estimate_discrete_transition: bool = True,
+    ) -> tuple[xr.Dataset, list[float]]:
+        """Estimate the intial conditions and/or discrete transition matrix of the model.
+
+        Parameters
+        ----------
+        fit_args : dict
+           Arguments that would be passed to the `fit` method.
+        predict_args : dict
+            Arguments that would be passed to the `predict` method.
+        tolerance : float, optional
+            Smallest change in data log likelihood for there to be no change in likelihood, by default 1e-4
+        max_iter : int, optional
+            Maximum number of iterations, by default 10
+        verbose : bool, optional
+            Log results of each iteration, by default True
+        store_likelihood : bool, optional
+            If True, don't reestimate the likelihood, by default True
+        estimate_initial_conditions : bool, optional
+            If True, estimate the initial conditions, by default True
+        estimate_discrete_transition : bool, optional
+            If True, estimate the discrete state transition, by default True
 
+        Returns
+        -------
+        results : xr.Dataset
+        data_log_likelihoods : list, len (n_iter,)
+            The data log likelihood of each iteration
+
+        """
         if "store_likelihood" in predict_args:
             store_likelihood = predict_args["store_likelihood"]
         else:
             predict_args["store_likelihood"] = store_likelihood
 
         self.fit(**fit_args)
         results = self.predict(**predict_args)
@@ -364,23 +476,71 @@
 
         return xr.Dataset(
             {key: (dims, value) for key, value in results1D.items()},
             coords=coords,
             attrs=results2D.attrs,
         )
 
+    def project_1D_position_to_2D(
+        self, results: xr.Dataset, posterior_type="acausal_posterior"
+    ) -> np.ndarray:
+        """Project the 1D most probable position into the 2D track graph space.
+
+        Only works for single environment.
+
+        Parameters
+        ----------
+        results : xr.Dataset
+        posterior_type : causal_posterior | acausal_posterior | likelihood
+
+        Returns
+        -------
+        map_position2D : np.ndarray
+
+        """
+        if len(self.environments) > 1:
+            print("Canont project back with multiple environments.")
+            return
+        map_position_ind = (
+            results[posterior_type].sum("state").argmax("position").to_numpy().squeeze()
+        )
+
+        return (
+            self.environments[0]
+            .place_bin_centers_nodes_df_.iloc[map_position_ind][
+                ["x_position", "y_position"]
+            ]
+            .to_numpy()
+        )
+
     def _get_results(
         self,
-        likelihood,
-        n_time,
-        time=None,
-        is_compute_acausal=True,
-        use_gpu=False,
-        state_names=None,
-    ):
+        likelihood: np.ndarray,
+        n_time: int,
+        time: Optional[np.ndarray] = None,
+        is_compute_acausal: bool = True,
+        use_gpu: bool = False,
+        state_names: Optional[list[str]] = None,
+    ) -> xr.Dataset:
+        """Computes the causal and acausal posterior after the likelihood has been computed.
+
+        Parameters
+        ----------
+        likelihood : np.ndarray
+        n_time : int
+        time : np.ndarray, optional
+        is_compute_acausal : bool, optional
+        use_gpu : bool, optional
+        state_names : list[str], optional
+
+        Returns
+        -------
+        results : xr.Dataset
+
+        """
         n_states = self.discrete_state_transition_.shape[0]
         results = {}
         dtype = np.float32 if use_gpu else np.float64
 
         results["likelihood"] = np.full(
             (n_time, n_states, self.max_pos_bins_, 1), np.nan, dtype=dtype
         )
@@ -458,16 +618,34 @@
                 )
 
             return self._convert_results_to_xarray_mutienvironment(
                 results, time, state_names, data_log_likelihood
             )
 
     def _convert_results_to_xarray(
-        self, results, time, state_names, data_log_likelihood
-    ):
+        self,
+        results: dict,
+        time: np.ndarray,
+        state_names: list,
+        data_log_likelihood: float,
+    ) -> xr.Dataset:
+        """Converts the results dict into a collection of labeled arrays.
+
+        Parameters
+        ----------
+        results : dict
+        time : np.ndarray
+        state_names : list
+        data_log_likelihood : float
+
+        Returns
+        -------
+        results : xr.Dataset
+
+        """
         attrs = {"data_log_likelihood": data_log_likelihood}
         n_position_dims = self.environments[0].place_bin_centers_.shape[1]
         diag_transition_names = np.diag(np.asarray(self.continuous_transition_types))
         if state_names is None:
             if len(np.unique(self.observation_models)) == 1:
                 state_names = diag_transition_names
             else:
@@ -522,16 +700,34 @@
                 coords=coords,
                 attrs=attrs,
             )
 
         return results
 
     def _convert_results_to_xarray_mutienvironment(
-        self, results, time, state_names, data_log_likelihood
-    ):
+        self,
+        results: dict,
+        time: np.ndarray,
+        state_names: list,
+        data_log_likelihood: float,
+    ) -> xr.Dataset:
+        """Converts the results dict into a collection of labeled arrays when there are multiple environments.
+
+        Parameters
+        ----------
+        results : dict
+        time : np.ndarray
+        state_names : list
+        data_log_likelihood : float
+
+        Returns
+        -------
+        results : xr.Dataset
+
+        """
         if state_names is None:
             state_names = [
                 f"{obs.environment_name}-{obs.encoding_group}"
                 for obs in self.observation_models
             ]
 
         attrs = {"data_log_likelihood": data_log_likelihood}
@@ -569,89 +765,156 @@
                 coords=coords,
                 attrs=attrs,
             )
 
         return results
 
     def fit(self):
+        """To be implemented by inheriting class"""
         raise NotImplementedError
 
     def predict(self):
+        """To be implemented by inheriting class"""
         raise NotImplementedError
 
-    def save_model(self, filename="model.pkl"):
+    def save_model(self, filename: str = "model.pkl") -> None:
+        """Save the classifier to a pickled file.
+
+        Parameters
+        ----------
+        filename : str, optional
+
+        """
         joblib.dump(self, filename)
 
     @staticmethod
-    def load_model(filename="model.pkl"):
+    def load_model(filename: str = "model.pkl"):
+        """Load the classifier from a file.
+
+        Parameters
+        ----------
+        filename : str, optional
+
+        Returns
+        -------
+        classifier instance
+
+        """
         return joblib.load(filename)
 
     @staticmethod
-    def predict_proba(results):
+    def predict_proba(results: xr.Dataset) -> xr.Dataset:
+        """Predicts the probability of each state.
+
+        Parameters
+        ----------
+        results : xr.Dataset
+
+        Returns
+        -------
+        results : xr.Dataset
+
+        """
         try:
             return results.sum(["x_position", "y_position"])
         except ValueError:
             return results.sum(["position"])
 
     def copy(self):
+        """Makes a copy of the classifier"""
         return deepcopy(self)
 
 
 class SortedSpikesClassifier(_ClassifierBase):
-    """
+    """Classifies neural population representation of position and trajectory from clustered cells.
 
-    Attributes
+    Parameters
     ----------
-    environment : Environment
-        The spatial environment and topology to fit
-    continuous_transition_types : tuple of tuples
-        The continuous state transition class instances to fit
-    discrete_transition_type : Discrete
-        The type of transition between states
-    initial_conditions_type : InitialConditions
-        The initial conditions class instance to fit
+    environments : list of Environment instances, optional
+        The spatial environment(s) to fit
+    observation_models : ObservationModel instance, optional
+        Links environments and encoding group
+    continuous_transition_types : list of list of transition matrix instances, optional
+        Types of transition models, by default _DEFAULT_CONTINUOUS_TRANSITIONS
+        Length correspond to number of discrete states.
+    discrete_transition_type : discrete transition instance, optional
+    initial_conditions_type : initial conditions instance, optional
+        The initial conditions class instance
     infer_track_interior : bool, optional
-        Whether to infer the valid position bins
-    sorted_spikes_algorithm : str
+        Whether to infer the spatial geometry of track from position
+    sorted_spikes_algorithm : str, optional
         The type of algorithm. See _SORTED_SPIKES_ALGORITHMS for keys
-    sorted_spikes_algorithm_params : dict
+    sorted_spikes_algorithm_params : dict, optional
         Parameters for the algorithm.
 
     """
 
     def __init__(
         self,
-        environments=_DEFAULT_ENVIRONMENT,
-        observation_models=None,
-        continuous_transition_types=_DEFAULT_CONTINUOUS_TRANSITIONS,
-        discrete_transition_type=DiagonalDiscrete(0.98),
-        initial_conditions_type=UniformInitialConditions(),
-        infer_track_interior=True,
-        sorted_spikes_algorithm="spiking_likelihood_kde",
-        sorted_spikes_algorithm_params=_DEFAULT_SORTED_SPIKES_MODEL_KWARGS,
+        environments: list[Environment] = _DEFAULT_ENVIRONMENT,
+        observation_models: Optional[ObservationModel] = None,
+        continuous_transition_types: list[
+            list[
+                Union[
+                    EmpiricalMovement,
+                    RandomWalk,
+                    RandomWalkDirection1,
+                    RandomWalkDirection2,
+                    Uniform,
+                ]
+            ]
+        ] = _DEFAULT_CONTINUOUS_TRANSITIONS,
+        discrete_transition_type: Union[
+            DiagonalDiscrete,
+            RandomDiscrete,
+            UniformDiscrete,
+            UserDefinedDiscrete,
+        ] = DiagonalDiscrete(0.98),
+        initial_conditions_type: Union[
+            UniformInitialConditions, UniformOneEnvironmentInitialConditions
+        ] = UniformInitialConditions(),
+        infer_track_interior: bool = True,
+        sorted_spikes_algorithm: str = "spiking_likelihood_kde",
+        sorted_spikes_algorithm_params: dict = _DEFAULT_SORTED_SPIKES_MODEL_KWARGS,
     ):
         super().__init__(
             environments,
             observation_models,
             continuous_transition_types,
             discrete_transition_type,
             initial_conditions_type,
             infer_track_interior,
         )
         self.sorted_spikes_algorithm = sorted_spikes_algorithm
         self.sorted_spikes_algorithm_params = sorted_spikes_algorithm_params
 
     def fit_place_fields(
         self,
-        position,
-        spikes,
-        is_training=None,
-        encoding_group_labels=None,
-        environment_labels=None,
-    ):
+        position: np.ndarray,
+        spikes: np.ndarray,
+        is_training: Optional[np.ndarray] = None,
+        encoding_group_labels: Optional[np.ndarray] = None,
+        environment_labels: Optional[np.ndarray] = None,
+    ) -> None:
+        """Fits the place intensity function for each encoding group and environment.
+
+        Parameters
+        ----------
+        position : np.ndarray, shape (n_time, n_position_dims)
+            Position of the animal.
+        spikes : np.ndarray, (n_time, n_neurons)
+            Binary indicator of whether there was a spike in a given time bin for a given neuron.
+        is_training : np.ndarray, shape (n_time,), optional
+            Boolean array to indicate which data should be included in fitting of place fields, by default None
+        encoding_group_labels : np.ndarray, shape (n_time,), optional
+            Label for the corresponding encoding group for each time point
+        environment_labels : np.ndarray, shape (n_time,), optional
+            Label for the corresponding environment for each time point
+
+        """
         logger.info("Fitting place fields...")
         n_time = position.shape[0]
         if is_training is None:
             is_training = np.ones((n_time,), dtype=bool)
 
         if encoding_group_labels is None:
             encoding_group_labels = np.zeros((n_time,), dtype=np.int32)
@@ -686,23 +949,26 @@
                 place_bin_edges=environment.place_bin_edges_,
                 edges=environment.edges_,
                 is_track_interior=environment.is_track_interior_,
                 is_track_boundary=environment.is_track_boundary_,
                 **kwargs,
             )
 
-    def plot_place_fields(self, sampling_frequency=1, figsize=(10, 7)):
-        """Plots all place fields.
+    def plot_place_fields(
+        self, sampling_frequency: int = 1, figsize: tuple[float, float] = (10.0, 7.0)
+    ):
+        """Plots place fields for each neuron.
 
         Parameters
         ----------
         sampling_frequency : int, optional
             samples per second, by default 1
         figsize : tuple, optional
             figure dimensions, by default (10, 7)
+
         """
         try:
             for (env, enc) in self.place_fields_:
                 is_track_interior = self.environments[
                     self.environments.index(env)
                 ].is_track_interior_[np.newaxis]
                 (
@@ -737,29 +1003,31 @@
                     .plot(x="position", hue="neuron", add_legend=False, ax=ax)
                 )
                 ax.set_title(f"Environment = {env_name}, Encoding Group = {enc_group}")
                 ax.set_ylabel("Firing Rate\n[spikes/s]")
 
     def fit(
         self,
-        position,
-        spikes,
-        is_training=None,
-        encoding_group_labels=None,
-        environment_labels=None,
+        position: np.ndarray,
+        spikes: np.ndarray,
+        is_training: Optional[np.ndarray] = None,
+        encoding_group_labels: Optional[np.ndarray] = None,
+        environment_labels: Optional[np.ndarray] = None,
     ):
         """Fit the spatial grid, initial conditions, place field model, and
         transition matrices.
 
         Parameters
         ----------
         position : np.ndarray, shape (n_time, n_position_dims)
+            Position of the animal.
         spikes : np.ndarray, shape (n_time, n_neurons)
-        is_training : None or bool np.ndarray, shape (n_time), optional
-            Time bins to be used for encoding.
+            Binary indicator of whether there was a spike in a given time bin for a given neuron.
+        is_training : None or np.ndarray, shape (n_time), optional
+            Boolean array to indicate which data should be included in fitting of place fields, by default None
         encoding_group_labels : None or np.ndarray, shape (n_time,)
             Label for the corresponding encoding group for each time point
         environment_labels : None or np.ndarray, shape (n_time,)
             Label for the corresponding environment for each time point
 
         Returns
         -------
@@ -782,31 +1050,37 @@
             position, spikes, is_training, encoding_group_labels, environment_labels
         )
 
         return self
 
     def predict(
         self,
-        spikes,
-        time=None,
-        is_compute_acausal=True,
-        use_gpu=False,
-        state_names=None,
-        store_likelihood=False,
-    ):
-        """Run the state space model on spikes.
+        spikes: np.ndarray,
+        time: Optional[np.ndarray] = None,
+        is_compute_acausal: bool = True,
+        use_gpu: bool = False,
+        state_names: Optional[list[str]] = None,
+        store_likelihood: bool = False,
+    ) -> xr.Dataset:
+        """Predict the probability of spatial position and category from the spikes.
 
         Parameters
         ----------
         spikes : np.ndarray, shape (n_time, n_neurons)
-        time : ndarray or None, shape (n_time,), optional
+            Binary indicator of whether there was a spike in a given time bin for a given neuron.
+        time : np.ndarray or None, shape (n_time,), optional
+            Label the time axis with these values.
         is_compute_acausal : bool, optional
+            If True, compute the acausal posterior.
         use_gpu : bool, optional
             Use GPU for the state space part of the model, not the likelihood.
         state_names : None or array_like, shape (n_states,)
+            Label the discrete states.
+        store_likelihood : bool, optional
+            Store the likelihood to reuse in next computation.
 
         Returns
         -------
         results : xarray.Dataset
 
         """
         spikes = np.asarray(spikes)
@@ -828,45 +1102,64 @@
 
         return self._get_results(
             likelihood, n_time, time, is_compute_acausal, use_gpu, state_names
         )
 
 
 class ClusterlessClassifier(_ClassifierBase):
-    """
+    """Classifies neural population representation of position and trajectory from multiunit spikes and waveforms.
 
-    Attributes
+    Parameters
     ----------
-    environment : Environment
-        The spatial environment and topology to fit
-    continuous_transition_types : tuple of tuples
-        The continuous state transition class instances to fit
-    discrete_transition_type : Discrete
-        The type of transition between states
-    initial_conditions_type : InitialConditions
-        The initial conditions class instance to fit
+    environments : list of Environment instances, optional
+        The spatial environment(s) to fit
+    observation_models : ObservationModel instance, optional
+        Links environments and encoding group
+    continuous_transition_types : list of list of transition matrix instances, optional
+        Types of transition models, by default _DEFAULT_CONTINUOUS_TRANSITIONS
+        Length correspond to number of discrete states.
+    discrete_transition_type : discrete transition instance, optional
+    initial_conditions_type : initial conditions instance, optional
+        The initial conditions class instance
     infer_track_interior : bool, optional
-        Whether to infer the valid position bins
+        Whether to infer the spatial geometry of track from position
     clusterless_algorithm : str
         The type of clusterless algorithm. See _ClUSTERLESS_ALGORITHMS for keys
     clusterless_algorithm_params : dict
         Parameters for the clusterless algorithms.
 
     """
 
     def __init__(
         self,
-        environments=_DEFAULT_ENVIRONMENT,
+        environments: list[Environment] = _DEFAULT_ENVIRONMENT,
         observation_models=None,
-        continuous_transition_types=_DEFAULT_CONTINUOUS_TRANSITIONS,
-        discrete_transition_type=DiagonalDiscrete(0.98),
-        initial_conditions_type=UniformInitialConditions(),
-        infer_track_interior=True,
-        clusterless_algorithm="multiunit_likelihood",
-        clusterless_algorithm_params=_DEFAULT_CLUSTERLESS_MODEL_KWARGS,
+        continuous_transition_types: list[
+            list[
+                Union[
+                    EmpiricalMovement,
+                    RandomWalk,
+                    RandomWalkDirection1,
+                    RandomWalkDirection2,
+                    Uniform,
+                ]
+            ]
+        ] = _DEFAULT_CONTINUOUS_TRANSITIONS,
+        discrete_transition_type: Union[
+            DiagonalDiscrete,
+            RandomDiscrete,
+            UniformDiscrete,
+            UserDefinedDiscrete,
+        ] = DiagonalDiscrete(0.98),
+        initial_conditions_type: Union[
+            UniformInitialConditions, UniformOneEnvironmentInitialConditions
+        ] = UniformInitialConditions(),
+        infer_track_interior: bool = True,
+        clusterless_algorithm: str = "multiunit_likelihood",
+        clusterless_algorithm_params: dict = _DEFAULT_CLUSTERLESS_MODEL_KWARGS,
     ):
         super().__init__(
             environments,
             observation_models,
             continuous_transition_types,
             discrete_transition_type,
             initial_conditions_type,
@@ -874,27 +1167,31 @@
         )
 
         self.clusterless_algorithm = clusterless_algorithm
         self.clusterless_algorithm_params = clusterless_algorithm_params
 
     def fit_multiunits(
         self,
-        position,
-        multiunits,
-        is_training=None,
-        encoding_group_labels=None,
-        environment_labels=None,
+        position: np.ndarray,
+        multiunits: np.ndarray,
+        is_training: Optional[np.ndarray] = None,
+        encoding_group_labels: Optional[np.ndarray] = None,
+        environment_labels: Optional[np.ndarray] = None,
     ):
         """Fit the clusterless place field model.
 
         Parameters
         ----------
-        position : array_like, shape (n_time, n_position_dims)
+        position : np.ndarray, shape (n_time, n_position_dims)
+            Position of the animal.
         multiunits : array_like, shape (n_time, n_marks, n_electrodes)
-        is_training : None or array_like, shape (n_time,)
+            Array where spikes are indicated by non-Nan values that correspond to the waveform features
+            for each electrode.
+        is_training : None or np.ndarray, shape (n_time), optional
+            Boolean array to indicate which data should be included in fitting of place fields, by default None
         encoding_group_labels : None or np.ndarray, shape (n_time,)
             Label for the corresponding encoding group for each time point
         environment_labels : None or np.ndarray, shape (n_time,)
             Label for the corresponding environment for each time point
 
         """
         logger.info("Fitting multiunits...")
@@ -939,28 +1236,32 @@
                 is_track_boundary=environment.is_track_boundary_,
                 edges=environment.edges_,
                 **kwargs,
             )
 
     def fit(
         self,
-        position,
-        multiunits,
-        is_training=None,
-        encoding_group_labels=None,
-        environment_labels=None,
+        position: np.ndarray,
+        multiunits: np.ndarray,
+        is_training: Optional[np.ndarray] = None,
+        encoding_group_labels: Optional[np.ndarray] = None,
+        environment_labels: Optional[np.ndarray] = None,
     ):
         """Fit the spatial grid, initial conditions, place field model, and
         transition matrices.
 
         Parameters
         ----------
-        position : array_like, shape (n_time, n_position_dims)
+        position : np.ndarray, shape (n_time, n_position_dims)
+            Position of the animal.
         multiunits : array_like, shape (n_time, n_marks, n_electrodes)
-        is_training : None or array_like, shape (n_time,)
+            Array where spikes are indicated by non-Nan values that correspond to the waveform features
+            for each electrode.
+        is_training : None or np.ndarray, shape (n_time), optional
+            Boolean array to indicate which data should be included in fitting of place fields, by default None
         encoding_group_labels : None or np.ndarray, shape (n_time,)
             Label for the corresponding encoding group for each time point
         environment_labels : None or np.ndarray, shape (n_time,)
             Label for the corresponding environment for each time point
 
         Returns
         -------
@@ -984,34 +1285,38 @@
             position, multiunits, is_training, encoding_group_labels, environment_labels
         )
 
         return self
 
     def predict(
         self,
-        multiunits,
-        time=None,
-        is_compute_acausal=True,
-        use_gpu=False,
-        state_names=None,
-        store_likelihood=False,
-    ):
-        """Run the state space model.
+        multiunits: np.ndarray,
+        time: Optional[np.ndarray] = None,
+        is_compute_acausal: bool = True,
+        use_gpu: bool = False,
+        state_names: Optional[list[str]] = None,
+        store_likelihood: bool = False,
+    ) -> xr.Dataset:
+        """Predict the probability of spatial position and category from the multiunit spikes and waveforms.
 
         Parameters
         ----------
         multiunits : array_like, shape (n_time, n_marks, n_electrodes)
-        time : None or np.ndarray, shape (n_time,)
+            Array where spikes are indicated by non-Nan values that correspond to the waveform features
+            for each electrode.
+        time : np.ndarray or None, shape (n_time,), optional
+            Label the time axis with these values.
         is_compute_acausal : bool, optional
-            Use future information to compute the posterior.
+            If True, compute the acausal posterior.
         use_gpu : bool, optional
             Use GPU for the state space part of the model, not the likelihood.
         state_names : None or array_like, shape (n_states,)
+            Label the discrete states.
         store_likelihood : bool, optional
-            Save the likelihood for EM computations
+            Store the likelihood to reuse in next computation.
 
         Returns
         -------
         results : xarray.Dataset
 
         """
         multiunits = np.asarray(multiunits)
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/core.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,63 @@
 """Core algorithms for decoding."""
 import numpy as np
 from numba import njit
 
 
-def atleast_2d(x):
-    """Appends a dimension at the end if `x` is one dimensional"""
+def atleast_2d(x: np.ndarray) -> np.ndarray:
+    """Appends a dimension at the end if `x` is one dimensional
+
+    Parameters
+    ----------
+    x : np.ndarray
+
+    Returns
+    -------
+    x : np.ndarray
+
+    """
     return np.atleast_2d(x).T if x.ndim < 2 else x
 
 
-def get_centers(edge):
-    """ "Given a set of bin edges, return the center of the bin"""
-    return edge[:-1] + np.diff(edge) / 2
+def get_centers(bin_edges: np.ndarray) -> np.ndarray:
+    """Given a set of bin edges, return the center of the bin.
+
+    Parameters
+    ----------
+    bin_edges : np.ndarray, shape (n_edges,)
+
+    Returns
+    -------
+    bin_centers : np.ndarray, shape (n_edges - 1,)
+
+    """
+    return bin_edges[:-1] + np.diff(bin_edges) / 2
 
 
 @njit(parallel=True, error_model="numpy")
-def normalize_to_probability(distribution):
+def normalize_to_probability(distribution: np.ndarray) -> np.ndarray:
     """Ensure the distribution integrates to 1 so that it is a probability
-    distribution
+    distribution.
+
+    Parameters
+    ----------
+    distribution : np.ndarray
+
+    Returns
+    -------
+    normalized_distribution : np.ndarray
+
     """
     return distribution / np.nansum(distribution)
 
 
 @njit(nogil=True, error_model="numpy", cache=False)
-def _causal_decode(initial_conditions, state_transition, likelihood):
+def _causal_decode(
+    initial_conditions: np.ndarray, state_transition: np.ndarray, likelihood: np.ndarray
+) -> tuple[np.ndarray, float]:
     """Adaptive filter to iteratively calculate the posterior probability
     of a state variable using past information.
 
     Parameters
     ----------
     initial_conditions : np.ndarray, shape (n_bins,)
     state_transition : np.ndarray, shape (n_bins, n_bins)
@@ -53,15 +84,17 @@
         log_data_likelihood += np.log(norm)
         posterior[k] /= norm
 
     return posterior, log_data_likelihood
 
 
 @njit(nogil=True, error_model="numpy", cache=False)
-def _acausal_decode(causal_posterior, state_transition):
+def _acausal_decode(
+    causal_posterior: np.ndarray, state_transition: np.ndarray
+) -> np.ndarray:
     """Uses past and future information to estimate the state.
 
     Parameters
     ----------
     causal_posterior : np.ndarray, shape (n_time, n_bins, 1)
     state_transition : np.ndarray, shape (n_bins, n_bins)
 
@@ -89,27 +122,26 @@
         )
 
     return acausal_posterior
 
 
 @njit(nogil=True, error_model="numpy", cache=False)
 def _causal_classify(
-    initial_conditions,
-    continuous_state_transition,
-    discrete_state_transition,
-    likelihood,
-):
+    initial_conditions: np.ndarray,
+    continuous_state_transition: np.ndarray,
+    discrete_state_transition: np.ndarray,
+    likelihood: np.ndarray,
+) -> tuple[np.ndarray, float]:
     """Adaptive filter to iteratively calculate the posterior probability
     of a state variable using past information.
 
     Parameters
     ----------
     initial_conditions : np.ndarray, shape (n_states, n_bins, 1)
-    continuous_state_transition : np.ndarray, shape (n_states, n_states,
-                                                  n_bins, n_bins)
+    continuous_state_transition : np.ndarray, shape (n_states, n_states, n_bins, n_bins)
     discrete_state_transition : np.ndarray, shape (n_states, n_states)
     likelihood : np.ndarray, shape (n_time, n_states, n_bins, 1)
 
     Returns
     -------
     causal_posterior : np.ndarray, shape (n_time, n_states, n_bins, 1)
     log_data_likelihood : float
@@ -138,23 +170,24 @@
         posterior[k] /= norm
 
     return posterior, log_data_likelihood
 
 
 @njit(nogil=True, error_model="numpy", cache=False)
 def _acausal_classify(
-    causal_posterior, continuous_state_transition, discrete_state_transition
-):
+    causal_posterior: np.ndarray,
+    continuous_state_transition: np.ndarray,
+    discrete_state_transition: np.ndarray,
+) -> np.ndarray:
     """Uses past and future information to estimate the state.
 
     Parameters
     ----------
     causal_posterior : np.ndarray, shape (n_time, n_states, n_bins, 1)
-    continuous_state_transition : np.ndarray, shape (n_states, n_states,
-                                                  n_bins, n_bins)
+    continuous_state_transition : np.ndarray, shape (n_states, n_states, n_bins, n_bins)
     discrete_state_transition : np.ndarray, shape (n_states, n_states)
 
     Return
     ------
     acausal_posterior : np.ndarray, shape (n_time, n_states, n_bins, 1)
 
     """
@@ -186,19 +219,21 @@
                 )
 
         acausal_posterior[k] = normalize_to_probability(weights * causal_posterior[k])
 
     return acausal_posterior
 
 
-def scaled_likelihood(log_likelihood, axis=1):
-    """
+def scaled_likelihood(log_likelihood: np.ndarray, axis: int = 1) -> np.ndarray:
+    """Scale the likelihood so the maximum value is 1.
+
     Parameters
     ----------
     log_likelihood : np.ndarray, shape (n_time, n_bins)
+    axis : int
 
     Returns
     -------
     scaled_log_likelihood : np.ndarray, shape (n_time, n_bins)
 
     """
     max_log_likelihood = np.nanmax(log_likelihood, axis=axis, keepdims=True)
@@ -211,58 +246,92 @@
     # Maximum likelihood is always 1
     likelihood = np.exp(log_likelihood - max_log_likelihood)
     # avoid zero likelihood
     likelihood += np.spacing(1, dtype=likelihood.dtype)
     return likelihood
 
 
-def mask(value, is_track_interior):
-    """Set bins that are not part of the track to NaN"""
+def mask(value: np.ndarray, is_track_interior: np.ndarray) -> np.ndarray:
+    """Set bins that are not part of the track to NaN.
+
+    Parameters
+    ----------
+    value : np.ndarray, shape (..., n_bins)
+    is_track_interior : np.ndarray, shape (n_bins,)
+
+    Returns
+    -------
+    masked_value : np.ndarray
+
+    """
     try:
         value[..., ~is_track_interior] = np.nan
     except IndexError:
         value[..., ~is_track_interior, :] = np.nan
     return value
 
 
-def check_converged(loglik, previous_loglik, tolerance=1e-4):
-    """
-    We have converged if the slope of the log-likelihood function falls below 'threshold',
-    i.e., |f(t) - f(t-1)| / avg < threshold,
+def check_converged(
+    log_likelihood: np.ndarray,
+    previous_log_likelihood: np.ndarray,
+    tolerance: float = 1e-4,
+) -> tuple[bool, bool]:
+    """We have converged if the slope of the log-likelihood function falls below 'tolerance',
+
+    i.e., |f(t) - f(t-1)| / avg < tolerance,
     where avg = (|f(t)| + |f(t-1)|)/2 and f(t) is log lik at iteration t.
-    'threshold' defaults to 1e-4.
 
-    This stopping criterion is from Numerical Recipes in C p423
+    Parameters
+    ----------
+    log_likelihood : np.ndarray
+        Current log likelihood
+    previous_log_likelihood : np.ndarray
+        Previous log likelihood
+    tolerance : float, optional
+        threshold for similarity, by default 1e-4
+
+    Returns
+    -------
+    is_converged : bool
+    is_increasing : bool
+
     """
-    delta_loglik = abs(loglik - previous_loglik)
-    avg_loglik = (abs(loglik) + abs(previous_loglik) + np.spacing(1)) / 2
+    delta_log_likelihood = abs(log_likelihood - previous_log_likelihood)
+    avg_log_likelihood = (
+        abs(log_likelihood) + abs(previous_log_likelihood) + np.spacing(1)
+    ) / 2
 
-    is_increasing = loglik - previous_loglik >= -1e-3
-    is_converged = (delta_loglik / avg_loglik) < tolerance
+    is_increasing = log_likelihood - previous_log_likelihood >= -1e-3
+    is_converged = (delta_log_likelihood / avg_log_likelihood) < tolerance
 
     return is_converged, is_increasing
 
 
 try:
     import cupy as cp
 
     @cp.fuse()
-    def _causal_decode_gpu(initial_conditions, state_transition, likelihood):
+    def _causal_decode_gpu(
+        initial_conditions: np.ndarray,
+        state_transition: np.ndarray,
+        likelihood: np.ndarray,
+    ) -> tuple[np.ndarray, float]:
         """Adaptive filter to iteratively calculate the posterior probability
         of a state variable using past information.
 
         Parameters
         ----------
         initial_conditions : np.ndarray, shape (n_bins,)
         state_transition : np.ndarray, shape (n_bins, n_bins)
         likelihood : np.ndarray, shape (n_time, n_bins)
 
         Returns
         -------
         posterior : np.ndarray, shape (n_time, n_bins)
+        log_data_likelihood : float
 
         """
 
         initial_conditions = cp.asarray(initial_conditions, dtype=cp.float32)
         state_transition = cp.asarray(state_transition, dtype=cp.float32)
         likelihood = cp.asarray(likelihood, dtype=cp.float32)
 
@@ -279,15 +348,17 @@
             norm = np.nansum(posterior[k])
             log_data_likelihood += cp.log(norm)
             posterior[k] /= norm
 
         return cp.asnumpy(posterior), cp.asnumpy(log_data_likelihood)
 
     @cp.fuse()
-    def _acausal_decode_gpu(causal_posterior, state_transition):
+    def _acausal_decode_gpu(
+        causal_posterior: np.ndarray, state_transition: np.ndarray
+    ) -> np.ndarray:
         """Uses past and future information to estimate the state.
 
         Parameters
         ----------
         causal_posterior : np.ndarray, shape (n_time, n_bins, 1)
         state_transition : np.ndarray, shape (n_bins, n_bins)
 
@@ -315,33 +386,33 @@
             acausal_posterior[time_ind] = weights * causal_posterior[time_ind]
             acausal_posterior[time_ind] /= np.nansum(acausal_posterior[time_ind])
 
         return cp.asnumpy(acausal_posterior)
 
     @cp.fuse()
     def _causal_classify_gpu(
-        initial_conditions,
-        continuous_state_transition,
-        discrete_state_transition,
-        likelihood,
-    ):
+        initial_conditions: np.ndarray,
+        continuous_state_transition: np.ndarray,
+        discrete_state_transition: np.ndarray,
+        likelihood: np.ndarray,
+    ) -> tuple(np.ndarray, float):
         """Adaptive filter to iteratively calculate the posterior probability
         of a state variable using past information.
 
         Parameters
         ----------
         initial_conditions : np.ndarray, shape (n_states, n_bins, 1)
-        continuous_state_transition : np.ndarray, shape (n_states, n_states,
-                                                      n_bins, n_bins)
+        continuous_state_transition : np.ndarray, shape (n_states, n_states, n_bins, n_bins)
         discrete_state_transition : np.ndarray, shape (n_states, n_states)
         likelihood : np.ndarray, shape (n_time, n_states, n_bins, 1)
 
         Returns
         -------
         causal_posterior : np.ndarray, shape (n_time, n_states, n_bins, 1)
+        log_data_likelihood : float
 
         """
         initial_conditions = cp.asarray(initial_conditions, dtype=cp.float32)
         continuous_state_transition = cp.asarray(
             continuous_state_transition, dtype=cp.float32
         )
         discrete_state_transition = cp.asarray(
@@ -370,23 +441,24 @@
             log_data_likelihood += cp.log(norm)
             posterior[k] /= norm
 
         return cp.asnumpy(posterior), cp.asnumpy(log_data_likelihood)
 
     @cp.fuse()
     def _acausal_classify_gpu(
-        causal_posterior, continuous_state_transition, discrete_state_transition
-    ):
+        causal_posterior: np.ndarray,
+        continuous_state_transition: np.ndarray,
+        discrete_state_transition: np.ndarray,
+    ) -> np.ndarray:
         """Uses past and future information to estimate the state.
 
         Parameters
         ----------
         causal_posterior : np.ndarray, shape (n_time, n_states, n_bins, 1)
-        continuous_state_transition : np.ndarray, shape (n_states, n_states,
-                                                      n_bins, n_bins)
+        continuous_state_transition : np.ndarray, shape (n_states, n_states, n_bins, n_bins)
         discrete_state_transition : np.ndarray, shape (n_states, n_states)
 
         Return
         ------
         acausal_posterior : np.ndarray, shape (n_time, n_states, n_bins, 1)
 
         """
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/decoder.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/decoder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-"""Main classeses for decoding trajectories from population spiking"""
+"""Main classes for decoding trajectories from population spiking"""
 
 from copy import deepcopy
 from logging import getLogger
+from typing import Optional, Union
 
 import joblib
 import numpy as np
 import sklearn
 import xarray as xr
+from sklearn.base import BaseEstimator
+
 from replay_trajectory_classification.continuous_state_transitions import (
     EmpiricalMovement,
     RandomWalk,
+    RandomWalkDirection1,
+    RandomWalkDirection2,
+    Uniform,
 )
 from replay_trajectory_classification.core import (
     _acausal_decode,
     _acausal_decode_gpu,
     _causal_decode,
     _causal_decode_gpu,
     atleast_2d,
@@ -23,15 +29,14 @@
 )
 from replay_trajectory_classification.environments import Environment
 from replay_trajectory_classification.initial_conditions import UniformInitialConditions
 from replay_trajectory_classification.likelihoods import (
     _SORTED_SPIKES_ALGORITHMS,
     _ClUSTERLESS_ALGORITHMS,
 )
-from sklearn.base import BaseEstimator
 
 logger = getLogger(__name__)
 
 sklearn.set_config(print_changed_only=False)
 
 _DEFAULT_CLUSTERLESS_MODEL_KWARGS = {
     "mark_std": 24.0,
@@ -42,41 +47,85 @@
     "position_std": 6.0,
     "use_diffusion": False,
     "block_size": None,
 }
 
 
 class _DecoderBase(BaseEstimator):
+    """Base class for decoder objects.
+
+    Parameters
+    ----------
+    environment : Environment, optional
+        The spatial environment to fit
+    transition_type : EmpiricalMovement | RandomWalk | RandomWalkDirection1 | RandomWalkDirection2 | Uniform
+        The continuous state transition matrix
+    initial_conditions_type : UniformInitialConditions, optional
+        The initial conditions class instance
+    infer_track_interior : bool, optional
+        Whether to infer the spatial geometry of track from position
+
+    """
+
     def __init__(
         self,
-        environment=Environment(environment_name=""),
-        transition_type=RandomWalk(),
-        initial_conditions_type=UniformInitialConditions(),
-        infer_track_interior=True,
+        environment: Environment = Environment(environment_name=""),
+        transition_type: Union[
+            EmpiricalMovement,
+            RandomWalk,
+            RandomWalkDirection1,
+            RandomWalkDirection2,
+            Uniform,
+        ] = RandomWalk(),
+        initial_conditions_type: UniformInitialConditions = UniformInitialConditions(),
+        infer_track_interior: bool = True,
     ):
         self.environment = environment
         self.transition_type = transition_type
         self.initial_conditions_type = initial_conditions_type
         self.infer_track_interior = infer_track_interior
 
-    def fit_environment(self, position):
+    def fit_environment(self, position: np.ndarray) -> None:
+        """Discretize the spatial environment into bins. Determine valid track positions.
+
+        Parameters
+        ----------
+        position : np.ndarray, shape (n_time, n_position_dims)
+            Position of the animal in the environment.
+        """
         self.environment.fit_place_grid(
             position, infer_track_interior=self.infer_track_interior
         )
 
     def fit_initial_conditions(self):
+        """Set the initial probability of position."""
         logger.info("Fitting initial conditions...")
         self.initial_conditions_ = self.initial_conditions_type.make_initial_conditions(
             [self.environment], [self.environment.environment_name]
         )[0]
 
     def fit_state_transition(
-        self, position, is_training=None, transition_type=RandomWalk()
+        self,
+        position: np.ndarray,
+        is_training: Optional[np.ndarray] = None,
+        transition_type: Optional[
+            Union[
+                EmpiricalMovement,
+                RandomWalk,
+                RandomWalkDirection1,
+                RandomWalkDirection2,
+                Uniform,
+            ]
+        ] = None,
     ):
         logger.info("Fitting state transition...")
+
+        if transition_type is not None:
+            self.transition_type = transition_type
+
         if isinstance(self.transition_type, EmpiricalMovement):
             if is_training is None:
                 is_training = np.ones((position.shape[0],), dtype=np.bool)
             is_training = np.asarray(is_training).squeeze()
             n_time = position.shape[0]
             encoding_group_labels = np.zeros((n_time,), dtype=np.int32)
             self.state_transition_ = self.transition_type.make_state_transition(
@@ -88,38 +137,98 @@
             )
         else:
             self.state_transition_ = self.transition_type.make_state_transition(
                 (self.environment,)
             )
 
     def fit(self):
+        """To be implemented by inheriting class"""
         raise NotImplementedError
 
     def predict(self):
+        """To be implemented by inheriting class"""
         raise NotImplementedError
 
     def save_model(self, filename="model.pkl"):
+        """Save the classifier to a pickled file.
+
+        Parameters
+        ----------
+        filename : str, optional
+
+        """
         joblib.dump(self, filename)
 
     @staticmethod
     def load_model(filename="model.pkl"):
+        """Load the classifier from a file.
+
+        Parameters
+        ----------
+        filename : str, optional
+
+        Returns
+        -------
+        classifier instance
+
+        """
         return joblib.load(filename)
 
     def copy(self):
+        """Makes a copy of the classifier"""
         return deepcopy(self)
 
+    def project_1D_position_to_2D(
+        self, results: xr.Dataset, posterior_type="acausal_posterior"
+    ) -> np.ndarray:
+        """Project the 1D most probable position into the 2D track graph space.
+
+        Only works for single environment.
+
+        Parameters
+        ----------
+        results : xr.Dataset
+        posterior_type : causal_posterior | acausal_posterior | likelihood
+
+        Returns
+        -------
+        map_position2D : np.ndarray
+
+        """
+        map_position_ind = (
+            results[posterior_type].sum("state").argmax("position").to_numpy().squeeze()
+        )
+
+        return self.environment.place_bin_centers_nodes_df_.iloc[map_position_ind][
+            ["x_position", "y_position"]
+        ].to_numpy()
+
     def _get_results(
         self,
-        results,
-        n_time,
-        time=None,
-        is_compute_acausal=True,
-        use_gpu=False,
+        results: dict,
+        n_time: int,
+        time: Optional[np.ndarray] = None,
+        is_compute_acausal: bool = True,
+        use_gpu: bool = False,
     ):
+        """Converts the results dict into a collection of labeled arrays.
 
+        Parameters
+        ----------
+        results : dict
+        n_time : int
+        time : np.ndarray
+        is_compute_acausal : bool
+        use_gpu : bool
+
+        Returns
+        -------
+        results : xr.Dataset
+
+        """
         is_track_interior = self.environment.is_track_interior_.ravel(order="F")
         n_position_bins = is_track_interior.shape[0]
         st_interior_ind = np.ix_(is_track_interior, is_track_interior)
 
         logger.info("Estimating causal posterior...")
         if not use_gpu:
             results["causal_posterior"] = np.full(
@@ -170,15 +279,30 @@
                 )
 
         if time is None:
             time = np.arange(n_time)
 
         return self.convert_results_to_xarray(results, time, data_log_likelihood)
 
-    def convert_results_to_xarray(self, results, time, data_log_likelihood):
+    def convert_results_to_xarray(
+        self, results: dict, time: np.ndarray, data_log_likelihood: float
+    ) -> xr.Dataset:
+        """Converts the results dict into a collection of labeled arrays.
+
+        Parameters
+        ----------
+        results : dict
+        time : np.ndarray
+        data_log_likelihood : float
+
+        Returns
+        -------
+        results : xr.Dataset
+
+        """
         n_position_dims = self.environment.place_bin_centers_.shape[1]
         n_time = time.shape[0]
 
         attrs = {"data_log_likelihood": data_log_likelihood}
 
         if n_position_dims > 1:
             dims = ["time", "x_position", "y_position"]
@@ -221,45 +345,70 @@
 
         return results
 
 
 class SortedSpikesDecoder(_DecoderBase):
     def __init__(
         self,
-        environment=Environment(environment_name=""),
-        transition_type=RandomWalk(),
-        initial_conditions_type=UniformInitialConditions(),
-        infer_track_interior=True,
-        sorted_spikes_algorithm="spiking_likelihood_kde",
-        sorted_spikes_algorithm_params=_DEFAULT_SORTED_SPIKES_MODEL_KWARGS,
+        environment: Environment = Environment(environment_name=""),
+        transition_type: Union[
+            EmpiricalMovement,
+            RandomWalk,
+            RandomWalkDirection1,
+            RandomWalkDirection2,
+            Uniform,
+        ] = RandomWalk(),
+        initial_conditions_type: UniformInitialConditions = UniformInitialConditions(),
+        infer_track_interior: bool = True,
+        sorted_spikes_algorithm: str = "spiking_likelihood_kde",
+        sorted_spikes_algorithm_params: dict = _DEFAULT_SORTED_SPIKES_MODEL_KWARGS,
     ):
-        """
+        """Decodes neural population representation of position from clustered cells.
 
-        Attributes
+        Parameters
         ----------
-        environment : Environment
-            The spatial environment and topology to fit
-        transition_type : (RandomWalk, Uniform, ...)
-            The continuous state transition class instance to fit
-        initial_conditions_type : InitialConditions
-            The initial conditions class instance to fit
+        environment : Environment instance, optional
+            The spatial environment to fit
+        transition_type : transition matrix instance, optional
+            Movement model for the continuous state
+        discrete_transition_type : discrete transition instance, optional
+        initial_conditions_type : initial conditions instance, optional
+            The initial conditions class instance
         infer_track_interior : bool, optional
-            Whether to infer the valid position bins
-        knot_spacing : float, optional
-            How far apart the spline knots are in position
-        spike_model_penalty : float, optional
-            L2 penalty (ridge) for the size of the regression coefficients
+            Whether to infer the spatial geometry of track from position
+        sorted_spikes_algorithm : str, optional
+            The type of algorithm. See _SORTED_SPIKES_ALGORITHMS for keys
+        sorted_spikes_algorithm_params : dict, optional
+            Parameters for the algorithm.
+
         """
         super().__init__(
             environment, transition_type, initial_conditions_type, infer_track_interior
         )
         self.sorted_spikes_algorithm = sorted_spikes_algorithm
         self.sorted_spikes_algorithm_params = sorted_spikes_algorithm_params
 
-    def fit_place_fields(self, position, spikes, is_training=None):
+    def fit_place_fields(
+        self,
+        position: np.ndarray,
+        spikes: np.ndarray,
+        is_training: Optional[np.ndarray] = None,
+    ):
+        """Fits the place intensity function.
+
+        Parameters
+        ----------
+        position : np.ndarray, shape (n_time, n_position_dims)
+            Position of the animal.
+        spikes : np.ndarray, (n_time, n_neurons)
+            Binary indicator of whether there was a spike in a given time bin for a given neuron.
+        is_training : np.ndarray, shape (n_time,), optional
+            Boolean array to indicate which data should be included in fitting of place fields, by default None
+
+        """
         logger.info("Fitting place fields...")
         if is_training is None:
             is_training = np.ones((position.shape[0],), dtype=np.bool)
         is_training = np.asarray(is_training).squeeze()
         kwargs = self.sorted_spikes_algorithm_params
         if kwargs is None:
             kwargs = {}
@@ -270,21 +419,25 @@
             place_bin_edges=self.environment.place_bin_edges_,
             edges=self.environment.edges_,
             is_track_interior=self.environment.is_track_interior_,
             is_track_boundary=self.environment.is_track_boundary_,
             **kwargs
         )
 
-    def plot_place_fields(self, sampling_frequency=1, col_wrap=5):
-        """Plots the fitted 2D place fields for each neuron.
+    def plot_place_fields(
+        self, sampling_frequency: int = 1, col_wrap: int = 5
+    ) -> xr.plot.FacetGrid:
+        """Plots the fitted place fields for each neuron.
 
         Parameters
         ----------
-        sampling_frequency : float, optional
+        sampling_frequency : int, optional
+            Number of samples per second
         col_wrap : int, optional
+            Number of columns in the subplot.
 
         Returns
         -------
         g : xr.plot.FacetGrid instance
 
         """
         try:
@@ -297,23 +450,31 @@
         except ValueError:
             g = (self.place_fields_ * sampling_frequency).plot(
                 x="position", col="neuron", col_wrap=col_wrap
             )
 
         return g
 
-    def fit(self, position, spikes, is_training=None):
-        """
+    def fit(
+        self,
+        position: np.ndarray,
+        spikes: np.ndarray,
+        is_training: Optional[np.ndarray] = None,
+    ):
+        """Fit the spatial grid, initial conditions, place field model, and
+        transition matrix.
 
         Parameters
         ----------
         position : np.ndarray, shape (n_time, n_position_dims)
+            Position of the animal.
         spikes : np.ndarray, shape (n_time, n_neurons)
-        is_training : None or bool np.ndarray, shape (n_time), optional
-            Time bins to be used for encoding.
+            Binary indicator of whether there was a spike in a given time bin for a given neuron.
+        is_training : None or np.ndarray, shape (n_time), optional
+            Boolean array to indicate which data should be included in fitting of place fields, by default None
 
         Returns
         -------
         self
 
         """
         position = atleast_2d(np.asarray(position))
@@ -323,22 +484,31 @@
         self.fit_state_transition(
             position, is_training, transition_type=self.transition_type
         )
         self.fit_place_fields(position, spikes, is_training)
 
         return self
 
-    def predict(self, spikes, time=None, is_compute_acausal=True, use_gpu=False):
-        """
+    def predict(
+        self,
+        spikes: np.ndarray,
+        time: Optional[np.ndarray] = None,
+        is_compute_acausal: bool = True,
+        use_gpu: bool = False,
+    ) -> xr.Dataset:
+        """Predict the probability of spatial position from the spikes.
 
         Parameters
         ----------
         spikes : np.ndarray, shape (n_time, n_neurons)
-        time : ndarray or None, shape (n_time,), optional
+            Binary indicator of whether there was a spike in a given time bin for a given neuron.
+        time : np.ndarray or None, shape (n_time,), optional
+            Label the time axis with these values.
         is_compute_acausal : bool, optional
+            If True, compute the acausal posterior.
         use_gpu : bool, optional
             Use GPU for the state space part of the model, not the likelihood.
 
         Returns
         -------
         results : xarray.Dataset
 
@@ -353,54 +523,66 @@
                 spikes, np.asarray(self.place_fields_)
             )
         )
         return self._get_results(results, n_time, time, is_compute_acausal, use_gpu)
 
 
 class ClusterlessDecoder(_DecoderBase):
-    """
+    """Classifies neural population representation of position from multiunit spikes and waveforms.
 
-    Attributes
+    Parameters
     ----------
-    environment : Environment
-        The spatial environment and topology to fit
-    transition_type : (RandomWalk, Uniform, ...)
-        The continuous state transition class instance to fit
-    initial_conditions_type : InitialConditions
-        The initial conditions class instance to fit
+    environment : Environment, optional
+        The spatial environment to fit
+    transition_type : EmpiricalMovement | RandomWalk | RandomWalkDirection1 | RandomWalkDirection2 | Uniform
+        The continuous state transition matrix
+    initial_conditions_type : UniformInitialConditions, optional
+        The initial conditions class instance
     infer_track_interior : bool, optional
-        Whether to infer the valid position bins
+        Whether to infer the spatial geometry of track from position
     clusterless_algorithm : str
         The type of clusterless algorithm. See _ClUSTERLESS_ALGORITHMS for keys
     clusterless_algorithm_params : dict
         Parameters for the clusterless algorithms.
+
     """
 
     def __init__(
         self,
-        environment=Environment(environment_name=""),
-        transition_type=RandomWalk(),
-        initial_conditions_type=UniformInitialConditions(),
-        infer_track_interior=True,
-        clusterless_algorithm="multiunit_likelihood",
-        clusterless_algorithm_params=_DEFAULT_CLUSTERLESS_MODEL_KWARGS,
+        environment: Environment = Environment(environment_name=""),
+        transition_type: Union[
+            EmpiricalMovement,
+            RandomWalk,
+            RandomWalkDirection1,
+            RandomWalkDirection2,
+            Uniform,
+        ] = RandomWalk(),
+        initial_conditions_type: UniformInitialConditions = UniformInitialConditions(),
+        infer_track_interior: bool = True,
+        clusterless_algorithm: str = "multiunit_likelihood",
+        clusterless_algorithm_params: dict = _DEFAULT_CLUSTERLESS_MODEL_KWARGS,
     ):
         super().__init__(
             environment, transition_type, initial_conditions_type, infer_track_interior
         )
         self.clusterless_algorithm = clusterless_algorithm
         self.clusterless_algorithm_params = clusterless_algorithm_params
 
-    def fit_multiunits(self, position, multiunits, is_training=None):
+    def fit_multiunits(
+        self,
+        position: np.ndarray,
+        multiunits: np.ndarray,
+        is_training: Optional[np.ndarray] = None,
+    ):
         """
 
         Parameters
         ----------
-        position : array_like, shape (n_time, n_position_dims)
-        multiunits : array_like, shape (n_time, n_marks, n_electrodes)
+        position : np.ndarray, shape (n_time, n_position_dims)
+        multiunits : np.ndarray, shape (n_time, n_marks, n_electrodes)
         is_training : None or array_like, shape (n_time,)
 
         """
         logger.info("Fitting multiunits...")
         if is_training is None:
             is_training = np.ones((position.shape[0],), dtype=np.bool)
         is_training = np.asarray(is_training).squeeze()
@@ -413,22 +595,32 @@
             position=position[is_training],
             multiunits=multiunits[is_training],
             place_bin_centers=self.environment.place_bin_centers_,
             is_track_interior=self.environment.is_track_interior_.ravel(order="F"),
             **kwargs
         )
 
-    def fit(self, position, multiunits, is_training=None):
-        """
+    def fit(
+        self,
+        position: np.ndarray,
+        multiunits: np.ndarray,
+        is_training: Optional[np.ndarray] = None,
+    ):
+        """Fit the spatial grid, initial conditions, place field model, and
+        transition matrices.
 
         Parameters
         ----------
-        position : array_like, shape (n_time, n_position_dims)
-        multiunits : array_like, shape (n_time, n_marks, n_electrodes)
-        is_training : None or array_like, shape (n_time,)
+        position : np.ndarray, shape (n_time, n_position_dims)
+            Position of the animal.
+        multiunits : np.ndarray, shape (n_time, n_marks, n_electrodes)
+            Array where spikes are indicated by non-Nan values that correspond to the waveform features
+            for each electrode.
+        is_training : None or np.ndarray, shape (n_time), optional
+            Boolean array to indicate which data should be included in fitting of place fields, by default None
 
         Returns
         -------
         self
 
         """
         position = atleast_2d(np.asarray(position))
@@ -439,23 +631,32 @@
         self.fit_state_transition(
             position, is_training, transition_type=self.transition_type
         )
         self.fit_multiunits(position, multiunits, is_training)
 
         return self
 
-    def predict(self, multiunits, time=None, is_compute_acausal=True, use_gpu=False):
-        """
+    def predict(
+        self,
+        multiunits: np.ndarray,
+        time: Optional[np.ndarray] = None,
+        is_compute_acausal: bool = True,
+        use_gpu: bool = False,
+    ) -> xr.Dataset:
+        """Predict the probability of spatial position and category from the multiunit spikes and waveforms.
 
         Parameters
         ----------
-        multiunits : array_like, shape (n_time, n_marks, n_electrodes)
-        time : None or np.ndarray, shape (n_time,)
+        multiunits : np.ndarray, shape (n_time, n_marks, n_electrodes)
+            Array where spikes are indicated by non-Nan values that correspond to the waveform features
+            for each electrode.
+        time : np.ndarray or None, shape (n_time,), optional
+            Label the time axis with these values.
         is_compute_acausal : bool, optional
-            Use future information to compute the posterior.
+            If True, compute the acausal posterior.
         use_gpu : bool, optional
             Use GPU for the state space part of the model, not the likelihood.
 
         Returns
         -------
         results : xarray.Dataset
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/discrete_state_transitions.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/discrete_state_transitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Classes to generate transitions between categories."""
 from dataclasses import dataclass
 
 import numpy as np
-from scipy.special import logsumexp
+import xarray as xr
 
 
 @dataclass
 class DiagonalDiscrete:
     """Transition matrix with `diagonal_value` on the value for n_states
 
     Off-diagonals are probability: (1 - `diagonal_value`) / (`n_states` - 1)
@@ -15,15 +15,15 @@
     ----------
     diagonal_value : float, optional
 
     """
 
     diagonal_value: float = 0.98
 
-    def make_state_transition(self, n_states):
+    def make_state_transition(self, n_states: int) -> np.ndarray:
         """Makes discrete state transition matrix.
 
         Parameters
         ----------
         n_states : int
 
         Returns
@@ -41,15 +41,15 @@
 
 @dataclass
 class UniformDiscrete:
     """All transitions to states (including self transitions) are the same
     probability.
     """
 
-    def make_state_transition(self, n_states):
+    def make_state_transition(self, n_states: int) -> np.ndarray:
         """Makes discrete state transition matrix.
 
         Parameters
         ----------
         n_states : int
 
         Returns
@@ -62,15 +62,15 @@
         return self.state_transition_
 
 
 @dataclass
 class RandomDiscrete:
     """All state transitions are random"""
 
-    def make_state_transition(self, n_states):
+    def make_state_transition(self, n_states: int) -> np.ndarray:
         """Makes discrete state transition matrix.
 
         Parameters
         ----------
         n_states : int
 
         Returns
@@ -92,30 +92,32 @@
     Attributes
     ----------
     state_transition : np.ndarray, shape (n_states, n_states)
     """
 
     state_transition_: np.ndarray
 
-    def make_state_transition(self, n_states):
+    def make_state_transition(self, n_states: int) -> np.ndarray:
         """Makes discrete state transition matrix.
 
         Parameters
         ----------
         n_states : int
 
         Returns
         -------
         discrete_state_transition : np.ndarray, shape (n_states, n_states)
 
         """
         return self.state_transition_
 
 
-def expected_duration(discrete_state_transition, sampling_frequency=1):
+def expected_duration(
+    discrete_state_transition: np.ndarray, sampling_frequency: int = 1
+):
     """The average duration of each discrete state if it follows
     a geometric distribution.
 
     Use `sampling_frequency` to convert duration to seconds. Time is in
     number of samples by default.
 
     Parameters
@@ -128,16 +130,30 @@
     duration : np.ndarray, shape (n_states)
 
     """
     self_transitions = np.diag(discrete_state_transition)
     return (1 / (1 - self_transitions)) / sampling_frequency
 
 
-def estimate_discrete_state_transition(classifier, results):
+def estimate_discrete_state_transition(
+    classifier,
+    results: xr.Dataset,
+) -> np.ndarray:
+    """Estimate a new discrete transition matrix given the old one and updated smoother results.
 
+    Parameters
+    ----------
+    classifier : ClusterlessClassifier or SortedSpikesClassifier instance
+    results : xr.Dataset
+
+    Returns
+    -------
+    new_transition_matrix : np.ndarray, shape (n_states, n_states)
+
+    """
     likelihood = results.likelihood.sum("position").values
     causal_prob = results.causal_posterior.sum("position").values
     acausal_prob = results.acausal_posterior.sum("position").values
     transition_matrix = classifier.discrete_state_transition_
 
     n_time, n_states = causal_prob.shape
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/environments.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/environments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Classes for constructing discrete grids representations of spatial environments in 1D and 2D"""
 from dataclasses import dataclass
+from typing import Optional, Union
 
 import joblib
+import matplotlib
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 import pandas as pd
 from numba import njit
 from scipy import ndimage
 from scipy.interpolate import interp1d
@@ -61,18 +63,34 @@
     is_track_interior: np.ndarray = None
     position_range: np.ndarray = None
     infer_track_interior: bool = True
     fill_holes: bool = False
     dilate: bool = False
     bin_count_threshold: int = 0
 
-    def __eq__(self, other):
+    def __eq__(self, other: str) -> bool:
         return self.environment_name == other
 
-    def fit_place_grid(self, position=None, infer_track_interior=True):
+    def fit_place_grid(
+        self, position: Optional[np.ndarray] = None, infer_track_interior: bool = True
+    ):
+        """Fits a discrete grid of the spatial environment.
+
+        Parameters
+        ----------
+        position : np.ndarray, optional
+            Position of the animal.
+        infer_track_interior : bool, optional
+            Whether to infer the spatial geometry of track from position
+
+        Returns
+        -------
+        self
+
+        """
         if self.track_graph is None:
             (
                 self.edges_,
                 self.place_bin_edges_,
                 self.place_bin_centers_,
                 self.centers_shape_,
             ) = get_grid(
@@ -120,41 +138,76 @@
                 self.edge_spacing,
                 self.place_bin_size,
             )
             self.is_track_boundary_ = None
 
         return self
 
-    def plot_grid(self, ax=None):
+    def plot_grid(self, ax: matplotlib.axes.Axes = None):
+        """Plot the fitted spatial grid of the environment.
+
+        Parameters
+        ----------
+        ax : plt.axes, optional
+            Plot on this axis if given, by default None
+
+        """
         if self.track_graph is not None:
             if ax is None:
-                fig, ax = plt.subplots(figsize=(15, 2))
+                _, ax = plt.subplots(figsize=(15, 2))
 
             plot_graph_as_1D(
                 self.track_graph, self.edge_order, self.edge_spacing, ax=ax
             )
             for edge in self.edges_[0]:
                 ax.axvline(edge.squeeze(), linewidth=0.5, color="black")
             ax.set_ylim((0, 0.1))
         else:
             if ax is None:
-                fig, ax = plt.subplots(figsize=(6, 7))
+                _, ax = plt.subplots(figsize=(6, 7))
             ax.pcolormesh(
                 self.edges_[0], self.edges_[1], self.is_track_interior_.T, cmap="bone_r"
             )
             ax.set_xticks(self.edges_[0], minor=True)
             ax.set_yticks(self.edges_[1], minor=True)
             ax.grid(visible=True, which="minor")
             ax.grid(visible=False, which="major")
 
-    def save_environment(self, filename="environment.pkl"):
-        joblib.dump(self, filename)
+    def save_environment(self, filename: str = "environment.pkl"):
+        """Saves the environment as a pickled file.
 
+        Parameters
+        ----------
+        filename : str, optional
+            File name to pickle the environment to, by default "environment.pkl"
 
-def get_n_bins(position, bin_size=2.5, position_range=None):
+        """
+        joblib.dump(self, filename)
+
+    @staticmethod
+    def load_environment(filename: str = "environment.pkl"):
+        """Load the environment from a file.
+
+        Parameters
+        ----------
+        filename : str, optional
+
+        Returns
+        -------
+        environment instance
+
+        """
+        return joblib.load(filename)
+
+
+def get_n_bins(
+    position: np.ndarray,
+    bin_size: float = 2.5,
+    position_range: Optional[list[np.ndarray]] = None,
+) -> int:
     """Get number of bins need to span a range given a bin size.
 
     Parameters
     ----------
     position : np.ndarray, shape (n_time,)
     bin_size : float, optional
     position_range : None or list of np.ndarray
@@ -169,15 +222,19 @@
         extent = np.diff(position_range, axis=1).squeeze()
     else:
         extent = np.ptp(position, axis=0)
 
     return np.ceil(extent / bin_size).astype(np.int32)
 
 
-def get_grid(position, bin_size=2.5, position_range=None):
+def get_grid(
+    position: np.ndarray,
+    bin_size: float = 2.5,
+    position_range: Optional[list[np.ndarray]] = None,
+) -> tuple[np.ndarray, np.ndarray, np.ndarray, tuple]:
     """Gets the spatial grid of bins.
 
     Parameters
     ----------
     position : np.ndarray, shape (n_time, n_position_dims)
     bin_size : float, optional
         Maximum size of each position bin.
@@ -216,16 +273,20 @@
     place_bin_centers = np.stack([center.ravel() for center in mesh_centers], axis=1)
     centers_shape = mesh_centers[0].T.shape
 
     return edges, place_bin_edges, place_bin_centers, centers_shape
 
 
 def get_track_interior(
-    position, bins, fill_holes=False, dilate=False, bin_count_threshold=0
-):
+    position: np.ndarray,
+    bins: int,
+    fill_holes: bool = False,
+    dilate: bool = False,
+    bin_count_threshold: int = 0,
+) -> np.ndarray:
     """Infers the interior bins of the track given positions.
 
     Parameters
     ----------
     position : np.ndarray, shape (n_time, n_position_dims)
     bins : sequence or int, optional
         The bin specification:
@@ -262,15 +323,15 @@
             is_track_interior = ndimage.binary_dilation(is_track_interior)
         # adjust for boundary edges in 2D
         is_track_interior[-1] = False
         is_track_interior[:, -1] = False
     return is_track_interior.astype(bool)
 
 
-def get_track_segments_from_graph(track_graph):
+def get_track_segments_from_graph(track_graph: nx.Graph) -> np.ndarray:
     """Returns a 2D array of node positions corresponding to each edge.
 
     Parameters
     ----------
     track_graph : networkx Graph
 
     Returns
@@ -283,15 +344,17 @@
         [
             (node_positions[node1], node_positions[node2])
             for node1, node2 in track_graph.edges()
         ]
     )
 
 
-def project_points_to_segment(track_segments, position):
+def project_points_to_segment(
+    track_segments: np.ndarray, position: np.ndarray
+) -> np.ndarray:
     """Finds the closet point on a track segment in terms of Euclidean distance
 
     Parameters
     ----------
     track_segments : np.ndarray, shape (n_segments, n_nodes, 2)
     position : np.ndarray, shape (n_time, 2)
 
@@ -311,16 +374,20 @@
     nx[np.where(nx > 1)] = 1.0
     return node1[np.newaxis, ...] + (
         nx[:, :, np.newaxis] * segment_diff[np.newaxis, ...]
     )
 
 
 def _calculate_linear_position(
-    track_graph, position, track_segment_id, edge_order, edge_spacing
-):
+    track_graph: nx.Graph,
+    position: np.ndarray,
+    track_segment_id: np.ndarray,
+    edge_order: list[tuple],
+    edge_spacing: Union[float, list],
+) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Determines the linear position given a 2D position and a track graph.
 
     Parameters
     ----------
     track_graph : nx.Graph
     position : np.ndarray, shape (n_time, n_position_dims)
     track_segment_id : np.ndarray, shape (n_time,)
@@ -392,15 +459,17 @@
     return (
         linear_position,
         projected_track_positions[:, 0],
         projected_track_positions[:, 1],
     )
 
 
-def make_track_graph_with_bin_centers_edges(track_graph, place_bin_size):
+def make_track_graph_with_bin_centers_edges(
+    track_graph: nx.Graph, place_bin_size: float
+) -> nx.Graph:
     """Insert the bin center and bin edge positions as nodes in the track graph.
 
     Parameters
     ----------
     track_graph : nx.Graph
     place_bin_size : float
 
@@ -456,16 +525,19 @@
         track_graph_with_bin_centers_edges.nodes[node2]["is_bin_edge"] = True
         n_nodes = len(track_graph_with_bin_centers_edges.nodes)
 
     return track_graph_with_bin_centers_edges
 
 
 def extract_bin_info_from_track_graph(
-    track_graph, track_graph_with_bin_centers_edges, edge_order, edge_spacing
-):
+    track_graph: nx.Graph,
+    track_graph_with_bin_centers_edges: nx.Graph,
+    edge_order: list[tuple],
+    edge_spacing: Union[float, list],
+) -> pd.DataFrame:
     """For each node, find edge_id, is_bin_edge, x_position, y_position, and
     linear_position.
 
     Parameters
     ----------
     track_graph : nx.Graph
     track_graph_with_bin_centers_edges : nx.Graph
@@ -507,15 +579,32 @@
         .set_index("node_id")
         .drop(columns="edge_avg_linear_position")
     )
 
     return nodes_df
 
 
-def get_track_grid(track_graph, edge_order, edge_spacing, place_bin_size):
+def get_track_grid(
+    track_graph: nx.Graph,
+    edge_order: list[tuple],
+    edge_spacing: Union[float, list],
+    place_bin_size: float,
+) -> tuple[
+    np.ndarray,
+    np.ndarray,
+    np.ndarray,
+    dict,
+    tuple,
+    tuple,
+    nx.Graph,
+    pd.DataFrame,
+    pd.DataFrame,
+    pd.DataFrame,
+    pd.DataFrame,
+]:
     """Figures out 1D spatial bins given a track graph.
 
     Parameters
     ----------
     track_graph : nx.Graph
     edge_order : list of 2-tuples
     edge_spacing : list, len n_edges - 1
@@ -626,15 +715,17 @@
         original_nodes_df,
         place_bin_edges_nodes_df,
         place_bin_centers_nodes_df,
         nodes_df.reset_index(),
     )
 
 
-def get_track_boundary(is_track_interior, n_position_dims=2, connectivity=1):
+def get_track_boundary(
+    is_track_interior: np.ndarray, n_position_dims: int = 2, connectivity: int = 1
+) -> np.ndarray:
     """Determines the boundary of the valid interior track bins. The boundary
     are not bins on the track but surround it.
 
     Parameters
     ----------
     is_track_interior : np.ndarray, shape (n_bins_x, n_bins_y)
     n_position_dims : int
@@ -656,18 +747,27 @@
     )
     return (
         ndimage.binary_dilation(is_track_interior, structure=structure)
         ^ is_track_interior
     )
 
 
-def order_boundary(boundary):
+def order_boundary(boundary: np.ndarray) -> np.ndarray:
     """Given boundary bin centers, orders them in a way to make a continuous line.
 
     https://stackoverflow.com/questions/37742358/sorting-points-to-form-a-continuous-line
+
+    Parameters
+    ----------
+    boundary : np.ndarray, shape (n_boundary_points, n_position_dims)
+
+    Returns
+    -------
+    ordered_boundary : np.ndarray, shape (n_boundary_points, n_position_dims)
+
     """
     n_points = boundary.shape[0]
     clf = NearestNeighbors(n_neighbors=2).fit(boundary)
     G = clf.kneighbors_graph()
     T = nx.from_scipy_sparse_matrix(G)
 
     paths = [list(nx.dfs_preorder_nodes(T, i)) for i in range(n_points)]
@@ -679,22 +779,28 @@
         if cost < min_dist:
             min_idx, min_dist = idx, cost
 
     opt_order = paths[min_idx]
     return boundary[opt_order][:-1]
 
 
-def get_track_boundary_points(is_track_interior, edges, connectivity=1):
+def get_track_boundary_points(
+    is_track_interior: np.ndarray, edges: list[np.ndarray], connectivity: int = 1
+):
     """
 
     Parameters
     ----------
     is_track_interior : np.ndarray, shape (n_x_bins, n_y_bins)
     edges : list of ndarray
 
+    Returns
+    -------
+    boundary_points : np.ndarray, shape (n_boundary_points, n_position_dims)
+
     """
     n_position_dims = len(edges)
     boundary = get_track_boundary(
         is_track_interior, n_position_dims=n_position_dims, connectivity=connectivity
     )
 
     inds = np.nonzero(boundary)
@@ -706,15 +812,15 @@
 @njit
 def diffuse(
     position_grid: np.ndarray,
     Fx: float,
     Fy: float,
     is_track_interior: np.ndarray,
     is_track_boundary: np.ndarray,
-):
+) -> np.ndarray:
     """Calculates diffusion for a single time step given a track.
 
     Parameters
     ----------
     position_grid : np.ndarray, shape (n_bins_x, n_bins_y)
         Function to diffusion
     Fx : float
@@ -762,18 +868,18 @@
 @njit
 def run_diffusion(
     position_grid: np.ndarray,
     is_track_interior: np.ndarray,
     is_track_boundary: np.ndarray,
     dx: float,
     dy: float,
-    std=6.0,
-    alpha=0.5,
-    dt=0.250,
-):
+    std: float = 6.0,
+    alpha: float = 0.5,
+    dt: float = 0.250,
+) -> np.ndarray:
     """Calculates diffusion of a single point over time up until it matches a
     Gaussian with standard deviation `std`.
 
     Parameters
     ----------
     position_grid : np.ndarray, shape (n_bins_x, n_bins_y)
         Function to diffusion
@@ -813,17 +919,17 @@
 
 @njit
 def diffuse_each_bin(
     is_track_interior: np.ndarray,
     is_track_boundary: np.ndarray,
     dx: float,
     dy: float,
-    std=6.0,
-    alpha=0.5,
-):
+    std: float = 6.0,
+    alpha: float = 0.5,
+) -> np.ndarray:
     """
     For each position bin in the grid, diffuse by `std`.
 
     Parameters
     ----------
     is_track_interior : np.ndarray, shape (n_bins_x, n_bins_y)
         Boolean that denotes which bins that are on the track
@@ -867,18 +973,29 @@
             alpha=alpha,
             dt=dt,
         )
 
     return diffused_grid
 
 
-def get_bin_ind(sample, edges):
+def get_bin_ind(sample: np.ndarray, edges: list[np.ndarray]) -> np.ndarray:
     """Figure out which bin a given sample falls into.
 
-    Extracted from np.histogramdd."""
+    Extracted from np.histogramdd.
+
+    Parameters
+    ----------
+    sample : np.ndarray
+    edges : list of np.ndarray
+
+    Returns
+    -------
+    Ncount : np.ndarray
+
+    """
 
     try:
         # Sample is an ND-array.
         N, D = sample.shape
     except (AttributeError, ValueError):
         # Sample is a sequence of 1D arrays.
         sample = np.atleast_2d(sample).T
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/initial_conditions.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/initial_conditions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,36 @@
-"""Classes for setting the initial conditions for the state space models."""
+"""Classes for constructing the initial conditions for the state space models."""
 
 from dataclasses import dataclass
+from replay_trajectory_classification.environments import Environment
 
 import numpy as np
 
 
 @dataclass
 class UniformInitialConditions:
     """Initial conditions where all discrete states and position bins are
     equally likely."""
 
     def make_initial_conditions(
-        self, environments: tuple, environment_names_to_state: tuple
-    ):
+        self, environments: tuple[Environment], environment_names_to_state: tuple[str]
+    ) -> list[np.ndarray]:
+        """Creates initial conditions array
+
+        Parameters
+        ----------
+        environments : tuple[Environment]
+            Spatial environments in the model
+        environment_names_to_state : tuple[str]
+            Mapping of environment names to state
+
+        Returns
+        -------
+        initial_conditions : list of arrays
+        """
         n_total_place_bins = 0
         initial_conditions = []
 
         for environment_name in environment_names_to_state:
             is_track_interior = environments[
                 environments.index(environment_name)
             ].is_track_interior_.ravel(order="F")
@@ -30,16 +44,29 @@
 class UniformOneEnvironmentInitialConditions:
     """Initial conditions where all position bins are
     equally likely for one environment and zero for other environments."""
 
     environment_name: str = ""
 
     def make_initial_conditions(
-        self, environments: tuple, environment_names_to_state: tuple
-    ):
+        self, environments: tuple[Environment], environment_names_to_state: tuple[str]
+    ) -> list[np.ndarray]:
+        """Creates initial conditions array
+
+        Parameters
+        ----------
+        environments : tuple[Environment]
+            Spatial environments in the model
+        environment_names_to_state : tuple[str]
+            Mapping of environment names to state
+
+        Returns
+        -------
+        initial_conditions : list of arrays
+        """
         n_total_place_bins = 0
         initial_conditions = []
 
         for environment_name in environment_names_to_state:
             is_track_interior = environments[
                 environments.index(environment_name)
             ].is_track_interior_.ravel(order="F")
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/__init__.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Functions to fit the position intensities and likelihoods for each data type"""
 # flake8: noqa
 from replay_trajectory_classification.likelihoods.calcium_likelihood import (
     estimate_calcium_likelihood,
     estimate_calcium_place_fields,
 )
 from replay_trajectory_classification.likelihoods.multiunit_likelihood import (
     estimate_multiunit_likelihood,
@@ -64,7 +65,11 @@
         estimate_spiking_likelihood_kde,
     ),
     "spiking_likelihood_kde_gpu": (
         estimate_place_fields_kde_gpu,
         estimate_spiking_likelihood_kde_gpu,
     ),
 }
+
+_CALCIUM_ALGORITHMS = {
+    "calcium_likelihood": (estimate_calcium_place_fields, estimate_calcium_likelihood)
+}
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/calcium_likelihood.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/calcium_likelihood.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,37 +3,41 @@
 References
 ----------
 [1] Farhoodi, S., Plitt, M.H., Giocomo, L., and Eden, U.T. (2020). Estimating Fluctuations in Neural Representations of Uncertain Environments. 20. .
 
 """
 
 import logging
+from typing import Optional
 
 import dask
 import numpy as np
 import pandas as pd
 import xarray as xr
 from dask.distributed import Client, get_client
-from patsy import build_design_matrices, dmatrix
+from patsy import DesignInfo, DesignMatrix, build_design_matrices, dmatrix
 from regularized_glm import penalized_IRLS
-from replay_trajectory_classification.environments import get_n_bins
 from statsmodels.api import families
 
+from replay_trajectory_classification.environments import get_n_bins
+
 
-def make_spline_design_matrix(position, place_bin_edges, knot_spacing=10):
+def make_spline_design_matrix(
+    position: np.ndarray, place_bin_edges: np.ndarray, knot_spacing: int = 10
+) -> DesignMatrix:
     """Creates a design matrix for regression with a position spline basis.
 
     Parameters
     ----------
     position : np.ndarray, shape (n_time, n_position_dims)
     place_bin_edges : np.ndarray, shape (n_bins, n_position_dims)
 
     Returns
     -------
-    design_matrix : statsmodels.DesignMatrix
+    design_matrix : patsy.DesignMatrix
 
     """
     # TODO: Add history dependence
     inner_knots = []
     for pos, edges in zip(position.T, place_bin_edges.T):
         n_points = get_n_bins(edges, bin_size=knot_spacing)
         knots = np.linspace(edges.min(), edges.max(), n_points)[1:-1]
@@ -51,31 +55,38 @@
         data[f"x{ind}"] = position[:, ind]
 
     formula += 'constraints="center")'
 
     return dmatrix(formula, data)
 
 
-def make_spline_predict_matrix(design_info, place_bin_centers):
+def make_spline_predict_matrix(
+    design_info: DesignInfo, place_bin_centers: np.ndarray
+) -> DesignMatrix:
     """Make a design matrix for position bins"""
     predict_data = {}
     for ind in range(place_bin_centers.shape[1]):
         predict_data[f"x{ind}"] = place_bin_centers[:, ind]
     return build_design_matrices([design_info], predict_data)[0]
 
 
-def get_activity_rate(design_matrix, results):
+def get_activity_rate(design_matrix: DesignMatrix, results: tuple) -> np.ndarray:
     """Predicts the calcium activity trace given fitted model coefficents."""
     rate = design_matrix @ results.coefficients
     rate[rate < 0.1] = 0.1
     return rate
 
 
 @dask.delayed
-def fit_glm(response, design_matrix, penalty=None, tolerance=1e-5):
+def fit_glm(
+    response: np.ndarray,
+    design_matrix: np.ndarray,
+    penalty: Optional[float] = None,
+    tolerance: float = 1e-5,
+) -> tuple:
     """Fits a L2-penalized GLM.
 
     Parameters
     ----------
     response : np.ndarray, shape (n_time,)
         Calcium activity trace
     design_matrix : np.ndarray, shape (n_time, n_coefficients)
@@ -100,26 +111,28 @@
         response.squeeze(),
         family=families.Gamma(families.links.identity()),
         penalty=penalty,
         tolerance=tolerance,
     )
 
 
-def gamma_log_likelihood(calcium_activity, place_field, scale):
+def gamma_log_likelihood(
+    calcium_activity: np.ndarray, place_field: np.ndarray, scale: float
+) -> np.ndarray:
     """Probability of parameters given spiking at a particular time.
 
     Parameters
     ----------
     calcium_activity : np.ndarray, shape (n_time,)
     place_field : np.ndaarray, shape (n_place_bins,)
     scale : float
 
     Returns
     -------
-    gamma_log_likelihood : array_like, shape (n_time, n_place_bins)
+    gamma_log_likelihood : np.ndarray, shape (n_time, n_place_bins)
 
     """
     # return scipy.stats.gamma.logpdf(v * calcium_activity / mu, v)
     # return scipy.stats.gamma.logpdf(mu, v)
     # return (-scipy.special.loggamma(v) +
     #         v * np.log(v * calcium_activity / mu) -
     #         v * calcium_activity / mu -
@@ -128,15 +141,17 @@
     return gamma.loglike_obs(
         endog=calcium_activity[:, np.newaxis],
         mu=place_field[np.newaxis, :],
         scale=scale,
     )
 
 
-def combined_likelihood(calcium_activity, place_fields, scales):
+def combined_likelihood(
+    calcium_activity: np.ndarray, place_fields: np.ndarray, scales: np.ndarray
+) -> np.ndarray:
     """Combines the likelihoods of all the cells.
 
     Parameters
     ----------
     calcium_activity : np.ndarray, shape (n_time, n_neurons)
         Deconvolved activity rate estimated from the fluorescence level.
     place_fields : np.ndarray, shape (n_bins, n_neurons)
@@ -150,16 +165,19 @@
     for activity, place_field, scale in zip(calcium_activity.T, place_fields.T, scales):
         log_likelihood += gamma_log_likelihood(activity, place_field, scale)
 
     return log_likelihood
 
 
 def estimate_calcium_likelihood(
-    calcium_activity, place_fields, scales, is_track_interior=None
-):
+    calcium_activity: np.ndarray,
+    place_fields: np.ndarray,
+    scales: np.ndarray,
+    is_track_interior: Optional[np.ndarray] = None,
+) -> np.ndarray:
     """Find the likelihood given a fitted place field model.
 
     Parameters
     ----------
     calcium_activity : np.ndarray, shape (n_time, n_neurons)
         Deconvolved activity rate estimated from the fluorescence level.
     place_fields : np.ndarray, shape (n_bins, n_neurons)
@@ -181,21 +199,21 @@
     mask = np.ones_like(is_track_interior, dtype=np.float)
     mask[~is_track_interior] = np.nan
 
     return log_likelihood * mask
 
 
 def estimate_calcium_place_fields(
-    position,
-    calcium_activity,
-    place_bin_centers,
-    place_bin_edges,
-    penalty=1e-1,
-    knot_spacing=10,
-):
+    position: np.ndarray,
+    calcium_activity: np.ndarray,
+    place_bin_centers: np.ndarray,
+    place_bin_edges: np.ndarray,
+    penalty: float = 1e-1,
+    knot_spacing: int = 10,
+) -> xr.DataArray:
     """Gives the conditional intensity of the neurons' spiking with respect to
     position.
 
     Parameters
     ----------
     position : np.ndarray, shape (n_time, n_position_dims)
     calcium_activity : np.ndarray, shape (n_time, n_neurons)
@@ -203,15 +221,15 @@
     place_bin_centers : np.ndarray, shape (n_bins, n_position_dims)
     place_bin_edges : np.ndarray, shape (n_bins + 1, n_position_dims)
     penalty : float, optional
     knot_spacing : int, optional
 
     Returns
     -------
-    conditional_intensity : np.ndarray, shape (n_bins, n_neurons)
+    conditional_intensity :xr.DataArray, shape (n_bins, n_neurons)
 
     """
     if np.any(np.ptp(place_bin_edges, axis=0) <= knot_spacing):
         logging.warning("Range of position is smaller than knot spacing.")
     design_matrix = make_spline_design_matrix(position, place_bin_edges, knot_spacing)
     design_info = design_matrix.design_info
     try:
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/diffusion.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/diffusion.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Calculate diffusion distances by simulating diffusion at
 each position bin. This can be used for more accurate 2D kernel density
 estimates with boundaries."""
 
 import numpy as np
 from replay_trajectory_classification.environments import diffuse_each_bin, get_bin_ind
 
+from typing import Optional
+
 
 def estimate_diffusion_position_distance(
-    positions,
-    edges,
-    is_track_interior=None,
-    is_track_boundary=None,
-    position_std=3.0,
-    bin_distances=None,
-):
+    positions: np.ndarray,
+    edges: np.ndarray,
+    is_track_interior: Optional[np.ndarray] = None,
+    is_track_boundary: Optional[np.ndarray] = None,
+    position_std: float = 3.0,
+    bin_distances: Optional[np.ndarray] = None,
+) -> np.ndarray:
     """Estimates a distance between a given position and all position bins
     using a diffusion.
 
     Parameters
     ----------
     positions : np.ndarray, shape (n_time, n_position_dims)
     position_std : float
@@ -45,22 +47,22 @@
     linear_ind = np.ravel_multi_index(
         bin_ind, [len(edge) - 1 for edge in edges], order="F"
     )
     return bin_distances[linear_ind]
 
 
 def estimate_diffusion_position_density(
-    positions,
-    edges,
-    is_track_interior=None,
-    is_track_boundary=None,
-    position_std=3.0,
-    bin_distances=None,
-    block_size=100,
-):
+    positions: np.ndarray,
+    edges: np.ndarray,
+    is_track_interior: Optional[np.ndarray] = None,
+    is_track_boundary: Optional[np.ndarray] = None,
+    position_std: float = 3.0,
+    bin_distances: Optional[np.ndarray] = None,
+    block_size: Optional[int] = 100,
+) -> np.ndarray:
     """Kernel density estimate over all position bins using diffusion.
 
     Parameters
     ----------
     place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
     positions : np.ndarray, shape (n_time, n_position_dims)
     position_std : float
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """Estimates a marked point process likelihood where the marks are
  features of the spike waveform. Features are float32."""
 
 
+from typing import Optional, Union
+
 import numpy as np
+from tqdm.autonotebook import tqdm
+
 from replay_trajectory_classification.core import atleast_2d
 from replay_trajectory_classification.likelihoods.diffusion import (
     diffuse_each_bin,
     estimate_diffusion_position_density,
     estimate_diffusion_position_distance,
 )
-from tqdm.autonotebook import tqdm
 
 
-def gaussian_pdf(x, mean, sigma):
+def gaussian_pdf(x: np.ndarray, mean: np.ndarray, sigma: np.ndarray) -> np.ndarray:
     """Compute the value of a Gaussian probability density function at x with
     given mean and sigma."""
     return np.exp(-0.5 * ((x - mean) / sigma) ** 2) / (sigma * np.sqrt(2.0 * np.pi))
 
 
-def estimate_position_distance(place_bin_centers, positions, position_std):
+def estimate_position_distance(
+    place_bin_centers: np.ndarray, positions: np.ndarray, position_std: np.ndarray
+) -> np.ndarray:
     """Estimates the Euclidean distance between positions and position bins.
 
     Parameters
     ----------
     place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
     positions : np.ndarray, shape (n_time, n_position_dims)
     position_std : array_like, shape (n_position_dims,)
@@ -47,16 +52,19 @@
             std,
         )
 
     return position_distance
 
 
 def estimate_position_density(
-    place_bin_centers, positions, position_std, block_size=100
-):
+    place_bin_centers: np.ndarray,
+    positions: np.ndarray,
+    position_std: np.ndarray,
+    block_size: int = 100,
+) -> np.ndarray:
     """Estimates a kernel density estimate over position bins using
     Euclidean distances.
 
     Parameters
     ----------
     place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
     positions : np.ndarray, shape (n_time, n_position_dims)
@@ -81,20 +89,24 @@
                 place_bin_centers[block_inds], positions, position_std
             ),
             axis=0,
         )
     return position_density
 
 
-def estimate_log_intensity(density, occupancy, mean_rate):
+def estimate_log_intensity(
+    density: np.ndarray, occupancy: np.ndarray, mean_rate: float
+) -> np.ndarray:
     """Calculates intensity in log space."""
     return np.log(mean_rate) + np.log(density) - np.log(occupancy)
 
 
-def estimate_intensity(density, occupancy, mean_rate):
+def estimate_intensity(
+    density: np.ndarray, occupancy: np.ndarray, mean_rate: float
+) -> np.ndarray:
     """Calculates intensity.
 
     Parameters
     ----------
     density : np.ndarray, shape (n_bins,)
     occupancy : np.ndarray, shape (n_bins,)
     mean_rate : float
@@ -104,25 +116,25 @@
     intensity : np.ndarray, shape (n_bins,)
 
     """
     return np.exp(estimate_log_intensity(density, occupancy, mean_rate))
 
 
 def estimate_log_joint_mark_intensity(
-    decoding_marks,
-    encoding_marks,
-    mark_std,
-    occupancy,
-    mean_rate,
-    place_bin_centers=None,
-    encoding_positions=None,
-    position_std=None,
-    max_mark_diff=6000,
-    set_diag_zero=False,
-    position_distance=None,
+    decoding_marks: np.ndarray,
+    encoding_marks: np.ndarray,
+    mark_std: np.ndarray,
+    occupancy: np.ndarray,
+    mean_rate: float,
+    place_bin_centers: Optional[np.ndarray] = None,
+    encoding_positions: Optional[np.ndarray] = None,
+    position_std: Union[np.ndarray, float, None] = None,
+    max_mark_diff: int = 6000,
+    set_diag_zero: bool = False,
+    position_distance: Optional[np.ndarray] = None,
 ):
     """Finds the joint intensity of the marks and positions in log space.
 
     Parameters
     ----------
     decoding_marks : np.ndarray, shape (n_decoding_spikes, n_features)
     encoding_marks : np.ndarray, shape (n_encoding_spikes, n_features)
@@ -168,26 +180,26 @@
 
     return estimate_log_intensity(
         mark_distance @ position_distance / n_encoding_spikes, occupancy, mean_rate
     )
 
 
 def fit_multiunit_likelihood(
-    position,
-    multiunits,
-    place_bin_centers,
-    mark_std,
-    position_std,
-    is_track_boundary=None,
-    is_track_interior=None,
-    edges=None,
-    block_size=100,
-    use_diffusion=False,
+    position: np.ndarray,
+    multiunits: np.ndarray,
+    place_bin_centers: np.ndarray,
+    mark_std: Union[np.ndarray, float],
+    position_std: Union[np.ndarray, float],
+    is_track_boundary: Optional[np.ndarray] = None,
+    is_track_interior: Optional[np.ndarray] = None,
+    edges: Optional[list[np.ndarray]] = None,
+    block_size: int = 100,
+    use_diffusion: bool = False,
     **kwargs
-):
+) -> dict:
     """Fits the clusterless place field model.
 
     Parameters
     ----------
     position : np.ndarray, shape (n_time, n_position_dims)
     multiunits : np.ndarray, shape (n_time, n_marks, n_electrodes)
     place_bin_centers : np.ndarray, shape (n_bins, n_position_dims)
@@ -318,34 +330,34 @@
         "use_diffusion": use_diffusion,
         "edges": edges,
         **kwargs,
     }
 
 
 def estimate_multiunit_likelihood(
-    multiunits,
-    encoding_marks,
-    mark_std,
-    place_bin_centers,
-    encoding_positions,
-    position_std,
-    occupancy,
-    mean_rates,
-    summed_ground_process_intensity,
-    bin_diffusion_distances,
-    edges,
-    max_mark_diff=6000,
-    set_diag_zero=False,
-    is_track_interior=None,
-    time_bin_size=1,
-    block_size=100,
-    ignore_no_spike=False,
-    disable_progress_bar=False,
-    use_diffusion=False,
-):
+    multiunits: np.ndarray,
+    encoding_marks: np.ndarray,
+    mark_std: np.ndarray,
+    place_bin_centers: np.ndarray,
+    encoding_positions: np.ndarray,
+    position_std: Union[float, np.ndarray],
+    occupancy: np.ndarray,
+    mean_rates: np.ndarray,
+    summed_ground_process_intensity: np.ndarray,
+    bin_diffusion_distances: np.ndarray,
+    edges: list[np.ndarray],
+    max_mark_diff: int = 6000,
+    set_diag_zero: bool = False,
+    is_track_interior: Optional[np.ndarray] = None,
+    time_bin_size: int = 1,
+    block_size: int = 100,
+    ignore_no_spike: bool = False,
+    disable_progress_bar: bool = False,
+    use_diffusion: bool = False,
+) -> np.ndarray:
     """Estimates the likelihood of position bins given multiunit marks.
 
     Parameters
     ----------
     multiunits : np.ndarray, shape (n_decoding_time, n_marks, n_electrodes)
     encoding_marks : np.ndarray, shape (n_encoding_spikes, n_marks, n_electrodes)
     mark_std : list, shape (n_marks,)
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood_gpu.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,483 +1,497 @@
 """Estimates a marked point process likelihood where the marks are
- features of the spike waveform using GPUs. Features are float32."""
+ features of the spike waveform. Mark features are int16.
+
+ Marks are converted to integers and KDE uses hash tables to compute Gaussian
+ kernels."""
+
+
+from typing import Optional, Union
 
 import numpy as np
+from tqdm.autonotebook import tqdm
+
 from replay_trajectory_classification.core import atleast_2d
 from replay_trajectory_classification.likelihoods.diffusion import (
     diffuse_each_bin,
     estimate_diffusion_position_density,
     estimate_diffusion_position_distance,
 )
-from tqdm.autonotebook import tqdm
-
-try:
-    import cupy as cp
-
-    @cp.fuse
-    def gaussian_pdf(x, mean, sigma):
-        """Compute the value of a Gaussian probability density function at x with
-        given mean and sigma."""
-        return cp.exp(-0.5 * ((x - mean) / sigma) ** 2) / (sigma * cp.sqrt(2.0 * cp.pi))
-
-    def estimate_position_distance(place_bin_centers, positions, position_std):
-        """Estimates the Euclidean distance between positions and position bins.
-
-        Parameters
-        ----------
-        place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
-        positions : np.ndarray, shape (n_time, n_position_dims)
-        position_std : array_like, shape (n_position_dims,)
-
-        Returns
-        -------
-        position_distance : np.ndarray, shape (n_time, n_position_bins)
-
-        """
-        n_time, n_position_dims = positions.shape
-        n_position_bins = place_bin_centers.shape[0]
-
-        if isinstance(position_std, (int, float)):
-            position_std = [position_std] * n_position_dims
-
-        position_distance = cp.ones((n_time, n_position_bins), dtype=cp.float32)
-
-        for position_ind, std in enumerate(position_std):
-            position_distance *= gaussian_pdf(
-                cp.expand_dims(place_bin_centers[:, position_ind], axis=0),
-                cp.expand_dims(positions[:, position_ind], axis=1),
-                std,
-            )
-
-        return position_distance
-
-    def estimate_position_density(
-        place_bin_centers, positions, position_std, block_size=100
-    ):
-        """Estimates a kernel density estimate over position bins using
-        Euclidean distances.
-
-        Parameters
-        ----------
-        place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
-        positions : np.ndarray, shape (n_time, n_position_dims)
-        position_std : float or array_like, shape (n_position_dims,)
-
-        Returns
-        -------
-        position_density : np.ndarray, shape (n_position_bins,)
-
-        """
-        n_time = positions.shape[0]
-        n_position_bins = place_bin_centers.shape[0]
-
-        if block_size is None:
-            block_size = n_time
 
-        position_density = cp.empty((n_position_bins,))
-        for start_ind in range(0, n_position_bins, block_size):
-            block_inds = slice(start_ind, start_ind + block_size)
-            position_density[block_inds] = cp.mean(
-                estimate_position_distance(
-                    place_bin_centers[block_inds], positions, position_std
-                ),
-                axis=0,
-            )
-        return position_density
 
-    def estimate_log_intensity(density, occupancy, mean_rate):
-        """Calculates intensity in log space."""
-        return cp.log(mean_rate) + cp.log(density) - cp.log(occupancy)
-
-    def estimate_intensity(density, occupancy, mean_rate):
-        """Calculates intensity.
-
-        Parameters
-        ----------
-        density : np.ndarray, shape (n_bins,)
-        occupancy : np.ndarray, shape (n_bins,)
-        mean_rate : float
-
-        Returns
-        -------
-        intensity : np.ndarray, shape (n_bins,)
+def gaussian_pdf(x: np.ndarray, mean: np.ndarray, sigma: np.ndarray) -> np.ndarray:
+    """Compute the value of a Gaussian probability density function at x with
+    given mean and sigma."""
+    return np.exp(-0.5 * ((x - mean) / sigma) ** 2) / (sigma * np.sqrt(2.0 * np.pi))
+
+
+def estimate_position_distance(
+    place_bin_centers: np.ndarray, positions: np.ndarray, position_std: np.ndarray
+) -> np.ndarray:
+    """Estimates the Euclidean distance between positions and position bins.
+
+    Parameters
+    ----------
+    place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
+    positions : np.ndarray, shape (n_time, n_position_dims)
+    position_std : array_like, shape (n_position_dims,)
+
+    Returns
+    -------
+    position_distance : np.ndarray, shape (n_time, n_position_bins)
+
+    """
+    n_time, n_position_dims = positions.shape
+    n_position_bins = place_bin_centers.shape[0]
+
+    if isinstance(position_std, (int, float)):
+        position_std = [position_std] * n_position_dims
+
+    position_distance = np.ones((n_time, n_position_bins), dtype=np.float32)
+
+    for position_ind, std in enumerate(position_std):
+        position_distance *= gaussian_pdf(
+            np.expand_dims(place_bin_centers[:, position_ind], axis=0),
+            np.expand_dims(positions[:, position_ind], axis=1),
+            std,
+        )
 
-        """
-        return cp.exp(estimate_log_intensity(density, occupancy, mean_rate))
+    return position_distance
 
-    def estimate_log_joint_mark_intensity(
-        decoding_marks,
-        encoding_marks,
-        mark_std,
-        occupancy,
-        mean_rate,
-        place_bin_centers=None,
-        encoding_positions=None,
-        position_std=None,
-        max_mark_diff=6000,
-        set_diag_zero=False,
-        position_distance=None,
-    ):
-        """Finds the joint intensity of the marks and positions in log space.
 
-        Parameters
-        ----------
-        decoding_marks : np.ndarray, shape (n_decoding_spikes, n_features)
-        encoding_marks : np.ndarray, shape (n_encoding_spikes, n_features)
-        mark_std : float or np.ndarray, shape (n_features,)
-        occupancy : np.ndarray, shape (n_position_bins,)
-        mean_rate : float
-        place_bin_centers : None or np.ndarray, shape (n_position_bins, n_position_dims)
-            If None, position distance must be not None
-        encoding_positions : None or np.ndarray, shape (n_decoding_spikes, n_position_dims)
-            If None, position distance must be not None
-        position_std : None or float or array_like, shape (n_position_dims,)
-            If None, position distance must be not None
-        max_mark_diff : int
-            Maximum distance between integer marks.
-        set_diag_zero : bool
-        position_distance : np.ndarray, shape (n_encoding_spikes, n_position_bins)
-            Precalculated distance between position and position bins.
-
-        Returns
-        -------
-        log_joint_mark_intensity : np.ndarray, shape (n_decoding_spikes, n_position_bins)
-
-        """
-        n_encoding_spikes, n_marks = encoding_marks.shape
-
-        n_decoding_spikes = decoding_marks.shape[0]
-        mark_distance = cp.ones(
-            (n_decoding_spikes, n_encoding_spikes), dtype=cp.float32
-        )
-
-        for mark_ind in range(n_marks):
-            mark_distance *= gaussian_pdf(
-                cp.expand_dims(decoding_marks[:, mark_ind], axis=1),
-                cp.expand_dims(encoding_marks[:, mark_ind], axis=0),
-                mark_std[mark_ind],
-            )
+def estimate_position_density(
+    place_bin_centers: np.ndarray,
+    positions: np.ndarray,
+    position_std: Union[np.ndarray, float],
+    block_size: int = 100,
+) -> np.ndarray:
+    """Estimates a kernel density estimate over position bins using
+    Euclidean distances.
+
+    Parameters
+    ----------
+    place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
+    positions : np.ndarray, shape (n_time, n_position_dims)
+    position_std : float or array_like, shape (n_position_dims,)
+
+    Returns
+    -------
+    position_density : np.ndarray, shape (n_position_bins,)
+
+    """
+    n_time = positions.shape[0]
+    n_position_bins = place_bin_centers.shape[0]
+
+    if block_size is None:
+        block_size = n_time
+
+    position_density = np.empty((n_position_bins,))
+    for start_ind in range(0, n_position_bins, block_size):
+        block_inds = slice(start_ind, start_ind + block_size)
+        position_density[block_inds] = np.mean(
+            estimate_position_distance(
+                place_bin_centers[block_inds], positions, position_std
+            ),
+            axis=0,
+        )
+    return position_density
 
-        if set_diag_zero:
-            diag_ind = (cp.arange(n_decoding_spikes), cp.arange(n_decoding_spikes))
-            mark_distance[diag_ind] = 0.0
 
-        if position_distance is None:
-            position_distance = estimate_position_distance(
-                place_bin_centers, encoding_positions, position_std
-            ).astype(cp.float32)
+def estimate_log_intensity(
+    density: np.ndarray, occupancy: np.ndarray, mean_rate: float
+) -> np.ndarray:
+    """Calculates intensity in log space."""
+    return np.log(mean_rate) + np.log(density) - np.log(occupancy)
+
+
+def estimate_intensity(density, occupancy, mean_rate):
+    """Calculates intensity.
+
+    Parameters
+    ----------
+    density : np.ndarray, shape (n_bins,)
+    occupancy : np.ndarray, shape (n_bins,)
+    mean_rate : float
+
+    Returns
+    -------
+    intensity : np.ndarray, shape (n_bins,)
+
+    """
+    return np.exp(estimate_log_intensity(density, occupancy, mean_rate))
+
+
+def normal_pdf_integer_lookup(
+    x: int, mean: int, std: float = 20.0, max_value: int = 6000
+) -> int:
+    """Fast density evaluation for integers by precomputing a hash table of
+    values.
+
+    Parameters
+    ----------
+    x : int
+    mean : int
+    std : float
+    max_value : int
+
+    Returns
+    -------
+    probability_density : int
+
+    """
+    normal_density = gaussian_pdf(np.arange(-max_value, max_value), 0, std).astype(
+        np.float32
+    )
+
+    return normal_density[(x - mean) + max_value]
+
+
+def estimate_log_joint_mark_intensity(
+    decoding_marks: np.ndarray,
+    encoding_marks: np.ndarray,
+    mark_std: Union[np.ndarray, float],
+    occupancy: np.ndarray,
+    mean_rate: float,
+    place_bin_centers: Optional[np.ndarray] = None,
+    encoding_positions: Optional[np.ndarray] = None,
+    position_std: Optional[np.ndarray] = None,
+    max_mark_diff: int = 6000,
+    set_diag_zero: bool = False,
+    position_distance: Optional[np.ndarray] = None,
+) -> np.ndarray:
+    """Finds the joint intensity of the marks and positions in log space.
+
+    Parameters
+    ----------
+    decoding_marks : np.ndarray, shape (n_decoding_spikes, n_features)
+    encoding_marks : np.ndarray, shape (n_encoding_spikes, n_features)
+    mark_std : float or np.ndarray, shape (n_features,)
+    occupancy : np.ndarray, shape (n_position_bins,)
+    mean_rate : float
+    place_bin_centers : None or np.ndarray, shape (n_position_bins, n_position_dims)
+        If None, position distance must be not None
+    encoding_positions : None or np.ndarray, shape (n_decoding_spikes, n_position_dims)
+        If None, position distance must be not None
+    position_std : None or float or array_like, shape (n_position_dims,)
+        If None, position distance must be not None
+    max_mark_diff : int
+        Maximum distance between integer marks.
+    set_diag_zero : bool
+    position_distance : np.ndarray, shape (n_encoding_spikes, n_position_bins)
+        Precalculated distance between position and position bins.
+
+    Returns
+    -------
+    log_joint_mark_intensity : np.ndarray, shape (n_decoding_spikes, n_position_bins)
+
+    """
+    n_encoding_spikes, n_marks = encoding_marks.shape
+    n_decoding_spikes = decoding_marks.shape[0]
+    mark_distance = np.ones((n_decoding_spikes, n_encoding_spikes), dtype=np.float32)
+
+    for mark_ind in range(n_marks):
+        mark_distance *= normal_pdf_integer_lookup(
+            np.expand_dims(decoding_marks[:, mark_ind], axis=1),
+            np.expand_dims(encoding_marks[:, mark_ind], axis=0),
+            std=mark_std,
+            max_value=max_mark_diff,
+        )
 
-        return cp.asnumpy(
-            estimate_log_intensity(
-                mark_distance @ position_distance / n_encoding_spikes,
-                occupancy,
-                mean_rate,
-            )
+    if set_diag_zero:
+        diag_ind = (np.arange(n_decoding_spikes), np.arange(n_decoding_spikes))
+        mark_distance[diag_ind] = 0.0
+
+    if position_distance is None:
+        position_distance = estimate_position_distance(
+            place_bin_centers, encoding_positions, position_std
+        ).astype(np.float32)
+
+    return estimate_log_intensity(
+        mark_distance @ position_distance / n_encoding_spikes, occupancy, mean_rate
+    )
+
+
+def fit_multiunit_likelihood_integer(
+    position: np.ndarray,
+    multiunits: np.ndarray,
+    place_bin_centers: np.ndarray,
+    mark_std: np.ndarray,
+    position_std: Union[np.ndarray, float],
+    is_track_boundary: Optional[np.ndarray] = None,
+    is_track_interior: Optional[np.ndarray] = None,
+    edges: Optional[list[np.ndarray]] = None,
+    block_size: int = 100,
+    use_diffusion: bool = False,
+    **kwargs
+) -> dict:
+    """Fits the clusterless place field model.
+
+    Parameters
+    ----------
+    position : np.ndarray, shape (n_time, n_position_dims)
+    multiunits : np.ndarray, shape (n_time, n_marks, n_electrodes)
+    place_bin_centers : np.ndarray, shape (n_bins, n_position_dims)
+    mark_std : float
+        Amount of smoothing for the mark features.  Standard deviation of kernel.
+    position_std : float or array_like, shape (n_position_dims,)
+        Amount of smoothing for position.  Standard deviation of kernel.
+    is_track_boundary : None or np.ndarray, shape (n_bins,)
+    is_track_interior : None or np.ndarray, shape (n_bins,)
+    edges : None or list of np.ndarray
+    block_size : int
+        Size of data to process in chunks
+    use_diffusion : bool
+        Use diffusion to respect the track geometry.
+
+    Returns
+    -------
+    encoding_model : dict
+
+    """
+    if is_track_interior is None:
+        is_track_interior = np.ones((place_bin_centers.shape[0],), dtype=np.bool)
+
+    position = atleast_2d(position)
+    place_bin_centers = atleast_2d(place_bin_centers)
+    interior_place_bin_centers = np.asarray(
+        place_bin_centers[is_track_interior.ravel(order="F")], dtype=np.float32
+    )
+    gpu_is_track_interior = np.asarray(is_track_interior.ravel(order="F"))
+
+    not_nan_position = np.all(~np.isnan(position), axis=1)
+
+    if use_diffusion & (position.shape[1] > 1):
+        n_total_bins = np.prod(is_track_interior.shape)
+        bin_diffusion_distances = diffuse_each_bin(
+            is_track_interior,
+            is_track_boundary,
+            dx=edges[0][1] - edges[0][0],
+            dy=edges[1][1] - edges[1][0],
+            std=position_std,
+        ).reshape((n_total_bins, -1), order="F")
+    else:
+        bin_diffusion_distances = None
+
+    if use_diffusion & (position.shape[1] > 1):
+        occupancy = np.asarray(
+            estimate_diffusion_position_density(
+                position[not_nan_position],
+                edges,
+                bin_distances=bin_diffusion_distances,
+            ),
+            dtype=np.float32,
+        )
+    else:
+        occupancy = np.zeros((place_bin_centers.shape[0],), dtype=np.float32)
+        occupancy[gpu_is_track_interior] = estimate_position_density(
+            interior_place_bin_centers,
+            np.asarray(position[not_nan_position], dtype=np.float32),
+            position_std,
+            block_size=block_size,
         )
 
-    def fit_multiunit_likelihood_gpu(
-        position,
-        multiunits,
-        place_bin_centers,
-        mark_std,
-        position_std,
-        is_track_boundary=None,
-        is_track_interior=None,
-        edges=None,
-        block_size=100,
-        use_diffusion=False,
-        **kwargs
-    ):
-        """Fits the clusterless place field model.
+    mean_rates = []
+    summed_ground_process_intensity = np.zeros(
+        (place_bin_centers.shape[0],), dtype=np.float32
+    )
+    encoding_marks = []
+    encoding_positions = []
+
+    for multiunit in np.moveaxis(multiunits, -1, 0):
+
+        # ground process intensity
+        is_spike = np.any(~np.isnan(multiunit), axis=1)
+        mean_rates.append(is_spike.mean())
+
+        if is_spike.sum() > 0:
+            if use_diffusion & (position.shape[1] > 1):
+                marginal_density = np.asarray(
+                    estimate_diffusion_position_density(
+                        position[is_spike & not_nan_position],
+                        edges,
+                        bin_distances=bin_diffusion_distances,
+                    ),
+                    dtype=np.float32,
+                )
+            else:
+                marginal_density = np.zeros(
+                    (place_bin_centers.shape[0],), dtype=np.float32
+                )
+                marginal_density[gpu_is_track_interior] = estimate_position_density(
+                    interior_place_bin_centers,
+                    np.asarray(position[is_spike & not_nan_position], dtype=np.float32),
+                    position_std,
+                    block_size=block_size,
+                )
 
-        Parameters
-        ----------
-        position : np.ndarray, shape (n_time, n_position_dims)
-        multiunits : np.ndarray, shape (n_time, n_marks, n_electrodes)
-        place_bin_centers : np.ndarray, shape (n_bins, n_position_dims)
-        mark_std : float or array_like, shape (n_marks,)
-            Amount of smoothing for the mark features.  Standard deviation of kernel.
-        position_std : float or array_like, shape (n_position_dims,)
-            Amount of smoothing for position.  Standard deviation of kernel.
-        is_track_boundary : None or np.ndarray, shape (n_bins,)
-        is_track_interior : None or np.ndarray, shape (n_bins,)
-        edges : None or list of np.ndarray
-        block_size : int
-            Size of data to process in chunks
-        use_diffusion : bool
-            Use diffusion to respect the track geometry.
-
-        Returns
-        -------
-        encoding_model : dict
-
-        """
-        if is_track_interior is None:
-            is_track_interior = np.ones((place_bin_centers.shape[0],), dtype=np.bool)
-
-        position = atleast_2d(position)
-        place_bin_centers = atleast_2d(place_bin_centers)
-        interior_place_bin_centers = cp.asarray(
-            place_bin_centers[is_track_interior.ravel(order="F")], dtype=cp.float32
-        )
-        gpu_is_track_interior = cp.asarray(is_track_interior.ravel(order="F"))
-
-        not_nan_position = np.all(~np.isnan(position), axis=1)
-
-        if use_diffusion & (position.shape[1] > 1):
-            n_total_bins = np.prod(is_track_interior.shape)
-            bin_diffusion_distances = diffuse_each_bin(
-                is_track_interior,
-                is_track_boundary,
-                dx=edges[0][1] - edges[0][0],
-                dy=edges[1][1] - edges[1][0],
-                std=position_std,
-            ).reshape((n_total_bins, -1), order="F")
-        else:
-            bin_diffusion_distances = None
+        summed_ground_process_intensity += estimate_intensity(
+            marginal_density, occupancy, mean_rates[-1]
+        )
 
-        if use_diffusion & (position.shape[1] > 1):
-            occupancy = cp.asarray(
-                estimate_diffusion_position_density(
-                    position[not_nan_position],
-                    edges,
-                    bin_distances=bin_diffusion_distances,
-                ),
-                dtype=cp.float32,
+        is_mark_features = np.any(~np.isnan(multiunit), axis=0)
+        encoding_marks.append(
+            np.asarray(
+                multiunit[np.ix_(is_spike & not_nan_position, is_mark_features)],
+                dtype=np.int16,
             )
-        else:
-            occupancy = cp.zeros((place_bin_centers.shape[0],), dtype=cp.float32)
-            occupancy[gpu_is_track_interior] = estimate_position_density(
-                interior_place_bin_centers,
-                cp.asarray(position[not_nan_position], dtype=cp.float32),
-                position_std,
-                block_size=block_size,
-            )
-
-        mean_rates = []
-        summed_ground_process_intensity = cp.zeros(
-            (place_bin_centers.shape[0],), dtype=cp.float32
-        )
-        encoding_marks = []
-        encoding_positions = []
-
-        n_marks = multiunits.shape[1]
-        if isinstance(mark_std, (int, float)):
-            mark_std = np.asarray([mark_std] * n_marks)
-        else:
-            mark_std = np.asarray(mark_std)
-
-        for multiunit in np.moveaxis(multiunits, -1, 0):
+        )
+        encoding_positions.append(position[is_spike & not_nan_position])
 
-            # ground process intensity
-            is_spike = np.any(~np.isnan(multiunit), axis=1)
-            mean_rates.append(is_spike.mean())
-
-            if is_spike.sum() > 0:
-                if use_diffusion & (position.shape[1] > 1):
-                    marginal_density = cp.asarray(
-                        estimate_diffusion_position_density(
-                            position[is_spike & not_nan_position],
-                            edges,
-                            bin_distances=bin_diffusion_distances,
-                        ),
-                        dtype=cp.float32,
-                    )
-                else:
-                    marginal_density = cp.zeros(
-                        (place_bin_centers.shape[0],), dtype=cp.float32
-                    )
-                    marginal_density[gpu_is_track_interior] = estimate_position_density(
-                        interior_place_bin_centers,
-                        cp.asarray(
-                            position[is_spike & not_nan_position], dtype=cp.float32
-                        ),
-                        position_std,
-                        block_size=block_size,
-                    )
+    summed_ground_process_intensity = summed_ground_process_intensity + np.spacing(1)
 
-            summed_ground_process_intensity += estimate_intensity(
-                marginal_density, occupancy, mean_rates[-1]
-            )
-
-            is_mark_features = np.any(~np.isnan(multiunit), axis=0)
-            encoding_marks.append(
-                cp.asarray(
-                    multiunit[np.ix_(is_spike & not_nan_position, is_mark_features)],
-                    dtype=cp.float32,
-                )
-            )
-            encoding_positions.append(position[is_spike & not_nan_position])
+    return {
+        "encoding_marks": encoding_marks,
+        "encoding_positions": encoding_positions,
+        "summed_ground_process_intensity": summed_ground_process_intensity,
+        "occupancy": occupancy,
+        "mean_rates": mean_rates,
+        "mark_std": mark_std,
+        "position_std": position_std,
+        "block_size": block_size,
+        "bin_diffusion_distances": bin_diffusion_distances,
+        "use_diffusion": use_diffusion,
+        "edges": edges,
+        **kwargs,
+    }
+
+
+def estimate_multiunit_likelihood_integer(
+    multiunits: np.ndarray,
+    encoding_marks: np.ndarray,
+    mark_std: np.ndarray,
+    place_bin_centers: np.ndarray,
+    encoding_positions: np.ndarray,
+    position_std: np.ndarray,
+    occupancy: np.ndarray,
+    mean_rates: np.ndarray,
+    summed_ground_process_intensity: np.ndarray,
+    bin_diffusion_distances: np.ndarray,
+    edges: list[np.ndarray],
+    max_mark_diff: int = 6000,
+    set_diag_zero: bool = False,
+    is_track_interior: Optional[np.ndarray] = None,
+    time_bin_size: int = 1,
+    block_size: int = 100,
+    ignore_no_spike: bool = False,
+    disable_progress_bar: bool = False,
+    use_diffusion: bool = False,
+) -> np.ndarray:
+    """Estimates the likelihood of position bins given multiunit marks.
+
+    Parameters
+    ----------
+    multiunits : np.ndarray, shape (n_decoding_time, n_marks, n_electrodes)
+    encoding_marks : np.ndarray, shape (n_encoding_spikes, n_marks, n_electrodes)
+    mark_std : float
+        Amount of smoothing for mark features.  Standard deviation of kernel.
+    place_bin_centers : np.ndarray, shape (n_bins, n_position_dims)
+    encoding_positions : np.ndarray, shape (n_encoding_spikes, n_position_dims)
+    position_std : float or array_like, shape (n_position_dims,)
+        Amount of smoothing for position.  Standard deviation of kernel.
+    occupancy : np.ndarray, (n_bins,)
+    mean_rates : list, len (n_electrodes,)
+    summed_ground_process_intensity : np.ndarray, shape (n_bins,)
+    bin_diffusion_distances : np.ndarray, shape (n_bins, n_bins)
+    edges : list of np.ndarray
+    max_mark_diff : int
+        Maximum difference between mark features
+    set_diag_zero : bool
+        Remove influence of the same mark in encoding and decoding.
+    is_track_interior : None or np.ndarray, shape (n_bins_x, n_bins_y)
+    time_bin_size : float
+        Size of time steps
+    block_size : int
+        Size of data to process in chunks
+    ignore_no_spike : bool
+        Set contribution of no spikes to zero
+    disable_progress_bar : bool
+        If False, a progress bar will be displayed.
+    use_diffusion : bool
+        Respect track geometry by using diffusion distances
+
+    Returns
+    -------
+    log_likelihood : np.ndarray, shape (n_time, n_bins)
+
+    """
+
+    if is_track_interior is None:
+        is_track_interior = np.ones((place_bin_centers.shape[0],), dtype=np.bool)
+    else:
+        is_track_interior = is_track_interior.ravel(order="F")
+
+    n_time = multiunits.shape[0]
+    if ignore_no_spike:
+        log_likelihood = (
+            -time_bin_size
+            * summed_ground_process_intensity
+            * np.zeros((n_time, 1), dtype=np.float32)
+        )
+    else:
+        log_likelihood = (
+            -time_bin_size
+            * summed_ground_process_intensity
+            * np.ones((n_time, 1), dtype=np.float32)
+        )
 
-        summed_ground_process_intensity = cp.asnumpy(
-            summed_ground_process_intensity
-        ) + np.spacing(1)
-
-        return {
-            "encoding_marks": encoding_marks,
-            "encoding_positions": encoding_positions,
-            "summed_ground_process_intensity": summed_ground_process_intensity,
-            "occupancy": occupancy,
-            "mean_rates": mean_rates,
-            "mark_std": mark_std,
-            "position_std": position_std,
-            "block_size": block_size,
-            "bin_diffusion_distances": bin_diffusion_distances,
-            "use_diffusion": use_diffusion,
-            "edges": edges,
-            **kwargs,
-        }
+    multiunits = np.moveaxis(multiunits, -1, 0)
+    n_position_bins = is_track_interior.sum()
+    interior_place_bin_centers = np.asarray(
+        place_bin_centers[is_track_interior], dtype=np.float32
+    )
+    gpu_is_track_interior = np.asarray(is_track_interior)
+    interior_occupancy = occupancy[gpu_is_track_interior]
 
-    def estimate_multiunit_likelihood_gpu(
-        multiunits,
+    for multiunit, enc_marks, enc_pos, mean_rate in zip(
+        tqdm(multiunits, desc="n_electrodes", disable=disable_progress_bar),
         encoding_marks,
-        mark_std,
-        place_bin_centers,
         encoding_positions,
-        position_std,
-        occupancy,
         mean_rates,
-        summed_ground_process_intensity,
-        bin_diffusion_distances,
-        edges,
-        max_mark_diff=6000,
-        set_diag_zero=False,
-        is_track_interior=None,
-        time_bin_size=1,
-        block_size=100,
-        ignore_no_spike=False,
-        disable_progress_bar=False,
-        use_diffusion=False,
     ):
-        """Estimates the likelihood of position bins given multiunit marks.
-
-        Parameters
-        ----------
-        multiunits : np.ndarray, shape (n_decoding_time, n_marks, n_electrodes)
-        encoding_marks : cp.ndarray, shape (n_encoding_spikes, n_marks, n_electrodes)
-        mark_std : list, shape (n_marks,)
-            Amount of smoothing for mark features
-        place_bin_centers : cp.ndarray, shape (n_bins, n_position_dims)
-        encoding_positions : cp.ndarray, shape (n_encoding_spikes, n_position_dims)
-        position_std : float or array_like, shape (n_position_dims,)
-            Amount of smoothing for position
-        occupancy : cp.ndarray, (n_bins,)
-        mean_rates : list, len (n_electrodes,)
-        summed_ground_process_intensity : np.ndarray, shape (n_bins,)
-        bin_diffusion_distances : np.ndarray, shape (n_bins, n_bins)
-        edges : list of np.ndarray
-        max_mark_diff : int
-            Maximum difference between mark features
-        set_diag_zero : bool
-            Remove influence of the same mark in encoding and decoding.
-        is_track_interior : None or np.ndarray, shape (n_bins_x, n_bins_y)
-        time_bin_size : float
-            Size of time steps
-        block_size : int
-            Size of data to process in chunks
-        ignore_no_spike : bool
-            Set contribution of no spikes to zero
-        disable_progress_bar : bool
-            If False, a progress bar will be displayed.
-        use_diffusion : bool
-            Respect track geometry by using diffusion distances
-
-        Returns
-        -------
-        log_likelihood : (n_time, n_bins)
-
-        """
+        is_spike = np.any(~np.isnan(multiunit), axis=1)
+        is_mark_features = np.any(~np.isnan(multiunit), axis=0)
+        decoding_marks = np.asarray(
+            multiunit[np.ix_(is_spike, is_mark_features)], dtype=np.int16
+        )
+        n_decoding_marks = decoding_marks.shape[0]
+        log_joint_mark_intensity = np.zeros(
+            (n_decoding_marks, n_position_bins), dtype=np.float32
+        )
 
-        if is_track_interior is None:
-            is_track_interior = np.ones((place_bin_centers.shape[0],), dtype=np.bool)
-        else:
-            is_track_interior = is_track_interior.ravel(order="F")
+        if block_size is None:
+            block_size = n_decoding_marks
 
-        n_time = multiunits.shape[0]
-        if ignore_no_spike:
-            log_likelihood = (
-                -time_bin_size
-                * summed_ground_process_intensity
-                * np.zeros((n_time, 1), dtype=np.float32)
+        if use_diffusion & (place_bin_centers.shape[1] > 1):
+            position_distance = np.asarray(
+                estimate_diffusion_position_distance(
+                    enc_pos,
+                    edges,
+                    bin_distances=bin_diffusion_distances,
+                )[:, is_track_interior],
+                dtype=np.float32,
             )
         else:
-            log_likelihood = (
-                -time_bin_size
-                * summed_ground_process_intensity
-                * np.ones((n_time, 1), dtype=np.float32)
-            )
-
-        multiunits = np.moveaxis(multiunits, -1, 0)
-        n_position_bins = is_track_interior.sum()
-        interior_place_bin_centers = cp.asarray(
-            place_bin_centers[is_track_interior], dtype=cp.float32
-        )
-        gpu_is_track_interior = cp.asarray(is_track_interior)
-        interior_occupancy = occupancy[gpu_is_track_interior]
-
-        for multiunit, enc_marks, enc_pos, mean_rate in zip(
-            tqdm(multiunits, desc="n_electrodes", disable=disable_progress_bar),
-            encoding_marks,
-            encoding_positions,
-            mean_rates,
-        ):
-            is_spike = np.any(~np.isnan(multiunit), axis=1)
-            is_mark_features = np.any(~np.isnan(multiunit), axis=0)
-            decoding_marks = cp.asarray(
-                multiunit[np.ix_(is_spike, is_mark_features)], dtype=cp.float32
-            )
-            n_decoding_marks = decoding_marks.shape[0]
-            log_joint_mark_intensity = np.zeros(
-                (n_decoding_marks, n_position_bins), dtype=np.float32
-            )
-
-            if block_size is None:
-                block_size = n_decoding_marks
-
-            if use_diffusion & (place_bin_centers.shape[1] > 1):
-                position_distance = cp.asarray(
-                    estimate_diffusion_position_distance(
-                        enc_pos,
-                        edges,
-                        bin_distances=bin_diffusion_distances,
-                    )[:, is_track_interior],
-                    dtype=cp.float32,
-                )
-            else:
-                position_distance = estimate_position_distance(
-                    interior_place_bin_centers,
-                    cp.asarray(enc_pos, dtype=cp.float32),
-                    position_std,
-                ).astype(cp.float32)
+            position_distance = estimate_position_distance(
+                interior_place_bin_centers,
+                np.asarray(enc_pos, dtype=np.float32),
+                position_std,
+            ).astype(np.float32)
 
-            for start_ind in range(0, n_decoding_marks, block_size):
-                block_inds = slice(start_ind, start_ind + block_size)
-                log_joint_mark_intensity[
-                    block_inds
-                ] = estimate_log_joint_mark_intensity(
-                    decoding_marks[block_inds],
-                    enc_marks,
-                    mark_std[is_mark_features],
-                    interior_occupancy,
-                    mean_rate,
-                    max_mark_diff=max_mark_diff,
-                    set_diag_zero=set_diag_zero,
-                    position_distance=position_distance,
-                )
-            log_likelihood[np.ix_(is_spike, is_track_interior)] += np.nan_to_num(
-                log_joint_mark_intensity
+        for start_ind in range(0, n_decoding_marks, block_size):
+            block_inds = slice(start_ind, start_ind + block_size)
+            log_joint_mark_intensity[block_inds] = estimate_log_joint_mark_intensity(
+                decoding_marks[block_inds],
+                enc_marks,
+                mark_std,
+                interior_occupancy,
+                mean_rate,
+                max_mark_diff=max_mark_diff,
+                set_diag_zero=set_diag_zero,
+                position_distance=position_distance,
             )
+        log_likelihood[np.ix_(is_spike, is_track_interior)] += np.nan_to_num(
+            log_joint_mark_intensity
+        )
 
-            mempool = cp.get_default_memory_pool()
-            mempool.free_all_blocks()
-
-        log_likelihood[:, ~is_track_interior] = np.nan
-
-        return log_likelihood
-
-except ImportError:
-
-    def estimate_multiunit_likelihood_gpu(*args, **kwargs):
-        print("Cupy is not installed or no GPU detected...")
+    log_likelihood[:, ~is_track_interior] = np.nan
 
-    def fit_multiunit_likelihood_gpu(*args, **kwargs):
-        print("Cupy is not installed or no GPU detected...")
+    return log_likelihood
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer_gpu_log.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,485 +1,541 @@
 """Estimates a marked point process likelihood where the marks are
- features of the spike waveform. Mark features are int16.
+ features of the spike waveform using GPUs. Mark features are int16.
+
+ This algorithm is more numerically stable KDE done in log space but slower
+ right now because of lack of matrix multiplication.
 
  Marks are converted to integers and KDE uses hash tables to compute Gaussian
  kernels."""
 
 
+import math
+
 import numpy as np
+from numba import cuda
 from replay_trajectory_classification.core import atleast_2d
 from replay_trajectory_classification.likelihoods.diffusion import (
     diffuse_each_bin,
     estimate_diffusion_position_density,
     estimate_diffusion_position_distance,
 )
 from tqdm.autonotebook import tqdm
 
+try:
+    import cupy as cp
 
-def gaussian_pdf(x, mean, sigma):
-    """Compute the value of a Gaussian probability density function at x with
-    given mean and sigma."""
-    return np.exp(-0.5 * ((x - mean) / sigma) ** 2) / (sigma * np.sqrt(2.0 * np.pi))
-
-
-def estimate_position_distance(place_bin_centers, positions, position_std):
-    """Estimates the Euclidean distance between positions and position bins.
-
-    Parameters
-    ----------
-    place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
-    positions : np.ndarray, shape (n_time, n_position_dims)
-    position_std : array_like, shape (n_position_dims,)
-
-    Returns
-    -------
-    position_distance : np.ndarray, shape (n_time, n_position_bins)
-
-    """
-    n_time, n_position_dims = positions.shape
-    n_position_bins = place_bin_centers.shape[0]
-
-    if isinstance(position_std, (int, float)):
-        position_std = [position_std] * n_position_dims
-
-    position_distance = np.ones((n_time, n_position_bins), dtype=np.float32)
-
-    for position_ind, std in enumerate(position_std):
-        position_distance *= gaussian_pdf(
-            np.expand_dims(place_bin_centers[:, position_ind], axis=0),
-            np.expand_dims(positions[:, position_ind], axis=1),
-            std,
-        )
+    def logsumexp(a, axis):
+        a_max = cp.amax(a, axis=axis, keepdims=True)
 
-    return position_distance
+        if a_max.ndim > 0:
+            a_max[~cp.isfinite(a_max)] = 0
+        elif not np.isfinite(a_max):
+            a_max = 0
 
+        return cp.log(cp.sum(cp.exp(a - a_max), axis=axis, keepdims=True)) + a_max
 
-def estimate_position_density(
-    place_bin_centers, positions, position_std, block_size=100
-):
-    """Estimates a kernel density estimate over position bins using
-    Euclidean distances.
-
-    Parameters
-    ----------
-    place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
-    positions : np.ndarray, shape (n_time, n_position_dims)
-    position_std : float or array_like, shape (n_position_dims,)
-
-    Returns
-    -------
-    position_density : np.ndarray, shape (n_position_bins,)
-
-    """
-    n_time = positions.shape[0]
-    n_position_bins = place_bin_centers.shape[0]
-
-    if block_size is None:
-        block_size = n_time
-
-    position_density = np.empty((n_position_bins,))
-    for start_ind in range(0, n_position_bins, block_size):
-        block_inds = slice(start_ind, start_ind + block_size)
-        position_density[block_inds] = np.mean(
-            estimate_position_distance(
-                place_bin_centers[block_inds], positions, position_std
-            ),
-            axis=0,
-        )
-    return position_density
+    def log_mean(x, axis):
+        return cp.squeeze(logsumexp(x, axis=axis) - cp.log(x.shape[axis]))
 
+    @cp.fuse()
+    def log_gaussian_pdf(x, sigma):
+        return -cp.log(sigma) - 0.5 * cp.log(2 * cp.pi) - 0.5 * (x / sigma) ** 2
 
-def estimate_log_intensity(density, occupancy, mean_rate):
-    """Calculates intensity in log space."""
-    return np.log(mean_rate) + np.log(density) - np.log(occupancy)
-
-
-def estimate_intensity(density, occupancy, mean_rate):
-    """Calculates intensity.
-
-    Parameters
-    ----------
-    density : np.ndarray, shape (n_bins,)
-    occupancy : np.ndarray, shape (n_bins,)
-    mean_rate : float
-
-    Returns
-    -------
-    intensity : np.ndarray, shape (n_bins,)
-
-    """
-    return np.exp(estimate_log_intensity(density, occupancy, mean_rate))
-
-
-def normal_pdf_integer_lookup(x, mean, std=20, max_value=6000):
-    """Fast density evaluation for integers by precomputing a hash table of
-    values.
-
-    Parameters
-    ----------
-    x : int
-    mean : int
-    std : float
-    max_value : int
-
-    Returns
-    -------
-    probability_density : int
-
-    """
-    normal_density = gaussian_pdf(np.arange(-max_value, max_value), 0, std).astype(
-        np.float32
-    )
-
-    return normal_density[(x - mean) + max_value]
-
-
-def estimate_log_joint_mark_intensity(
-    decoding_marks,
-    encoding_marks,
-    mark_std,
-    occupancy,
-    mean_rate,
-    place_bin_centers=None,
-    encoding_positions=None,
-    position_std=None,
-    max_mark_diff=6000,
-    set_diag_zero=False,
-    position_distance=None,
-):
-    """Finds the joint intensity of the marks and positions in log space.
-
-    Parameters
-    ----------
-    decoding_marks : np.ndarray, shape (n_decoding_spikes, n_features)
-    encoding_marks : np.ndarray, shape (n_encoding_spikes, n_features)
-    mark_std : float or np.ndarray, shape (n_features,)
-    occupancy : np.ndarray, shape (n_position_bins,)
-    mean_rate : float
-    place_bin_centers : None or np.ndarray, shape (n_position_bins, n_position_dims)
-        If None, position distance must be not None
-    encoding_positions : None or np.ndarray, shape (n_decoding_spikes, n_position_dims)
-        If None, position distance must be not None
-    position_std : None or float or array_like, shape (n_position_dims,)
-        If None, position distance must be not None
-    max_mark_diff : int
-        Maximum distance between integer marks.
-    set_diag_zero : bool
-    position_distance : np.ndarray, shape (n_encoding_spikes, n_position_bins)
-        Precalculated distance between position and position bins.
-
-    Returns
-    -------
-    log_joint_mark_intensity : np.ndarray, shape (n_decoding_spikes, n_position_bins)
-
-    """
-    n_encoding_spikes, n_marks = encoding_marks.shape
-    n_decoding_spikes = decoding_marks.shape[0]
-    mark_distance = np.ones((n_decoding_spikes, n_encoding_spikes), dtype=np.float32)
-
-    for mark_ind in range(n_marks):
-        mark_distance *= normal_pdf_integer_lookup(
-            np.expand_dims(decoding_marks[:, mark_ind], axis=1),
-            np.expand_dims(encoding_marks[:, mark_ind], axis=0),
-            std=mark_std,
-            max_value=max_mark_diff,
-        )
+    @cp.fuse()
+    def estimate_log_intensity(log_density, log_occupancy, log_mean_rate):
+        return log_mean_rate + log_density - log_occupancy
 
-    if set_diag_zero:
-        diag_ind = (np.arange(n_decoding_spikes), np.arange(n_decoding_spikes))
-        mark_distance[diag_ind] = 0.0
-
-    if position_distance is None:
-        position_distance = estimate_position_distance(
-            place_bin_centers, encoding_positions, position_std
-        ).astype(np.float32)
-
-    return estimate_log_intensity(
-        mark_distance @ position_distance / n_encoding_spikes, occupancy, mean_rate
-    )
-
-
-def fit_multiunit_likelihood_integer(
-    position,
-    multiunits,
-    place_bin_centers,
-    mark_std,
-    position_std,
-    is_track_boundary=None,
-    is_track_interior=None,
-    edges=None,
-    block_size=100,
-    use_diffusion=False,
-    **kwargs
-):
-    """Fits the clusterless place field model.
-
-    Parameters
-    ----------
-    position : np.ndarray, shape (n_time, n_position_dims)
-    multiunits : np.ndarray, shape (n_time, n_marks, n_electrodes)
-    place_bin_centers : np.ndarray, shape (n_bins, n_position_dims)
-    mark_std : float
-        Amount of smoothing for the mark features.  Standard deviation of kernel.
-    position_std : float or array_like, shape (n_position_dims,)
-        Amount of smoothing for position.  Standard deviation of kernel.
-    is_track_boundary : None or np.ndarray, shape (n_bins,)
-    is_track_interior : None or np.ndarray, shape (n_bins,)
-    edges : None or list of np.ndarray
-    block_size : int
-        Size of data to process in chunks
-    use_diffusion : bool
-        Use diffusion to respect the track geometry.
-
-    Returns
-    -------
-    encoding_model : dict
-
-    """
-    if is_track_interior is None:
-        is_track_interior = np.ones((place_bin_centers.shape[0],), dtype=np.bool)
-
-    position = atleast_2d(position)
-    place_bin_centers = atleast_2d(place_bin_centers)
-    interior_place_bin_centers = np.asarray(
-        place_bin_centers[is_track_interior.ravel(order="F")], dtype=np.float32
-    )
-    gpu_is_track_interior = np.asarray(is_track_interior.ravel(order="F"))
-
-    not_nan_position = np.all(~np.isnan(position), axis=1)
-
-    if use_diffusion & (position.shape[1] > 1):
-        n_total_bins = np.prod(is_track_interior.shape)
-        bin_diffusion_distances = diffuse_each_bin(
-            is_track_interior,
-            is_track_boundary,
-            dx=edges[0][1] - edges[0][0],
-            dy=edges[1][1] - edges[1][0],
-            std=position_std,
-        ).reshape((n_total_bins, -1), order="F")
-    else:
-        bin_diffusion_distances = None
-
-    if use_diffusion & (position.shape[1] > 1):
-        occupancy = np.asarray(
-            estimate_diffusion_position_density(
-                position[not_nan_position],
-                edges,
-                bin_distances=bin_diffusion_distances,
-            ),
-            dtype=np.float32,
-        )
-    else:
-        occupancy = np.zeros((place_bin_centers.shape[0],), dtype=np.float32)
-        occupancy[gpu_is_track_interior] = estimate_position_density(
-            interior_place_bin_centers,
-            np.asarray(position[not_nan_position], dtype=np.float32),
-            position_std,
-            block_size=block_size,
-        )
+    @cp.fuse()
+    def estimate_intensity(log_density, log_occupancy, log_mean_rate):
+        return cp.exp(estimate_log_intensity(log_density, log_occupancy, log_mean_rate))
+
+    def estimate_log_position_distance(place_bin_centers, positions, position_std):
+        """Estimates the Euclidean distance between positions and position bins.
+
+        Parameters
+        ----------
+        place_bin_centers : cp.ndarray, shape (n_position_bins, n_position_dims)
+        positions : cp.ndarray, shape (n_time, n_position_dims)
+        position_std : array_like, shape (n_position_dims,)
+
+        Returns
+        -------
+        log_position_distance : np.ndarray, shape (n_time, n_position_bins)
+
+        """
+        n_time, n_position_dims = positions.shape
+        n_position_bins = place_bin_centers.shape[0]
+
+        if isinstance(position_std, (int, float)):
+            position_std = [position_std] * n_position_dims
+
+        log_position_distance = cp.zeros((n_time, n_position_bins), dtype=cp.float32)
+
+        for position_ind, std in enumerate(position_std):
+            log_position_distance += log_gaussian_pdf(
+                cp.expand_dims(place_bin_centers[:, position_ind], axis=0)
+                - cp.expand_dims(positions[:, position_ind], axis=1),
+                std,
+            )
+
+        return log_position_distance
+
+    def estimate_log_position_density(
+        place_bin_centers, positions, position_std, block_size=100
+    ):
+        """Estimates a kernel density estimate over position bins using
+        Euclidean distances.
+
+        Parameters
+        ----------
+        place_bin_centers : cp.ndarray, shape (n_position_bins, n_position_dims)
+        positions : cp.ndarray, shape (n_time, n_position_dims)
+        position_std : float or array_like, shape (n_position_dims,)
+        block_size : int
+
+        Returns
+        -------
+        log_position_density : cp.ndarray, shape (n_position_bins,)
+
+        """
+        n_time = positions.shape[0]
+        n_position_bins = place_bin_centers.shape[0]
+
+        if block_size is None:
+            block_size = n_time
+
+        log_position_density = cp.empty((n_position_bins,))
+        for start_ind in range(0, n_position_bins, block_size):
+            block_inds = slice(start_ind, start_ind + block_size)
+            log_position_density[block_inds] = log_mean(
+                estimate_log_position_distance(
+                    place_bin_centers[block_inds], positions, position_std
+                ),
+                axis=0,
+            )
+
+        return log_position_density
+
+    @cuda.jit()
+    def log_mean_over_bins(log_mark_distances, log_position_distances, output):
+        """
+
+        Parameters
+        ----------
+        log_mark_distances : cp.ndarray, shape (n_decoding_spikes, n_encoding_spikes)
+        log_position_distances : cp.ndarray, shape (n_encoding_spikes, n_position_bins)
+
+        Returns
+        -------
+        output : cp.ndarray, shape (n_decoding_spikes, n_position_bins)
+
+        """
+        thread_id = cuda.grid(1)
 
-    mean_rates = []
-    summed_ground_process_intensity = np.zeros(
-        (place_bin_centers.shape[0],), dtype=np.float32
-    )
-    encoding_marks = []
-    encoding_positions = []
-
-    for multiunit in np.moveaxis(multiunits, -1, 0):
-
-        # ground process intensity
-        is_spike = np.any(~np.isnan(multiunit), axis=1)
-        mean_rates.append(is_spike.mean())
-
-        if is_spike.sum() > 0:
-            if use_diffusion & (position.shape[1] > 1):
-                marginal_density = np.asarray(
+        n_decoding_spikes, n_position_bins = output.shape
+        n_encoding_spikes = log_position_distances.shape[0]
+
+        decoding_ind = thread_id // n_position_bins
+        pos_bin_ind = thread_id % n_position_bins
+
+        if (decoding_ind < n_decoding_spikes) and (pos_bin_ind < n_position_bins):
+
+            # find maximum
+            max_exp = (
+                log_mark_distances[decoding_ind, 0]
+                + log_position_distances[0, pos_bin_ind]
+            )
+
+            for encoding_ind in range(1, n_encoding_spikes):
+                candidate_max = (
+                    log_mark_distances[decoding_ind, encoding_ind]
+                    + log_position_distances[encoding_ind, pos_bin_ind]
+                )
+                if candidate_max > max_exp:
+                    max_exp = candidate_max
+
+            # logsumexp
+            tmp = 0.0
+            for encoding_ind in range(n_encoding_spikes):
+                tmp += math.exp(
+                    log_mark_distances[decoding_ind, encoding_ind]
+                    + log_position_distances[encoding_ind, pos_bin_ind]
+                    - max_exp
+                )
+
+            output[decoding_ind, pos_bin_ind] = math.log(tmp) + max_exp
+
+            # divide by n_spikes to get the mean
+            output[decoding_ind, pos_bin_ind] -= math.log(n_encoding_spikes)
+
+    def estimate_log_joint_mark_intensity(
+        decoding_marks,
+        encoding_marks,
+        mark_std,
+        log_position_distances,
+        log_occupancy,
+        log_mean_rate,
+        max_mark_diff=6000,
+        set_diag_zero=False,
+    ):
+        """Finds the joint intensity of the marks and positions in log space.
+
+        Parameters
+        ----------
+        decoding_marks : cp.ndarray, shape (n_decoding_spikes, n_features)
+        encoding_marks : cp.ndarray, shape (n_encoding_spikes, n_features)
+        mark_std : float
+        log_position_distance : cp.ndarray, shape (n_encoding_spikes, n_position_bins)
+            Precalculated distance between position and position bins.
+        log_occupancy : cp.ndarray, shape (n_position_bins,)
+        log_mean_rate : float
+        max_mark_diff : int
+            Maximum distance between integer marks.
+        set_diag_zero : bool
+
+        Returns
+        -------
+        log_joint_mark_intensity : np.ndarray, shape (n_decoding_spikes, n_position_bins)
+
+        """
+        n_encoding_spikes, n_marks = encoding_marks.shape
+        n_decoding_spikes = decoding_marks.shape[0]
+        log_mark_distances = cp.zeros(
+            (n_decoding_spikes, n_encoding_spikes), dtype=cp.float32
+        )
+
+        log_normal_pdf_lookup = cp.asarray(
+            log_gaussian_pdf(cp.arange(-max_mark_diff, max_mark_diff), mark_std),
+            dtype=cp.float32,
+        )
+
+        for mark_ind in range(n_marks):
+            log_mark_distances += log_normal_pdf_lookup[
+                (
+                    cp.expand_dims(decoding_marks[:, mark_ind], axis=1)
+                    - cp.expand_dims(encoding_marks[:, mark_ind], axis=0)
+                )
+                + max_mark_diff
+            ]
+
+        if set_diag_zero:
+            diag_ind = (cp.arange(n_decoding_spikes), cp.arange(n_decoding_spikes))
+            log_mark_distances[diag_ind] = cp.nan_to_num(cp.log(0).astype(cp.float32))
+
+        n_position_bins = log_position_distances.shape[1]
+        pdf = cp.empty((n_decoding_spikes, n_position_bins), dtype=cp.float32)
+
+        log_mean_over_bins.forall(pdf.size)(
+            log_mark_distances, log_position_distances, pdf
+        )
+
+        return cp.asnumpy(estimate_log_intensity(pdf, log_occupancy, log_mean_rate))
+
+    def fit_multiunit_likelihood_integer_gpu_log(
+        position,
+        multiunits,
+        place_bin_centers,
+        mark_std,
+        position_std,
+        is_track_boundary=None,
+        is_track_interior=None,
+        edges=None,
+        block_size=100,
+        use_diffusion=False,
+        **kwargs
+    ):
+        """Fits the clusterless place field model.
+
+        Parameters
+        ----------
+        position : np.ndarray, shape (n_time, n_position_dims)
+        multiunits : np.ndarray, shape (n_time, n_marks, n_electrodes)
+        place_bin_centers : np.ndarray, shape (n_bins, n_position_dims)
+        mark_std : float
+            Amount of smoothing for the mark features.  Standard deviation of kernel.
+        position_std : float or array_like, shape (n_position_dims,)
+            Amount of smoothing for position.  Standard deviation of kernel.
+        is_track_boundary : None or np.ndarray, shape (n_bins,)
+        is_track_interior : None or np.ndarray, shape (n_bins,)
+        edges : None or list of np.ndarray
+        block_size : int
+            Size of data to process in chunks
+        use_diffusion : bool
+            Use diffusion to respect the track geometry.
+
+        Returns
+        -------
+        encoding_model : dict
+
+        """
+        if is_track_interior is None:
+            is_track_interior = np.ones((place_bin_centers.shape[0],), dtype=np.bool)
+
+        position = atleast_2d(position)
+        place_bin_centers = atleast_2d(place_bin_centers)
+        interior_place_bin_centers = cp.asarray(
+            place_bin_centers[is_track_interior.ravel(order="F")], dtype=cp.float32
+        )
+        gpu_is_track_interior = cp.asarray(is_track_interior.ravel(order="F"))
+
+        not_nan_position = np.all(~np.isnan(position), axis=1)
+
+        if use_diffusion & (position.shape[1] > 1):
+            n_total_bins = np.prod(is_track_interior.shape)
+            bin_diffusion_distances = diffuse_each_bin(
+                is_track_interior,
+                is_track_boundary,
+                dx=edges[0][1] - edges[0][0],
+                dy=edges[1][1] - edges[1][0],
+                std=position_std,
+            ).reshape((n_total_bins, -1), order="F")
+        else:
+            bin_diffusion_distances = None
+
+        if use_diffusion & (position.shape[1] > 1):
+            log_occupancy = cp.log(
+                cp.asarray(
                     estimate_diffusion_position_density(
-                        position[is_spike & not_nan_position],
+                        position[not_nan_position],
                         edges,
                         bin_distances=bin_diffusion_distances,
                     ),
-                    dtype=np.float32,
-                )
-            else:
-                marginal_density = np.zeros(
-                    (place_bin_centers.shape[0],), dtype=np.float32
-                )
-                marginal_density[gpu_is_track_interior] = estimate_position_density(
-                    interior_place_bin_centers,
-                    np.asarray(position[is_spike & not_nan_position], dtype=np.float32),
-                    position_std,
-                    block_size=block_size,
+                    dtype=cp.float32,
                 )
+            )
+        else:
+            log_occupancy = cp.zeros((place_bin_centers.shape[0],), dtype=cp.float32)
+            log_occupancy[gpu_is_track_interior] = estimate_log_position_density(
+                interior_place_bin_centers,
+                cp.asarray(position[not_nan_position], dtype=cp.float32),
+                position_std,
+                block_size=block_size,
+            )
 
-        summed_ground_process_intensity += estimate_intensity(
-            marginal_density, occupancy, mean_rates[-1]
-        )
+        log_mean_rates = []
+        encoding_marks = []
+        encoding_positions = []
+        summed_ground_process_intensity = cp.zeros(
+            (place_bin_centers.shape[0],), dtype=cp.float32
+        )
+
+        for multiunit in np.moveaxis(multiunits, -1, 0):
+
+            # ground process intensity
+            is_spike = np.any(~np.isnan(multiunit), axis=1)
+            log_mean_rates.append(np.log(is_spike.mean()))
+
+            if is_spike.sum() > 0:
+                if use_diffusion & (position.shape[1] > 1):
+                    log_marginal_density = cp.log(
+                        cp.asarray(
+                            estimate_diffusion_position_density(
+                                position[is_spike & not_nan_position],
+                                edges,
+                                bin_distances=bin_diffusion_distances,
+                            ),
+                            dtype=cp.float32,
+                        )
+                    )
+                else:
+                    log_marginal_density = cp.zeros(
+                        (place_bin_centers.shape[0],), dtype=cp.float32
+                    )
+                    log_marginal_density[
+                        gpu_is_track_interior
+                    ] = estimate_log_position_density(
+                        interior_place_bin_centers,
+                        cp.asarray(
+                            position[is_spike & not_nan_position], dtype=cp.float32
+                        ),
+                        position_std,
+                        block_size=block_size,
+                    )
 
-        is_mark_features = np.any(~np.isnan(multiunit), axis=0)
-        encoding_marks.append(
-            np.asarray(
-                multiunit[np.ix_(is_spike & not_nan_position, is_mark_features)],
-                dtype=np.int16,
+            summed_ground_process_intensity += estimate_intensity(
+                log_marginal_density, log_occupancy, log_mean_rates[-1]
             )
-        )
-        encoding_positions.append(position[is_spike & not_nan_position])
 
-    summed_ground_process_intensity = summed_ground_process_intensity + np.spacing(1)
-
-    return {
-        "encoding_marks": encoding_marks,
-        "encoding_positions": encoding_positions,
-        "summed_ground_process_intensity": summed_ground_process_intensity,
-        "occupancy": occupancy,
-        "mean_rates": mean_rates,
-        "mark_std": mark_std,
-        "position_std": position_std,
-        "block_size": block_size,
-        "bin_diffusion_distances": bin_diffusion_distances,
-        "use_diffusion": use_diffusion,
-        "edges": edges,
-        **kwargs,
-    }
-
-
-def estimate_multiunit_likelihood_integer(
-    multiunits,
-    encoding_marks,
-    mark_std,
-    place_bin_centers,
-    encoding_positions,
-    position_std,
-    occupancy,
-    mean_rates,
-    summed_ground_process_intensity,
-    bin_diffusion_distances,
-    edges,
-    max_mark_diff=6000,
-    set_diag_zero=False,
-    is_track_interior=None,
-    time_bin_size=1,
-    block_size=100,
-    ignore_no_spike=False,
-    disable_progress_bar=False,
-    use_diffusion=False,
-):
-    """Estimates the likelihood of position bins given multiunit marks.
-
-    Parameters
-    ----------
-    multiunits : np.ndarray, shape (n_decoding_time, n_marks, n_electrodes)
-    encoding_marks : cp.ndarray, shape (n_encoding_spikes, n_marks, n_electrodes)
-    mark_std : float
-        Amount of smoothing for mark features.  Standard deviation of kernel.
-    place_bin_centers : cp.ndarray, shape (n_bins, n_position_dims)
-    encoding_positions : cp.ndarray, shape (n_encoding_spikes, n_position_dims)
-    position_std : float or array_like, shape (n_position_dims,)
-        Amount of smoothing for position.  Standard deviation of kernel.
-    occupancy : cp.ndarray, (n_bins,)
-    mean_rates : list, len (n_electrodes,)
-    summed_ground_process_intensity : np.ndarray, shape (n_bins,)
-    bin_diffusion_distances : np.ndarray, shape (n_bins, n_bins)
-    edges : list of np.ndarray
-    max_mark_diff : int
-        Maximum difference between mark features
-    set_diag_zero : bool
-        Remove influence of the same mark in encoding and decoding.
-    is_track_interior : None or np.ndarray, shape (n_bins_x, n_bins_y)
-    time_bin_size : float
-        Size of time steps
-    block_size : int
-        Size of data to process in chunks
-    ignore_no_spike : bool
-        Set contribution of no spikes to zero
-    disable_progress_bar : bool
-        If False, a progress bar will be displayed.
-    use_diffusion : bool
-        Respect track geometry by using diffusion distances
-
-    Returns
-    -------
-    log_likelihood : (n_time, n_bins)
-
-    """
-
-    if is_track_interior is None:
-        is_track_interior = np.ones((place_bin_centers.shape[0],), dtype=np.bool)
-    else:
-        is_track_interior = is_track_interior.ravel(order="F")
-
-    n_time = multiunits.shape[0]
-    if ignore_no_spike:
-        log_likelihood = (
-            -time_bin_size
-            * summed_ground_process_intensity
-            * np.zeros((n_time, 1), dtype=np.float32)
-        )
-    else:
-        log_likelihood = (
-            -time_bin_size
-            * summed_ground_process_intensity
-            * np.ones((n_time, 1), dtype=np.float32)
-        )
+            is_mark_features = np.any(~np.isnan(multiunit), axis=0)
+            encoding_marks.append(
+                cp.asarray(
+                    multiunit[np.ix_(is_spike & not_nan_position, is_mark_features)],
+                    dtype=cp.int16,
+                )
+            )
+            encoding_positions.append(position[is_spike & not_nan_position])
 
-    multiunits = np.moveaxis(multiunits, -1, 0)
-    n_position_bins = is_track_interior.sum()
-    interior_place_bin_centers = np.asarray(
-        place_bin_centers[is_track_interior], dtype=np.float32
-    )
-    gpu_is_track_interior = np.asarray(is_track_interior)
-    interior_occupancy = occupancy[gpu_is_track_interior]
+        summed_ground_process_intensity = cp.asnumpy(
+            summed_ground_process_intensity
+        ) + np.spacing(1)
+
+        return {
+            "encoding_marks": encoding_marks,
+            "encoding_positions": encoding_positions,
+            "summed_ground_process_intensity": summed_ground_process_intensity,
+            "log_occupancy": log_occupancy,
+            "log_mean_rates": log_mean_rates,
+            "mark_std": mark_std,
+            "position_std": position_std,
+            "block_size": block_size,
+            "bin_diffusion_distances": bin_diffusion_distances,
+            "use_diffusion": use_diffusion,
+            "edges": edges,
+            **kwargs,
+        }
 
-    for multiunit, enc_marks, enc_pos, mean_rate in zip(
-        tqdm(multiunits, desc="n_electrodes", disable=disable_progress_bar),
+    def estimate_multiunit_likelihood_integer_gpu_log(
+        multiunits,
         encoding_marks,
+        mark_std,
+        place_bin_centers,
         encoding_positions,
-        mean_rates,
+        position_std,
+        log_occupancy,
+        log_mean_rates,
+        summed_ground_process_intensity,
+        bin_diffusion_distances,
+        edges,
+        max_mark_diff=6000,
+        set_diag_zero=False,
+        is_track_interior=None,
+        time_bin_size=1,
+        block_size=100,
+        ignore_no_spike=False,
+        disable_progress_bar=False,
+        use_diffusion=False,
     ):
-        is_spike = np.any(~np.isnan(multiunit), axis=1)
-        is_mark_features = np.any(~np.isnan(multiunit), axis=0)
-        decoding_marks = np.asarray(
-            multiunit[np.ix_(is_spike, is_mark_features)], dtype=np.int16
-        )
-        n_decoding_marks = decoding_marks.shape[0]
-        log_joint_mark_intensity = np.zeros(
-            (n_decoding_marks, n_position_bins), dtype=np.float32
-        )
+        """Estimates the likelihood of position bins given multiunit marks.
 
-        if block_size is None:
-            block_size = n_decoding_marks
+        Parameters
+        ----------
+        multiunits : np.ndarray, shape (n_decoding_time, n_marks, n_electrodes)
+        encoding_marks : cp.ndarray, shape (n_encoding_spikes, n_marks, n_electrodes)
+        mark_std : float
+            Amount of smoothing for mark features
+        place_bin_centers : cp.ndarray, shape (n_bins, n_position_dims)
+        encoding_positions : cp.ndarray, shape (n_encoding_spikes, n_position_dims)
+        position_std : float or array_like, shape (n_position_dims,)
+            Amount of smoothing for position
+        log_occupancy : cp.ndarray, (n_bins,)
+        log_mean_rates : list, len (n_electrodes,)
+        summed_ground_process_intensity : np.ndarray, shape (n_bins,)
+        bin_diffusion_distances : np.ndarray, shape (n_bins, n_bins)
+        edges : list of np.ndarray
+        max_mark_diff : int
+            Maximum difference between mark features
+        set_diag_zero : bool
+            Remove influence of the same mark in encoding and decoding.
+        is_track_interior : None or np.ndarray, shape (n_bins_x, n_bins_y)
+        time_bin_size : float
+            Size of time steps
+        block_size : int
+            Size of data to process in chunks
+        ignore_no_spike : bool
+            Set contribution of no spikes to zero
+        disable_progress_bar : bool
+            If False, a progress bar will be displayed.
+        use_diffusion : bool
+            Respect track geometry by using diffusion distances
+
+        Returns
+        -------
+        log_likelihood : (n_time, n_bins)
 
-        if use_diffusion & (place_bin_centers.shape[1] > 1):
-            position_distance = np.asarray(
-                estimate_diffusion_position_distance(
-                    enc_pos,
-                    edges,
-                    bin_distances=bin_diffusion_distances,
-                )[:, is_track_interior],
-                dtype=np.float32,
+        """
+
+        if is_track_interior is None:
+            is_track_interior = np.ones((place_bin_centers.shape[0],), dtype=np.bool)
+        else:
+            is_track_interior = is_track_interior.ravel(order="F")
+
+        n_time = multiunits.shape[0]
+        if ignore_no_spike:
+            log_likelihood = (
+                -time_bin_size
+                * summed_ground_process_intensity
+                * np.zeros((n_time, 1), dtype=np.float32)
             )
         else:
-            position_distance = estimate_position_distance(
-                interior_place_bin_centers,
-                np.asarray(enc_pos, dtype=np.float32),
-                position_std,
-            ).astype(np.float32)
+            log_likelihood = (
+                -time_bin_size
+                * summed_ground_process_intensity
+                * np.ones((n_time, 1), dtype=np.float32)
+            )
 
-        for start_ind in range(0, n_decoding_marks, block_size):
-            block_inds = slice(start_ind, start_ind + block_size)
-            log_joint_mark_intensity[block_inds] = estimate_log_joint_mark_intensity(
-                decoding_marks[block_inds],
-                enc_marks,
-                mark_std,
-                interior_occupancy,
-                mean_rate,
-                max_mark_diff=max_mark_diff,
-                set_diag_zero=set_diag_zero,
-                position_distance=position_distance,
+        multiunits = np.moveaxis(multiunits, -1, 0)
+        n_position_bins = is_track_interior.sum()
+        interior_place_bin_centers = cp.asarray(
+            place_bin_centers[is_track_interior], dtype=cp.float32
+        )
+        gpu_is_track_interior = cp.asarray(is_track_interior)
+        interior_log_occupancy = log_occupancy[gpu_is_track_interior]
+
+        for multiunit, enc_marks, enc_pos, log_mean_rate in zip(
+            tqdm(multiunits, desc="n_electrodes", disable=disable_progress_bar),
+            encoding_marks,
+            encoding_positions,
+            log_mean_rates,
+        ):
+            is_spike = np.any(~np.isnan(multiunit), axis=1)
+            is_mark_features = np.any(~np.isnan(multiunit), axis=0)
+            decoding_marks = cp.asarray(
+                multiunit[np.ix_(is_spike, is_mark_features)], dtype=cp.int16
             )
-        log_likelihood[np.ix_(is_spike, is_track_interior)] += np.nan_to_num(
-            log_joint_mark_intensity
-        )
+            n_decoding_marks = decoding_marks.shape[0]
+            log_joint_mark_intensity = np.zeros(
+                (n_decoding_marks, n_position_bins), dtype=np.float32
+            )
+
+            if block_size is None:
+                block_size = n_decoding_marks
+
+            if use_diffusion & (place_bin_centers.shape[1] > 1):
+                log_position_distances = cp.log(
+                    cp.asarray(
+                        estimate_diffusion_position_distance(
+                            enc_pos,
+                            edges,
+                            bin_distances=bin_diffusion_distances,
+                        )[:, is_track_interior],
+                        dtype=cp.float32,
+                    )
+                )
+            else:
+                log_position_distances = estimate_log_position_distance(
+                    interior_place_bin_centers,
+                    cp.asarray(enc_pos, dtype=cp.float32),
+                    position_std,
+                ).astype(cp.float32)
+
+            for start_ind in range(0, n_decoding_marks, block_size):
+                block_inds = slice(start_ind, start_ind + block_size)
+                log_joint_mark_intensity[
+                    block_inds
+                ] = estimate_log_joint_mark_intensity(
+                    decoding_marks[block_inds],
+                    enc_marks,
+                    mark_std,
+                    log_position_distances,
+                    interior_log_occupancy,
+                    log_mean_rate,
+                    max_mark_diff=max_mark_diff,
+                    set_diag_zero=set_diag_zero,
+                )
+            log_likelihood[np.ix_(is_spike, is_track_interior)] += np.nan_to_num(
+                log_joint_mark_intensity
+            )
+
+            mempool = cp.get_default_memory_pool()
+            mempool.free_all_blocks()
+
+        log_likelihood[:, ~is_track_interior] = np.nan
+
+        return log_likelihood
+
+except ImportError:
 
-    log_likelihood[:, ~is_track_interior] = np.nan
+    def estimate_multiunit_likelihood_integer_gpu_log(*args, **kwargs):
+        print("Cupy is not installed or no GPU detected...")
 
-    return log_likelihood
+    def fit_multiunit_likelihood_integer_gpu_log(*args, **kwargs):
+        print("Cupy is not installed or no GPU detected...")
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer_gpu.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer_gpu.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 """Estimates a marked point process likelihood where the marks are
  features of the spike waveform using GPUs. Mark features are int16.
 
  Marks are converted to integers and KDE uses hash tables to compute Gaussian
  kernels."""
 
 
+from typing import Optional, Union
+
 import numpy as np
+from tqdm.autonotebook import tqdm
+
 from replay_trajectory_classification.core import atleast_2d
 from replay_trajectory_classification.likelihoods.diffusion import (
     diffuse_each_bin,
     estimate_diffusion_position_density,
     estimate_diffusion_position_distance,
 )
-from tqdm.autonotebook import tqdm
 
 try:
     import cupy as cp
 
     @cp.fuse
-    def gaussian_pdf(x, mean, sigma):
+    def gaussian_pdf(x: cp.ndarray, mean: cp.ndarray, sigma: cp.ndarray) -> cp.ndarray:
         """Compute the value of a Gaussian probability density function at x with
         given mean and sigma."""
         return cp.exp(-0.5 * ((x - mean) / sigma) ** 2) / (sigma * cp.sqrt(2.0 * cp.pi))
 
-    def estimate_position_distance(place_bin_centers, positions, position_std):
+    def estimate_position_distance(
+        place_bin_centers: cp.ndarray, positions: cp.ndarray, position_std: cp.ndarray
+    ) -> cp.ndarray:
         """Estimates the Euclidean distance between positions and position bins.
 
         Parameters
         ----------
-        place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
-        positions : np.ndarray, shape (n_time, n_position_dims)
-        position_std : array_like, shape (n_position_dims,)
+        place_bin_centers : cp.ndarray, shape (n_position_bins, n_position_dims)
+        positions : cp.ndarray, shape (n_time, n_position_dims)
+        position_std : cp.ndarray, shape (n_position_dims,)
 
         Returns
         -------
-        position_distance : np.ndarray, shape (n_time, n_position_bins)
+        position_distance : cp.ndarray, shape (n_time, n_position_bins)
 
         """
         n_time, n_position_dims = positions.shape
         n_position_bins = place_bin_centers.shape[0]
 
         if isinstance(position_std, (int, float)):
             position_std = [position_std] * n_position_dims
@@ -51,28 +56,31 @@
                 cp.expand_dims(positions[:, position_ind], axis=1),
                 std,
             )
 
         return position_distance
 
     def estimate_position_density(
-        place_bin_centers, positions, position_std, block_size=100
-    ):
+        place_bin_centers: cp.ndarray,
+        positions: cp.ndarray,
+        position_std: Union[cp.ndarray, float],
+        block_size: Optional[int] = 100,
+    ) -> cp.ndarray:
         """Estimates a kernel density estimate over position bins using
         Euclidean distances.
 
         Parameters
         ----------
-        place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
-        positions : np.ndarray, shape (n_time, n_position_dims)
+        place_bin_centers : cp.ndarray, shape (n_position_bins, n_position_dims)
+        positions : cp.ndarray, shape (n_time, n_position_dims)
         position_std : float or array_like, shape (n_position_dims,)
 
         Returns
         -------
-        position_density : np.ndarray, shape (n_position_bins,)
+        position_density : cp.ndarray, shape (n_position_bins,)
 
         """
         n_time = positions.shape[0]
         n_position_bins = place_bin_centers.shape[0]
 
         if block_size is None:
             block_size = n_time
@@ -84,19 +92,23 @@
                 estimate_position_distance(
                     place_bin_centers[block_inds], positions, position_std
                 ),
                 axis=0,
             )
         return position_density
 
-    def estimate_log_intensity(density, occupancy, mean_rate):
+    def estimate_log_intensity(
+        density: cp.ndarray, occupancy: cp.ndarray, mean_rate: float
+    ):
         """Calculates intensity in log space."""
         return cp.log(mean_rate) + cp.log(density) - cp.log(occupancy)
 
-    def estimate_intensity(density, occupancy, mean_rate):
+    def estimate_intensity(
+        density: cp.ndarray, occupancy: cp.ndarray, mean_rate: float
+    ) -> cp.ndarray:
         """Calculates intensity.
 
         Parameters
         ----------
         density : np.ndarray, shape (n_bins,)
         occupancy : np.ndarray, shape (n_bins,)
         mean_rate : float
@@ -104,15 +116,17 @@
         Returns
         -------
         intensity : np.ndarray, shape (n_bins,)
 
         """
         return cp.exp(estimate_log_intensity(density, occupancy, mean_rate))
 
-    def normal_pdf_integer_lookup(x, mean, std=20, max_value=6000):
+    def normal_pdf_integer_lookup(
+        x: int, mean: int, std: float = 20.0, max_value: int = 6000
+    ):
         """Fast density evaluation for integers by precomputing a hash table of
         values.
 
         Parameters
         ----------
         x : int
         mean : int
@@ -127,26 +141,26 @@
         normal_density = gaussian_pdf(cp.arange(-max_value, max_value), 0, std).astype(
             cp.float32
         )
 
         return normal_density[(x - mean) + max_value]
 
     def estimate_log_joint_mark_intensity(
-        decoding_marks,
-        encoding_marks,
-        mark_std,
-        occupancy,
-        mean_rate,
-        place_bin_centers=None,
-        encoding_positions=None,
-        position_std=None,
-        max_mark_diff=6000,
-        set_diag_zero=False,
-        position_distance=None,
-    ):
+        decoding_marks: cp.ndarray,
+        encoding_marks: cp.ndarray,
+        mark_std: float,
+        occupancy: cp.ndarray,
+        mean_rate: float,
+        place_bin_centers: Optional[cp.ndarray] = None,
+        encoding_positions: Optional[cp.ndarray] = None,
+        position_std: Union[float, cp.ndarray, None] = None,
+        max_mark_diff: int = 6000,
+        set_diag_zero: bool = False,
+        position_distance: Optional[cp.ndarray] = None,
+    ) -> np.ndarray:
         """Finds the joint intensity of the marks and positions in log space.
 
         Parameters
         ----------
         decoding_marks : np.ndarray, shape (n_decoding_spikes, n_features)
         encoding_marks : np.ndarray, shape (n_encoding_spikes, n_features)
         mark_std : float
@@ -197,24 +211,24 @@
                 mark_distance @ position_distance / n_encoding_spikes,
                 occupancy,
                 mean_rate,
             )
         )
 
     def fit_multiunit_likelihood_integer_gpu(
-        position,
-        multiunits,
-        place_bin_centers,
-        mark_std,
-        position_std,
-        is_track_boundary=None,
-        is_track_interior=None,
-        edges=None,
-        block_size=100,
-        use_diffusion=False,
+        position: np.ndarray,
+        multiunits: np.ndarray,
+        place_bin_centers: np.ndarray,
+        mark_std: float,
+        position_std: Union[float, np.ndarray],
+        is_track_boundary: Optional[np.ndarray] = None,
+        is_track_interior: Optional[np.ndarray] = None,
+        edges: Optional[list[np.ndarray]] = None,
+        block_size: int = 100,
+        use_diffusion: bool = False,
         **kwargs
     ):
         """Fits the clusterless place field model.
 
         Parameters
         ----------
         position : np.ndarray, shape (n_time, n_position_dims)
@@ -344,45 +358,45 @@
             "bin_diffusion_distances": bin_diffusion_distances,
             "use_diffusion": use_diffusion,
             "edges": edges,
             **kwargs,
         }
 
     def estimate_multiunit_likelihood_integer_gpu(
-        multiunits,
-        encoding_marks,
-        mark_std,
-        place_bin_centers,
-        encoding_positions,
-        position_std,
-        occupancy,
-        mean_rates,
-        summed_ground_process_intensity,
-        bin_diffusion_distances,
-        edges,
-        max_mark_diff=6000,
-        set_diag_zero=False,
-        is_track_interior=None,
-        time_bin_size=1,
-        block_size=100,
-        ignore_no_spike=False,
-        disable_progress_bar=False,
-        use_diffusion=False,
+        multiunits: np.ndarray,
+        encoding_marks: cp.ndarray,
+        mark_std: float,
+        place_bin_centers: cp.ndarray,
+        encoding_positions: cp.ndarray,
+        position_std: Union[float, np.ndarray],
+        occupancy: cp.ndarray,
+        mean_rates: list,
+        summed_ground_process_intensity: np.ndarray,
+        bin_diffusion_distances: np.ndarray,
+        edges: list[np.ndarray],
+        max_mark_diff: int = 6000,
+        set_diag_zero: bool = False,
+        is_track_interior: Optional[np.ndarray] = None,
+        time_bin_size: int = 1,
+        block_size: int = 100,
+        ignore_no_spike: bool = False,
+        disable_progress_bar: bool = False,
+        use_diffusion: bool = False,
     ):
         """Estimates the likelihood of position bins given multiunit marks.
 
         Parameters
         ----------
         multiunits : np.ndarray, shape (n_decoding_time, n_marks, n_electrodes)
         encoding_marks : cp.ndarray, shape (n_encoding_spikes, n_marks, n_electrodes)
         mark_std : float
             Amount of smoothing for mark features.  Standard deviation of kernel.
         place_bin_centers : cp.ndarray, shape (n_bins, n_position_dims)
         encoding_positions : cp.ndarray, shape (n_encoding_spikes, n_position_dims)
-        position_std : float or array_like, shape (n_position_dims,)
+        position_std : float or np.ndarray, shape (n_position_dims,)
             Amount of smoothing for position.  Standard deviation of kernel.
         occupancy : cp.ndarray, (n_bins,)
         mean_rates : list, len (n_electrodes,)
         summed_ground_process_intensity : np.ndarray, shape (n_bins,)
         bin_diffusion_distances : np.ndarray, shape (n_bins, n_bins)
         edges : list of np.ndarray
         max_mark_diff : int
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood_integer_gpu_log.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood_gpu.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,262 +1,231 @@
 """Estimates a marked point process likelihood where the marks are
- features of the spike waveform using GPUs. Mark features are int16.
+ features of the spike waveform using GPUs. Features are float32."""
 
- This algorithm is more numerically stable KDE done in log space but slower
- right now because of lack of matrix multiplication.
-
- Marks are converted to integers and KDE uses hash tables to compute Gaussian
- kernels."""
-
-
-import math
+from typing import Optional, Union
 
 import numpy as np
-from numba import cuda
+from tqdm.autonotebook import tqdm
+
 from replay_trajectory_classification.core import atleast_2d
 from replay_trajectory_classification.likelihoods.diffusion import (
     diffuse_each_bin,
     estimate_diffusion_position_density,
     estimate_diffusion_position_distance,
 )
-from tqdm.autonotebook import tqdm
 
 try:
     import cupy as cp
 
-    def logsumexp(a, axis):
-        a_max = cp.amax(a, axis=axis, keepdims=True)
-
-        if a_max.ndim > 0:
-            a_max[~cp.isfinite(a_max)] = 0
-        elif not np.isfinite(a_max):
-            a_max = 0
-
-        return cp.log(cp.sum(cp.exp(a - a_max), axis=axis, keepdims=True)) + a_max
-
-    def log_mean(x, axis):
-        return cp.squeeze(logsumexp(x, axis=axis) - cp.log(x.shape[axis]))
-
-    @cp.fuse()
-    def log_gaussian_pdf(x, sigma):
-        return -cp.log(sigma) - 0.5 * cp.log(2 * cp.pi) - 0.5 * (x / sigma) ** 2
-
-    @cp.fuse()
-    def estimate_log_intensity(log_density, log_occupancy, log_mean_rate):
-        return log_mean_rate + log_density - log_occupancy
-
-    @cp.fuse()
-    def estimate_intensity(log_density, log_occupancy, log_mean_rate):
-        return cp.exp(estimate_log_intensity(log_density, log_occupancy, log_mean_rate))
-
-    def estimate_log_position_distance(place_bin_centers, positions, position_std):
+    @cp.fuse
+    def gaussian_pdf(x: cp.ndarray, mean: cp.ndarray, sigma: cp.ndarray) -> cp.ndarray:
+        """Compute the value of a Gaussian probability density function at x with
+        given mean and sigma."""
+        return cp.exp(-0.5 * ((x - mean) / sigma) ** 2) / (sigma * cp.sqrt(2.0 * cp.pi))
+
+    def estimate_position_distance(
+        place_bin_centers: cp.ndarray,
+        positions: cp.ndarray,
+        position_std: Union[float, cp.ndarray],
+    ) -> cp.ndarray:
         """Estimates the Euclidean distance between positions and position bins.
 
         Parameters
         ----------
         place_bin_centers : cp.ndarray, shape (n_position_bins, n_position_dims)
         positions : cp.ndarray, shape (n_time, n_position_dims)
-        position_std : array_like, shape (n_position_dims,)
+        position_std : cp.ndarray, shape (n_position_dims,)
 
         Returns
         -------
-        log_position_distance : np.ndarray, shape (n_time, n_position_bins)
+        position_distance : cp.ndarray, shape (n_time, n_position_bins)
 
         """
         n_time, n_position_dims = positions.shape
         n_position_bins = place_bin_centers.shape[0]
 
         if isinstance(position_std, (int, float)):
             position_std = [position_std] * n_position_dims
 
-        log_position_distance = cp.zeros((n_time, n_position_bins), dtype=cp.float32)
+        position_distance = cp.ones((n_time, n_position_bins), dtype=cp.float32)
 
         for position_ind, std in enumerate(position_std):
-            log_position_distance += log_gaussian_pdf(
-                cp.expand_dims(place_bin_centers[:, position_ind], axis=0)
-                - cp.expand_dims(positions[:, position_ind], axis=1),
+            position_distance *= gaussian_pdf(
+                cp.expand_dims(place_bin_centers[:, position_ind], axis=0),
+                cp.expand_dims(positions[:, position_ind], axis=1),
                 std,
             )
 
-        return log_position_distance
+        return position_distance
 
-    def estimate_log_position_density(
-        place_bin_centers, positions, position_std, block_size=100
-    ):
+    def estimate_position_density(
+        place_bin_centers: cp.ndarray,
+        positions: cp.ndarray,
+        position_std: Union[float, cp.ndarray],
+        block_size: int = 100,
+    ) -> cp.ndarray:
         """Estimates a kernel density estimate over position bins using
         Euclidean distances.
 
         Parameters
         ----------
         place_bin_centers : cp.ndarray, shape (n_position_bins, n_position_dims)
         positions : cp.ndarray, shape (n_time, n_position_dims)
-        position_std : float or array_like, shape (n_position_dims,)
-        block_size : int
+        position_std : float or cp.ndarray, shape (n_position_dims,)
 
         Returns
         -------
-        log_position_density : cp.ndarray, shape (n_position_bins,)
+        position_density : cp.ndarray, shape (n_position_bins,)
 
         """
         n_time = positions.shape[0]
         n_position_bins = place_bin_centers.shape[0]
 
         if block_size is None:
             block_size = n_time
 
-        log_position_density = cp.empty((n_position_bins,))
+        position_density = cp.empty((n_position_bins,))
         for start_ind in range(0, n_position_bins, block_size):
             block_inds = slice(start_ind, start_ind + block_size)
-            log_position_density[block_inds] = log_mean(
-                estimate_log_position_distance(
+            position_density[block_inds] = cp.mean(
+                estimate_position_distance(
                     place_bin_centers[block_inds], positions, position_std
                 ),
                 axis=0,
             )
+        return position_density
 
-        return log_position_density
-
-    @cuda.jit()
-    def log_mean_over_bins(log_mark_distances, log_position_distances, output):
-        """
+    def estimate_log_intensity(
+        density: cp.ndarray, occupancy: cp.ndarray, mean_rate: float
+    ) -> cp.ndarray:
+        """Calculates intensity in log space."""
+        return cp.log(mean_rate) + cp.log(density) - cp.log(occupancy)
+
+    def estimate_intensity(
+        density: cp.ndarray, occupancy: cp.ndarray, mean_rate: float
+    ) -> cp.ndarray:
+        """Calculates intensity.
 
         Parameters
         ----------
-        log_mark_distances : cp.ndarray, shape (n_decoding_spikes, n_encoding_spikes)
-        log_position_distances : cp.ndarray, shape (n_encoding_spikes, n_position_bins)
+        density : cp.ndarray, shape (n_bins,)
+        occupancy : cp.ndarray, shape (n_bins,)
+        mean_rate : float
 
         Returns
         -------
-        output : cp.ndarray, shape (n_decoding_spikes, n_position_bins)
+        intensity : cp.ndarray, shape (n_bins,)
 
         """
-        thread_id = cuda.grid(1)
-
-        n_decoding_spikes, n_position_bins = output.shape
-        n_encoding_spikes = log_position_distances.shape[0]
-
-        decoding_ind = thread_id // n_position_bins
-        pos_bin_ind = thread_id % n_position_bins
-
-        if (decoding_ind < n_decoding_spikes) and (pos_bin_ind < n_position_bins):
-
-            # find maximum
-            max_exp = (
-                log_mark_distances[decoding_ind, 0]
-                + log_position_distances[0, pos_bin_ind]
-            )
-
-            for encoding_ind in range(1, n_encoding_spikes):
-                candidate_max = (
-                    log_mark_distances[decoding_ind, encoding_ind]
-                    + log_position_distances[encoding_ind, pos_bin_ind]
-                )
-                if candidate_max > max_exp:
-                    max_exp = candidate_max
-
-            # logsumexp
-            tmp = 0.0
-            for encoding_ind in range(n_encoding_spikes):
-                tmp += math.exp(
-                    log_mark_distances[decoding_ind, encoding_ind]
-                    + log_position_distances[encoding_ind, pos_bin_ind]
-                    - max_exp
-                )
-
-            output[decoding_ind, pos_bin_ind] = math.log(tmp) + max_exp
-
-            # divide by n_spikes to get the mean
-            output[decoding_ind, pos_bin_ind] -= math.log(n_encoding_spikes)
+        return cp.exp(estimate_log_intensity(density, occupancy, mean_rate))
 
     def estimate_log_joint_mark_intensity(
-        decoding_marks,
-        encoding_marks,
-        mark_std,
-        log_position_distances,
-        log_occupancy,
-        log_mean_rate,
-        max_mark_diff=6000,
-        set_diag_zero=False,
-    ):
+        decoding_marks: cp.ndarray,
+        encoding_marks: cp.ndarray,
+        mark_std: Union[float, cp.ndarray],
+        occupancy: cp.ndarray,
+        mean_rate: float,
+        place_bin_centers: Optional[cp.ndarray] = None,
+        encoding_positions: Optional[cp.ndarray] = None,
+        position_std: Union[float, cp.ndarray, None] = None,
+        max_mark_diff: int = 6000,
+        set_diag_zero: bool = False,
+        position_distance: Optional[cp.ndarray] = None,
+    ) -> np.ndarray:
         """Finds the joint intensity of the marks and positions in log space.
 
         Parameters
         ----------
-        decoding_marks : cp.ndarray, shape (n_decoding_spikes, n_features)
-        encoding_marks : cp.ndarray, shape (n_encoding_spikes, n_features)
-        mark_std : float
-        log_position_distance : cp.ndarray, shape (n_encoding_spikes, n_position_bins)
-            Precalculated distance between position and position bins.
-        log_occupancy : cp.ndarray, shape (n_position_bins,)
-        log_mean_rate : float
+        decoding_marks : np.ndarray, shape (n_decoding_spikes, n_features)
+        encoding_marks : np.ndarray, shape (n_encoding_spikes, n_features)
+        mark_std : float or np.ndarray, shape (n_features,)
+        occupancy : np.ndarray, shape (n_position_bins,)
+        mean_rate : float
+        place_bin_centers : None or np.ndarray, shape (n_position_bins, n_position_dims)
+            If None, position distance must be not None
+        encoding_positions : None or np.ndarray, shape (n_decoding_spikes, n_position_dims)
+            If None, position distance must be not None
+        position_std : None or float or array_like, shape (n_position_dims,)
+            If None, position distance must be not None
         max_mark_diff : int
             Maximum distance between integer marks.
         set_diag_zero : bool
+        position_distance : np.ndarray, shape (n_encoding_spikes, n_position_bins)
+            Precalculated distance between position and position bins.
 
         Returns
         -------
         log_joint_mark_intensity : np.ndarray, shape (n_decoding_spikes, n_position_bins)
 
         """
         n_encoding_spikes, n_marks = encoding_marks.shape
+
         n_decoding_spikes = decoding_marks.shape[0]
-        log_mark_distances = cp.zeros(
+        mark_distance = cp.ones(
             (n_decoding_spikes, n_encoding_spikes), dtype=cp.float32
         )
 
-        log_normal_pdf_lookup = cp.asarray(
-            log_gaussian_pdf(cp.arange(-max_mark_diff, max_mark_diff), mark_std),
-            dtype=cp.float32,
-        )
-
         for mark_ind in range(n_marks):
-            log_mark_distances += log_normal_pdf_lookup[
-                (
-                    cp.expand_dims(decoding_marks[:, mark_ind], axis=1)
-                    - cp.expand_dims(encoding_marks[:, mark_ind], axis=0)
-                )
-                + max_mark_diff
-            ]
+            mark_distance *= gaussian_pdf(
+                cp.expand_dims(decoding_marks[:, mark_ind], axis=1),
+                cp.expand_dims(encoding_marks[:, mark_ind], axis=0),
+                mark_std[mark_ind],
+            )
 
         if set_diag_zero:
             diag_ind = (cp.arange(n_decoding_spikes), cp.arange(n_decoding_spikes))
-            log_mark_distances[diag_ind] = cp.nan_to_num(cp.log(0).astype(cp.float32))
-
-        n_position_bins = log_position_distances.shape[1]
-        pdf = cp.empty((n_decoding_spikes, n_position_bins), dtype=cp.float32)
+            mark_distance[diag_ind] = 0.0
 
-        log_mean_over_bins.forall(pdf.size)(
-            log_mark_distances, log_position_distances, pdf
+        if position_distance is None:
+            position_distance = estimate_position_distance(
+                place_bin_centers, encoding_positions, position_std
+            ).astype(cp.float32)
+
+        return cp.asnumpy(
+            estimate_log_intensity(
+                mark_distance @ position_distance / n_encoding_spikes,
+                occupancy,
+                mean_rate,
+            )
         )
 
-        return cp.asnumpy(estimate_log_intensity(pdf, log_occupancy, log_mean_rate))
-
-    def fit_multiunit_likelihood_integer_gpu_log(
-        position,
-        multiunits,
-        place_bin_centers,
-        mark_std,
-        position_std,
-        is_track_boundary=None,
-        is_track_interior=None,
-        edges=None,
-        block_size=100,
-        use_diffusion=False,
+    def fit_multiunit_likelihood_gpu(
+        position: np.ndarray,
+        multiunits: np.ndarray,
+        place_bin_centers: np.ndarray,
+        mark_std: Union[float, np.ndarray],
+        position_std: Union[float, np.ndarray],
+        is_track_boundary: Optional[np.ndarray] = None,
+        is_track_interior: Optional[np.ndarray] = None,
+        edges: Optional[list[np.ndarray]] = None,
+        block_size: int = 100,
+        use_diffusion: bool = False,
         **kwargs
-    ):
+    ) -> dict[
+        cp.ndarray,
+        cp.ndarray,
+        cp.ndarray,
+        cp.ndarray,
+        cp.ndarray,
+        np.ndarray,
+        np.ndarray,
+        int,
+        np.ndarray,
+        list[np.ndarray],
+    ]:
         """Fits the clusterless place field model.
 
         Parameters
         ----------
         position : np.ndarray, shape (n_time, n_position_dims)
         multiunits : np.ndarray, shape (n_time, n_marks, n_electrodes)
         place_bin_centers : np.ndarray, shape (n_bins, n_position_dims)
-        mark_std : float
+        mark_std : float or np.ndarray, shape (n_marks,)
             Amount of smoothing for the mark features.  Standard deviation of kernel.
-        position_std : float or array_like, shape (n_position_dims,)
+        position_std : float or np.ndarray, shape (n_position_dims,)
             Amount of smoothing for position.  Standard deviation of kernel.
         is_track_boundary : None or np.ndarray, shape (n_bins,)
         is_track_interior : None or np.ndarray, shape (n_bins,)
         edges : None or list of np.ndarray
         block_size : int
             Size of data to process in chunks
         use_diffusion : bool
@@ -288,140 +257,140 @@
                 dy=edges[1][1] - edges[1][0],
                 std=position_std,
             ).reshape((n_total_bins, -1), order="F")
         else:
             bin_diffusion_distances = None
 
         if use_diffusion & (position.shape[1] > 1):
-            log_occupancy = cp.log(
-                cp.asarray(
-                    estimate_diffusion_position_density(
-                        position[not_nan_position],
-                        edges,
-                        bin_distances=bin_diffusion_distances,
-                    ),
-                    dtype=cp.float32,
-                )
+            occupancy = cp.asarray(
+                estimate_diffusion_position_density(
+                    position[not_nan_position],
+                    edges,
+                    bin_distances=bin_diffusion_distances,
+                ),
+                dtype=cp.float32,
             )
         else:
-            log_occupancy = cp.zeros((place_bin_centers.shape[0],), dtype=cp.float32)
-            log_occupancy[gpu_is_track_interior] = estimate_log_position_density(
+            occupancy = cp.zeros((place_bin_centers.shape[0],), dtype=cp.float32)
+            occupancy[gpu_is_track_interior] = estimate_position_density(
                 interior_place_bin_centers,
                 cp.asarray(position[not_nan_position], dtype=cp.float32),
                 position_std,
                 block_size=block_size,
             )
 
-        log_mean_rates = []
-        encoding_marks = []
-        encoding_positions = []
+        mean_rates = []
         summed_ground_process_intensity = cp.zeros(
             (place_bin_centers.shape[0],), dtype=cp.float32
         )
+        encoding_marks = []
+        encoding_positions = []
+
+        n_marks = multiunits.shape[1]
+        if isinstance(mark_std, (int, float)):
+            mark_std = np.asarray([mark_std] * n_marks)
+        else:
+            mark_std = np.asarray(mark_std)
 
         for multiunit in np.moveaxis(multiunits, -1, 0):
 
             # ground process intensity
             is_spike = np.any(~np.isnan(multiunit), axis=1)
-            log_mean_rates.append(np.log(is_spike.mean()))
+            mean_rates.append(is_spike.mean())
 
             if is_spike.sum() > 0:
                 if use_diffusion & (position.shape[1] > 1):
-                    log_marginal_density = cp.log(
-                        cp.asarray(
-                            estimate_diffusion_position_density(
-                                position[is_spike & not_nan_position],
-                                edges,
-                                bin_distances=bin_diffusion_distances,
-                            ),
-                            dtype=cp.float32,
-                        )
+                    marginal_density = cp.asarray(
+                        estimate_diffusion_position_density(
+                            position[is_spike & not_nan_position],
+                            edges,
+                            bin_distances=bin_diffusion_distances,
+                        ),
+                        dtype=cp.float32,
                     )
                 else:
-                    log_marginal_density = cp.zeros(
+                    marginal_density = cp.zeros(
                         (place_bin_centers.shape[0],), dtype=cp.float32
                     )
-                    log_marginal_density[
-                        gpu_is_track_interior
-                    ] = estimate_log_position_density(
+                    marginal_density[gpu_is_track_interior] = estimate_position_density(
                         interior_place_bin_centers,
                         cp.asarray(
                             position[is_spike & not_nan_position], dtype=cp.float32
                         ),
                         position_std,
                         block_size=block_size,
                     )
 
             summed_ground_process_intensity += estimate_intensity(
-                log_marginal_density, log_occupancy, log_mean_rates[-1]
+                marginal_density, occupancy, mean_rates[-1]
             )
 
             is_mark_features = np.any(~np.isnan(multiunit), axis=0)
             encoding_marks.append(
                 cp.asarray(
                     multiunit[np.ix_(is_spike & not_nan_position, is_mark_features)],
-                    dtype=cp.int16,
+                    dtype=cp.float32,
                 )
             )
             encoding_positions.append(position[is_spike & not_nan_position])
 
         summed_ground_process_intensity = cp.asnumpy(
             summed_ground_process_intensity
         ) + np.spacing(1)
 
         return {
             "encoding_marks": encoding_marks,
             "encoding_positions": encoding_positions,
             "summed_ground_process_intensity": summed_ground_process_intensity,
-            "log_occupancy": log_occupancy,
-            "log_mean_rates": log_mean_rates,
+            "occupancy": occupancy,
+            "mean_rates": mean_rates,
             "mark_std": mark_std,
             "position_std": position_std,
             "block_size": block_size,
             "bin_diffusion_distances": bin_diffusion_distances,
             "use_diffusion": use_diffusion,
             "edges": edges,
             **kwargs,
         }
 
-    def estimate_multiunit_likelihood_integer_gpu_log(
-        multiunits,
-        encoding_marks,
-        mark_std,
-        place_bin_centers,
-        encoding_positions,
-        position_std,
-        log_occupancy,
-        log_mean_rates,
-        summed_ground_process_intensity,
-        bin_diffusion_distances,
-        edges,
-        max_mark_diff=6000,
-        set_diag_zero=False,
-        is_track_interior=None,
-        time_bin_size=1,
-        block_size=100,
-        ignore_no_spike=False,
-        disable_progress_bar=False,
-        use_diffusion=False,
-    ):
+    def estimate_multiunit_likelihood_gpu(
+        multiunits: np.ndarray,
+        encoding_marks: cp.ndarray,
+        mark_std: np.ndarray,
+        place_bin_centers: np.ndarray,
+        encoding_positions: cp.ndarray,
+        position_std: np.ndarray,
+        occupancy: cp.ndarray,
+        mean_rates: cp.ndarray,
+        summed_ground_process_intensity: np.ndarray,
+        bin_diffusion_distances: np.ndarray,
+        edges: list[np.ndarray],
+        max_mark_diff: int = 6000,
+        set_diag_zero: bool = False,
+        is_track_interior: Optional[np.ndarray] = None,
+        time_bin_size: int = 1,
+        block_size: int = 100,
+        ignore_no_spike: bool = False,
+        disable_progress_bar: bool = False,
+        use_diffusion: bool = False,
+    ) -> np.ndarray:
         """Estimates the likelihood of position bins given multiunit marks.
 
         Parameters
         ----------
         multiunits : np.ndarray, shape (n_decoding_time, n_marks, n_electrodes)
         encoding_marks : cp.ndarray, shape (n_encoding_spikes, n_marks, n_electrodes)
-        mark_std : float
+        mark_std : list, shape (n_marks,)
             Amount of smoothing for mark features
         place_bin_centers : cp.ndarray, shape (n_bins, n_position_dims)
         encoding_positions : cp.ndarray, shape (n_encoding_spikes, n_position_dims)
         position_std : float or array_like, shape (n_position_dims,)
             Amount of smoothing for position
-        log_occupancy : cp.ndarray, (n_bins,)
-        log_mean_rates : list, len (n_electrodes,)
+        occupancy : cp.ndarray, (n_bins,)
+        mean_rates : list, len (n_electrodes,)
         summed_ground_process_intensity : np.ndarray, shape (n_bins,)
         bin_diffusion_distances : np.ndarray, shape (n_bins, n_bins)
         edges : list of np.ndarray
         max_mark_diff : int
             Maximum difference between mark features
         set_diag_zero : bool
             Remove influence of the same mark in encoding and decoding.
@@ -464,78 +433,76 @@
 
         multiunits = np.moveaxis(multiunits, -1, 0)
         n_position_bins = is_track_interior.sum()
         interior_place_bin_centers = cp.asarray(
             place_bin_centers[is_track_interior], dtype=cp.float32
         )
         gpu_is_track_interior = cp.asarray(is_track_interior)
-        interior_log_occupancy = log_occupancy[gpu_is_track_interior]
+        interior_occupancy = occupancy[gpu_is_track_interior]
 
-        for multiunit, enc_marks, enc_pos, log_mean_rate in zip(
+        for multiunit, enc_marks, enc_pos, mean_rate in zip(
             tqdm(multiunits, desc="n_electrodes", disable=disable_progress_bar),
             encoding_marks,
             encoding_positions,
-            log_mean_rates,
+            mean_rates,
         ):
             is_spike = np.any(~np.isnan(multiunit), axis=1)
             is_mark_features = np.any(~np.isnan(multiunit), axis=0)
             decoding_marks = cp.asarray(
-                multiunit[np.ix_(is_spike, is_mark_features)], dtype=cp.int16
+                multiunit[np.ix_(is_spike, is_mark_features)], dtype=cp.float32
             )
             n_decoding_marks = decoding_marks.shape[0]
             log_joint_mark_intensity = np.zeros(
                 (n_decoding_marks, n_position_bins), dtype=np.float32
             )
 
             if block_size is None:
                 block_size = n_decoding_marks
 
             if use_diffusion & (place_bin_centers.shape[1] > 1):
-                log_position_distances = cp.log(
-                    cp.asarray(
-                        estimate_diffusion_position_distance(
-                            enc_pos,
-                            edges,
-                            bin_distances=bin_diffusion_distances,
-                        )[:, is_track_interior],
-                        dtype=cp.float32,
-                    )
+                position_distance = cp.asarray(
+                    estimate_diffusion_position_distance(
+                        enc_pos,
+                        edges,
+                        bin_distances=bin_diffusion_distances,
+                    )[:, is_track_interior],
+                    dtype=cp.float32,
                 )
             else:
-                log_position_distances = estimate_log_position_distance(
+                position_distance = estimate_position_distance(
                     interior_place_bin_centers,
                     cp.asarray(enc_pos, dtype=cp.float32),
                     position_std,
                 ).astype(cp.float32)
 
             for start_ind in range(0, n_decoding_marks, block_size):
                 block_inds = slice(start_ind, start_ind + block_size)
                 log_joint_mark_intensity[
                     block_inds
                 ] = estimate_log_joint_mark_intensity(
                     decoding_marks[block_inds],
                     enc_marks,
-                    mark_std,
-                    log_position_distances,
-                    interior_log_occupancy,
-                    log_mean_rate,
+                    mark_std[is_mark_features],
+                    interior_occupancy,
+                    mean_rate,
                     max_mark_diff=max_mark_diff,
                     set_diag_zero=set_diag_zero,
+                    position_distance=position_distance,
                 )
             log_likelihood[np.ix_(is_spike, is_track_interior)] += np.nan_to_num(
                 log_joint_mark_intensity
             )
 
             mempool = cp.get_default_memory_pool()
             mempool.free_all_blocks()
 
         log_likelihood[:, ~is_track_interior] = np.nan
 
         return log_likelihood
 
 except ImportError:
 
-    def estimate_multiunit_likelihood_integer_gpu_log(*args, **kwargs):
+    def estimate_multiunit_likelihood_gpu(*args, **kwargs):
         print("Cupy is not installed or no GPU detected...")
 
-    def fit_multiunit_likelihood_integer_gpu_log(*args, **kwargs):
+    def fit_multiunit_likelihood_gpu(*args, **kwargs):
         print("Cupy is not installed or no GPU detected...")
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/multiunit_likelihood_track_graph.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/multiunit_likelihood_track_graph.py`

 * *Files identical despite different names*

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/spiking_likelihood_glm.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/spiking_likelihood_glm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """Estimates a Poisson likelihood using place fields estimated with a GLM
 with a spline basis"""
 import logging
+from typing import Optional, Union
 
 import dask
 import numpy as np
 import pandas as pd
 import scipy.stats
 import xarray as xr
 from dask.distributed import Client, get_client
-from patsy import build_design_matrices, dmatrix
+from patsy import DesignInfo, DesignMatrix, build_design_matrices, dmatrix
 from regularized_glm import penalized_IRLS
-from replay_trajectory_classification.environments import get_n_bins
 from statsmodels.api import families
 
+from replay_trajectory_classification.environments import get_n_bins
+
 
-def make_spline_design_matrix(position, place_bin_edges, knot_spacing=10):
+def make_spline_design_matrix(
+    position: np.ndarray, place_bin_edges: np.ndarray, knot_spacing: float = 10.0
+) -> DesignMatrix:
     """Creates a design matrix for regression with a position spline basis.
 
     Parameters
     ----------
     position : np.ndarray, shape (n_time, n_position_dims)
     place_bin_edges : np.ndarray, shape (n_bins, n_position_dims)
 
     Returns
     -------
-    design_matrix : statsmodels.DesignMatrix
+    design_matrix : patsy.DesignMatrix
 
     """
     inner_knots = []
     for pos, edges in zip(position.T, place_bin_edges.T):
         n_points = get_n_bins(edges, bin_size=knot_spacing)
         knots = np.linspace(edges.min(), edges.max(), n_points)[1:-1]
         knots = knots[(knots > pos.min()) & (knots < pos.max())]
@@ -45,35 +49,44 @@
         data[f"x{ind}"] = position[:, ind]
 
     formula += 'constraints="center")'
 
     return dmatrix(formula, data)
 
 
-def make_spline_predict_matrix(design_info, place_bin_centers):
+def make_spline_predict_matrix(
+    design_info: DesignInfo, place_bin_centers: np.ndarray
+) -> DesignMatrix:
     """Make a design matrix for position bins"""
     predict_data = {}
     for ind in range(place_bin_centers.shape[1]):
         predict_data[f"x{ind}"] = place_bin_centers[:, ind]
     return build_design_matrices([design_info], predict_data)[0]
 
 
-def get_firing_rate(design_matrix, results, sampling_frequency=1):
+def get_firing_rate(
+    design_matrix: DesignMatrix, results: tuple, sampling_frequency: int = 1
+):
     """Predicts the firing rate given fitted model coefficents."""
     if np.any(np.isnan(results.coefficients)):
         n_time = design_matrix.shape[0]
         rate = np.zeros((n_time,))
     else:
         rate = np.exp(design_matrix @ results.coefficients) * sampling_frequency
 
     return rate
 
 
 @dask.delayed
-def fit_glm(response, design_matrix, penalty=None, tolerance=1e-5):
+def fit_glm(
+    response: np.ndarray,
+    design_matrix: np.ndarray,
+    penalty: Optional[float] = None,
+    tolerance: float = 1e-5,
+) -> tuple:
     """Fits a L2-penalized GLM.
 
     Parameters
     ----------
     response : np.ndarray, shape (n_time,)
         Calcium activity trace
     design_matrix : np.ndarray, shape (n_time, n_coefficients)
@@ -98,37 +111,41 @@
         response.squeeze(),
         family=families.Poisson(),
         penalty=penalty,
         tolerance=tolerance,
     )
 
 
-def poisson_log_likelihood(spikes, conditional_intensity):
+def poisson_log_likelihood(
+    spikes: np.ndarray, conditional_intensity: np.ndarray
+) -> np.ndarray:
     """Probability of parameters given spiking at a particular time.
 
     Parameters
     ----------
     spikes : np.ndarray, shape (n_time,)
         Indicator of spike or no spike at current time.
     conditional_intensity : np.ndarray, shape (n_place_bins,)
         Instantaneous probability of observing a spike
 
     Returns
     -------
-    poisson_log_likelihood : array_like, shape (n_time, n_place_bins)
+    poisson_log_likelihood : np.ndarray, shape (n_time, n_place_bins)
 
     """
     # Logarithm of the absolute value of the gamma function is always 0 when
     # spikes are 0 or 1
     return scipy.stats.poisson.logpmf(
         spikes[:, np.newaxis], conditional_intensity[np.newaxis, :] + np.spacing(1)
     )
 
 
-def combined_likelihood(spikes, conditional_intensity):
+def combined_likelihood(
+    spikes: np.ndarray, conditional_intensity: np.ndarray
+) -> np.ndarray:
     """Combines the likelihoods of all the cells.
 
     Parameters
     ----------
     spikes : np.ndarray, shape (n_time, n_neurons)
     conditional_intensity : np.ndarray, shape (n_bins, n_neurons)
 
@@ -139,26 +156,31 @@
 
     for is_spike, ci in zip(spikes.T, conditional_intensity.T):
         log_likelihood += poisson_log_likelihood(is_spike, ci)
 
     return log_likelihood
 
 
-def estimate_spiking_likelihood(spikes, conditional_intensity, is_track_interior=None):
+def estimate_spiking_likelihood(
+    spikes: np.ndarray,
+    conditional_intensity: np.ndarray,
+    is_track_interior: Optional[np.ndarray] = None,
+) -> np.ndarray:
     """
 
     Parameters
     ----------
     spikes : np.ndarray, shape (n_time, n_neurons)
     conditional_intensity : np.ndarray, shape (n_bins, n_neurons)
     is_track_interior : None or np.ndarray, optional, shape (n_x_position_bins,
                                                              n_y_position_bins)
     Returns
     -------
     likelihood : np.ndarray, shape (n_time, n_bins)
+
     """
     if is_track_interior is not None:
         is_track_interior = is_track_interior.ravel(order="F")
     else:
         n_bins = conditional_intensity.shape[0]
         is_track_interior = np.ones((n_bins,), dtype=np.bool)
 
@@ -167,24 +189,24 @@
     mask = np.ones_like(is_track_interior, dtype=np.float)
     mask[~is_track_interior] = np.nan
 
     return log_likelihood * mask
 
 
 def estimate_place_fields(
-    position,
-    spikes,
-    place_bin_centers,
-    place_bin_edges,
-    edges=None,
-    is_track_boundary=None,
-    is_track_interior=None,
-    penalty=1e-1,
-    knot_spacing=10,
-):
+    position: np.ndarray,
+    spikes: np.ndarray,
+    place_bin_centers: np.ndarray,
+    place_bin_edges: np.ndarray,
+    edges: Optional[np.ndarray] = None,
+    is_track_boundary: Optional[np.ndarray] = None,
+    is_track_interior: Optional[np.ndarray] = None,
+    penalty: float = 1e-1,
+    knot_spacing: int = 10,
+) -> xr.DataArray:
     """Gives the conditional intensity of the neurons' spiking with respect to
     position.
 
     Parameters
     ----------
     position : np.ndarray, shape (n_time, n_position_dims)
     spikes : np.ndarray, shape (n_time, n_neurons)
@@ -195,15 +217,15 @@
     penalty : None or float, optional
         L2 penalty on regression. If None, penalty is smallest possible.
     knot_spacing : int, optional
         Spacing of position knots. Controls how smooth the firing rate is.
 
     Returns
     -------
-    conditional_intensity : np.ndarray, shape (n_bins, n_neurons)
+    conditional_intensity : xr.DataArray, shape (n_bins, n_neurons)
 
     """
     if np.any(np.ptp(place_bin_edges, axis=0) <= knot_spacing):
         logging.warning("Range of position is smaller than knot spacing.")
     design_matrix = make_spline_design_matrix(position, place_bin_edges, knot_spacing)
     design_info = design_matrix.design_info
     try:
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/spiking_likelihood_kde.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/spiking_likelihood_kde.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-"""Estimates a Poisson likelihood using place fields estimated with a KDE"""
+"""Estimates a Poisson likelihood using place fields estimated with a kernel density estimate."""
+
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
+from tqdm.auto import tqdm
+
 from replay_trajectory_classification.core import atleast_2d
 from replay_trajectory_classification.likelihoods.diffusion import (
     diffuse_each_bin,
     estimate_diffusion_position_density,
 )
-from tqdm.auto import tqdm
 
 
-def gaussian_pdf(x, mean, sigma):
+def gaussian_pdf(x: np.ndarray, mean: np.ndarray, sigma: np.ndarray) -> np.ndarray:
     """Compute the value of a Gaussian probability density function at x with
     given mean and sigma."""
     return np.exp(-0.5 * ((x - mean) / sigma) ** 2) / (sigma * np.sqrt(2.0 * np.pi))
 
 
-def estimate_position_distance(place_bin_centers, positions, position_std):
+def estimate_position_distance(
+    place_bin_centers: np.ndarray, positions: np.ndarray, position_std: np.ndarray
+) -> np.ndarray:
     """Estimates the Euclidean distance between positions and position bins.
 
     Parameters
     ----------
     place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
     positions : np.ndarray, shape (n_time, n_position_dims)
     position_std : array_like, shape (n_position_dims,)
@@ -46,24 +51,28 @@
             std,
         )
 
     return position_distance
 
 
 def estimate_position_density(
-    place_bin_centers, positions, position_std, block_size=100
-):
+    place_bin_centers: np.ndarray,
+    positions: np.ndarray,
+    position_std: Union[float, np.ndarray],
+    block_size: int = 100,
+) -> np.ndarray:
     """Estimates a kernel density estimate over position bins using
     Euclidean distances.
 
     Parameters
     ----------
     place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
     positions : np.ndarray, shape (n_time, n_position_dims)
     position_std : float or array_like, shape (n_position_dims,)
+    block_size : int
 
     Returns
     -------
     position_density : np.ndarray, shape (n_position_bins,)
 
     """
     n_time = positions.shape[0]
@@ -81,23 +90,23 @@
             ),
             axis=0,
         )
     return position_density
 
 
 def get_firing_rate(
-    is_spike,
-    position,
-    place_bin_centers,
-    is_track_interior,
-    not_nan_position,
-    occupancy,
-    position_std,
-    block_size=None,
-):
+    is_spike: np.ndarray,
+    position: np.ndarray,
+    place_bin_centers: np.ndarray,
+    is_track_interior: np.ndarray,
+    not_nan_position: np.ndarray,
+    occupancy: np.ndarray,
+    position_std: np.ndarray,
+    block_size: Optional[int] = None,
+) -> np.ndarray:
     if is_spike.sum() > 0:
         mean_rate = is_spike.mean()
         marginal_density = np.zeros((place_bin_centers.shape[0],), dtype=np.float32)
 
         marginal_density[is_track_interior] = estimate_position_density(
             place_bin_centers[is_track_interior],
             np.asarray(position[is_spike & not_nan_position], dtype=np.float32),
@@ -106,46 +115,46 @@
         )
         return np.exp(np.log(mean_rate) + np.log(marginal_density) - np.log(occupancy))
     else:
         return np.zeros_like(occupancy)
 
 
 def get_diffusion_firing_rate(
-    is_spike,
-    position,
-    edges,
-    bin_diffusion_distances,
-    occupancy,
-    not_nan_position,
-):
+    is_spike: np.ndarray,
+    position: np.ndarray,
+    edges: list[np.ndarray],
+    bin_diffusion_distances: np.ndarray,
+    occupancy: np.ndarray,
+    not_nan_position: np.ndarray,
+) -> np.ndarray:
     if is_spike.sum() > 0:
         mean_rate = is_spike.mean()
         marginal_density = estimate_diffusion_position_density(
             position[is_spike & not_nan_position],
             edges,
             bin_distances=bin_diffusion_distances,
         ).astype(np.float32)
 
         return np.exp(np.log(mean_rate) + np.log(marginal_density) - np.log(occupancy))
     else:
         return np.zeros_like(occupancy)
 
 
 def estimate_place_fields_kde(
-    position,
-    spikes,
-    place_bin_centers,
-    position_std,
-    is_track_boundary=None,
-    is_track_interior=None,
-    edges=None,
-    place_bin_edges=None,
-    use_diffusion=False,
-    block_size=None,
-):
+    position: np.ndarray,
+    spikes: np.ndarray,
+    place_bin_centers: np.ndarray,
+    position_std: np.ndarray,
+    is_track_boundary: Optional[np.ndarray] = None,
+    is_track_interior: Optional[np.ndarray] = None,
+    edges: Optional[list[np.ndarray]] = None,
+    place_bin_edges: Optional[np.ndarray] = None,
+    use_diffusion: bool = False,
+    block_size: Optional[int] = None,
+) -> xr.DataArray:
     """Gives the conditional intensity of the neurons' spiking with respect to
     position.
 
     Parameters
     ----------
     position : np.ndarray, shape (n_time, n_position_dims)
     spikes : np.ndarray, shape (n_time,)
@@ -237,15 +246,17 @@
                 place_bin_centers.T.tolist(), names=names
             )
         }
 
     return xr.DataArray(data=place_fields, coords=coords, dims=DIMS)
 
 
-def poisson_log_likelihood(spikes, conditional_intensity):
+def poisson_log_likelihood(
+    spikes: np.ndarray, conditional_intensity: np.ndarray
+) -> np.ndarray:
     """Probability of parameters given spiking at a particular time.
 
     Parameters
     ----------
     spikes : np.ndarray, shape (n_time,)
         Indicator of spike or no spike at current time.
     conditional_intensity : np.ndarray, shape (n_place_bins,)
@@ -259,15 +270,17 @@
     return (
         np.log(conditional_intensity[np.newaxis, :] + np.spacing(1))
         * spikes[:, np.newaxis]
         - conditional_intensity[np.newaxis, :]
     )
 
 
-def combined_likelihood(spikes, conditional_intensity):
+def combined_likelihood(
+    spikes: np.ndarray, conditional_intensity: np.ndarray
+) -> np.ndarray:
     """
 
     Parameters
     ----------
     spikes : np.ndarray, shape (n_time, n_neurons)
     conditional_intensity : np.ndarray, shape (n_bins, n_neurons)
 
@@ -279,27 +292,30 @@
     for is_spike, ci in zip(tqdm(spikes.T), conditional_intensity.T):
         log_likelihood += poisson_log_likelihood(is_spike, ci)
 
     return log_likelihood
 
 
 def estimate_spiking_likelihood_kde(
-    spikes, conditional_intensity, is_track_interior=None
-):
+    spikes: np.ndarray,
+    conditional_intensity: np.ndarray,
+    is_track_interior: Optional[np.ndarray] = None,
+) -> np.ndarray:
     """
 
     Parameters
     ----------
     spikes : np.ndarray, shape (n_time, n_neurons)
     conditional_intensity : np.ndarray, shape (n_bins, n_neurons)
     is_track_interior : None or np.ndarray, optional, shape (n_x_position_bins,
                                                              n_y_position_bins)
     Returns
     -------
     likelihood : np.ndarray, shape (n_time, n_bins)
+
     """
     spikes = np.asarray(spikes, dtype=np.float32)
 
     if is_track_interior is not None:
         is_track_interior = is_track_interior.ravel(order="F")
     else:
         n_bins = conditional_intensity.shape[0]
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/likelihoods/spiking_likelihood_kde_gpu.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/likelihoods/spiking_likelihood_kde_gpu.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 """Estimates a Poisson likelihood using place fields estimated with a KDE
 using GPUs"""
+from typing import Optional, Union
+
 import numpy as np
 import pandas as pd
 import xarray as xr
+from tqdm.auto import tqdm
+
 from replay_trajectory_classification.core import atleast_2d
 from replay_trajectory_classification.likelihoods.diffusion import (
     diffuse_each_bin,
     estimate_diffusion_position_density,
 )
-from tqdm.auto import tqdm
 
 try:
     import cupy as cp
 
-    def gaussian_pdf(x, mean, sigma):
+    def gaussian_pdf(x: np.ndarray, mean: np.ndarray, sigma: np.ndarray) -> np.ndarray:
         """Compute the value of a Gaussian probability density function at x with
         given mean and sigma."""
         return np.exp(-0.5 * ((x - mean) / sigma) ** 2) / (sigma * np.sqrt(2.0 * np.pi))
 
-    def estimate_position_distance(place_bin_centers, positions, position_std):
+    def estimate_position_distance(
+        place_bin_centers: np.ndarray, positions: np.ndarray, position_std: np.ndarray
+    ) -> np.ndarray:
         """Estimates the Euclidean distance between positions and position bins.
 
         Parameters
         ----------
         place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
         positions : np.ndarray, shape (n_time, n_position_dims)
-        position_std : array_like, shape (n_position_dims,)
+        position_std : np.ndarray, shape (n_position_dims,)
 
         Returns
         -------
         position_distance : np.ndarray, shape (n_time, n_position_bins)
 
         """
         n_time, n_position_dims = positions.shape
@@ -46,16 +51,19 @@
                 np.expand_dims(positions[:, position_ind], axis=1),
                 std,
             )
 
         return position_distance
 
     def estimate_position_density(
-        place_bin_centers, positions, position_std, block_size=100
-    ):
+        place_bin_centers: np.ndarray,
+        positions: np.ndarray,
+        position_std: Union[float, np.ndarray],
+        block_size: int = 100,
+    ) -> np.ndarray:
         """Estimates a kernel density estimate over position bins using
         Euclidean distances.
 
         Parameters
         ----------
         place_bin_centers : np.ndarray, shape (n_position_bins, n_position_dims)
         positions : np.ndarray, shape (n_time, n_position_dims)
@@ -80,23 +88,23 @@
                     place_bin_centers[block_inds], positions, position_std
                 ),
                 axis=0,
             )
         return position_density
 
     def get_firing_rate(
-        is_spike,
-        position,
-        place_bin_centers,
-        is_track_interior,
-        not_nan_position,
-        occupancy,
-        position_std,
-        block_size=None,
-    ):
+        is_spike: np.ndarray,
+        position: np.ndarray,
+        place_bin_centers: np.ndarray,
+        is_track_interior: np.ndarray,
+        not_nan_position: np.ndarray,
+        occupancy: np.ndarray,
+        position_std: np.ndarray,
+        block_size: Optional[int] = None,
+    ) -> np.ndarray:
         if is_spike.sum() > 0:
             mean_rate = is_spike.mean()
             marginal_density = np.zeros((place_bin_centers.shape[0],), dtype=np.float32)
 
             marginal_density[is_track_interior] = estimate_position_density(
                 place_bin_centers[is_track_interior],
                 np.asarray(position[is_spike & not_nan_position], dtype=np.float32),
@@ -106,21 +114,21 @@
             return np.exp(
                 np.log(mean_rate) + np.log(marginal_density) - np.log(occupancy)
             )
         else:
             return np.zeros_like(occupancy)
 
     def get_diffusion_firing_rate(
-        is_spike,
-        position,
-        edges,
-        bin_diffusion_distances,
-        occupancy,
-        not_nan_position,
-    ):
+        is_spike: np.ndarray,
+        position: np.ndarray,
+        edges: list[np.ndarray],
+        bin_diffusion_distances: np.ndarray,
+        occupancy: np.ndarray,
+        not_nan_position: np.ndarray,
+    ) -> np.ndarray:
         if is_spike.sum() > 0:
             mean_rate = is_spike.mean()
             marginal_density = estimate_diffusion_position_density(
                 position[is_spike & not_nan_position],
                 edges,
                 bin_distances=bin_diffusion_distances,
             ).astype(np.float32)
@@ -128,25 +136,25 @@
             return np.exp(
                 np.log(mean_rate) + np.log(marginal_density) - np.log(occupancy)
             )
         else:
             return np.zeros_like(occupancy)
 
     def estimate_place_fields_kde_gpu(
-        position,
-        spikes,
-        place_bin_centers,
-        position_std,
-        is_track_boundary=None,
-        is_track_interior=None,
-        edges=None,
-        place_bin_edges=None,
-        use_diffusion=False,
-        block_size=None,
-    ):
+        position: np.ndarray,
+        spikes: np.ndarray,
+        place_bin_centers: np.ndarray,
+        position_std: Union[float, np.ndarray],
+        is_track_boundary: Optional[np.ndarray] = None,
+        is_track_interior: Optional[np.ndarray] = None,
+        edges: Optional[list[np.ndarray]] = None,
+        place_bin_edges: Optional[np.ndarray] = None,
+        use_diffusion: bool = False,
+        block_size: Optional[int] = None,
+    ) -> xr.DataArray:
         """Gives the conditional intensity of the neurons' spiking with respect to
         position.
 
         Parameters
         ----------
         position : np.ndarray, shape (n_time, n_position_dims)
         spikes : np.ndarray, shape (n_time,)
@@ -161,15 +169,15 @@
         use_diffusion : bool
             Respect track geometry by using diffusion distances
         block_size : int
             Size of data to process in chunks
 
         Returns
         -------
-        conditional_intensity : np.ndarray, shape (n_bins, n_neurons)
+        conditional_intensity : xr.DataArray, shape (n_bins, n_neurons)
 
         """
 
         position = atleast_2d(position).astype(np.float32)
         place_bin_centers = atleast_2d(place_bin_centers).astype(np.float32)
         not_nan_position = np.all(~np.isnan(position), axis=1)
         spikes = np.asarray(spikes, dtype=bool)
@@ -238,74 +246,82 @@
                 "position": pd.MultiIndex.from_arrays(
                     place_bin_centers.T.tolist(), names=names
                 )
             }
 
         return xr.DataArray(data=place_fields, coords=coords, dims=DIMS)
 
-    def poisson_log_likelihood(spikes, conditional_intensity):
+    def poisson_log_likelihood(
+        spikes: cp.ndarray, conditional_intensity: cp.ndarray
+    ) -> cp.ndarray:
         """Probability of parameters given spiking at a particular time.
 
         Parameters
         ----------
-        spikes : np.ndarray, shape (n_time,)
+        spikes : cp.ndarray, shape (n_time,)
             Indicator of spike or no spike at current time.
-        conditional_intensity : np.ndarray, shape (n_place_bins,)
+        conditional_intensity : cp.ndarray, shape (n_place_bins,)
             Instantaneous probability of observing a spike
 
         Returns
         -------
-        poisson_log_likelihood : array_like, shape (n_time, n_place_bins)
+        poisson_log_likelihood : cp.ndarray, shape (n_time, n_place_bins)
 
         """
         # Logarithm of the absolute value of the gamma function is always 0 when
         # spikes are 0 or 1
         return (
             cp.log(conditional_intensity[cp.newaxis, :] + np.spacing(1))
             * spikes[:, np.newaxis]
             - conditional_intensity[cp.newaxis, :]
         )
 
-    def combined_likelihood(spikes, conditional_intensity):
+    def combined_likelihood(
+        spikes: np.ndarray, conditional_intensity: np.ndarray
+    ) -> np.ndarray:
         """
 
         Parameters
         ----------
         spikes : np.ndarray, shape (n_time, n_neurons)
         conditional_intensity : np.ndarray, shape (n_bins, n_neurons)
 
         """
         n_time = spikes.shape[0]
         n_bins = conditional_intensity.shape[0]
-        log_likelihood = cp.zeros((n_time, n_bins))
+        log_likelihood = cp.zeros((n_time, n_bins), dtype=cp.float32)
 
         mempool = cp.get_default_memory_pool()
 
         for is_spike, ci in zip(
-            tqdm(cp.asarray(spikes).T), cp.asarray(conditional_intensity).T
+            tqdm(cp.asarray(spikes, dtype=cp.float32).T),
+            cp.asarray(conditional_intensity, dtype=cp.float32).T,
         ):
             log_likelihood += poisson_log_likelihood(is_spike, ci)
             mempool.free_all_blocks()
 
         return cp.asnumpy(log_likelihood)
 
     def estimate_spiking_likelihood_kde_gpu(
-        spikes, conditional_intensity, is_track_interior=None
-    ):
+        spikes: np.ndarray,
+        conditional_intensity: np.ndarray,
+        is_track_interior: Optional[np.ndarray] = None,
+    ) -> np.ndarray:
         """
 
         Parameters
         ----------
         spikes : np.ndarray, shape (n_time, n_neurons)
         conditional_intensity : np.ndarray, shape (n_bins, n_neurons)
         is_track_interior : None or np.ndarray, optional, shape (n_x_position_bins,
                                                                  n_y_position_bins)
         Returns
         -------
         likelihood : np.ndarray, shape (n_time, n_bins)
+
         """
         spikes = np.asarray(spikes, dtype=np.float32)
 
         if is_track_interior is not None:
             is_track_interior = is_track_interior.ravel(order="F")
         else:
             n_bins = conditional_intensity.shape[0]
```

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification/standard_decoder.py` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification/standard_decoder.py`

 * *Files identical despite different names*

### Comparing `replay_trajectory_classification-1.3.8/replay_trajectory_classification.egg-info/SOURCES.txt` & `replay_trajectory_classification-1.3.9/replay_trajectory_classification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `replay_trajectory_classification-1.3.8/setup.py` & `replay_trajectory_classification-1.3.9/setup.py`

 * *Files identical despite different names*

