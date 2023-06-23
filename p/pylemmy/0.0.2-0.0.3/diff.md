# Comparing `tmp/pylemmy-0.0.2.tar.gz` & `tmp/pylemmy-0.0.3.tar.gz`

## Comparing `pylemmy-0.0.2.tar` & `pylemmy-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pylemmy-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.github/workflows/integration.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.github/workflows/lint.yaml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/index.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/api/lemmy.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/api/utils.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/api/models/comment.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/api/models/community.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylemmy-0.0.2/docs/api/models/post.md
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pylemmy-0.0.2/examples/lmgtfy.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/__about__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/__init__.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/endpoints.py
--rw-r--r--   0        0        0     7579 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/lemmy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/py.typed
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/auth.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/comment.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/community.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/listing.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/person.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/post.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/site.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/api/utils.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/models/__init__.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/models/comment.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/models/community.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pylemmy/models/post.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/integration/__init__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/integration/docker-compose.yml
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/integration/lemmy.hjson
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/integration/test_api.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 pylemmy-0.0.2/tests/integration/test_lemmy.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pylemmy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pylemmy-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 pylemmy-0.0.2/README.md
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 pylemmy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pylemmy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pylemmy-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.github/workflows/integration.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/index.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/api/lemmy.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/api/utils.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/api/models/comment.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/api/models/community.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylemmy-0.0.3/docs/api/models/post.md
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pylemmy-0.0.3/examples/lmgtfy.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/__about__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/endpoints.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/lemmy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/py.typed
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/auth.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/comment.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/community.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/listing.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/person.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/post.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/site.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/api/utils.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/models/__init__.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/models/comment.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/models/community.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pylemmy/models/post.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/integration/docker-compose.yml
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/integration/lemmy.hjson
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/integration/test_api.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 pylemmy-0.0.3/tests/integration/test_lemmy.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pylemmy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pylemmy-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 pylemmy-0.0.3/README.md
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 pylemmy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pylemmy-0.0.3/PKG-INFO
```

### Comparing `pylemmy-0.0.2/mkdocs.yml` & `pylemmy-0.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/.github/workflows/docs.yaml` & `pylemmy-0.0.3/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/.github/workflows/publish.yaml` & `pylemmy-0.0.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/docs/index.md` & `pylemmy-0.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/examples/lmgtfy.py` & `pylemmy-0.0.3/examples/lmgtfy.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/pylemmy/lemmy.py` & `pylemmy-0.0.3/pylemmy/lemmy.py`

 * *Files 12% similar despite different names*

```diff
@@ -175,14 +175,38 @@
             raise ValueError(msg)
 
         result = self.get_request(LemmyAPI.Post, params=payload)
         parsed_result = api.post.GetPostResponse(**result)
 
         return Post(self, parsed_result.post_view)
 
+    def list_post_reports(self, **kwargs) -> List[api.post.PostReportView]:
+        """List post reports.
+
+        :param kwargs: See optional arguments in [ListPostReports](
+        https://join-lemmy.org/api/interfaces/ListPostReports.html).
+        """
+        payload = api.post.ListPostReports(auth=self.get_token(), **kwargs)
+        result = self.get_request(LemmyAPI.ListPostReports, params=payload)
+        parsed_result = api.post.ListPostReportsResponse(**result)
+
+        return parsed_result.post_reports
+
+    def list_comment_reports(self, **kwargs) -> List[api.comment.CommentReportView]:
+        """List comment reports.
+
+        :param kwargs: See optional arguments in [ListCommentReports](
+        https://join-lemmy.org/api/interfaces/ListCommentReports.html).
+        """
+        payload = api.comment.ListCommentReports(auth=self.get_token(), **kwargs)
+        result = self.get_request(LemmyAPI.ListPostReports, params=payload)
+        parsed_result = api.comment.ListCommentReportsResponse(**result)
+
+        return parsed_result.comment_reports
+
     def post_request(
         self,
         path: LemmyAPI,
         params: Optional[BaseApiModel] = None,
     ):
         """Send a POST request to the desired path.
 
@@ -208,7 +232,24 @@
         """
         response = self.session.get(
             self._get_url(path),
             params=params.dict() if params is not None else {},
             timeout=self.request_timeout,
         )
         return response.json()
+
+    def put_request(
+        self,
+        path: LemmyAPI,
+        params: Optional[BaseApiModel] = None,
+    ):
+        """Send a PUT request to the desired path.
+
+        :param path: A Lemmy endpoint.
+        :param params: Parameters to send with the request (in the URL).
+        """
+        response = self.session.put(
+            self._get_url(path),
+            params=params.dict() if params is not None else {},
+            timeout=self.request_timeout,
+        )
+        return response.json()
```

### Comparing `pylemmy-0.0.2/pylemmy/utils.py` & `pylemmy-0.0.3/pylemmy/utils.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/pylemmy/api/comment.py` & `pylemmy-0.0.3/pylemmy/api/comment.py`

 * *Files 17% similar despite different names*

```diff
@@ -82,7 +82,64 @@
     saved_only: Optional[int]
     sort: Optional[CommentSortType]
     type_: Optional[ListingType]
 
 
 class GetCommentsResponse(BaseApiModel):
     comments: List[CommentView]
