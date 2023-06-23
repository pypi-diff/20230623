# Comparing `tmp/wappstore-0.0.0.tar.gz` & `tmp/wappstore-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wappstore-0.0.0.tar", max compression
+gzip compressed data, was "wappstore-1.0.1.tar", max compression
```

## Comparing `wappstore-0.0.0.tar` & `wappstore-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0    11344 2023-06-09 04:52:14.975530 wappstore-0.0.0/LICENSE
--rw-r--r--   0        0        0     1657 2023-06-11 08:37:04.206917 wappstore-0.0.0/README.md
--rw-r--r--   0        0        0      786 2023-06-11 10:28:15.647400 wappstore-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-10 10:57:51.601395 wappstore-0.0.0/wappstore/__init__.py
--rw-r--r--   0        0        0       96 2023-06-07 14:03:48.378353 wappstore-0.0.0/wappstore/data/README.md
--rw-r--r--   0        0        0        0 2023-06-07 17:13:24.757929 wappstore-0.0.0/wappstore/data/__init__.py
--rw-r--r--   0        0        0      512 2023-06-09 10:15:28.997971 wappstore-0.0.0/wappstore/data/crud.py
--rw-r--r--   0        0        0      462 2023-06-08 09:09:05.364909 wappstore-0.0.0/wappstore/data/database.py
--rw-r--r--   0        0        0     3431 2023-06-09 09:32:24.222208 wappstore-0.0.0/wappstore/data/models.py
--rw-r--r--   0        0        0      437 2023-06-08 05:47:35.769547 wappstore-0.0.0/wappstore/data/schemas.py
--rw-r--r--   0        0        0       58 2023-06-07 09:52:50.301257 wappstore-0.0.0/wappstore/input.css
--rw-r--r--   0        0        0     5934 2023-06-11 09:41:30.653194 wappstore-0.0.0/wappstore/main.py
--rw-r--r--   0        0        0    25608 2023-06-09 10:36:06.675464 wappstore-0.0.0/wappstore/static/output.css
--rw-r--r--   0        0        0      481 2023-06-08 09:42:32.941055 wappstore-0.0.0/wappstore/templates/apps/detail.html
--rw-r--r--   0        0        0     4121 2023-06-09 10:36:20.011761 wappstore-0.0.0/wappstore/templates/apps/index.html
--rw-r--r--   0        0        0     2036 2023-06-08 06:47:45.178547 wappstore-0.0.0/wappstore/templates/apps/new.html
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 wappstore-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-06-23 17:18:07.031036 wappstore-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2169 2023-06-23 17:18:07.031036 wappstore-1.0.1/README.md
+-rw-r--r--   0        0        0      942 2023-06-23 17:18:07.031036 wappstore-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/__init__.py
+-rw-r--r--   0        0        0       96 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/data/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/data/__init__.py
+-rw-r--r--   0        0        0      944 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/data/crud.py
+-rw-r--r--   0        0        0      805 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/data/database.py
+-rw-r--r--   0        0        0     5919 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/data/models.py
+-rw-r--r--   0        0        0     1455 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/data/seeding.py
+-rw-r--r--   0        0        0       58 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/input.css
+-rw-r--r--   0        0        0     6987 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/main.py
+-rw-r--r--   0        0        0     3286 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/models.py
+-rw-r--r--   0        0        0    17110 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/static/output.css
+-rw-r--r--   0        0        0     3562 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/templates/apps/detail.html
+-rw-r--r--   0        0        0     6119 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/templates/apps/index.html
+-rw-r--r--   0        0        0     2904 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/templates/apps/new.html
+-rw-r--r--   0        0        0      457 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/url.py
+-rw-r--r--   0        0        0     7125 2023-06-23 17:18:07.031036 wappstore-1.0.1/wappstore/webmanifest.py
+-rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 wappstore-1.0.1/PKG-INFO
```

### Comparing `wappstore-0.0.0/LICENSE` & `wappstore-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wappstore-0.0.0/pyproject.toml` & `wappstore-1.0.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [tool.poetry]
 name = "wappstore"
