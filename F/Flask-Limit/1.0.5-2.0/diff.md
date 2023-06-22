# Comparing `tmp/Flask_Limit-1.0.5.tar.gz` & `tmp/Flask_Limit-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask_Limit-1.0.5.tar", last modified: Sun Jun 11 00:30:09 2023, max compression
+gzip compressed data, was "Flask_Limit-2.0.tar", last modified: Thu Jun 22 23:03:47 2023, max compression
```

## Comparing `Flask_Limit-1.0.5.tar` & `Flask_Limit-2.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-11 00:30:09.899022 Flask_Limit-1.0.5/
--rw-r--r--   0 tabot      (501) staff       (20)       35 2022-12-30 01:49:43.000000 Flask_Limit-1.0.5/AUTHORS
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-11 00:30:09.898089 Flask_Limit-1.0.5/Flask_Limit.egg-info/
--rw-r--r--   0 tabot      (501) staff       (20)     3376 2023-06-11 00:30:09.000000 Flask_Limit-1.0.5/Flask_Limit.egg-info/PKG-INFO
--rw-r--r--   0 tabot      (501) staff       (20)      362 2023-06-11 00:30:09.000000 Flask_Limit-1.0.5/Flask_Limit.egg-info/SOURCES.txt
--rw-r--r--   0 tabot      (501) staff       (20)        1 2023-06-11 00:30:09.000000 Flask_Limit-1.0.5/Flask_Limit.egg-info/dependency_links.txt
--rw-r--r--   0 tabot      (501) staff       (20)        1 2022-12-30 01:51:34.000000 Flask_Limit-1.0.5/Flask_Limit.egg-info/not-zip-safe
--rw-r--r--   0 tabot      (501) staff       (20)        6 2023-06-11 00:30:09.000000 Flask_Limit-1.0.5/Flask_Limit.egg-info/requires.txt
--rw-r--r--   0 tabot      (501) staff       (20)       12 2023-06-11 00:30:09.000000 Flask_Limit-1.0.5/Flask_Limit.egg-info/top_level.txt
--rw-r--r--   0 tabot      (501) staff       (20)     1068 2022-12-30 01:49:43.000000 Flask_Limit-1.0.5/LICENSE
--rw-r--r--   0 tabot      (501) staff       (20)       80 2022-12-30 01:49:43.000000 Flask_Limit-1.0.5/MANIFEST.in
--rw-r--r--   0 tabot      (501) staff       (20)     3376 2023-06-11 00:30:09.898893 Flask_Limit-1.0.5/PKG-INFO
--rw-r--r--   0 tabot      (501) staff       (20)     2573 2022-12-30 01:49:43.000000 Flask_Limit-1.0.5/README.md
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-11 00:30:09.898229 Flask_Limit-1.0.5/docs/
--rw-r--r--   0 tabot      (501) staff       (20)     3017 2022-12-30 01:49:43.000000 Flask_Limit-1.0.5/docs/index.rst
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-11 00:30:09.898492 Flask_Limit-1.0.5/flask_limit/
--rw-r--r--   0 tabot      (501) staff       (20)       59 2023-06-11 00:29:03.000000 Flask_Limit-1.0.5/flask_limit/__init__.py
--rwxr-xr-x   0 tabot      (501) staff       (20)     3975 2023-06-11 00:28:49.000000 Flask_Limit-1.0.5/flask_limit/rate_limit.py
--rw-r--r--   0 tabot      (501) staff       (20)       38 2023-06-11 00:30:09.899058 Flask_Limit-1.0.5/setup.cfg
--rwxr-xr-x   0 tabot      (501) staff       (20)     1383 2022-12-30 01:49:43.000000 Flask_Limit-1.0.5/setup.py
-drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-11 00:30:09.898725 Flask_Limit-1.0.5/tests/
--rw-r--r--   0 tabot      (501) staff       (20)        0 2022-12-30 01:49:43.000000 Flask_Limit-1.0.5/tests/__init__.py
--rw-r--r--   0 tabot      (501) staff       (20)     1906 2022-12-30 01:49:43.000000 Flask_Limit-1.0.5/tests/test_rate_limit.py
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:03:47.287762 Flask_Limit-2.0/
+-rw-r--r--   0 tabot      (501) staff       (20)       35 2023-06-11 23:35:14.000000 Flask_Limit-2.0/AUTHORS
+-rw-r--r--   0 tabot      (501) staff       (20)     1068 2023-06-11 23:35:14.000000 Flask_Limit-2.0/LICENSE
+-rw-r--r--   0 tabot      (501) staff       (20)       80 2023-06-11 23:35:14.000000 Flask_Limit-2.0/MANIFEST.in
+-rw-r--r--   0 tabot      (501) staff       (20)     4102 2023-06-22 23:03:47.287821 Flask_Limit-2.0/PKG-INFO
+-rw-r--r--   0 tabot      (501) staff       (20)     3443 2023-06-22 22:06:20.000000 Flask_Limit-2.0/README.md
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:03:47.284607 Flask_Limit-2.0/docs/
+-rw-r--r--   0 tabot      (501) staff       (20)     4145 2023-06-22 22:06:17.000000 Flask_Limit-2.0/docs/index.rst
+-rw-r--r--   0 tabot      (501) staff       (20)   850764 2023-06-22 21:19:36.000000 Flask_Limit-2.0/docs/proof.png
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:03:47.283152 Flask_Limit-2.0/flask_limit/
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:03:47.286754 Flask_Limit-2.0/flask_limit/Flask_Limit.egg-info/
+-rw-r--r--   0 tabot      (501) staff       (20)     4102 2023-06-22 23:03:47.000000 Flask_Limit-2.0/flask_limit/Flask_Limit.egg-info/PKG-INFO
+-rw-r--r--   0 tabot      (501) staff       (20)      525 2023-06-22 23:03:47.000000 Flask_Limit-2.0/flask_limit/Flask_Limit.egg-info/SOURCES.txt
+-rw-r--r--   0 tabot      (501) staff       (20)        1 2023-06-22 23:03:47.000000 Flask_Limit-2.0/flask_limit/Flask_Limit.egg-info/dependency_links.txt
+-rw-r--r--   0 tabot      (501) staff       (20)        1 2023-06-19 02:52:57.000000 Flask_Limit-2.0/flask_limit/Flask_Limit.egg-info/not-zip-safe
+-rw-r--r--   0 tabot      (501) staff       (20)       32 2023-06-22 23:03:47.000000 Flask_Limit-2.0/flask_limit/Flask_Limit.egg-info/requires.txt
+-rw-r--r--   0 tabot      (501) staff       (20)        9 2023-06-22 23:03:47.000000 Flask_Limit-2.0/flask_limit/Flask_Limit.egg-info/top_level.txt
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:03:47.287412 Flask_Limit-2.0/flask_limit/limiters/
+-rw-r--r--   0 tabot      (501) staff       (20)      120 2023-06-19 02:52:18.000000 Flask_Limit-2.0/flask_limit/limiters/__init__.py
+-rw-r--r--   0 tabot      (501) staff       (20)       44 2023-06-18 17:50:49.000000 Flask_Limit-2.0/flask_limit/limiters/exceptions.py
+-rw-r--r--   0 tabot      (501) staff       (20)     2354 2023-06-18 17:48:16.000000 Flask_Limit-2.0/flask_limit/limiters/limiters.py
+-rw-r--r--   0 tabot      (501) staff       (20)       95 2023-06-19 02:37:16.000000 Flask_Limit-2.0/pyproject.toml
+-rw-r--r--   0 tabot      (501) staff       (20)      870 2023-06-22 23:03:47.288091 Flask_Limit-2.0/setup.cfg
+-rwxr-xr-x   0 tabot      (501) staff       (20)       38 2023-06-19 01:33:15.000000 Flask_Limit-2.0/setup.py
+drwxr-xr-x   0 tabot      (501) staff       (20)        0 2023-06-22 23:03:47.287644 Flask_Limit-2.0/tests/
+-rw-r--r--   0 tabot      (501) staff       (20)        0 2023-06-11 23:35:14.000000 Flask_Limit-2.0/tests/__init__.py
+-rw-r--r--   0 tabot      (501) staff       (20)     2048 2023-06-22 20:24:17.000000 Flask_Limit-2.0/tests/test_rate_limit.py
```

### Comparing `Flask_Limit-1.0.5/Flask_Limit.egg-info/PKG-INFO` & `Flask_Limit-2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 Metadata-Version: 2.1
-Name: Flask-Limit
-Version: 1.0.5
+Name: Flask_Limit
+Version: 2.0
 Summary: An extension that provides rate limiting for Flask routes.
 Home-page: https://github.com/tabotkevin/flask_limit
 Author: Tabot Kevin
 Author-email: tabot.kevin@gmail.com
 License: MIT
