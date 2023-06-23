# Comparing `tmp/twscrape-0.2.2.tar.gz` & `tmp/twscrape-0.3.0.tar.gz`

## Comparing `twscrape-0.2.2.tar` & `twscrape-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.2.2/.gitattributes
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 twscrape-0.2.2/Dockerfile-test
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 twscrape-0.2.2/Makefile
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.2.2/.github/CODEOWNERS
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.2.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.2.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.2.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.2.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/test_api.py
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/test_parser.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/test_pool.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/test_queue_client.py
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/favoriters_raw.json
--rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/followers_raw.json
--rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/following_raw.json
--rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/retweeters_raw.json
--rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/search_raw.json
--rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/tweet_details_raw.json
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/user_by_id_raw.json
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/user_by_login_raw.json
--rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/user_tweets_and_replies_raw.json
--rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.2.2/tests/mocked-data/user_tweets_raw.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/__init__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/account.py
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/accounts_pool.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/api.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/cli.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/constants.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/db.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/imap.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/logger.py
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/login.py
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/models.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/queue_client.py
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 twscrape-0.2.2/twscrape/utils.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.2.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.2.2/LICENSE
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 twscrape-0.2.2/readme.md
--rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 twscrape-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.3.0/.gitattributes
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 twscrape-0.3.0/Dockerfile-test
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 twscrape-0.3.0/Makefile
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.3.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.3.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/test_api.py
+-rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/test_parser.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/test_pool.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/test_queue_client.py
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/favoriters_raw.json
+-rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/followers_raw.json
+-rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/following_raw.json
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/manual_tweet_with_video_1.json
+-rw-r--r--   0        0        0    84696 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/manual_tweet_with_video_2.json
+-rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/retweeters_raw.json
+-rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/search_raw.json
+-rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/tweet_details_raw.json
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/user_by_id_raw.json
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/user_by_login_raw.json
+-rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/user_tweets_and_replies_raw.json
+-rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.3.0/tests/mocked-data/user_tweets_raw.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/account.py
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/accounts_pool.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/api.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/cli.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/constants.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/db.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/imap.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/logger.py
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/login.py
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/models.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/queue_client.py
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 twscrape-0.3.0/twscrape/utils.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 twscrape-0.3.0/readme.md
+-rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 twscrape-0.3.0/PKG-INFO
```

### Comparing `twscrape-0.2.2/Dockerfile-test` & `twscrape-0.3.0/Dockerfile-test`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/Makefile` & `twscrape-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/.github/workflows/publish.yml` & `twscrape-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/conftest.py` & `twscrape-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/test_api.py` & `twscrape-0.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/test_parser.py` & `twscrape-0.3.0/tests/test_parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import json
 import os
 
 from twscrape import API, AccountsPool, gather
 from twscrape.logger import set_log_level
+from twscrape.models import Tweet, User
 
 BASE_DIR = os.path.dirname(__file__)
 DATA_DIR = os.path.join(BASE_DIR, "mocked-data")
 os.makedirs(DATA_DIR, exist_ok=True)
 
 set_log_level("DEBUG")
 
@@ -21,66 +22,111 @@
     following_raw = "following_raw.json"
     retweeters_raw = "retweeters_raw.json"
     favoriters_raw = "favoriters_raw.json"
     user_tweets_raw = "user_tweets_raw.json"
     user_tweets_and_replies_raw = "user_tweets_and_replies_raw.json"
 
 
-def fake_rep(fn: str):
-    filename = os.path.join(DATA_DIR, getattr(Files, fn))
+def fake_rep(fn: str, filename: str | None = None):
+    if filename is None:
+        filename = os.path.join(DATA_DIR, getattr(Files, fn))
 
     with open(filename) as fp:
         data = fp.read()
 
     rep = lambda: None  # noqa: E731
     rep.text = data
     rep.json = lambda: json.loads(data)
     return rep
 
 
-def mock_rep(obj, fn: str):
+def mock_rep(obj, fn: str, filename: str | None = None):
     async def cb_rep(*args, **kwargs):
-        return fake_rep(fn)
+        return fake_rep(fn, filename)
 
     setattr(obj, fn, cb_rep)
 
 
 def mock_gen(obj, fn: str):
     async def cb_gen(*args, **kwargs):
         yield fake_rep(fn)
 
     setattr(obj, fn, cb_gen)
 
 
+def check_tweet(doc: Tweet):
+    assert doc.id is not None
+    assert doc.id_str is not None
+    assert isinstance(doc.id, int)
+    assert isinstance(doc.id_str, str)
+    assert doc.id == int(doc.id_str)
+
+    assert doc.url is not None
+    assert doc.id_str in doc.url
+    assert doc.user is not None
+
+    obj = doc.dict()
+    assert doc.id == obj["id"]
+    assert doc.user.id == obj["user"]["id"]
+
+    assert "url" in obj
+    assert "_type" in obj
+    assert obj["_type"] == "snscrape.modules.twitter.Tweet"
+
+    assert "url" in obj["user"]
+    assert "_type" in obj["user"]
+    assert obj["user"]["_type"] == "snscrape.modules.twitter.User"
+
+    txt = doc.json()
+    assert isinstance(txt, str)
+    assert str(doc.id) in txt
+
+    if doc.media is not None:
+        if len(doc.media.photos) > 0:
+            assert doc.media.photos[0].url is not None
+
+        if len(doc.media.videos) > 0:
+            for x in doc.media.videos:
+                assert x.thumbnailUrl is not None
+                assert x.duration is not None
+                for v in x.variants:
+                    assert v.url is not None
+                    assert v.bitrate is not None
+                    assert v.contentType is not None
+
+    check_user(doc.user)
+
+
+def check_user(doc: User):
+    assert doc.id is not None
+    assert doc.id_str is not None
+    assert isinstance(doc.id, int)
+    assert isinstance(doc.id_str, str)
+    assert doc.id == int(doc.id_str)
+
+    assert doc.username is not None
+
+    obj = doc.dict()
+    assert doc.id == obj["id"]
+    assert doc.username == obj["username"]
+
+    txt = doc.json()
+    assert isinstance(txt, str)
+    assert str(doc.id) in txt
+
+
 async def test_search():
     api = API(AccountsPool())
     mock_gen(api, "search_raw")
 
     items = await gather(api.search("elon musk lang:en", limit=20))
     assert len(items) > 0
 
     for doc in items:
-        assert doc.id is not None
-        assert doc.user is not None
-
-        obj = doc.dict()
-        assert doc.id == obj["id"]
-        assert doc.user.id == obj["user"]["id"]
-
-        assert "url" in obj
-        assert "_type" in obj
-        assert obj["_type"] == "snscrape.modules.twitter.Tweet"
-
-        assert "url" in obj["user"]
-        assert "_type" in obj["user"]
-        assert obj["user"]["_type"] == "snscrape.modules.twitter.User"
-
-        txt = doc.json()
-        assert isinstance(txt, str)
-        assert str(doc.id) in txt
+        check_tweet(doc)
 
 
 async def test_user_by_id():
     api = API(AccountsPool())
     mock_rep(api, "user_by_id_raw")
 
     doc = await api.user_by_id(2244994945)
@@ -114,144 +160,97 @@
 
 
 async def test_tweet_details():
     api = API(AccountsPool())
     mock_rep(api, "tweet_details_raw")
 
     doc = await api.tweet_details(1649191520250245121)
+    check_tweet(doc)
     assert doc.id == 1649191520250245121
     assert doc.user is not None
 
-    obj = doc.dict()
-    assert doc.id == obj["id"]
-    assert doc.user.id == obj["user"]["id"]
-
-    txt = doc.json()
-    assert isinstance(txt, str)
-    assert str(doc.id) in txt
-
 
 async def test_followers():
     api = API(AccountsPool())
     mock_gen(api, "followers_raw")
 
     users = await gather(api.followers(2244994945))
     assert len(users) > 0
 
     for doc in users:
-        assert doc.id is not None
-        assert doc.username is not None
-
-        obj = doc.dict()
-        assert doc.id == obj["id"]
-        assert doc.username == obj["username"]
-
-        txt = doc.json()
-        assert isinstance(txt, str)
-        assert str(doc.id) in txt
+        check_user(doc)
 
 
 async def test_following():
     api = API(AccountsPool())
     mock_gen(api, "following_raw")
 
     users = await gather(api.following(2244994945))
     assert len(users) > 0
 
     for doc in users:
-        assert doc.id is not None
-        assert doc.username is not None
-
-        obj = doc.dict()
-        assert doc.id == obj["id"]
-        assert doc.username == obj["username"]
-
-        txt = doc.json()
-        assert isinstance(txt, str)
-        assert str(doc.id) in txt
+        check_user(doc)
 
 
 async def test_retweters():
     api = API(AccountsPool())
     mock_gen(api, "retweeters_raw")
 
     users = await gather(api.retweeters(1649191520250245121))
     assert len(users) > 0
 
     for doc in users:
-        assert doc.id is not None
-        assert doc.username is not None
-
-        obj = doc.dict()
-        assert doc.id == obj["id"]
-        assert doc.username == obj["username"]
-
-        txt = doc.json()
-        assert isinstance(txt, str)
-        assert str(doc.id) in txt
+        check_user(doc)
 
 
 async def test_favoriters():
     api = API(AccountsPool())
     mock_gen(api, "favoriters_raw")
 
     users = await gather(api.favoriters(1649191520250245121))
     assert len(users) > 0
 
     for doc in users:
-        assert doc.id is not None
-        assert doc.username is not None
-
-        obj = doc.dict()
-        assert doc.id == obj["id"]
-        assert doc.username == obj["username"]
-
-        txt = doc.json()
-        assert isinstance(txt, str)
-        assert str(doc.id) in txt
+        check_user(doc)
 
 
 async def test_user_tweets():
     api = API(AccountsPool())
     mock_gen(api, "user_tweets_raw")
 
     tweets = await gather(api.user_tweets(2244994945))
     assert len(tweets) > 0
 
     for doc in tweets:
-        assert doc.id is not None
-        assert doc.user is not None
-
-        obj = doc.dict()
-        assert doc.id == obj["id"]
-        assert doc.user.id == obj["user"]["id"]
-
-        txt = doc.json()
-        assert isinstance(txt, str)
-        assert str(doc.id) in txt
+        check_tweet(doc)
 
 
 async def test_user_tweets_and_replies():
     api = API(AccountsPool())
     mock_gen(api, "user_tweets_and_replies_raw")
 
     tweets = await gather(api.user_tweets_and_replies(2244994945))
     assert len(tweets) > 0
 
     for doc in tweets:
-        assert doc.id is not None
-        assert doc.user is not None
+        check_tweet(doc)
+
+
+async def test_tweet_with_video():
+    api = API(AccountsPool())
 
-        obj = doc.dict()
-        assert doc.id == obj["id"]
-        assert doc.user.id == obj["user"]["id"]
-
-        txt = doc.json()
-        assert isinstance(txt, str)
-        assert str(doc.id) in txt
+    files = [
+        ("manual_tweet_with_video_1.json", 1671508600538161153),
+        ("manual_tweet_with_video_2.json", 1671753569412820992),
+    ]
+
+    for file, twid in files:
+        mock_rep(api, "tweet_details_raw", os.path.join(DATA_DIR, file))
+        doc = await api.tweet_details(twid)
+        check_tweet(doc)
 
 
 async def main():
     # prepare mock files from real twitter replies
     # you need to have some account to perform this
     FRESH = False
```