-version = "0.0.0"
+version = "1.0.1"
 description = "Improve Web App discoverability"
 authors = ["Claas <claas.moehlmann@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/SantaClaas/wApp"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 fastapi = "^0.96.0"
 uvicorn = "^0.22.0"
 # For database stuff
 sqlalchemy = "^2.0.15"
 # For HTML templating
 jinja2 = "^3.1.2"
 # To ensure form support as recommended by FastAPI
 python-multipart = "^0.0.6"
+# Make http requests eaiser (urlopen is hard to work with or I am unfamiliar with it so currently it is annoying)
+httpx = "^0.24.1"
+marshmallow = "^3.19.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
 autopep8 = "^2.0.2"
 black = "^23.3.0"
 yapf = "^0.33.0"
 bandit = "^1.7.5"
```

### Comparing `wappstore-0.0.0/wappstore/templates/apps/index.html` & `wappstore-1.0.1/wappstore/templates/apps/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,62 @@
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
     <meta charset="utf-8">
-    <title> Apps - Web App Store</title>
+    <title>Apps - Web App Store</title>
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link href="{{ url_for('static', path='/output.css') }}" rel="stylesheet">
+    <meta name="description" content="Discover the apps of the web!">
+    <base href="/">
+    <link href="static/output.css" rel="stylesheet">
 </head>
 
 <body class="bg-slate-50">
-    <header class="p-8">
+    <header class="p-8 flex justify-between">
 
-        <h1 class="text-4xl font-bold leading-7 text-slate-900 sm:truncate sm:text-5xl sm:tracking-tight">Apps
+        <h1 class="text-4xl font-bold text-slate-900 sm:truncate sm:text-5xl sm:tracking-tight">Apps
         </h1>
 
+
+        {% if not is_delete %}
+        <a href="/apps/delete" class="h-10 w-10 p-2 text-slate-500">
+            <svg fill="none" stroke="currentColor" stroke-width="1.5" viewBox="0 0 24 24"
+                xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
+                <path stroke-linecap="round" stroke-linejoin="round"
+                    d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0">
+                </path>
+            </svg>
+        </a>
+        {% else %}
+        <a href="/apps" class="h-10 w-10 p-2 text-slate-500">
+            <svg fill="none" stroke="currentColor" stroke-width="1.5" viewBox="0 0 24 24"
+                xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
+                <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"></path>
+            </svg>
+        </a>
+
+
+        {% endif %}
+
     </header>
 
     <main class="p-8">
         <ul role="list" class="grid grid-cols-2 gap-x-4 gap-y-8 sm:grid-cols-3 sm:gap-x-6 lg:grid-cols-4 xl:gap-x-8 ">
             {% for app in apps %}
             {# Remember to repeat with add item #}
             <li class="relative bg-slate-100 rounded-2xl group hover:opacity-75 shadow-md">
+                {% if is_delete %}
+                <a href="apps/delete/{{ app['id']}}"
+                    class="absolute -top-4 -right-4 p-2 rounded-full bg-red-600 text-slate-50 w-10 h-10">
+                    <svg fill="none" stroke="currentColor" stroke-width="1.5" viewBox="0 0 24 24"
+                        xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
+                        <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"></path>
+                    </svg>
+                </a>
+                {% endif %}
                 <section class="block aspect-square overflow-hidden rounded-xl bg-slate-200 focus-within:ring-2 shadow
                            focus-within:ring-indigo-500 focus-within:ring-offset-2 focus-within:ring-offset-slate-100">
                     <img src="{{ app['icon_url'] }}" alt="App icon for {{ app['name'] }}"
                         class="pointer-events-none w-full h-full object-center group-hover:opacity-75">
 
                 </section>
                 <section class="px-4 pt-2">
@@ -45,23 +77,28 @@
                     <h2 class="pointer-events-none block truncate text-base font-normal text-slate-900">
                         {{
                         app["name"]
                         }}
                     </h2>
 
 
+                    {% if app["description"] %}
                     <p class="pointer-events-none block text-sm font-normal text-slate-500">{{
                         app["description"] }}</p>
+                    {% endif %}
 
 
 
                 </section>
+
+                {% if not is_delete %}
                 <a href="apps/{{ app['id'] }}" class="absolute inset-0 focus:outline-none ">
                     <span class="sr-only">View details for {{ app["name"] }} </span>
                 </a>
+                {% endif %}
             </li>
             {% endfor %}
             <li class="relative bg-slate-100 rounded-2xl group hover:opacity-75 shadow-md ">
                 <section class="block aspect-square overflow-hidden rounded-xl bg-slate-200 focus-within:ring-2 shadow
                            focus-within:ring-indigo-500 focus-within:ring-offset-2 focus-within:ring-offset-slate-100">
                     <svg class="fill-none stroke-slate-300 pointer-events-none w-full h-full object-center group-hover:opacity-75"
                         fill="none" stroke-width="1.5" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"
```

#### html2text {}

```diff
@@ -1,17 +1,21 @@
 
-****** Apps ******
 
+
+****** Apps ******
+{% if not is_delete %} ___ {% else %} __ {% endif %}
     * {% for app in apps %} {# Remember to repeat with add item #}
-    *  [App icon for {{ app['name'] }}]
+    * {% if is_delete %} __ {% endif %}  [App icon for {{ app['name'] }}]
       {% for category in app["categories"] %}  {{ category }}  {% if
       loop.length > 1 and loop.index != loop.length %} Â· {% endif %} {% endfor
       %}
 
       ***** {{ app["name"] }} *****
+      {% if app["description"] %}
       {{ app["description"] }}
-       View_details_for_{{_app["name"]_}}_
+      {% endif %}  {% if not is_delete %} View_details_for_{{_app["name"]_}}_
+      {% endif %}
     * {% endfor %}
     *
       ***** Add new App *****
       Add an app from its web manifest url
        Add_new_App
```

### Comparing `wappstore-0.0.0/wappstore/templates/apps/new.html` & `wappstore-1.0.1/wappstore/templates/apps/new.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,55 @@
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
     <meta charset="utf-8">
     <title>Web App Store</title>
     <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link href="{{ url_for('static', path='/output.css') }}" rel="stylesheet">
+    <meta name="description" content="Discover the apps of the web!">
+    <base href="/">
+    <link href="static/output.css" rel="stylesheet">
 </head>
 
-<body class="p-4 h-screen grid place-content-center">
-    <article>
-
-        <div class="bg-white shadow sm:rounded-lg">
+<body class="p-4 h-screen ">
+    <nav class="absolute top-4 left-4">
+        <a href="/apps"
+            class="rounded-full block px-2.5 py-1 text-xs font-semibold text-indigo-600 hover:text-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
+            <svg class="w-16 h-16" stroke-width="1.5" stroke="currentColor" fill="none" viewBox="0 0 24 24"
+                xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
+                <path stroke-linecap="round" stroke-linejoin="round" d="M10.5 19.5L3 12m0 0l7.5-7.5M3 12h18"></path>
+            </svg>
+        </a>
+    </nav>
+    <main class="grid place-content-center h-full">
+        <div class="bg-white shadow sm:rounded-lg h-full">
             <div class="px-4 py-5 sm:p-6">
                 <h1 class="text-base font-semibold leading-6 text-gray-900">Add Web App</h1>
                 <div class="mt-2 max-w-xl text-sm text-gray-500">
                     <p>Enter the Web App's <span
                             class="font-mono bg-gray-100 text-indigo-600 tracking-wide rounded-sm px-1">.webmanifest</span>
                         file url
                         to add
                         the App to
                         the store
                     </p>
                 </div>
+                {% if error_message %}
+                <p class="mt-2 max-w-xl text-sm text-red-500 max-w-2xl">{{ error_message }}</p>
+                {% endif %}
                 <form class="mt-5 sm:flex sm:items-center" action="/apps" method="post">
                     <div class="w-full sm:max-w-xs">
                         <label for="url" class="sr-only">Manifest Url</label>
                         <input type="url" name="url" id="url" required
                             class="block w-full rounded-md border-0 py-1.5 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6"
                             placeholder="https://example.com/app.webmanifest">
                     </div>
                     <button type="submit"
                         class="mt-3 inline-flex w-full items-center justify-center rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 sm:ml-3 sm:mt-0 sm:w-auto">Submit</button>
                 </form>
             </div>
         </div>
-    </article>
+    </main>
 
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,11 @@
 
+
+
+ __
 ****** Add Web App ******
 Enter the Web App's .webmanifest file url to add the App to the store
+{% if error_message %}
+{{ error_message }}
+{% endif %}
 Manifest Url [Unknown INPUT type]
 Submit
```

