# Comparing `tmp/sabledocs-0.4.182.dev0.tar.gz` & `tmp/sabledocs-0.4.184.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.4.182.dev0.tar", last modified: Fri Jun 23 18:58:22 2023, max compression
+gzip compressed data, was "sabledocs-0.4.184.dev0.tar", last modified: Fri Jun 23 19:09:43 2023, max compression
```

## Comparing `sabledocs-0.4.182.dev0.tar` & `sabledocs-0.4.184.dev0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.387031 sabledocs-0.4.182.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4805 2023-06-23 18:58:22.387031 sabledocs-0.4.182.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4260 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-06-23 18:58:22.391031 sabledocs-0.4.182.dev0/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.383031 sabledocs-0.4.182.dev0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.383031 sabledocs-0.4.182.dev0/src/sabledocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3346 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/lunr_search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13645 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.383031 sabledocs-0.4.182.dev0/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.387031 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5412 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/search.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.387031 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   260942 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.387031 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4805 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4261 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.599387 sabledocs-0.4.184.dev0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/lunr_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13934 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.599387 sabledocs-0.4.184.dev0/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5412 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/search.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   260942 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.4.182.dev0/LICENSE` & `sabledocs-0.4.184.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/PKG-INFO` & `sabledocs-0.4.184.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.4.182.dev0
+Version: 0.4.184.dev0
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,15 +34,15 @@
 protoc *.proto -o descriptor.pb --include_source_info
 ```
 
 *(It's important to use the `--include_source_info` flag, otherwise the comments will not be included in the generated documentation.)*
 
 The generated `descriptor.pb` file will be the input needed to build the documentation site.
 
-### Build the documetation
+### Build the documentation
 
 Install the `sabledocs` package. It requires [Python](https://www.python.org/downloads/) (version 3.11 or higher) to be installed.
 
 ```
 pip install sabledocs
 ```
```

### Comparing `sabledocs-0.4.182.dev0/README.md` & `sabledocs-0.4.184.dev0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 protoc *.proto -o descriptor.pb --include_source_info
 ```
 
 *(It's important to use the `--include_source_info` flag, otherwise the comments will not be included in the generated documentation.)*
 
 The generated `descriptor.pb` file will be the input needed to build the documentation site.
 
-### Build the documetation
+### Build the documentation
 
 Install the `sabledocs` package. It requires [Python](https://www.python.org/downloads/) (version 3.11 or higher) to be installed.
 
 ```
 pip install sabledocs
 ```
```

### Comparing `sabledocs-0.4.182.dev0/pyproject.toml` & `sabledocs-0.4.184.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/__main__.py` & `sabledocs-0.4.184.dev0/src/sabledocs/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     package_template = jinja_env.get_template("package.html")
 
     if not os.path.exists(sable_config.output_dir):
         os.makedirs(sable_config.output_dir)
 
     # NOTE: When the output files are generated, the encode('utf-8') option has to be used, otherwise Unicode characters like © can end up garbled.
     for package in sable_context.packages:
-        with open(os.path.join(sable_config.output_dir, f'{package.name}.html'), 'wb') as fh:
+        with open(os.path.join(sable_config.output_dir, f'{package.name if package.name else "__default"}.html'), 'wb') as fh:
             output = package_template.render(
                 sable_config=sable_config,
                 package=package,
                 packages=sable_context.packages,
                 all_messages=sable_context.all_messages,
                 all_enums=sable_context.all_enums).encode('utf-8')
