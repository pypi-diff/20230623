# Comparing `tmp/kumo-ai-0.1.7.tar.gz` & `tmp/kumo-ai-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kumo-ai-0.1.7.tar", last modified: Thu May 25 21:18:30 2023, max compression
+gzip compressed data, was "kumo-ai-0.1.8.tar", last modified: Fri Jun 23 03:33:46 2023, max compression
```

## Comparing `kumo-ai-0.1.7.tar` & `kumo-ai-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 21:18:30.912098 kumo-ai-0.1.7/
--rw-r--r--   0 siyang     (501) staff       (20)     1800 2023-02-27 18:06:46.000000 kumo-ai-0.1.7/.gitignore
--rw-r--r--   0 siyang     (501) staff       (20)      933 2023-03-17 21:55:08.000000 kumo-ai-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 siyang     (501) staff       (20)     1061 2023-02-23 21:09:43.000000 kumo-ai-0.1.7/LICENSE
--rw-r--r--   0 siyang     (501) staff       (20)      194 2023-05-25 20:14:27.000000 kumo-ai-0.1.7/Makefile
--rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-25 21:18:30.911940 kumo-ai-0.1.7/PKG-INFO
--rw-r--r--   0 siyang     (501) staff       (20)       39 2023-02-23 21:09:43.000000 kumo-ai-0.1.7/README.md
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 21:18:30.909299 kumo-ai-0.1.7/kumo_ai.egg-info/
--rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-25 21:18:30.000000 kumo-ai-0.1.7/kumo_ai.egg-info/PKG-INFO
--rw-r--r--   0 siyang     (501) staff       (20)      722 2023-05-25 21:18:30.000000 kumo-ai-0.1.7/kumo_ai.egg-info/SOURCES.txt
--rw-r--r--   0 siyang     (501) staff       (20)        1 2023-05-25 21:18:30.000000 kumo-ai-0.1.7/kumo_ai.egg-info/dependency_links.txt
--rw-r--r--   0 siyang     (501) staff       (20)       34 2023-05-25 21:18:30.000000 kumo-ai-0.1.7/kumo_ai.egg-info/requires.txt
--rw-r--r--   0 siyang     (501) staff       (20)        7 2023-05-25 21:18:30.000000 kumo-ai-0.1.7/kumo_ai.egg-info/top_level.txt
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 21:18:30.909541 kumo-ai-0.1.7/kumoai/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.7/kumoai/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)    15118 2023-05-25 17:33:50.000000 kumo-ai-0.1.7/kumoai/client.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 21:18:30.910208 kumo-ai-0.1.7/kumoai/datamodel/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.7/kumoai/datamodel/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)      974 2023-04-03 17:42:04.000000 kumo-ai-0.1.7/kumoai/datamodel/data_source.py
--rw-r--r--   0 siyang     (501) staff       (20)     6537 2023-05-25 20:37:19.000000 kumo-ai-0.1.7/kumoai/datamodel/jobs.py
--rw-r--r--   0 siyang     (501) staff       (20)      561 2023-04-05 16:11:01.000000 kumo-ai-0.1.7/kumoai/datamodel/json_serde.py
--rw-r--r--   0 siyang     (501) staff       (20)     6471 2023-05-24 04:53:09.000000 kumo-ai-0.1.7/kumoai/datamodel/pquery.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 21:18:30.911760 kumo-ai-0.1.7/kumoai/examples/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-03-29 16:49:40.000000 kumo-ai-0.1.7/kumoai/examples/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)     4807 2023-05-18 17:13:05.000000 kumo-ai-0.1.7/kumoai/examples/financial.py
--rw-r--r--   0 siyang     (501) staff       (20)     8950 2023-05-12 16:27:03.000000 kumo-ai-0.1.7/kumoai/examples/financial_binary_classify_S3.json
--rw-r--r--   0 siyang     (501) staff       (20)     9339 2023-04-04 17:45:36.000000 kumo-ai-0.1.7/kumoai/examples/financial_binary_classify_SNOWFLAKE.json
--rw-r--r--   0 siyang     (501) staff       (20)     5373 2023-03-29 17:21:11.000000 kumo-ai-0.1.7/kumoai/examples/hm_churn.json
--rw-r--r--   0 siyang     (501) staff       (20)     3080 2023-05-18 17:13:05.000000 kumo-ai-0.1.7/kumoai/examples/orchestration.py
--rw-r--r--   0 siyang     (501) staff       (20)     3434 2023-05-18 17:13:05.000000 kumo-ai-0.1.7/kumoai/examples/save_load_modify_pquery.py
--rw-r--r--   0 siyang     (501) staff       (20)      967 2023-05-18 17:51:43.000000 kumo-ai-0.1.7/precommit-pyrightconfig.json
--rw-r--r--   0 siyang     (501) staff       (20)      924 2023-05-18 17:52:10.000000 kumo-ai-0.1.7/pyrightconfig.json
--rw-r--r--   0 siyang     (501) staff       (20)       38 2023-05-25 21:18:30.912136 kumo-ai-0.1.7/setup.cfg
--rw-r--r--   0 siyang     (501) staff       (20)      885 2023-05-25 21:18:11.000000 kumo-ai-0.1.7/setup.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-06-23 03:33:46.696894 kumo-ai-0.1.8/
+-rw-r--r--   0 siyang     (501) staff       (20)     1800 2023-02-27 18:06:46.000000 kumo-ai-0.1.8/.gitignore
+-rw-r--r--   0 siyang     (501) staff       (20)      933 2023-03-17 21:55:08.000000 kumo-ai-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 siyang     (501) staff       (20)     1061 2023-02-23 21:09:43.000000 kumo-ai-0.1.8/LICENSE
+-rw-r--r--   0 siyang     (501) staff       (20)      194 2023-05-25 20:14:27.000000 kumo-ai-0.1.8/Makefile
+-rw-r--r--   0 siyang     (501) staff       (20)      482 2023-06-23 03:33:46.696755 kumo-ai-0.1.8/PKG-INFO
+-rw-r--r--   0 siyang     (501) staff       (20)       39 2023-02-23 21:09:43.000000 kumo-ai-0.1.8/README.md
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-06-23 03:33:46.694876 kumo-ai-0.1.8/kumo_ai.egg-info/
+-rw-r--r--   0 siyang     (501) staff       (20)      482 2023-06-23 03:33:46.000000 kumo-ai-0.1.8/kumo_ai.egg-info/PKG-INFO
+-rw-r--r--   0 siyang     (501) staff       (20)      722 2023-06-23 03:33:46.000000 kumo-ai-0.1.8/kumo_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 siyang     (501) staff       (20)        1 2023-06-23 03:33:46.000000 kumo-ai-0.1.8/kumo_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 siyang     (501) staff       (20)       34 2023-06-23 03:33:46.000000 kumo-ai-0.1.8/kumo_ai.egg-info/requires.txt
+-rw-r--r--   0 siyang     (501) staff       (20)        7 2023-06-23 03:33:46.000000 kumo-ai-0.1.8/kumo_ai.egg-info/top_level.txt
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-06-23 03:33:46.695115 kumo-ai-0.1.8/kumoai/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.8/kumoai/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)    15118 2023-05-25 17:33:50.000000 kumo-ai-0.1.8/kumoai/client.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-06-23 03:33:46.695719 kumo-ai-0.1.8/kumoai/datamodel/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.8/kumoai/datamodel/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)      974 2023-04-03 17:42:04.000000 kumo-ai-0.1.8/kumoai/datamodel/data_source.py
+-rw-r--r--   0 siyang     (501) staff       (20)     6537 2023-05-25 20:37:19.000000 kumo-ai-0.1.8/kumoai/datamodel/jobs.py
+-rw-r--r--   0 siyang     (501) staff       (20)      561 2023-04-05 16:11:01.000000 kumo-ai-0.1.8/kumoai/datamodel/json_serde.py
+-rw-r--r--   0 siyang     (501) staff       (20)     6473 2023-06-23 03:31:27.000000 kumo-ai-0.1.8/kumoai/datamodel/pquery.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-06-23 03:33:46.696582 kumo-ai-0.1.8/kumoai/examples/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-03-29 16:49:40.000000 kumo-ai-0.1.8/kumoai/examples/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)     4836 2023-06-23 03:32:38.000000 kumo-ai-0.1.8/kumoai/examples/financial.py
+-rw-r--r--   0 siyang     (501) staff       (20)     8952 2023-06-23 03:32:04.000000 kumo-ai-0.1.8/kumoai/examples/financial_binary_classify_S3.json
+-rw-r--r--   0 siyang     (501) staff       (20)     9341 2023-06-23 03:32:04.000000 kumo-ai-0.1.8/kumoai/examples/financial_binary_classify_SNOWFLAKE.json
+-rw-r--r--   0 siyang     (501) staff       (20)     5375 2023-06-23 03:32:04.000000 kumo-ai-0.1.8/kumoai/examples/hm_churn.json
+-rw-r--r--   0 siyang     (501) staff       (20)     3080 2023-05-18 17:13:05.000000 kumo-ai-0.1.8/kumoai/examples/orchestration.py
+-rw-r--r--   0 siyang     (501) staff       (20)     3436 2023-06-23 03:31:27.000000 kumo-ai-0.1.8/kumoai/examples/save_load_modify_pquery.py
+-rw-r--r--   0 siyang     (501) staff       (20)      967 2023-05-18 17:51:43.000000 kumo-ai-0.1.8/precommit-pyrightconfig.json
+-rw-r--r--   0 siyang     (501) staff       (20)      924 2023-05-18 17:52:10.000000 kumo-ai-0.1.8/pyrightconfig.json
+-rw-r--r--   0 siyang     (501) staff       (20)       38 2023-06-23 03:33:46.696942 kumo-ai-0.1.8/setup.cfg
+-rw-r--r--   0 siyang     (501) staff       (20)      885 2023-06-23 03:33:15.000000 kumo-ai-0.1.8/setup.py
```

### Comparing `kumo-ai-0.1.7/.gitignore` & `kumo-ai-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/.pre-commit-config.yaml` & `kumo-ai-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/LICENSE` & `kumo-ai-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/kumo_ai.egg-info/SOURCES.txt` & `kumo-ai-0.1.8/kumo_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/kumoai/client.py` & `kumo-ai-0.1.8/kumoai/client.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/kumoai/datamodel/data_source.py` & `kumo-ai-0.1.8/kumoai/datamodel/data_source.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/kumoai/datamodel/jobs.py` & `kumo-ai-0.1.8/kumoai/datamodel/jobs.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/kumoai/datamodel/json_serde.py` & `kumo-ai-0.1.8/kumoai/datamodel/json_serde.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/kumoai/datamodel/pquery.py` & `kumo-ai-0.1.8/kumoai/datamodel/pquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,14 @@
 
 
 @dataclass
 class PQueryResource:
     """Predictive Query resource definition."""
     name: str
 