### Comparing `twscrape-0.2.2/tests/test_pool.py` & `twscrape-0.3.0/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/test_queue_client.py` & `twscrape-0.3.0/tests/test_queue_client.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/mocked-data/favoriters_raw.json` & `twscrape-0.3.0/tests/mocked-data/favoriters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/mocked-data/followers_raw.json` & `twscrape-0.3.0/tests/mocked-data/followers_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/mocked-data/following_raw.json` & `twscrape-0.3.0/tests/mocked-data/following_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/mocked-data/retweeters_raw.json` & `twscrape-0.3.0/tests/mocked-data/retweeters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/mocked-data/search_raw.json` & `twscrape-0.3.0/tests/mocked-data/search_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/mocked-data/tweet_details_raw.json` & `twscrape-0.3.0/tests/mocked-data/tweet_details_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/mocked-data/user_by_id_raw.json` & `twscrape-0.3.0/tests/mocked-data/user_by_id_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/mocked-data/user_by_login_raw.json` & `twscrape-0.3.0/tests/mocked-data/user_by_login_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/mocked-data/user_tweets_and_replies_raw.json` & `twscrape-0.3.0/tests/mocked-data/user_tweets_and_replies_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/tests/mocked-data/user_tweets_raw.json` & `twscrape-0.3.0/tests/mocked-data/user_tweets_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/twscrape/account.py` & `twscrape-0.3.0/twscrape/account.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/twscrape/accounts_pool.py` & `twscrape-0.3.0/twscrape/accounts_pool.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/twscrape/api.py` & `twscrape-0.3.0/twscrape/api.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/twscrape/cli.py` & `twscrape-0.3.0/twscrape/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
 import io
