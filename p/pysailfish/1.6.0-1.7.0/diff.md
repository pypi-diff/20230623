# Comparing `tmp/pysailfish-1.6.0.tar.gz` & `tmp/pysailfish-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysailfish-1.6.0.tar", max compression
+gzip compressed data, was "pysailfish-1.7.0.tar", max compression
```

## Comparing `pysailfish-1.6.0.tar` & `pysailfish-1.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     9184 2023-05-02 01:57:06.179743 pysailfish-1.6.0/README.md
--rw-r--r--   0        0        0      267 2023-06-21 13:36:24.341790 pysailfish-1.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 01:21:34.884388 pysailfish-1.6.0/pysailfish/__init__.py
--rw-r--r--   0        0        0     7671 2023-05-02 01:29:21.852922 pysailfish-1.6.0/pysailfish/app/EAs/MA_EA.py
--rw-r--r--   0        0        0     1213 2023-05-02 01:28:29.628493 pysailfish-1.6.0/pysailfish/app/EAs/MT4ClientEA.py
--rw-r--r--   0        0        0      401 2023-05-02 01:21:34.912388 pysailfish-1.6.0/pysailfish/app/Mainpage.dox
--rw-r--r--   0        0        0        0 2023-05-02 01:23:53.313928 pysailfish-1.6.0/pysailfish/app/__init__.py
--rw-r--r--   0        0        0     3376 2023-06-01 03:56:23.982981 pysailfish-1.6.0/pysailfish/app/main.py
--rw-r--r--   0        0        0     2097 2023-06-01 03:56:53.079013 pysailfish-1.6.0/pysailfish/app/test_tcp_client.py
--rw-r--r--   0        0        0     3458 2023-06-01 03:57:52.851079 pysailfish-1.6.0/pysailfish/app/test_tcp_server_client.py
--rw-r--r--   0        0        0     5822 2023-06-01 03:57:42.707068 pysailfish-1.6.0/pysailfish/internal/DataCtrl/MT4DataCtrl/MT4DataCtrl.py
--rw-r--r--   0        0        0    29758 2023-06-07 03:04:16.960200 pysailfish-1.6.0/pysailfish/internal/MT_EA/MT4_EA.py
--rw-r--r--   0        0        0     1741 2023-05-02 01:29:21.852922 pysailfish-1.6.0/pysailfish/internal/MT_EA/account_information.py
--rw-r--r--   0        0        0     3617 2023-06-07 03:03:45.212187 pysailfish-1.6.0/pysailfish/internal/MT_EA/chart_operations.py
--rw-r--r--   0        0        0     1672 2023-05-02 01:29:21.852922 pysailfish-1.6.0/pysailfish/internal/MT_EA/common_functions.py
--rw-r--r--   0        0        0     4531 2023-05-02 01:29:21.852922 pysailfish-1.6.0/pysailfish/internal/MT_EA/market_info.py
--rw-r--r--   0        0        0     9675 2023-05-02 01:24:33.698340 pysailfish-1.6.0/pysailfish/internal/MT_EA/mt4_const.py
--rw-r--r--   0        0        0    10493 2023-05-02 01:24:33.698340 pysailfish-1.6.0/pysailfish/internal/MT_EA/mt4_fun_num_map.py
--rw-r--r--   0        0        0    18293 2023-05-02 01:33:23.550747 pysailfish-1.6.0/pysailfish/internal/MT_EA/object_functions.py
--rw-r--r--   0        0        0      485 2023-05-02 01:24:33.698340 pysailfish-1.6.0/pysailfish/internal/MT_EA/predefined_variables.py
--rw-r--r--   0        0        0    25760 2023-05-02 01:29:21.852922 pysailfish-1.6.0/pysailfish/internal/MT_EA/technical_indicators.py
--rw-r--r--   0        0        0    20106 2023-06-21 13:35:59.733762 pysailfish-1.6.0/pysailfish/internal/MT_EA/timeseries_and_indicators_access.py
--rw-r--r--   0        0        0     5219 2023-05-02 01:29:21.852922 pysailfish-1.6.0/pysailfish/internal/MT_EA/trade_functions.py
--rw-r--r--   0        0        0     4456 2023-05-02 01:24:33.698340 pysailfish-1.6.0/pysailfish/internal/Network/TCPCast.py
--rw-r--r--   0        0        0        0 2023-05-02 01:21:34.912388 pysailfish-1.6.0/pysailfish/internal/__init__.py
--rw-r--r--   0        0        0      566 2023-06-01 03:56:12.466967 pysailfish-1.6.0/pysailfish/internal/devTools/AtomicData.py
--rw-r--r--   0        0        0     1399 2023-06-01 04:42:42.081336 pysailfish-1.6.0/pysailfish/internal/devTools/ThreadClass.py
--rw-r--r--   0        0        0        0 2023-06-01 03:56:12.466967 pysailfish-1.6.0/pysailfish/internal/observability/__init__.py
--rw-r--r--   0        0        0     3957 2023-06-01 04:42:27.569313 pysailfish-1.6.0/pysailfish/internal/observability/log_helper.py
--rw-r--r--   0        0        0      163 2023-06-01 04:43:00.497366 pysailfish-1.6.0/pysailfish/internal/observability/logging_json/__init__.py
--rw-r--r--   0        0        0     2814 2023-06-01 03:56:12.466967 pysailfish-1.6.0/pysailfish/internal/observability/logging_json/_formatter.py
--rw-r--r--   0        0        0      372 2023-06-01 03:56:12.466967 pysailfish-1.6.0/pysailfish/internal/observability/logging_json/version.py
--rw-r--r--   0        0        0        0 2023-06-01 03:56:12.466967 pysailfish-1.6.0/pysailfish/internal/observability/logstash/__init__.py
--rw-r--r--   0        0        0     4792 2023-06-01 03:56:12.466967 pysailfish-1.6.0/pysailfish/internal/observability/logstash/formatter.py
--rw-r--r--   0        0        0     4874 2023-06-01 04:43:06.065375 pysailfish-1.6.0/pysailfish/internal/observability/logstash/handler_amqp.py
--rw-r--r--   0        0        0     1227 2023-06-01 04:43:10.993383 pysailfish-1.6.0/pysailfish/internal/observability/logstash/handler_tcp.py
--rw-r--r--   0        0        0      909 2023-06-01 04:43:17.081392 pysailfish-1.6.0/pysailfish/internal/observability/logstash/handler_udp.py
--rw-r--r--   0        0        0    10288 1970-01-01 00:00:00.000000 pysailfish-1.6.0/setup.py
--rw-r--r--   0        0        0     9621 1970-01-01 00:00:00.000000 pysailfish-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     9184 2023-05-02 01:57:06.179743 pysailfish-1.7.0/README.md
+-rw-r--r--   0        0        0      267 2023-06-23 01:58:59.716794 pysailfish-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 01:21:34.884388 pysailfish-1.7.0/pysailfish/__init__.py
+-rw-r--r--   0        0        0     7671 2023-05-02 01:29:21.852922 pysailfish-1.7.0/pysailfish/app/EAs/MA_EA.py
+-rw-r--r--   0        0        0     1213 2023-05-02 01:28:29.628493 pysailfish-1.7.0/pysailfish/app/EAs/MT4ClientEA.py
+-rw-r--r--   0        0        0      401 2023-05-02 01:21:34.912388 pysailfish-1.7.0/pysailfish/app/Mainpage.dox
+-rw-r--r--   0        0        0        0 2023-05-02 01:23:53.313928 pysailfish-1.7.0/pysailfish/app/__init__.py
+-rw-r--r--   0        0        0     3376 2023-06-01 03:56:23.982981 pysailfish-1.7.0/pysailfish/app/main.py
+-rw-r--r--   0        0        0     2097 2023-06-01 03:56:53.079013 pysailfish-1.7.0/pysailfish/app/test_tcp_client.py
+-rw-r--r--   0        0        0     3458 2023-06-01 03:57:52.851079 pysailfish-1.7.0/pysailfish/app/test_tcp_server_client.py
+-rw-r--r--   0        0        0     5822 2023-06-01 03:57:42.707068 pysailfish-1.7.0/pysailfish/internal/DataCtrl/MT4DataCtrl/MT4DataCtrl.py
+-rw-r--r--   0        0        0    29758 2023-06-07 03:04:16.960200 pysailfish-1.7.0/pysailfish/internal/MT_EA/MT4_EA.py
+-rw-r--r--   0        0        0     1741 2023-05-02 01:29:21.852922 pysailfish-1.7.0/pysailfish/internal/MT_EA/account_information.py
+-rw-r--r--   0        0        0     3617 2023-06-07 03:03:45.212187 pysailfish-1.7.0/pysailfish/internal/MT_EA/chart_operations.py
+-rw-r--r--   0        0        0     1672 2023-05-02 01:29:21.852922 pysailfish-1.7.0/pysailfish/internal/MT_EA/common_functions.py
+-rw-r--r--   0        0        0     4531 2023-05-02 01:29:21.852922 pysailfish-1.7.0/pysailfish/internal/MT_EA/market_info.py
+-rw-r--r--   0        0        0     9675 2023-05-02 01:24:33.698340 pysailfish-1.7.0/pysailfish/internal/MT_EA/mt4_const.py
+-rw-r--r--   0        0        0    10493 2023-05-02 01:24:33.698340 pysailfish-1.7.0/pysailfish/internal/MT_EA/mt4_fun_num_map.py
+-rw-r--r--   0        0        0    18293 2023-05-02 01:33:23.550747 pysailfish-1.7.0/pysailfish/internal/MT_EA/object_functions.py
+-rw-r--r--   0        0        0      485 2023-05-02 01:24:33.698340 pysailfish-1.7.0/pysailfish/internal/MT_EA/predefined_variables.py
+-rw-r--r--   0        0        0    25760 2023-05-02 01:29:21.852922 pysailfish-1.7.0/pysailfish/internal/MT_EA/technical_indicators.py
+-rw-r--r--   0        0        0    20106 2023-06-23 01:58:48.000802 pysailfish-1.7.0/pysailfish/internal/MT_EA/timeseries_and_indicators_access.py
+-rw-r--r--   0        0        0     5219 2023-05-02 01:29:21.852922 pysailfish-1.7.0/pysailfish/internal/MT_EA/trade_functions.py
+-rw-r--r--   0        0        0     4456 2023-05-02 01:24:33.698340 pysailfish-1.7.0/pysailfish/internal/Network/TCPCast.py
+-rw-r--r--   0        0        0        0 2023-05-02 01:21:34.912388 pysailfish-1.7.0/pysailfish/internal/__init__.py
+-rw-r--r--   0        0        0      566 2023-06-01 03:56:12.466967 pysailfish-1.7.0/pysailfish/internal/devTools/AtomicData.py
+-rw-r--r--   0        0        0     1399 2023-06-01 04:42:42.081336 pysailfish-1.7.0/pysailfish/internal/devTools/ThreadClass.py
+-rw-r--r--   0        0        0        0 2023-06-01 03:56:12.466967 pysailfish-1.7.0/pysailfish/internal/observability/__init__.py
+-rw-r--r--   0        0        0     3957 2023-06-01 04:42:27.569313 pysailfish-1.7.0/pysailfish/internal/observability/log_helper.py
+-rw-r--r--   0        0        0      163 2023-06-01 04:43:00.497366 pysailfish-1.7.0/pysailfish/internal/observability/logging_json/__init__.py
+-rw-r--r--   0        0        0     2814 2023-06-01 03:56:12.466967 pysailfish-1.7.0/pysailfish/internal/observability/logging_json/_formatter.py
+-rw-r--r--   0        0        0      372 2023-06-01 03:56:12.466967 pysailfish-1.7.0/pysailfish/internal/observability/logging_json/version.py
+-rw-r--r--   0        0        0        0 2023-06-01 03:56:12.466967 pysailfish-1.7.0/pysailfish/internal/observability/logstash/__init__.py
+-rw-r--r--   0        0        0     4792 2023-06-01 03:56:12.466967 pysailfish-1.7.0/pysailfish/internal/observability/logstash/formatter.py
+-rw-r--r--   0        0        0     4874 2023-06-01 04:43:06.065375 pysailfish-1.7.0/pysailfish/internal/observability/logstash/handler_amqp.py
+-rw-r--r--   0        0        0     1227 2023-06-01 04:43:10.993383 pysailfish-1.7.0/pysailfish/internal/observability/logstash/handler_tcp.py
+-rw-r--r--   0        0        0      909 2023-06-01 04:43:17.081392 pysailfish-1.7.0/pysailfish/internal/observability/logstash/handler_udp.py
+-rw-r--r--   0        0        0    10288 1970-01-01 00:00:00.000000 pysailfish-1.7.0/setup.py
+-rw-r--r--   0        0        0     9621 1970-01-01 00:00:00.000000 pysailfish-1.7.0/PKG-INFO
```

### Comparing `pysailfish-1.6.0/README.md` & `pysailfish-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/app/EAs/MA_EA.py` & `pysailfish-1.7.0/pysailfish/app/EAs/MA_EA.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/app/EAs/MT4ClientEA.py` & `pysailfish-1.7.0/pysailfish/app/EAs/MT4ClientEA.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/app/main.py` & `pysailfish-1.7.0/pysailfish/app/main.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/app/test_tcp_client.py` & `pysailfish-1.7.0/pysailfish/app/test_tcp_client.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/app/test_tcp_server_client.py` & `pysailfish-1.7.0/pysailfish/app/test_tcp_server_client.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/DataCtrl/MT4DataCtrl/MT4DataCtrl.py` & `pysailfish-1.7.0/pysailfish/internal/DataCtrl/MT4DataCtrl/MT4DataCtrl.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/MT4_EA.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/MT4_EA.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/account_information.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/account_information.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/chart_operations.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/chart_operations.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/common_functions.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/common_functions.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/market_info.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/market_info.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/mt4_const.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/mt4_const.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/mt4_fun_num_map.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/mt4_fun_num_map.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/object_functions.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/object_functions.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/technical_indicators.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/technical_indicators.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/timeseries_and_indicators_access.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/timeseries_and_indicators_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,57 +219,57 @@
         self.__data_ctrl.send_message()
 
         return parse_fun(str_ret=self.__data_ctrl.receive_string_from_mt4())
 
     def __copy_time_common(self, str_ret: str) -> List[datetime]:
         if str_ret == "-1":
             return list()
