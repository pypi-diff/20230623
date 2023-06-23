# Comparing `tmp/meilisearch_tui-0.7.4.tar.gz` & `tmp/meilisearch_tui-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_tui-0.7.4.tar", max compression
+gzip compressed data, was "meilisearch_tui-0.8.0.tar", max compression
```

## Comparing `meilisearch_tui-0.7.4.tar` & `meilisearch_tui-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-06-20 01:05:08.575002 meilisearch_tui-0.7.4/LICENSE
--rw-r--r--   0        0        0     2045 2023-06-20 01:05:08.575002 meilisearch_tui-0.7.4/README.md
--rw-r--r--   0        0        0        0 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/__init__.py
--rw-r--r--   0        0        0      115 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/__main__.py
--rw-r--r--   0        0        0      608 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/client.py
--rw-r--r--   0        0        0     3226 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/config.py
--rw-r--r--   0        0        0       86 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/errors.py
--rw-r--r--   0        0        0     2780 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/main.py
--rw-r--r--   0        0        0     1908 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/meilisearch.css
--rw-r--r--   0        0        0        0 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/py.typed
--rw-r--r--   0        0        0        0 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/screens/__init__.py
--rw-r--r--   0        0        0     4518 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/screens/configuration.py
--rw-r--r--   0        0        0    28829 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/screens/indexes.py
--rw-r--r--   0        0        0     6228 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/screens/search.py
--rw-r--r--   0        0        0      897 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/utils.py
--rw-r--r--   0        0        0        0 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/widgets/__init__.py
--rw-r--r--   0        0        0      844 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/widgets/index.py
--rw-r--r--   0        0        0     1543 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/widgets/index_sidebar.py
--rw-r--r--   0        0        0     1730 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/widgets/input.py
--rw-r--r--   0        0        0      709 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/meilisearch_tui/widgets/messages.py
--rw-r--r--   0        0        0     2099 2023-06-20 01:05:08.579002 meilisearch_tui-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 meilisearch_tui-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-23 13:58:16.256510 meilisearch_tui-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2045 2023-06-23 13:58:16.256510 meilisearch_tui-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/__main__.py
+-rw-r--r--   0        0        0      608 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/client.py
+-rw-r--r--   0        0        0     3226 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/config.py
+-rw-r--r--   0        0        0       86 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/errors.py
+-rw-r--r--   0        0        0     2780 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/main.py
+-rw-r--r--   0        0        0     1908 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/meilisearch.css
+-rw-r--r--   0        0        0        0 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/py.typed
+-rw-r--r--   0        0        0        0 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/screens/__init__.py
+-rw-r--r--   0        0        0     4518 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/screens/configuration.py
+-rw-r--r--   0        0        0    28829 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/screens/indexes.py
+-rw-r--r--   0        0        0     6974 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/screens/search.py
+-rw-r--r--   0        0        0      897 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/utils.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/widgets/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/widgets/index.py
+-rw-r--r--   0        0        0     1543 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/widgets/index_sidebar.py
+-rw-r--r--   0        0        0     1730 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/widgets/input.py
+-rw-r--r--   0        0        0      709 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/widgets/messages.py
+-rw-r--r--   0        0        0     2099 2023-06-23 13:58:16.264511 meilisearch_tui-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 meilisearch_tui-0.8.0/PKG-INFO
```

### Comparing `meilisearch_tui-0.7.4/LICENSE` & `meilisearch_tui-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/README.md` & `meilisearch_tui-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/client.py` & `meilisearch_tui-0.8.0/meilisearch_tui/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/config.py` & `meilisearch_tui-0.8.0/meilisearch_tui/config.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/main.py` & `meilisearch_tui-0.8.0/meilisearch_tui/main.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/meilisearch.css` & `meilisearch_tui-0.8.0/meilisearch_tui/meilisearch.css`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/screens/configuration.py` & `meilisearch_tui-0.8.0/meilisearch_tui/screens/configuration.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/screens/indexes.py` & `meilisearch_tui-0.8.0/meilisearch_tui/screens/indexes.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/screens/search.py` & `meilisearch_tui-0.8.0/meilisearch_tui/screens/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
     def compose(self) -> ComposeResult:
         yield ErrorMessage("", classes="message-centered", id="generic-error")
         yield IndexSidebar(classes="sidebar")
         with VerticalScroll(id="body"):
             yield Static("No index selected", id="index-name", classes="bottom-spacer")
             yield Input(placeholder="Search", classes="bottom-spacer", id="search")
+            with Center():
+                yield Button(label="Clear Search Box", classes="bottom-spacer", id="clear-search")
             with VerticalScroll(id="results-container"):
                 yield Markdown(id="results")
             with Center():
                 yield Button(label="Load More", classes="bottom-spacer", id="load-more-button")
         yield Footer()
 
     @cached_property
@@ -51,14 +53,18 @@
         return self.query_one("#index-name", Static)
 
     @cached_property
     def search_input(self) -> Input:
         return self.query_one("#search", Input)
 
     @cached_property
+    def clear_search(self) -> Button:
+        return self.query_one("#clear-search", Button)
+
+    @cached_property
     def results_container(self) -> VerticalScroll:
         return self.query_one("#results-container", VerticalScroll)
 
     @cached_property
     def results(self) -> Markdown:
         return self.query_one("#results", Markdown)
 
@@ -113,28 +119,39 @@
     async def on_button_pressed(self, event: Button.Pressed) -> None:
         button_id = event.button.id
 
         if button_id == "load-more-button":
             self.limit += 20
             await self.search(self.search_input.value)
 
+        if button_id == "clear-search":
+            self.search_input.value = ""
+            self.search_input.focus()
+
     @cached(ttl=10)
     async def search(self, search: str) -> None:
         if not self.selected_index and search == self.search_input.value:
             self.results.update("Error: No index provided")
             return
 
         if not self.selected_index:
             self.results.update("No index selected")
             return
 
         async with get_client() as client:
             index = client.index(self.selected_index)
             try:
-                results = await index.search(self.search_input.value, limit=self.limit)
+                results = await index.search(
+                    self.search_input.value,
+                    limit=self.limit,
+                    attributes_to_highlight=["*"],
+                    highlight_pre_tag="***",
+                    highlight_post_tag="***",
+                )
+
             except Exception as e:
                 if search == self.search_input.value:
                     self.results.update(f"Error: {e}")
                 return
 
         # Make sure a new search hasn't started. This prevents race conditions with displaying
         # the search results by only updating the display if the search is still relavent.
@@ -152,13 +169,17 @@
 
         lines.append(
             f"## Hits: ~{results.estimated_total_hits} | Search time: {results.processing_time_ms} ms"
         )
 
         if results.hits:
             for hit in results.hits:
-                for k, v in hit.items():
-                    lines.append(f"{k}: {v}\n")
+                if hit.get("_formatted"):
+                    for k, v in hit["_formatted"].items():
+                        lines.append(f"{k}: {v}\n")
+                else:
+                    for k, v in hit.items():
+                        lines.append(f"{k}: {v}\n")
                 lines.append("-------------------------------")
             return "\n".join(lines)
 
         return "No results found"
```

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/utils.py` & `meilisearch_tui-0.8.0/meilisearch_tui/utils.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/widgets/index.py` & `meilisearch_tui-0.8.0/meilisearch_tui/widgets/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/widgets/index_sidebar.py` & `meilisearch_tui-0.8.0/meilisearch_tui/widgets/index_sidebar.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/widgets/input.py` & `meilisearch_tui-0.8.0/meilisearch_tui/widgets/input.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/meilisearch_tui/widgets/messages.py` & `meilisearch_tui-0.8.0/meilisearch_tui/widgets/messages.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.7.4/pyproject.toml` & `meilisearch_tui-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-tui"
-version = "0.7.4"
+version = "0.8.0"
 description = "A TUI for Managing and Searching with Meilisearch"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-tui"
 homepage = "https://github.com/sanders41/meilisearch-tui"
 documentation = "https://github.com/sanders41/meilisearch-tui"
