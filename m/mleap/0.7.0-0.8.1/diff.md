# Comparing `tmp/mleap-0.7.0.tar.gz` & `tmp/mleap-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mleap-0.7.0.tar", last modified: Thu Apr 27 22:36:07 2017, max compression
+gzip compressed data, was "dist/mleap-0.8.1.tar", last modified: Mon Oct  9 04:28:30 2017, max compression
```

## Comparing `mleap-0.7.0.tar` & `mleap-0.8.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/
--rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/__init__.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/bundle/
--rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/bundle/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)     7479 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/bundle/serialize.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/pyspark/
--rw-r--r--   0 mikhail    (501) staff       (20)      231 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/pyspark/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)     2228 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/pyspark/feature.py
--rw-r--r--   0 mikhail    (501) staff       (20)     1806 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/pyspark/spark_support.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/sklearn/
--rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)     3532 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/base.py
--rw-r--r--   0 mikhail    (501) staff       (20)     8261 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/base_tests.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/sklearn/decomposition/
--rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/decomposition/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)     2420 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/decomposition/pca.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/sklearn/ensemble/
--rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/ensemble/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)     4147 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/ensemble/forest.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/sklearn/extensions/
--rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/extensions/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)     3719 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/extensions/data.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/sklearn/feature_extraction/
--rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/feature_extraction/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)     2397 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/feature_extraction/text.py
--rw-r--r--   0 mikhail    (501) staff       (20)     2336 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/feature_union.py
--rw-r--r--   0 mikhail    (501) staff       (20)     4059 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/logistic.py
--rw-r--r--   0 mikhail    (501) staff       (20)     6234 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/pipeline.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/sklearn/preprocessing/
--rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/preprocessing/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)    33877 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/preprocessing/data.py
--rw-r--r--   0 mikhail    (501) staff       (20)    36250 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/preprocessing/tests.py
--rw-r--r--   0 mikhail    (501) staff       (20)     3879 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/svm.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/sklearn/tree/
--rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/tree/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)     5126 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/sklearn/tree/tree.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap/tensorflow/
--rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/tensorflow/__init__.py
--rw-r--r--   0 mikhail    (501) staff       (20)     2609 2017-04-27 20:00:53.000000 mleap-0.7.0/mleap/tensorflow/test.py
--rw-r--r--   0 mikhail    (501) staff       (20)      828 2017-04-27 22:34:18.000000 mleap-0.7.0/mleap/version.py
-drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap.egg-info/
--rw-r--r--   0 mikhail    (501) staff       (20)        1 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap.egg-info/dependency_links.txt
--rw-r--r--   0 mikhail    (501) staff       (20)        1 2016-12-18 00:51:55.000000 mleap-0.7.0/mleap.egg-info/not-zip-safe
--rw-r--r--   0 mikhail    (501) staff       (20)      859 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap.egg-info/PKG-INFO
--rw-r--r--   0 mikhail    (501) staff       (20)      118 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap.egg-info/requires.txt
--rw-r--r--   0 mikhail    (501) staff       (20)     1062 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap.egg-info/SOURCES.txt
--rw-r--r--   0 mikhail    (501) staff       (20)        6 2017-04-27 22:36:07.000000 mleap-0.7.0/mleap.egg-info/top_level.txt
--rw-r--r--   0 mikhail    (501) staff       (20)      859 2017-04-27 22:36:07.000000 mleap-0.7.0/PKG-INFO
--rw-r--r--   0 mikhail    (501) staff       (20)       79 2017-04-27 22:36:07.000000 mleap-0.7.0/setup.cfg
--rw-r--r--   0 mikhail    (501) staff       (20)     2516 2017-04-27 20:00:53.000000 mleap-0.7.0/setup.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/
+-rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/__init__.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/bundle/
+-rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/bundle/__init__.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     7918 2017-09-21 17:54:17.000000 mleap-0.8.1/mleap/bundle/serialize.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/pyspark/
+-rw-r--r--   0 mikhail    (501) staff       (20)      231 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/pyspark/__init__.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     2228 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/pyspark/feature.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     1804 2017-06-11 21:40:39.000000 mleap-0.8.1/mleap/pyspark/spark_support.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/sklearn/
+-rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/__init__.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     3532 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/base.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     8965 2017-09-21 17:54:17.000000 mleap-0.8.1/mleap/sklearn/base_tests.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/sklearn/decomposition/
+-rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/decomposition/__init__.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     2420 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/decomposition/pca.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/sklearn/ensemble/
+-rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/ensemble/__init__.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     4147 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/ensemble/forest.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/sklearn/extensions/
+-rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/extensions/__init__.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     3719 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/extensions/data.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/sklearn/feature_extraction/
+-rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/feature_extraction/__init__.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     2397 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/feature_extraction/text.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     2336 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/feature_union.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     4059 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/logistic.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     6217 2017-09-21 17:54:17.000000 mleap-0.8.1/mleap/sklearn/pipeline.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/sklearn/preprocessing/
+-rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/preprocessing/__init__.py
+-rw-r--r--   0 mikhail    (501) staff       (20)    39368 2017-09-21 17:54:17.000000 mleap-0.8.1/mleap/sklearn/preprocessing/data.py
+-rw-r--r--   0 mikhail    (501) staff       (20)    39328 2017-09-21 17:54:17.000000 mleap-0.8.1/mleap/sklearn/preprocessing/tests.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     3879 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/svm.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/sklearn/tree/
+-rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/tree/__init__.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     5126 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/sklearn/tree/tree.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap/tensorflow/
+-rw-r--r--   0 mikhail    (501) staff       (20)        0 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/tensorflow/__init__.py
+-rw-r--r--   0 mikhail    (501) staff       (20)     2609 2017-04-27 20:00:53.000000 mleap-0.8.1/mleap/tensorflow/test.py
+-rw-r--r--   0 mikhail    (501) staff       (20)      828 2017-10-09 04:23:22.000000 mleap-0.8.1/mleap/version.py
+drwxr-xr-x   0 mikhail    (501) staff       (20)        0 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap.egg-info/
+-rw-r--r--   0 mikhail    (501) staff       (20)        1 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhail    (501) staff       (20)        1 2016-12-18 00:51:55.000000 mleap-0.8.1/mleap.egg-info/not-zip-safe
+-rw-r--r--   0 mikhail    (501) staff       (20)      859 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap.egg-info/PKG-INFO
+-rw-r--r--   0 mikhail    (501) staff       (20)      118 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap.egg-info/requires.txt
+-rw-r--r--   0 mikhail    (501) staff       (20)     1062 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhail    (501) staff       (20)        6 2017-10-09 04:28:30.000000 mleap-0.8.1/mleap.egg-info/top_level.txt
+-rw-r--r--   0 mikhail    (501) staff       (20)      859 2017-10-09 04:28:30.000000 mleap-0.8.1/PKG-INFO
+-rw-r--r--   0 mikhail    (501) staff       (20)      100 2017-10-09 04:28:30.000000 mleap-0.8.1/setup.cfg
+-rw-r--r--   0 mikhail    (501) staff       (20)     2516 2017-04-27 20:00:53.000000 mleap-0.8.1/setup.py
```

### Comparing `mleap-0.7.0/mleap/pyspark/feature.py` & `mleap-0.8.1/mleap/pyspark/feature.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/pyspark/spark_support.py` & `mleap-0.8.1/mleap/pyspark/spark_support.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 
 
 def serializeToBundle(self, path, dataset=None):
     serializer = SimpleSparkSerializer()
     serializer.serializeToBundle(self, path, dataset=dataset)
 
 
-def deserializeFromBundle(self, path):
+def deserializeFromBundle(path):
     serializer = SimpleSparkSerializer()
     return serializer.deserializeFromBundle(path)
 
 setattr(Transformer, 'serializeToBundle', serializeToBundle)
-setattr(Transformer.__class__, 'deserializeFromBundle', deserializeFromBundle)
+setattr(Transformer, 'deserializeFromBundle', staticmethod(deserializeFromBundle))
 
 
 class SimpleSparkSerializer(object):
     def __init__(self):
         super(SimpleSparkSerializer, self).__init__()
         self._java_obj = _jvm().ml.combust.mleap.spark.SimpleSparkSerializer()
```

### Comparing `mleap-0.7.0/mleap/sklearn/base.py` & `mleap-0.8.1/mleap/sklearn/base.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/sklearn/base_tests.py` & `mleap-0.8.1/mleap/sklearn/base_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import json
 import uuid
 
 from sklearn.linear_model import LinearRegression, LogisticRegression, LogisticRegressionCV
 from sklearn.preprocessing import Binarizer
 from mleap.sklearn.base import LinearRegression
 from mleap.sklearn.logistic import LogisticRegression, LogisticRegressionCV
-from mleap.sklearn.preprocessing.data import Binarizer
+from mleap.sklearn.preprocessing.data import FeatureExtractor, Binarizer
 
 
 class TransformerTests(unittest.TestCase):
     def setUp(self):
         self.df = pd.DataFrame(np.random.randn(10, 5), columns=['a', 'b', 'c', 'd', 'e'])
         self.tmp_dir = "/tmp/mleap.python.tests/{}".format(uuid.uuid1())
 