```

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/lunr_search.py` & `sabledocs-0.4.184.dev0/src/sabledocs/lunr_search.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.4.184.dev0/src/sabledocs/proto_descriptor_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         ev.description_html = markdown.markdown(ev.description)
         ev.line_number = ctx.GetLineNumber()
 
         return ev
 
     e = Enum()
     e.name = enum.name
-    e.full_name = f"{ctx.package.name}.{nested_type_chain}{enum.name}"
+    e.full_name = f"{ctx.package.name}.{nested_type_chain}{enum.name}".lstrip(".")
     e.parent_message = parent_message
     e.description = ctx.GetComments()
     e.description_html = markdown.markdown(e.description)
     e.source_file_path = ctx.source_file_path
     e.line_number = ctx.GetLineNumber()
     e.repository_url = build_source_code_url(
         ctx.config.repository_url,
@@ -138,15 +138,15 @@
 
 def parse_message(message: DescriptorProto, ctx: ParseContext, parent_message, nested_type_chain: str):
     #if message.oneof_decl:
         #pprint.pprint(message.oneof_decl)
 
     m = Message()
     m.name = message.name
-    m.full_name = f"{ctx.package.name}.{nested_type_chain}{message.name}"
+    m.full_name = f"{ctx.package.name}.{nested_type_chain}{message.name}".lstrip(".")
     m.parent_message = parent_message
     m.description = ctx.GetComments()
     m.description_html = markdown.markdown(m.description)
     m.source_file_path = ctx.source_file_path
     m.line_number = ctx.GetLineNumber()
     m.repository_url = build_source_code_url(
         ctx.config.repository_url,
@@ -194,15 +194,15 @@
 
     return sm
 
 
 def parse_service(service: ServiceDescriptorProto, ctx: ParseContext):
     s = Service()
     s.name = service.name
-    s.full_name = f"{ctx.package.name}.{service.name}"
+    s.full_name = f"{ctx.package.name}.{service.name}".lstrip(".")
     s.description = ctx.GetComments()
     s.description_html = markdown.markdown(s.description)
     s.source_file_path = ctx.source_file_path
     s.line_number = ctx.GetLineNumber()
     s.repository_url = build_source_code_url(
         ctx.config.repository_url,
         ctx.config.repository_type,
@@ -218,14 +218,22 @@
 def parse_services(services: list[ServiceDescriptorProto], ctx: ParseContext):
     for (i, service) in enumerate(services):
         ctx.package.services.append(parse_service(service, ctx.ExtendPath(i)))
 
     ctx.package.services.sort(key=lambda s: s.name)
 
 
+def extract_package_name_from_full_name(full_type_name: str):
+    last_dot = full_type_name.rfind(".")
+    if last_dot == -1:
+        return ""
+    else:
+        return full_type_name[:last_dot]
+
+
 def add_package_references(messages: list[Message], services: list[Service], packages):
     for m in messages:
         package = next(filter(lambda p: m.full_name.startswith(p.name), packages), None)
         if package is not None:
             m.package = package
 
         for mf in m.fields:
@@ -238,19 +246,19 @@
 
             package = next(filter(lambda p: mf.full_type.startswith(p.name), packages), None)
             if package is not None:
                 mf.package = package
 
     for s in services:
         for sm in s.methods:
-            requestPackage = next(filter(lambda p: sm.request.full_type.startswith(p.name), packages), None)
+            requestPackage = next(filter(lambda p: extract_package_name_from_full_name(sm.request.full_type) == p.name, packages), None)
             if requestPackage is not None:
                 sm.request.package = requestPackage
 
-            responsePackage = next(filter(lambda p: sm.response.full_type.startswith(p.name), packages), None)
+            responsePackage = next(filter(lambda p: extract_package_name_from_full_name(sm.response.full_type) == p.name, packages), None)
             if responsePackage is not None:
                 sm.response.package = responsePackage
 
 
 def build_location_map(source_code_info):
     def build_key(path):
         return '.'.join(map(lambda i: str(i), path))
```

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/proto_model.py` & `sabledocs-0.4.184.dev0/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/sable_config.py` & `sabledocs-0.4.184.dev0/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/base.html` & `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/index.html` & `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -9,15 +9,19 @@
   <h3 id="packages" class="title is-3">
     Packages
   </h3>
   <div class="block">This site contains the documentation for the following Protobuf packages.</div>
   <div class="block">
   {% for p in packages %}
     <h5 class="title is-5">
-      <a href="{{ p.name }}.html">{{ p.name }}</a>
+      {% if p.name %}
+        <a href="{{ p.name }}.html">{{ p.name }}</a>
+      {% else %}
+        <a href="__default.html">(Default package)</a>
+      {% endif %}
     </h4>
     {% if p.description_html %}
     <div style="margin-top: -0.5rem; margin-bottom: 2.5rem">
       {{ p.description_html | safe }}
     </div>
     {% endif %}
   {% endfor %}
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_bfstswrg_/tmptvyfc8j2_TarContainer/0/19.html", line 19, column 6: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_bfstswrg_/tmptvyfc8j2_TarContainer/0/19.html", line 19, column 6: Levels of opening and closing headings don't match*

