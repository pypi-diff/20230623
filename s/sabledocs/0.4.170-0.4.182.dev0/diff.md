# Comparing `tmp/sabledocs-0.4.170.tar.gz` & `tmp/sabledocs-0.4.182.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.4.170.tar", last modified: Thu Jun  8 17:31:11 2023, max compression
+gzip compressed data, was "sabledocs-0.4.182.dev0.tar", last modified: Fri Jun 23 18:58:22 2023, max compression
```

## Comparing `sabledocs-0.4.170.tar` & `sabledocs-0.4.182.dev0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 17:31:11.266822 sabledocs-0.4.170/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-08 17:30:58.000000 sabledocs-0.4.170/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-08 17:30:58.000000 sabledocs-0.4.170/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2023-06-08 17:31:11.266822 sabledocs-0.4.170/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4261 2023-06-08 17:30:58.000000 sabledocs-0.4.170/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-08 17:30:58.000000 sabledocs-0.4.170/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-06-08 17:31:11.270822 sabledocs-0.4.170/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 17:31:11.262822 sabledocs-0.4.170/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 17:31:11.266822 sabledocs-0.4.170/src/sabledocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/lunr_search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13934 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 17:31:11.266822 sabledocs-0.4.170/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 17:31:11.266822 sabledocs-0.4.170/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2242 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2582 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/templates/_default/search.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 17:31:11.266822 sabledocs-0.4.170/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   257784 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2023-06-08 17:30:58.000000 sabledocs-0.4.170/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 17:31:11.266822 sabledocs-0.4.170/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2023-06-08 17:31:11.000000 sabledocs-0.4.170/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-08 17:31:11.000000 sabledocs-0.4.170/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 17:31:11.000000 sabledocs-0.4.170/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-08 17:31:11.000000 sabledocs-0.4.170/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-08 17:31:11.000000 sabledocs-0.4.170/src/sabledocs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-08 17:31:11.000000 sabledocs-0.4.170/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.387031 sabledocs-0.4.182.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4805 2023-06-23 18:58:22.387031 sabledocs-0.4.182.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4260 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-06-23 18:58:22.391031 sabledocs-0.4.182.dev0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.383031 sabledocs-0.4.182.dev0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.383031 sabledocs-0.4.182.dev0/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3346 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/lunr_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13645 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.383031 sabledocs-0.4.182.dev0/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.387031 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5412 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/search.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.387031 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   260942 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-06-23 18:58:08.000000 sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 18:58:22.387031 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4805 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-23 18:58:22.000000 sabledocs-0.4.182.dev0/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.4.170/LICENSE` & `sabledocs-0.4.182.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.170/PKG-INFO` & `sabledocs-0.4.182.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.4.170
+Version: 0.4.182.dev0
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
 