-        parts = str_ret.split("-")
+        parts = str_ret.split("~")
         arr_size = int(parts[0])
         if arr_size+1 != len(parts):
             return list()
 
         datetime_array: List[datetime] = list()
         for ele in parts[1:]:
             datetime_array.append(datetime.strptime(ele, "%Y.%m.%d %H:%M:%S"))
 
         return datetime_array
 
     def __copy_float_common(self, str_ret: str) -> List[float]:
         if str_ret == "-1":
             return list()
-        parts = str_ret.split("-")
+        parts = str_ret.split("~")
         arr_size = int(parts[0])
         if arr_size+1 != len(parts):
             return list()
 
         float_array: List[float] = list()
         for ele in parts[1:]:
             float_array.append(float(ele))
 
         return float_array
 
     def __copy_int_common(self, str_ret: str) -> List[int]:
         if str_ret == "-1":
             return list()
-        parts = str_ret.split("-")
+        parts = str_ret.split("~")
         arr_size = int(parts[0])
         if arr_size+1 != len(parts):
             return list()
 
         int_array: List[float] = list()
         for ele in parts[1:]:
             int_array.append(int(ele))
 
         return int_array
 
     def __copy_rates_common(self, str_ret: str) -> List[Union[datetime, float, float, float, float, int, int, int]]:
         if str_ret == "-1":
             return list()
