# Comparing `tmp/fa-models-1.0.43.tar.gz` & `tmp/fa-models-1.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.43.tar", last modified: Thu Jun 22 12:09:54 2023, max compression
+gzip compressed data, was "fa-models-1.0.44.tar", last modified: Fri Jun 23 14:44:40 2023, max compression
```

## Comparing `fa-models-1.0.43.tar` & `fa-models-1.0.44.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.778478 fa-models-1.0.43/
--rw-rw-rw-   0        0        0     3510 2023-06-22 12:09:54.776020 fa-models-1.0.43/PKG-INFO
--rw-rw-rw-   0        0        0     2946 2023-06-22 12:07:42.000000 fa-models-1.0.43/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.695349 fa-models-1.0.43/fa_models.egg-info/
--rw-rw-rw-   0        0        0     3510 2023-06-22 12:09:54.000000 fa-models-1.0.43/fa_models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      812 2023-06-22 12:09:54.000000 fa-models-1.0.43/fa_models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 12:09:54.000000 fa-models-1.0.43/fa_models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-06-22 12:09:54.000000 fa-models-1.0.43/fa_models.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 12:09:54.000000 fa-models-1.0.43/fa_models.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.702810 fa-models-1.0.43/famodels/
--rw-rw-rw-   0        0        0        0 2023-03-18 09:51:48.000000 fa-models-1.0.43/famodels/__init__.py
--rw-rw-rw-   0        0        0       92 2023-03-18 09:48:40.000000 fa-models-1.0.43/famodels/direction.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.714328 fa-models-1.0.43/famodels/generators/
--rw-rw-rw-   0        0        0        0 2023-03-18 09:47:08.000000 fa-models-1.0.43/famodels/generators/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-03-26 21:17:57.000000 fa-models-1.0.43/famodels/generators/data_generator.py
--rw-rw-rw-   0        0        0    11151 2023-03-23 08:14:14.000000 fa-models-1.0.43/famodels/generators/schema_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.755856 fa-models-1.0.43/famodels/models/
--rw-rw-rw-   0        0        0        0 2023-03-18 09:14:45.000000 fa-models-1.0.43/famodels/models/__init__.py
--rw-rw-rw-   0        0        0       92 2023-01-19 12:24:54.000000 fa-models-1.0.43/famodels/models/direction.py
--rw-rw-rw-   0        0        0     1374 2023-06-18 19:02:13.000000 fa-models-1.0.43/famodels/models/order.py
--rw-rw-rw-   0        0        0       96 2023-01-19 12:25:47.000000 fa-models-1.0.43/famodels/models/order_type.py
--rw-rw-rw-   0        0        0     1275 2023-06-18 19:01:06.000000 fa-models-1.0.43/famodels/models/processed_signal.py
--rw-rw-rw-   0        0        0       83 2023-01-19 12:24:30.000000 fa-models-1.0.43/famodels/models/side.py
--rw-rw-rw-   0        0        0      274 2023-06-13 12:35:17.000000 fa-models-1.0.43/famodels/models/state_of_signal.py
--rw-rw-rw-   0        0        0      884 2023-01-19 12:25:20.000000 fa-models-1.0.43/famodels/models/state_of_trade.py
--rw-rw-rw-   0        0        0     1890 2023-03-18 09:33:40.000000 fa-models-1.0.43/famodels/models/trade.py
--rw-rw-rw-   0        0        0     3293 2023-06-18 19:01:29.000000 fa-models-1.0.43/famodels/models/trading_signal.py
--rw-rw-rw-   0        0        0     1854 2023-06-18 19:00:18.000000 fa-models-1.0.43/famodels/models/virtual_order.py
--rw-rw-rw-   0        0        0     1342 2023-06-22 12:09:22.000000 fa-models-1.0.43/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 12:09:54.779509 fa-models-1.0.43/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-03-18 09:51:35.000000 fa-models-1.0.43/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:09:54.771441 fa-models-1.0.43/tests/
--rw-rw-rw-   0        0        0      272 2023-03-18 09:52:10.000000 fa-models-1.0.43/tests/test_data_generator.py
--rw-rw-rw-   0        0        0     1427 2023-06-13 13:04:30.000000 fa-models-1.0.43/tests/test_processed_trading_signal.py
--rw-rw-rw-   0        0        0      857 2023-03-18 09:37:22.000000 fa-models-1.0.43/tests/test_produce_schemas.py
--rw-rw-rw-   0        0        0     2338 2023-03-22 15:14:28.000000 fa-models-1.0.43/tests/test_schema_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:40.371692 fa-models-1.0.44/
+-rw-rw-rw-   0        0        0     3511 2023-06-23 14:44:40.370524 fa-models-1.0.44/PKG-INFO
+-rw-rw-rw-   0        0        0     2947 2023-06-23 08:37:23.000000 fa-models-1.0.44/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:40.318349 fa-models-1.0.44/fa_models.egg-info/
+-rw-rw-rw-   0        0        0     3511 2023-06-23 14:44:40.000000 fa-models-1.0.44/fa_models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2023-06-23 14:44:40.000000 fa-models-1.0.44/fa_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 14:44:40.000000 fa-models-1.0.44/fa_models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-06-23 14:44:40.000000 fa-models-1.0.44/fa_models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 14:44:40.000000 fa-models-1.0.44/fa_models.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:40.323590 fa-models-1.0.44/famodels/
+-rw-rw-rw-   0        0        0        0 2023-03-18 09:51:48.000000 fa-models-1.0.44/famodels/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-03-18 09:48:40.000000 fa-models-1.0.44/famodels/direction.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:40.330589 fa-models-1.0.44/famodels/generators/
+-rw-rw-rw-   0        0        0        0 2023-03-18 09:47:08.000000 fa-models-1.0.44/famodels/generators/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-03-26 21:17:57.000000 fa-models-1.0.44/famodels/generators/data_generator.py
+-rw-rw-rw-   0        0        0    11151 2023-03-23 08:14:14.000000 fa-models-1.0.44/famodels/generators/schema_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:40.357639 fa-models-1.0.44/famodels/models/
+-rw-rw-rw-   0        0        0        0 2023-03-18 09:14:45.000000 fa-models-1.0.44/famodels/models/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-01-19 12:24:54.000000 fa-models-1.0.44/famodels/models/direction.py
+-rw-rw-rw-   0        0        0     1374 2023-06-18 19:02:13.000000 fa-models-1.0.44/famodels/models/order.py
+-rw-rw-rw-   0        0        0       96 2023-01-19 12:25:47.000000 fa-models-1.0.44/famodels/models/order_type.py
+-rw-rw-rw-   0        0        0     1277 2023-06-23 14:18:39.000000 fa-models-1.0.44/famodels/models/processed_signal.py
+-rw-rw-rw-   0        0        0       83 2023-01-19 12:24:30.000000 fa-models-1.0.44/famodels/models/side.py
+-rw-rw-rw-   0        0        0      274 2023-06-13 12:35:17.000000 fa-models-1.0.44/famodels/models/state_of_signal.py
+-rw-rw-rw-   0        0        0      884 2023-01-19 12:25:20.000000 fa-models-1.0.44/famodels/models/state_of_trade.py
+-rw-rw-rw-   0        0        0     2000 2023-06-23 14:18:24.000000 fa-models-1.0.44/famodels/models/trade.py
+-rw-rw-rw-   0        0        0     3295 2023-06-23 08:37:23.000000 fa-models-1.0.44/famodels/models/trading_signal.py
+-rw-rw-rw-   0        0        0     1856 2023-06-23 07:07:35.000000 fa-models-1.0.44/famodels/models/virtual_order.py
+-rw-rw-rw-   0        0        0     1342 2023-06-23 14:44:06.000000 fa-models-1.0.44/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:44:40.371692 fa-models-1.0.44/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-03-18 09:51:35.000000 fa-models-1.0.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:40.368522 fa-models-1.0.44/tests/
+-rw-rw-rw-   0        0        0      272 2023-03-18 09:52:10.000000 fa-models-1.0.44/tests/test_data_generator.py
+-rw-rw-rw-   0        0        0     1427 2023-06-13 13:04:30.000000 fa-models-1.0.44/tests/test_processed_trading_signal.py
+-rw-rw-rw-   0        0        0      857 2023-03-18 09:37:22.000000 fa-models-1.0.44/tests/test_produce_schemas.py
+-rw-rw-rw-   0        0        0     2338 2023-03-22 15:14:28.000000 fa-models-1.0.44/tests/test_schema_generator.py
```

### Comparing `fa-models-1.0.43/PKG-INFO` & `fa-models-1.0.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.43
+Version: 1.0.44
 Summary: The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