@@ -17,30 +17,30 @@
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-meilisearch-python-async = "1.4.0"
-textual = "0.27.0"
+meilisearch-python-async = "1.4.1"
+textual = "0.28.1"
 uvloop = {version = "0.17.0", markers = "sys_platform != 'win32'"}
 aiocache = "0.12.1"
 
 [tool.poetry.group.dev.dependencies]
 aiohttp = "3.8.4"
 black = "23.3.0"
 click = "8.1.3"
 msgpack = "1.0.5"
-mypy = "1.3.0"
+mypy = "1.4.0"
 pre-commit = "3.3.3"
 pytest = "7.3.2"
 pytest-asyncio = "0.21.0"
 pytest-cov = "4.1.0"
-ruff = "0.0.272"
+ruff = "0.0.275"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 meilisearch = "meilisearch_tui.__main__:main"
```

### Comparing `meilisearch_tui-0.7.4/PKG-INFO` & `meilisearch_tui-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-tui
-Version: 0.7.4
+Version: 0.8.0
 Summary: A TUI for Managing and Searching with Meilisearch
 Home-page: https://github.com/sanders41/meilisearch-tui
 License: MIT
 Keywords: meilisearch,tui
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,16 +13,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocache (==0.12.1)
-Requires-Dist: meilisearch-python-async (==1.4.0)
-Requires-Dist: textual (==0.27.0)
+Requires-Dist: meilisearch-python-async (==1.4.1)
+Requires-Dist: textual (==0.28.1)
 Requires-Dist: uvloop (==0.17.0) ; sys_platform != "win32"
 Project-URL: Documentation, https://github.com/sanders41/meilisearch-tui
 Project-URL: Repository, https://github.com/sanders41/meilisearch-tui
 Description-Content-Type: text/markdown
 
 # Meilisearch TUI
```