-Platform: any
+Project-URL: Bug Tracker, https://github.com/tabotkevin/flask_limit/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-Flask_Limit
-==============
+# Flask_Limit
+
+[![Build status](https://github.com/tabotkevin/flask_limit/actions/workflows/tests.yml/badge.svg)](https://github.com/tabotkevin/flask_limit/actions)
 
 An extension that provides rate limiting for Flask routes.
 
-Installation
-------------
+## Installation
+
 The easiest way to install this is through pip.
-```
+
+```shell
 pip install Flask_Limit
 ```
 
-Configuration
-----------------------------
+## Configuration
 
 This extension depends on two configuration parameters **RATELIMITE_LIMIT** and **RATELIMIT_PERIOD**.
 If this parameters are not set, default values of **10** and **20** are used respectively,
 which represents the number of allowed requests(limit) within a given time(period).
 
-Basic Usage
-----------------------------
+## Basic Usage
 
 The easiest way to rate limit the entire application is limit the application's before request method.
 The **rate_limit** decorator can be called with or without the **litmit** and **period** paramters.
 If this parameters are not provided, the values are gotten from the application's configuration.
 In the example below, after rate limiting the **before_request** method, a get request to **/greet/<name>**
 will show from the response headers that the rate limiting is working.
 
+## In-Memory example
+
+This example uses `MemRateLimit` which is the default Rate-Limiter.
+
 ```python
 from flask import Flask, g
 from flask_limit import RateLimiter
 
 class Config:
-	RATELIMITE_LIMIT = 10
-	RATELIMIT_PERIOD = 30
+	RATELIMIT_LIMIT = 10  # Number of allowed requests.
+	RATELIMIT_PERIOD = 30  # Period in seconds.
 
 app = Flask(__name__)
 app.config.from_object(Config)
 limiter = RateLimiter(app)
 
 @app.before_request
 @limiter.rate_limit
@@ -77,25 +78,66 @@
     return f'Hello {name}!'
 
 
 if __name__ == '__main__':
     app.run()
 ```
 
+## Redis example
+
+This example uses `RedisRateLimit` as the Rate-Limiter.
+Remember to set the `REDIS_URL` parameter in your configuration
+
+```python
+from flask import Flask, g
+from flask_limit import RateLimiter
+
+class Config:
+    RATELIMIT_LIMIT = 10
+    RATELIMIT_PERIOD = 30
+    REDIS_URL = "redis://localhost:6379/0"
+
+
+app = Flask(__name__)
+app.config.from_object(Config)
+limiter = RateLimiter(app, limiter="redis")
+
+
+@app.before_request
+@limiter.rate_limit
+def before_request():
+    pass
+
+
+@app.after_request
+def after_request(rv):
+    headers = getattr(g, "headers", {})
+    rv.headers.extend(headers)
+    return rv
+
+
+@app.route("/greet/<name>")
+def greet(name):
+    return f"Hello {name}!"
+
+
+if __name__ == "__main__":
+    app.run()
+```
+
+## Complex example
 
-Complex example
------------------------------
 More than one route can be rate limited.
 
 ```python
 from flask import Flask, g
 from flask_limit import RateLimiter
 
 class Config:
-	RATELIMITE_LIMIT = 10
+	RATELIMIT_LIMIT = 10
 	RATELIMIT_PERIOD = 30
 
 app = Flask(__name__)
 app.config.from_object(Config)
 limiter = RateLimiter(app)
 
 @app.before_request
@@ -120,18 +162,19 @@
 def get_auth_token():
     return {'token': '<auth-token>'}
 
 if __name__ == '__main__':
     app.run()
 ```
 
+## Tests
 
-Proof
-----------------------------
-
-![proof](proof.png)
+```shell
+  python -m pip install --upgrade pip
+  pip install tox tox-gh-actions
 
+  tox
+```
 
-Credit
-----------------------------
+## Proof
 
-Credit to **Miguel Grinberg** for his exception work on rate limiting, from which this extension is based on.
+![proof](proof.png)
```

### Comparing `Flask_Limit-1.0.5/LICENSE` & `Flask_Limit-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask_Limit-1.0.5/PKG-INFO` & `Flask_Limit-2.0/flask_limit/Flask_Limit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 Metadata-Version: 2.1
-Name: Flask_Limit
-Version: 1.0.5
+Name: Flask-Limit
+Version: 2.0
 Summary: An extension that provides rate limiting for Flask routes.
 Home-page: https://github.com/tabotkevin/flask_limit
 Author: Tabot Kevin
 Author-email: tabot.kevin@gmail.com
 License: MIT
-Platform: any
+Project-URL: Bug Tracker, https://github.com/tabotkevin/flask_limit/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-Flask_Limit
-==============
+# Flask_Limit
+
+[![Build status](https://github.com/tabotkevin/flask_limit/actions/workflows/tests.yml/badge.svg)](https://github.com/tabotkevin/flask_limit/actions)
 
 An extension that provides rate limiting for Flask routes.
 
-Installation
-------------
+## Installation
+
 The easiest way to install this is through pip.
-```
+
+```shell
 pip install Flask_Limit
 ```
 
-Configuration
-----------------------------
+## Configuration
 
 This extension depends on two configuration parameters **RATELIMITE_LIMIT** and **RATELIMIT_PERIOD**.
 If this parameters are not set, default values of **10** and **20** are used respectively,
 which represents the number of allowed requests(limit) within a given time(period).
 
-Basic Usage
-----------------------------
+## Basic Usage
 
 The easiest way to rate limit the entire application is limit the application's before request method.
 The **rate_limit** decorator can be called with or without the **litmit** and **period** paramters.
 If this parameters are not provided, the values are gotten from the application's configuration.
 In the example below, after rate limiting the **before_request** method, a get request to **/greet/<name>**
 will show from the response headers that the rate limiting is working.
 
+## In-Memory example
+
+This example uses `MemRateLimit` which is the default Rate-Limiter.
+
 ```python
 from flask import Flask, g
 from flask_limit import RateLimiter
 
 class Config:
-	RATELIMITE_LIMIT = 10
-	RATELIMIT_PERIOD = 30
+	RATELIMIT_LIMIT = 10  # Number of allowed requests.
+	RATELIMIT_PERIOD = 30  # Period in seconds.
 
 app = Flask(__name__)
 app.config.from_object(Config)
 limiter = RateLimiter(app)
 
 @app.before_request
 @limiter.rate_limit
@@ -77,25 +78,66 @@
     return f'Hello {name}!'
 
 
 if __name__ == '__main__':
     app.run()
 ```
 
+## Redis example
+
+This example uses `RedisRateLimit` as the Rate-Limiter.
+Remember to set the `REDIS_URL` parameter in your configuration
+
+```python
+from flask import Flask, g
+from flask_limit import RateLimiter
+
+class Config:
+    RATELIMIT_LIMIT = 10
+    RATELIMIT_PERIOD = 30
+    REDIS_URL = "redis://localhost:6379/0"
+
+
+app = Flask(__name__)
+app.config.from_object(Config)
+limiter = RateLimiter(app, limiter="redis")
+
+
+@app.before_request
+@limiter.rate_limit
+def before_request():
+    pass
+
+
+@app.after_request
+def after_request(rv):
+    headers = getattr(g, "headers", {})
+    rv.headers.extend(headers)
+    return rv
+
+
+@app.route("/greet/<name>")
+def greet(name):
+    return f"Hello {name}!"
+
+
+if __name__ == "__main__":
+    app.run()
+```
+
+## Complex example
 
-Complex example
------------------------------
 More than one route can be rate limited.
 
 ```python
 from flask import Flask, g
 from flask_limit import RateLimiter
 
 class Config:
-	RATELIMITE_LIMIT = 10
+	RATELIMIT_LIMIT = 10
 	RATELIMIT_PERIOD = 30
 
 app = Flask(__name__)
 app.config.from_object(Config)
 limiter = RateLimiter(app)
 
 @app.before_request
@@ -120,18 +162,19 @@
 def get_auth_token():
     return {'token': '<auth-token>'}
 
 if __name__ == '__main__':
     app.run()
 ```
 
+## Tests
 
-Proof
-----------------------------
-
-![proof](proof.png)
+```shell
+  python -m pip install --upgrade pip
+  pip install tox tox-gh-actions
 
+  tox
+```
 
-Credit
-----------------------------
+## Proof
 
-Credit to **Miguel Grinberg** for his exception work on rate limiting, from which this extension is based on.
+![proof](proof.png)
```

### Comparing `Flask_Limit-1.0.5/README.md` & `Flask_Limit-2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-Flask_Limit
-==============
+# Flask_Limit
+
+[![Build status](https://github.com/tabotkevin/flask_limit/actions/workflows/tests.yml/badge.svg)](https://github.com/tabotkevin/flask_limit/actions)
 
 An extension that provides rate limiting for Flask routes.
 
-Installation
-------------
+## Installation
+
 The easiest way to install this is through pip.
-```
+
+```shell
 pip install Flask_Limit
 ```
 
-Configuration
-----------------------------
+## Configuration
 
 This extension depends on two configuration parameters **RATELIMITE_LIMIT** and **RATELIMIT_PERIOD**.
 If this parameters are not set, default values of **10** and **20** are used respectively,
 which represents the number of allowed requests(limit) within a given time(period).
 
-Basic Usage
-----------------------------
+## Basic Usage
 
 The easiest way to rate limit the entire application is limit the application's before request method.
 The **rate_limit** decorator can be called with or without the **litmit** and **period** paramters.
 If this parameters are not provided, the values are gotten from the application's configuration.
 In the example below, after rate limiting the **before_request** method, a get request to **/greet/<name>**
 will show from the response headers that the rate limiting is working.
 
+## In-Memory example
+
+This example uses `MemRateLimit` which is the default Rate-Limiter.
+
 ```python
 from flask import Flask, g
 from flask_limit import RateLimiter
 
 class Config:
-	RATELIMITE_LIMIT = 10
-	RATELIMIT_PERIOD = 30
+	RATELIMIT_LIMIT = 10  # Number of allowed requests.
+	RATELIMIT_PERIOD = 30  # Period in seconds.
 
 app = Flask(__name__)
 app.config.from_object(Config)
 limiter = RateLimiter(app)
 
 @app.before_request
 @limiter.rate_limit
@@ -55,25 +59,66 @@
     return f'Hello {name}!'
 
 
 if __name__ == '__main__':
     app.run()
 ```
 
+## Redis example
+
+This example uses `RedisRateLimit` as the Rate-Limiter.
+Remember to set the `REDIS_URL` parameter in your configuration
+
+```python
+from flask import Flask, g
+from flask_limit import RateLimiter
+
+class Config:
+    RATELIMIT_LIMIT = 10
+    RATELIMIT_PERIOD = 30
+    REDIS_URL = "redis://localhost:6379/0"
+
+
+app = Flask(__name__)
+app.config.from_object(Config)
+limiter = RateLimiter(app, limiter="redis")
+
+
+@app.before_request
+@limiter.rate_limit
+def before_request():
+    pass
+
+
+@app.after_request
+def after_request(rv):
+    headers = getattr(g, "headers", {})
+    rv.headers.extend(headers)
+    return rv
+
+
+@app.route("/greet/<name>")
+def greet(name):
+    return f"Hello {name}!"
+
+
+if __name__ == "__main__":
+    app.run()
+```
+
+## Complex example
 
-Complex example
------------------------------
 More than one route can be rate limited.
 
 ```python
 from flask import Flask, g
 from flask_limit import RateLimiter
 
 class Config:
-	RATELIMITE_LIMIT = 10
+	RATELIMIT_LIMIT = 10
 	RATELIMIT_PERIOD = 30
 
 app = Flask(__name__)
 app.config.from_object(Config)
 limiter = RateLimiter(app)
 
 @app.before_request
@@ -98,18 +143,19 @@
 def get_auth_token():
     return {'token': '<auth-token>'}
 
 if __name__ == '__main__':
     app.run()
 ```
 
+## Tests
 
-Proof
-----------------------------
-
-![proof](proof.png)
+```shell
+  python -m pip install --upgrade pip
+  pip install tox tox-gh-actions
 
+  tox
+```
 
-Credit
-----------------------------
+## Proof
 
-Credit to **Miguel Grinberg** for his exception work on rate limiting, from which this extension is based on.
+![proof](proof.png)
```

### Comparing `Flask_Limit-1.0.5/docs/index.rst` & `Flask_Limit-2.0/docs/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,19 @@
    sphinx-quickstart on Wed Dec 25 15:29:13 2019.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to Flask-Limit's documentation!
 ==========================================
 
+.. raw:: html
+   <a href="https://github.com/tabotkevin/flask_limit/actions">
+    <img src="https://github.com/tabotkevin/flask_limit/actions/workflows/tests.yml/badge.svg">
+   </a>
+
 **Flask-Limit** is an extension that provides rate limiting for Flask routes.
 
 
 Installation
 -----------------------------
 
 The easiest way to install this is through pip::
@@ -26,22 +31,27 @@
 Basic Example
 -----------------------------
 
 The easiest way to rate limit the entire application is limit the application's before request method.
 The **rate_limit** decorator can be called with or without the **litmit** and **period** paramters.
 If this parameters are not provided, the values are gotten from the application's configuration.
 In the example below, after rate limiting the **before_request** method, a get request to **/greet/<name>**
-will show from the response headers that the rate limiting is working.::
+will show from the response headers that the rate limiting is working.
+
+
+In-Memory example
+-----------------------------
+This example uses `MemRateLimit` which is the default Rate-Limiter.::
 
    from flask import Flask, g
    from flask_limit import RateLimiter
 
    class Config:
-      RATELIMITE_LIMIT = 10
-      RATELIMIT_PERIOD = 30
+      RATELIMITE_LIMIT = 10  # Number of allowed requests.
+      RATELIMIT_PERIOD = 30  # Period in seconds.
 
    app = Flask(__name__)
    app.config.from_object(Config)
    limiter = RateLimiter(app)
 
    @app.before_request
    @limiter.rate_limit
@@ -57,15 +67,56 @@
    @app.route('/greet/<name>')
    def greet(name):
        return f'Hello {name}!'
 
 
    if __name__ == '__main__':
        app.run()
-    
+
+
+Redis example
+-----------------------------
+This example uses `RedisRateLimit` as the Rate-Limiter.
+Remember to set the `REDIS_URL` parameter in your configuration.::
+
+   from flask import Flask, g
+   from flask_limit import RateLimiter
+
+  class Config:
+      RATELIMIT_LIMIT = 10
+      RATELIMIT_PERIOD = 30
+      REDIS_URL = "redis://localhost:6379/0"
+
+
+  app = Flask(__name__)
+  app.config.from_object(Config)
+  limiter = RateLimiter(app, limiter="redis")
+
+
+  @app.before_request
+  @limiter.rate_limit
+  def before_request():
+      pass
+
+
+  @app.after_request
+  def after_request(rv):
+      headers = getattr(g, "headers", {})
+      rv.headers.extend(headers)
+      return rv
+
+
+  @app.route("/greet/<name>")
+  def greet(name):
+      return f"Hello {name}!"
+
+
+  if __name__ == "__main__":
+      app.run()
+
 
 Complex example
 -----------------------------
 More than one route can be rate limited::
 
    from flask import Flask, g
    from flask_limit import RateLimiter
@@ -98,17 +149,22 @@
    def get_auth_token():
         return {'token': '<auth-token>'}
 
    if __name__ == '__main__':
        app.run()
 
 
-Proof
+
+Tests
 ----------------------------
+::
+
+  python -m pip install --upgrade pip
+  pip install tox tox-gh-actions
 
-.. image:: ../proof.png
+  tox
 
 
-Credit
+Proof
 ----------------------------
 
-Credit to **Miguel Grinberg** for his exception work on rate limiting, from which this extension is based on.
+.. image:: proof.png
```

### Comparing `Flask_Limit-1.0.5/tests/test_rate_limit.py` & `Flask_Limit-2.0/tests/test_rate_limit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 import unittest
 from flask import Flask, g
 import json
 from flask_limit import RateLimiter
 
 
 class RateLimiterTestCase(unittest.TestCase):
-
     def setUp(self):
         app = Flask(__name__)
-        app.config['RATELIMITE_LIMIT'] = 10
-        app.config['RATELIMIT_PERIOD'] = 30
+        app.config["RATELIMITE_LIMIT"] = 10
+        app.config["RATELIMIT_PERIOD"] = 30
 
         limiter = RateLimiter(app)
 
         @app.before_request
         @limiter.rate_limit
         def before_request():
             pass
 
         @app.after_request
         def after_request(rv):
-            headers = getattr(g, 'headers', {})
+            headers = getattr(g, "headers", {})
             rv.headers.extend(headers)
             return rv
 
-        @app.route('/greet/<name>')
+        @app.route("/greet/<name>")
         def greet(name):
             return self.greeting
 
-        @app.route('/get-auth-token')
+        @app.route("/get-auth-token")
         @limiter.rate_limit(limit=1, period=600)  # one call per 10 minute period
         def get_auth_token():
-            return self.token
+            return "<token>"
 
         self.app = app
         self.client = app.test_client()
-        self.name = 'Tabot'
-        self.greeting = f'Hello {self.name}!'
+        self.name = "Tabot"
+        self.greeting = f"Hello {self.name}!"
         self.error_message = {
             "error": "too many requests",
             "message": "You have exceeded your request rate",
-            "status": 429
+            "status": 429,
         }
 
     def test_rate_limit(self):
-        limit = self.app.config['RATELIMITE_LIMIT']
+        limit = self.app.config["RATELIMIT_LIMIT"]
         count = limit
         while count > 0:
             if count != 0:
-                response = self.client.get(f'/greet/{self.name}')
+                response = self.client.get(f"/greet/{self.name}")
                 self.assertEqual(response.status_code, 200)
-                self.assertEqual(response.headers['X-RateLimit-Limit'], str(limit))
-                self.assertEqual(response.headers['X-RateLimit-Remaining'], str(count-1))
-                self.assertEqual(response.data.decode('utf-8'), self.greeting)
+                self.assertEqual(response.headers["X-RateLimit-Limit"], str(limit))
+                self.assertEqual(
+                    response.headers["X-RateLimit-Remaining"], str(count - 1)
+                )
+                self.assertEqual(response.data.decode("utf-8"), self.greeting)
             else:
+                response = self.client.get(f"/greet/{self.name}")
                 self.assertEqual(response.status_code, 429)
-                self.assertEqual(json.loads(response.data.decode('utf-8')), self.error_message)
+                self.assertEqual(
+                    json.loads(response.data.decode("utf-8")), self.error_message
+                )
             count -= 1
```