@@ -75,15 +75,15 @@
 Prerequisite: make sure that you give your Operating System user the right to modify files in the python directory. The directory where pyhton is installed.
 Use `python setup.py bdist_wheel` to create the dist, build and .eggs folder.
 
 ## Reference from a different project
 In order to use your own version of the project - to maybe contribute to the library - simply clone the code from github into new directory. Then add the path of that new directory to the requirements.txt file of your project. Then change in fa-models whatever you recommend to improve. Don't forget the Open-Closed Principle: extend only (unless it requires a breaking change)
 
 
-### Releasing a new version
+## Releasing a new version
 
 Delete any old files in the /dist and build folder of your local environment.
 Update your pip: 
 ```
 python -m pip install --upgrade pip
 ```
 
@@ -117,14 +117,15 @@
 ```
 twine upload -r testpypi dist/*
 ```
 
 Login with username: svabra (password should be known)
 
 If the test-upload was successful, finally, upload to pypi production: 
+
 ```
 twine upload dist/*
 ```
 
 Done.
 
 (P.S. Do not forget to update the library in your projects: `pip install --upgrade fa-models`)bumpver update --patch
```

### Comparing `fa-models-1.0.43/README.md` & `fa-models-1.0.44/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 Prerequisite: make sure that you give your Operating System user the right to modify files in the python directory. The directory where pyhton is installed.
 Use `python setup.py bdist_wheel` to create the dist, build and .eggs folder.
 
 ## Reference from a different project
 In order to use your own version of the project - to maybe contribute to the library - simply clone the code from github into new directory. Then add the path of that new directory to the requirements.txt file of your project. Then change in fa-models whatever you recommend to improve. Don't forget the Open-Closed Principle: extend only (unless it requires a breaking change)
 
 
