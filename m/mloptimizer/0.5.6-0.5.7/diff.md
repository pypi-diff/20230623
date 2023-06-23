# Comparing `tmp/mloptimizer-0.5.6.tar.gz` & `tmp/mloptimizer-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mloptimizer-0.5.6.tar", last modified: Wed Apr  5 00:25:58 2023, max compression
+gzip compressed data, was "mloptimizer-0.5.7.tar", last modified: Fri Jun 23 14:21:06 2023, max compression
```

## Comparing `mloptimizer-0.5.6.tar` & `mloptimizer-0.5.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:25:58.831793 mloptimizer-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-05 00:25:58.831793 mloptimizer-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:25:58.827793 mloptimizer-0.5.6/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1954444 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/data/data_sample.csv
--rw-r--r--   0 runner    (1001) docker     (123)   694332 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/data/data_sample_test.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1260187 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/data/data_sample_train.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:25:58.827793 mloptimizer-0.5.6/mloptimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    38000 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/genoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/model_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:25:58.831793 mloptimizer-0.5.6/mloptimizer/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/test/test_TreeOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/test/test_XGBClassifierOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/test/test_alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/test/test_genoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/mloptimizer/test/test_param.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:25:58.831793 mloptimizer-0.5.6/mloptimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-05 00:25:58.000000 mloptimizer-0.5.6/mloptimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-05 00:25:58.000000 mloptimizer-0.5.6/mloptimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 00:25:58.000000 mloptimizer-0.5.6/mloptimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-05 00:25:58.000000 mloptimizer-0.5.6/mloptimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-05 00:25:58.000000 mloptimizer-0.5.6/mloptimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 00:25:58.831793 mloptimizer-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-04-05 00:25:45.000000 mloptimizer-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:21:06.654225 mloptimizer-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-23 14:21:06.654225 mloptimizer-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:21:06.650225 mloptimizer-0.5.7/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1954444 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/data/data_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   694332 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/data/data_sample_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1260187 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/data/data_sample_train.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:21:06.650225 mloptimizer-0.5.7/mloptimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39217 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/genoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/model_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:21:06.654225 mloptimizer-0.5.7/mloptimizer/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/test_TreeOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/test_XGBClassifierOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/test_alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/test_genoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/test_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:21:06.654225 mloptimizer-0.5.7/mloptimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-23 14:21:06.000000 mloptimizer-0.5.7/mloptimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-23 14:21:06.000000 mloptimizer-0.5.7/mloptimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:21:06.000000 mloptimizer-0.5.7/mloptimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 14:21:06.000000 mloptimizer-0.5.7/mloptimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 14:21:06.000000 mloptimizer-0.5.7/mloptimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:21:06.654225 mloptimizer-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/setup.py
```

### Comparing `mloptimizer-0.5.6/LICENSE` & `mloptimizer-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/PKG-INFO` & `mloptimizer-0.5.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.5.6
+Version: 0.5.7
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mloptimizer-0.5.6/README.md` & `mloptimizer-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/data/data_sample.csv` & `mloptimizer-0.5.7/data/data_sample.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/data/data_sample_test.csv` & `mloptimizer-0.5.7/data/data_sample_test.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/data/data_sample_train.csv` & `mloptimizer-0.5.7/data/data_sample_train.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/mloptimizer/alg_wrapper.py` & `mloptimizer-0.5.7/mloptimizer/alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/mloptimizer/genoptimizer.py` & `mloptimizer-0.5.7/mloptimizer/genoptimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import xgboost as xgb
 from keras.wrappers.scikit_learn import KerasClassifier
 from catboost import CatBoostClassifier
 import joblib
 import os
 import shutil
 from datetime import datetime
+import time
 from mloptimizer.plots import plot_search_space, plot_logbook
 
 
 class Param(object):
     """
     Object to store param info, type and range of values
     """
