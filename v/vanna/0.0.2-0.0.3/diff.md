# Comparing `tmp/vanna-0.0.2.tar.gz` & `tmp/vanna-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.0.2.tar", last modified: Wed Jun 21 20:17:00 2023, max compression
+gzip compressed data, was "vanna-0.0.3.tar", last modified: Fri Jun 23 19:25:50 2023, max compression
```

## Comparing `vanna-0.0.2.tar` & `vanna-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:17:00.824407 vanna-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 20:16:48.000000 vanna-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-21 20:17:00.824407 vanna-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 20:16:48.000000 vanna-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-21 20:16:48.000000 vanna-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:17:00.824407 vanna-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:17:00.820407 vanna-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:17:00.824407 vanna-0.0.2/src/vanna/
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-21 20:16:48.000000 vanna-0.0.2/src/vanna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-21 20:16:48.000000 vanna-0.0.2/src/vanna/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:17:00.824407 vanna-0.0.2/src/vanna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-21 20:17:00.000000 vanna-0.0.2/src/vanna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-21 20:17:00.000000 vanna-0.0.2/src/vanna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:17:00.000000 vanna-0.0.2/src/vanna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 20:17:00.000000 vanna-0.0.2/src/vanna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 20:17:00.000000 vanna-0.0.2/src/vanna.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:25:50.081479 vanna-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 19:25:40.000000 vanna-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-23 19:25:50.081479 vanna-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 19:25:40.000000 vanna-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-23 19:25:40.000000 vanna-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:25:50.081479 vanna-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:25:50.081479 vanna-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:25:50.081479 vanna-0.0.3/src/vanna/
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-23 19:25:40.000000 vanna-0.0.3/src/vanna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-23 19:25:40.000000 vanna-0.0.3/src/vanna/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:25:50.081479 vanna-0.0.3/src/vanna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-23 19:25:50.000000 vanna-0.0.3/src/vanna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-23 19:25:50.000000 vanna-0.0.3/src/vanna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:25:50.000000 vanna-0.0.3/src/vanna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 19:25:50.000000 vanna-0.0.3/src/vanna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 19:25:50.000000 vanna-0.0.3/src/vanna.egg-info/top_level.txt
```

### Comparing `vanna-0.0.2/LICENSE` & `vanna-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vanna-0.0.2/PKG-INFO` & `vanna-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vanna-0.0.2/pyproject.toml` & `vanna-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vanna"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vanna-0.0.2/src/vanna/__init__.py` & `vanna-0.0.3/src/vanna/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     if 'result' not in d:
         return False
     
     status = Status(**d['result'])
 
     return status.success
 
-def generate_sql(question: str) -> str | None:
+def generate_sql(question: str) -> str:
     """
     Generate an SQL query using the Vanna.AI API.
 
     Args:
         question (str): The question to generate an SQL query for.
 
     Returns:
@@ -161,15 +161,15 @@
         return None
 
     # Load the result into a dataclass
     sql_answer = SQLAnswer(**d['result'])
 
     return sql_answer.sql
 
-def generate_plotly_code(question: str | None, sql: str | None, df: pd.DataFrame) -> str | None:
+def generate_plotly_code(question: Union[str, None], sql: Union[str, None], df: pd.DataFrame) -> str:
     """
     Generate Plotly code using the Vanna.AI API.
 
     Args:
         question (str): The question to generate Plotly code for.
         sql (str): The SQL query to generate Plotly code for.
         df (pd.DataFrame): The dataframe to generate Plotly code for.
@@ -191,15 +191,15 @@
         return None
 
     # Load the result into a dataclass
     plotly_code = PlotlyResult(**d['result'])
 
     return plotly_code.plotly_code
 
-def get_plotly_figure(plotly_code: str, df: pd.DataFrame, dark_mode: bool = True) -> plotly.graph_objs.Figure | None:
+def get_plotly_figure(plotly_code: str, df: pd.DataFrame, dark_mode: bool = True) -> plotly.graph_objs.Figure:
     """
     Get a Plotly figure from a dataframe and Plotly code.
 
     Args:
         df (pd.DataFrame): The dataframe to use.
         plotly_code (str): The Plotly code to use.
 
@@ -219,52 +219,50 @@
 
     return fig
 
 def get_results(cs, default_database: str, sql: str) -> pd.DataFrame:
     """
     Get the results of an SQL query using the Vanna.AI API.
 
-    :param cs: The Snowflake cursor to use.
-    :type cs: snowflake.connector.cursor.SnowflakeCursor
-    :param default_database: The default database to use (executed as "USE DATABASE {default_database};")
-    :type default_database: str
-    :param sql: The SQL query to run.
-    :type sql: str
-    
-    :return: The results of the SQL query.
-    :rtype: pd.DataFrame
+    Args:
+        cs (pyodbc.Cursor): The cursor to use.
+        default_database (str): The default database to use.
+        sql (str): The SQL query to execute.
+
+    Returns:
+        pd.DataFrame: The results of the SQL query.
     """
     cs.execute(f"USE DATABASE {default_database}")
 
     cur = cs.execute(sql)
 
     results = cur.fetchall()
         
     # Create a pandas dataframe from the results
     df = pd.DataFrame(results, columns=[desc[0] for desc in cur.description])
 
     return df
 
 
-def generate_explanation(sql: str) -> str | None:
+def generate_explanation(sql: str) -> str:
     """
 
     ## Example
     ```python
     vn.generate_explanation(sql="SELECT * FROM students WHERE name = 'John Doe'")
     # 'AI Response'
     ```
     
     Generate an explanation of an SQL query using the Vanna.AI API.
 
-    :param sql: The SQL query to explain.
-    :type sql: str
-
-    :return: The explanation of the SQL query, or None if an error occurred.
-    :rtype: str or None
+    Args:
+        sql (str): The SQL query to generate an explanation for.
+    
+    Returns:
+        str or None: The explanation, or None if an error occurred.
 
     """
     params = [SQLAnswer(
         raw_answer="",
         prefix="",
         postfix="",
         sql=sql,
@@ -275,7 +273,42 @@
     if 'result' not in d:
         return None
 
     # Load the result into a dataclass
     explanation = Explanation(**d['result'])
 
     return explanation.explanation
+
+def generate_question(sql: str) -> str:
+    """
+
+    ## Example
+    ```python
+    vn.generate_question(sql="SELECT * FROM students WHERE name = 'John Doe'")
+    # 'AI Response'
+    ```
+    
+    Generate a question from an SQL query using the Vanna.AI API.
+
+    Args:
+        sql (str): The SQL query to generate a question for.
+    
+    Returns:
+        str or None: The question, or None if an error occurred.
+
+    """
+    params = [SQLAnswer(
+        raw_answer="",
+        prefix="",
+        postfix="",
+        sql=sql,
+    )]
+
+    d = __rpc_call(method="generate_question", params=params)
+
+    if 'result' not in d:
+        return None
+
+    # Load the result into a dataclass
+    question = Question(**d['result'])
+
+    return question.question
```

### Comparing `vanna-0.0.2/src/vanna/types.py` & `vanna-0.0.3/src/vanna/types.py`

 * *Files identical despite different names*

### Comparing `vanna-0.0.2/src/vanna.egg-info/PKG-INFO` & `vanna-0.0.3/src/vanna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