-### Releasing a new version
+## Releasing a new version
 
 Delete any old files in the /dist and build folder of your local environment.
 Update your pip: 
 ```
 python -m pip install --upgrade pip
 ```
 
@@ -104,14 +104,15 @@
 ```
 twine upload -r testpypi dist/*
 ```
 
 Login with username: svabra (password should be known)
 
 If the test-upload was successful, finally, upload to pypi production: 
+
 ```
 twine upload dist/*
 ```
 
 Done.
 
 (P.S. Do not forget to update the library in your projects: `pip install --upgrade fa-models`)bumpver update --patch
```

### Comparing `fa-models-1.0.43/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.44/fa_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.43
+Version: 1.0.44
 Summary: The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
@@ -75,15 +75,15 @@
 Prerequisite: make sure that you give your Operating System user the right to modify files in the python directory. The directory where pyhton is installed.
 Use `python setup.py bdist_wheel` to create the dist, build and .eggs folder.
 
 ## Reference from a different project
 In order to use your own version of the project - to maybe contribute to the library - simply clone the code from github into new directory. Then add the path of that new directory to the requirements.txt file of your project. Then change in fa-models whatever you recommend to improve. Don't forget the Open-Closed Principle: extend only (unless it requires a breaking change)
 
 
-### Releasing a new version
+## Releasing a new version
 
 Delete any old files in the /dist and build folder of your local environment.
 Update your pip: 
 ```
 python -m pip install --upgrade pip
 ```
 
@@ -117,14 +117,15 @@
 ```
 twine upload -r testpypi dist/*
 ```
 
 Login with username: svabra (password should be known)
 
 If the test-upload was successful, finally, upload to pypi production: 
+
 ```
 twine upload dist/*
 ```
 
 Done.
 
 (P.S. Do not forget to update the library in your projects: `pip install --upgrade fa-models`)bumpver update --patch
```

### Comparing `fa-models-1.0.43/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.44/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.43/famodels/generators/data_generator.py` & `fa-models-1.0.44/famodels/generators/data_generator.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.43/famodels/generators/schema_generator.py` & `fa-models-1.0.44/famodels/generators/schema_generator.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.43/famodels/models/order.py` & `fa-models-1.0.44/famodels/models/order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.43/famodels/models/processed_signal.py` & `fa-models-1.0.44/famodels/models/processed_signal.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from famodels.models.trading_signal import TradingSignal
 from famodels.models.state_of_signal import StateOfSignal
 from redis_om import Migrator
 from redis_om import (Field, JsonModel)
 from redis_om.connections import get_redis_connection
 
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
-print(f"the env-var REDIS_OM_URL is: {REDIS_OM_URL}")
+print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
 class ProcessedSignal(TradingSignal):
     """As soon a trading signal is processed by the signal qualifier, it is declared as a Processed Signal.
         When instantiating, use the **kwargs to map the TradingSignal values to the attributes of the processed trading signal.
         e.g. ProcessedTradingSignal(status=StateOfSignal.ACCEPTED, process_info=[], **signal.__dict__)
         Caution: Attributes other than status and process_info needs to added to the signal first before initializing an object.
     """
