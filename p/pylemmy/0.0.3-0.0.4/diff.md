# Comparing `tmp/pylemmy-0.0.3.tar.gz` & `tmp/pylemmy-0.0.4.tar.gz`

## Comparing `pylemmy-0.0.3.tar` & `pylemmy-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pylemmy-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.github/workflows/integration.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.github/workflows/lint.yaml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/index.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/api/lemmy.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/api/utils.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/api/models/comment.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/api/models/community.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/api/models/post.md
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pylemmy-0.0.3/examples/lmgtfy.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/__about__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/__init__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/endpoints.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/lemmy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/py.typed
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/auth.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/comment.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/community.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/listing.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/person.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/post.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/site.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/utils.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/models/__init__.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/models/comment.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/models/community.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/models/post.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/integration/__init__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/integration/docker-compose.yml
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/integration/lemmy.hjson
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/integration/test_api.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/integration/test_lemmy.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pylemmy-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 pylemmy-0.0.3/README.md
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pylemmy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pylemmy-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.github/workflows/integration.yml
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.github/workflows/run.yaml
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/index.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/api/lemmy.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/api/utils.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/api/models/comment.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/api/models/community.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/api/models/post.md
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pylemmy-0.0.4/examples/lmgtfy.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/__about__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/endpoints.py
+-rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/lemmy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/py.typed
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/auth.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/comment.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/community.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/listing.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/person.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/post.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/site.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/utils.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/models/__init__.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/models/comment.py
+-rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/models/community.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/models/post.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/integration/docker-compose.yml
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/integration/lemmy.hjson
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/integration/test_api.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/integration/test_lemmy.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/unit/test_utils.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pylemmy-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 pylemmy-0.0.4/README.md
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pylemmy-0.0.4/PKG-INFO
```

### Comparing `pylemmy-0.0.3/mkdocs.yml` & `pylemmy-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/.github/workflows/docs.yaml` & `pylemmy-0.0.4/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/.github/workflows/publish.yaml` & `pylemmy-0.0.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/examples/lmgtfy.py` & `pylemmy-0.0.4/examples/lmgtfy.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/pylemmy/endpoints.py` & `pylemmy-0.0.4/pylemmy/endpoints.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/pylemmy/lemmy.py` & `pylemmy-0.0.4/pylemmy/lemmy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Implements the Lemmy class."""
 import urllib.parse
-from typing import List, Optional, Union
+from typing import Iterable, List, Optional, Union
 
 import requests
 from pydantic import AnyUrl, parse_obj_as
 
 from pylemmy import api
 from pylemmy.api.utils import BaseApiModel
 from pylemmy.endpoints import LemmyAPI
-from pylemmy.models.community import Community
+from pylemmy.models.community import Community, MultiCommunityStream
 from pylemmy.models.post import Post
 
 
 class Lemmy:
     """The Lemmy class provides the main entrypoint for pylemmy, and Lemmy's API.
 
     This class manages all the settings relating how to access your chosen
@@ -249,7 +249,33 @@
         """
         response = self.session.put(
             self._get_url(path),
             params=params.dict() if params is not None else {},
             timeout=self.request_timeout,
         )
         return response.json()
+
+    def multi_communities_stream(
+        self, communities: Iterable[Union[int, str, Community]]
+    ) -> MultiCommunityStream:
+        """Get streams for multiple communities.
+
+        Example:
+        A simple example where we want to print the content of each post/comment.
+
+            def process_content(elem: Union[Post, Comment]):
+                if isinstance(Post, elem):
+                    print(elem.post_view.post.name)
+                elif isinstance(Comment, elem):
+                    print(elem.comment_view.comment.content
+
+            multi_stream = lemmy.multi_communities_stream(["community1", "community2"])
+            multi_stream.content_apply(process_content)
+
+        :param communities: An iterable of community ids, names or instances of
+        [Community][pylemmy.community.Community].
+        """
+        communities_list = (
+            x if isinstance(x, Community) else self.get_community(x)
+            for x in communities
+        )
+        return MultiCommunityStream(list(communities_list))
```

### Comparing `pylemmy-0.0.3/pylemmy/api/comment.py` & `pylemmy-0.0.4/pylemmy/api/comment.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/pylemmy/api/community.py` & `pylemmy-0.0.4/pylemmy/api/community.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/pylemmy/api/post.py` & `pylemmy-0.0.4/pylemmy/api/post.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/pylemmy/models/comment.py` & `pylemmy-0.0.4/pylemmy/models/comment.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/pylemmy/models/post.py` & `pylemmy-0.0.4/pylemmy/models/post.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/tests/integration/docker-compose.yml` & `pylemmy-0.0.4/tests/integration/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/tests/integration/lemmy.hjson` & `pylemmy-0.0.4/tests/integration/lemmy.hjson`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/tests/integration/test_api.py` & `pylemmy-0.0.4/tests/integration/test_api.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/tests/integration/test_lemmy.py` & `pylemmy-0.0.4/tests/integration/test_lemmy.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/.gitignore` & `pylemmy-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/LICENSE.txt` & `pylemmy-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/README.md` & `pylemmy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.3/pyproject.toml` & `pylemmy-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "pydantic>=1.7",
     "requests>=2.18",
     "loguru>=0.3",
+    "aiostream~=0.4.5",
 ]
 
 [project.urls]
 Documentation = "https://dcferreira.com/pylemmy"
 Issues = "https://github.com/dcferreira/pylemmy/issues"
 Source = "https://github.com/dcferreira/pylemmy"
 
@@ -56,14 +57,15 @@
 ]
 cov = [
     "test-cov",
     "cov-report",
 ]
 typing = ["mypy {args:.}"]
 integration = "pytest tests/integration"
+unit = "pytest tests/unit"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
@@ -179,8 +181,14 @@
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
 ]
 
 [tool.pytest.ini_options]
 addopts = """
 --docker-compose=tests/integration/docker-compose.yml \
---docker-compose-remove-volumes"""
+--docker-compose-remove-volumes"""
+
+[[tool.mypy.overrides]]
+module = [
+    "aiostream",
+]
+ignore_missing_imports = true
```

### Comparing `pylemmy-0.0.3/PKG-INFO` & `pylemmy-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylemmy
-Version: 0.0.3
+Version: 0.0.4
 Summary: pylemmy enables simple access to Lemmy's API with Python
 Project-URL: Documentation, https://dcferreira.com/pylemmy
 Project-URL: Issues, https://github.com/dcferreira/pylemmy/issues
 Project-URL: Source, https://github.com/dcferreira/pylemmy
 Author-email: Daniel Ferreira <daniel.ferreira.1@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: aiostream~=0.4.5
 Requires-Dist: loguru>=0.3
 Requires-Dist: pydantic>=1.7
 Requires-Dist: requests>=2.18
 Description-Content-Type: text/markdown
 
 # pylemmy
```

