# Comparing `tmp/EnergyModels-0.0.8.tar.gz` & `tmp/EnergyModels-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnergyModels-0.0.8.tar", last modified: Wed Dec  7 03:09:14 2022, max compression
+gzip compressed data, was "EnergyModels-0.0.9.tar", last modified: Fri Jun 23 18:55:40 2023, max compression
```

## Comparing `EnergyModels-0.0.8.tar` & `EnergyModels-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-12-07 03:09:14.780822 EnergyModels-0.0.8/
-drwxrwxrwx   0        0        0        0 2022-12-07 03:09:14.549597 EnergyModels-0.0.8/Data/
--rw-rw-rw-   0        0        0        0 2022-10-17 14:11:26.000000 EnergyModels-0.0.8/Data/__init__.py
--rw-rw-rw-   0        0        0     1736 2022-10-16 23:07:56.000000 EnergyModels-0.0.8/Data/preprocess_data.py
-drwxrwxrwx   0        0        0        0 2022-12-07 03:09:14.591632 EnergyModels-0.0.8/EnergyModels.egg-info/
--rw-rw-rw-   0        0        0     3972 2022-12-07 03:09:14.000000 EnergyModels-0.0.8/EnergyModels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2022-12-07 03:09:14.000000 EnergyModels-0.0.8/EnergyModels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-07 03:09:14.000000 EnergyModels-0.0.8/EnergyModels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-12-07 03:09:14.000000 EnergyModels-0.0.8/EnergyModels.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-07 03:09:14.777344 EnergyModels-0.0.8/Energy_Models/
--rw-rw-rw-   0        0        0     1659 2022-11-18 23:12:53.000000 EnergyModels-0.0.8/Energy_Models/BiGRU.py
--rw-rw-rw-   0        0        0     1124 2022-11-18 23:11:28.000000 EnergyModels-0.0.8/Energy_Models/BiLSTM.py
--rw-rw-rw-   0        0        0     1507 2022-11-18 23:15:45.000000 EnergyModels-0.0.8/Energy_Models/CNN.py
--rw-rw-rw-   0        0        0     1182 2022-11-18 23:17:24.000000 EnergyModels-0.0.8/Energy_Models/CNN_LSTM.py
--rw-rw-rw-   0        0        0      975 2022-11-18 23:13:22.000000 EnergyModels-0.0.8/Energy_Models/Evaluation_Metrix.py
--rw-rw-rw-   0        0        0     1301 2022-11-18 23:18:37.000000 EnergyModels-0.0.8/Energy_Models/GRU.py
--rw-rw-rw-   0        0        0     1194 2022-11-18 23:19:32.000000 EnergyModels-0.0.8/Energy_Models/LSTM.py
--rw-rw-rw-   0        0        0    30508 2022-12-07 02:39:16.000000 EnergyModels-0.0.8/Energy_Models/Performer.py
--rw-rw-rw-   0        0        0     5154 2022-11-18 23:20:41.000000 EnergyModels-0.0.8/Energy_Models/TCN.py
--rw-rw-rw-   0        0        0     1555 2022-11-18 23:21:18.000000 EnergyModels-0.0.8/Energy_Models/TimeDistributed.py
--rw-rw-rw-   0        0        0     1917 2022-11-18 23:00:41.000000 EnergyModels-0.0.8/Energy_Models/Transformer.py
--rw-rw-rw-   0        0        0        0 2022-11-15 04:21:06.000000 EnergyModels-0.0.8/Energy_Models/__init__.py
--rw-rw-rw-   0        0        0     1089 2022-09-28 20:30:23.000000 EnergyModels-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3972 2022-12-07 03:09:14.781487 EnergyModels-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3498 2022-11-18 23:58:42.000000 EnergyModels-0.0.8/README.md
--rw-rw-rw-   0        0        0      110 2022-09-20 21:40:40.000000 EnergyModels-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      570 2022-12-07 03:09:14.788235 EnergyModels-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 18:55:40.962361 EnergyModels-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-06-23 18:55:40.887561 EnergyModels-0.0.9/Data/
+-rw-rw-rw-   0        0        0        0 2022-10-17 14:11:26.000000 EnergyModels-0.0.9/Data/__init__.py
+-rw-rw-rw-   0        0        0     1736 2022-10-16 23:07:56.000000 EnergyModels-0.0.9/Data/preprocess_data.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:55:40.896537 EnergyModels-0.0.9/EnergyModels.egg-info/
+-rw-rw-rw-   0        0        0     3347 2023-06-23 18:55:40.000000 EnergyModels-0.0.9/EnergyModels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-06-23 18:55:40.000000 EnergyModels-0.0.9/EnergyModels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 18:55:40.000000 EnergyModels-0.0.9/EnergyModels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-23 18:55:40.000000 EnergyModels-0.0.9/EnergyModels.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 18:55:40.960367 EnergyModels-0.0.9/Energy_Models/
+-rw-rw-rw-   0        0        0     9345 2023-06-23 18:07:10.000000 EnergyModels-0.0.9/Energy_Models/Autoformer.py
+-rw-rw-rw-   0        0        0     1659 2022-11-18 23:12:53.000000 EnergyModels-0.0.9/Energy_Models/BiGRU.py
+-rw-rw-rw-   0        0        0     1124 2022-11-18 23:11:28.000000 EnergyModels-0.0.9/Energy_Models/BiLSTM.py
+-rw-rw-rw-   0        0        0     1507 2022-11-18 23:15:45.000000 EnergyModels-0.0.9/Energy_Models/CNN.py
+-rw-rw-rw-   0        0        0     1182 2022-11-18 23:17:24.000000 EnergyModels-0.0.9/Energy_Models/CNN_LSTM.py
+-rw-rw-rw-   0        0        0     2248 2023-06-23 18:11:23.000000 EnergyModels-0.0.9/Energy_Models/ConvLstm.py
+-rw-rw-rw-   0        0        0     2938 2023-06-23 18:12:10.000000 EnergyModels-0.0.9/Energy_Models/DeepAr.py
+-rw-rw-rw-   0        0        0      975 2022-11-18 23:13:22.000000 EnergyModels-0.0.9/Energy_Models/Evaluation_Metrix.py
+-rw-rw-rw-   0        0        0     1097 2023-03-20 00:09:01.000000 EnergyModels-0.0.9/Energy_Models/FNN.py
+-rw-rw-rw-   0        0        0     1301 2022-11-18 23:18:37.000000 EnergyModels-0.0.9/Energy_Models/GRU.py
+-rw-rw-rw-   0        0        0    16824 2023-06-23 18:18:04.000000 EnergyModels-0.0.9/Energy_Models/Informer.py
+-rw-rw-rw-   0        0        0     1194 2022-11-18 23:19:32.000000 EnergyModels-0.0.9/Energy_Models/LSTM.py
+-rw-rw-rw-   0        0        0    16339 2023-06-23 18:20:14.000000 EnergyModels-0.0.9/Energy_Models/LstNet.py
+-rw-rw-rw-   0        0        0     1133 2023-03-29 01:23:58.000000 EnergyModels-0.0.9/Energy_Models/MLP.py
+-rw-rw-rw-   0        0        0    11613 2023-06-23 18:21:48.000000 EnergyModels-0.0.9/Energy_Models/NBEATS.py
+-rw-rw-rw-   0        0        0    29759 2023-06-23 18:15:22.000000 EnergyModels-0.0.9/Energy_Models/Performer.py
+-rw-rw-rw-   0        0        0     2168 2023-03-05 21:23:44.000000 EnergyModels-0.0.9/Energy_Models/RBFN.py
+-rw-rw-rw-   0        0        0    18158 2023-06-23 18:24:47.000000 EnergyModels-0.0.9/Energy_Models/Seq2Seq.py
+-rw-rw-rw-   0        0        0     5154 2022-11-18 23:20:41.000000 EnergyModels-0.0.9/Energy_Models/TCN.py
+-rw-rw-rw-   0        0        0     1555 2022-11-18 23:21:18.000000 EnergyModels-0.0.9/Energy_Models/TimeDistributed.py
+-rw-rw-rw-   0        0        0     1917 2022-11-18 23:00:41.000000 EnergyModels-0.0.9/Energy_Models/Transformer.py
+-rw-rw-rw-   0        0        0        0 2022-11-15 04:21:06.000000 EnergyModels-0.0.9/Energy_Models/__init__.py
+-rw-rw-rw-   0        0        0    15123 2023-06-23 18:11:00.000000 EnergyModels-0.0.9/Energy_Models/bert.py
+-rw-rw-rw-   0        0        0     1089 2022-09-28 20:30:23.000000 EnergyModels-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3347 2023-06-23 18:55:40.962361 EnergyModels-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2873 2023-06-23 18:02:47.000000 EnergyModels-0.0.9/README.md
+-rw-rw-rw-   0        0        0      110 2022-09-20 21:40:40.000000 EnergyModels-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      570 2023-06-23 18:55:40.963359 EnergyModels-0.0.9/setup.cfg
```

### Comparing `EnergyModels-0.0.8/Data/preprocess_data.py` & `EnergyModels-0.0.9/Data/preprocess_data.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/EnergyModels.egg-info/SOURCES.txt` & `EnergyModels-0.0.9/EnergyModels.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,19 +4,30 @@
 setup.cfg
 Data/__init__.py
 Data/preprocess_data.py
 EnergyModels.egg-info/PKG-INFO
 EnergyModels.egg-info/SOURCES.txt
 EnergyModels.egg-info/dependency_links.txt
 EnergyModels.egg-info/top_level.txt
