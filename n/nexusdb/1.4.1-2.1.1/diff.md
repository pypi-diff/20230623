# Comparing `tmp/nexusdb-1.4.1.tar.gz` & `tmp/nexusdb-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexusdb-1.4.1.tar", last modified: Fri Jun 23 10:42:49 2023, max compression
+gzip compressed data, was "nexusdb-2.1.1.tar", last modified: Fri Jun 23 21:11:45 2023, max compression
```

## Comparing `nexusdb-1.4.1.tar` & `nexusdb-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:42:49.975408 nexusdb-1.4.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:42:49.975408 nexusdb-1.4.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.4.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:42:49.975408 nexusdb-1.4.1/nexus/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2023-06-23 10:33:24.000000 nexusdb-1.4.1/nexus/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26342 2023-06-23 10:41:36.000000 nexusdb-1.4.1/nexus/main.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:42:49.975408 nexusdb-1.4.1/nexusdb.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-23 10:42:49.975408 nexusdb-1.4.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1088 2023-06-23 10:42:28.000000 nexusdb-1.4.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 21:11:45.212666 nexusdb-2.1.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 21:11:45.212666 nexusdb-2.1.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-2.1.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 21:11:45.208668 nexusdb-2.1.1/nexus/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2023-06-23 10:33:24.000000 nexusdb-2.1.1/nexus/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34895 2023-06-23 21:04:49.000000 nexusdb-2.1.1/nexus/main.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 21:11:45.208668 nexusdb-2.1.1/nexusdb.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 21:11:45.000000 nexusdb-2.1.1/nexusdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2023-06-23 21:11:45.000000 nexusdb-2.1.1/nexusdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-23 21:11:45.000000 nexusdb-2.1.1/nexusdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2023-06-23 21:11:45.000000 nexusdb-2.1.1/nexusdb.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-23 21:11:45.000000 nexusdb-2.1.1/nexusdb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-06-23 21:11:45.000000 nexusdb-2.1.1/nexusdb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-23 21:11:45.212666 nexusdb-2.1.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1088 2023-06-23 21:05:06.000000 nexusdb-2.1.1/setup.py
```

### Comparing `nexusdb-1.4.1/PKG-INFO` & `nexusdb-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.4.1
+Version: 2.1.1
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.4.1/nexus/main.py` & `nexusdb-2.1.1/nexus/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.logs_path = os.path.join(self.db_path, 'logs', 'logs.json')
         logs_dir = os.path.join(self.db_path, 'logs')
         if not os.path.exists(logs_dir):
             os.makedirs(logs_dir)
 
         self.config = {}
        
-    def set_app_mode(self, mode):
+    def set_app(self, mode):
         BOLD_RED = "\033[91m"
         RESET_COLOR = "\033[0m"
         if mode.lower() not in ["production", "development"]:
             raise ValueError(f"{BOLD_RED}Invalid app mode. Choose either 'Production' or 'Development'.{RESET_COLOR}")
         self.config['APP_MODE'] = mode.lower()
 
         if mode.lower() == "production":
@@ -41,33 +41,33 @@
                     os.chmod(os.path.join(root, dir), 0o444)
         elif mode.lower() == "development":
             BOLD_RED = "\033[91m"
             BOLD_YELLOW = "\033[93m"
             RESET_COLOR = "\033[0m"
             BOLD_WHITE = "\033[97m"
             current_date_time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            message = f"{BOLD_WHITE}Development mode enabled - 127.0.0.1:37017 [{current_date_time}] \n"
+            message = f"{BOLD_WHITE}Development mode enabled - 127.0.0.1:3717 [{current_date_time}] \n"
             message += f"{BOLD_RED}* NexusClient['production'] -- Restart with stat{RESET_COLOR} \n"
             message += f"{BOLD_YELLOW}* DEBUGGER ID: {uuid.uuid4()} {RESET_COLOR}\n"
-            message += f"{BOLD_WHITE}* CONNECTION: 127.0.0.1:37017 connected{RESET_COLOR}\n"
-            message += f"{BOLD_RED}Note: For production usage use db.config['APP_MODE'] == 'production' v.1.2.0 {RESET_COLOR}\n"
+            message += f"{BOLD_WHITE}* CONNECTION: 127.0.0.1:3717 connected{RESET_COLOR}\n"
+            message += f"{BOLD_RED}Note: For production usage use db.config['APP_MODE'] == 'production' v.2.1.1 {RESET_COLOR}\n"
             message += f"{BOLD_YELLOW}Version control by NexusDB @2023 JsonComponents{RESET_COLOR}\n"
             message += f"{BOLD_WHITE}output: {RESET_COLOR}"
             print(message)
                
     def connect(self, connection_url):
         BOLD_RED = "\033[91m"
         RESET_COLOR = "\033[0m"
         parsed_url = urlparse(connection_url)
 
