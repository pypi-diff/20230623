# Comparing `tmp/streaming_indicators-0.0.3.tar.gz` & `tmp/streaming_indicators-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming_indicators-0.0.3.tar", last modified: Thu Jun 15 09:07:42 2023, max compression
+gzip compressed data, was "streaming_indicators-0.0.4.tar", last modified: Fri Jun 23 06:27:14 2023, max compression
```

## Comparing `streaming_indicators-0.0.3.tar` & `streaming_indicators-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 09:07:41.969957 streaming_indicators-0.0.3/
--rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3040 2023-06-15 09:07:41.969957 streaming_indicators-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1283 2023-06-15 08:59:38.000000 streaming_indicators-0.0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      847 2023-06-15 09:07:42.001960 streaming_indicators-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 09:07:41.795809 streaming_indicators-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 09:07:41.857708 streaming_indicators-0.0.3/src/streaming_indicators/
--rw-rw-rw-   0        0        0       35 2023-05-12 17:50:29.000000 streaming_indicators-0.0.3/src/streaming_indicators/__init__.py
--rw-rw-rw-   0        0        0     6194 2023-06-15 08:56:53.000000 streaming_indicators-0.0.3/src/streaming_indicators/streaming_indicators.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:07:41.969957 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/
--rw-rw-rw-   0        0        0     3040 2023-06-15 09:07:41.000000 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-06-15 09:07:41.000000 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 09:07:41.000000 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-15 09:07:41.000000 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-15 09:07:41.000000 streaming_indicators-0.0.3/src/streaming_indicators.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 06:27:14.084177 streaming_indicators-0.0.4/
+-rw-rw-rw-   0        0        0     1082 2023-05-12 14:45:21.000000 streaming_indicators-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3279 2023-06-23 06:27:14.084177 streaming_indicators-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1522 2023-06-20 14:02:39.000000 streaming_indicators-0.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-12 14:44:06.000000 streaming_indicators-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      847 2023-06-23 06:27:14.091168 streaming_indicators-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 06:27:14.010775 streaming_indicators-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 06:27:14.025770 streaming_indicators-0.0.4/src/streaming_indicators/
+-rw-rw-rw-   0        0        0       35 2023-05-12 17:50:29.000000 streaming_indicators-0.0.4/src/streaming_indicators/__init__.py
+-rw-rw-rw-   0        0        0     7719 2023-06-20 15:46:51.000000 streaming_indicators-0.0.4/src/streaming_indicators/streaming_indicators.py
+drwxrwxrwx   0        0        0        0 2023-06-23 06:27:14.083158 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/
+-rw-rw-rw-   0        0        0     3279 2023-06-23 06:27:13.000000 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-06-23 06:27:13.000000 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 06:27:13.000000 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-23 06:27:13.000000 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-23 06:27:13.000000 streaming_indicators-0.0.4/src/streaming_indicators.egg-info/top_level.txt
```

### Comparing `streaming_indicators-0.0.3/LICENSE.txt` & `streaming_indicators-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streaming_indicators-0.0.3/PKG-INFO` & `streaming_indicators-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming_indicators
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,24 @@
 ```
 from streaming_indicators import SMA
 
 sma = SMA(10)
 for i in range(20):
     print(i, sma.update(i))
 ```
+
+## List of indicators
+- Simple Moving Average (SMA)
+- Exponential Moving Average (EMA)
+- Relative Strength Index (RSI)
+- True Range (TR)
+- Average True Range (ATR)
+- Heikin Ashi Candlesticks (HeikinAshi)
+- Renko Bricks (Renko)
+
 ## TODO
 - Not all indicators current support compute method.
 - Add documentation.
 - HeikinAshi depends on key names, eg ('open','close'). Should be independent, i.e. given in input.
 - Implement more indicators.
 MIT License
```

### Comparing `streaming_indicators-0.0.3/README.md` & `streaming_indicators-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -20,12 +20,22 @@
 ```
 from streaming_indicators import SMA
 
 sma = SMA(10)
 for i in range(20):
     print(i, sma.update(i))
 ```
+
+## List of indicators
+- Simple Moving Average (SMA)
+- Exponential Moving Average (EMA)
+- Relative Strength Index (RSI)
+- True Range (TR)
+- Average True Range (ATR)
+- Heikin Ashi Candlesticks (HeikinAshi)
+- Renko Bricks (Renko)
+
 ## TODO
 - Not all indicators current support compute method.
 - Add documentation.
 - HeikinAshi depends on key names, eg ('open','close'). Should be independent, i.e. given in input.
 - Implement more indicators.