+Energy_Models/Autoformer.py
 Energy_Models/BiGRU.py
 Energy_Models/BiLSTM.py
 Energy_Models/CNN.py
 Energy_Models/CNN_LSTM.py
+Energy_Models/ConvLstm.py
+Energy_Models/DeepAr.py
 Energy_Models/Evaluation_Metrix.py
+Energy_Models/FNN.py
 Energy_Models/GRU.py
+Energy_Models/Informer.py
 Energy_Models/LSTM.py
+Energy_Models/LstNet.py
+Energy_Models/MLP.py
+Energy_Models/NBEATS.py
 Energy_Models/Performer.py
+Energy_Models/RBFN.py
+Energy_Models/Seq2Seq.py
 Energy_Models/TCN.py
 Energy_Models/TimeDistributed.py
 Energy_Models/Transformer.py
-Energy_Models/__init__.py
+Energy_Models/__init__.py
+Energy_Models/bert.py
```

### Comparing `EnergyModels-0.0.8/Energy_Models/BiGRU.py` & `EnergyModels-0.0.9/Energy_Models/BiGRU.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/Energy_Models/BiLSTM.py` & `EnergyModels-0.0.9/Energy_Models/BiLSTM.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/Energy_Models/CNN.py` & `EnergyModels-0.0.9/Energy_Models/CNN.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/Energy_Models/CNN_LSTM.py` & `EnergyModels-0.0.9/Energy_Models/CNN_LSTM.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/Energy_Models/Evaluation_Metrix.py` & `EnergyModels-0.0.9/Energy_Models/Evaluation_Metrix.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/Energy_Models/GRU.py` & `EnergyModels-0.0.9/Energy_Models/GRU.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/Energy_Models/LSTM.py` & `EnergyModels-0.0.9/Energy_Models/LSTM.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/Energy_Models/Performer.py` & `EnergyModels-0.0.9/Energy_Models/Performer.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,30 +94,14 @@
     strings = chr_idx[:rank+1]
     data_notation = strings[:-1]
     sampling_matrix_notation = strings[:2] + strings[-1] + strings[-2]
     product = data_notation[:-1]+strings[-1]
     combine_equation = f"{data_notation},{sampling_matrix_notation}->{product}"
     return combine_equation
 
