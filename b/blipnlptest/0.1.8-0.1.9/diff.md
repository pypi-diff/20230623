# Comparing `tmp/blipnlptest-0.1.8.tar.gz` & `tmp/blipnlptest-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blipnlptest-0.1.8.tar", max compression
+gzip compressed data, was "blipnlptest-0.1.9.tar", max compression
```

## Comparing `blipnlptest-0.1.8.tar` & `blipnlptest-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2023-06-23 16:36:38.908554 blipnlptest-0.1.8/blipnlptest/__init__.py
--rw-r--r--   0        0        0     6386 2023-06-23 16:46:15.984456 blipnlptest-0.1.8/blipnlptest/blipnlptest.py
--rw-r--r--   0        0        0     1088 2023-06-23 16:36:39.125375 blipnlptest-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0      624 2023-06-23 16:50:05.821770 blipnlptest-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3170 2023-06-23 16:45:52.911940 blipnlptest-0.1.8/README.md
--rw-r--r--   0        0        0     3954 1970-01-01 00:00:00.000000 blipnlptest-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-06-23 16:36:38.908554 blipnlptest-0.1.9/blipnlptest/__init__.py
+-rw-r--r--   0        0        0     6387 2023-06-23 17:00:03.784134 blipnlptest-0.1.9/blipnlptest/blipnlptest.py
+-rw-r--r--   0        0        0     1088 2023-06-23 16:36:39.125375 blipnlptest-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0      624 2023-06-23 17:03:18.128299 blipnlptest-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3170 2023-06-23 16:45:52.911940 blipnlptest-0.1.9/README.md
+-rw-r--r--   0        0        0     3954 1970-01-01 00:00:00.000000 blipnlptest-0.1.9/PKG-INFO
```

### Comparing `blipnlptest-0.1.8/blipnlptest/blipnlptest.py` & `blipnlptest-0.1.9/blipnlptest/blipnlptest.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
       for i in range(len(df)):
         if df.Entities[i] != '[]':
           ent.append(pd.json_normalize(json.loads(df.Entities[i])).value.tolist())
         else:
           ent.append('')
       
-      df.loc[:, 'Content'] = [selftest(model='n', intention=df.Intention[x], entities=ent[x]) for x in range(len(df.Entities))]
+      df.loc[:, 'Content'] = [self.test(model='n', intention=df.Intention[x], entities=ent[x]) for x in range(len(df.Entities))]
       
       df = df.sort_values(by='Content',ascending=False)
       df = self.check_threshold(df)
       return(df)
     
     except KeyError: 
       print("O seu dataframe deve conter as seguintes colunas ['Text', 'Intention', 'Entities', 'Score']. Você pode obtê-las pela tabela vwidentityanalysis.")
```

### Comparing `blipnlptest-0.1.8/LICENSE.txt` & `blipnlptest-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.1.8/pyproject.toml` & `blipnlptest-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blipnlptest"
-version = "0.1.8"
+version = "0.1.9"
 authors = ["Caio Souza <caios@blip.ai>"]
 
 description = "Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo."
 readme = "README.md"
 
 
 classifiers = [
```

### Comparing `blipnlptest-0.1.8/README.md` & `blipnlptest-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.1.8/PKG-INFO` & `blipnlptest-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blipnlptest
-Version: 0.1.8
+Version: 0.1.9
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@blip.ai
 Requires-Python: >=3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