@@ -44,159 +44,179 @@
     def tearDown(self):
         shutil.rmtree(self.tmp_dir)
         pass
 
     def test_linear_regression_serializer(self):
 
         linear_regression = LinearRegression(fit_intercept=True, normalize=False)
-        linear_regression.mlinit(input_features=['a', 'b', 'c'],
-                                 prediction_column=['e'])
+        linear_regression.mlinit(input_features='a',
+                                 prediction_column='e')
 
-        linear_regression.fit(self.df[linear_regression.input_features], self.df[linear_regression.prediction_column])
+        linear_regression.fit(self.df[['a']], self.df[['e']])
 
         linear_regression.serialize_to_bundle(self.tmp_dir, linear_regression.name)
 
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, linear_regression.name)) as json_data:
             model = json.load(json_data)
 
         self.assertEqual(model['op'], 'linear_regression')
-        self.assertTrue(model['attributes']['intercept']['value'] is not None)
+        self.assertTrue(model['attributes']['intercept']['double'] is not None)
 
     def test_linear_regression_deserializer(self):
 
         linear_regression = LinearRegression(fit_intercept=True, normalize=False)
-        linear_regression.mlinit(input_features=['a', 'b', 'c'],
-                                 prediction_column=['e'])
+        linear_regression.mlinit(input_features='a',
+                                 prediction_column='e')
 
-        linear_regression.fit(self.df[linear_regression.input_features], self.df[linear_regression.prediction_column])
+        linear_regression.fit(self.df[['a']], self.df[['e']])
 
         linear_regression.serialize_to_bundle(self.tmp_dir, linear_regression.name)
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, linear_regression.name)) as json_data:
             model = json.load(json_data)
 
         # Now deserialize it back
         node_name = "{}.node".format(linear_regression.name)
         linear_regression_tf = LinearRegression()
         linear_regression_tf = linear_regression_tf.deserialize_from_bundle(self.tmp_dir, node_name)
 
-        res_a = linear_regression.predict(self.df[linear_regression.input_features])
-        res_b = linear_regression_tf.predict(self.df[linear_regression_tf.input_features])
+        res_a = linear_regression.predict(self.df[['a']])
+        res_b = linear_regression_tf.predict(self.df[['a']])
 
         self.assertEqual(res_a[0], res_b[0])
         self.assertEqual(res_a[1], res_b[1])
         self.assertEqual(res_a[2], res_b[2])
 
     def test_logistic_regression_serializer(self):
 
         logistic_regression = LogisticRegression(fit_intercept=True)
-        logistic_regression.mlinit(input_features=['a', 'b', 'c'],
-                                 prediction_column=['e_binary'])
+        logistic_regression.mlinit(input_features='a',
+                                 prediction_column='e_binary')
+
+        extract_features = ['e']
+        feature_extractor = FeatureExtractor(input_scalars=['e'],
+                                         output_vector='extracted_e_output',
+                                         output_vector_items=["{}_out".format(x) for x in extract_features])
 
         binarizer = Binarizer(threshold=0.0)
-        binarizer.mlinit(input_features=['e'],
-                         output_features=['e_binary'])
+        binarizer.mlinit(prior_tf=feature_extractor,
+                         output_features='e_binary')
 
         Xres = binarizer.fit_transform(self.df[['a']])
 
-        logistic_regression.fit(self.df[logistic_regression.input_features], Xres)
+        logistic_regression.fit(self.df[['a']], Xres)
 
         logistic_regression.serialize_to_bundle(self.tmp_dir, logistic_regression.name)
 
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, logistic_regression.name)) as json_data:
             model = json.load(json_data)
 
         self.assertEqual(model['op'], 'logistic_regression')
-        self.assertTrue(model['attributes']['intercept']['value'] is not None)
+        self.assertTrue(model['attributes']['intercept']['double'] is not None)
 
     def test_logistic_regression_deserializer(self):
 
         logistic_regression = LogisticRegression(fit_intercept=True)
-        logistic_regression.mlinit(input_features=['a', 'b', 'c'],
-                                   prediction_column=['e_binary'])
+        logistic_regression.mlinit(input_features='a',
+                                   prediction_column='e_binary')
+
+        extract_features = ['e']
+        feature_extractor = FeatureExtractor(input_scalars=['e'],
+                                         output_vector='extracted_e_output',
+                                         output_vector_items=["{}_out".format(x) for x in extract_features])
 
         binarizer = Binarizer(threshold=0.0)
-        binarizer.mlinit(input_features=['e'],
-                         output_features=['e_binary'])
+        binarizer.mlinit(prior_tf=feature_extractor,
+                         output_features='e_binary')
 
         Xres = binarizer.fit_transform(self.df[['a']])
 
-        logistic_regression.fit(self.df[logistic_regression.input_features], Xres)
+        logistic_regression.fit(self.df[['a']], Xres)
 
         logistic_regression.serialize_to_bundle(self.tmp_dir, logistic_regression.name)
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, logistic_regression.name)) as json_data:
             model = json.load(json_data)
 
         # Now deserialize it back
         node_name = "{}.node".format(logistic_regression.name)
         logistic_regression_tf = LogisticRegression()
         logistic_regression_tf = logistic_regression_tf.deserialize_from_bundle(self.tmp_dir, node_name)
 
-        res_a = logistic_regression.predict(self.df[logistic_regression.input_features])
-        res_b = logistic_regression_tf.predict(self.df[logistic_regression_tf.input_features])
+        res_a = logistic_regression.predict(self.df[['a']])
+        res_b = logistic_regression_tf.predict(self.df[['a']])
 
         self.assertEqual(res_a[0], res_b[0])
         self.assertEqual(res_a[1], res_b[1])
         self.assertEqual(res_a[2], res_b[2])
 
     def test_logistic_regression_cv_serializer(self):
 
         logistic_regression = LogisticRegressionCV(fit_intercept=True)
-        logistic_regression.mlinit(input_features=['a', 'b', 'c'],
-                                 prediction_column=['e_binary'])
+        logistic_regression.mlinit(input_features='a',
+                                 prediction_column='e_binary')
+
+        extract_features = ['e']
+        feature_extractor = FeatureExtractor(input_scalars=['e'],
+                                             output_vector='extracted_e_output',
+                                             output_vector_items=["{}_out".format(x) for x in extract_features])
 
         binarizer = Binarizer(threshold=0.0)
-        binarizer.mlinit(input_features=['e'],
-                         output_features=['e_binary'])
+        binarizer.mlinit(prior_tf=feature_extractor,
+                         output_features='e_binary')
 
         Xres = binarizer.fit_transform(self.df[['a']])
 
-        logistic_regression.fit(self.df[logistic_regression.input_features], Xres)
+        logistic_regression.fit(self.df[['a']], Xres)
 
         logistic_regression.serialize_to_bundle(self.tmp_dir, logistic_regression.name)
 
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, logistic_regression.name)) as json_data:
             model = json.load(json_data)
 
         self.assertEqual(model['op'], 'logistic_regression')
-        self.assertTrue(model['attributes']['intercept']['value'] is not None)
+        self.assertTrue(model['attributes']['intercept']['double'] is not None)
 
     def test_logistic_regression_cv_deserializer(self):
 
         logistic_regression = LogisticRegressionCV(fit_intercept=True)
-        logistic_regression.mlinit(input_features=['a', 'b', 'c'],
-                                   prediction_column=['e_binary'])
+        logistic_regression.mlinit(input_features='a',
+                                   prediction_column='e_binary')
+
+        extract_features = ['e']
+        feature_extractor = FeatureExtractor(input_scalars=['e'],
+                                             output_vector='extracted_e_output',
+                                             output_vector_items=["{}_out".format(x) for x in extract_features])
 
         binarizer = Binarizer(threshold=0.0)
-        binarizer.mlinit(input_features=['e'],
-                         output_features=['e_binary'])
+        binarizer.mlinit(prior_tf=feature_extractor,
+                         output_features='e_binary')
 
         Xres = binarizer.fit_transform(self.df[['a']])
 
-        logistic_regression.fit(self.df[logistic_regression.input_features], Xres)
+        logistic_regression.fit(self.df[['a']], Xres)
 
         logistic_regression.serialize_to_bundle(self.tmp_dir, logistic_regression.name)
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, logistic_regression.name)) as json_data:
             model = json.load(json_data)
 
         # Now deserialize it back
         node_name = "{}.node".format(logistic_regression.name)
         logistic_regression_tf = LogisticRegressionCV()
         logistic_regression_tf = logistic_regression_tf.deserialize_from_bundle(self.tmp_dir, node_name)
 
-        res_a = logistic_regression.predict(self.df[logistic_regression.input_features])
-        res_b = logistic_regression_tf.predict(self.df[logistic_regression_tf.input_features])
+        res_a = logistic_regression.predict(self.df[['a']])
+        res_b = logistic_regression_tf.predict(self.df[['a']])
 
         self.assertEqual(res_a[0], res_b[0])
         self.assertEqual(res_a[1], res_b[1])
         self.assertEqual(res_a[2], res_b[2])