+import json
 import sqlite3
 from importlib.metadata import version
 
 from .api import API, AccountsPool
 from .db import get_sqlite_version
 from .logger import logger, set_log_level
 from .utils import print_table
@@ -23,14 +24,20 @@
         if name in args:
             return name, getattr(args, name)
 
     logger.error(f"Missing argument: {names}")
     exit(1)
 
 
+def to_str(doc):
+    # doc is httpx.Response or twscrape.User / twscrape.Tweet
+    # both have .json method but with different return type
+    return doc if isinstance(doc, str) else json.dumps(doc.json(), default=str)
+
+
 async def main(args):
     if args.debug:
         set_log_level("DEBUG")
 
     if args.command == "version":
         print(f"twscrape: {version('twscrape')}")
         print(f"SQLite client: {sqlite3.version}")
@@ -63,18 +70,18 @@
         logger.error(f"Unknown command: {args.command}")
         exit(1)
 
     _, val = get_fn_arg(args)
 
     if "limit" in args:
         async for doc in fn(val, limit=args.limit):
-            print(doc.json())
+            print(to_str(doc))
     else:
         doc = await fn(val)
-        print(doc.json())
+        print(to_str(doc))
 
 
 def custom_help(p):
     buffer = io.StringIO()
     p.print_help(buffer)
     msg = buffer.getvalue()
