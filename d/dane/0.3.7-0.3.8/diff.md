# Comparing `tmp/dane-0.3.7.tar.gz` & `tmp/dane-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dane-0.3.7.tar", max compression
+gzip compressed data, was "dane-0.3.8.tar", max compression
```

## Comparing `dane-0.3.7.tar` & `dane-0.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2022-12-20 11:50:37.871142 dane-0.3.7/LICENSE
--rw-r--r--   0        0        0     2362 2022-12-20 11:50:37.871142 dane-0.3.7/README.md
--rw-r--r--   0        0        0      245 2023-06-19 12:18:27.536564 dane-0.3.7/dane/__init__.py
--rw-r--r--   0        0        0    14243 2023-06-19 12:18:27.536564 dane-0.3.7/dane/base_classes.py
--rw-r--r--   0        0        0     4478 2023-06-19 14:20:12.773557 dane-0.3.7/dane/config.py
--rw-r--r--   0        0        0     5679 2022-12-20 11:50:37.871142 dane-0.3.7/dane/document.py
--rw-r--r--   0        0        0     2187 2022-12-20 11:50:37.871142 dane-0.3.7/dane/errors.py
--rw-r--r--   0        0        0     4858 2023-06-19 12:18:27.536564 dane-0.3.7/dane/es_queries.py
--rw-r--r--   0        0        0    39686 2023-06-19 12:18:27.536564 dane-0.3.7/dane/handlers/ESHandler.py
--rw-r--r--   0        0        0     4335 2023-06-19 12:18:27.536564 dane-0.3.7/dane/handlers/RabbitMQHandler.py
--rw-r--r--   0        0        0      213 2022-12-20 11:50:37.871142 dane-0.3.7/dane/handlers/__init__.py
--rw-r--r--   0        0        0     9821 2023-06-19 12:18:27.536564 dane-0.3.7/dane/handlers/base_handler.py
--rw-r--r--   0        0        0     3770 2022-12-20 11:50:37.871142 dane-0.3.7/dane/results.py
--rw-r--r--   0        0        0     1883 2023-06-19 14:20:12.773557 dane-0.3.7/dane/s3_util.py
--rw-r--r--   0        0        0     1384 2023-06-19 12:18:27.536564 dane-0.3.7/dane/state.py
--rw-r--r--   0        0        0     9860 2023-06-19 12:18:27.536564 dane-0.3.7/dane/tasks.py
--rw-r--r--   0        0        0     1357 2022-12-20 11:50:37.871142 dane-0.3.7/dane/utils.py
--rw-r--r--   0        0        0     1836 2023-06-20 13:31:55.983683 dane-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 dane-0.3.7/setup.py
--rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 dane-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-12-20 11:50:37.871142 dane-0.3.8/LICENSE
+-rw-r--r--   0        0        0     2362 2022-12-20 11:50:37.871142 dane-0.3.8/README.md
+-rw-r--r--   0        0        0      245 2023-06-19 12:18:27.536564 dane-0.3.8/dane/__init__.py
+-rw-r--r--   0        0        0    14589 2023-06-23 07:10:50.684841 dane-0.3.8/dane/base_classes.py
+-rw-r--r--   0        0        0     4478 2023-06-19 14:20:12.773557 dane-0.3.8/dane/config.py
+-rw-r--r--   0        0        0     5679 2022-12-20 11:50:37.871142 dane-0.3.8/dane/document.py
+-rw-r--r--   0        0        0     2187 2022-12-20 11:50:37.871142 dane-0.3.8/dane/errors.py
+-rw-r--r--   0        0        0     4858 2023-06-19 12:18:27.536564 dane-0.3.8/dane/es_queries.py
+-rw-r--r--   0        0        0    39686 2023-06-19 12:18:27.536564 dane-0.3.8/dane/handlers/ESHandler.py
+-rw-r--r--   0        0        0     4335 2023-06-19 12:18:27.536564 dane-0.3.8/dane/handlers/RabbitMQHandler.py
+-rw-r--r--   0        0        0      213 2022-12-20 11:50:37.871142 dane-0.3.8/dane/handlers/__init__.py
+-rw-r--r--   0        0        0     9821 2023-06-19 12:18:27.536564 dane-0.3.8/dane/handlers/base_handler.py
+-rw-r--r--   0        0        0     3770 2022-12-20 11:50:37.871142 dane-0.3.8/dane/results.py
+-rw-r--r--   0        0        0     1883 2023-06-19 14:20:12.773557 dane-0.3.8/dane/s3_util.py
+-rw-r--r--   0        0        0     1384 2023-06-19 12:18:27.536564 dane-0.3.8/dane/state.py
+-rw-r--r--   0        0        0     9860 2023-06-19 12:18:27.536564 dane-0.3.8/dane/tasks.py
+-rw-r--r--   0        0        0     1357 2022-12-20 11:50:37.871142 dane-0.3.8/dane/utils.py
+-rw-r--r--   0        0        0     1836 2023-06-23 07:01:49.285214 dane-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 dane-0.3.8/setup.py
+-rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 dane-0.3.8/PKG-INFO
```

### Comparing `dane-0.3.7/LICENSE` & `dane-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/README.md` & `dane-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/base_classes.py` & `dane-0.3.8/dane/base_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -313,46 +313,52 @@
                 correlation_id=props.correlation_id, delivery_mode=2
             ),
             body=json.dumps(response),  # convert to string
         )
 
         ch.basic_ack(delivery_tag=method.delivery_tag)
 
