# Comparing `tmp/speedracer-0.0.1.tar.gz` & `tmp/speedracer-0.0.2.tar.gz`

## Comparing `speedracer-0.0.1.tar` & `speedracer-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,5 @@
--rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 speedracer-0.0.1/build/lib/speedracer/__init__.py
--rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 speedracer-0.0.1/build/lib/speedracer/connection.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 speedracer-0.0.1/build/lib/speedracer/jwt_manager.py
--rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 speedracer-0.0.1/src/speedracer/__init__.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 speedracer-0.0.1/src/speedracer.egg-info/PKG-INFO
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 speedracer-0.0.1/src/speedracer.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 speedracer-0.0.1/src/speedracer.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 speedracer-0.0.1/src/speedracer.egg-info/requires.txt
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 speedracer-0.0.1/src/speedracer.egg-info/top_level.txt
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 speedracer-0.0.1/LICENSE
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 speedracer-0.0.1/README.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 speedracer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 speedracer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    15855 2020-02-02 00:00:00.000000 speedracer-0.0.2/src/speedracer/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 speedracer-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 speedracer-0.0.2/README.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 speedracer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 speedracer-0.0.2/PKG-INFO
```

### Comparing `speedracer-0.0.1/build/lib/speedracer/__init__.py` & `speedracer-0.0.2/src/speedracer/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,71 +118,67 @@
 
 class Offset(str, Enum):
     '''The offset to start consuming messages from'''
     BEGIN = 'begin'
     NOW = 'now'
 
 class Connection:
-    '''This class holds information for connection to the Mission Data Broker (MDB)'''
-    def __init__(self, url:str, cert:Tuple[str, str]=(Path.home().joinpath('cert.crt'),
-                Path.home().joinpath('cert.key')),
+    '''Connect to the Mission Data Broker (MDB)'''
+    def __init__(self, url:str, cert:Tuple[str, str]=(Path.home().joinpath('/.ssh/cert.crt'),
+                Path.home().joinpath('/.ssh/cert.key')),
             ca_bundle:Optional[str]=None) -> None:
-        '''Create a Connection
-
+        '''
         Example:
             ```python
-            conn = Connection('https://mdb-account-server.com')
+            conn = Connection('https://mdb-account-server/')
             ```
 
         Arguments:
-          url: Base URL of the MDB Acccount Server (MAS)
-          cert: A Tuple containing the paths to the certificate and
-            key to use with the API Gateway. By default, looks in the
-            user's home directory for the files cert.crt and cert.key
-          ca_bundle: A path to a Certificate Authority
+          url: URL of the Autobahn MDB account server
+          cert: Paths to a PEM formated X.509 certificate and key file
+            Defaults to ('$HOME/.ssh/cert.crt', '$HOME/.ssh/cert.key')
+          ca_bundle: A path to a PEM encoded certificate authority file
         '''
         def get_urls():
             config_url = urlparse(url)
             config_url = urlunparse(config_url._replace(path='/api/v1/config'))
             return requests.get(config_url, verify=self.verify, timeout=10).json()
 
         self.cert: Tuple[str, str] = cert
-        '''Certificate path, key path Tuple. Default looks for cert.crt and
-        cert.key in user's home directory'''
+        '''Client certificate. Invalid certificates result in `SSLError`'''
         self.ca_bundle: Optional[str] = ca_bundle
-        '''Path to Certificate Authority'''
+        '''Certificate Authority used to verify server SSL certificates'''
         self.verify: Union[str, bool] = ca_bundle if ca_bundle else True
-        '''Used by requests. Set to value self.ca_bundle if set and True otherwise'''
+        '''Verify server SSL certificates. Set to false if a valid ca_bundle is not available.'''
         self.urls: Dict = get_urls()
-        '''A dict containing URLs to services'''
+        '''URLs to Autobahn services (read-only)'''
         self.jwt_manager: JWTManager = JWTManager(self.urls['api_gateway_url'],
                 cert=cert, verify=self.verify)
         '''A `JWTManager` for authenticating to the MDB'''
         self.subscriptions: List = []
         '''An array of all Subscriptions associated with this Connection'''
 
-    async def subscribe(self, dataset:str, offset:Offset=Offset.BEGIN, batch_size:int=10,
+    async def subscribe(self, dataset:str, offset:Offset=Offset.NOW, batch:int=10,
             callback:Optional[Callable]=None) -> Iterable:
-        '''Subscribe to a data stream. Returns a Subscription which is an Iterable
+        '''Subscribe to a dataset.
 
         Example:
             ```python
             sub = await conn.subscribe('mydataset')
             async for msg in sub:
                 print(msg.data.decode())
             ```
 
         Arguments:
-            dataset: The slug of the dataset to subscribe to
+            dataset: The slug of the dataset
             offset: The offset to start consuming messages from
-            batch_size: The number of messages the client will
-                pull at a time
+            batch: The number of messages retrieved at a time
         '''
         sub = self.Subscription(self.urls, self.jwt_manager, self.ca_bundle,
-                dataset, offset, batch_size, callback)
+                dataset, offset, batch, callback)
         await sub.start()
         self.subscriptions.append(sub)
         return sub
 
     async def close(self):
         '''Close all subscriptions associated with this Connection'''
 
@@ -194,48 +190,47 @@
                 await sub.close()
             except Exception as ex:
                 print('exception closing subscription:', ex)
             self.subscriptions = []
 
 
     class Subscription:
-        '''This class is a subscription to a data stream. Iterable'''
+        '''A subscription to a dataset. Iterable'''
 
         # pylint: disable=too-many-instance-attributes
-        # Seven attributes is not enough
 
         # pylint: disable=too-many-arguments
         # Only called internally so it is fine
 
         def __init__(self, urls:Dict, jwt_manager:JWTManager, ca_bundle:Optional[str],
-                dataset:str, offset:Offset, batch_size:int, callback:Optional[Callable]) -> None:
+                dataset:str, offset:Offset, batch:int, callback:Optional[Callable]) -> None:
             '''Create a subscription. Use a Connection's `subscribe` method instead
 
             Arguments:
                 urls: A Dict containing URLs to services
                 jwt_manager: A `JWTManager` for authenticating to the MDB
                 ca_bundle: Path to a Certificate Authority
                 dataset: The slug of the dataset to subscribe to
                 offset: The offset to start consuming messages from
-                batch_size: The number of messages the client will pull
-                    at a time
+                batch: The number of messages the client will pull at a time
                 callback: A Callable that takes a NATS message as an
                     argument. Called for each messages received
             '''
             self.verify:Union[str, bool] = ca_bundle if ca_bundle else True
-            '''Used by requests. Set to value of ca_bundle if set and True otherwise'''
+            '''Verify server SSL certificates. Set to false if a valid 
+            ca_bundle is not available.'''
             self.urls:Dict = urls
-            '''A Dict containing URLs to services'''
+            '''URLs to Autobahn services (read-only)'''
             self.jwt_manager:JWTManager = jwt_manager
             '''A JWTManager for authenticating to the MDB'''
             self.dataset:str = dataset
             '''The dataset slug for this subscription'''
             self.offset:Offset = offset
             '''The offset to start consuming messages from'''
-            self.batch_size:int = batch_size
+            self.batch:int = batch
             '''Number of messages the subscription will pull at a time'''
             self.callback:Optional[Callable] = callback
             '''Optional callback that takes a NATS message as an argument'''
             self.__ssl_context:ssl.SSLContext = ssl.create_default_context()
             '''SSL context used by aiohttp'''
             if ca_bundle:
                 self.__ssl_context.load_verify_locations(ca_bundle)
@@ -268,30 +263,30 @@
 
             self.subject: str = get_subject()
             '''NATS Subject'''
 
         async def __aiter__(self):
             while True:
                 try:
-                    msgs = await self.__psub.fetch(self.batch_size)
+                    msgs = await self.__psub.fetch(self.batch, timeout=10)
                     for msg in msgs:
                         await msg.ack()
                     for msg in msgs:
                         yield msg
                 except NatsTimeoutError: # no messages to return yet
                     pass
                 except KeyboardInterrupt:
                     break
 
         async def __call_callback(self):
             async for msg in self:
                 self.callback(msg)
 
         async def start(self):
-            '''Start the Subscription. This is called automatically
+            '''Start receiving data from the dataset. This is called automatically
             when using `Connection.subscribe()`'''
             def signature(_):
                 return bytes('', 'UTF-8')
 
             def get_mas_jwt() -> bytearray:
                 resp = requests.get(f"{self.urls['mas_url']}/api/v1/user/jwt/{self.dataset}",
                         headers=self.jwt_manager.get_headers(), verify=self.verify, timeout=10)
@@ -339,42 +334,45 @@
                     subject=self.subject,
                     durable=self.__consumer_name,
                     config=cfg)
 
             if self.callback and not self.__cb_task:
                 self.__cb_task = asyncio.create_task(self.__call_callback())
 
-        async def seek(self, start_sequence=None, start_datetime=None) -> None:
+        async def seek(self, seq_or_datetime: Union[int, datetime.datetime]) -> None:
             '''Move cursor to specified sequence number or datetime
 
             Example:
                 ```python
-                await sub.seek(start_sequence=1)
-                await sub.seek(start_datetime=datetime.datetime.utcnow() -
+                await sub.seek(1)
+                await sub.seek(datetime.datetime.utcnow() -
                     datetime.timedelta(minutes=5))
                 ```
 
             Arguments:
-                start_sequence: The sequence number of the message to seek to
-                start_datetime: The datetime to seek to
+                seq_or_datetime: Sequence number or datetime to seek to
             '''
-            if start_sequence is None and start_datetime is None:
-                return
+            if isinstance(seq_or_datetime, int):
+                start_sequence = seq_or_datetime
+            elif isinstance(seq_or_datetime, datetime.datetime):
+                start_datetime = seq_or_datetime
+            else:
+                raise TypeError("seek to argument must be int or datetime")
             await self.__psub.unsubscribe()
             await self.__delete_consumer()
             await self.__create_sub(start_sequence, start_datetime)
 
         async def __delete_consumer(self) -> bool:
             stream_name = self.subject.replace('.', '_')
             return await self.__js_ctx.delete_consumer(stream_name, self.__consumer_name)
 
         async def wait(self, messages:Union[int, None]=None,
                 timeout:Union[int, datetime.datetime, datetime.timedelta, None]=None) -> None:
-            '''Block until specified number of messages consumed
-            and specified amount of time has elapsed
+            '''Block until specified number of messages are consumed or specified
+            amount of time has elapsed
 
             Example:
                 ```python
                 await sub.wait(messages=15)
                 await sub.wait(timeout=5)
                 ```
```

### Comparing `speedracer-0.0.1/src/speedracer.egg-info/PKG-INFO` & `speedracer-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-Metadata-Version: 2.1
-Name: speedracer
-Version: 0.0.1
-Summary: Conveniently access data
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # What is speedracer?
 
-speedracer provides convenience classes for
+speedracer is an asyncio enabled python library for interacting with Autobahn.
 
-- Subscribing to the Mission Data Broker (MDB)
-- Authenticating to Autobahn APIs
+- Subscribe to datasets available in the Mission Data Broker (MDB)
+- Authenticate with Autobahn APIs
 
 # Quickstart
 
-## Subscribing to the MDB
+## Subscribe to a dataset
 
 To subscribe to a dataset on the MDB
   1. Provide the base URL of the MDB Account Server (MAS) when creating a Connection
   2. Provide the dataset to the subscribe method
 
 ```python
-conn = Connection('https://mdb-account-server.com')
+conn = Connection('https://mdb-account-server/')
 sub = await conn.subscribe('mydataset')
 async for msg in sub:
     print(msg.data.decode())
 ```
 
-## Authenticating to Autobahn APIs
+## Authenticate with Autobahn APIs
 
-To authenticate to Autobahn's REST APIs
-  1. Create a `JWTManager` with the API Gateway's URL
-  2. Call the `get_headers` method to get an Authorization HTTP header
+Autobahn uses JWT credentials for authorization. These tokens are put into the `Authorization`
+header for all HTTPs requests. 
 
-```python
-manager = JWTManager('https://api-gateway.com/getjwt')
-headers = manager.get_headers()
-```
+JWTs are obtained by exchanging private keys with the API Gateway server and
+must be periodically refreshed.
 
-If already subscribed to MDB, you can reuse your `Connection`'s `JWTManager`
+`speedracer` automates the process of fetching JWTs and refreshing them when they expire.
 
 ```python
-conn.jwt_manager.get_headers()
+manager = JWTManager('https://api-gateway/getjwt')
+auth_headers = manager.get_headers()
+requests.get('https://autobahn-service/', headers=auth_headers)
 ```
 
 # Advanced Usage
 
-## MDB
+## Dataset Subscriptions
 
 ### Callback
 
-Instead of iterating over a `Subscription`, you can provide a callback that takes a message as an argument.
+Instead of iterating over a `Subscription`, you can provide a callback that
+takes a message as an argument.
 
 ```python
 def cb(msg):
     print(msg.data.decode())
 
 conn = Connection('https://mdb-account-server.com')
 sub = await conn.subscribe('mydataset', callback=cb)
-
-# Since subscribe does not block, call sub.wait to block
-await sub.wait(messages=15)
-await sub.wait(timeout=5)
+await sub.wait(messages=10) # exit after 10 messages received
 ```
 
 ### Seek
 
-To move the cursor of your `Subscription`, use `seek`.
+Autobahn maintains a short history of messages (by default 7 days) for each 
+dataset. To navigate to different points in the stream use the `seek` method.
+Seek accepts a message sequence number or a datetime object.
 
 ```python
 # seek to message sequence 1
-await sub.seek(start_sequence=1)
+await sub.seek(1)
 
 # seek to 5 minutes ago
-await sub.seek(start_datetime=datetime.datetime.utcnow() - datetime.timedelta(minutes=5)
+await sub.seek(datetime.datetime.utcnow() - datetime.timedelta(minutes=5))
 ```
 
 ### Offset
 
-By default, `subscribe` starts with the oldest message. To start at the current time, specify offset.
+By default, `subscribe` starts at the current time; to start at the beginning
+of the stream use `Offset.BEGIN`
 
 ```python
-sub = await conn.subscribe('mydataset', offset=Offset.NOW)
+sub = await conn.subscribe('mydataset', offset=Offset.BEGIN)
 ```
 
 ### Low Latency
 
-By default, `Subscription`s fetch messages in batches of 10. If the server has less than 10 messages to send, it will wait a bit for new messages before returning the messages it does have. If that waiting is a problem, you may want to set `batch_size` to 1.
+By default, each `Subscription` fetches messages in batches of 10. If the
+server has less than 10 messages to send, it will wait up to 10 seconds
+for new messages before returning the messages it does have. For low-latency
+applications set the `batch` size to 1.
 
 ```python
-sub = await conn.subscribe('mydataset', batch_size=1)
+sub = await conn.subscribe('mydataset', batch=1)
 ```
 
-# Frequently Asked Questions
+# Important Notes
 
 ## TLS Errors
 
 TLS errors occur for 2 reasons
-  1. Not specifying client certificates
-  2. Not specifying a Certificate Authority
+  1. Invalid or missing client certificates
+  2. No certificate authority configured
 
 ### Client certificates
 
-By default, speedracer looks for certificates in the user's home directory named `cert.crt` and `cert.key`. To specify a different path, pass `cert=('./mycert.crt', './mycert.key')`.
+By default, speedracer uses PEM formatted X.509 certificates for user
+authentication. By default speedracer will use certificates placed in
+the users `$HOME/.ssh` directory. The certificate and key files should be named
+`$HOME/.ssh/cert.crt` and `$HOME/.ssh/cert.key`, respectively.
 
-```python
-conn = Connection('https://mdb-account-server.com', cert=('./mycert.crt', './mycert.key'))
+To specify a different path, pass a tuple containing the path to the certificate
+and key files to the `cert` argument.
 
-manager = JWTManager('https://api-gateway.com/getjwt', cert=('./mycert.crt', './mycert.key'))
+```python
+conn = Connection('https://mdb-account-server', cert=('./mycert.crt', './mycert.key'))
 ```
 
 ### Certificate Authority
 
-To specify a Certificate Authorty
+Certificate Authorities establish a chain of trust. This is usually configured globally
+as part of the operating system. There are cases where the OS does not have the proper
+certificate authority configured.
+
+In these instances, users may specify a cabundle as a X.509 PEM file via the environment
+variable `SSL_CA_BUNDLE` or via the arugment `ca_bundle`.
 
 ```
 conn = Connection('https://mdb-account-server.com', ca_bundle='ca.pem')
-
-manager = JWTManager('https://api-gateway.com/getjwt', verify='./ca.pem')
 ```
 
-`JWTManager` also supports verify=False, but `Connection` does not offer an insecure option.
-
 ## Subscription not starting at specified offset
 
-The MDB remembers your subscription's place. If your program restarts, the subscription will pick up where it left off. If that is not the behavior you want, then use the Subscription's seek method.
+Subscriptions to datasets are **durable**. This means that once you have subscribed to a
+dataset, message delivery restarts where you left off--even if your program restarts.
+
+Subscriptions will expire after 1-week if not used.
```

### Comparing `speedracer-0.0.1/LICENSE` & `speedracer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `speedracer-0.0.1/PKG-INFO` & `speedracer-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedracer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Conveniently access data
 Author: RRC
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -12,125 +12,136 @@
 Requires-Dist: nats-py[nkeys]~=2.3.1
 Requires-Dist: pyjwt~=2.7.0
 Requires-Dist: requests~=2.31.0
 Description-Content-Type: text/markdown
 
 # What is speedracer?
 
-speedracer provides convenience classes for
+speedracer is an asyncio enabled python library for interacting with Autobahn.
 
-- Subscribing to the Mission Data Broker (MDB)
-- Authenticating to Autobahn APIs
+- Subscribe to datasets available in the Mission Data Broker (MDB)
+- Authenticate with Autobahn APIs
 
 # Quickstart
 
-## Subscribing to the MDB
+## Subscribe to a dataset
 
 To subscribe to a dataset on the MDB
   1. Provide the base URL of the MDB Account Server (MAS) when creating a Connection
   2. Provide the dataset to the subscribe method
 
 ```python
-conn = Connection('https://mdb-account-server.com')
+conn = Connection('https://mdb-account-server/')
 sub = await conn.subscribe('mydataset')
 async for msg in sub:
     print(msg.data.decode())
 ```
 
-## Authenticating to Autobahn APIs
+## Authenticate with Autobahn APIs
 
-To authenticate to Autobahn's REST APIs
-  1. Create a `JWTManager` with the API Gateway's URL
-  2. Call the `get_headers` method to get an Authorization HTTP header
+Autobahn uses JWT credentials for authorization. These tokens are put into the `Authorization`
+header for all HTTPs requests. 
 
-```python
-manager = JWTManager('https://api-gateway.com/getjwt')
-headers = manager.get_headers()
-```
+JWTs are obtained by exchanging private keys with the API Gateway server and
+must be periodically refreshed.
 
-If already subscribed to MDB, you can reuse your `Connection`'s `JWTManager`
+`speedracer` automates the process of fetching JWTs and refreshing them when they expire.
 
 ```python
-conn.jwt_manager.get_headers()
+manager = JWTManager('https://api-gateway/getjwt')
+auth_headers = manager.get_headers()
+requests.get('https://autobahn-service/', headers=auth_headers)
 ```
 
 # Advanced Usage
 
-## MDB
+## Dataset Subscriptions
 
 ### Callback
 
-Instead of iterating over a `Subscription`, you can provide a callback that takes a message as an argument.
+Instead of iterating over a `Subscription`, you can provide a callback that
+takes a message as an argument.
 
 ```python
 def cb(msg):
     print(msg.data.decode())
 
 conn = Connection('https://mdb-account-server.com')
 sub = await conn.subscribe('mydataset', callback=cb)
-
-# Since subscribe does not block, call sub.wait to block
-await sub.wait(messages=15)
-await sub.wait(timeout=5)
+await sub.wait(messages=10) # exit after 10 messages received
 ```
 
 ### Seek
 
-To move the cursor of your `Subscription`, use `seek`.
+Autobahn maintains a short history of messages (by default 7 days) for each 
+dataset. To navigate to different points in the stream use the `seek` method.
+Seek accepts a message sequence number or a datetime object.
 
 ```python
 # seek to message sequence 1
-await sub.seek(start_sequence=1)
+await sub.seek(1)
 
 # seek to 5 minutes ago
-await sub.seek(start_datetime=datetime.datetime.utcnow() - datetime.timedelta(minutes=5)
+await sub.seek(datetime.datetime.utcnow() - datetime.timedelta(minutes=5))
 ```
 
 ### Offset
 
-By default, `subscribe` starts with the oldest message. To start at the current time, specify offset.
+By default, `subscribe` starts at the current time; to start at the beginning
+of the stream use `Offset.BEGIN`
 
 ```python
-sub = await conn.subscribe('mydataset', offset=Offset.NOW)
+sub = await conn.subscribe('mydataset', offset=Offset.BEGIN)
 ```
 
 ### Low Latency
 
-By default, `Subscription`s fetch messages in batches of 10. If the server has less than 10 messages to send, it will wait a bit for new messages before returning the messages it does have. If that waiting is a problem, you may want to set `batch_size` to 1.
+By default, each `Subscription` fetches messages in batches of 10. If the
+server has less than 10 messages to send, it will wait up to 10 seconds
+for new messages before returning the messages it does have. For low-latency
+applications set the `batch` size to 1.
 
 ```python
-sub = await conn.subscribe('mydataset', batch_size=1)
+sub = await conn.subscribe('mydataset', batch=1)
 ```
 
-# Frequently Asked Questions
+# Important Notes
 
 ## TLS Errors
 
 TLS errors occur for 2 reasons
-  1. Not specifying client certificates
-  2. Not specifying a Certificate Authority
+  1. Invalid or missing client certificates
+  2. No certificate authority configured
 
 ### Client certificates
 
-By default, speedracer looks for certificates in the user's home directory named `cert.crt` and `cert.key`. To specify a different path, pass `cert=('./mycert.crt', './mycert.key')`.
+By default, speedracer uses PEM formatted X.509 certificates for user
+authentication. By default speedracer will use certificates placed in
+the users `$HOME/.ssh` directory. The certificate and key files should be named
+`$HOME/.ssh/cert.crt` and `$HOME/.ssh/cert.key`, respectively.
 
-```python
-conn = Connection('https://mdb-account-server.com', cert=('./mycert.crt', './mycert.key'))
+To specify a different path, pass a tuple containing the path to the certificate
+and key files to the `cert` argument.
 
-manager = JWTManager('https://api-gateway.com/getjwt', cert=('./mycert.crt', './mycert.key'))
+```python
+conn = Connection('https://mdb-account-server', cert=('./mycert.crt', './mycert.key'))
 ```
 
 ### Certificate Authority
 
-To specify a Certificate Authorty
+Certificate Authorities establish a chain of trust. This is usually configured globally
+as part of the operating system. There are cases where the OS does not have the proper
+certificate authority configured.
+
+In these instances, users may specify a cabundle as a X.509 PEM file via the environment
+variable `SSL_CA_BUNDLE` or via the arugment `ca_bundle`.
 
 ```
 conn = Connection('https://mdb-account-server.com', ca_bundle='ca.pem')
-
-manager = JWTManager('https://api-gateway.com/getjwt', verify='./ca.pem')
 ```
 
-`JWTManager` also supports verify=False, but `Connection` does not offer an insecure option.
-
 ## Subscription not starting at specified offset
 
-The MDB remembers your subscription's place. If your program restarts, the subscription will pick up where it left off. If that is not the behavior you want, then use the Subscription's seek method.
+Subscriptions to datasets are **durable**. This means that once you have subscribed to a
+dataset, message delivery restarts where you left off--even if your program restarts.
+
+Subscriptions will expire after 1-week if not used.
```