@@ -84,40 +85,50 @@
         equals = (self.name == other_param.name and self.min_value == other_param.min_value and
                   self.type == other_param.type and self.denominator == other_param.denominator and
                   self.max_value == other_param.max_value)
         return equals
 
     def __str__(self):
         """Overrides the default implementation"""
-        return "Param({}, {}, {}, {})".format(
-            self.name,
-            self.min_value,
-            self.max_value,
-            self.type.__name__
-        )
+        if self.type == float:
+            param_str = "Param('{}', {}, {}, {}, {})".format(
+                self.name,
+                self.min_value,
+                self.max_value,
+                self.type.__name__,
+                self.denominator
+            )
+        else:
+            param_str = "Param('{}', {}, {}, {})".format(
+                self.name,
+                self.min_value,
+                self.max_value,
+                self.type.__name__
+            )
+
+        return param_str
 
     def __repr__(self):
         """Overrides the default implementation"""
-        return "Param({}, {}, {}, {})".format(
-            self.name,
-            self.min_value,
-            self.max_value,
-            self.type.__name__
-        )
+        return self.__str__()
 
 
 class BaseOptimizer(object):
     """
     Abstract class to create optimizer for different machine learning classifier algorithms
     """
     __metaclass__ = ABCMeta
 
     def __init__(self, features: np.array, labels: np.array, folder=None, log_file="mloptimizer.log",
                  custom_params: dict = {},
                  custom_fixed_params: dict = {}, eval_function=KFoldStratifiedAccuracy):
+        self.logbook = None
+        self.progress_path = None
+        self.progress_path = None
+        self.exe_path = None
         self.features = features
         self.labels = labels
         self.folder = miscellaneous.create_optimization_folder(folder)
         self.custom_params = custom_params
         self.custom_fixed_params = custom_fixed_params
         self.params = self.get_params()
         self.fixed_params = self.get_fixed_params()
@@ -150,16 +161,16 @@
         return ind
 
     @abstractmethod
     def individual2dict(self, individual):
         individual_dict = {}
         keys = list(self.params.keys())
         for i in range(len(keys)):