```

### Comparing `mleap-0.7.0/mleap/sklearn/decomposition/pca.py` & `mleap-0.8.1/mleap/sklearn/decomposition/pca.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/sklearn/ensemble/forest.py` & `mleap-0.8.1/mleap/sklearn/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/sklearn/extensions/data.py` & `mleap-0.8.1/mleap/sklearn/extensions/data.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/sklearn/feature_extraction/text.py` & `mleap-0.8.1/mleap/sklearn/feature_extraction/text.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/sklearn/feature_union.py` & `mleap-0.8.1/mleap/sklearn/feature_union.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/sklearn/logistic.py` & `mleap-0.8.1/mleap/sklearn/logistic.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/sklearn/pipeline.py` & `mleap-0.8.1/mleap/sklearn/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from sklearn.pipeline import Pipeline
 from mleap.version import __version__
 import os
 import json
 import shutil
 import uuid
 import zipfile
-
+import datetime
 
 def serialize_to_bundle(self, path, model_name, init=False):
     serializer = SimpleSerializer()
     serializer.serialize_to_bundle(self, path, model_name, init)
 
 
 def deserialize_from_bundle(self, path):
@@ -122,14 +122,15 @@
 
     @staticmethod
     def get_bundle(transformer):
         js = {
           "name": transformer.name,
           "format": "json",
           "version": __version__,
+          "timestamp": datetime.datetime.now().isoformat(),
           "uid": "{}".format(uuid.uuid4())
         }
         return js
 
     @staticmethod
     def get_node(transformer):
         js = {
@@ -142,33 +143,30 @@
         return js
 
     def get_model(self, transformer):
         js = {
           "op": transformer.op,
             "attributes": {
                 "nodes": {
-                    "type": {
-                        "type": "list",
-                        "base": "string"
-                    },
-                    "value": self._extract_nodes(transformer.steps)
+                    "type": "list",
+                    "string": self._extract_nodes(transformer.steps)
                 }
             }
         }
         return js
 
     @staticmethod
     def _extract_nodes(steps):
         pipeline_steps = []
         for name, step in steps:
             if step.op == 'feature_union':
                 union_steps = [x[1].name for x in step.transformer_list if hasattr(x[1], 'serialize_to_bundle') and x[1].serializable]
                 pipeline_steps += union_steps
             elif hasattr(step, 'serialize_to_bundle') and step.serializable:
-                pipeline_steps.append(name)
+                pipeline_steps.append(step.name)
         return pipeline_steps
 
 
 def zip_pipeline(path, name):
     zip_file = zipfile.ZipFile("{}/{}.zip".format(path, name), 'w', zipfile.ZIP_DEFLATED)
     abs_src = os.path.abspath("{}/{}".format(path, name))
     for root, dirs, files in os.walk("{}/{}".format(path, name)):
```

### Comparing `mleap-0.7.0/mleap/sklearn/preprocessing/data.py` & `mleap-0.8.1/mleap/sklearn/preprocessing/data.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 #
 
 from sklearn.preprocessing.data import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, Imputer, Binarizer, PolynomialFeatures
 from sklearn.preprocessing.data import OneHotEncoder
 from sklearn.preprocessing.label import LabelEncoder
-from mleap.bundle.serialize import MLeapSerializer, MLeapDeserializer
+from mleap.bundle.serialize import MLeapSerializer, MLeapDeserializer, Vector
 from sklearn.utils import column_or_1d
 from sklearn.utils.validation import check_is_fitted
 from sklearn.utils.fixes import np_version
 import warnings
 import numpy as np
 import pandas as pd
 import uuid
@@ -67,19 +67,46 @@
 
 
 def deserialize_from_bundle(self, path, node_name):
     serializer = SimpleSerializer()
     return serializer.deserialize_from_bundle(self, path, node_name)
 
 
-def mleap_init(self, input_features, output_features):
-    self.input_features = input_features
-    self.output_features = output_features
+def mleap_init(self, prior_tf, output_features=None):
+
     self.name = "{}_{}".format(self.op, uuid.uuid1())
 
+    if prior_tf.op == 'vector_assembler':
+        self.input_features = prior_tf.output_vector
+        output_shape = 'tensor'
+        output_size = len(prior_tf.input_features)
+        output_feature_name = prior_tf.output_vector
+
+    else:
+        self.input_features = prior_tf.output_features
+        output_shape = 'scalar'
+        output_size = 1
+        output_feature_name = prior_tf.output_features
+
+    class_name = "{}".format(self.__init__.im_class).split('.')[-1].replace('>','').replace("'",'')
+
+    if output_features is not None:
+        self.output_features = output_features
+    else:
+        self.output_features = "{}_{}".format(output_feature_name, class_name.lower())
+
+    if class_name == 'PolynomialFeatures':
+        self.input_size = len(prior_tf.input_features)
+
+    elif output_shape == 'tensor':
+        self.input_shapes = {'data_shape': [{'shape':'tensor',
+                                                 "tensor_shape": {"dimensions": [{"size": output_size}]}}]}
+    else:
+        self.input_shapes = {'data_shape': [{'shape': output_shape}]}
+
 
 setattr(StandardScaler, 'op', ops.STANDARD_SCALER)
 setattr(StandardScaler, 'serialize_to_bundle', serialize_to_bundle)
 setattr(StandardScaler, 'deserialize_from_bundle', deserialize_from_bundle)
 setattr(StandardScaler, 'mlinit', mleap_init)
 setattr(StandardScaler, 'serializable', True)
 
@@ -162,60 +189,104 @@
 def _to_list(x):
     if isinstance(x, list):
         return x
     return list(x)
 
 
 class FeatureExtractor(BaseEstimator, TransformerMixin, MLeapSerializer):
-    def __init__(self, input_features, output_vector, output_vector_items):
+    def __init__(self, input_scalars=None, input_vectors=None, output_vector=None, output_vector_items=None):
         """
         Selects a subset of features from a pandas dataframe that are then passed into a subsequent transformer.
         MLeap treats this transformer like a VectorAssembler equivalent in spark.
         >>> data = pd.DataFrame([['a', 0, 1], ['b', 1, 2], ['c', 3, 4]], columns=['col_a', 'col_b', 'col_c'])
         >>> vector_items = ['col_b', 'col_c']
-        >>> feature_extractor2_tf = FeatureExtractor(vector_items, 'continuous_features', vector_items)
+        >>> input_shapes = {'data_shape': [{'shape':'scalar'}, {'shape':'scalar'}]}
+        >>> input_shapes = {'data_shape': [{'shape':'tensor', "tensor_shape": {"dimensions": [{"size": 23}]}}]}
+        >>> feature_extractor2_tf = FeatureExtractor(vector_items, 'continuous_features', vector_items, input_shapes)
         >>> feature_extractor2_tf.fit_transform(data).head(1).values
         >>> array([[0, 1]])
+        :param input_vectors: List of scalar feature names that are being extracted from a DataFrame
+        :param input_vectors: List of FeatureExtractors that were used to generate the input vectors
         :param input_features: List of features to extracts from a pandas data frame
         :param output_vector: Name of the output vector, only used for serialization
         :param output_vector_items: List of output feature names
+        :param input_shapes: the shape of each input feature, whether it is scalar or a vector
+        if it's a vector, then we include size information of the vector
         :return:
         """
-        self.input_features = input_features
+        self.input_scalars = input_scalars
+        self.input_vectors = input_vectors
+        self.input_features = self.get_input_features(input_scalars, input_vectors)
         self.output_vector_items = output_vector_items
         self.output_vector = output_vector
         self.op = 'vector_assembler'
         self.name = "{}_{}".format(self.op, uuid.uuid1())
         self.dtypes = None
         self.serializable = True
         self.skip_fit_transform = False
+        self.input_size = None
+        self.input_shapes = None
+
+    def get_input_features(self, input_scalars, input_vectors):
+        if input_scalars is not None:
+            return input_scalars
+        elif input_vectors is not None and isinstance(input_vectors, list) and len(input_vectors)>0:
+            features = list()
+            for x in input_vectors:
+                if 'output_vector' in x.__dict__:
+                    features.append(x.output_vector)
+                elif 'output_features' in x.__dict__:
+                    features.append(x.output_features)
+            return features
+        else:
+            raise BaseException("Unable To Define Input Features")
 
     def transform(self, df, **params):
         if not self.skip_fit_transform:
             return df[self.input_features]
         return df
 
-    def fit(self, df, y=None, **fit_params):
+    def assign_input_shapes(self, X):
+        # Figure out the data shape
+        if self.input_scalars is not None and isinstance(X, pd.DataFrame):
+            self.input_shapes = {'data_shape': [{'shape': 'scalar'}]*len(self.input_features)}
+
+        elif self.input_vectors is not None:
+            self.input_shapes = {'data_shape': []}
+            for vector in self.input_vectors:
+                if vector.op not in [ops.ONE_HOT_ENCODER, ops.POLYNOMIALEXPANSION]:
+                    shape = {'shape': 'tensor', "tensor_shape": {"dimensions": [{"size": len(vector.input_features)}]}}
+                    self.input_shapes['data_shape'].append(shape)
+                elif vector.op == ops.ONE_HOT_ENCODER:
+                    shape = {'shape': 'tensor', "tensor_shape": {"dimensions": [{"size": vector.n_values_[0] - 1}]}}
+                    self.input_shapes['data_shape'].append(shape)
+        return self
+
+    def fit(self, X, y=None, **fit_params):
+        self.assign_input_shapes(X)
         if not self.skip_fit_transform:
-            self.dtypes = df[self.input_features].dtypes.to_dict()
+            self.dtypes = X[self.input_features].dtypes.to_dict()
             if len([x for x in self.dtypes.values() if x.type == np.object_]) != 0:
                 self.serializable = False
         return self
 
     def fit_transform(self, X, y=None, **fit_params):
         if not self.skip_fit_transform:
             self.fit(X)
+        else:
+            self.assign_input_shapes(X)
 
         df_subset = self.transform(X)
         return df_subset
 
     def serialize_to_bundle(self, path, model_name):
 
         # compile tuples of model attributes to serialize
-        attributes = None
+        attributes = list()
+        attributes.append(("input_shapes", self.input_shapes))
 
         # define node inputs and outputs
         inputs = [{'name': x, 'port': 'input{}'.format(self.input_features.index(x))} for x in self.input_features]
 
         outputs = [{
                   "name": self.output_vector,
                   "port": "output"
@@ -232,16 +303,15 @@
     Converts categorical values of a single column into categorical indices. This transformer should be followed by a
     NDArrayToDataFrame transformer to maintain a data structure required by scikit pipelines.
 
     NOTE: You can only LabelEncode/String Index one feature at a time!!!
 
     >>> data = pd.DataFrame([['a', 0], ['b', 1], ['b', 3], ['c', 1]], columns=['col_a', 'col_b'])
     >>> # Label Encoder for x1 Label
-    >>> label_encoder_tf = LabelEncoder()
-    >>> label_encoder_tf.mlinit(input_features = ['col_a'] , output_features='col_a_label_le')
+    >>> label_encoder_tf = LabelEncoder(input_features = ['col_a'] , output_features='col_a_label_le')
     >>> # Convert output of Label Encoder to Data Frame instead of 1d-array
     >>> n_dim_array_to_df_tf = NDArrayToDataFrame('col_a_label_le')
     >>> n_dim_array_to_df_tf.fit_transform(label_encoder_tf.fit_transform(data['col_a']))
 
     Encode labels with value between 0 and n_classes-1.
 
     Read more in the :ref:`User Guide <preprocessing_targets>`.
@@ -365,14 +435,15 @@
         return self.classes_[y]
 
     def serialize_to_bundle(self, path, model_name):
 
         # compile tuples of model attributes to serialize
         attributes = list()
         attributes.append(('labels', self.classes_.tolist()))
+        attributes.append(('nullable_input', False))
 
         # define node inputs and outputs
         inputs = [{
                   "name": self.input_features[0],
                   "port": "input"
                 }]
 
@@ -460,16 +531,16 @@
 
     def serialize_to_bundle(self, transformer, path, model_name):
 
         # compile tuples of model attributes to serialize
         attributes = list()
         attributes.append(('strategy', transformer.strategy))
         attributes.append(('surrogate_value', transformer.statistics_.tolist()[0]))
-        if transformer.missing_values is not np.NaN:
-            attributes.append(('missing_value', transformer.missing_values[0]))
+        if transformer.missing_values is not "NaN":
+            attributes.append(('missing_value', transformer.missing_values))
 
         # define node inputs and outputs
         inputs = [{
                   "name": transformer.input_features,
                   "port": "input"
                 }]
 
@@ -592,19 +663,22 @@
         return transformer
 
 
 class BinarizerSerializer(MLeapSerializer, MLeapDeserializer):
     def __init__(self):
         super(BinarizerSerializer, self).__init__()
 
+
+
     def serialize_to_bundle(self, transformer, path, model_name):
 
         # compile tuples of model attributes to serialize
         attributes = list()
         attributes.append(('threshold', transformer.threshold))
+        attributes.append(("input_shapes", transformer.input_shapes))
 
         # define node inputs and outputs
         inputs = [{
                   "name": transformer.input_features,
                   "port": "input"
                 }]
 
@@ -628,14 +702,15 @@
         super(PolynomialExpansionSerializer, self).__init__()
 
     def serialize_to_bundle(self, transformer, path, model_name):
 
         # compile tuples of model attributes to serialize
         attributes = list()
         attributes.append(('degree', transformer.degree))
+        attributes.append(('input_size', transformer.input_size))
 
         # define node inputs and outputs
         inputs = [{
                   "name": transformer.input_features,
                   "port": "input"
                 }]
 
@@ -987,7 +1062,60 @@
         attributes_map = {
             'operation': 'transform_type'
         }
         full_node_path = os.path.join(node_path, node_name)
         transformer = self.deserialize_single_input_output(self, full_node_path, attributes_map)
         return transformer
 
+class StringMap(BaseEstimator, TransformerMixin, MLeapSerializer, MLeapDeserializer):
+
+    def __init__(self, input_features=None, output_features=None, labels=None):
+        self.op = 'string_map'
+        self.name = "{}_{}".format(self.op, uuid.uuid4())
+        self.input_features = input_features
+        self.output_features = output_features
+        self.serializable = True
+        self.labels = labels
+        if labels is not None:
+            self.label_keys = self.labels.keys
+            self.label_values = self.labels.values
+
+    def fit(self, y):
+        if self.labels is None:
+            self.labels = dict(zip(self.label_keys, self.label_values))
+        return self
+
+    def transform(self, y):
+       return y.applymap(lambda input : self.labels[input]).values
+
+    def fit_transform(self, X, y=None, **fit_params):
+        self.fit(X)
+        return self.transform(X)
+
+    def serialize_to_bundle(self, path, model_name):
+        # compile tuples of model attributes to serialize
+        attributes = list()
+        attributes.append(("labels", self.labels.keys()))
+        attributes.append(("values", Vector(self.labels.values())))
+
+        # define node inputs and outputs
+        inputs = [{
+            "name": self.input_features[0],
+            "port": "input"
+        }]
+
+        outputs = [{
+            "name": self.output_features[0],
+            "port": "output"
+        }]
+
+        self.serialize(self, path, model_name, attributes, inputs, outputs)
+
+    def deserialize_from_bundle(self, node_path, node_name):
+        attributes_map = {
+            'labels': 'label_keys',
+            'values': 'label_values'
+        }
+
+        full_node_path = os.path.join(node_path, node_name)
+        transformer = self.deserialize_single_input_output(self, full_node_path, attributes_map)
+        return transformer
```

### Comparing `mleap-0.7.0/mleap/sklearn/preprocessing/tests.py` & `mleap-0.8.1/mleap/sklearn/preprocessing/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import numpy as np
 import os
 import shutil
 import json
 import uuid
 
 import mleap.sklearn.preprocessing.data
-from mleap.sklearn.preprocessing.data import FeatureExtractor, MathUnary, MathBinary
+from mleap.sklearn.preprocessing.data import FeatureExtractor, MathUnary, MathBinary, StringMap
 from mleap.sklearn.preprocessing.data import StandardScaler, MinMaxScaler, LabelEncoder, Imputer, Binarizer, PolynomialFeatures
 from mleap.sklearn.preprocessing.data import OneHotEncoder
 
 
 class TransformerTests(unittest.TestCase):
     def setUp(self):
         self.df = pd.DataFrame(np.random.randn(10, 5), columns=['a', 'b', 'c', 'd', 'e'])
@@ -45,88 +45,90 @@
 
     def test_standard_scaler_serializer(self):
 
         standard_scaler = StandardScaler(with_mean=True,
                                          with_std=True
                                          )
 
-        standard_scaler.mlinit(input_features='a',
+        extract_features = ['a']
+        feature_extractor = FeatureExtractor(input_scalars=['a'],
+                                             output_vector='extracted_a_output',
+                                             output_vector_items=["{}_out".format(x) for x in extract_features])
+
+        standard_scaler.mlinit(prior_tf=feature_extractor,
                                output_features='a_scaled')
 
         standard_scaler.fit(self.df[['a']])
 
         standard_scaler.serialize_to_bundle(self.tmp_dir, standard_scaler.name)
 
         expected_mean = self.df.a.mean()
         expected_std = np.sqrt(np.var(self.df.a))
 
         expected_model = {
             "op": "standard_scaler",
             "attributes": {
                 "mean": {
-                    "type": {
-                        "type": "tensor",
-                        "tensor": {
-                           "base": "double"
-                        }
-                     },
-                     "value": {
-                         "values": [expected_mean],
-                         "dimensions": [
-                             1
-                         ]
-                     }
+                    "double": [expected_mean],
+                    "shape": {
+                        "dimensions": [{
+                            "size": 1,
+                            "name": ""
+                        }]
+                    },
+                    "type": "tensor"
                 },
                 "std": {
-                    "type": {
-                        "type": "tensor",
-                        "tensor": {
-                           "base": "double"
-                        }
-                     },
-                     "value": {
-                         "values": [expected_std],
-                         "dimensions": [
-                             1
-                         ]
-                     }
+                    "double": [expected_std],
+                    "shape": {
+                        "dimensions": [{
+                            "size": 1,
+                            "name": ""
+                        }]
+                    },
+                    "type": "tensor"
                 }
             }
         }
 
         self.assertAlmostEqual(expected_mean, standard_scaler.mean_.tolist()[0], places = 7)
         self.assertAlmostEqual(expected_std, np.sqrt(standard_scaler.var_.tolist()[0]), places = 7)
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, standard_scaler.name)) as json_data:
             model = json.load(json_data)
 
         self.assertEqual(standard_scaler.op, expected_model['op'])
-        self.assertEqual(expected_model['attributes']['mean']['value']['dimensions'][0], model['attributes']['mean']['value']['dimensions'][0])
-        self.assertEqual(expected_model['attributes']['std']['value']['dimensions'][0], model['attributes']['std']['value']['dimensions'][0])
-        self.assertAlmostEqual(expected_model['attributes']['mean']['value']['values'][0], model['attributes']['mean']['value']['values'][0], places = 7)
-        self.assertAlmostEqual(expected_model['attributes']['std']['value']['values'][0], model['attributes']['std']['value']['values'][0], places = 7)
+        self.assertEqual(expected_model['attributes']['mean']['shape']['dimensions'][0]['size'], model['attributes']['mean']['shape']['dimensions'][0]['size'])
+        self.assertEqual(expected_model['attributes']['std']['shape']['dimensions'][0]['size'], model['attributes']['std']['shape']['dimensions'][0]['size'])
+        self.assertAlmostEqual(expected_model['attributes']['mean']['double'][0], model['attributes']['mean']['double'][0], places = 7)
+        self.assertAlmostEqual(expected_model['attributes']['std']['double'][0], model['attributes']['std']['double'][0], places = 7)
 
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, standard_scaler.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(standard_scaler.name, node['name'])
         self.assertEqual(standard_scaler.input_features, node['shape']['inputs'][0]['name'])
         self.assertEqual(standard_scaler.output_features, node['shape']['outputs'][0]['name'])
 
     def test_standard_scaler_deserializer(self):
 
+        extract_features = ['a']
+        feature_extractor = FeatureExtractor(input_scalars=['a'],
+                                         output_vector='extracted_a_output',
+                                         output_vector_items=["{}_out".format(x) for x in extract_features])
+
         # Serialize a standard scaler to a bundle
         standard_scaler = StandardScaler(with_mean=True,
                                          with_std=True
                                          )
 
-        standard_scaler.mlinit(input_features=['a'],
-                               output_features=['a_scaled'])
+        standard_scaler.mlinit(prior_tf=feature_extractor,
+                               output_features='a_scaled')
 
         standard_scaler.fit(self.df[['a']])
 
         standard_scaler.serialize_to_bundle(self.tmp_dir, standard_scaler.name)
 
         # Now deserialize it back
 
@@ -144,20 +146,25 @@
         self.assertEqual(standard_scaler.name, standard_scaler_tf.name)
         self.assertEqual(standard_scaler.op, standard_scaler_tf.op)
         self.assertEqual(standard_scaler.mean_, standard_scaler_tf.mean_)
         self.assertEqual(standard_scaler.scale_, standard_scaler_tf.scale_)
 
     def test_standard_scaler_multi_deserializer(self):
 
+        extract_features = ['a', 'b']
+        feature_extractor = FeatureExtractor(input_scalars=['a', 'b'],
+                                             output_vector='extracted_multi_outputs',
+                                             output_vector_items=["{}_out".format(x) for x in extract_features])
+
         # Serialize a standard scaler to a bundle
         standard_scaler = StandardScaler(with_mean=True,
                                          with_std=True
                                          )
 
-        standard_scaler.mlinit(input_features=['a', 'b'],
+        standard_scaler.mlinit(prior_tf=feature_extractor,
                                output_features=['a_scaled', 'b_scaled'])
 
         standard_scaler.fit(self.df[['a', 'b']])
 
         standard_scaler.serialize_to_bundle(self.tmp_dir, standard_scaler.name)
 
         # Now deserialize it back
@@ -179,148 +186,87 @@
         self.assertEqual(standard_scaler.mean_[0], standard_scaler_tf.mean_[0])
         self.assertEqual(standard_scaler.mean_[1], standard_scaler_tf.mean_[1])
         self.assertEqual(standard_scaler.scale_[0], standard_scaler_tf.scale_[0])
         self.assertEqual(standard_scaler.scale_[1], standard_scaler_tf.scale_[1])
 
     def test_min_max_scaler_serializer(self):
 
-        scaler = MinMaxScaler()
-        scaler.mlinit(input_features=['a'],
-                      output_features=['a_scaled'])
-
-        scaler.fit(self.df[['a']])
-
-        scaler.serialize_to_bundle(self.tmp_dir, scaler.name)
-
-        expected_min = self.df.a.min()
-        expected_max = self.df.a.max()
-
-        expected_model = {
-           "op": "min_max_scaler",
-            "attributes": {
-                "min": {
-                         "type": {
-                            "type": "tensor",
-                            "tensor": {
-                               "base": "double",
-                               "dimensions": [
-                                  -1
-                               ]
-                            }
-                         },
-                         "value": [expected_min]
-                      },
-                "max": {
-                         "type": {
-                            "type": "tensor",
-                            "tensor": {
-                               "base": "double",
-                               "dimensions": [
-                                  -1
-                               ]
-                            }
-                         },
-                         "value": [expected_max]
-                      }
-            }
-        }
-
-        self.assertEqual(expected_min, scaler.data_min_.tolist()[0])
-        self.assertEqual(expected_max, scaler.data_max_.tolist()[0])
-
-        # Test model.json
-        with open("{}/{}.node/model.json".format(self.tmp_dir, scaler.name)) as json_data:
-            model = json.load(json_data)
-
-        self.assertEqual(scaler.op, expected_model['op'])
-        self.assertEqual(expected_model['attributes']['min']['type']['tensor']['dimensions'][0], model['attributes']['min']['type']['tensor']['dimensions'][0])
-        self.assertEqual(expected_model['attributes']['min']['value'][0], model['attributes']['min']['value'][0])
-        self.assertEqual(expected_model['attributes']['max']['value'][0], model['attributes']['max']['value'][0])
-
-        # Test node.json
-        with open("{}/{}.node/node.json".format(self.tmp_dir, scaler.name)) as json_data:
-            node = json.load(json_data)
-
-        self.assertEqual(scaler.name, node['name'])
-        self.assertEqual(scaler.input_features, node['shape']['inputs'][0]['name'])
-        self.assertEqual(scaler.output_features, node['shape']['outputs'][0]['name'])
-
-    def test_min_max_scaler_serializer(self):
+        extract_features = ['a']
+        feature_extractor = FeatureExtractor(input_scalars=['a'],
+                                         output_vector='extracted_a_output',
+                                         output_vector_items=["{}_out".format(x) for x in extract_features])
 
         scaler = MinMaxScaler()
-        scaler.mlinit(input_features='a',
+        scaler.mlinit(prior_tf = feature_extractor,
                       output_features='a_scaled')
 
         scaler.fit(self.df[['a']])
 
         scaler.serialize_to_bundle(self.tmp_dir, scaler.name)
 
         expected_min = self.df.a.min()
         expected_max = self.df.a.max()
 
         expected_model = {
            "op": "min_max_scaler",
             "attributes": {
                 "min": {
-                         "type": {
-                            "type": "tensor",
-                            "tensor": {
-                               "base": "double"
-                            }
-                         },
-                         "value": {
-                             "values": [expected_min],
-                             "dimensions": [
-                                 1
-                             ]
-                         }
-                      },
+                    "double": [expected_min],
+                    "shape": {
+                        "dimensions": [{
+                            "size": 1,
+                            "name": ""
+                        }]
+                    },
+                    "type": "tensor"
+                },
                 "max": {
-                         "type": {
-                            "type": "tensor",
-                            "tensor": {
-                               "base": "double"
-                            }
-                         },
-                         "value": {
-                             "values": [expected_max],
-                             "dimensions": [
-                                 1
-                             ]
-                         }
-                      }
+                    "double": [expected_max],
+                    "shape": {
+                        "dimensions": [{
+                            "size": 1,
+                            "name": ""
+                        }]
+                    },
+                    "type": "tensor"
+                }
             }
         }
 
-        self.assertAlmostEqual(expected_min, scaler.data_min_.tolist()[0], places = 7)
-        self.assertAlmostEqual(expected_max, scaler.data_max_.tolist()[0], places = 7)
+        self.assertEqual(expected_min, scaler.data_min_.tolist()[0])
+        self.assertEqual(expected_max, scaler.data_max_.tolist()[0])
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, scaler.name)) as json_data:
             model = json.load(json_data)
 
         self.assertEqual(scaler.op, expected_model['op'])
