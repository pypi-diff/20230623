# Comparing `tmp/openrlbenchmark-0.2.1a3.tar.gz` & `tmp/openrlbenchmark-0.2.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrlbenchmark-0.2.1a3.tar", max compression
+gzip compressed data, was "openrlbenchmark-0.2.1a4.tar", max compression
```

## Comparing `openrlbenchmark-0.2.1a3.tar` & `openrlbenchmark-0.2.1a4.tar`

### file list

```diff
@@ -1,16 +1,12 @@
--rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.2.1a3/LICENSE
--rw-r--r--   0        0        0    20353 2023-06-07 20:05:43.595075 openrlbenchmark-0.2.1a3/README.md
--rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.2.1a3/openrlbenchmark/__init__.py
--rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340069 openrlbenchmark-0.2.1a3/openrlbenchmark/cache.py
--rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340155 openrlbenchmark-0.2.1a3/openrlbenchmark/cache_legacy.py
--rw-r--r--   0        0        0     6147 2023-06-07 19:47:32.024056 openrlbenchmark-0.2.1a3/openrlbenchmark/capped_hns.py
--rw-r--r--   0        0        0     6050 2023-04-04 00:37:30.606222 openrlbenchmark-0.2.1a3/openrlbenchmark/hns.py
--rw-r--r--   0        0        0     2178 2023-05-23 20:34:08.340377 openrlbenchmark-0.2.1a3/openrlbenchmark/offline_db.py
--rw-r--r--   0        0        0    37404 2023-06-16 13:19:06.422225 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops.py
--rw-r--r--   0        0        0    30367 2023-06-07 20:11:32.994334 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_hns.py
--rw-r--r--   0        0        0    24994 2023-06-16 13:11:33.831627 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_multi_metrics.py
--rw-r--r--   0        0        0    25030 2023-06-12 14:59:30.792810 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_multi_metrics_oai.py
--rw-r--r--   0        0        0    36919 2023-06-07 20:07:01.541242 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_trl.py
--rw-r--r--   0        0        0    25177 2023-06-07 20:11:32.986812 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_trl_multi_metrics.py
--rw-r--r--   0        0        0      748 2023-06-16 13:19:35.534932 openrlbenchmark-0.2.1a3/pyproject.toml
--rw-r--r--   0        0        0    21316 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-17 17:13:06.153628 openrlbenchmark-0.2.1a4/LICENSE
+-rw-r--r--   0        0        0    20292 2023-06-17 17:13:06.158964 openrlbenchmark-0.2.1a4/README.md
+-rw-r--r--   0        0        0       75 2023-06-17 17:13:06.159222 openrlbenchmark-0.2.1a4/openrlbenchmark/__init__.py
+-rw-r--r--   0        0        0     1746 2023-06-17 17:13:06.159306 openrlbenchmark-0.2.1a4/openrlbenchmark/cache.py
+-rw-r--r--   0        0        0     1746 2023-06-17 17:13:06.159383 openrlbenchmark-0.2.1a4/openrlbenchmark/cache_legacy.py
+-rw-r--r--   0        0        0     4955 2023-06-17 17:13:06.159494 openrlbenchmark-0.2.1a4/openrlbenchmark/hns.py
+-rw-r--r--   0        0        0     2178 2023-06-17 17:13:06.159579 openrlbenchmark-0.2.1a4/openrlbenchmark/offline_db.py
+-rw-r--r--   0        0        0    38510 2023-06-23 18:34:32.020807 openrlbenchmark-0.2.1a4/openrlbenchmark/rlops.py
+-rw-r--r--   0        0        0    30367 2023-06-17 17:13:06.159933 openrlbenchmark-0.2.1a4/openrlbenchmark/rlops_hns.py
+-rw-r--r--   0        0        0    26652 2023-06-23 18:34:32.020521 openrlbenchmark-0.2.1a4/openrlbenchmark/rlops_multi_metrics.py
+-rw-r--r--   0        0        0      748 2023-06-23 18:38:06.899376 openrlbenchmark-0.2.1a4/pyproject.toml
+-rw-r--r--   0        0        0    21255 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.1a4/PKG-INFO
```

### Comparing `openrlbenchmark-0.2.1a3/LICENSE` & `openrlbenchmark-0.2.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a3/README.md` & `openrlbenchmark-0.2.1a4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 * `cen`: the custom key for the experiment name
 * `metric`: the metric we are interested in
 
 So we are fetching metrics from [https://wandb.ai/openrlbenchmark/baselines](https://wandb.ai/openrlbenchmark/baselines). The environment id is stored in the `env` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`.
 
 Similarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `baselines-ppo2-mlp?cl=openai/baselines PPO2`.
 
-The labels of the figure can be customized with the `--pc.xlabel` and `--pc.ylabel` flags. The `--pc.ncols` flag specifies the number of columns in the figure. The `--pc.ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure
+The labels of the figure can be customized with the `--pc.xlabel` and `--pc.ylabel` flags. You can also specify the maximum number of timesteps to plot with `--pc.max_steps`. The `--pc.ncols` flag specifies the number of columns in the figure. The `--pc.ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure
 
 The `--rliable` toggles our [rliable](https://github.com/google-research/rliable) integration, and its configuration can be tweeked via `--rc`. The command above generates the following plot:
 
 ![](static/baseline_vs_cleanrl.png)
 ![](static/baseline_vs_cleanrl-time.png)
 ![](static/baseline_vs_cleanrl_sample_walltime_efficiency.png)
 ![](static/baseline_vs_cleanrl_sample_efficiency.png)
@@ -291,34 +291,36 @@
     --output-filename static/td3_vs_cleanrl \
     --scan-history
 ```
 ![](static/td3_vs_cleanrl.png)
 
 
 
-### Compare MORL Baselines algorithms on deterministic environments
+### Compare MORL Baselines algorithms
+Notice the number of timesteps is adjusted using `--pc.max_steps 400000`.
 
 ```shell
 python -m openrlbenchmark.rlops_multi_metrics \
-  --filters '?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metrics=eval/hypervolume&metrics=eval/igd&metrics=eval/sparsity&metrics=eval/eum&metrics=eval/mul' \
-  'Pareto Q-Learning?cl=Pareto Q-Learning' \
-  'MultiPolicy MO Q-Learning?cl=MultiPolicy MO Q-Learning' \
-  'MultiPolicy MO Q-Learning (OLS)?cl=MultiPolicy MO Q-Learning (OLS)' \
-  'MultiPolicy MO Q-Learning (GPI-LS)?cl=MultiPolicy MO Q-Learning (GPI-LS)' \
-  --env-ids deep-sea-treasure-v0 deep-sea-treasure-concave-v0 fruit-tree-v0 \
-  --pc.ncols 3 \
+  --filters '?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metrics=eval/hypervolume&metrics=eval/sparsity&metrics=eval/eum' \
+  'PGMORL?cl=PGMORL' \
+  'CAPQL?cl=CAPQL' \
+  'GPI-LS Continuous Action?cl=GPI-LS' \
+  'GPI-PD Continuous Action?cl=GPI-PD' \
+  --env-ids mo-halfcheetah-v4 mo-hopper-2d-v4  \
+  --pc.ncols 2 \
   --pc.ncols-legend 4 \
   --pc.xlabel 'Training steps' \
   --pc.ylabel '' \
-  --output-filename morl_deterministic_envs/ \
+  --pc.max_steps 400000 \
+  --output-filename morl/morl_continuous \
   --scan-history
 ```
 
-![](static/morl_deterministic_envs.png)
-![](static/morl_deterministic_envs-time.png)
+![](static/morl_continuous.png)
+![](static/morl_continuous-time.png)
 
 ### Calculate human normalized scores
 
 ```shell
 python -m openrlbenchmark.hns --files static/cleanrl_vs_baselines.csv static/machado_10M.csv static/machado_50M.csv 
 ```
```

### Comparing `openrlbenchmark-0.2.1a3/openrlbenchmark/cache.py` & `openrlbenchmark-0.2.1a4/openrlbenchmark/cache.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a3/openrlbenchmark/cache_legacy.py` & `openrlbenchmark-0.2.1a4/openrlbenchmark/cache_legacy.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a3/openrlbenchmark/capped_hns.py` & `openrlbenchmark-0.2.1a4/openrlbenchmark/hns.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 
 
 def parse_args():
     # fmt: off
     parser = argparse.ArgumentParser()
     parser.add_argument("--files", nargs="+", default=[],
         help="the csv files to calculate the median human normalized scores")
-    parser.add_argument("--percentiles", nargs="+", default=[], type=float,
-        help="the displayed percentile range of the median human normalized scores (e.g., 0.45 0.55)")
     # fmt: on
     return parser.parse_args()
 
 
 atari_human_normalized_scores = {
     "Alien-v5": (227.8, 7127.7),
     "Amidar-v5": (5.8, 1719.5),
@@ -106,35 +104,18 @@
         # env_ids = atari_human_normalized_scores.keys()
         env_ids = df.index
         for runset_name in df.columns:
             if runset_name in runset_names:
                 continue
             runset_names.add(runset_name)
             hnss = []
-            hnss_std = []
             for env_id in env_ids:
                 # if env_id not in df.index:
                 #     continue
                 episodic_return = float(df.loc[env_id, runset_name].split(" ± ")[0])
-                episodic_return_std = float(df.loc[env_id, runset_name].split(" ± ")[1])
                 hns = (episodic_return - atari_human_normalized_scores[env_id][0]) / (
                     atari_human_normalized_scores[env_id][1] - atari_human_normalized_scores[env_id][0]
                 )
-                capped_hns =  max(min(hns, 1), 0)
-                hnss += [capped_hns]
-                hns_std = (episodic_return_std - atari_human_normalized_scores[env_id][0]) / (
-                    atari_human_normalized_scores[env_id][1] - atari_human_normalized_scores[env_id][0]
-                )
-                hnss_std += [hns_std]
+                hnss += [hns]
             print(f"{runset_name}")
-            # print(hnss)
-            print(f"┣━━ median capped hns: {np.median(hnss)}")
-            if len(args.percentiles) > 0:
-
-                start_idx = int(len(hnss) * args.percentiles[0])
-                end_idx = int(len(hnss) * args.percentiles[1])
-                hnss, hnss_std, env_ids = zip(*sorted(zip(hnss, hnss_std, env_ids)))
-                print(f"┣━━━━━ median environments between {args.percentiles[0]} and {args.percentiles[1]} percentile")
-                for idx in range(start_idx, end_idx):
-                    print(f"┣━━━━━━━ {env_ids[idx]}: {hnss[idx]} ± {hnss_std[idx]}")
-
-            print(f"┣━━ mean capped hns: {np.mean(hnss)}")
+            print(f"┣━━ median hns: {np.median(hnss)}")
+            print(f"┣━━ mean hns: {np.mean(hnss)}")
```

### Comparing `openrlbenchmark-0.2.1a3/openrlbenchmark/offline_db.py` & `openrlbenchmark-0.2.1a4/openrlbenchmark/offline_db.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a3/openrlbenchmark/rlops.py` & `openrlbenchmark-0.2.1a4/openrlbenchmark/rlops.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     """the number of legend columns in the chart"""
     xlabel: str = "Steps"
     """the label of the x-axis"""
     ylabel: str = "Episodic Return"
     """the label of the y-axis"""
     sharex: bool = False
     """if toggled, we will share the x-axis across all subplots"""
+    max_steps: int = None
+    """if specified, the maximum number of steps to plot"""
     rolling: int = 100
     """the rolling window for smoothing the curves"""
     time_unit: str = "m"
     """the unit of time in the x-axis of the chart (e.g., `s` for seconds, `m` for minutes, `h` for hours); default: `m`"""
     cm: float = 4.0
     """the multiplier for the column width"""
     rm: float = 3.0
@@ -92,16 +94,14 @@
     """the last n number of episodes to average metric over in the result table"""
     scan_history: bool = False
     """if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)"""
     check_empty_runs: bool = True
     """if toggled, we will check for empty wandb runs"""
     report: bool = False
     """if toggled, a wandb report will be created"""
-    wandb_project_name: str = "cleanrl"
-    """the wandb project name for the report creation"""
     offline: bool = False
     """if toggled, we will use the offline database instead of wandb"""
     pc: PlotConfig = field(default_factory=PlotConfig)
     """the plot configuration"""
     rliable: bool = False
     """if toggled, we will use rliable to compute the metrics"""
     rc: RliableConfig = field(default_factory=RliableConfig)
@@ -141,20 +141,47 @@
         self.tags = tags
         self.username = username
         self.offline_db = offline_db
         self.offline = offline
 
         user = [{"username": self.username}] if self.username else []
         include_tag_groups = [{"tags": {"$in": [tag]}} for tag in self.tags] if len(self.tags) > 0 else []
+        
+        # hack to deal with wandb's nested config
+        # click the "View Raw Data" button of the config in
+        # https://wandb.ai/costa-huang/cleanRL/runs/3nhnaboz/overview
+        # to see how .value is added to the config
+        # it should look like this:
+        # {
+        #     ...
+        #     "env_id": { "desc": null, "value": "Pendulum-v1" },
+        # }
+        # so the correct key is `config.env_id.value`
+        # but sometimes configs are stored in a weird way like
+        # https://wandb.ai/costa-huang/trl/runs/lpwu2w4g/overview
+        # {
+        #   "trl_ppo_trainer_config": {
+        #     "desc": null,
+        #     "value": {
+        #       "lam": 0.95,
+        #       ...
+        #     }
+        #   }
+        # }
+        # so the correct key is `config.trl_ppo_trainer_config.value.lam`
+        if ".value" not in self.custom_env_id_key:
+            self.custom_env_id_key += ".value"
+        if ".value" not in self.custom_exp_name_key:
+            self.custom_exp_name_key += ".value"
         self.wandb_filters = {
             "$and": [
-                {f"config.{self.custom_env_id_key}.value": self.env_id},
+                {f"config.{self.custom_env_id_key}": self.env_id},
                 *include_tag_groups,
                 *user,
-                {f"config.{self.custom_exp_name_key}.value": self.exp_name},
+                {f"config.{self.custom_exp_name_key}": self.exp_name},
             ]
         }
 
     @property
     def runs(self):
         if not self.offline:
             return wandb.Api().runs(
@@ -202,15 +229,15 @@
     console.print(table)
 
 
 def create_hypothesis(runset: Runset, scan_history: bool = False) -> Hypothesis:
     runs = []
     for idx, run in enumerate(runset.runs):
         print("loading", run, run.url)
-        if run.state == "running" or run.state == "crashed":
+        if run.state == "running":
             print(f"Skipping running run: {run}")
             continue
         if scan_history:
             run = openrlbenchmark.cache.CachedRun(run, cache_dir=os.path.join(openrlbenchmark.__path__[0], "dataset"))
             with runset.offline_db.bind_ctx([OfflineRun, OfflineRunTag, Tag]):
                 tags = []
                 for tag_str in run.run.tags:
@@ -262,15 +289,15 @@
     report: bool = False,
     pc: PlotConfig = None,
 ):
     blocks = []
     if report:
         for idx, env_id in enumerate(env_ids):
             metric_over_step = wb.LinePlot(
-                x="global_step",
+                x=runsets[idx].custom_xaxis_key,
                 y=list({runsets[idx].metric for runsets in runsetss}),
                 title=env_id,
                 title_x="Steps",
                 title_y="Episodic Return",
                 max_runs_to_show=100,
                 smoothing_factor=0.8,
                 groupby_rangefunc="stderr",
@@ -373,14 +400,16 @@
             n_samples=10000,
             rolling=pc.rolling,
             colors=[runsets[idx].color for runsets in runsetss],
             legend=False,
         )
         ax.set_xlabel("")
         ax.set_ylabel("")
+        if pc.max_steps is not None:
+            ax.set_xlim(0, pc.max_steps)
         ax_time = axes_time_flatten[idx]
         ex.plot(
             ax=ax_time,
             title=env_id,
             x="_runtime",
             y="charts/episodic_return",
             err_style="band",
@@ -457,15 +486,15 @@
 def maxmin_normalize_score(score_dict: Dict[str, np.ndarray]):
     all_scores = np.concatenate([score_dict[key] for key in score_dict], axis=0)
     max_scores = all_scores.max(0).max(1)  # 1) max over all experiments and seds 2) max over all steps
     min_scores = all_scores.min(0).min(1)  # 1) min over all experiments and seds 2) min over all steps
     return normalize_score(score_dict, max_scores, min_scores)
 
 
-def atari_normalize_score(original_env_ids):
+def atari_normalize_score(score_dict, original_env_ids):
     env_ids = []
     for env_id in original_env_ids:
         if env_id.endswith("NoFrameskip-v4"):
             env_id = env_id.replace("NoFrameskip-v4", "-v5")
         env_ids.append(env_id)
     max_scores = np.array([atari_hns[env_id][1] for env_id in env_ids])
     min_scores = np.array([atari_hns[env_id][0] for env_id in env_ids])
@@ -632,15 +661,15 @@
             console,
         )
 
         # normalize scores.
         if args.rc.score_normalization_method == "maxmin":
             normalized_score_dict = maxmin_normalize_score(score_dict)
         elif args.rc.score_normalization_method == "atari":
-            normalized_score_dict = atari_normalize_score(args.env_ids[0])
+            normalized_score_dict = atari_normalize_score(score_dict, args.env_ids[0])
         else:
             raise NotImplementedError(f"Normalization method {args.rc.score_normalization_method} not implemented")
         performance_profile_normalized_score_dict = {}
         for key, value in normalized_score_dict.items():
             performance_profile_normalized_score_dict[key] = np.nanmean(value[:, :, -1:], axis=-1)
         metric_fns = [
             metrics.aggregate_median,
```

### Comparing `openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_hns.py` & `openrlbenchmark-0.2.1a4/openrlbenchmark/rlops_hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_multi_metrics.py` & `openrlbenchmark-0.2.1a4/openrlbenchmark/rlops_multi_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     """the number of legend columns in the chart"""
     xlabel: str = "Steps"
     """the label of the x-axis"""
     ylabel: str = "Episodic Return"
     """the label of the y-axis"""
     sharex: bool = False
     """if toggled, we will share the x-axis across all subplots"""
+    max_steps: int = None
+    """if specified, the maximum number of steps to plot"""
     rolling: int = 100
     """the rolling window for smoothing the curves"""
     time_unit: str = "m"
     """the unit of time in the x-axis of the chart (e.g., `s` for seconds, `m` for minutes, `h` for hours); default: `m`"""
     cm: float = 4.0
     """the multiplier for the column width"""
     rm: float = 3.0
@@ -92,16 +94,14 @@
     """the last n number of episodes to average metric over in the result table"""
     scan_history: bool = False
     """if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)"""
     check_empty_runs: bool = True
     """if toggled, we will check for empty wandb runs"""
     report: bool = False
     """if toggled, a wandb report will be created"""
-    wandb_project_name: str = "cleanrl"
-    """the wandb project name for the report creation"""
     offline: bool = False
     """if toggled, we will use the offline database instead of wandb"""
     pc: PlotConfig = field(default_factory=PlotConfig)
     """the plot configuration"""
     rliable: bool = False
     """if toggled, we will use rliable to compute the metrics"""
     rc: RliableConfig = field(default_factory=RliableConfig)
@@ -113,14 +113,15 @@
         self,
         name: str,
         entity: str,
         project: str,
         metrics: List[str] = ["charts/episodic_return"],
         groupby: str = "",
         custom_exp_name_key: str = "exp_name",
+        custom_xaxis_key: str = "global_step",
         exp_name: str = "",
         custom_env_id_key: str = "env_id",
         env_id: str = "",
         tags: List[str] = [],
         username: str = "",
         color: str = "#000000",
         offline_db: pw.Database = None,
@@ -128,31 +129,59 @@
     ):
         self.name = name
         self.entity = entity
         self.project = project
         self.metrics = metrics
         self.groupby = groupby
         self.custom_exp_name_key = custom_exp_name_key
+        self.custom_xaxis_key = custom_xaxis_key
         self.exp_name = exp_name
         self.custom_env_id_key = custom_env_id_key
         self.env_id = env_id
         self.color = color
         self.tags = tags
         self.username = username
         self.offline_db = offline_db
         self.offline = offline
 
         user = [{"username": self.username}] if self.username else []
         include_tag_groups = [{"tags": {"$in": [tag]}} for tag in self.tags] if len(self.tags) > 0 else []
+        
+        # hack to deal with wandb's nested config
+        # click the "View Raw Data" button of the config in
+        # https://wandb.ai/costa-huang/cleanRL/runs/3nhnaboz/overview
+        # to see how .value is added to the config
+        # it should look like this:
+        # {
+        #     ...
+        #     "env_id": { "desc": null, "value": "Pendulum-v1" },
+        # }
+        # so the correct key is `config.env_id.value`
+        # but sometimes configs are stored in a weird way like
+        # https://wandb.ai/costa-huang/trl/runs/lpwu2w4g/overview
+        # {
+        #   "trl_ppo_trainer_config": {
+        #     "desc": null,
+        #     "value": {
+        #       "lam": 0.95,
+        #       ...
+        #     }
+        #   }
+        # }
+        # so the correct key is `config.trl_ppo_trainer_config.value.lam`
+        if ".value" not in self.custom_env_id_key:
+            self.custom_env_id_key += ".value"
+        if ".value" not in self.custom_exp_name_key:
+            self.custom_exp_name_key += ".value"
         self.wandb_filters = {
             "$and": [
-                {f"config.{self.custom_env_id_key}.value": self.env_id},
+                {f"config.{self.custom_env_id_key}": self.env_id},
                 *include_tag_groups,
                 *user,
-                {f"config.{self.custom_exp_name_key}.value": self.exp_name},
+                {f"config.{self.custom_exp_name_key}": self.exp_name},
             ]
         }
 
     @property
     def runs(self):
         if not self.offline:
             return wandb.Api().runs(
@@ -196,15 +225,15 @@
         table.add_column(column)
     for _, row in df.iterrows():
         table.add_row(*row.astype(str).tolist())
     console.rule(f"[bold red]{title}")
     console.print(table)
 
 
-def create_hypothesis(runset: Runset, scan_history: bool = False) -> Hypothesis:
+def create_hypothesis(runset: Runset, target_metrics, scan_history: bool = False) -> Hypothesis:
     runs = []
     for idx, run in enumerate(runset.runs):
         print("loading", run, run.url)
         if run.state == "running":
             print(f"Skipping running run: {run}")
             continue
         if scan_history:
@@ -234,19 +263,20 @@
                 )
                 offline_run.save()
             run_df = run.run_df
         else:
             run_df = run.history(samples=1500)
         if "videos" in run_df:
             run_df = run_df.drop(columns=["videos"], axis=1)
-        if len(runset.metrics) == 1 and len(runset.metrics[0]) == 0:
-            run_df["charts/episodic_return"] = run_df[metrics]
-            cleaned_df = run_df[["global_step", "_runtime", "charts/episodic_return"]].dropna()
-        else:
-            cleaned_df = run_df[["global_step", "_runtime"] + runset.metrics].dropna(how="all")
+        if runset.custom_xaxis_key in run_df:
+            run_df["global_step"] = run_df[runset.custom_xaxis_key]
+        for source_metric, target_metric in zip(runset.metrics, target_metrics):
+            if source_metric in run_df:
+                run_df[target_metric] = run_df[source_metric]
+        cleaned_df = run_df[["global_step", "_runtime"] + target_metrics].dropna(how="all")
         runs += [Run(f"seed{idx}", cleaned_df)]
     return Hypothesis(runset.name, runs)
 
 
 def compare(
     console: Console,
     runsetss: List[List[Runset]],
@@ -260,15 +290,15 @@
     blocks = []
     if report:
         for idx, env_id in enumerate(env_ids):
             metrics_over_step = []
             metrics_over_time = []
             for i in range(len(runsetss[0][idx].metrics)):
                 metric_over_step = wb.LinePlot(
-                    x="global_step",
+                    x=runsetss[0][idx].custom_xaxis_key,
                     y=list({runsets[idx].metrics[i] for runsets in runsetss}),
                     title=runsetss[0][idx].metrics[i] + " " + env_id,
                     title_x="Steps",
                     title_y="Episodic Return",
                     max_runs_to_show=100,
                     smoothing_factor=0.8,
                     groupby_rangefunc="stderr",
@@ -292,23 +322,24 @@
             flattened_metrics = [metrics_over_step, metrics_over_time]
             flattened_metrics = [item for sublist in flattened_metrics for item in sublist]
             pg = wb.PanelGrid(
                 runsets=[runsets[idx].report_runset for runsets in runsetss],
                 panels=flattened_metrics,
             )
             custom_run_colors = {}
-            for runsets in runsetss:
-                custom_run_colors.update(
-                    {
-                        (
-                            runsets[idx].report_runset.name,
-                            runsets[idx].runs[0].config[runsets[idx].custom_exp_name_key],
-                        ): runsets[idx].color
-                    }
-                )
+            # TODO: color stuff doesn't work because of the filter syntax
+            # for runsets in runsetss:
+            #     custom_run_colors.update(
+            #         {
+            #             (
+            #                 runsets[idx].report_runset.name,
+            #                 runsets[idx].runs[0].config[runsets[idx].custom_exp_name_key],
+            #             ): runsets[idx].color
+            #         }
+            #     )
             pg.custom_run_colors = custom_run_colors  # IMPORTANT: custom_run_colors is implemented as a custom `setter` that needs to be overwritten unlike regular dictionaries
             blocks += [pg]
 
     figsize = (pc.ncols * pc.cm, pc.nrows * pc.rm)
     fig, axes = plt.subplots(
         nrows=pc.nrows,
         ncols=pc.ncols,
@@ -331,15 +362,15 @@
 
     result_table = pd.DataFrame(index=env_ids, columns=[runsets[0].name for runsets in runsetss])
     exs = []
     runtimes = []
     global_steps = []
     for idx, env_id in enumerate(env_ids):
         print(f"collecting runs for {env_id}")
-        hypotheses = [create_hypothesis(runsets[idx], scan_history) for runsets in runsetss]
+        hypotheses = [create_hypothesis(runsets[idx], runsetss[0][idx].metrics, scan_history) for runsets in runsetss]
         ex = expt.Experiment("Comparison", hypotheses)
         exs.append(ex)
 
         # for each run `i` get the average of the last `rolling` episodes as r_i
         # then take the average and std of r_i as the results.
         result = []
         for hypothesis in ex.hypotheses:
@@ -363,30 +394,33 @@
             metric_str = metric.replace("eval/", "")
             ax = axes_flatten[len(env_ids) * idx_metric + idx]
             ex.plot(
                 ax=ax,
                 title=env_id,
                 x="global_step",
                 y=metric,
-                err_style="band",
+                err_style="unit_traces",
                 std_alpha=0.1,
                 n_samples=10000,
                 rolling=pc.rolling,
                 colors=[runsets[idx].color for runsets in runsetss],
                 legend=False,
             )
+            # breakpoint()
             ax.set_xlabel("")
             if idx_metric == 0:
                 ax.set_title(env_id)
             else:
                 ax.set_title("")
             if idx == 0:
                 ax.set_ylabel(metric_str)
             else:
                 ax.set_ylabel("")
+            if pc.max_steps is not None:
+                ax.set_xlim(0, pc.max_steps)
             ax_time = axes_time_flatten[len(env_ids) * idx_metric + idx]
             ex.plot(
                 ax=ax_time,
                 title=env_id,
                 x="_runtime",
                 y=metric,
                 err_style="band",
@@ -406,15 +440,15 @@
             else:
                 ax_time.set_ylabel("")
     runtimes = pd.DataFrame(np.array(runtimes), index=env_ids, columns=list(ex.summary()["name"]))
     global_steps = pd.DataFrame(np.array(global_steps), index=env_ids, columns=list(ex.summary()["name"]))
     print_rich_table(f"Runtime ({pc.time_unit}) (mean ± std)", runtimes.rename_axis("Environment").reset_index(), console)
 
     # create the required directory for `output_filename`
-    if os.path.dirname(output_filename) != "":
+    if len(os.path.dirname(output_filename)) > 0:
         os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     print_rich_table(f"{pc.ylabel} (mean ± std)", result_table.rename_axis("Environment").reset_index(), console)
     result_table.to_markdown(open(f"{output_filename}.md", "w"))
     result_table.to_csv(open(f"{output_filename}.csv", "w"))
     runtimes.to_markdown(open(f"{output_filename}_runtimes.md", "w"))
     runtimes.to_csv(open(f"{output_filename}_runtimes.csv", "w"))
     average_runtime = pd.DataFrame(runtimes.mean(axis=0)).reset_index()
@@ -468,15 +502,15 @@
 def maxmin_normalize_score(score_dict: Dict[str, np.ndarray]):
     all_scores = np.concatenate([score_dict[key] for key in score_dict], axis=0)
     max_scores = all_scores.max(0).max(1)  # 1) max over all experiments and seds 2) max over all steps
     min_scores = all_scores.min(0).min(1)  # 1) min over all experiments and seds 2) min over all steps
     return normalize_score(score_dict, max_scores, min_scores)
 
 
-def atari_normalize_score(original_env_ids):
+def atari_normalize_score(score_dict, original_env_ids):
     env_ids = []
     for env_id in original_env_ids:
         if env_id.endswith("NoFrameskip-v4"):
             env_id = env_id.replace("NoFrameskip-v4", "-v5")
         env_ids.append(env_id)
     max_scores = np.array([atari_hns[env_id][1] for env_id in env_ids])
     min_scores = np.array([atari_hns[env_id][0] for env_id in env_ids])
@@ -485,43 +519,44 @@
 
 if __name__ == "__main__":
     args = tyro.cli(Args)
     # by default assume all the env_ids are the same
     if len(args.filters) > 1 and len(args.env_ids) == 1:
         args.env_ids = args.env_ids * len(args.filters)
 
-    parse_result = urlparse(args.filters[0][0])
-    query = parse_qs(parse_result.query)
-    metrics = query["metrics"] if "metrics" in query else ["charts/episodic_return"]
-    # calculate the number of rows
-    args.pc.nrows = np.ceil(len(args.env_ids[0]) * len(metrics) / args.pc.ncols).astype(int)
-
     console = Console()
     blocks = []
     runsetss = []
     offline_dbs = {}
     colors_flatten_original = [c for item in ["deep", "dark", "bright"] for c in sns.color_palette(item).as_hex()]
     plt.rcParams["axes.prop_cycle"] = plt.cycler("color", colors_flatten_original)
     colors_flatten = copy.deepcopy(colors_flatten_original)
     colors = []
     for filters in args.filters:
         colors += [colors_flatten[: len(filters) - 1]]
         colors_flatten = colors_flatten[len(filters) - 1 :]
 
     for filters_idx, filters in enumerate(args.filters):
+        parse_result = urlparse(filters[0])
+        query = parse_qs(parse_result.query)
+        metrics = query["metrics"] if "metrics" in query else ["charts/episodic_return"]
+        # calculate the number of rows
+        args.pc.nrows = np.ceil(len(args.env_ids[0]) * len(metrics) / args.pc.ncols).astype(int)
         wandb_project_name = query["wpn"][0] if "wpn" in query else args.wandb_project_name
         wandb_entity = query["we"][0] if "we" in query else args.wandb_entity
         custom_env_id_key = query["ceik"][0] if "ceik" in query else "env_id"
         custom_exp_name_key = query["cen"][0] if "cen" in query else "exp_name"
+        custom_xaxis_key = query["xaxis"][0] if "xaxis" in query else "global_step"
         pprint(
             {
                 "wandb_project_name": wandb_project_name,
                 "wandb_entity": wandb_entity,
                 "custom_env_id_key": custom_env_id_key,
                 "custom_exp_name_key": custom_exp_name_key,
+                "custom_xaxis_key": custom_xaxis_key,
                 "metrics": metrics,
             },
             expand_all=True,
         )
         if f"{wandb_entity}/{wandb_project_name}" not in offline_dbs:
             offline_db_folder = os.path.join(openrlbenchmark.__path__[0], "dataset", f"{wandb_entity}/{wandb_project_name}")
             offline_db_path = os.path.join(offline_db_folder, "offline.sqlite")
@@ -553,14 +588,15 @@
                         if custom_legend == ""
                         else custom_legend,
                         entity=wandb_entity,
                         project=wandb_project_name,
                         metrics=metrics,
                         groupby=custom_exp_name_key,
                         custom_exp_name_key=custom_exp_name_key,
+                        custom_xaxis_key=custom_xaxis_key,
                         exp_name=exp_name,
                         custom_env_id_key=custom_env_id_key,
                         env_id=env_id,
                         tags=tags,
                         username=username,
                         color=color,
                         offline_db=offline_dbs[f"{wandb_entity}/{wandb_project_name}"],
```

### Comparing `openrlbenchmark-0.2.1a3/pyproject.toml` & `openrlbenchmark-0.2.1a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openrlbenchmark"
-version = "0.2.1a3"
+version = "0.2.1a4"
 description = ""
 authors = ["Costa Huang <costa.huang@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "openrlbenchmark" },
 ]
```

### Comparing `openrlbenchmark-0.2.1a3/PKG-INFO` & `openrlbenchmark-0.2.1a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrlbenchmark
-Version: 0.2.1a3
+Version: 0.2.1a4
 Summary: 
 Author: Costa Huang
 Author-email: costa.huang@outlook.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -103,15 +103,15 @@
 * `cen`: the custom key for the experiment name
 * `metric`: the metric we are interested in
 
 So we are fetching metrics from [https://wandb.ai/openrlbenchmark/baselines](https://wandb.ai/openrlbenchmark/baselines). The environment id is stored in the `env` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`.
 
 Similarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `baselines-ppo2-mlp?cl=openai/baselines PPO2`.
 
-The labels of the figure can be customized with the `--pc.xlabel` and `--pc.ylabel` flags. The `--pc.ncols` flag specifies the number of columns in the figure. The `--pc.ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure
+The labels of the figure can be customized with the `--pc.xlabel` and `--pc.ylabel` flags. You can also specify the maximum number of timesteps to plot with `--pc.max_steps`. The `--pc.ncols` flag specifies the number of columns in the figure. The `--pc.ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure
 
 The `--rliable` toggles our [rliable](https://github.com/google-research/rliable) integration, and its configuration can be tweeked via `--rc`. The command above generates the following plot:
 
 ![](static/baseline_vs_cleanrl.png)
 ![](static/baseline_vs_cleanrl-time.png)
 ![](static/baseline_vs_cleanrl_sample_walltime_efficiency.png)
 ![](static/baseline_vs_cleanrl_sample_efficiency.png)
@@ -318,34 +318,36 @@
     --output-filename static/td3_vs_cleanrl \
     --scan-history
 ```
 ![](static/td3_vs_cleanrl.png)
 
 
 
-### Compare MORL Baselines algorithms on deterministic environments
+### Compare MORL Baselines algorithms
+Notice the number of timesteps is adjusted using `--pc.max_steps 400000`.
 
 ```shell
 python -m openrlbenchmark.rlops_multi_metrics \
-  --filters '?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metrics=eval/hypervolume&metrics=eval/igd&metrics=eval/sparsity&metrics=eval/eum&metrics=eval/mul' \
-  'Pareto Q-Learning?cl=Pareto Q-Learning' \
-  'MultiPolicy MO Q-Learning?cl=MultiPolicy MO Q-Learning' \
-  'MultiPolicy MO Q-Learning (OLS)?cl=MultiPolicy MO Q-Learning (OLS)' \
-  'MultiPolicy MO Q-Learning (GPI-LS)?cl=MultiPolicy MO Q-Learning (GPI-LS)' \
-  --env-ids deep-sea-treasure-v0 deep-sea-treasure-concave-v0 fruit-tree-v0 \
-  --pc.ncols 3 \
+  --filters '?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metrics=eval/hypervolume&metrics=eval/sparsity&metrics=eval/eum' \
+  'PGMORL?cl=PGMORL' \
+  'CAPQL?cl=CAPQL' \
+  'GPI-LS Continuous Action?cl=GPI-LS' \
+  'GPI-PD Continuous Action?cl=GPI-PD' \
+  --env-ids mo-halfcheetah-v4 mo-hopper-2d-v4  \
+  --pc.ncols 2 \
   --pc.ncols-legend 4 \
   --pc.xlabel 'Training steps' \
   --pc.ylabel '' \
-  --output-filename morl_deterministic_envs/ \
+  --pc.max_steps 400000 \
+  --output-filename morl/morl_continuous \
   --scan-history
 ```
 
-![](static/morl_deterministic_envs.png)
-![](static/morl_deterministic_envs-time.png)
+![](static/morl_continuous.png)
+![](static/morl_continuous-time.png)
 
 ### Calculate human normalized scores
 
 ```shell
 python -m openrlbenchmark.hns --files static/cleanrl_vs_baselines.csv static/machado_10M.csv static/machado_50M.csv 
 ```
```