-# Lint as: python3
-# Copyright 2019 The TensorFlow Authors. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-"""Keras-based attention layer."""
 
 _CHR_IDX = string.ascii_lowercase
 
 
 def _build_attention_equation(rank, attn_axes):
   """Builds einsum equations for the attention computation.
 
@@ -727,14 +711,15 @@
         self.num_heads = num_heads
         self.ff_dim = ff_dim
         self.method = method
         self.supports = supports
         self.rate = rate
 
     def getModel(self):
+        
         inp = layers.Input(shape=(self.n_features,))
         x = TokenAndPositionEmbedding(self.maxlen, self.vocab_size, self.embed_dim)(inp)
         x = TransformerBlock(self.embed_dim, self.num_heads, self.ff_dim, self.method, self.supports, self.rate)(x)
         x = layers.GlobalAveragePooling1D()(x)
         x = layers.Dropout(0.1)(x)
         x = layers.Dense(20, activation="relu")(x)
         x = layers.Dropout(0.1)(x)
```

### Comparing `EnergyModels-0.0.8/Energy_Models/TCN.py` & `EnergyModels-0.0.9/Energy_Models/TCN.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/Energy_Models/TimeDistributed.py` & `EnergyModels-0.0.9/Energy_Models/TimeDistributed.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/Energy_Models/Transformer.py` & `EnergyModels-0.0.9/Energy_Models/Transformer.py`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/LICENSE` & `EnergyModels-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `EnergyModels-0.0.8/README.md` & `EnergyModels-0.0.9/EnergyModels.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,25 @@
+Metadata-Version: 2.1
+Name: EnergyModels
+Version: 0.0.9
+Summary: Prediction models in timeseries
+Home-page: https://github.com/IntElligence0?tab=repositories
+Author: Abd_Elrahman Basala
+Author-email: Abdoubasala2001@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Energy Models Package
 
                              THIS IS A PACKAGE OF MODELS OF PREDICT IN TIMESERIES FORECASTING                
-             this package helps any developer in univariate and multivariate-multi-step time series forcasting in house-power-consumption dataset lets take a look about each type 
+             this package helps any developer in univariate and multivariate-multi-step time series forcasting lets take a look about each type 
              Real-world time series forecasting is challenging for a whole host of reasons not limited to problem features such as having multiple input variables,the requirement 
              to predict multiple time steps,nd the need to a perform the same type of prediction for multiple physical sites.
 
 # Installation
 
 ````
 pip install EnergyModels
@@ -19,14 +33,25 @@
   * GRU
   * BIGRU
   * TimeDistributer
   * CNN
   * TCN
   * Transformer
   * Performer
+  * Informer
+  * Seq2Seq
+  * Bert
+  * Lstnet
+  * DeepAr
+  * FNN
+  * Conv-Lstm
+  * MLP
+  * Nbeats
+  * RBFN
+  * Autoformer
   
   All models take 3 parameters except
   
   * TCN :
     
         * must take value 
           * 1 : n_steps
@@ -63,43 +88,21 @@
             * 8 : method => 'linear'
             * 9 : supports => 10
             * 10 : rate => 0.1 
             
   
 # Package Folders 
  
- * Data
  * Energy_Models
  
 # how to use the package
 
  first you must read the data set you want to use the models on it 
- and then import preprocess_data from Data folder :
- 
- ````
- from Data import preprocess_data as pr
- 
- df = pd.read_csv('Data.txt',sep=';', 
-                  parse_dates={'date_time' : ['Date', 'Time']}, infer_datetime_format=True, 
-                  low_memory=False, na_values=['nan','?'], index_col='date_time')
-
- pr.fill_missing(df.values)
- df.to_csv('new_data.csv')
+ and then preprocess the data
  
- df = pd.read_csv('new_data.csv',parse_dates=['date_time'], index_col= 'date_time')
- ````
- 
- next step you can use functions on preprocess_data to split and scale the data . 
- 
-   ````
-   X_train, X_test = pr.train_test_split(df)
-   X_train, X_test, scaler = pr.scale_data(X_train, X_test)
-   ```` 
-   
- After that converting the data to supervised.
  now you can build model by import it from Energy_Models folder :
  
   ````
   from Energy_Models import ==== as m
   
   ** [====] refer to model name **
   
@@ -123,8 +126,8 @@
   ````
   from Energy_Models import Evaluation_Metrix as mx
   ````
  
   ````
   mx.print_metrics(Y_train,Y_pred_train,Y_test,Y_pred_test)
   
-  ```` 
+  ````
```

### Comparing `EnergyModels-0.0.8/setup.cfg` & `EnergyModels-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2045 6e65 7267 794d 6f64 656c 730d   = EnergyModels.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e38  .version = 0.0.8
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e39  .version = 0.0.9
 00000030: 0d0a 6175 7468 6f72 203d 2041 6264 5f45  ..author = Abd_E
 00000040: 6c72 6168 6d61 6e20 4261 7361 6c61 0d0a  lrahman Basala..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 2041  author_email = A
 00000060: 6264 6f75 6261 7361 6c61 3230 3031 4067  bdoubasala2001@g
 00000070: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000080: 7074 696f 6e20 3d20 5072 6564 6963 7469  ption = Predicti
 00000090: 6f6e 206d 6f64 656c 7320 696e 2074 696d  on models in tim
```