-        if parsed_url.scheme != "nexusdb":
-            raise ValueError(f"{BOLD_RED}Invalid connection URL. Scheme must be 'nexusdb'.{RESET_COLOR}")
+        if parsed_url.scheme != "nexus":
+            raise ValueError(f"{BOLD_RED}Invalid connection URL. Scheme must be 'nexus'.{RESET_COLOR}")
 
         if parsed_url.netloc != "localhost:3717":
-            raise ValueError(f"{BOLD_RED}Invalid connection URL. Host must be 'localhost' and port must be '3717'.{RESET_COLOR}")
+            raise ValueError(f"{BOLD_RED}Invalid connection URL. invalid host and port use deafult host 'localhost' and port '3717'.{RESET_COLOR}")
 
         query_params = parse_qs(parsed_url.query)
         if "rsa_id" not in query_params or "encryption" not in query_params:
             raise ValueError(f"{BOLD_RED}Invalid connection URL. 'rsa_id' and 'encryption' query parameters are required.{RESET_COLOR}")
 
         email, password = self._extract_email_password(parsed_url.path)
         rsa_id = query_params["rsa_id"][0]
@@ -598,8 +598,204 @@
                     with open(compact_file_path, 'w') as f:
                         json.dump(data, f, separators=(',', ':'))
         shutil.rmtree(self.db_path)
         shutil.move(compact_db_path, self.db_path)
         print('Database compacted successfully.')
         self._log_action('compact_database')
         