```

### Comparing `streaming_indicators-0.0.3/setup.cfg` & `streaming_indicators-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7472 6561 6d69 6e67 5f69 6e64   = streaming_ind
 00000020: 6963 6174 6f72 730d 0a76 6572 7369 6f6e  icators..version
-00000030: 203d 2030 2e30 2e33 0d0a 6175 7468 6f72   = 0.0.3..author
+00000030: 203d 2030 2e30 2e34 0d0a 6175 7468 6f72   = 0.0.4..author
 00000040: 203d 2052 6973 6861 6268 2047 7570 7461   = Rishabh Gupta
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2072 6973 6861 6268 6731 3939 3740 676d   rishabhg1997@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2070 7974 686f 6e20  tion = A python 
 00000090: 6c69 6272 6172 7920 666f 7220 636f 6d70  library for comp
 000000a0: 7574 696e 6720 7465 6368 6e69 6361 6c20  uting technical
```

### Comparing `streaming_indicators-0.0.3/src/streaming_indicators/streaming_indicators.py` & `streaming_indicators-0.0.4/src/streaming_indicators/streaming_indicators.py`

 * *Files 13% similar despite different names*

```diff
@@ -66,14 +66,65 @@
                 self.avg_gain = ((self.avg_gain*(self.period-1)) + self.gains[-1])/self.period
                 self.avg_loss = ((self.avg_loss*(self.period-1)) + self.losses[-1])/self.period
             rs = self.avg_gain / self.avg_loss
             self.rsi = 100 - (100/(1+rs))
             self.value = self.rsi
         return self.value
 
+class TRANGE:
+    '''True Range'''
+    def __init__(self):
+        self.prev_close = None
+        self.value = None
+    def compute(self, candle):
+        if(self.prev_close is None):
+            return candle['high'] - candle['low']
+        else:
+            return max(
+                candle['high'] - candle['low'],
+                abs(candle['high'] - self.prev_close),
+                abs(candle['low'] - self.prev_close)
+            )
+    def update(self, candle):
+        self.value = self.compute(candle)
+        self.prev_close = candle['close']
+        return self.value
+
+class ATR:
+    '''Average True Range'''
+    def __init__(self, period):
+        self.period = period
+        self.period_1 = period-1
+        self.TR = TRANGE()
+        self.atr = 0
+        self.value = None
+        self.count = 0
+    def compute(self, candle):
+        tr = self.TR.compute(candle)
+        if(self.count < self.period):
+            return None
+        elif(self.count == self.period):
+            return (self.atr + tr)/self.period
+        else:
+            return (self.atr*self.period_1 + tr)/self.period
+
+    def update(self, candle):
+        self.count += 1
+        tr = self.TR.update(candle)
+        if(self.count < self.period):
+            self.atr += tr
+            return None
+        if(self.count == self.period):
+            self.atr += tr
+            self.atr /= self.period
+        else:
+            self.atr = (self.atr*self.period_1 + tr)/self.period
+        self.value = self.atr
+        return self.value
+
 class HeikinAshi:
     def __init__(self):
         self.value = None
 
     def compute(self, candle):
         ha = {}
         ha['close'] = round((candle.open+candle.high+candle.low+candle.close)/4,4)
```

### Comparing `streaming_indicators-0.0.3/src/streaming_indicators.egg-info/PKG-INFO` & `streaming_indicators-0.0.4/src/streaming_indicators.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming-indicators
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library for computing technical analysis indicators on streaming data.
 Home-page: https://github.com/mr-easy/streaming_indicators
 Author: Rishabh Gupta
 Author-email: rishabhg1997@gmail.com
 Project-URL: Bug Tracker, https://github.com/mr-easy/streaming_indicators/issues
 Project-URL: Code, https://github.com/mr-easy/streaming_indicators
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,24 @@
 ```
 from streaming_indicators import SMA
 
 sma = SMA(10)
 for i in range(20):
     print(i, sma.update(i))
 ```
+
+## List of indicators
+- Simple Moving Average (SMA)
+- Exponential Moving Average (EMA)
+- Relative Strength Index (RSI)
+- True Range (TR)
+- Average True Range (ATR)
+- Heikin Ashi Candlesticks (HeikinAshi)
+- Renko Bricks (Renko)
+
 ## TODO
 - Not all indicators current support compute method.
 - Add documentation.
 - HeikinAshi depends on key names, eg ('open','close'). Should be independent, i.e. given in input.
 - Implement more indicators.
 MIT License
```

