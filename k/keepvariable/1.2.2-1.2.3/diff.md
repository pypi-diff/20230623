# Comparing `tmp/keepvariable-1.2.2.tar.gz` & `tmp/keepvariable-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepvariable-1.2.2.tar", last modified: Mon Jun 19 02:42:09 2023, max compression
+gzip compressed data, was "keepvariable-1.2.3.tar", last modified: Fri Jun 23 13:33:14 2023, max compression
```

## Comparing `keepvariable-1.2.2.tar` & `keepvariable-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 02:42:09.804723 keepvariable-1.2.2/
--rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     2146 2023-06-19 02:42:09.804723 keepvariable-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 02:42:09.785774 keepvariable-1.2.2/keepvariable/
--rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.2.2/keepvariable/__init__.py
--rw-rw-rw-   0        0        0    23249 2023-06-19 02:41:49.000000 keepvariable-1.2.2/keepvariable/keepvariable_core.py
--rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.2.2/keepvariable/keepvariable_model.py
--rw-rw-rw-   0        0        0     1684 2023-05-25 15:03:40.000000 keepvariable-1.2.2/keepvariable/kv_redis_example.py
-drwxrwxrwx   0        0        0        0 2023-06-19 02:42:09.803725 keepvariable-1.2.2/keepvariable.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-06-19 02:42:09.000000 keepvariable-1.2.2/keepvariable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-06-19 02:42:09.000000 keepvariable-1.2.2/keepvariable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 02:42:09.000000 keepvariable-1.2.2/keepvariable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 02:42:09.000000 keepvariable-1.2.2/keepvariable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-19 02:42:09.000000 keepvariable-1.2.2/keepvariable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 02:42:09.804723 keepvariable-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-06-19 02:41:53.000000 keepvariable-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:33:14.194908 keepvariable-1.2.3/
+-rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2146 2023-06-23 13:33:14.194908 keepvariable-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 13:33:14.174961 keepvariable-1.2.3/keepvariable/
+-rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.2.3/keepvariable/__init__.py
+-rw-rw-rw-   0        0        0    24705 2023-06-23 13:26:36.000000 keepvariable-1.2.3/keepvariable/keepvariable_core.py
+-rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.2.3/keepvariable/keepvariable_model.py
+-rw-rw-rw-   0        0        0     1684 2023-05-25 15:03:40.000000 keepvariable-1.2.3/keepvariable/kv_redis_example.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:33:14.193910 keepvariable-1.2.3/keepvariable.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-06-23 13:33:13.000000 keepvariable-1.2.3/keepvariable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-06-23 13:33:14.000000 keepvariable-1.2.3/keepvariable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 13:33:13.000000 keepvariable-1.2.3/keepvariable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-23 13:33:13.000000 keepvariable-1.2.3/keepvariable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-23 13:33:13.000000 keepvariable-1.2.3/keepvariable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 13:33:14.194908 keepvariable-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-06-23 13:33:10.000000 keepvariable-1.2.3/setup.py
```

### Comparing `keepvariable-1.2.2/LICENSE` & `keepvariable-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `keepvariable-1.2.2/PKG-INFO` & `keepvariable-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.2.2/README.md` & `keepvariable-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `keepvariable-1.2.2/keepvariable/keepvariable_core.py` & `keepvariable-1.2.3/keepvariable/keepvariable_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,36 @@
             item.elements.pop(index)
 
     def __str__(self):
         return str(self.elements)
 
 
 class AbstractKeepVariableServer(ABC):