-            individual_dict[keys[i]] = individual[i]
-        return individual_dict
+            individual_dict[keys[i]] = self.params[keys[i]].correct(individual[i])
+        return {**individual_dict, **self.get_fixed_params()}
 
     @abstractmethod
     def get_params(self):
         """
         Params for the creation of individuals (relative to the algorithm)
         These params define the name of the param, min value, max value, and type
 
@@ -195,37 +206,31 @@
         }
         return default_fixed_params
 
     @abstractmethod
     def get_clf(self, individual):
         pass
 
-    def get_corrected_clf(self, individual_in):
-        individual = copy.copy(individual_in)
-        keys = list(self.params.keys())
-        for i in range(len(keys)):
-            individual[i] = self.params[keys[i]].correct(individual[i])
-        return self.get_clf(individual)
 
     def evaluate_clf(self, individual):
         """
         Method to evaluate the individual, in this case the classifier
 
         :param individual: individual for evaluation
         :return: fitness
         """
-        mean = self.eval_function(self.features, self.labels, self.get_corrected_clf(individual))
+        mean = self.eval_function(self.features, self.labels, self.get_clf(individual))
         return (mean,)
 
     def population_2_df(self):
         data = []
         n = 0
         for p in self.populations:
             for i in p:
-                i_params = self.get_corrected_clf(i[0]).get_params()
+                i_params = self.get_clf(i[0]).get_params()
                 i_params['fitness'] = i[1].values[0]
                 i_params['population'] = n
                 data.append(i_params)
             n += 1
 
         df = pd.DataFrame(data)
         return df
@@ -300,26 +305,30 @@
             self.results_path = os.path.join(self.checkpoint_path, "results")
             self.graphics_path = os.path.join(self.checkpoint_path, "graphics")
         else:
 
             self.logbook.header = ['gen', 'nevals'] + (stats.fields if stats else [])
 
             # Create checkpoint_path from date and algorithm
-            checkpoint_exe_name = "{}_{}".format(
+            exe_name = "{}_{}".format(
                 datetime.now().strftime("%Y%m%d_%s"),
                 type(self).__name__)
-            self.checkpoint_path = os.path.join(self.folder, checkpoint_exe_name)
-            self.results_path = os.path.join(self.checkpoint_path, "results")
-            self.graphics_path = os.path.join(self.checkpoint_path, "graphics")
-            if os.path.exists(self.checkpoint_path):
-                shutil.rmtree(self.checkpoint_path)
+            self.exe_path = os.path.join(self.folder, exe_name)
+            self.checkpoint_path = os.path.join(self.exe_path, "checkpoints")
+            self.results_path = os.path.join(self.exe_path, "results")
+            self.graphics_path = os.path.join(self.exe_path, "graphics")
+            self.progress_path = os.path.join(self.exe_path, "progress")
+            if os.path.exists(self.exe_path):
+                shutil.rmtree(self.exe_path)
+            os.mkdir(self.exe_path)
             os.mkdir(self.checkpoint_path)
             os.mkdir(self.results_path)
             os.mkdir(self.graphics_path)
-            self.optimization_logger, _ = miscellaneous.init_logger(os.path.join(self.checkpoint_path, "opt.log"))
+            os.mkdir(self.progress_path)
+            self.optimization_logger, _ = miscellaneous.init_logger(os.path.join(self.exe_path, "opt.log"))
 
         # Methods for genetic algorithm
         toolbox.register("mate", tools.cxTwoPoint)
         toolbox.register("mutate", tools.mutUniformInt, low=[x.min_value for x in self.params.values()],
                          up=[x.max_value for x in self.params.values()], indpb=0.5)
         toolbox.register("select", tools.selTournament, tournsize=4)
         toolbox.register("evaluate", self.evaluate_clf)
@@ -338,16 +347,16 @@
         self.optimization_logger.info("LOGBOOK: \n{}".format(self.logbook))
         self.optimization_logger.info("HALL OF FAME: {} individuals".format(len(hof)))
 
         for i in range(len(hof)):
             best_score = hof[i].fitness.values[:]
             self.optimization_logger.info("Individual TOP {}".format(i + 1))
             self.optimization_logger.info("Individual accuracy: {}".format(best_score))
-            self.optimization_logger.info("Best classifier: {}".format(str(self.get_corrected_clf(hof[i]))))
-            self.optimization_logger.info("Params: {}".format(str(self.get_corrected_clf(hof[i]).get_params())))
+            self.optimization_logger.info("Best classifier: {}".format(str(self.get_clf(hof[i]))))
+            self.optimization_logger.info("Params: {}".format(str(self.get_clf(hof[i]).get_params())))
 
         # self.file_out.write("LOGBOOK: \n"+str(logbook)+"\n")
         # self.file_out.write("Best accuracy: "+str(best_score[0])+"\n")
         # self.file_out.write("Best classifier(without parameter formating(DECIMALS)): "+str(self.get_clf(hof[0])))
         self._write_population_file()
         self._write_logbook_file()
         # self.plot_logbook(logbook=logbook)
@@ -358,15 +367,15 @@
         g.savefig(os.path.join(self.graphics_path, "search_space.png"))
         plt.close()
 
         g2 = plot_logbook(self.logbook)
         g2.savefig(os.path.join(self.graphics_path, "logbook.png"))
         plt.close()
 
-        return self.get_corrected_clf(hof[0])
+        return self.get_clf(hof[0])
 
     def custom_ea_simple(self, population, toolbox, logbook,
                          cxpb, mutpb, start_gen=0, ngen=4, checkpoint_path=None, stats=None,
                          halloffame=None, verbose=__debug__, checkpoint_flag=True):
         """This algorithm reproduce the simplest evolutionary algorithm as
         presented in chapter 7 of [Back2000]_.
 