```

### Comparing `twscrape-0.2.2/twscrape/constants.py` & `twscrape-0.3.0/twscrape/constants.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/twscrape/db.py` & `twscrape-0.3.0/twscrape/db.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/twscrape/imap.py` & `twscrape-0.3.0/twscrape/imap.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/twscrape/login.py` & `twscrape-0.3.0/twscrape/login.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/twscrape/models.py` & `twscrape-0.3.0/twscrape/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import email.utils
 import json
 import re
-from dataclasses import asdict, dataclass
+from dataclasses import asdict, dataclass, field
 from datetime import datetime
 from typing import Optional
 
+from .logger import logger
 from .utils import find_item, get_or, int_or_none
 
 
 @dataclass
 class JSONTrait:
     def dict(self):
         return asdict(self)
@@ -82,14 +83,15 @@
     def parse(obj: dict):
         return UserRef(id=int(obj["id_str"]), username=obj["screen_name"], displayname=obj["name"])
 
 
 @dataclass
 class User(JSONTrait):
     id: int
+    id_str: str
     url: str
     username: str
     displayname: str
     rawDescription: str
     created: datetime
     followersCount: int
     friendsCount: int
@@ -109,14 +111,15 @@
     # link: typing.Optional[TextLink] = None
     # label: typing.Optional["UserLabel"] = None
 
     @staticmethod
     def parse(obj: dict):
         return User(
             id=int(obj["id_str"]),
+            id_str=obj["id_str"],
             url=f'https://twitter.com/{obj["screen_name"]}',
             username=obj["screen_name"],
             displayname=obj["name"],
             rawDescription=obj["description"],
             created=email.utils.parsedate_to_datetime(obj["created_at"]),
             followersCount=obj["followers_count"],
             friendsCount=obj["friends_count"],
@@ -131,14 +134,15 @@
             protected=obj.get("protected"),
         )
 
 
 @dataclass
 class Tweet(JSONTrait):
     id: int