-        self.assertEqual(expected_model['attributes']['min']['value']['dimensions'][0], model['attributes']['min']['value']['dimensions'][0])
-        self.assertEqual(expected_model['attributes']['max']['value']['dimensions'][0], model['attributes']['max']['value']['dimensions'][0])
-        self.assertAlmostEqual(expected_model['attributes']['min']['value']['values'][0], model['attributes']['min']['value']['values'][0])
-        self.assertAlmostEqual(expected_model['attributes']['max']['value']['values'][0], model['attributes']['max']['value']['values'][0])
+        self.assertEqual(expected_model['attributes']['min']['shape']['dimensions'][0]['size'], model['attributes']['min']['shape']['dimensions'][0]['size'])
+        self.assertEqual(expected_model['attributes']['max']['shape']['dimensions'][0]['size'], model['attributes']['max']['shape']['dimensions'][0]['size'])
+        self.assertEqual(expected_model['attributes']['min']['double'][0], model['attributes']['min']['double'][0])
+        self.assertEqual(expected_model['attributes']['max']['double'][0], model['attributes']['max']['double'][0])
 
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, scaler.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(scaler.name, node['name'])
         self.assertEqual(scaler.input_features, node['shape']['inputs'][0]['name'])
         self.assertEqual(scaler.output_features, node['shape']['outputs'][0]['name'])
 
     def test_min_max_scaler_deserializer(self):
 
