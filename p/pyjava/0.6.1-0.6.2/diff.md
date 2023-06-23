# Comparing `tmp/pyjava-0.6.1.tar.gz` & `tmp/pyjava-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjava-0.6.1.tar", last modified: Wed Jun 14 11:44:58 2023, max compression
+gzip compressed data, was "pyjava-0.6.2.tar", last modified: Fri Jun 23 14:50:16 2023, max compression
```

## Comparing `pyjava-0.6.1.tar` & `pyjava-0.6.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-14 11:44:58.656529 pyjava-0.6.1/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-06-14 11:44:58.656529 pyjava-0.6.1/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      448 2023-04-11 04:53:45.000000 pyjava-0.6.1/README.md
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-14 11:44:58.656529 pyjava-0.6.1/pyjava/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2612 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-14 11:44:58.656529 pyjava-0.6.1/pyjava/api/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      688 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/api/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16024 2023-05-26 04:03:49.000000 pyjava-0.6.1/pyjava/api/mlsql.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4524 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/api/serve.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-14 11:44:58.656529 pyjava-0.6.1/pyjava/cache/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/cache/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      489 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/cache/code_cache.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42222 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/cloudpickle.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7048 2023-04-17 05:24:46.000000 pyjava-0.6.1/pyjava/daemon.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-14 11:44:58.656529 pyjava-0.6.1/pyjava/data/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/data/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1185 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/data/datasource.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-14 11:44:58.656529 pyjava-0.6.1/pyjava/datatype/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/datatype/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    64554 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/datatype/types.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2190 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/rayfix.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30195 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/serializers.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-14 11:44:58.656529 pyjava-0.6.1/pyjava/storage/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/storage/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2825 2023-04-24 06:01:20.000000 pyjava-0.6.1/pyjava/storage/streaming_tar.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-14 11:44:58.656529 pyjava-0.6.1/pyjava/udf/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5888 2023-06-14 11:44:07.000000 pyjava-0.6.1/pyjava/udf/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3916 2023-04-11 04:53:45.000000 pyjava-0.6.1/pyjava/utils.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      828 2023-06-14 11:44:39.000000 pyjava-0.6.1/pyjava/version.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6457 2023-04-18 03:10:44.000000 pyjava-0.6.1/pyjava/worker.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-14 11:44:58.656529 pyjava-0.6.1/pyjava.egg-info/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-06-14 11:44:58.000000 pyjava-0.6.1/pyjava.egg-info/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      596 2023-06-14 11:44:58.000000 pyjava-0.6.1/pyjava.egg-info/SOURCES.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-06-14 11:44:58.000000 pyjava-0.6.1/pyjava.egg-info/dependency_links.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        7 2023-06-14 11:44:58.000000 pyjava-0.6.1/pyjava.egg-info/top_level.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       79 2023-06-14 11:44:58.656529 pyjava-0.6.1/setup.cfg
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2955 2023-04-11 04:53:45.000000 pyjava-0.6.1/setup.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.843610 pyjava-0.6.2/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-06-23 14:50:16.843610 pyjava-0.6.2/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      448 2023-04-11 04:53:45.000000 pyjava-0.6.2/README.md
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.839610 pyjava-0.6.2/pyjava/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2612 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.839610 pyjava-0.6.2/pyjava/api/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      688 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/api/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16024 2023-05-26 04:03:49.000000 pyjava-0.6.2/pyjava/api/mlsql.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4524 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/api/serve.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.839610 pyjava-0.6.2/pyjava/cache/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/cache/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      489 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/cache/code_cache.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42222 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/cloudpickle.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7048 2023-04-17 05:24:46.000000 pyjava-0.6.2/pyjava/daemon.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.843610 pyjava-0.6.2/pyjava/data/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/data/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1185 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/data/datasource.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.843610 pyjava-0.6.2/pyjava/datatype/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/datatype/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    64554 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/datatype/types.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2190 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/rayfix.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30195 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/serializers.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.843610 pyjava-0.6.2/pyjava/storage/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.2/pyjava/storage/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2825 2023-04-24 06:01:20.000000 pyjava-0.6.2/pyjava/storage/streaming_tar.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.843610 pyjava-0.6.2/pyjava/udf/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6176 2023-06-23 14:39:18.000000 pyjava-0.6.2/pyjava/udf/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3990 2023-06-23 13:03:45.000000 pyjava-0.6.2/pyjava/utils.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      828 2023-06-23 14:49:59.000000 pyjava-0.6.2/pyjava/version.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6457 2023-04-18 03:10:44.000000 pyjava-0.6.2/pyjava/worker.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-23 14:50:16.839610 pyjava-0.6.2/pyjava.egg-info/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-06-23 14:50:16.000000 pyjava-0.6.2/pyjava.egg-info/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      596 2023-06-23 14:50:16.000000 pyjava-0.6.2/pyjava.egg-info/SOURCES.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-06-23 14:50:16.000000 pyjava-0.6.2/pyjava.egg-info/dependency_links.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        7 2023-06-23 14:50:16.000000 pyjava-0.6.2/pyjava.egg-info/top_level.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       79 2023-06-23 14:50:16.843610 pyjava-0.6.2/setup.cfg
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2955 2023-04-11 04:53:45.000000 pyjava-0.6.2/setup.py
```

### Comparing `pyjava-0.6.1/PKG-INFO` & `pyjava-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjava
-Version: 0.6.1
+Version: 0.6.2
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyjava-0.6.1/pyjava/__init__.py` & `pyjava-0.6.2/pyjava/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/api/__init__.py` & `pyjava-0.6.2/pyjava/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/api/mlsql.py` & `pyjava-0.6.2/pyjava/api/mlsql.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/api/serve.py` & `pyjava-0.6.2/pyjava/api/serve.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/cloudpickle.py` & `pyjava-0.6.2/pyjava/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/daemon.py` & `pyjava-0.6.2/pyjava/daemon.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/data/datasource.py` & `pyjava-0.6.2/pyjava/data/datasource.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/datatype/types.py` & `pyjava-0.6.2/pyjava/datatype/types.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/rayfix.py` & `pyjava-0.6.2/pyjava/rayfix.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/serializers.py` & `pyjava-0.6.2/pyjava/serializers.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/storage/streaming_tar.py` & `pyjava-0.6.2/pyjava/storage/streaming_tar.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava/udf/__init__.py` & `pyjava-0.6.2/pyjava/udf/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,61 +3,68 @@
 from typing import Any, NoReturn, Callable, Dict, List
 import ray
 from ray.util.client.common import ClientActorHandle, ClientObjectRef
 
 from pyjava.api.mlsql import RayContext
 from pyjava.storage import streaming_tar
 import threading
