# Comparing `tmp/LumosWeb-1.0.3.tar.gz` & `tmp/LumosWeb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-1.0.3.tar", last modified: Wed Jun  7 07:39:56 2023, max compression
+gzip compressed data, was "LumosWeb-1.1.0.tar", last modified: Fri Jun 23 09:18:11 2023, max compression
```

## Comparing `LumosWeb-1.0.3.tar` & `LumosWeb-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 07:39:56.274551 LumosWeb-1.0.3/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 07:39:55.951808 LumosWeb-1.0.3/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.0.3/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5438 2023-06-03 13:53:15.000000 LumosWeb-1.0.3/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-05-31 20:54:27.000000 LumosWeb-1.0.3/LumosWeb/cli.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.0.3/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6349 2023-06-07 07:36:56.000000 LumosWeb-1.0.3/LumosWeb/orm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.0.3/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 07:39:56.221969 LumosWeb-1.0.3/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4417 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-06-07 07:39:55.000000 LumosWeb-1.0.3/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4417 2023-06-07 07:39:56.268591 LumosWeb-1.0.3/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4249 2023-06-03 20:19:34.000000 LumosWeb-1.0.3/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-07 07:39:56.278043 LumosWeb-1.0.3/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-06-07 07:39:22.000000 LumosWeb-1.0.3/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 09:18:11.147117 LumosWeb-1.1.0/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 09:18:10.807735 LumosWeb-1.1.0/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.1.0/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5438 2023-06-03 13:53:15.000000 LumosWeb-1.1.0/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-05-31 20:54:27.000000 LumosWeb-1.1.0/LumosWeb/cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.1.0/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6349 2023-06-07 07:36:56.000000 LumosWeb-1.1.0/LumosWeb/orm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.1.0/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 09:18:11.082922 LumosWeb-1.1.0/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6269 2023-06-23 09:18:09.000000 LumosWeb-1.1.0/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-23 09:18:10.000000 LumosWeb-1.1.0/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-23 09:18:09.000000 LumosWeb-1.1.0/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-06-23 09:18:09.000000 LumosWeb-1.1.0/LumosWeb.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-06-23 09:18:09.000000 LumosWeb-1.1.0/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-06-23 09:18:10.000000 LumosWeb-1.1.0/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6269 2023-06-23 09:18:11.139455 LumosWeb-1.1.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6174 2023-06-23 09:17:18.000000 LumosWeb-1.1.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-23 09:18:11.150378 LumosWeb-1.1.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-06-22 16:12:27.000000 LumosWeb-1.1.0/setup.py
```

### Comparing `LumosWeb-1.0.3/LumosWeb/api.py` & `LumosWeb-1.1.0/LumosWeb/api.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.3/LumosWeb/cli.py` & `LumosWeb-1.1.0/LumosWeb/cli.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.3/LumosWeb/middleware.py` & `LumosWeb-1.1.0/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.3/LumosWeb/orm.py` & `LumosWeb-1.1.0/LumosWeb/orm.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.3/LumosWeb/response.py` & `LumosWeb-1.1.0/LumosWeb/response.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.3/README.md` & `LumosWeb-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -43,16 +43,17 @@
     resp.text = "We don't have to use decorators!"
 
 app.add_route("/sample", handler, allowed_methods=["get", "post"])
 
 
 ```
 ### Run Server 
-Go to the directory on Terminal where your api instance is located
+Navigate to the directory in the Terminal where the file of your API instance is located
 > Lumosweb --app <module_name> run
+
 And lights are on!
 
 ### Unit Test
 
 The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
 that you may want to use when writing unit tests with LumosWeb. The first one is `app` which is an instance of the main `API` class:
 ```python
@@ -132,8 +133,78 @@
         print("Before dispatch", req.url)
 
     def process_response(self, req, res):
         print("After dispatch", req.url)
 
 
 app.add_middleware(SimpleCustomMiddleware)
-```
+```
+
+ ### Database
+ You can create custom middleware classes by inheriting from the `LumosWeb.orm.Database` class
+ First create models file and create a class for each table in the database
+ models.py
+ ```python
+from LumosWeb.orm import Table, Column
+class Book(Table):
+    author = Column(str)
+    name = Column(str)
+ ```
+Then create a storage file and import the models
+storage.py
+```python
+from models import Book
+
+class BookStorage:
+    _id = 0
+
+    def __init__(self):
+        self._books = []
+
+    def all(self):
+        return [book._asdict() for book in self._books]
+
+    def get(self, id: int):
+        for book in self._books:
+            if book.id == id:
+                return book
+
+        return None
+
+    def create(self, **kwargs):
+        self._id += 1
+        kwargs["id"] = self._id
+        book = Book(**kwargs)
+        self._books.append(book)
+        return book
+
+    def delete(self, id):
+        for ind, book in enumerate(self._books):
+            if book.id == id:
+                del self._books[ind]
+```
+Then use them
+app.py
+ ```python
+from LumosWeb.orm import Database
+db = Database("./lumos.db")  # lumos.db is the name of the database file
+db.create(Book)
+
+@app.route("/", allowed_methods=["get"])
+def index(req, resp):
+    books = db.all(Book)
+    resp.html = app.template("index.html", context={"books": books})
+
+@app.route("/books", allowed_methods=["post"])
+def create_book(req, resp):
+    book = Book(**req.POST)  # Creates a Book instance with the given data in the request.
+    db.save(book)
+
+    resp.status_code = 201  # Created
+    resp.json = {"name": book.name, "author": book.author}
+
+@app.route("/books/{id:d}", allowed_methods=["delete"])
+def delete_book(req, resp, id):
+    db.delete(Book, id=id)
+    resp.status_code = 204  # No content (resource has successfully been deleted.)
+
+```
```

### Comparing `LumosWeb-1.0.3/setup.py` & `LumosWeb-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.0.3"
+VERSION = "1.1.0"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