+        extract_features = ['a']
+        feature_extractor = FeatureExtractor(input_scalars=['a'],
+                                             output_vector='extracted_a_output',
+                                             output_vector_items=["{}_out".format(x) for x in extract_features])
+
         scaler = MinMaxScaler()
-        scaler.mlinit(input_features=['a'],
-                      output_features=['a_scaled'])
+        scaler.mlinit(prior_tf=feature_extractor,
+                      output_features='a_scaled')
 
         scaler.fit(self.df[['a']])
 
         scaler.serialize_to_bundle(self.tmp_dir, scaler.name)
 
         # Deserialize the MinMaxScaler
         node_name = "{}.node".format(scaler.name)
@@ -334,16 +280,21 @@
         self.assertEqual(res_a[0], res_b[0])
 
         self.assertEqual(scaler.name, min_max_scaler_tf.name)
         self.assertEqual(scaler.op, min_max_scaler_tf.op)
 
     def test_min_max_scaler_multi_deserializer(self):
 
+        extract_features = ['a', 'b']
+        feature_extractor = FeatureExtractor(input_scalars=['a', 'b'],
+                                             output_vector='extracted_multi_outputs',
+                                             output_vector_items=["{}_out".format(x) for x in extract_features])
+
         scaler = MinMaxScaler()