+
+
+class CommentReport(BaseApiModel):
+    comment_id: int
+    creator_id: int
+    id: int
+    original_comment_text: str
+    published: str
+    reason: str
+    resolved: bool
+    resolver_id: Optional[int]
+    updated: Optional[str]
+
+
+class CommentReportView(BaseApiModel):
+    comment: Comment
+    comment_creator: Person
+    comment_report: CommentReport
+    community: Community
+    counts: CommentAggregates
+    creator: Person
+    creator_banned_from_community: bool
+    my_vote: Optional[int]
+    post: Post
+    resolver: Person
+
+
+class CreateCommentReport(BaseApiModel):
+    auth: str
+    comment_id: int
+    reason: str
+
+
+class CommentReportResponse(BaseApiModel):
+    comment_report_view: CommentReportView
+
+
+class ResolveCommentReport(BaseApiModel):
+    auth: str
+    report_id: int
+    resolved: bool
+
+
+class CommentResolveResponse(BaseApiModel):
+    comment_report_view: CommentReportView
+
+
+class ListCommentReports(BaseApiModel):
+    auth: str
+    community_id: Optional[int]
+    limit: Optional[int]
+    page: Optional[int]
+    unresolved_only: Optional[bool]
+
+
+class ListCommentReportsResponse(BaseApiModel):
+    comment_reports: List[CommentReportView]
```

### Comparing `pylemmy-0.0.2/pylemmy/api/community.py` & `pylemmy-0.0.3/pylemmy/api/community.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/pylemmy/api/post.py` & `pylemmy-0.0.3/pylemmy/api/post.py`

 * *Files 20% similar despite different names*

```diff
@@ -99,7 +99,65 @@
     saved_only: Optional[bool]
     sort: Optional[SortType]
     type_: Optional[ListingType]
 
 
 class GetPostsResponse(BaseApiModel):
     posts: List[PostView]
+
+
+class PostReport(BaseApiModel):
+    id: int
+    creator_id: int
+    post_id: int
+    original_post_name: str
+    original_post_url: Optional[str]
+    original_post_body: Optional[str]
+    reason: str
+    resolved: bool
+    resolved_id: Optional[int]
+    published: str
+    updated: Optional[str]
+
+
+class PostReportView(BaseApiModel):
+    post_report: PostReport
+    post: Post
+    community: int
+    creator: Person
+    post_creator: Person
+    creator_banned_from_community: bool
+    my_vote: Optional[int]
+    counts: PostAggregates
+    resolve: Optional[Person]
+
+
+class CreatePostReport(BaseApiModel):
+    auth: str
+    post_id: int
+    reason: str
+
+
+class PostReportResponse(BaseApiModel):
+    post_report_view: PostReportView
+
+
+class ResolvePostReport(BaseApiModel):
+    auth: str
+    report_id: int
+    resolved: bool
+
+
+class PostResolveResponse(BaseApiModel):
+    post_report_view: PostReportView
+
+
+class ListPostReports(BaseApiModel):
+    auth: str
+    page: int
+    limit: int
+    unresolved_only: Optional[bool]
+    community_id: Optional[int]
+
+
+class ListPostReportsResponse(BaseApiModel):
+    post_reports: List[PostReportView]
```

### Comparing `pylemmy-0.0.2/pylemmy/models/community.py` & `pylemmy-0.0.3/pylemmy/models/community.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,14 +70,30 @@
             auth=self.lemmy.get_token_optional(), community_id=self.safe.id, **kwargs
         )
         result = self.lemmy.get_request(LemmyAPI.GetComments, params=payload)
         parsed_result = api.comment.GetCommentsResponse(**result)
 
         return [Comment(self.lemmy, comment) for comment in parsed_result.comments]
 
+    def list_post_reports(self, **kwargs) -> List[api.post.PostReportView]:
+        """List post reports in this community.
+
+        :param kwargs: See optional arguments in [ListPostReports](
+        https://join-lemmy.org/api/interfaces/ListPostReports.html).
+        """
+        return self.lemmy.list_post_reports(community_id=self.safe.id, **kwargs)
+
+    def list_comment_reports(self, **kwargs) -> List[api.comment.CommentReportView]:
+        """List comment reports in this community.
+
+        :param kwargs: See optional arguments in [ListCommentReports](
+        https://join-lemmy.org/api/interfaces/ListCommentReports.html).
+        """
+        return self.lemmy.list_comment_reports(community_id=self.safe.id, **kwargs)
+
     @property
     def stream(self) -> "CommunityStream":
         """Returns a stream of content.
 
         This stream is to be used to monitor posts or comments.
 
         Example:
```

### Comparing `pylemmy-0.0.2/tests/integration/docker-compose.yml` & `pylemmy-0.0.3/tests/integration/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/tests/integration/lemmy.hjson` & `pylemmy-0.0.3/tests/integration/lemmy.hjson`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/tests/integration/test_api.py` & `pylemmy-0.0.3/tests/integration/test_api.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/tests/integration/test_lemmy.py` & `pylemmy-0.0.3/tests/integration/test_lemmy.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/.gitignore` & `pylemmy-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/LICENSE.txt` & `pylemmy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/README.md` & `pylemmy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/pyproject.toml` & `pylemmy-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.2/PKG-INFO` & `pylemmy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylemmy
-Version: 0.0.2
+Version: 0.0.3
 Summary: pylemmy enables simple access to Lemmy's API with Python
 Project-URL: Documentation, https://dcferreira.com/pylemmy
 Project-URL: Issues, https://github.com/dcferreira/pylemmy/issues
 Project-URL: Source, https://github.com/dcferreira/pylemmy
 Author-email: Daniel Ferreira <daniel.ferreira.1@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