@@ -429,30 +438,46 @@
         if checkpoint_flag and (checkpoint_path is None or not os.path.isdir(checkpoint_path)):
             error_msg = "checkpoint_flag is True and checkpoint_path {} " \
                         "is not a folder or does not exist".format(checkpoint_path)
             self.optimization_logger.error(error_msg)
             raise NotADirectoryError(error_msg)
 
         # Begin the generational process
+
         for gen in range(start_gen, ngen + 1):
+            progress_gen_path = os.path.join(self.progress_path, "Generation_{}.csv".format(gen))
+            progress_gen_file = open(progress_gen_path, "w")
+            header_progress_gen_file = "i;total;time(s);Individual;fitness\n"
+            progress_gen_file.write(header_progress_gen_file)
             self.optimization_logger.info("Generation: {}".format(gen))
             # Vary the pool of individuals
             population = varAnd(population, toolbox, cxpb, mutpb)
 
             # Evaluate the individuals with an invalid fitness
             invalid_ind = [ind for ind in population if not ind.fitness.valid]
             fitnesses = toolbox.map(toolbox.evaluate, invalid_ind)
             c = 1
+            evaluations_pending = len(invalid_ind)
             for ind, fit in zip(invalid_ind, fitnesses):
                 self.optimization_logger.info(
-                    "Fitting individual (informational purpose): gen {} - ind {}".format(
-                        gen, c
+                    "Fitting individual (informational purpose): gen {} - ind {} of {}".format(
+                        gen, c, evaluations_pending
                     )
                 )
+                t0_evaluation = time.time()
                 ind.fitness.values = fit
+                t1_evaluation = time.time()
+                t_evaluation = t1_evaluation - t0_evaluation
+                ind_formatted = self.individual2dict(ind)
+                progress_gen_file.write(
+                    "{};{};{};{};{}\n".format(c,
+                                              evaluations_pending,
+                                              t_evaluation,
+                                              ind_formatted, fit)
+                )
                 c = c + 1
 
             halloffame.update(population)
 
             record = stats.compile(population) if stats else {}
 
             logbook.record(gen=gen, nevals=len(invalid_ind), **record)
@@ -462,28 +487,31 @@
             # Select the next generation individuals
             population = toolbox.select(population, len(population))
 
             for i in range(len(halloffame[:2])):
                 best_score = halloffame[i].fitness.values[:]
                 self.optimization_logger.info("Individual TOP {}".format(i + 1))
                 self.optimization_logger.info("Individual accuracy: {}".format(best_score))
-                self.optimization_logger.info("Best classifier: {}".format(str(self.get_corrected_clf(halloffame[i]))))
+                self.optimization_logger.info("Best classifier: {}".format(str(self.get_clf(halloffame[i]))))
                 self.optimization_logger.info(
-                    "Params: {}".format(str(self.get_corrected_clf(halloffame[i]).get_params())))
+                    "Params: {}".format(str(self.get_clf(halloffame[i]).get_params())))
 
             # Store the space param and fitness for each
             self.populations.append([[ind, ind.fitness] for ind in population])
 
             if checkpoint_flag:
                 # Fill the dictionary using the dict(key=value[, ...]) constructor
                 cp = dict(population=population, generation=gen, halloffame=halloffame,
                           logbook=logbook, rndstate=random.getstate())
 
                 cp_file = os.path.join(checkpoint_path, "cp_gen_{}.pkl".format(gen))
                 joblib.dump(cp, cp_file)