+    id_str: str
     url: str
     date: datetime
     user: User
     lang: str
     rawContent: str
     replyCount: int
     retweetCount: int
@@ -155,30 +159,31 @@
     place: Optional[Place] = None
     coordinates: Optional[Coordinates] = None
     inReplyToTweetId: int | None = None
     inReplyToUser: UserRef | None = None
     source: str | None = None
     sourceUrl: str | None = None
     sourceLabel: str | None = None
+    media: Optional["Media"] = None
     _type: str = "snscrape.modules.twitter.Tweet"
 
     # todo:
     # renderedContent: str
-    # media: typing.Optional[typing.List["Medium"]] = None
     # card: typing.Optional["Card"] = None
     # vibe: typing.Optional["Vibe"] = None
 
     @staticmethod
     def parse(obj: dict, res: dict):
         tw_usr = User.parse(res["users"][obj["user_id_str"]])
         rt_obj = get_or(res, f"tweets.{obj.get('retweeted_status_id_str')}")
         qt_obj = get_or(res, f"tweets.{obj.get('quoted_status_id_str')}")
 
         return Tweet(
             id=int(obj["id_str"]),
+            id_str=obj["id_str"],
             url=f'https://twitter.com/{tw_usr.username}/status/{obj["id_str"]}',
             date=email.utils.parsedate_to_datetime(obj["created_at"]),
             user=tw_usr,
             lang=obj["lang"],
             rawContent=obj["full_text"],
             replyCount=obj["reply_count"],
             retweetCount=obj["retweet_count"],
@@ -195,17 +200,112 @@
             place=Place.parse(obj["place"]) if obj.get("place") else None,
             coordinates=Coordinates.parse(obj),
             inReplyToTweetId=int_or_none(obj, "in_reply_to_status_id_str"),
             inReplyToUser=_get_reply_user(obj, res),
             source=obj.get("source", None),
             sourceUrl=_get_source_url(obj),
             sourceLabel=_get_source_label(obj),
+            media=Media.parse(obj),
         )
 
 