-    def getDirs(self, document):
+    def getDirs(self, document, create_input_dir=True, create_output_dir=True):
         """This function returns the TEMP and OUT directories for this job
         creating them if they do not yet exist
         output should be stored in response['SHARED']
 
         :param job: The job
         :type job: :class:`Job`
         :return: Dict with keys `TEMP_FOLDER` and `OUT_FOLDER`
         :rtype: dict
         """
-        logger.info("Generating TEMP_FOLDER and OUT_FOLDER")
+        logger.info(
+            f"Generating TEMP_FOLDER (auto create={create_input_dir}) and OUT_FOLDER (auto create={create_output_dir})"
+        )
         # expect that TEMP and OUT folder exist
         TEMP_SOURCE = self.config.PATHS.TEMP_FOLDER
         OUT_SOURCE = self.config.PATHS.OUT_FOLDER
 
-        if not os.path.exists(TEMP_SOURCE):
-            os.mkdir(TEMP_SOURCE)
-        if not os.path.exists(OUT_SOURCE):
-            os.mkdir(OUT_SOURCE)
-
         # Get a more specific path name, by chunking id into (at most)
         # three chunks of 2 characters
         chunks = os.path.join(
             *[document._id[i : 2 + i] for i in range(0, min(len(document._id), 6), 2)]
         )
         TEMP_DIR = os.path.join(TEMP_SOURCE, chunks, document._id)
         OUT_DIR = os.path.join(OUT_SOURCE, chunks, document._id)
 
