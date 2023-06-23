# Comparing `tmp/speedracer-0.0.2.tar.gz` & `tmp/speedracer-0.0.3.tar.gz`

## Comparing `speedracer-0.0.2.tar` & `speedracer-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    15855 2020-02-02 00:00:00.000000 speedracer-0.0.2/src/speedracer/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 speedracer-0.0.2/LICENSE
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 speedracer-0.0.2/README.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 speedracer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 speedracer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    15931 2020-02-02 00:00:00.000000 speedracer-0.0.3/src/speedracer/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 speedracer-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 speedracer-0.0.3/README.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 speedracer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 speedracer-0.0.3/PKG-INFO
```

### Comparing `speedracer-0.0.2/src/speedracer/__init__.py` & `speedracer-0.0.3/src/speedracer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         # get HTTP headers dictionary with an Authorization header set
         headers = manager.get_headers()
 
         # get your Common Name
         name = manager.get_cn()
         ```
     """
-    def __init__(self, url:str, cert:Tuple[str, str]=(Path.home().joinpath('cert.crt'),
-            Path.home().joinpath('cert.key')),
+    def __init__(self, url:str, cert:Tuple[str, str]=(Path.home().joinpath('.ssh/cert.crt'),
+            Path.home().joinpath('.ssh/cert.key')),
             verify:Union[str, bool]=True) -> None:
         '''Create a JWT Manager
 
         Arguments:
             url: The URL of the API Gateway to fetch JWTs from
             cert: A Tuple containing the paths to the certificate and
                 key to use with the API Gateway. By default, looks in the
@@ -119,16 +119,16 @@
 class Offset(str, Enum):
     '''The offset to start consuming messages from'''
     BEGIN = 'begin'
     NOW = 'now'
 
 class Connection:
     '''Connect to the Mission Data Broker (MDB)'''
-    def __init__(self, url:str, cert:Tuple[str, str]=(Path.home().joinpath('/.ssh/cert.crt'),
-                Path.home().joinpath('/.ssh/cert.key')),
+    def __init__(self, url:str, cert:Tuple[str, str]=(Path.home().joinpath('.ssh/cert.crt'),
+                Path.home().joinpath('.ssh/cert.key')),
             ca_bundle:Optional[str]=None) -> None:
         '''
         Example:
             ```python
             conn = Connection('https://mdb-account-server/')
             ```
 
@@ -347,14 +347,16 @@
                 await sub.seek(datetime.datetime.utcnow() -
                     datetime.timedelta(minutes=5))
                 ```
 
             Arguments:
                 seq_or_datetime: Sequence number or datetime to seek to
             '''
+            start_sequence = None
+            start_datetime = None
             if isinstance(seq_or_datetime, int):
                 start_sequence = seq_or_datetime
             elif isinstance(seq_or_datetime, datetime.datetime):
                 start_datetime = seq_or_datetime
             else:
                 raise TypeError("seek to argument must be int or datetime")
             await self.__psub.unsubscribe()
```

### Comparing `speedracer-0.0.2/LICENSE` & `speedracer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `speedracer-0.0.2/README.md` & `speedracer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `speedracer-0.0.2/PKG-INFO` & `speedracer-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedracer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Conveniently access data
 Author: RRC
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

