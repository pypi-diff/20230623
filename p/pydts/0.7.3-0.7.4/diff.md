# Comparing `tmp/pydts-0.7.3.tar.gz` & `tmp/pydts-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydts-0.7.3.tar", max compression
+gzip compressed data, was "pydts-0.7.4.tar", max compression
```

## Comparing `pydts-0.7.3.tar` & `pydts-0.7.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.7.3/LICENSE
--rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.7.3/README.md
--rw-r--r--   0        0        0     1418 2023-05-03 11:59:33.612549 pydts-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.7.3/src/pydts/.DS_Store
--rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.7.3/src/pydts/__init__.py
--rw-r--r--   0        0        0    12925 2023-05-02 14:58:03.593428 pydts-0.7.3/src/pydts/base_fitters.py
--rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.7.3/src/pydts/config.py
--rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.7.3/src/pydts/cross_validation.py
--rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.7.3/src/pydts/data_generation.py
--rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.7.3/src/pydts/datasets/.DS_Store
--rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.7.3/src/pydts/datasets/LOS_simulated_data.csv
--rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.7.3/src/pydts/evaluation.py
--rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.7.3/src/pydts/examples_utils/__init__.py
--rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.7.3/src/pydts/examples_utils/datasets.py
--rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.7.3/src/pydts/examples_utils/generate_simulations_data.py
--rw-r--r--   0        0        0    31441 2023-05-03 11:48:22.485542 pydts-0.7.3/src/pydts/examples_utils/plots.py
--rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.7.3/src/pydts/examples_utils/simulations_data_config.py
--rw-r--r--   0        0        0    31641 2023-05-02 17:17:43.984979 pydts-0.7.3/src/pydts/fitters.py
--rw-r--r--   0        0        0     8936 2023-02-22 11:16:27.801701 pydts-0.7.3/src/pydts/model_selection.py
--rw-r--r--   0        0        0     5994 2022-12-02 13:43:44.154153 pydts-0.7.3/src/pydts/utils.py
--rw-r--r--   0        0        0     3853 2023-05-03 11:59:46.543892 pydts-0.7.3/setup.py
--rw-r--r--   0        0        0     3981 2023-05-03 11:59:46.544218 pydts-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.7.4/LICENSE
+-rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.7.4/README.md
+-rw-r--r--   0        0        0     1418 2023-06-23 19:40:20.475297 pydts-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.7.4/src/pydts/.DS_Store
+-rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.7.4/src/pydts/__init__.py
+-rw-r--r--   0        0        0    12925 2023-05-02 14:58:03.593428 pydts-0.7.4/src/pydts/base_fitters.py
+-rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.7.4/src/pydts/config.py
+-rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.7.4/src/pydts/cross_validation.py
+-rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.7.4/src/pydts/data_generation.py
+-rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.7.4/src/pydts/datasets/.DS_Store
+-rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.7.4/src/pydts/datasets/LOS_simulated_data.csv
+-rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.7.4/src/pydts/evaluation.py
+-rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.7.4/src/pydts/examples_utils/__init__.py
+-rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.7.4/src/pydts/examples_utils/datasets.py
+-rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.7.4/src/pydts/examples_utils/generate_simulations_data.py
+-rw-r--r--   0        0        0    14554 2023-06-22 21:08:27.939724 pydts-0.7.4/src/pydts/examples_utils/mimic_consts.py
+-rw-r--r--   0        0        0    33784 2023-06-23 19:40:20.486964 pydts-0.7.4/src/pydts/examples_utils/plots.py
+-rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.7.4/src/pydts/examples_utils/simulations_data_config.py
+-rw-r--r--   0        0        0    31476 2023-06-23 19:40:20.471655 pydts-0.7.4/src/pydts/fitters.py
+-rw-r--r--   0        0        0     8936 2023-02-22 11:16:27.801701 pydts-0.7.4/src/pydts/model_selection.py
+-rw-r--r--   0        0        0     5994 2022-12-02 13:43:44.154153 pydts-0.7.4/src/pydts/utils.py
+-rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 pydts-0.7.4/PKG-INFO
```

### Comparing `pydts-0.7.3/LICENSE` & `pydts-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/README.md` & `pydts-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/pyproject.toml` & `pydts-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydts"
-version = "0.7.3"
+version = "0.7.4"
 description = "Discrete time survival analysis with competing risks"
 authors = ["Tomer Meir <tomer1812@gmail.com>", "Rom Gutman <rom.gutman1@gmail.com>", "Malka Gorfine <malkago12@gmail.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/tomer1812/pydts"
 repository = "https://github.com/tomer1812/pydts"
 keywords = ["Discrete Time", "Time to Event" ,"Survival Analysis", "Competing Events"]
```

### Comparing `pydts-0.7.3/src/pydts/.DS_Store` & `pydts-0.7.4/src/pydts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/src/pydts/base_fitters.py` & `pydts-0.7.4/src/pydts/base_fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/src/pydts/cross_validation.py` & `pydts-0.7.4/src/pydts/cross_validation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/src/pydts/data_generation.py` & `pydts-0.7.4/src/pydts/data_generation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/src/pydts/datasets/.DS_Store` & `pydts-0.7.4/src/pydts/datasets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/src/pydts/datasets/LOS_simulated_data.csv` & `pydts-0.7.4/src/pydts/datasets/LOS_simulated_data.csv`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/src/pydts/evaluation.py` & `pydts-0.7.4/src/pydts/evaluation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/src/pydts/examples_utils/generate_simulations_data.py` & `pydts-0.7.4/src/pydts/examples_utils/generate_simulations_data.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/src/pydts/examples_utils/plots.py` & `pydts-0.7.4/src/pydts/examples_utils/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                s=130, alpha=0.4)
     ax.set_xlabel('Covariate', fontsize=18)
     ax.set_ylabel(r'$\beta}$', fontsize=18)
     ax.legend(loc='upper center', fontsize=12)
     ax.set_ylim([-1.5, 1])
     fig.tight_layout()
     if filename is not None:
-        fig.savefig(os.path.join(OUTPUT_DIR, filename), dpi=300)
+        fig.savefig(filename, dpi=300)
 
 
 def plot_LOS_simulation_figure1(data_df):
     text_sz = 16
 
     fig, axes = plt.subplots(2, 2, figsize=(14, 8))
 
@@ -517,14 +517,58 @@
     if filename is not None:
         fig.savefig(os.path.join(OUTPUT_DIR, filename), dpi=300)
 
     if return_summary:
         return res_dict
 
 
+def plot_jss_reps_coef_std(rep_dict: dict, return_summary: bool = True, filename: str = None, paper_plots: bool = False):
+    alphabet_list = list(string.ascii_lowercase)
+    first_key = next(iter(rep_dict))    # deal with cases where there isn't 0 in samples
+    coef_types = list(rep_dict[first_key].keys())  # alpha, beta
+    event_types = rep_dict[first_key][coef_types[0]].keys()
+    fig, axes = plt.subplots(1, 2, figsize=(12, 5))
+    res_dict = {coef: {event_type: None for event_type in event_types} for coef in coef_types}
+    for idct, coef_type in enumerate(coef_types):
+        for idet, event_type in enumerate(event_types):
+            if coef_type == 'alpha':
+                ax = axes[event_type - 1]
+                add_panel_text(ax=ax, text=alphabet_list[idct*len(event_types)+idet])
+                ax.tick_params(axis='both', which='major', labelsize=15)
+                ax.tick_params(axis='both', which='minor', labelsize=15)
+            df = pd.concat([dfs[coef_type][event_type] for dfs in rep_dict.values()])
+            temp_df = df.groupby(df.index).agg(["mean", "std"])
+            prefix = "a" if coef_type == "alpha" else "Z"
+            temp_df = temp_df.loc[[f"{prefix}{idx}_{event_type}" for idx in range(1, temp_df.shape[0]+1)]]
+            temp_df.columns = temp_df.columns.get_level_values(0) + "_" + temp_df.columns.get_level_values(1)
+            res_dict[coef_type][event_type] = temp_df.copy()
+            if coef_type == 'alpha':
+                temp_df.plot(x="Lee_std", y="Ours_std", kind="scatter", ax=ax)
+                ax.set_xlabel("Lee et al. std", fontsize=18)
+                ax.set_ylabel("two-step std", fontsize=18)
+                ax.plot([0, 1], [0, 1], "--", transform=ax.transAxes, alpha=0.3, color="tab:green");
+                ax.grid()
+                if ((idct == 0) and (idet == 0)):
+                    ax.set_xlim([0, 0.2])
+                    ax.set_ylim([0, 0.2])
+                elif ((idct == 0) and (idet == 1)):
+                    ax.set_xlim([0, 0.25])
+                    ax.set_ylim([0, 0.25])
+                latter = "\\alpha" if coef_type == "alpha" else "\\beta"
+                ax.set_title(f"${latter}{event_type}$", fontsize=18)
+    fig.tight_layout()
+    fig.show()
+    if filename is not None:
+        fig.savefig(filename, dpi=300)
+
+    if return_summary:
+        return res_dict
+
+
+
 def plot_times(times_dict: dict,
                filename: str = None,
                ax = None, color='tab:blue') -> None:
     if ax is None:
 
         ax = pd.DataFrame.from_dict(times_dict).boxplot(figsize=(8, 6), boxprops={"lw": 1.5, "color": "tab:blue"},
                                                         medianprops={"lw": 2, "color": "tab:green"},
```

### Comparing `pydts-0.7.3/src/pydts/examples_utils/simulations_data_config.py` & `pydts-0.7.4/src/pydts/examples_utils/simulations_data_config.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/src/pydts/fitters.py` & `pydts-0.7.4/src/pydts/fitters.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,15 +565,14 @@
         ax.legend()
         if show:
             plt.show()
         return ax
 
 
 def repetitive_fitters(rep: int, n_patients: int, n_cov: int, d_times: int, j_events: int, pid_col: str,
-                       test_size: float,
                        drop_cols: Iterable = ("C", "T"),
                        model1: ExpansionBasedFitter = DataExpansionFitter,
                        model1_name="Lee",
                        model2: ExpansionBasedFitter = TwoStagesFitter,
                        model2_name: str = "Ours",
                        allow_fails: int = 20,
                        verbose: int = 2,
@@ -612,44 +611,42 @@
             its beta/alpha/real coefficients dataframe (value).
         times (dict): Dictionary which  contains for each model (key) a list of the training times (value).
         ret_df (pd.DataFrame): Dataframe which contains for each time in d times, the average amount of events for it.
 
     """
 
     from .examples_utils.plots import compare_beta_models_for_example
-    from sklearn.model_selection import train_test_split
     from tqdm import trange
     from time import time
     assert real_coef_dict is not None, "The user should supply the coefficients of the experiment"
     rep_dict = {}
     times = {model1_name: [], model2_name: []}
     counts_df_list = []
     final = 0
     failed = 0
     for samp in trange(rep+allow_fails):
         try:
             patients_df = generate_quick_start_df(n_patients=n_patients, n_cov=n_cov, d_times=d_times,
                                                   j_events=j_events,
                                                   pid_col=pid_col, seed=samp, real_coef_dict=real_coef_dict,
                                                   censoring_prob=censoring_prob )
-            train_df, test_df = train_test_split(patients_df, test_size=test_size)
-            counts_df = train_df[train_df['X'] <= d_times].groupby(['J', 'X']).size().to_frame(samp)
+            counts_df = patients_df[patients_df['X'] <= d_times].groupby(['J', 'X']).size().to_frame(samp)
             assert not (counts_df.reset_index()['X'].value_counts() < (j_events + 1)).any(), "Not enough events"
             counts_df_list.append(counts_df)
             drop_cols = pd.Index(drop_cols)
             start_1 = time()
             fitter = model1()
-            fitter.fit(df=train_df.drop(drop_cols, axis=1))
+            fitter.fit(df=patients_df.drop(drop_cols, axis=1))
             end_1 = time()
             start_2 = time()
             new_fitter = model2()
             if isinstance(new_fitter, TwoStagesFitter):
-                new_fitter.fit(df=train_df.drop(drop_cols, axis=1), verbose=verbose)
+                new_fitter.fit(df=patients_df.drop(drop_cols, axis=1), verbose=verbose)
             else:
-                new_fitter.fit(df=train_df.drop(drop_cols, axis=1))
+                new_fitter.fit(df=patients_df.drop(drop_cols, axis=1))
             end_2 = time()
             times[model1_name].append(end_1 - start_1)
             times[model2_name].append(end_2 - start_2)
             res_dict = compare_beta_models_for_example(fitter.event_models,
                                                        new_fitter.event_models, real_coef_dict=real_coef_dict)
             rep_dict[samp] = res_dict
             final += 1
@@ -658,8 +655,8 @@
         except Exception as e:
             print(e)
             failed += 1
             print(f'Failed to fit sample {samp+1}, fail #{failed}')
             continue
     print(f'final: {final}')
     ret_df = pd.concat(counts_df_list, axis=1).fillna(0).mean(axis=1).apply(np.ceil).to_frame()
-    return rep_dict, times, ret_df
+    return rep_dict, times, ret_df
```

### Comparing `pydts-0.7.3/src/pydts/model_selection.py` & `pydts-0.7.4/src/pydts/model_selection.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/src/pydts/utils.py` & `pydts-0.7.4/src/pydts/utils.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.3/PKG-INFO` & `pydts-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pydts
-Version: 0.7.3
+Version: 0.7.4
 Summary: Discrete time survival analysis with competing risks
 Home-page: https://github.com/tomer1812/pydts
 License: GNU GPLv3
 Keywords: Discrete Time,Time to Event,Survival Analysis,Competing Events
 Author: Tomer Meir
 Author-email: tomer1812@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: ipython (>=8.2.0,<9.0.0)
 Requires-Dist: lifelines (>=0.26.4,<0.27.0)
 Requires-Dist: mkdocs (>=1.2.3,<2.0.0)
 Requires-Dist: mkdocs-material (>=8.2.4,<9.0.0)
 Requires-Dist: mkdocstrings (>=0.18.1,<0.19.0)
 Requires-Dist: mknotebooks (>=0.7.1,<0.8.0)
 Requires-Dist: numpy (>=1.23.4)
```