-        parts = str_ret.split("-")
+        parts = str_ret.split("~")
         arr_size = int(parts[0])
         if (arr_size*8)+1 != len(parts):
             return list()
 
         rates_array: List[Union[datetime, float, float, float, float, int, int, int]] = list()
         for idx in range(1, len(parts), 8):
             rates_array.append((datetime.strptime(parts[idx], "%Y.%m.%d %H:%M:%S")
```

### Comparing `pysailfish-1.6.0/pysailfish/internal/MT_EA/trade_functions.py` & `pysailfish-1.7.0/pysailfish/internal/MT_EA/trade_functions.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/Network/TCPCast.py` & `pysailfish-1.7.0/pysailfish/internal/Network/TCPCast.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/devTools/AtomicData.py` & `pysailfish-1.7.0/pysailfish/internal/devTools/AtomicData.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/devTools/ThreadClass.py` & `pysailfish-1.7.0/pysailfish/internal/devTools/ThreadClass.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/observability/log_helper.py` & `pysailfish-1.7.0/pysailfish/internal/observability/log_helper.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/observability/logging_json/_formatter.py` & `pysailfish-1.7.0/pysailfish/internal/observability/logging_json/_formatter.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/observability/logstash/formatter.py` & `pysailfish-1.7.0/pysailfish/internal/observability/logstash/formatter.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/observability/logstash/handler_amqp.py` & `pysailfish-1.7.0/pysailfish/internal/observability/logstash/handler_amqp.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/observability/logstash/handler_tcp.py` & `pysailfish-1.7.0/pysailfish/internal/observability/logstash/handler_tcp.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/pysailfish/internal/observability/logstash/handler_udp.py` & `pysailfish-1.7.0/pysailfish/internal/observability/logstash/handler_udp.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.6.0/setup.py` & `pysailfish-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'pysailfish.internal.observability.logstash']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pysailfish',
-    'version': '1.6.0',
+    'version': '1.7.0',
     'description': '',
     'long_description': '\n## pysailfish\n\n### Example EA --- simple client\n```python\nfrom pysailfish.internal.MT_EA.MT4_EA import MT4_EA\n\nclass MT4DemoEA(MT4_EA):\n    def __init__(self):\n        super().__init__()\n\n    # override\n    def _OnInit(self) -> int:\n        self._logger.info(self._user_inputs)\n        self._logger.info("Here")\n        return 0\n\n    # override\n    def _OnDeinit(self, reason: int) -> None:\n        self._logger.info(f"Here reason: {reason}")\n        return None\n\n    # override\n    def _OnTick(self) -> None:\n        self._logger.info("Here")\n        return None\n\n    # override\n    def _OnTimer(self) -> None:\n        return None\n\n    # override\n    def _OnTester(self) -> float:\n        self._logger.info("Here")\n        return 0.0\n\n    # override\n    def _OnChartEvent(self\n                      , id: int\n                      , lparam: int\n                      , dparam: float\n                      , sparam: str) -> None:\n        self._logger.info(f"Here id: {id} lparam: {lparam} dparam: {dparam} sparam: {sparam}")\n        return None\n\ndef main() -> None:\n    ea = MT4DemoEA()\n    ea.InitComponent(server_ip="127.0.0.1"\n                     , server_port=23456\n                     , ea_name="MT4DemoEA")\n    ea.StartEA()\n\nif __name__ == "__main__":\n    main()\n```\n\n### Example EA --- Moving Average EA\n```python\nfrom datetime import datetime\n\nimport pysailfish.internal.MT_EA.mt4_const as mc\nfrom pysailfish.internal.MT_EA.MT4_EA import MT4_EA\n\nclass MA_EA(MT4_EA):\n    def __init__(self):\n        super().__init__()\n\n    # override\n    def _OnInit(self) -> int:\n        self._logger.info(self._user_inputs)\n        self._logger.info("Here")\n        return 0\n\n    # override\n    def _OnDeinit(self, reason: int) -> None:\n        self._logger.info(f"Here reason: {reason}")\n        return None\n\n    # override\n    def _OnTick(self) -> None:\n        vv = self.iADX(symbol=self._pv.symbol\n                       , timeframe=mc.PERIOD_CURRENT\n                       , period=self._user_inputs["MovingPeriod"]\n                       , applied_price=mc.PRICE_CLOSE\n                       , mode=mc.MODE_MAIN\n                       , shift=0)\n        # self._logger.info(f"Here {self._pv.symbol} {self._pv.time[0]}")\n        # --- check for history and trading\n        if self._pv.bars < 100 or self._pv.is_trade_allowed == False:\n            return\n\n        # --- calculate open orders by current symbol\n        if self.__calculate_current_orders(self._pv.symbol) == 0:\n            self.__check_for_open()\n        else:\n            self.__check_for_close()\n        return None\n\n    # override\n    def _OnTimer(self) -> None:\n        return None\n\n    # override\n    def _OnTester(self) -> float:\n        self._logger.info("Here")\n        return 0.0\n\n    # override\n    def _OnChartEvent(self\n                      , id: int\n                      , lparam: int\n                      , dparam: float\n                      , sparam: str) -> None:\n        self._logger.info(f"Here id: {id} lparam: {lparam} dparam: {dparam} sparam: {sparam}")\n        return None\n\n    def __check_for_close(self) -> None:\n        ma: float = 0\n        #--- go trading only for first tiks of new bar\n        if self._pv.volume[0] > 1:\n            return None\n        #--- get Moving Average\n        ma = self.iMA(symbol=self._pv.symbol\n                      , timeframe=mc.PERIOD_CURRENT\n                      , ma_period=self._user_inputs["MovingPeriod"]\n                      , ma_shift=self._user_inputs["MovingShift"]\n                      , ma_method=mc.MODE_SMA\n                      , applied_price=mc.PRICE_CLOSE\n                      , shift=0)\n        #---\n        for i in range(self.OrdersTotal()):\n            if self.OrderSelect(index=i, select=mc.SELECT_BY_POS, pool=mc.MODE_TRADES) == False:\n                break\n            if self.OrderMagicNumber() != self._pv.magic_num or self.OrderSymbol() != self._pv.symbol:\n                continue\n            #--- check order type\n            if self.OrderType() == mc.OP_BUY:\n                if self._pv.open[1] > ma and self._pv.close[1] < ma:\n                    if not self.OrderClose(ticket=self.OrderTicket(), lots=self.OrderLots(), price=self._pv.bid, slippage=3, arrow_color=mc.clrWhite):\n                        self._logger.error(f"OrderClose error {self.GetLastError()}")\n                break\n            if self.OrderType() == mc.OP_SELL:\n                if self._pv.open[1] < ma and self._pv.close[1] > ma:\n                    if not self.OrderClose(ticket=self.OrderTicket(), lots=self.OrderLots(), price=self._pv.ask, slippage=3, arrow_color=mc.clrWhite):\n                        self._logger.error(f"OrderClose error {self.GetLastError()}");\n                break\n\n    def __lots_optimized(self) -> float:\n        lot: float = float(self._user_inputs["Lots"])\n        maximum_risk: float = float(self._user_inputs["MaximumRisk"])\n        decrease_factor: float = float(self._user_inputs["DecreaseFactor"])\n        orders: int = self.OrdersHistoryTotal() # history orders total\n        losses: int = 0 # number of losses orders without a break\n        #--- select lot size\n        lot = self.NormalizeDouble(value=(self.AccountFreeMargin() * maximum_risk / 1000.0), digits=1);\n        #--- calcuulate number of losses orders without a break\n        if decrease_factor > 0:\n            for i in reversed(range(orders)):\n                if self.OrderSelect(index=i, select=mc.SELECT_BY_POS, pool=mc.MODE_HISTORY) == False:\n                    self._logger.error("Error in history")\n                    break\n                if self.OrderSymbol() != self._pv.symbol or self.OrderType() > mc.OP_SELL:\n                    continue\n                #---\n                if self.OrderProfit() > 0:\n                    break\n                if self.OrderProfit() < 0:\n                    losses += 1\n            if losses > 1:\n                lot = self.NormalizeDouble(value=(lot - lot * losses / decrease_factor), digits=1)\n        #--- return lot size\n        if lot < 0.1:\n            lot = 0.1\n        return lot\n\n    def __check_for_open(self) -> None:\n        ma: float = 0\n        res: int = 0\n        #--- go trading only for first tiks of new bar\n        if self._pv.volume[0] > 1:\n            return None\n        #--- get Moving Average\n        ma = self.iMA(symbol=self._pv.symbol\n                      , timeframe=mc.PERIOD_CURRENT\n                      , ma_period=self._user_inputs["MovingPeriod"]\n                      , ma_shift=self._user_inputs["MovingShift"]\n                      , ma_method=mc.MODE_SMA\n                      , applied_price=mc.PRICE_CLOSE\n                      , shift=0)\n        #--- sell conditions\n        if self._pv.open[1] > ma and self._pv.close[1] < ma:\n            res = self.OrderSend(symbol=self._pv.symbol\n                                 , cmd=mc.OP_SELL\n                                 , volume=self.__lots_optimized()\n                                 , price=self._pv.bid\n                                 , slippage=3\n                                 , stoploss=0\n                                 , takeprofit=0\n                                 , comment=""\n                                 , magic=self._pv.magic_num\n                                 , expiration=datetime(1970, 1, 1, 0, 0, 0)\n                                 , arrow_color=mc.clrRed)\n            return None\n        #--- buy conditions\n        if self._pv.open[1] < ma and self._pv.close[1] > ma:\n            res = self.OrderSend(symbol=self._pv.symbol\n                                 , cmd=mc.OP_BUY\n                                 , volume=self.__lots_optimized()\n                                 , price=self._pv.ask\n                                 , slippage=3\n                                 , stoploss=0\n                                 , takeprofit=0\n                                 , comment=""\n                                 , magic=self._pv.magic_num\n                                 , expiration=datetime(1970, 1, 1, 0, 0, 0)\n                                 , arrow_color=mc.clrBlue)\n            return None\n\n    def __calculate_current_orders(self, symbol: str) -> int:\n        buys: int = 0\n        sells: int = 0\n        # ---\n        for i in range(self.OrdersTotal()):\n            if self._tf.order_select(index=i, select=mc.SELECT_BY_POS, pool=mc.MODE_TRADES) == False:\n                break\n            if self.OrderSymbol() == self._pv.symbol and self.OrderMagicNumber() == self._pv.magic_num:\n                if self.OrderType() == mc.OP_BUY:\n                    buys += 1\n                if self.OrderType() == mc.OP_SELL:\n                    sells += 1\n        # --- return orders volume\n        if buys > 0:\n            return buys\n        else:\n            return -sells\n\ndef main() -> None:\n    ea = MA_EA()\n    ea.InitComponent(server_ip="127.0.0.1"\n                     , server_port=23456\n                     , ea_name="MA_EA")\n    ea.StartEA()\n\nif __name__ == "__main__":\n    main()\n```\n\n### How to publish to pypi\n```bash\n# set up pypi token\n$ poetry config pypi-token.pypi my-token\n\n# build the project\n$ poetry build\n\n# publish the project\n$ poetry publish\n\n# DONE\n```\n',
     'author': 'SulfredLee',
     'author_email': 'sflee1112@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pysailfish-1.6.0/PKG-INFO` & `pysailfish-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysailfish
-Version: 1.6.0
+Version: 1.7.0
 Summary: 
 Author: SulfredLee
 Author-email: sflee1112@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