+    def _json_serialize_dataframe(self, df:pd.DataFrame) -> str:
+        """Takes a pandas DataFrame and serialized it to a json-like string.
+        The function uses pd.DataFrame().to_json() approach so as to handle various variable types with ease (pd.NA, pd.NaT, datetime etc.)
+
+        Example:
+            input: df2 = pd.DataFrame([[1,datetime.datetime.now(),3],[4,5,pd.NA],[pd.NaT,8,None]])
+            output: {"columns": [0, 1, 2], "data": [[1, 1685402664424, 3], [4, 5, null], [null, 8, null]], "object_type": "pd.DataFrame", "attrs": {}}'
+
+        Args:
+            df (pd.DataFrame): DataFrame to be serialized
+
+        Returns:
+            str: DataFrame serialized into json-like string
+        """        
+        df_json = df.to_json(orient='split')
+        df_as_dict = json.loads(df_json)
+        df_as_dict["object_type"] = 'pd.DataFrame'
+        df_as_dict["attrs"] = df.attrs
+        df_json = json.dumps(df_as_dict)
+        
+        return df_json
+
     def parse_saved_value(self, value, additional_params: Optional[dict] = None):
         """
         Parse enterted value to json format. Certain special type values are serialized (DFs, datetimes, functions, classes).
 
         :param value: Entered value of any type (not all types can get serialized and stored however!)
         :type value: Any
         :param additional_params: Additional parameters used for serialization, e.g. for a function variable it's
@@ -163,23 +185,26 @@
         if additional_params is None:
             additional_params = {}
 
         if isinstance(value, list) or isinstance(value,
                                                  bool) or isinstance(value, dict):
             value = json.dumps(value)
         elif isinstance(value, pd.DataFrame):
-            data = value.values.tolist()
-            columns = list(value.columns)
-            final_data = {
-                "columns": columns,
-                "data": data,
-                "object_type": "pd.DataFrame",
-            }
-            print(final_data)
-            value = json.dumps(final_data)
+            value = self._json_serialize_dataframe(value)
+            # Old implementation
+            # TODO: Keep for now, delete in following commits
+            # data = value.values.tolist()
+            # columns = list(value.columns)
+            # final_data = {
+            #     "columns": columns,
+            #     "data": data,
+            #     "object_type": "pd.DataFrame",
+            # }
+            # print(final_data)
+            # value = json.dumps(final_data)
         elif isinstance(value, np.ndarray):
             data = value.tolist()
             final_data = {"data": data, "object_type": "np.ndarray"}
             value = json.dumps(final_data)
 
         elif isinstance(value, datetime.datetime):
             data = value.strftime("%Y-%m-%d %H:%M:%S")
@@ -252,15 +277,15 @@
         pass
 
     @abstractmethod
     def query(
         self, *, text_params: Optional[dict[str, tuple]] = None,
         tag_params: Optional[dict[str, tuple]] = None,
         field_to_sort_by: Optional[str] = None, asc=True, **kwargs
-    ) -> list[tuple]:
+    ) ->  dict[str, dict]:
         """Query KeepVariable store - explanations are in abstract subclasses docstrings."""
         pass
 
     # Implemented, but currently not used
     @abstractmethod
     def arrlen(self, name: str, path: str) -> Optional[int]:
         """
@@ -344,63 +369,63 @@
                 element[last_element][last_index] = value
             else:
                 element[last_element] = value
 
     def query(
         self,
         *,
-        text_params: dict[str, tuple] = None,
-        tag_params: dict[str, tuple] = None,
+        text_params: Optional[dict[str, tuple]] = None,
+        tag_params: Optional[dict[str, tuple]] = None,
         name: str,
         field_to_sort_by: Optional[str] = None,
         asc=True,
         **kwargs,
-    ) -> list[tuple]:
+    ) -> dict[str, dict]:
         """
         Simplified alternative to RedisSearch. Allows to search and sort by values of specified fields.
 
         :param text_params: key name to a tuple of values mapping, e.g. {'status': ('pipel', ...), ...}
         :type text_params: dict[str, tuple]
         :param tag_params: key name to a tuple of values mapping, e.g. {'status': ('QUEUED', ...), ...}
         :type tag_params: dict[str, tuple]
         :param sort_by_name: attribute name by which results should be sorted
         :type sort_by_name: str
         :return: [('jobs:43', job_dict), ...]
         :rtype: list[tuple]
         """
-        found_jobs: list[tuple] = [
-            (job_name, value)
+        found_jobs: dict[str, dict] = {
+            job_name: value
             for job_name, value in self.storage.items()
             if name in job_name
-        ]  # [('jobs:43', job_dict), ...]
+          }  # {'jobs:43': job_dict, ...}
 
         # TAG search
         if tag_params is not None:
             for field, values in tag_params.items():
-                found_jobs = [
-                    job for job in found_jobs
-                    if job[1].get(field) and job[1].get(field) in values
-                ]
+                found_jobs = {
+                    job_id: job for job_id, job in found_jobs.items()
+                    if job.get(field) and job.get(field) in values
+                }
 
         # TEXT search
         if text_params is not None:
             for field, values in text_params.items():
                 for value in values:
-                    # E.g. value = "QUEU", job[1].get(field) = "QUEUED"
-                    found_jobs = [
-                        job for job in found_jobs
-                        if job[1].get(field) and value in job[1].get(field)
-                    ]
+                    # E.g. value = "QUEU", job.get(field) = "QUEUED"
+                    found_jobs = {
+                        job_id: job for job_id, job in found_jobs.items()
+                        if job.get(field) and value in job.get(field)
+                    }
 
         if field_to_sort_by:
-            found_jobs = sorted(found_jobs, key=lambda x: x[1][field_to_sort_by])
+            found_jobs_list = sorted(found_jobs.items(), key=lambda x: x[1][field_to_sort_by])
         if not asc:
-            found_jobs.reverse()
+            found_jobs_list.reverse()
 
-        return found_jobs
+        return dict(found_jobs_list)
 
     def arrlen(self, name: str, path: str) -> Optional[int]:
         try:
             element, last_element, last_index = self._extract_object_from_path(
                 name, path
             )
             if last_index:
@@ -551,51 +576,53 @@
                 pipe.json().set(name, json_xpath, value)
             pipe.execute()
 
     def query(
         self, *, text_params: Optional[dict[str, tuple]] = None,
         tag_params: Optional[dict[str, tuple]] = None, index_name: str,
         field_to_sort_by: Optional[str] = None, asc=True, **kwargs
-    ) -> list[tuple]:
+    ) -> dict[str, dict]:
         """
         Simplified wrapper to RedisSearch. Allows to search and sort by a value of Redis TAG/TEXT fields.
         Simplistic on purpose, to avoid bloat. Additional functionality should be added in case of need.
 
         :param text_params: key name to a tuple of values mapping, e.g. {'status': ('pipel', ...), ...}
         :type text_params: dict[str, tuple]
         :param tag_params: key name to a tuple of values mapping, e.g. {'status': ('QUEUED', ...), ...}
         :type tag_params: dict[str, tuple]
         :param index_name: name of the Redis index used for querying
         :type index_name: str
         :param field_to_sort_by: attribute name by which results should be sorted, defaults to None
         :type field_to_sort_by: Optional[str], optional
         :param asc: True if sort in ascending order, defaults to True
         :type asc: bool, optional
-        :return: [('jobs:43', job_json), ...]
-        :rtype: list[str]
+        :return: {'jobs:43': job_json, ...}
+        :rtype: dict[str, dict]
         """
         final_query = ""
 
         if text_params is not None:
-            text_query_template = "{field}:{value}"
+            text_query_template = "@{field}:{value}"
             for field, values in text_params.items():
                 value_str = "|".join(values)
                 final_query += text_query_template.format(field=field, value=value_str)
 
         if tag_params is not None:
             tag_query_template = "@{field}:{{{value}}}"
             for field, values in tag_params.items():
                 value_str = "|".join(values)
                 final_query += tag_query_template.format(field=field, value=value_str)
 
+        # Query example: "@type:PIPEL @status:{QUEUED|COMPLETED}"
+        # Explanation: find all jobs with type field containing 'PIPEL' and status being either 'QUEUED' or 'COMPLETED'
         query_object = Query(final_query)
         if field_to_sort_by:
             query_object.sort_by(field_to_sort_by, asc=asc)
-        job_docs: list = self.redis.ft(index_name).search(query_object).docs
 
-        return [(job_doc.id, job_doc.json) for job_doc in job_docs]
+        job_docs: list = self.redis.ft(index_name).search(query_object).docs
+        return {job_doc.id: job_doc.json for job_doc in job_docs}
 
     def arrlen(self, name: str, path: str) -> Optional[int]:
         return self.redis.json().arrlen(name, path).pop()
 
     def arrappend(self, name: str, path: str, objects: Sequence) -> Optional[int]:
         return self.redis.json().arrappend(name, path, *objects).pop()
```

### Comparing `keepvariable-1.2.2/keepvariable/kv_redis_example.py` & `keepvariable-1.2.3/keepvariable/kv_redis_example.py`

 * *Files identical despite different names*

### Comparing `keepvariable-1.2.2/keepvariable.egg-info/PKG-INFO` & `keepvariable-1.2.3/keepvariable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.2.2/setup.py` & `keepvariable-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='keepvariable',
-    version='1.2.2',
+    version='1.2.3',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='A Python package keeping the values of variables between separate runs in a seamless and effortless way.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/keepvariable',
     packages=setuptools.find_packages(),
```