-        scaler.mlinit(input_features=['a', 'b'],
+        scaler.mlinit(prior_tf=feature_extractor,
                       output_features=['a_scaled', 'b_scaled'])
 
         scaler.fit(self.df[['a']])
 
         scaler.serialize_to_bundle(self.tmp_dir, scaler.name)
 
         # Deserialize the MinMaxScaler
@@ -361,36 +312,45 @@
         self.assertEqual(scaler.name, min_max_scaler_tf.name)
         self.assertEqual(scaler.op, min_max_scaler_tf.op)
 
     def label_encoder_test(self):
 
         labels = ['a', 'b', 'c']
 
-        le = LabelEncoder(input_features='label_feature',
+        le = LabelEncoder(input_features=['label_feature'],
                   output_features='label_feature_le_encoded')
 
         le.fit(labels)
 
         self.assertEqual(labels, le.classes_.tolist())
 
         le.serialize_to_bundle(self.tmp_dir, le.name)
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, le.name)) as json_data:
             model = json.load(json_data)
 
         self.assertEqual(le.op, model['op'])
-        self.assertEqual('labels', model['attributes'].keys()[0])
+        self.assertEqual('nullable_input', model['attributes'].keys()[0])
+        self.assertEqual('labels', model['attributes'].keys()[1])
+
+        # Test node.json
+        with open("{}/{}.node/node.json".format(self.tmp_dir, le.name)) as json_data:
+            node = json.load(json_data)
+
+        self.assertEqual(le.name, node['name'])
+        self.assertEqual(le.input_features[0], node['shape']['inputs'][0]['name'])
+        self.assertEqual(le.output_features, node['shape']['outputs'][0]['name'])
 
     def label_encoder_deserializer_test(self):
 
         labels = ['a', 'b', 'c']
 
         le = LabelEncoder(input_features=['label_feature'],
-                          output_features=['label_feature_le_encoded'])
+                          output_features='label_feature_le_encoded')
 
         le.fit(labels)
 
         self.assertEqual(labels, le.classes_.tolist())
 
         le.serialize_to_bundle(self.tmp_dir, le.name)
 
@@ -408,60 +368,56 @@
         res_b = label_encoder_tf.transform(labels)
         print("le.output_features: {}".format(le.output_features))
         print("label_encoder_tf.output_features: {}".format(label_encoder_tf.output_features))
         self.assertEqual(res_a[0], res_b[0])
         self.assertEqual(res_a[1], res_b[1])
         self.assertEqual(res_a[2], res_b[2])
         self.assertEqual(le.input_features, label_encoder_tf.input_features)
-        self.assertEqual(le.output_features, label_encoder_tf.output_features)
+        self.assertEqual(le.output_features, label_encoder_tf.output_features[0])
 
     def one_hot_encoder_serializer_test(self):
 
         labels = ['a', 'b', 'c']
 
         le = LabelEncoder(input_features=['label_feature'],
-                          output_features=['label_feature_le_encoded'])
+                          output_features='label_feature_le_encoded')
 
         oh_data = le.fit_transform(labels).reshape(3, 1)
 
         one_hot_encoder_tf = OneHotEncoder(sparse=False)
-        one_hot_encoder_tf.mlinit(input_features = le.output_features,
-                                  output_features = '{}_one_hot_encoded'.format(le.output_features))
+        one_hot_encoder_tf.mlinit(prior_tf=le,
+                                  output_features='{}_one_hot_encoded'.format(le.output_features))
         one_hot_encoder_tf.fit(oh_data)
 
         one_hot_encoder_tf.serialize_to_bundle(self.tmp_dir, one_hot_encoder_tf.name)
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, one_hot_encoder_tf.name)) as json_data:
             model = json.load(json_data)
 
         self.assertEqual(one_hot_encoder_tf.op, model['op'])
-        self.assertEqual(3, model['attributes']['size']['value'])
-        self.assertEqual(True, model['attributes']['drop_last']['value'])
+        self.assertEqual(3, model['attributes']['size']['long'])
+        self.assertEqual(True, model['attributes']['drop_last']['boolean'])
 
     def one_hot_encoder_deserializer_test(self):
 
         labels = ['a', 'b', 'c']
 
         le = LabelEncoder(input_features=['label_feature'],
-                          output_features=['label_feature_le_encoded'])
+                          output_features='label_feature_le_encoded')
 
         oh_data = le.fit_transform(labels).reshape(3, 1)
 
         one_hot_encoder_tf = OneHotEncoder(sparse=False)
-        one_hot_encoder_tf.mlinit(input_features = le.output_features,
-                                  output_features=['{}_one_hot_encoded'.format(le.output_features[0])])
+        one_hot_encoder_tf.mlinit(prior_tf = le,
+                                  output_features='{}_one_hot_encoded'.format(le.output_features))
         one_hot_encoder_tf.fit(oh_data)
 
         one_hot_encoder_tf.serialize_to_bundle(self.tmp_dir, one_hot_encoder_tf.name)
 
-        # Test model.json
-        with open("{}/{}.node/model.json".format(self.tmp_dir, one_hot_encoder_tf.name)) as json_data:
-            model = json.load(json_data)
-
         # Deserialize the OneHotEncoder
         node_name = "{}.node".format(one_hot_encoder_tf.name)
         one_hot_encoder_tf_ds = OneHotEncoder()
         one_hot_encoder_tf_ds.deserialize_from_bundle(self.tmp_dir, node_name)
 
         # Transform some sample data
         res_a = one_hot_encoder_tf.transform(oh_data)
@@ -472,22 +428,22 @@
         self.assertEqual(res_a[2][0], res_b[2][0])
 
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, one_hot_encoder_tf.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(one_hot_encoder_tf_ds.name, node['name'])
-        self.assertEqual(one_hot_encoder_tf_ds.input_features, node['shape']['inputs'][0]['name'])
-        self.assertEqual(one_hot_encoder_tf_ds.output_features, node['shape']['outputs'][0]['name'])
+        self.assertEqual(one_hot_encoder_tf_ds.input_features[0], node['shape']['inputs'][0]['name'])
+        self.assertEqual(one_hot_encoder_tf_ds.output_features[0], node['shape']['outputs'][0]['name'])
 
     def feature_extractor_test(self):
 
         extract_features = ['a', 'd']
 