```diff
@@ -1,12 +1,12 @@
 {% extends "base.html" %} {% block content %} {% if main_page_content %}
 â_Packages
 {{ main_page_content | safe }}
 {% endif %}
 **** Packages ****
 This site contains the documentation for the following Protobuf packages.
 {% for p in packages %}
-** {{_p.name_}} **
+** {% if p.name %} {{_p.name_}} {% else %} (Default_package) {% endif %} **
 {% if p.description_html %}
 {{ p.description_html | safe }}
 {% endif %} {% endfor %}
 {% endblock %}
```

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/message.html` & `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/package.html` & `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/package.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 {% extends "base.html" %}
 {% block content %}
   <p class="mb-2">
     <a style="font-size: 0.9em" href="index.html">← Back to packages</a>
   </p>
   <h4 class="title is-4">
+    {% if package.name %}
     Package <code>{{ package.name }}</code>
+    {% else %}
+    Default package
+    {% endif %}
   </h4>
 
   <div class="block">
     {% for service in package.services %}
     <p>
       <a href="#service-{{ service.full_name }}">
         <span class="tag" style="min-width: 6em">Service</span>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends "base.html" %} {% block content %}
 â_Back_to_packages
-*** Package {{ package.name }} ***
+*** {% if package.name %} Package {{ package.name }} {% else %} Default package
+{% endif %} ***
 {% for service in package.services %}
 Service_{{_service.name_}}
 {% endfor %} {% for message in package.messages %} {% if not
 message.is_map_entry %}
 Message_{{_message.name_}}
 {% endif %} {% endfor %} {% for enum in package.enums %}
 Enum_{{_enum.name_}}
```

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/search.html` & `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/search.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/service.html` & `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/type_name.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ## The %- and -% syntax is used everywhere to trim all the whitespace, to make sure no extra unwanted spaces are around the type name, for example if it's displayed between parens.
 {%- macro type_name(message_field) -%}
   {%- if message_field.package and message_field.type_kind != "UNKNOWN" -%}
     {%- if message_field.type_kind == "MESSAGE" -%}
-      <a href="{{ message_field.package.name }}.html#message-{{ message_field.full_type }}">
+      <a href="{{ message_field.package.name if message_field.package.name else "__default" }}.html#message-{{ message_field.full_type }}">
     {%- else -%}
-      <a href="{{ message_field.package.name }}.html#enum-{{ message_field.full_type }}">
+      <a href="{{ message_field.package.name if message_field.package.name else "__default" }}.html#enum-{{ message_field.full_type }}">
     {%- endif -%}
-      <span title="{{ message_field.full_type }}">{{ message_field.full_type }}</span></a>
+      <span title="{{ message_field.full_type }}">{{ message_field.full_type }}</span>
+    </a>
   {%- else -%}
   <span>{{ message_field.full_type }}</span>
   {%- endif -%}
 {%- endmacro -%}
```

#### html2text {}

```diff
@@ -1,7 +1,9 @@
 ## The %- and -% syntax is used everywhere to trim all the whitespace, to make
 sure no extra unwanted spaces are around the type name, for example if it's
 displayed between parens. {%- macro type_name(message_field) -%} {%- if
 message_field.package and message_field.type_kind != "UNKNOWN" -%} {%- if
-message_field.type_kind == "MESSAGE" -%} {%-_else_-%}_{%-_endif_-%}_{
-{_message_field.full_type_}}_{%-_else_-%}_{{_message_field.full_type_}}_{%-
-endif_-%}_{%-_endmacro_-%}_
+message_field.type_kind == "MESSAGE" -%}
+ }}.html#message-{{ message_field.full_type }}"> {%- else -%}
+ }}.html#enum-{{ message_field.full_type }}"> {%- endif -%} {
+{ message_field.full_type }}
+ {%- else -%} {{ message_field.full_type }} {%- endif -%} {%- endmacro -%}
```

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.4.184.dev0/src/sabledocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.4.182.dev0
+Version: 0.4.184.dev0
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,15 +34,15 @@
 protoc *.proto -o descriptor.pb --include_source_info
 ```
 
 *(It's important to use the `--include_source_info` flag, otherwise the comments will not be included in the generated documentation.)*
 
 The generated `descriptor.pb` file will be the input needed to build the documentation site.
 
-### Build the documetation
+### Build the documentation
 
 Install the `sabledocs` package. It requires [Python](https://www.python.org/downloads/) (version 3.11 or higher) to be installed.
 
 ```
 pip install sabledocs
 ```
```

### Comparing `sabledocs-0.4.182.dev0/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.4.184.dev0/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