-    query_yaml: str
+    query_string: str
 
     graph: GraphDefinition
 
     graph_display_name: Optional[str] = None
 
     advanced_options_yaml: Optional[str] = None
```

### Comparing `kumo-ai-0.1.7/kumoai/examples/financial.py` & `kumo-ai-0.1.8/kumoai/examples/financial.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,16 @@
             ColumnKey(table_name='ORDERS', col_name='ACCOUNT_ID'),
             ColumnKey(table_name='TRANS', col_name='ACCOUNT_ID'),
         ]))
     pquery = PQueryResource(
         name=pquery_name,
         graph=graph,
         graph_display_name=f'financial_graph_{data_source_type}',
-        query_yaml="entity: TRANS.TRANS_ID\ntarget: TRANS.K_SYMBOL = 'DUCHOD'")
+        query_string=("entity: TRANS.TRANS_ID\n"
+                      "target: TRANS.K_SYMBOL = 'DUCHOD'"))
 
     query_json_file_path = os.path.join(
         os.path.dirname(os.path.realpath(__file__)), f'{pquery.name}.json')
     with open(query_json_file_path, 'w') as file:
         file.write(to_json(pquery))
         logger.info('Saved %s to file: %s', pquery.name, query_json_file_path)
```

### Comparing `kumo-ai-0.1.7/kumoai/examples/financial_binary_classify_S3.json` & `kumo-ai-0.1.8/kumoai/examples/financial_binary_classify_S3.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {"'query_string'": '"entity: TRANS.TRANS_ID\\ntarget: TRANS.K_SYMBOL = \'DUCHOD\'"',*

 * * 'delete': "['query_yaml']"}*