-        feature_extractor = FeatureExtractor(input_features=extract_features,
+        feature_extractor = FeatureExtractor(input_scalars=extract_features,
                                              output_vector='extract_features_output',
                                              output_vector_items=["{}_out".format(x) for x in extract_features])
 
         res = feature_extractor.fit_transform(self.df)
 
         self.assertEqual(len(res.columns), 2)
 
@@ -498,24 +454,61 @@
             node = json.load(json_data)
 
         self.assertEqual(feature_extractor.name, node['name'])
         self.assertEqual(feature_extractor.input_features[0], node['shape']['inputs'][0]['name'])
         self.assertEqual(feature_extractor.input_features[1], node['shape']['inputs'][1]['name'])
         self.assertEqual(feature_extractor.output_vector, node['shape']['outputs'][0]['name'])
 
+        # Test model.json
+        with open("{}/{}.node/model.json".format(self.tmp_dir, feature_extractor.name)) as json_data:
+            model = json.load(json_data)
+
+        expected_model = {
+            "op": "vector_assembler",
+            "attributes": {
+                "input_shapes": {
+                    "data_shape": [
+                        {
+                        "base": "scalar",
+                        "isNullable": False
+                        },
+                        {
+                        "base": "scalar",
+                        "isNullable": False
+                        }],
+                    "type": "list"
+                }
+            }
+        }
+
+        self.assertEqual(expected_model['op'], model['op'])
+        self.assertEqual(expected_model['attributes']['input_shapes']['data_shape'][0]['base'],
+                         model['attributes']['input_shapes']['data_shape'][0]['base'])
+        self.assertEqual(expected_model['attributes']['input_shapes']['data_shape'][0]['isNullable'],
+                         model['attributes']['input_shapes']['data_shape'][0]['isNullable'])
+        self.assertEqual(expected_model['attributes']['input_shapes']['data_shape'][1]['base'],
+                         model['attributes']['input_shapes']['data_shape'][1]['base'])
+        self.assertEqual(expected_model['attributes']['input_shapes']['data_shape'][1]['isNullable'],
+                     model['attributes']['input_shapes']['data_shape'][1]['isNullable'])
+
     def imputer_test(self):
 
         def _set_nulls(df):
             row = df['index']
             if row in [2,5]:
                 return np.NaN
             return df.a
 
+        extract_features = ['a']
+        feature_extractor = FeatureExtractor(input_scalars=['a'],
+                                         output_vector='extracted_a_output',
+                                         output_vector_items=["{}_out".format(x) for x in extract_features])
+
         imputer = Imputer(strategy='mean')
-        imputer.mlinit(input_features='a',
+        imputer.mlinit(prior_tf=feature_extractor,
                        output_features='a_imputed')
 
         df2 = self.df
         df2.reset_index(inplace=True)
         df2['a'] = df2.apply(_set_nulls, axis=1)
 
         imputer.fit(df2[['a']])
@@ -524,74 +517,89 @@
 
         imputer.serialize_to_bundle(self.tmp_dir, imputer.name)
 
         expected_model = {
           "op": "imputer",
           "attributes": {
             "surrogate_value": {
-              "type": "double",
-              "value": df2.a.mean()
+              "double": df2.a.mean()
             },
             "strategy": {
-              "type": "string",
-              "value": "mean"
+              "string": "mean"
             }
           }
         }
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, imputer.name)) as json_data:
             model = json.load(json_data)
 
-        self.assertEqual(expected_model['attributes']['strategy']['value'], model['attributes']['strategy']['value'])
-        self.assertAlmostEqual(expected_model['attributes']['surrogate_value']['value'], model['attributes']['surrogate_value']['value'], places = 7)
+        self.assertEqual(expected_model['attributes']['strategy']['string'], model['attributes']['strategy']['string'])
+        self.assertAlmostEqual(expected_model['attributes']['surrogate_value']['double'], model['attributes']['surrogate_value']['double'], places = 7)
 
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, imputer.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(imputer.name, node['name'])
         self.assertEqual(imputer.input_features, node['shape']['inputs'][0]['name'])
         self.assertEqual(imputer.output_features, node['shape']['outputs'][0]['name'])
 
     def binarizer_test(self):
 
+        extract_features = ['a']
+        feature_extractor = FeatureExtractor(input_scalars=['a'],
+                                         output_vector='extracted_a_output',
+                                         output_vector_items=["{}_out".format(x) for x in extract_features])
+
         binarizer = Binarizer(threshold=0.0)
-        binarizer.mlinit(input_features='a',
+        binarizer.mlinit(prior_tf=feature_extractor,
                          output_features='a_binary')
 
         Xres = binarizer.fit_transform(self.df[['a']])
 
         # Test that the binarizer functions as expected
         self.assertEqual(float(len(self.df[self.df.a >= 0]))/10.0, Xres.mean())
 
         binarizer.serialize_to_bundle(self.tmp_dir, binarizer.name)
 
         expected_model = {
           "op": "binarizer",
           "attributes": {
             "threshold": {
-              "type": "double",
-              "value": 0.0
+              "double": 0.0
             }
           }
         }
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, binarizer.name)) as json_data:
             model = json.load(json_data)
 
-        self.assertEqual(expected_model['attributes']['threshold']['value'],
-                         model['attributes']['threshold']['value'])
+        self.assertEqual(expected_model['attributes']['threshold']['double'],
+                         model['attributes']['threshold']['double'])
+
+        # Test node.json
+        with open("{}/{}.node/node.json".format(self.tmp_dir, binarizer.name)) as json_data:
+            node = json.load(json_data)
+
+        self.assertEqual(binarizer.name, node['name'])
+        self.assertEqual(binarizer.input_features, node['shape']['inputs'][0]['name'])
+        self.assertEqual(binarizer.output_features, node['shape']['outputs'][0]['name'])
 
     def binarizer_deserializer_test(self):
 
+        extract_features = ['a']
+        feature_extractor = FeatureExtractor(input_scalars=['a'],
+                                         output_vector='extracted_a_output',
+                                         output_vector_items=["{}_out".format(x) for x in extract_features])
+
         binarizer = Binarizer(threshold=0.0)
-        binarizer.mlinit(input_features=['a'],
-                         output_features=['a_binary'])
+        binarizer.mlinit(prior_tf=feature_extractor,
+                         output_features='a_binary')
 
         Xres = binarizer.fit_transform(self.df[['a']])
 
         # Test that the binarizer functions as expected
         self.assertEqual(float(len(self.df[self.df.a >= 0]))/10.0, Xres.mean())
 
         binarizer.serialize_to_bundle(self.tmp_dir, binarizer.name)
@@ -606,79 +614,50 @@
         res_b = binarizer_tf_ds.transform(self.df[['a']])
 
         self.assertEqual(res_a[0][0], res_b[0][0])
         self.assertEqual(res_a[1][0], res_b[1][0])
         self.assertEqual(res_a[2][0], res_b[2][0])
         self.assertEqual(res_a[3][0], res_b[3][0])
 
-         # Test node.json
-        with open("{}/{}.node/node.json".format(self.tmp_dir, binarizer.name)) as json_data:
-            node = json.load(json_data)
-
-        self.assertEqual(binarizer.name, node['name'])
-        self.assertEqual(binarizer.input_features, node['shape']['inputs'][0]['name'])
-        self.assertEqual(binarizer.output_features, node['shape']['outputs'][0]['name'])
-
     def polynomial_expansion_test(self):
 
+        extract_features = ['a']
+        feature_extractor = FeatureExtractor(input_scalars=['a'],
+                                         output_vector='extracted_a_output',
+                                         output_vector_items=["{}_out".format(x) for x in extract_features])
+
         polynomial_exp = PolynomialFeatures(degree=2, include_bias=False)
-        polynomial_exp.mlinit(input_features='a',
+        polynomial_exp.mlinit(prior_tf=feature_extractor,
                               output_features='poly')
 
         Xres = polynomial_exp.fit_transform(self.df[['a']])
 
         self.assertEqual(Xres[0][1], Xres[0][0] * Xres[0][0])
 
         polynomial_exp.serialize_to_bundle(self.tmp_dir, polynomial_exp.name)
 
         expected_model = {
           "op": "polynomial_expansion",
           "attributes": {
             "degree": {
-              "type": "double",
-              "value": 2
+              "long": 2
+            },
+            "input_size": {
+                  "long": 1
             }
           }
         }
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, polynomial_exp.name)) as json_data:
             model = json.load(json_data)
 
-        self.assertEqual(expected_model['attributes']['degree']['value'], model['attributes']['degree']['value'])
-
-    def polynomial_expansion_deserializer_test(self):
-
-        polynomial_exp = PolynomialFeatures(degree=2, include_bias=False)
-        polynomial_exp.mlinit(input_features=['a', 'b'],
-                              output_features=['a', 'b', 'a_sqd', 'a_mult_b', 'b_sqd'])
-
-        Xres = polynomial_exp.fit_transform(self.df[['a', 'b']])
-
-        self.assertEqual(Xres[0][2], Xres[0][0] * Xres[0][0])
-
-        polynomial_exp.serialize_to_bundle(self.tmp_dir, polynomial_exp.name)
-
-        # Deserialize the PolynomialExpansion
-        node_name = "{}.node".format(polynomial_exp.name)
-        poly_tf_ds = PolynomialFeatures()
-        poly_tf_ds.deserialize_from_bundle(self.tmp_dir, node_name)
-
-        # Transform some sample data
-        res_a = polynomial_exp.transform(self.df[['a', 'b']])
-        res_b = poly_tf_ds.transform(self.df[['a', 'b']])
+        self.assertEqual(expected_model['attributes']['degree']['long'], model['attributes']['degree']['long'])
+        self.assertEqual(expected_model['attributes']['input_size']['long'], model['attributes']['input_size']['long'])
 
-        self.assertEqual(res_a[0][0], res_b[0][0])
-        self.assertEqual(res_a[1][0], res_b[1][0])
-        self.assertEqual(res_a[2][0], res_b[2][0])
-        self.assertEqual(res_a[3][0], res_b[3][0])
-        self.assertEqual(res_a[0][1], res_b[0][1])
-        self.assertEqual(res_a[1][1], res_b[1][1])
-        self.assertEqual(res_a[2][1], res_b[2][1])
-        self.assertEqual(res_a[3][1], res_b[3][1])
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, polynomial_exp.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(polynomial_exp.name, node['name'])
         self.assertEqual(polynomial_exp.input_features, node['shape']['inputs'][0]['name'])
         self.assertEqual(polynomial_exp.output_features, node['shape']['outputs'][0]['name'])
@@ -693,25 +672,24 @@
 
         math_unary_tf.serialize_to_bundle(self.tmp_dir, math_unary_tf.name)
 
         expected_model = {
           "op": "math_unary",
           "attributes": {
             "operation": {
-              "type": "string",
-              "value": 'exp'
+              "string": 'exp'
             }
           }
         }
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, math_unary_tf.name)) as json_data:
             model = json.load(json_data)
 