-    
+    @check_authentication 
+    def insert_many(self, collection_name, documents):
+        for document in documents:
+            self.insert(collection_name, document)
+
+    @check_authentication 
+    def update_many(self, collection_name, query, update_data):
+        collection_path = os.path.join(self.db_path, collection_name)
+        for filename in os.listdir(collection_path):
+            if filename.endswith('.json'):
+                document_path = os.path.join(collection_path, filename)
+                with open(document_path, 'r') as f:
+                    document = json.load(f)
+                    if all(item in document.items() for item in query.items()):
+                        document.update(update_data)
+                        with open(document_path, 'w') as f:
+                            json.dump(document, f)
+
+    @check_authentication 
+    def delete_many(self, collection_name, query):
+        collection_path = os.path.join(self.db_path, collection_name)
+        for filename in os.listdir(collection_path):
+            if filename.endswith('.json'):
+                document_path = os.path.join(collection_path, filename)
+                with open(document_path, 'r') as f:
+                    document = json.load(f)
+                    if all(item in document.items() for item in query.items()):
+                        os.remove(document_path)
+
+    @check_authentication 
+    def aggregate(self, collection_name, pipeline):
+        collection_path = os.path.join(self.db_path, collection_name)
+        documents = []
+        for filename in os.listdir(collection_path):
+            if filename.endswith('.json'):
+                document_path = os.path.join(collection_path, filename)
+                with open(document_path, 'r') as f:
+                    document = json.load(f)
+                    documents.append(document)
+
+        for stage in pipeline:
+            if stage.get('$match'):
+                match_query = stage['$match']
+                documents = [doc for doc in documents if all(item in doc.items() for item in match_query.items())]
+            elif stage.get('$sort'):
+                sort_query = stage['$sort']
+                key = list(sort_query.keys())[0]
+                reverse = sort_query[key] == -1
+                documents = sorted(documents, key=lambda doc: doc.get(key), reverse=reverse)
+            elif stage.get('$limit'):
+                limit = stage['$limit']
+                documents = documents[:limit]
+
+        return documents
+
+    @check_authentication 
+    def distinct(self, collection_name, field):
+        collection_path = os.path.join(self.db_path, collection_name)
+        values = set()
+        for filename in os.listdir(collection_path):
+            if filename.endswith('.json'):
+                document_path = os.path.join(collection_path, filename)
+                with open(document_path, 'r') as f:
+                    document = json.load(f)
+                    value = document.get(field)
+                    if value:
+                        values.add(value)
+        return list(values)
+
+    @check_authentication 
+    def find_one_and_update(self, collection_name, query, update_data):
+        document = self.find_one(collection_name, query)
+        if document:
+            document.update(update_data)
+            return document
+
+    @check_authentication 
+    def find_one_and_delete(self, collection_name, query):
+        document = self.find_one(collection_name, query)
+        if document:
+            collection_path = os.path.join(self.db_path, collection_name)
+            document_path = os.path.join(collection_path, f"{document['document_id']}.json")
+            os.remove(document_path)
+            return document
+
+    @check_authentication 
+    def bulk_write(self, collection_name, operations):
+        for operation in operations:
+            if operation['type'] == 'insert':
+                document = operation['document']
+                self.insert(collection_name, document)
+            elif operation['type'] == 'update':
+                query = operation['query']
+                update_data = operation['update_data']
+                self.update_many(collection_name, query, update_data)
+            elif operation['type'] == 'delete':
+                query = operation['query']
+                self.delete_many(collection_name, query)
+
+    @check_authentication
+    def create_view(self, view_name, collection_name, pipeline):
+        view_path = os.path.join(self.db_path, 'views', view_name)
+        
+        try:
+            os.makedirs(view_path, exist_ok=True)
+            
+            view_pipeline_path = os.path.join(view_path, 'pipeline.json')
+            with open(view_pipeline_path, 'w') as f:
+                json.dump(pipeline, f)
+            
+            print(f"View '{view_name}' has been created successfully.")
+        except FileExistsError:
+            print(f"View '{view_name}' already exists.")
+        except PermissionError:
+            print(f"Permission denied: Unable to create view '{view_name}'.")
+        except Exception as e:
+            print(f"An error occurred while creating view '{view_name}': {str(e)}")
+
+    @check_authentication
+    def rename_collection(self, collection_name, new_collection_name):
+        collection_path = os.path.join(self.db_path, collection_name + ".json")
+        new_collection_path = os.path.join(self.db_path, new_collection_name + ".json")
+
+        try:
+            os.rename(collection_path, new_collection_path)
+            print(f"Collection '{collection_name}' has been renamed to '{new_collection_name}' successfully.")
+        except FileNotFoundError:
+            print(f"Collection '{collection_name}' does not exist.")
+        except FileExistsError:
+            print(f"Collection '{new_collection_name}' already exists.")
+        except PermissionError:
+            print(f"Permission denied: Unable to rename collection '{collection_name}'.")
+        except Exception as e:
+            print(f"An error occurred while renaming collection '{collection_name}': {str(e)}")
+
+    @check_authentication 
+    def aggregate_cursor(self, collection_name, pipeline):
+        collection_path = os.path.join(self.db_path, collection_name)
+        documents = []
+        for filename in os.listdir(collection_path):
+            if filename.endswith('.json'):
+                document_path = os.path.join(collection_path, filename)
+                with open(document_path, 'r') as f:
+                    document = json.load(f)
+                    documents.append(document)
+
+        for stage in pipeline:
+            if stage.get('$match'):
+                match_query = stage['$match']
+                documents = [doc for doc in documents if all(item in doc.items() for item in match_query.items())]
+            elif stage.get('$sort'):
+                sort_query = stage['$sort']
+                key = list(sort_query.keys())[0]
+                reverse = sort_query[key] == -1
+                documents = sorted(documents, key=lambda doc: doc.get(key), reverse=reverse)
+            elif stage.get('$limit'):
+                limit = stage['$limit']
+                documents = documents[:limit]
+
+        for document in documents:
+            yield document
+     
+    @check_authentication        
+    def is_capped(self, collection_name):
+        BOLD_RED = "\033[91m"
+        RESET_COLOR = "\033[0m"
+        collection_path = os.path.join(self.db_path, collection_name + '.json')
+        if not os.path.exists(collection_path):
+            raise ValueError(f'{BOLD_RED}Collection does not exist{RESET_COLOR}')
+        
+        with open(collection_path, 'r') as f:
+            data = json.load(f)
+        
+        if isinstance(data, list):
+            return False
+        elif isinstance(data, dict):
+            return True
+        else:
+            raise ValueError(f'{BOLD_RED}Invalid collection format{RESET_COLOR}')
+        
+    @check_authentication
+    def list_collections(self):
+        collections = []
+        for root, dirs, files in os.walk(self.db_path):
+            for file in files:
+                if file.endswith('.json'):
+                    collection_name = file[:-5]  # Remove the '.json' extension
+                    collections.append(collection_name)
+                    for name in collections:
+                        print (name)
+    
+    @check_authentication
+    def list_databases(self):
+        database_names = os.listdir('database')
+        for name in database_names:
+            print(name)
+
```

### Comparing `nexusdb-1.4.1/nexusdb.egg-info/PKG-INFO` & `nexusdb-2.1.1/nexusdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.4.1
+Version: 2.1.1
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.4.1/setup.py` & `nexusdb-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nexusdb",
-    version="1.4.1",
+    version="2.1.1",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight JSON-based database system for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/nexusdb",
```