+from ..utils import print_flush
 
 @ray.remote
 class UDFMaster(object):
     def __init__(self, num: int, conf: Dict[str, str],
                  init_func: Callable[[List[ClientObjectRef], Dict[str, str]], Any],
                  apply_func: Callable[[Any, Any], Any]):
         self.lock = threading.Lock()         
+        self.num = num
+        self.conf = conf
+        self.init_func = init_func
+        self.apply_func = apply_func
+        self.actors = {}
+        self._idle_actors = []
+
+    def create_workers(self, conf):
         udf_worker_conf = {}
 
         if "num_cpus" in conf:
             udf_worker_conf["num_cpus"] = float(conf["num_cpus"])
 
         if "num_gpus" in conf:
             udf_worker_conf["num_gpus"] = float(conf["num_gpus"])
 
         custom_resources = [(key.split("resource.")[1], float(conf[key])) for key in
                             conf.keys() if
                             key.startswith("resource.")]
 
         if len(custom_resources) > 0:
             udf_worker_conf["resources"] = dict(custom_resources)
-                
-        standalone = conf.get("standalone", "false") == "true"
-        
-        model_refs = []
 
         udf_name  = conf["UDF_CLIENT"] if "UDF_CLIENT" in conf else "UNKNOW MODEL"
-                
+        standalone = conf.get("standalone", "false") == "true"
+        model_refs = []
         if "modelServers" in conf and not standalone:
             model_servers = RayContext.parse_servers(conf["modelServers"])  