-        if not os.path.exists(TEMP_DIR):
-            os.makedirs(TEMP_DIR)
-        if not os.path.exists(OUT_DIR):
-            os.makedirs(OUT_DIR)
+        if create_input_dir:
+            logger.info(f"Creating input dir: {TEMP_DIR}")
+            if not os.path.exists(TEMP_SOURCE):
+                os.mkdir(TEMP_SOURCE)
+            if not os.path.exists(TEMP_DIR):
+                os.makedirs(TEMP_DIR)
+
+        if create_output_dir:
+            logger.info(f"Creating output dir: {OUT_DIR}")
+            if not os.path.exists(OUT_SOURCE):
+                os.mkdir(OUT_SOURCE)
+            if not os.path.exists(OUT_DIR):
+                os.makedirs(OUT_DIR)
 
         return {"TEMP_FOLDER": TEMP_DIR, "OUT_FOLDER": OUT_DIR}
 
     @abstractmethod
     def callback(self, task, document):
         """Function containing the core functionality that is specific to
         a worker.
```

### Comparing `dane-0.3.7/dane/config.py` & `dane-0.3.8/dane/config.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/document.py` & `dane-0.3.8/dane/document.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/errors.py` & `dane-0.3.8/dane/errors.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/es_queries.py` & `dane-0.3.8/dane/es_queries.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/handlers/ESHandler.py` & `dane-0.3.8/dane/handlers/ESHandler.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/handlers/RabbitMQHandler.py` & `dane-0.3.8/dane/handlers/RabbitMQHandler.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/handlers/base_handler.py` & `dane-0.3.8/dane/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/results.py` & `dane-0.3.8/dane/results.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/s3_util.py` & `dane-0.3.8/dane/s3_util.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/state.py` & `dane-0.3.8/dane/state.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/tasks.py` & `dane-0.3.8/dane/tasks.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/dane/utils.py` & `dane-0.3.8/dane/utils.py`

 * *Files identical despite different names*

### Comparing `dane-0.3.7/pyproject.toml` & `dane-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DANE"
-version = "0.3.7"
+version = "0.3.8"
 description = "Utils for working with the Distributed Annotation and Enrichment system"
 readme = "README.md"
 authors = [
     "Nanne van Noord <n.j.e.vannoord@uva.nl>",
     "jblom <jblom@beeldengeluid.nl>"
 ]
 license = "Apache License 2.0"
```

### Comparing `dane-0.3.7/setup.py` & `dane-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pika>=1.3.1,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'urllib3>=1.26.12,<2.0.0',
  'yacs>=0.1.8,<0.2.0']
 
 setup_kwargs = {
     'name': 'dane',
-    'version': '0.3.7',
+    'version': '0.3.8',
     'description': 'Utils for working with the Distributed Annotation and Enrichment system',
     'long_description': "# DANE\nThe Distributed Annotation 'n' Enrichment (DANE) system handles compute task assignment and file storage for the automatic annotation of content.\n\nThis repository contains contains the building blocks for with DANE, such as creating custom analysis workers or submitting new task.\n\n## Installation\n\nThis package can be installed through pip:\n\n    pip install dane\n\n### Configuration\n\nDANE components are configured through the dane.config module, which is described here: https://dane.readthedocs.io/en/latest/intro.html#configuration \nIt is however noteable that, because all DANE components are expected to rely on it, some of the DANE-server, ElasticSearch and RabbitMQ configuration \nare included in the default config. As such it is recommended that you create a `$HOME/.dane/config.yml` or `$DANE_HOME/config.yml` which contain machine-wide settings for how to connect to these services, which involves specifying the following settings:\n\n```\nDANE:\n    API_URL: 'http://localhost:5500/DANE/'\n    MANAGE_URL: 'http://localhost:5500/manage/'\nRABBITMQ:\n    HOST: 'localhost'\n    PORT: 5672\n    EXCHANGE: 'DANE-exchange'\n    RESPONSE_QUEUE: 'DANE-response-queue'\n    USER: 'guest'\n    PASSWORD: 'guest'\nELASTICSEARCH:\n    HOST: ['localhost']\n    PORT: 9200\n    USER: 'elastic'\n    PASSWORD: 'changeme'\n    SCHEME: 'http'\n    INDEX: 'your_dane_index'\n```\n\nThe values given here are the default values.\n\n### Usage\n\nExamples of how to use DANE can be found in the `examples/` directory.\n\n## Local Development\n\nWe moved from `setup.py` & `requirements.txt` to a single `pyproject.toml`. For local builds and publishing we use [poetry](https://python-poetry.org/).\n\nFor local installation:\n\n```bash\npoetry install\npoetry shell\n```\n\nAfter installation the following unit test should succeed:\n\n```bash\npython -m test.test_dane\n```\n\nTo build a wheel + source package (will end up in `dist` directory):\n\n```bash\npoetry build\n```\n\nThe wheel can be conveniently tested in e.g. your own DANE worker by installing it e.g. using `pip`:\n\n```bash\npip install path_to_dane_wheel_file\n```\n\nor with poetry\n\n```bash\npoetry add path_to_dane_wheel_file\n```\n\n### Breaking changes after 0.3.1 \n\nSince version 0.3.1 DANE must be imported in lowercase letters:\n\n```python\nimport dane\n```\n\nBefore version 0.3.1 you should import using uppercase letters:\n\n```python\nimport DANE\n```",
     'author': 'Nanne van Noord',
     'author_email': 'n.j.e.vannoord@uva.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CLARIAH/DANE',
```

### Comparing `dane-0.3.7/PKG-INFO` & `dane-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dane
-Version: 0.3.7
+Version: 0.3.8
 Summary: Utils for working with the Distributed Annotation and Enrichment system
 Home-page: https://github.com/CLARIAH/DANE
 License: Apache-2.0
 Author: Nanne van Noord
 Author-email: n.j.e.vannoord@uva.nl
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