```diff
@@ -379,9 +379,9 @@
                 "table_type": "fact",
                 "time_col": "DATE"
             }
         }
     },
     "graph_display_name": "financial_graph_S3",
     "name": "financial_binary_classify_S3",
-    "query_yaml": "entity: TRANS.TRANS_ID\ntarget: TRANS.K_SYMBOL = 'DUCHOD'"
+    "query_string": "entity: TRANS.TRANS_ID\ntarget: TRANS.K_SYMBOL = 'DUCHOD'"
 }
```

### Comparing `kumo-ai-0.1.7/kumoai/examples/financial_binary_classify_SNOWFLAKE.json` & `kumo-ai-0.1.8/kumoai/examples/financial_binary_classify_SNOWFLAKE.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {"'query_string'": '"entity: TRANS.TRANS_ID\\ntarget: TRANS.K_SYMBOL = \'DUCHOD\'"',*

 * * 'delete': "['query_yaml']"}*

```diff
@@ -395,9 +395,9 @@
                 "table_type": "fact",
                 "time_col": "DATE"
             }
         }
     },
     "graph_display_name": "financial_graph_SNOWFLAKE",
     "name": "financial_binary_classify_SNOWFLAKE",
-    "query_yaml": "entity: TRANS.TRANS_ID\ntarget: TRANS.K_SYMBOL = 'DUCHOD'"
+    "query_string": "entity: TRANS.TRANS_ID\ntarget: TRANS.K_SYMBOL = 'DUCHOD'"
 }
```