-### Build the documentation
+### Build the documetation
 
 Install the `sabledocs` package. It requires [Python](https://www.python.org/downloads/) (version 3.11 or higher) to be installed.
 
 ```
 pip install sabledocs
 ```
```

### Comparing `sabledocs-0.4.170/README.md` & `sabledocs-0.4.182.dev0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 protoc *.proto -o descriptor.pb --include_source_info
 ```
 
 *(It's important to use the `--include_source_info` flag, otherwise the comments will not be included in the generated documentation.)*
 
 The generated `descriptor.pb` file will be the input needed to build the documentation site.
 
-### Build the documentation
+### Build the documetation
 
 Install the `sabledocs` package. It requires [Python](https://www.python.org/downloads/) (version 3.11 or higher) to be installed.
 
 ```
 pip install sabledocs
 ```
```

### Comparing `sabledocs-0.4.170/pyproject.toml` & `sabledocs-0.4.182.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.170/src/sabledocs/__main__.py` & `sabledocs-0.4.182.dev0/src/sabledocs/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     package_template = jinja_env.get_template("package.html")
 
     if not os.path.exists(sable_config.output_dir):
         os.makedirs(sable_config.output_dir)
 
     # NOTE: When the output files are generated, the encode('utf-8') option has to be used, otherwise Unicode characters like © can end up garbled.
     for package in sable_context.packages:
-        with open(os.path.join(sable_config.output_dir, f'{package.name if package.name else "__default"}.html'), 'wb') as fh:
+        with open(os.path.join(sable_config.output_dir, f'{package.name}.html'), 'wb') as fh:
             output = package_template.render(
                 sable_config=sable_config,
                 package=package,
                 packages=sable_context.packages,
                 all_messages=sable_context.all_messages,
                 all_enums=sable_context.all_enums).encode('utf-8')
```

### Comparing `sabledocs-0.4.170/src/sabledocs/lunr_search.py` & `sabledocs-0.4.182.dev0/src/sabledocs/lunr_search.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.170/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.4.182.dev0/src/sabledocs/proto_descriptor_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         ev.description_html = markdown.markdown(ev.description)
         ev.line_number = ctx.GetLineNumber()
 
         return ev
 
     e = Enum()
     e.name = enum.name
-    e.full_name = f"{ctx.package.name}.{nested_type_chain}{enum.name}".lstrip(".")
+    e.full_name = f"{ctx.package.name}.{nested_type_chain}{enum.name}"
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
-    m.full_name = f"{ctx.package.name}.{nested_type_chain}{message.name}".lstrip(".")
+    m.full_name = f"{ctx.package.name}.{nested_type_chain}{message.name}"
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
-    s.full_name = f"{ctx.package.name}.{service.name}".lstrip(".")
+    s.full_name = f"{ctx.package.name}.{service.name}"
     s.description = ctx.GetComments()
     s.description_html = markdown.markdown(s.description)
     s.source_file_path = ctx.source_file_path
     s.line_number = ctx.GetLineNumber()
     s.repository_url = build_source_code_url(
         ctx.config.repository_url,
         ctx.config.repository_type,
@@ -218,22 +218,14 @@
 def parse_services(services: list[ServiceDescriptorProto], ctx: ParseContext):
     for (i, service) in enumerate(services):
         ctx.package.services.append(parse_service(service, ctx.ExtendPath(i)))
 
     ctx.package.services.sort(key=lambda s: s.name)
 
 
-def extract_package_name_from_full_name(full_type_name: str):
-    last_dot = full_type_name.rfind(".")
-    if last_dot == -1:
-        return ""
-    else:
-        return full_type_name[:last_dot]
-
-
 def add_package_references(messages: list[Message], services: list[Service], packages):
     for m in messages:
         package = next(filter(lambda p: m.full_name.startswith(p.name), packages), None)
         if package is not None:
             m.package = package
 
         for mf in m.fields:
@@ -246,19 +238,19 @@
 
             package = next(filter(lambda p: mf.full_type.startswith(p.name), packages), None)
             if package is not None:
                 mf.package = package
 
     for s in services:
         for sm in s.methods:
-            requestPackage = next(filter(lambda p: extract_package_name_from_full_name(sm.request.full_type) == p.name, packages), None)
+            requestPackage = next(filter(lambda p: sm.request.full_type.startswith(p.name), packages), None)
             if requestPackage is not None:
                 sm.request.package = requestPackage
 
-            responsePackage = next(filter(lambda p: extract_package_name_from_full_name(sm.response.full_type) == p.name, packages), None)
+            responsePackage = next(filter(lambda p: sm.response.full_type.startswith(p.name), packages), None)
             if responsePackage is not None:
                 sm.response.package = responsePackage
 
 
 def build_location_map(source_code_info):
     def build_key(path):
         return '.'.join(map(lambda i: str(i), path))
```

### Comparing `sabledocs-0.4.170/src/sabledocs/proto_model.py` & `sabledocs-0.4.182.dev0/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.170/src/sabledocs/sable_config.py` & `sabledocs-0.4.182.dev0/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.170/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.170/src/sabledocs/templates/_default/index.html` & `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -9,19 +9,15 @@
   <h3 id="packages" class="title is-3">
     Packages
   </h3>
   <div class="block">This site contains the documentation for the following Protobuf packages.</div>
   <div class="block">
   {% for p in packages %}
     <h5 class="title is-5">
-      {% if p.name %}
-        <a href="{{ p.name }}.html">{{ p.name }}</a>
-      {% else %}
-        <a href="__default.html">(Default package)</a>
-      {% endif %}
+      <a href="{{ p.name }}.html">{{ p.name }}</a>
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

 * *File "/tmp/diffoscope_03vcyyng_/tmpkpl9shrg_TarContainer/0/19.html", line 23, column 6: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_03vcyyng_/tmpkpl9shrg_TarContainer/0/19.html", line 23, column 6: Levels of opening and closing headings don't match*

```diff
@@ -1,12 +1,12 @@
 {% extends "base.html" %} {% block content %} {% if main_page_content %}
 â_Packages
 {{ main_page_content | safe }}
 {% endif %}
 **** Packages ****
 This site contains the documentation for the following Protobuf packages.
 {% for p in packages %}
-** {% if p.name %} {{_p.name_}} {% else %} (Default_package) {% endif %} **
+** {{_p.name_}} **
 {% if p.description_html %}
 {{ p.description_html | safe }}
 {% endif %} {% endfor %}
 {% endblock %}
```

### Comparing `sabledocs-0.4.170/src/sabledocs/templates/_default/message.html` & `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.170/src/sabledocs/templates/_default/package.html` & `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/package.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 {% extends "base.html" %}
 {% block content %}
   <p class="mb-2">
     <a style="font-size: 0.9em" href="index.html">← Back to packages</a>
   </p>
   <h4 class="title is-4">
-    {% if package.name %}
     Package <code>{{ package.name }}</code>
-    {% else %}
-    Default package
-    {% endif %}
   </h4>
 
   <div class="block">
     {% for service in package.services %}
     <p>
       <a href="#service-{{ service.full_name }}">
         <span class="tag" style="min-width: 6em">Service</span>
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
 {% extends "base.html" %} {% block content %}
 â_Back_to_packages
-*** {% if package.name %} Package {{ package.name }} {% else %} Default package
-{% endif %} ***
+*** Package {{ package.name }} ***
 {% for service in package.services %}
 Service_{{_service.name_}}
 {% endfor %} {% for message in package.messages %} {% if not
 message.is_map_entry %}
 Message_{{_message.name_}}
 {% endif %} {% endfor %} {% for enum in package.enums %}
 Enum_{{_enum.name_}}
```

### Comparing `sabledocs-0.4.170/src/sabledocs/templates/_default/search.html` & `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/search.html`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 searchResults.innerHTML = resultList
             } else {
                 searchResults.innerHTML = '<p>No search results.</p>';
             }
         }
     }
 
-    window.onload = displaySearchResults;
+    window.addEventListener("load", displaySearchResults);
 </script>
 
   <div>
     <p class="block">
       Enter a query to search this documentation.
     </p>
     <div class="field is-horizontal">
```

### Comparing `sabledocs-0.4.170/src/sabledocs/templates/_default/service.html` & `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/service.html`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 <div class="block content">
   <p>{{ service.description_html | safe }}</p>
 </div>
 
 {% for method in service.methods %}
 <div class="box">
-  <h6 class="title is-6">rpc <code>{{ method.name }} ({{ common.type_name(method.request) }}) -> {{ common.type_name(method.response) }}</code></h6>
+  <h6 class="title is-6">rpc <code>{{ method.name }} ({{ common.type_name(method.request) | trim }}) -> {{ common.type_name(method.response) }}</code></h6>
+
   {% if method.description_html %}
   <div class="block">
     <p>{{ method.description_html | safe }}</p>
   </div>
   {% endif %}
 </div>
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% import "type_name.html" as common %}
 ** service_{{_service.name_}} {% if service.repository_url %} {
 {_service.source_file_path_}} {% endif %} **
 {{ service.description_html | safe }}
 {% for method in service.methods %}
-* rpc {{ method.name }} ({{ common.type_name(method.request) }}) -> {
+* rpc {{ method.name }} ({{ common.type_name(method.request) | trim }}) -> {
 { common.type_name(method.response) }} *
 {% if method.description_html %}
 {{ method.description_html | safe }}
 {% endif %}
 {% endfor %}
```

### Comparing `sabledocs-0.4.170/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 /*! bulma.io v0.9.4 | MIT License | github.com/jgthms/bulma */
 /* Bulma Utilities */
+@import "https://unpkg.com/open-props/easings.min.css";
 .button, .input, .textarea, .select select, .file-cta,
 .file-name, .pagination-previous,
 .pagination-next,
 .pagination-link,
 .pagination-ellipsis {
   -moz-appearance: none;
   -webkit-appearance: none;
@@ -667,75 +668,75 @@
       .button.is-light.is-inverted.is-outlined[disabled],
       fieldset[disabled] .button.is-light.is-inverted.is-outlined {
         background-color: transparent;
         border-color: rgba(0, 0, 0, 0.7);
         box-shadow: none;
         color: rgba(0, 0, 0, 0.7); }
   .button.is-dark {
-    background-color: #363636;
+    background-color: #181818;
     border-color: transparent;
     color: #fff; }
     .button.is-dark:hover, .button.is-dark.is-hovered {
-      background-color: #2f2f2f;
+      background-color: #121212;
       border-color: transparent;
       color: #fff; }
     .button.is-dark:focus, .button.is-dark.is-focused {
       border-color: transparent;
       color: #fff; }
       .button.is-dark:focus:not(:active), .button.is-dark.is-focused:not(:active) {
-        box-shadow: 0 0 0 0.125em rgba(54, 54, 54, 0.25); }
+        box-shadow: 0 0 0 0.125em rgba(24, 24, 24, 0.25); }
     .button.is-dark:active, .button.is-dark.is-active {
-      background-color: #292929;
+      background-color: #0b0b0b;
       border-color: transparent;
       color: #fff; }
     .button.is-dark[disabled],
     fieldset[disabled] .button.is-dark {
-      background-color: #363636;
-      border-color: #363636;
+      background-color: #181818;
+      border-color: #181818;
       box-shadow: none; }
     .button.is-dark.is-inverted {
       background-color: #fff;
-      color: #363636; }
+      color: #181818; }
       .button.is-dark.is-inverted:hover, .button.is-dark.is-inverted.is-hovered {
         background-color: #f2f2f2; }
       .button.is-dark.is-inverted[disabled],
       fieldset[disabled] .button.is-dark.is-inverted {
         background-color: #fff;
         border-color: transparent;
         box-shadow: none;
-        color: #363636; }
+        color: #181818; }
     .button.is-dark.is-loading::after {
       border-color: transparent transparent #fff #fff !important; }
     .button.is-dark.is-outlined {
       background-color: transparent;
-      border-color: #363636;
-      color: #363636; }
+      border-color: #181818;
+      color: #181818; }
       .button.is-dark.is-outlined:hover, .button.is-dark.is-outlined.is-hovered, .button.is-dark.is-outlined:focus, .button.is-dark.is-outlined.is-focused {
-        background-color: #363636;
-        border-color: #363636;
+        background-color: #181818;
+        border-color: #181818;
         color: #fff; }
       .button.is-dark.is-outlined.is-loading::after {
-        border-color: transparent transparent #363636 #363636 !important; }
+        border-color: transparent transparent #181818 #181818 !important; }
       .button.is-dark.is-outlined.is-loading:hover::after, .button.is-dark.is-outlined.is-loading.is-hovered::after, .button.is-dark.is-outlined.is-loading:focus::after, .button.is-dark.is-outlined.is-loading.is-focused::after {
         border-color: transparent transparent #fff #fff !important; }
       .button.is-dark.is-outlined[disabled],
       fieldset[disabled] .button.is-dark.is-outlined {
         background-color: transparent;
-        border-color: #363636;
+        border-color: #181818;
         box-shadow: none;
-        color: #363636; }
+        color: #181818; }
     .button.is-dark.is-inverted.is-outlined {
       background-color: transparent;
       border-color: #fff;
       color: #fff; }
       .button.is-dark.is-inverted.is-outlined:hover, .button.is-dark.is-inverted.is-outlined.is-hovered, .button.is-dark.is-inverted.is-outlined:focus, .button.is-dark.is-inverted.is-outlined.is-focused {
         background-color: #fff;
-        color: #363636; }
+        color: #181818; }
       .button.is-dark.is-inverted.is-outlined.is-loading:hover::after, .button.is-dark.is-inverted.is-outlined.is-loading.is-hovered::after, .button.is-dark.is-inverted.is-outlined.is-loading:focus::after, .button.is-dark.is-inverted.is-outlined.is-loading.is-focused::after {
-        border-color: transparent transparent #363636 #363636 !important; }
+        border-color: transparent transparent #181818 #181818 !important; }
       .button.is-dark.is-inverted.is-outlined[disabled],
       fieldset[disabled] .button.is-dark.is-inverted.is-outlined {
         background-color: transparent;
         border-color: #fff;
         box-shadow: none;
         color: #fff; }
   .button.is-primary {
@@ -1641,15 +1642,15 @@
   .notification.is-black {
     background-color: #0a0a0a;
     color: white; }
   .notification.is-light {
     background-color: whitesmoke;
     color: rgba(0, 0, 0, 0.7); }
   .notification.is-dark {
-    background-color: #363636;
+    background-color: #181818;
     color: #fff; }
   .notification.is-primary {
     background-color: #016FB9;
     color: #fff; }
     .notification.is-primary.is-light {
       background-color: #ebf7ff;
       color: #018fee; }
@@ -1724,21 +1725,21 @@
   .progress.is-light::-moz-progress-bar {
     background-color: whitesmoke; }
   .progress.is-light::-ms-fill {
     background-color: whitesmoke; }
   .progress.is-light:indeterminate {
     background-image: linear-gradient(to right, whitesmoke 30%, #ededed 30%); }
   .progress.is-dark::-webkit-progress-value {
-    background-color: #363636; }
+    background-color: #181818; }
   .progress.is-dark::-moz-progress-bar {
-    background-color: #363636; }
+    background-color: #181818; }
   .progress.is-dark::-ms-fill {
-    background-color: #363636; }
+    background-color: #181818; }
   .progress.is-dark:indeterminate {
-    background-image: linear-gradient(to right, #363636 30%, #ededed 30%); }
+    background-image: linear-gradient(to right, #181818 30%, #ededed 30%); }
   .progress.is-primary::-webkit-progress-value {
     background-color: #016FB9; }
   .progress.is-primary::-moz-progress-bar {
     background-color: #016FB9; }
   .progress.is-primary::-ms-fill {
     background-color: #016FB9; }
   .progress.is-primary:indeterminate {
@@ -1834,16 +1835,16 @@
     .table td.is-light,
     .table th.is-light {
       background-color: whitesmoke;
       border-color: whitesmoke;
       color: rgba(0, 0, 0, 0.7); }
     .table td.is-dark,
     .table th.is-dark {
-      background-color: #363636;
-      border-color: #363636;
+      background-color: #181818;
+      border-color: #181818;
       color: #fff; }
     .table td.is-primary,
     .table th.is-primary {
       background-color: #016FB9;
       border-color: #016FB9;
       color: #fff; }
     .table td.is-link,
@@ -2004,15 +2005,15 @@
   .tag:not(body).is-black {
     background-color: #0a0a0a;
     color: white; }
   .tag:not(body).is-light {
     background-color: whitesmoke;
     color: rgba(0, 0, 0, 0.7); }
   .tag:not(body).is-dark {
-    background-color: #363636;
+    background-color: #181818;
     color: #fff; }
   .tag:not(body).is-primary {
     background-color: #016FB9;
     color: #fff; }
     .tag:not(body).is-primary.is-light {
       background-color: #ebf7ff;
       color: #018fee; }
@@ -2248,17 +2249,17 @@
     .is-black.input:focus, .is-black.textarea:focus, .is-black.is-focused.input, .is-black.is-focused.textarea, .is-black.input:active, .is-black.textarea:active, .is-black.is-active.input, .is-black.is-active.textarea {
       box-shadow: 0 0 0 0.125em rgba(10, 10, 10, 0.25); }
   .is-light.input, .is-light.textarea {
     border-color: whitesmoke; }
     .is-light.input:focus, .is-light.textarea:focus, .is-light.is-focused.input, .is-light.is-focused.textarea, .is-light.input:active, .is-light.textarea:active, .is-light.is-active.input, .is-light.is-active.textarea {
       box-shadow: 0 0 0 0.125em rgba(245, 245, 245, 0.25); }
   .is-dark.input, .is-dark.textarea {
-    border-color: #363636; }
+    border-color: #181818; }
     .is-dark.input:focus, .is-dark.textarea:focus, .is-dark.is-focused.input, .is-dark.is-focused.textarea, .is-dark.input:active, .is-dark.textarea:active, .is-dark.is-active.input, .is-dark.is-active.textarea {
-      box-shadow: 0 0 0 0.125em rgba(54, 54, 54, 0.25); }
+      box-shadow: 0 0 0 0.125em rgba(24, 24, 24, 0.25); }
   .is-primary.input, .is-primary.textarea {
     border-color: #016FB9; }
     .is-primary.input:focus, .is-primary.textarea:focus, .is-primary.is-focused.input, .is-primary.is-focused.textarea, .is-primary.input:active, .is-primary.textarea:active, .is-primary.is-active.input, .is-primary.is-active.textarea {
       box-shadow: 0 0 0 0.125em rgba(1, 111, 185, 0.25); }
   .is-link.input, .is-link.textarea {
     border-color: #016FB9; }
     .is-link.input:focus, .is-link.textarea:focus, .is-link.is-focused.input, .is-link.is-focused.textarea, .is-link.input:active, .is-link.textarea:active, .is-link.is-active.input, .is-link.is-active.textarea {
@@ -2394,21 +2395,21 @@
   .select.is-light select {
     border-color: whitesmoke; }
     .select.is-light select:hover, .select.is-light select.is-hovered {
       border-color: #e8e8e8; }
     .select.is-light select:focus, .select.is-light select.is-focused, .select.is-light select:active, .select.is-light select.is-active {
       box-shadow: 0 0 0 0.125em rgba(245, 245, 245, 0.25); }
   .select.is-dark:not(:hover)::after {
-    border-color: #363636; }
+    border-color: #181818; }
   .select.is-dark select {
-    border-color: #363636; }
+    border-color: #181818; }
     .select.is-dark select:hover, .select.is-dark select.is-hovered {
-      border-color: #292929; }
+      border-color: #0b0b0b; }
     .select.is-dark select:focus, .select.is-dark select.is-focused, .select.is-dark select:active, .select.is-dark select.is-active {
-      box-shadow: 0 0 0 0.125em rgba(54, 54, 54, 0.25); }
+      box-shadow: 0 0 0 0.125em rgba(24, 24, 24, 0.25); }
   .select.is-primary:not(:hover)::after {
     border-color: #016FB9; }
   .select.is-primary select {
     border-color: #016FB9; }
     .select.is-primary select:hover, .select.is-primary select.is-hovered {
       border-color: #0160a0; }
     .select.is-primary select:focus, .select.is-primary select.is-focused, .select.is-primary select:active, .select.is-primary select.is-active {
@@ -2530,27 +2531,27 @@
     box-shadow: 0 0 0.5em rgba(245, 245, 245, 0.25);
     color: rgba(0, 0, 0, 0.7); }
   .file.is-light:active .file-cta, .file.is-light.is-active .file-cta {
     background-color: #e8e8e8;
     border-color: transparent;
     color: rgba(0, 0, 0, 0.7); }
   .file.is-dark .file-cta {
-    background-color: #363636;
+    background-color: #181818;
     border-color: transparent;
     color: #fff; }
   .file.is-dark:hover .file-cta, .file.is-dark.is-hovered .file-cta {
-    background-color: #2f2f2f;
+    background-color: #121212;
     border-color: transparent;
     color: #fff; }
   .file.is-dark:focus .file-cta, .file.is-dark.is-focused .file-cta {
     border-color: transparent;
-    box-shadow: 0 0 0.5em rgba(54, 54, 54, 0.25);
+    box-shadow: 0 0 0.5em rgba(24, 24, 24, 0.25);
     color: #fff; }
   .file.is-dark:active .file-cta, .file.is-dark.is-active .file-cta {
-    background-color: #292929;
+    background-color: #0b0b0b;
     border-color: transparent;
     color: #fff; }
   .file.is-primary .file-cta {
     background-color: #016FB9;
     border-color: transparent;
     color: #fff; }
   .file.is-primary:hover .file-cta, .file.is-primary.is-hovered .file-cta {
@@ -2788,15 +2789,15 @@
   .help.is-white {
     color: white; }
   .help.is-black {
     color: #0a0a0a; }
   .help.is-light {
     color: whitesmoke; }
   .help.is-dark {
-    color: #363636; }
+    color: #181818; }
   .help.is-primary {
     color: #016FB9; }
   .help.is-link {
     color: #016FB9; }
   .help.is-info {
     color: #3e8ed0; }
   .help.is-success {
@@ -3377,18 +3378,18 @@
       background-color: whitesmoke;
       color: rgba(0, 0, 0, 0.7); }
     .message.is-light .message-body {
       border-color: whitesmoke; }
   .message.is-dark {
     background-color: #fafafa; }
     .message.is-dark .message-header {
-      background-color: #363636;
+      background-color: #181818;
       color: #fff; }
     .message.is-dark .message-body {
-      border-color: #363636; }
+      border-color: #181818; }
   .message.is-primary {
     background-color: #ebf7ff; }
     .message.is-primary .message-header {
       background-color: #016FB9;
       color: #fff; }
     .message.is-primary .message-body {
       border-color: #016FB9;
@@ -3684,24 +3685,24 @@
       .navbar.is-light .navbar-item.has-dropdown.is-active .navbar-link {
         background-color: #e8e8e8;
         color: rgba(0, 0, 0, 0.7); }
       .navbar.is-light .navbar-dropdown a.navbar-item.is-active {
         background-color: whitesmoke;
         color: rgba(0, 0, 0, 0.7); } }
   .navbar.is-dark {
-    background-color: #363636;
+    background-color: #181818;
     color: #fff; }
     .navbar.is-dark .navbar-brand > .navbar-item,
     .navbar.is-dark .navbar-brand .navbar-link {
       color: #fff; }
     .navbar.is-dark .navbar-brand > a.navbar-item:focus, .navbar.is-dark .navbar-brand > a.navbar-item:hover, .navbar.is-dark .navbar-brand > a.navbar-item.is-active,
     .navbar.is-dark .navbar-brand .navbar-link:focus,
     .navbar.is-dark .navbar-brand .navbar-link:hover,
     .navbar.is-dark .navbar-brand .navbar-link.is-active {
-      background-color: #292929;
+      background-color: #0b0b0b;
       color: #fff; }
     .navbar.is-dark .navbar-brand .navbar-link::after {
       border-color: #fff; }
     .navbar.is-dark .navbar-burger {
       color: #fff; }
     @media screen and (min-width: 1024px) {
       .navbar.is-dark .navbar-start > .navbar-item,
@@ -3715,26 +3716,26 @@
       .navbar.is-dark .navbar-start .navbar-link.is-active,
       .navbar.is-dark .navbar-end > a.navbar-item:focus,
       .navbar.is-dark .navbar-end > a.navbar-item:hover,
       .navbar.is-dark .navbar-end > a.navbar-item.is-active,
       .navbar.is-dark .navbar-end .navbar-link:focus,
       .navbar.is-dark .navbar-end .navbar-link:hover,
       .navbar.is-dark .navbar-end .navbar-link.is-active {
-        background-color: #292929;
+        background-color: #0b0b0b;
         color: #fff; }
       .navbar.is-dark .navbar-start .navbar-link::after,
       .navbar.is-dark .navbar-end .navbar-link::after {
         border-color: #fff; }
       .navbar.is-dark .navbar-item.has-dropdown:focus .navbar-link,
       .navbar.is-dark .navbar-item.has-dropdown:hover .navbar-link,
       .navbar.is-dark .navbar-item.has-dropdown.is-active .navbar-link {
-        background-color: #292929;
+        background-color: #0b0b0b;
         color: #fff; }
       .navbar.is-dark .navbar-dropdown a.navbar-item.is-active {
-        background-color: #363636;
+        background-color: #181818;
         color: #fff; } }
   .navbar.is-primary {
     background-color: #016FB9;
     color: #fff; }
     .navbar.is-primary .navbar-brand > .navbar-item,
     .navbar.is-primary .navbar-brand .navbar-link {
       color: #fff; }
@@ -4496,20 +4497,20 @@
     background-color: whitesmoke;
     color: rgba(0, 0, 0, 0.7); }
   .panel.is-light .panel-tabs a.is-active {
     border-bottom-color: whitesmoke; }
   .panel.is-light .panel-block.is-active .panel-icon {
     color: whitesmoke; }
   .panel.is-dark .panel-heading {
-    background-color: #363636;
+    background-color: #181818;
     color: #fff; }
   .panel.is-dark .panel-tabs a.is-active {
-    border-bottom-color: #363636; }
+    border-bottom-color: #181818; }
   .panel.is-dark .panel-block.is-active .panel-icon {
-    color: #363636; }
+    color: #181818; }
   .panel.is-primary .panel-heading {
     background-color: #016FB9;
     color: #fff; }
   .panel.is-primary .panel-tabs a.is-active {
     border-bottom-color: #016FB9; }
   .panel.is-primary .panel-block.is-active .panel-icon {
     color: #016FB9; }
@@ -5949,21 +5950,21 @@
 a.has-text-light:hover, a.has-text-light:focus {
   color: #dbdbdb !important; }
 
 .has-background-light {
   background-color: whitesmoke !important; }
 
 .has-text-dark {
-  color: #363636 !important; }
+  color: #181818 !important; }
 
 a.has-text-dark:hover, a.has-text-dark:focus {
-  color: #1c1c1c !important; }
+  color: black !important; }
 
 .has-background-dark {
-  background-color: #363636 !important; }
+  background-color: #181818 !important; }
 
 .has-text-primary {
   color: #016FB9 !important; }
 
 a.has-text-primary:hover, a.has-text-primary:focus {
   color: #015186 !important; }
 
@@ -7483,58 +7484,58 @@
       color: whitesmoke; }
     .hero.is-light.is-bold {
       background-image: linear-gradient(141deg, #dfd8d9 0%, whitesmoke 71%, white 100%); }
       @media screen and (max-width: 768px) {
         .hero.is-light.is-bold .navbar-menu {
           background-image: linear-gradient(141deg, #dfd8d9 0%, whitesmoke 71%, white 100%); } }
   .hero.is-dark {
-    background-color: #363636;
+    background-color: #181818;
     color: #fff; }
     .hero.is-dark a:not(.button):not(.dropdown-item):not(.tag):not(.pagination-link.is-current),
     .hero.is-dark strong {
       color: inherit; }
     .hero.is-dark .title {
       color: #fff; }
     .hero.is-dark .subtitle {
       color: rgba(255, 255, 255, 0.9); }
       .hero.is-dark .subtitle a:not(.button),
       .hero.is-dark .subtitle strong {
         color: #fff; }
     @media screen and (max-width: 1023px) {
       .hero.is-dark .navbar-menu {
-        background-color: #363636; } }
+        background-color: #181818; } }
     .hero.is-dark .navbar-item,
     .hero.is-dark .navbar-link {
       color: rgba(255, 255, 255, 0.7); }
     .hero.is-dark a.navbar-item:hover, .hero.is-dark a.navbar-item.is-active,
     .hero.is-dark .navbar-link:hover,
     .hero.is-dark .navbar-link.is-active {
-      background-color: #292929;
+      background-color: #0b0b0b;
       color: #fff; }
     .hero.is-dark .tabs a {
       color: #fff;
       opacity: 0.9; }
       .hero.is-dark .tabs a:hover {
         opacity: 1; }
     .hero.is-dark .tabs li.is-active a {
-      color: #363636 !important;
+      color: #181818 !important;
       opacity: 1; }
     .hero.is-dark .tabs.is-boxed a, .hero.is-dark .tabs.is-toggle a {
       color: #fff; }
       .hero.is-dark .tabs.is-boxed a:hover, .hero.is-dark .tabs.is-toggle a:hover {
         background-color: rgba(10, 10, 10, 0.1); }
     .hero.is-dark .tabs.is-boxed li.is-active a, .hero.is-dark .tabs.is-boxed li.is-active a:hover, .hero.is-dark .tabs.is-toggle li.is-active a, .hero.is-dark .tabs.is-toggle li.is-active a:hover {
       background-color: #fff;
       border-color: #fff;
-      color: #363636; }
+      color: #181818; }
     .hero.is-dark.is-bold {
-      background-image: linear-gradient(141deg, #1f191a 0%, #363636 71%, #46403f 100%); }
+      background-image: linear-gradient(141deg, black 0%, #181818 71%, #272423 100%); }
       @media screen and (max-width: 768px) {
         .hero.is-dark.is-bold .navbar-menu {
-          background-image: linear-gradient(141deg, #1f191a 0%, #363636 71%, #46403f 100%); } }
+          background-image: linear-gradient(141deg, black 0%, #181818 71%, #272423 100%); } }
   .hero.is-primary {
     background-color: #016FB9;
     color: #fff; }
     .hero.is-primary a:not(.button):not(.dropdown-item):not(.tag):not(.pagination-link.is-current),
     .hero.is-primary strong {
       color: inherit; }
     .hero.is-primary .title {
@@ -7901,7 +7902,140 @@
 .bottom-border {
   border-width: 0 0 0.06em 0;
   border-style: solid;
   border-color: #DDDDDD; }
 
 .navbar-search-query-input {
   width: 13em; }
+
+body {
+  min-height: 100vh; }
+
+body .subtitle,
+body .title {
+  color: #181818; }
+
+body.dark,
+body.dark .box,
+body.dark table {
+  background-color: #181818;
+  color: whitesmoke; }
+
+body.dark th {
+  color: whitesmoke; }
+
+body.dark .table.is-hoverable tbody tr:not(.is-selected):hover {
+  background-color: #252525; }
+
+body.dark a:hover {
+  color: whitesmoke; }
+
+body.dark .box,
+body.dark .type-heading,
+body.dark td,
+body.dark th {
+  border-color: #444444; }
+
+body.dark .subtitle,
+body.dark .title {
+  color: whitesmoke; }
+
+body.dark footer {
+  background-color: #101010; }
+
+body.dark .bottom-border {
+  border-color: #444444; }
+
+body.dark hr {
+  background-color: #444444; }
+
+body.dark .input, .textarea, .select select {
+  background-color: #363636;
+  border-color: #565656;
+  border-radius: 4px;
+  color: white; }
+
+body.dark code {
+  background: #2A2A2A;
+  color: #569cd6; }
+
+body.dark code a {
+  color: #569cd6; }
+
+body.dark .tag {
+  background: #2A2A2A;
+  color: whitesmoke; }
+
+.theme-toggle {
+  --size: 2rem;
+  --icon-fill: #016FB9;
+  --icon-fill-hover: #363636;
+  background: none;
+  border: none;
+  padding: 0;
+  inline-size: var(--size);
+  block-size: var(--size);
+  aspect-ratio: 1;
+  border-radius: 50%;
+  cursor: pointer;
+  touch-action: manipulation;
+  -webkit-tap-highlight-color: transparent;
+  outline-offset: 5px; }
+
+.theme-toggle > svg {
+  inline-size: 100%;
+  block-size: 100%;
+  stroke-linecap: round; }
+
+[data-theme=dark] .theme-toggle {
+  --icon-fill-hover: whitesmoke; }
+
+.sun-and-moon > :is(.moon, .sun, .sun-beams) {
+  transform-origin: center; }
+
+.sun-and-moon > :is(.moon, .sun) {
+  fill: var(--icon-fill); }
+
+.theme-toggle:is(:hover, :focus-visible) > .sun-and-moon > :is(.moon, .sun) {
+  fill: var(--icon-fill-hover); }
+
+.sun-and-moon > .sun-beams {
+  stroke: var(--icon-fill);
+  stroke-width: 2px; }
+
+.theme-toggle:is(:hover, :focus-visible) .sun-and-moon > .sun-beams {
+  stroke: var(--icon-fill-hover); }
+
+[data-theme="dark"] .sun-and-moon > .sun {
+  transform: scale(1.75); }
+
+[data-theme="dark"] .sun-and-moon > .sun-beams {
+  opacity: 0; }
+
+[data-theme="dark"] .sun-and-moon > .moon > circle {
+  transform: translateX(-7px); }
+
+@supports (cx: 1) {
+  [data-theme="dark"] .sun-and-moon > .moon > circle {
+    cx: 17;
+    transform: translateX(0); } }
+
+@media (prefers-reduced-motion: no-preference) {
+  .sun-and-moon > .sun {
+    transition: transform 0.5s var(--ease-elastic-3); }
+  .sun-and-moon > .sun-beams {
+    transition: transform 0.5s var(--ease-elastic-4), opacity 0.5s var(--ease-3); }
+  .sun-and-moon .moon > circle {
+    transition: transform 0.25s var(--ease-out-5); }
+  @supports (cx: 1) {
+    .sun-and-moon .moon > circle {
+      transition: cx 0.25s var(--ease-out-5); } }
+  [data-theme="dark"] .sun-and-moon > .sun {
+    transition-timing-function: var(--ease-3);
+    transition-duration: .25s;
+    transform: scale(1.75); }
+  [data-theme="dark"] .sun-and-moon > .sun-beams {
+    transition-duration: .15s;
+    transform: rotateZ(-25deg); }
+  [data-theme="dark"] .sun-and-moon > .moon > circle {
+    transition-duration: .5s;
+    transition-delay: .25s; } }
```

### Comparing `sabledocs-0.4.170/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.4.182.dev0/src/sabledocs/templates/_default/type_name.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-{% macro type_name(message_field) -%}
-  {% if message_field.package and message_field.type_kind != "UNKNOWN" %}
-    {% if message_field.type_kind == "MESSAGE" %}
-      <a href="{{ message_field.package.name if message_field.package.name else "__default" }}.html#message-{{ message_field.full_type }}">
-    {% else %}
-      <a href="{{ message_field.package.name if message_field.package.name else "__default" }}.html#enum-{{ message_field.full_type }}">
-    {% endif %}
-      <span title="{{ message_field.full_type }}">{{ message_field.full_type }}</span>
-    </a>
-  {% else %}
+## The %- and -% syntax is used everywhere to trim all the whitespace, to make sure no extra unwanted spaces are around the type name, for example if it's displayed between parens.
+{%- macro type_name(message_field) -%}
+  {%- if message_field.package and message_field.type_kind != "UNKNOWN" -%}
+    {%- if message_field.type_kind == "MESSAGE" -%}
+      <a href="{{ message_field.package.name }}.html#message-{{ message_field.full_type }}">
+    {%- else -%}
+      <a href="{{ message_field.package.name }}.html#enum-{{ message_field.full_type }}">
+    {%- endif -%}
+      <span title="{{ message_field.full_type }}">{{ message_field.full_type }}</span></a>
+  {%- else -%}
   <span>{{ message_field.full_type }}</span>
-  {% endif %}
-{%- endmacro %}
+  {%- endif -%}
+{%- endmacro -%}
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-{% macro type_name(message_field) -%} {% if message_field.package and
-message_field.type_kind != "UNKNOWN" %} {% if message_field.type_kind ==
-"MESSAGE" %}
- }}.html#message-{{ message_field.full_type }}"> {% else %}
- }}.html#enum-{{ message_field.full_type }}"> {% endif %} {
-{ message_field.full_type }}
- {% else %} {{ message_field.full_type }} {% endif %} {%- endmacro %}
+## The %- and -% syntax is used everywhere to trim all the whitespace, to make
+sure no extra unwanted spaces are around the type name, for example if it's
+displayed between parens. {%- macro type_name(message_field) -%} {%- if
+message_field.package and message_field.type_kind != "UNKNOWN" -%} {%- if
+message_field.type_kind == "MESSAGE" -%} {%-_else_-%}_{%-_endif_-%}_{
+{_message_field.full_type_}}_{%-_else_-%}_{{_message_field.full_type_}}_{%-
+endif_-%}_{%-_endmacro_-%}_
```

### Comparing `sabledocs-0.4.170/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.4.182.dev0/src/sabledocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.4.170
+Version: 0.4.182.dev0
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
 
-### Build the documentation
+### Build the documetation
 
 Install the `sabledocs` package. It requires [Python](https://www.python.org/downloads/) (version 3.11 or higher) to be installed.
 
 ```
 pip install sabledocs
 ```
```

### Comparing `sabledocs-0.4.170/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.4.182.dev0/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