+@dataclass
+class MediaPhoto(JSONTrait):
+    url: str
+
+    @staticmethod
+    def parse(obj: dict):
+        return MediaPhoto(
+            url=obj["media_url_https"],
+        )
+
+
+@dataclass
+class MediaVideo(JSONTrait):
+    thumbnailUrl: str
+    variants: list["MediaVideoVariant"]
+    duration: int
+    views: int | None = None
+
+    @staticmethod
+    def parse(obj: dict):
+        return MediaVideo(
+            thumbnailUrl=obj["media_url_https"],
+            variants=[
+                MediaVideoVariant.parse(x) for x in obj["video_info"]["variants"] if "bitrate" in x
+            ],
+            duration=obj["video_info"]["duration_millis"],
+            views=int_or_none(obj, "mediaStats.viewCount"),
+        )
+
+
+@dataclass
+class MediaAnimated(JSONTrait):
+    thumbnailUrl: str
+    videoUrl: str
+
+    @staticmethod
+    def parse(obj: dict):
+        try:
+            return MediaAnimated(
+                thumbnailUrl=obj["media_url_https"],
+                videoUrl=obj["video_info"]["variants"][0]["url"],
+            )
+        except KeyError:
+            return None
+
+
+@dataclass
+class MediaVideoVariant(JSONTrait):
+    contentType: str
+    bitrate: int
+    url: str
+
+    @staticmethod
+    def parse(obj: dict):
+        return MediaVideoVariant(
+            contentType=obj["content_type"],
+            bitrate=obj["bitrate"],
+            url=obj["url"],
+        )
+
+
+@dataclass
+class Media(JSONTrait):
+    photos: list[MediaPhoto] = field(default_factory=list)
+    videos: list[MediaVideo] = field(default_factory=list)
+    animated: list[MediaAnimated] = field(default_factory=list)
+
+    @staticmethod
+    def parse(obj: dict):
+        photos: list[MediaPhoto] = []
+        videos: list[MediaVideo] = []
+        animated: list[MediaAnimated] = []
+
+        for x in get_or(obj, "extended_entities.media", []):
+            if x["type"] == "video":
+                if video := MediaVideo.parse(x):
+                    videos.append(video)
+                continue
+
+            if x["type"] == "photo":
+                if photo := MediaPhoto.parse(x):
+                    photos.append(photo)
+                continue
+
+            if x["type"] == "animated_gif":
+                if animated_gif := MediaAnimated.parse(x):
+                    animated.append(animated_gif)
+                continue
+
+            logger.warning(f"Unknown media type: {x['type']}: {json.dumps(x)}")
+
+        return Media(photos=photos, videos=videos, animated=animated)
+
+
 def _get_reply_user(tw_obj: dict, res: dict):
     user_id = tw_obj.get("in_reply_to_user_id_str", None)
     if user_id is None:
         return None
 
     if user_id in res["users"]:
         return UserRef.parse(res["users"][user_id])
```

### Comparing `twscrape-0.2.2/twscrape/queue_client.py` & `twscrape-0.3.0/twscrape/queue_client.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/twscrape/utils.py` & `twscrape-0.3.0/twscrape/utils.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/.gitignore` & `twscrape-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/LICENSE` & `twscrape-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/pyproject.toml` & `twscrape-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "twscrape"
-version = "0.2.2"
+version = "0.3.0"
 authors = [{name = "vladkens", email = "v.pronsky@gmail.com"}]
 description = "Twitter GraphQL and Search API implementation with SNScrape data models"
 readme = "readme.md"
 requires-python = ">=3.10"
 keywords = ["twitter", "scrape", "scrapper", "api", "snscrape"]
 license = {text = "MIT"}
 classifiers = [
```

### Comparing `twscrape-0.2.2/readme.md` & `twscrape-0.3.0/readme.md`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.2/PKG-INFO` & `twscrape-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twscrape
-Version: 0.2.2
+Version: 0.3.0
 Summary: Twitter GraphQL and Search API implementation with SNScrape data models
 Project-URL: repository, https://github.com/vladkens/twscrape
 Author-email: vladkens <v.pronsky@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: api,scrape,scrapper,snscrape,twitter
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twscrape Version: 0.2.2 Summary: Twitter GraphQL
+Metadata-Version: 2.1 Name: twscrape Version: 0.3.0 Summary: Twitter GraphQL
 and Search API implementation with SNScrape data models Project-URL:
 repository, https://github.com/vladkens/twscrape Author-email: vladkens
 pronsky@gmail.com> License: MIT License-File: LICENSE Keywords:
 api,scrape,scrapper,snscrape,twitter Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10 Requires-Dist: aiosqlite==0.17.0 Requires-Dist: fake-
```