-            print(f"MODEL[{udf_name}] Transfer model from {model_servers[0].host}:{model_servers[0].port} to Ray Object Store")                       
-            time1 = time.time()
-            items = RayContext.collect_from(model_servers)            
-            for item in items:
-                if len(model_refs) % 5000 == 0:
-                    print(f"MODEL[{udf_name}] Transfer model from {model_servers[0].host}:{model_servers[0].port} to Ray Object Store, current count: {len(model_refs)}")
+            print_flush(f"MODEL[{udf_name}] Transfer model from {model_servers[0].host}:{model_servers[0].port} to Ray Object Store")                       
+            time1 = time.time()            
+            count = 0           
+            for item in RayContext.collect_from(model_servers):
+                if count % 1000 == 0:
+                    print_flush(f"MODEL[{udf_name}] , current count: {count}")
+                count += 1    
                 model_refs.append(ray.put(item))            
             time2 = time.time()
-            print(f"MODEL[{udf_name}] Successful to put the model in Ray, time taken:{time2-time1}s. The total refs: {len(model_refs)}")    
-            
-
+            print_flush(f"MODEL[{udf_name}] Successful to put the model in Ray, time taken:{time2-time1}s. The total refs: {count}") 
+        
         self.actors = dict(
             [(index,
-              UDFWorker.options(**udf_worker_conf).remote(model_refs, conf, init_func,
-                                                          apply_func)) for index in
-             range(num)])
-        self._idle_actors = [index for index in range(num)]
+              UDFWorker.options(**udf_worker_conf).remote(model_refs, conf, self.init_func,
+                                                          self.apply_func)) for index in
+             range(self.num)])
+        self._idle_actors = [index for index in range(self.num)]   
+
 
     def get(self) -> List[Any]:
         while len(self._idle_actors) == 0:
                 time.sleep(0.001)
         with self.lock:            
             index = self._idle_actors.pop()        
         return [index, self.actors[index]]
@@ -76,19 +83,19 @@
                  model_refs: List[ClientObjectRef],
                  conf: Dict[str, str],
                  init_func: Callable[[List[ClientObjectRef], Dict[str, str]], Any],
                  apply_func: Callable[[Any, Any], Any]):
         
         udf_name  = conf["UDF_CLIENT"] if "UDF_CLIENT" in conf else "UNKNOW MODEL"
 
-        print(f"MODEL[{udf_name}] Init Model,It make take a while.")
+        print_flush(f"MODEL[{udf_name}] Init Model,It may take a while.")
         time1 = time.time()
         self.model = init_func(model_refs, conf)
         time2 = time.time()
-        print(f"MODEL[{udf_name}] Successful to init model, time taken:{time2-time1}s")
+        print_flush(f"MODEL[{udf_name}] Successful to init model, time taken:{time2-time1}s")
         self.apply_func = apply_func
 
     def apply(self, v: Any) -> Any:
         return self.apply_func(self.model, v)
 
     def shutdown(self):
         ray.actor.exit_actor()
@@ -120,14 +127,17 @@
         except Exception as inst:
             print(inst)
             pass
                 
         UDFMaster.options(name=udf_name, lifetime="detached",
                           max_concurrency=masterMaxConcurrency).remote(
             max_concurrency, conf, init_func, apply_func)
+        
+        temp_udf_master = ray.get_actor(udf_name)
+        ray.get(temp_udf_master.create_workers.remote(conf))
         ray_context.build_result([])
 
     @staticmethod
     def apply(ray_context: RayContext):
         conf = ray_context.conf()
         udf_name = conf["UDF_CLIENT"]
         udf_master = ray.get_actor(udf_name)
```

### Comparing `pyjava-0.6.1/pyjava/utils.py` & `pyjava-0.6.2/pyjava/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -112,7 +112,10 @@
             return (sockfile, sock)
         except socket.error as e:
             emsg = _exception_message(e)
             errors.append("tried to connect to %s, but an error occured: %s" % (sa, emsg))
             sock.close()
             sock = None
     raise Exception("could not open socket: %s" % errors)
+
+def print_flush(*args, **kwargs):
+    print(*args, **kwargs, flush=True)
```

### Comparing `pyjava-0.6.1/pyjava/version.py` & `pyjava-0.6.2/pyjava/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
```

### Comparing `pyjava-0.6.1/pyjava/worker.py` & `pyjava-0.6.2/pyjava/worker.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/pyjava.egg-info/PKG-INFO` & `pyjava-0.6.2/pyjava.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjava
-Version: 0.6.1
+Version: 0.6.2
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyjava-0.6.1/pyjava.egg-info/SOURCES.txt` & `pyjava-0.6.2/pyjava.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.1/setup.py` & `pyjava-0.6.2/setup.py`

 * *Files identical despite different names*