-        self.assertEqual(expected_model['attributes']['operation']['value'], model['attributes']['operation']['value'])
+        self.assertEqual(expected_model['attributes']['operation']['string'], model['attributes']['operation']['string'])
 
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, math_unary_tf.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(math_unary_tf.name, node['name'])
         self.assertEqual(math_unary_tf.input_features[0], node['shape']['inputs'][0]['name'])
@@ -749,25 +727,24 @@
 
         math_unary_tf.serialize_to_bundle(self.tmp_dir, math_unary_tf.name)
 
         expected_model = {
           "op": "math_unary",
           "attributes": {
             "operation": {
-              "type": "string",
-              "value": 'sin'
+              "string": 'sin'
             }
           }
         }
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, math_unary_tf.name)) as json_data:
             model = json.load(json_data)
 
-        self.assertEqual(expected_model['attributes']['operation']['value'], model['attributes']['operation']['value'])
+        self.assertEqual(expected_model['attributes']['operation']['string'], model['attributes']['operation']['string'])
 
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, math_unary_tf.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(math_unary_tf.name, node['name'])
         self.assertEqual(math_unary_tf.input_features[0], node['shape']['inputs'][0]['name'])
@@ -783,25 +760,24 @@
 
         math_binary_tf.serialize_to_bundle(self.tmp_dir, math_binary_tf.name)
 
         expected_model = {
           "op": "math_binary",
           "attributes": {
             "operation": {
-              "type": "string",
-              "value": 'add'
+              "string": 'add'
             }
           }
         }
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, math_binary_tf.name)) as json_data:
             model = json.load(json_data)
 
-        self.assertEqual(expected_model['attributes']['operation']['value'], model['attributes']['operation']['value'])
+        self.assertEqual(expected_model['attributes']['operation']['string'], model['attributes']['operation']['string'])
 
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, math_binary_tf.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(math_binary_tf.name, node['name'])
         self.assertEqual(math_binary_tf.input_features[0], node['shape']['inputs'][0]['name'])
@@ -837,25 +813,24 @@
 
         math_binary_tf.serialize_to_bundle(self.tmp_dir, math_binary_tf.name)
 
         expected_model = {
           "op": "math_binary",
           "attributes": {
             "operation": {
-              "type": "string",
-              "value": 'sub'
+              "string": 'sub'
             }
           }
         }
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, math_binary_tf.name)) as json_data:
             model = json.load(json_data)
 
-        self.assertEqual(expected_model['attributes']['operation']['value'], model['attributes']['operation']['value'])
+        self.assertEqual(expected_model['attributes']['operation']['string'], model['attributes']['operation']['string'])
 
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, math_binary_tf.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(math_binary_tf.name, node['name'])
         self.assertEqual(math_binary_tf.input_features[0], node['shape']['inputs'][0]['name'])
@@ -872,25 +847,24 @@
 
         math_binary_tf.serialize_to_bundle(self.tmp_dir, math_binary_tf.name)
 
         expected_model = {
           "op": "math_binary",
           "attributes": {
             "operation": {
-              "type": "string",
-              "value": 'mul'
+              "string": 'mul'
             }
           }
         }
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, math_binary_tf.name)) as json_data:
             model = json.load(json_data)
 
-        self.assertEqual(expected_model['attributes']['operation']['value'], model['attributes']['operation']['value'])
+        self.assertEqual(expected_model['attributes']['operation']['string'], model['attributes']['operation']['string'])
 
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, math_binary_tf.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(math_binary_tf.name, node['name'])
         self.assertEqual(math_binary_tf.input_features[0], node['shape']['inputs'][0]['name'])
@@ -907,27 +881,93 @@
 
         math_binary_tf.serialize_to_bundle(self.tmp_dir, math_binary_tf.name)
 
         expected_model = {
           "op": "math_binary",
           "attributes": {
             "operation": {
-              "type": "string",
-              "value": 'div'
+              "string": 'div'
             }
           }
         }
 
         # Test model.json
         with open("{}/{}.node/model.json".format(self.tmp_dir, math_binary_tf.name)) as json_data:
             model = json.load(json_data)
 
-        self.assertEqual(expected_model['attributes']['operation']['value'], model['attributes']['operation']['value'])
+        self.assertEqual(expected_model['attributes']['operation']['string'], model['attributes']['operation']['string'])
 
         # Test node.json
         with open("{}/{}.node/node.json".format(self.tmp_dir, math_binary_tf.name)) as json_data:
             node = json.load(json_data)
 
         self.assertEqual(math_binary_tf.name, node['name'])
         self.assertEqual(math_binary_tf.input_features[0], node['shape']['inputs'][0]['name'])
         self.assertEqual(math_binary_tf.input_features[1], node['shape']['inputs'][1]['name'])
         self.assertEqual(math_binary_tf.output_features[0], node['shape']['outputs'][0]['name'])
+
+    def string_map_test(self):
+
+        df = pd.DataFrame(['test_one', 'test_two', 'test_one', 'test_one', 'test_two'], columns=['a'])
+        string_map_tf = StringMap(input_features=['a'], output_features=['a_mapped'], labels={"test_one":1.0, "test_two": 0.0})
+
+        Xres = string_map_tf.fit_transform(df)
+        self.assertEqual(1.0, Xres[0])
+        self.assertEqual(0.0, Xres[1])
+        self.assertEqual(1.0, Xres[2])
+        self.assertEqual(1.0, Xres[3])
+        self.assertEqual(0.0, Xres[4])
+
+        string_map_tf.serialize_to_bundle(self.tmp_dir, string_map_tf.name)
+
+        expected_model = {
+            "op": "string_map",
+            "attributes": {
+                "labels": {
+                    "type": "list",
+                    "string": ["test_one", "test_two"]
+                },
+                "values": {
+                    "type": "list",
+                    "double": [1.0, 0.0]
+                }
+            }
+        }
+        #
+        # Test model.json
+        with open("{}/{}.node/model.json".format(self.tmp_dir, string_map_tf.name)) as json_data:
+            model = json.load(json_data)
+
+        self.assertEqual(expected_model['attributes']['labels']['string'], model['attributes']['labels']['string'])
+        self.assertEqual(expected_model['attributes']['values']['double'], model['attributes']['values']['double'])
+
+        # Test node.json
+        with open("{}/{}.node/node.json".format(self.tmp_dir, string_map_tf.name)) as json_data:
+            node = json.load(json_data)
+
+        self.assertEqual(string_map_tf.name, node['name'])
+        self.assertEqual(string_map_tf.input_features[0], node['shape']['inputs'][0]['name'])
+        self.assertEqual(string_map_tf.output_features[0], node['shape']['outputs'][0]['name'])
+
+    def string_map_deserializer_test(self):
+
+        df = pd.DataFrame(['test_one', 'test_two', 'test_one', 'test_one', 'test_two'], columns=['a'])
+        string_map = StringMap(input_features=['a'], output_features=['a_mapped'], labels={"test_one":1.0, "test_two": 0.0})
+        string_map.serialize_to_bundle(self.tmp_dir, string_map.name)
+
+        # Now deserialize it back
+        node_name = "{}.node".format(string_map.name)
+        string_map_tf = StringMap()
+        string_map_tf = string_map_tf.deserialize_from_bundle(self.tmp_dir, node_name)
+
+        # Transform some sample data
+        res_a = string_map.fit_transform(df)
+        res_b = string_map_tf.fit_transform(df)
+
+        self.assertEqual(res_a[0], res_b[0])
+        self.assertEqual(res_a[1], res_b[1])
+        self.assertEqual(res_a[2], res_b[2])
+        self.assertEqual(res_a[3], res_b[3])
+        self.assertEqual(res_a[4], res_b[4])
+        self.assertEqual(string_map.name, string_map_tf.name)
+        self.assertEqual(string_map.op, string_map_tf.op)
+        self.assertEqual(string_map.labels, string_map_tf.labels)
```

### Comparing `mleap-0.7.0/mleap/sklearn/svm.py` & `mleap-0.8.1/mleap/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/sklearn/tree/tree.py` & `mleap-0.8.1/mleap/sklearn/tree/tree.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/tensorflow/test.py` & `mleap-0.8.1/mleap/tensorflow/test.py`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/mleap/version.py` & `mleap-0.8.1/mleap/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.7.0"
+__version__ = "0.8.1"
```

### Comparing `mleap-0.7.0/mleap.egg-info/PKG-INFO` & `mleap-0.8.1/mleap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mleap
-Version: 0.7.0
+Version: 0.8.1
 Summary: MLeap Python API
 Home-page: https://github.com/combust/mleap/tree/feature/scikit-v2/python
 Author: MLeap Developers
 Author-email: combust@combust.ml
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `mleap-0.7.0/mleap.egg-info/SOURCES.txt` & `mleap-0.8.1/mleap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mleap-0.7.0/PKG-INFO` & `mleap-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mleap
-Version: 0.7.0
+Version: 0.8.1
 Summary: MLeap Python API
 Home-page: https://github.com/combust/mleap/tree/feature/scikit-v2/python
 Author: MLeap Developers
 Author-email: combust@combust.ml
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `mleap-0.7.0/setup.py` & `mleap-0.8.1/setup.py`

 * *Files identical despite different names*