@@ -21,8 +21,8 @@
     process_info: List[str]
 
     class Meta:
         global_key_prefix="signal-processing"
         model_key_prefix="processed-signal"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
-Migrator().run()
+# Migrator().run()
```

### Comparing `fa-models-1.0.43/famodels/models/state_of_trade.py` & `fa-models-1.0.44/famodels/models/state_of_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.43/famodels/models/trade.py` & `fa-models-1.0.44/famodels/models/trade.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from datetime import datetime
+import os
 from famodels.models.state_of_trade import StateOfTrade
 from famodels.models.direction import Direction
 from typing import Optional
-from sqlmodel import Field, SQLModel
 import uuid
+from redis_om import Migrator
+from redis_om import (Field, JsonModel)
+from redis_om.connections import get_redis_connection
 
-class BaseTradeSQLModel(SQLModel):
-    def __init__(self, **kwargs):
-        self.__config__.table = False
-        super().__init__(**kwargs)
-        self.__config__.table = True
+REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
+print(f"the env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
-    class Config:
-        validate_assignment = True
 
-class Trade(BaseTradeSQLModel, table=True):
+class Trade(JsonModel):
     """A trade in our system is composed of a buy and a sell order. Do not mistaken it for a trade from the CEX.
         Create a new Trade record for every update and correlate them with trade_id. See attribute #trade_id"""   
-
-    __table_args__ = {'extend_existing': True}
     id: Optional[int] = Field(default=None, primary_key=True)    
     trade_id: Optional[str] = Field(default=str(uuid.uuid4()), nullable=False)
     # sort_index:int = field(init=False, repr=False)
     #trade_id: Optional[str] = Field(default=uuid.uuid4(), primary_key=True)
     """The trade id is the reference that keeps the state updates correlated. It will generate a UUID by default.
         Use this for the first record you insert. Inserting updated records (new records should then have the trade_id
         provided to create the correlation.)"""
@@ -36,9 +32,16 @@
     sell_order_id:Optional[str] = None
     take_profit:Optional[int] = None
     stop_loss:Optional[int] = None
     """This is usually the receiving timestamp."""        
     profit_and_loss_percentage: Optional[float] = None
     profit_and_loss_amount: Optional[float] = None
 
+    class Meta:
+        global_key_prefix="order-and-trade-processing"
+        model_key_prefix="trade"
+        database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
+
     def __getitem__(self, key):
-        return self.__dict__[key]    
+        return self.__dict__[key]    
+    
+# Migrator().run()
```

### Comparing `fa-models-1.0.43/famodels/models/trading_signal.py` & `fa-models-1.0.44/famodels/models/trading_signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     """The timestamp in milliseconds when the signal was entering our interface. This will be overridden."""    
 
     class Meta:
         global_key_prefix="signal-processing"
         model_key_prefix="raw-signal"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
-Migrator().run()
+# Migrator().run()
```

### Comparing `fa-models-1.0.43/famodels/models/virtual_order.py` & `fa-models-1.0.44/famodels/models/virtual_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,8 +42,8 @@
         global_key_prefix="performance-validation"
         model_key_prefix="virtual-order"        
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
     def __getitem__(self, key):
         return self.__dict__[key]
     
-Migrator().run()
+# Migrator().run()
```

### Comparing `fa-models-1.0.43/pyproject.toml` & `fa-models-1.0.44/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.43"
+version = "1.0.44"
 description = "The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.43"
+current_version = "1.0.44"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.43/setup.py` & `fa-models-1.0.44/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.43/tests/test_processed_trading_signal.py` & `fa-models-1.0.44/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.43/tests/test_produce_schemas.py` & `fa-models-1.0.44/tests/test_produce_schemas.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.43/tests/test_schema_generator.py` & `fa-models-1.0.44/tests/test_schema_generator.py`

 * *Files identical despite different names*