+            self._write_population_file()
+            self._write_logbook_file()
+            progress_gen_file.close()
 
         return population, logbook, halloffame
 
 
 class TreeOptimizer(BaseOptimizer, ABC):
     """
     Concrete optimizer for sklearn classifier -> sklearn.tree.DecisionTreeClassifier
```

### Comparing `mloptimizer-0.5.6/mloptimizer/miscellaneous.py` & `mloptimizer-0.5.7/mloptimizer/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/mloptimizer/model_evaluation.py` & `mloptimizer-0.5.7/mloptimizer/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/mloptimizer/plots.py` & `mloptimizer-0.5.7/mloptimizer/plots.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/mloptimizer/test/test_TreeOptimizer.py` & `mloptimizer-0.5.7/mloptimizer/test/test_TreeOptimizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     return TreeOptimizer(X, y, custom_params=custom_params)
 
 
 @pytest.fixture
 def custom_fixed_params_tree_optimizer():
     fixed_params = {
         "max_depth": 4,
+        "min_samples_split": 10
     }
     X, y = load_iris(return_X_y=True)
     return TreeOptimizer(X, y, custom_fixed_params=fixed_params)
 
 
 # Test vanilla TreeOptimizer
 # Test custom parameters TreeOptimizer
@@ -48,22 +49,28 @@
 
 
 def test_custom_tree_optimizer_get_params(custom_params_tree_optimizer):
     assert custom_params_tree_optimizer.get_params() != custom_params_tree_optimizer.get_default_params()
 
 
 def test_custom_fixed_tree_optimizer_get_params(custom_fixed_params_tree_optimizer):
-    assert custom_fixed_params_tree_optimizer.get_params() != custom_fixed_params_tree_optimizer.get_default_params()
+    custom_p = custom_fixed_params_tree_optimizer.get_params()
+    default_p = custom_fixed_params_tree_optimizer.get_default_params()
+    assert custom_p != default_p
 
 
 def test_create_tree_optimizer(default_tree_optimizer):
     assert os.path.isdir(default_tree_optimizer.get_folder()) and os.path.exists(default_tree_optimizer.get_log_file())
     shutil.rmtree(default_tree_optimizer.get_folder())
 
 
+def test_create_custom_fixed_params_tree_optimizer(custom_fixed_params_tree_optimizer):
+    custom_fixed_params_tree_optimizer.optimize_clf(8, 10)
+
+
 def test_create_tree_optimizer2(default_tree_optimizer2):
     assert os.path.isdir(default_tree_optimizer2.get_folder()) and os.path.exists(
         default_tree_optimizer2.get_log_file())
     shutil.rmtree(default_tree_optimizer2.get_folder())
 
 
 def test_tree_optimizer_get_params(default_tree_optimizer):
```

### Comparing `mloptimizer-0.5.6/mloptimizer/test/test_alg_wrapper.py` & `mloptimizer-0.5.7/mloptimizer/test/test_alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/mloptimizer/test/test_genoptimizer.py` & `mloptimizer-0.5.7/mloptimizer/test/test_genoptimizer.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/mloptimizer/test/test_param.py` & `mloptimizer-0.5.7/mloptimizer/test/test_param.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,7 +40,12 @@
     assert nexp_param.correct(11) == 0.0000000001
 
 
 def test_x10_param_correct(x10_param):
     assert x10_param.correct(5) == 50
     assert x10_param.correct(-1) == 0
     assert x10_param.correct(11) == 100
+
+
+def test_str_float_param(float_param):
+    float_param_str = str(float_param)
+    assert float_param_str == "Param('float_param', 1, 200, float, 100)"
```

### Comparing `mloptimizer-0.5.6/mloptimizer.egg-info/PKG-INFO` & `mloptimizer-0.5.7/mloptimizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.5.6
+Version: 0.5.7
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mloptimizer-0.5.6/mloptimizer.egg-info/SOURCES.txt` & `mloptimizer-0.5.7/mloptimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.6/setup.py` & `mloptimizer-0.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     name="mloptimizer",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.5.6",  # Required
+    version="0.5.7",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="mloptimizer is a Python library "
                 "for optimizing hyperparameters of machine learning algorithms using genetic algorithms.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
```