### Comparing `kumo-ai-0.1.7/kumoai/examples/hm_churn.json` & `kumo-ai-0.1.8/kumoai/examples/hm_churn.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {"'query_string'": "'entity: customers.customer_id\\ntemporal_entity_filter: "*

 * *                   'COUNT(transactions_train.price, -60, 0) > 0\\ntarget: '*

 * *                   "COUNT(transactions_train.price, 0, 30) = 0'",*

 * * 'delete': "['query_yaml']"}*

```diff
@@ -211,9 +211,9 @@
                 "sql": null,
                 "time_col": "t_dat"
             }
         }
     },
     "graph_display_name": null,
     "name": "hm_churn",
-    "query_yaml": "entity: customers.customer_id\ntemporal_entity_filter: COUNT(transactions_train.price, -60, 0) > 0\ntarget: COUNT(transactions_train.price, 0, 30) = 0"
+    "query_string": "entity: customers.customer_id\ntemporal_entity_filter: COUNT(transactions_train.price, -60, 0) > 0\ntarget: COUNT(transactions_train.price, 0, 30) = 0"
 }
```

### Comparing `kumo-ai-0.1.7/kumoai/examples/orchestration.py` & `kumo-ai-0.1.8/kumoai/examples/orchestration.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/kumoai/examples/save_load_modify_pquery.py` & `kumo-ai-0.1.8/kumoai/examples/save_load_modify_pquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
     This example demonstrates how we can start from an existing predictive
     query, make a few changes, and create a new query.
     """
     # Example 1: reuse the same graph, but write a different query yaml
     query1 = kumo_client.get_pquery('hm_churn')
     query1.name = "hm_ltv"
-    query1.query_yaml = """
+    query1.query_string = """
 entity: customers.customer_id\nwhatif: COUNT(transactions_train.*, 0, 90)
  > 0\ntarget: SUM(transactions_train.price, 0, 90) = 0
 """
     # Create the new pquery in Kumo Cloud
     kumo_client.create_pquery(query1)
     run_training_job(query1.name)  # Launch training for the new query!
```

### Comparing `kumo-ai-0.1.7/precommit-pyrightconfig.json` & `kumo-ai-0.1.8/precommit-pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/pyrightconfig.json` & `kumo-ai-0.1.8/pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.7/setup.py` & `kumo-ai-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'Kumo.ai Client SDK'
 LONG_DESCRIPTION = """
 SDK/API for Kumo.ai clients to allow programmatic access to Kumo.ai
 """
 
 install_requires = [
     "pydantic==1.10.4",
```

